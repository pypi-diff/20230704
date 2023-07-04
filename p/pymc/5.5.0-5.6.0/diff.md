# Comparing `tmp/pymc-5.5.0.tar.gz` & `tmp/pymc-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.5.0.tar", last modified: Fri Jun  9 14:56:28 2023, max compression
+gzip compressed data, was "dist/pymc-5.6.0.tar", last modified: Tue Jul  4 12:11:14 2023, max compression
```

## Comparing `pymc-5.5.0.tar` & `pymc-5.6.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 14:56:17.000000 pymc-5.5.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-09 14:56:17.000000 pymc-5.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-09 14:56:17.000000 pymc-5.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-06-09 14:56:17.000000 pymc-5.5.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-06-09 14:56:17.000000 pymc-5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 14:56:17.000000 pymc-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-09 14:56:28.000000 pymc-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-09 14:56:17.000000 pymc-5.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-06-09 14:56:17.000000 pymc-5.5.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16569 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    40140 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36243 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89110 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    33914 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    90171 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39241 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 14:56:17.000000 pymc-5.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 14:56:17.000000 pymc-5.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-09 14:56:17.000000 pymc-5.5.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-06-09 14:56:17.000000 pymc-5.5.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 14:56:28.000000 pymc-5.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-06-09 14:56:17.000000 pymc-5.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-06-09 14:56:17.000000 pymc-5.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-04 12:11:04.000000 pymc-5.6.0/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-04 12:11:04.000000 pymc-5.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 12:11:04.000000 pymc-5.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-04 12:11:04.000000 pymc-5.6.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-04 12:11:04.000000 pymc-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 12:11:04.000000 pymc-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-04 12:11:14.000000 pymc-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-04 12:11:04.000000 pymc-5.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-04 12:11:04.000000 pymc-5.6.0/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46063 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89229 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85069 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39443 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 12:11:04.000000 pymc-5.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 12:11:04.000000 pymc-5.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-04 12:11:04.000000 pymc-5.6.0/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-04 12:11:04.000000 pymc-5.6.0/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 12:11:14.000000 pymc-5.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-07-04 12:11:04.000000 pymc-5.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-04 12:11:04.000000 pymc-5.6.0/versioneer.py
```

### Comparing `pymc-5.5.0/ARCHITECTURE.md` & `pymc-5.6.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/CODE_OF_CONDUCT.md` & `pymc-5.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/CONTRIBUTING.md` & `pymc-5.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/GOVERNANCE.md` & `pymc-5.6.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/LICENSE` & `pymc-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/PKG-INFO` & `pymc-5.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.5.0
+Version: 5.6.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -157,14 +157,16 @@
         
         |NumFOCUS|
         
         |PyMCLabs|
         
         |Mistplay|
         
+        |ODSC|
+        
         .. |Binder| image:: https://mybinder.org/badge_logo.svg
            :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
         .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
            :target: https://github.com/pymc-devs/pymc/actions
         .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
            :target: https://codecov.io/gh/pymc-devs/pymc
         .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
@@ -173,14 +175,16 @@
            :target: http://www.numfocus.org/
         .. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
            :target: http://www.numfocus.org/
         .. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
            :target: https://pymc-labs.io
         .. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
            :target: https://www.mistplay.com/
+        .. |ODSC| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/odsc/sponsor_odsc.png?raw=true
+           :target: https://odsc.com/california/?utm_source=pymc&utm_medium=referral
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pymc-5.5.0/README.rst` & `pymc-5.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,16 @@
 
 |NumFOCUS|
 
 |PyMCLabs|
 
 |Mistplay|
 
+|ODSC|
+
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
 .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
    :target: https://github.com/pymc-devs/pymc/actions
 .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pymc-devs/pymc
 .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
@@ -165,7 +167,9 @@
    :target: http://www.numfocus.org/
 .. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
    :target: http://www.numfocus.org/
 .. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
    :target: https://pymc-labs.io
 .. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
    :target: https://www.mistplay.com/
+.. |ODSC| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/odsc/sponsor_odsc.png?raw=true
+   :target: https://odsc.com/california/?utm_source=pymc&utm_medium=referral
```

### Comparing `pymc-5.5.0/RELEASE-NOTES.md` & `pymc-5.6.0/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/__init__.py` & `pymc-5.6.0/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/backends/__init__.py` & `pymc-5.6.0/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/backends/arviz.py` & `pymc-5.6.0/pymc/backends/arviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,22 +394,32 @@
     @requires("model")
     def constant_data_to_xarray(self):
         """Convert constant data to xarray."""
         constant_data = find_constants(self.model)
         if not constant_data:
             return None
 
-        return dict_to_dataset(
+        xarray_dataset = dict_to_dataset(
             constant_data,
             library=pymc,
             coords=self.coords,
             dims=self.dims,
             default_dims=[],
         )
 
+        # provisional handling of scalars in constant
+        # data to prevent promotion to rank 1
+        # in the future this will be handled by arviz
+        scalars = [var_name for var_name, value in constant_data.items() if np.ndim(value) == 0]
+        for s in scalars:
+            s_dim_0_name = f"{s}_dim_0"
+            xarray_dataset = xarray_dataset.squeeze(s_dim_0_name, drop=True)
+
+        return xarray_dataset
+
     def to_inference_data(self):
         """Convert all available data to an InferenceData object.
 
         Note that if groups can not be created (e.g., there is no `trace`, so
         the `posterior` and `sample_stats` can not be extracted), then the InferenceData
         will not have those groups.
         """
```

### Comparing `pymc-5.5.0/pymc/backends/base.py` & `pymc-5.6.0/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/backends/mcbackend.py` & `pymc-5.6.0/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/backends/ndarray.py` & `pymc-5.6.0/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/backends/report.py` & `pymc-5.6.0/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/blocking.py` & `pymc-5.6.0/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/data.py` & `pymc-5.6.0/pymc/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,19 @@
             "Add variable inside a 'with model:' block."
         )
     name = model.name_for(name)
 
     # `convert_observed_data` takes care of parameter `value` and
     # transforms it to something digestible for PyTensor.
     arr = convert_observed_data(value)
+    if isinstance(arr, np.ma.MaskedArray):
+        raise NotImplementedError(
+            "Masked arrays or arrays with `nan` entries are not supported. "
+            "Pass them directly to `observed` if you want to trigger auto-imputation"
+        )
 
     if mutable is None:
         warnings.warn(
             "The `mutable` kwarg was not specified. Before v4.1.0 it defaulted to `pm.Data(mutable=True)`,"
             " which is equivalent to using `pm.MutableData()`."
             " In v4.1.0 the default changed to `pm.Data(mutable=False)`, equivalent to `pm.ConstantData`."
             " Use `pm.ConstantData`/`pm.MutableData` or pass `pm.Data(..., mutable=False/True)` to avoid this warning.",
```

### Comparing `pymc-5.5.0/pymc/distributions/__init__.py` & `pymc-5.6.0/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/bound.py` & `pymc-5.6.0/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/censored.py` & `pymc-5.6.0/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/continuous.py` & `pymc-5.6.0/pymc/distributions/continuous.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-# Contains code from Aeppl, Copyright (c) 2021-2022, PyTensor Developers.
+# Contains code from AePPL, Copyright (c) 2021-2022, Aesara Developers.
 
 # coding: utf-8
 """
 A collection of common probability distributions for stochastic
 nodes in PyMC.
 """
 
@@ -53,14 +53,15 @@
     uniform,
     vonmises,
 )
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.var import TensorConstant
 
 from pymc.logprob.abstract import _logcdf_helper, _logprob_helper
+from pymc.logprob.basic import icdf
 
 try:
     from polyagamma import polyagamma_cdf, polyagamma_pdf, random_polyagamma
 except ImportError:  # pragma: no cover
 
     def random_polyagamma(*args, **kwargs):
         raise RuntimeError("polyagamma package is not installed!")
@@ -852,14 +853,19 @@
 
         return check_parameters(
             logcdf,
             sigma > 0,
             msg="sigma > 0",
         )
 
+    def icdf(value, loc, sigma):
+        res = icdf(Normal.dist(loc, sigma), (value + 1.0) / 2.0)
+        res = check_icdf_value(res, value)
+        return res
+
 
 class WaldRV(RandomVariable):
     name = "wald"
     ndim_supp = 0
     ndims_params = [0, 0, 0]
     dtype = "floatX"
     _print_name = ("Wald", "\\operatorname{Wald}")
@@ -1717,14 +1723,18 @@
 
         return check_parameters(
             res,
             sigma > 0,
             msg="sigma > 0",
         )
 
+    def icdf(value, mu, sigma):
+        res = pt.exp(icdf(Normal.dist(mu, sigma), value))
+        return res
+
 
 Lognormal = LogNormal
 
 
 class StudentTRV(RandomVariable):
     name = "studentt"
     ndim_supp = 0
@@ -2035,14 +2045,23 @@
         res = pt.log(0.5 + pt.arctan((value - alpha) / beta) / np.pi)
         return check_parameters(
             res,
             beta > 0,
             msg="beta > 0",
         )
 
+    def icdf(value, alpha, beta):
+        res = alpha + beta * pt.tan(np.pi * (value - 0.5))
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            beta > 0,
+            msg="beta > 0",
+        )
+
 
 class HalfCauchy(PositiveContinuous):
     r"""
     Half-Cauchy log-likelihood.
 
     The pdf of this distribution is
 
@@ -2109,14 +2128,23 @@
 
         return check_parameters(
             res,
             beta > 0,
             msg="beta > 0",
         )
 
+    def icdf(value, loc, beta):
+        res = loc + beta * pt.tan(np.pi * (value) / 2.0)
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            beta > 0,
+            msg="beta > 0",
+        )
+
 
 class Gamma(PositiveContinuous):
     r"""
     Gamma log-likelihood.
 
     Represents the sum of alpha exponentially distributed random variables,
     each of which has rate beta.
@@ -2514,14 +2542,24 @@
         return check_parameters(
             res,
             alpha > 0,
             beta > 0,
             msg="alpha > 0, beta > 0",
         )
 
+    def icdf(value, alpha, beta):
+        res = beta * (-pt.log(1 - value)) ** (1 / alpha)
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            alpha > 0,
+            beta > 0,
+            msg="alpha > 0, beta > 0",
+        )
+
 
 class HalfStudentTRV(RandomVariable):
     name = "halfstudentt"
     ndim_supp = 0
     ndims_params = [0, 0]
     dtype = "floatX"
     _print_name = ("HalfStudentT", "\\operatorname{HalfStudentT}")
@@ -3057,14 +3095,28 @@
         return check_parameters(
             res,
             lower <= c,
             c <= upper,
             msg="lower <= c <= upper",
         )
 
+    def icdf(value, lower, c, upper):
+        res = pt.switch(
+            pt.lt(value, ((c - lower) / (upper - lower))),
+            lower + np.sqrt((upper - lower) * (c - lower) * value),
+            upper - np.sqrt((upper - lower) * (upper - c) * (1 - value)),
+        )
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            lower <= c,
+            c <= upper,
+            msg="lower <= c <= upper",
+        )
+
 
 @_default_transform.register(Triangular)
 def triangular_default_transform(op, rv):
     return bounded_cont_transform(op, rv, Triangular.bound_args_indices)
 
 
 class Gumbel(Continuous):
@@ -3145,14 +3197,23 @@
 
         return check_parameters(
             res,
             beta > 0,
             msg="beta > 0",
         )
 
+    def icdf(value, mu, beta):
+        res = mu - beta * pt.log(-pt.log(value))
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            beta > 0,
+            msg="beta > 0",
+        )
+
 
 class RiceRV(RandomVariable):
     name = "rice"
     ndim_supp = 0
     ndims_params = [0, 0]
     dtype = "floatX"
     _print_name = ("Rice", "\\operatorname{Rice}")
@@ -3353,14 +3414,23 @@
 
         return check_parameters(
             res,
             s > 0,
             msg="s > 0",
         )
 
+    def icdf(value, mu, s):
+        res = mu + s * pt.log(value / (1 - value))
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            s > 0,
+            msg="s > 0",
+        )
+
 
 class LogitNormalRV(RandomVariable):
     name = "logit_normal"
     ndim_supp = 0
     ndims_params = [0, 0]
     dtype = "floatX"
     _print_name = ("logitNormal", "\\operatorname{logitNormal}")
@@ -3692,14 +3762,23 @@
         res = pt.log(pt.erfc(pt.exp(-scaled / 2) * (2**-0.5)))
         return check_parameters(
             res,
             sigma > 0,
             msg="sigma > 0",
         )
 
+    def icdf(value, mu, sigma):
+        res = sigma * -pt.log(2.0 * pt.erfcinv(value) ** 2) + mu
+        res = check_icdf_value(res, value)
+        return check_parameters(
+            res,
+            sigma > 0,
+            msg="sigma > 0",
+        )
+
 
 class PolyaGammaRV(RandomVariable):
     """Polya-Gamma random variable."""
 
     name = "polyagamma"
     ndim_supp = 0
     ndims_params = [0, 0]
@@ -3793,29 +3872,30 @@
 
     .. plot::
         :context: close-figs
 
         import matplotlib.pyplot as plt
         import numpy as np
         from polyagamma import polyagamma_pdf
-        plt.style.use('seaborn-darkgrid')
+        import arviz as az
+        plt.style.use('arviz-darkgrid')
         x = np.linspace(0.01, 5, 500);x.sort()
         hs = [1., 5., 10., 15.]
         zs = [0.] * 4
         for h, z in zip(hs, zs):
             pdf = polyagamma_pdf(x, h=h, z=z)
             plt.plot(x, pdf, label=r'$h$ = {}, $z$ = {}'.format(h, z))
         plt.xlabel('x', fontsize=12)
         plt.ylabel('f(x)', fontsize=12)
         plt.legend(loc=1)
         plt.show()
 
     ========  =============================
     Support   :math:`x \in (0, \infty)`
-    Mean      :math:`dfrac{h}{4} if :math:`z=0`, :math:`\dfrac{tanh(z/2)h}{2z}` otherwise.
+    Mean      :math:`\dfrac{h}{4}` if :math:`z=0`, :math:`\dfrac{tanh(z/2)h}{2z}` otherwise.
     Variance  :math:`0.041666688h` if :math:`z=0`, :math:`\dfrac{h(sinh(z) - z)(1 - tanh^2(z/2))}{4z^3}` otherwise.
     ========  =============================
 
     Parameters
     ----------
     h : tensor_like of float, default 1
         The shape parameter of the distribution (h > 0).
```

### Comparing `pymc-5.5.0/pymc/distributions/discrete.py` & `pymc-5.6.0/pymc/distributions/discrete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1351,15 +1351,15 @@
     sigma : tensor_like of float, default 1.0
          Standard deviation of the probit function.
     compute_p : boolean, default True
         Whether to compute and store in the trace the inferred probabilities of each categories,
         based on the cutpoints' values. Defaults to True.
         Might be useful to disable it if memory usage is of interest.
 
-    Example
+    Examples
     --------
     .. code:: python
 
         # Generate data for a simple 1 dimensional example problem
         n1_c = 300; n2_c = 300; n3_c = 300
         cluster1 = np.random.randn(n1_c) + -1
         cluster2 = np.random.randn(n2_c) + 0
```

### Comparing `pymc-5.5.0/pymc/distributions/dist_math.py` & `pymc-5.6.0/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/distribution.py` & `pymc-5.6.0/pymc/distributions/distribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 from functools import singledispatch
 from typing import Callable, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from pytensor import tensor as pt
 from pytensor.compile.builders import OpFromGraph
-from pytensor.graph import node_rewriter
+from pytensor.graph import FunctionGraph, node_rewriter
 from pytensor.graph.basic import Node, Variable
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import in2out
 from pytensor.graph.utils import MetaType
 from pytensor.tensor.basic import as_tensor_variable
 from pytensor.tensor.random.op import RandomVariable
+from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
 from pytensor.tensor.random.utils import normalize_size_param
 from pytensor.tensor.var import TensorVariable
 from typing_extensions import TypeAlias
 
 from pymc.distributions.shape_utils import (
     Dims,
     Shape,
@@ -45,14 +46,15 @@
     convert_size,
     find_size,
     rv_size_is_none,
     shape_from_dims,
 )
 from pymc.exceptions import BlockModelAccessError
 from pymc.logprob.abstract import MeasurableVariable, _icdf, _logcdf, _logprob
+from pymc.logprob.basic import logp
 from pymc.logprob.rewriting import logprob_rewrites_db
 from pymc.model import BlockModelAccess
 from pymc.printing import str_for_dist
 from pymc.pytensorf import collect_default_updates, convert_observed_data, floatX
 from pymc.util import UNSET, _add_future_warning_tag
 from pymc.vartypes import continuous_types, string_types
 
@@ -192,14 +194,15 @@
     If `False`, a logprob function must be dispatched directly to the subclass type.
     """
 
     _print_name: Tuple[str, str] = ("Unknown", "\\operatorname{Unknown}")
     """Tuple of (name, latex name) used for for pretty-printing variables of this type"""
 
     def __init__(self, *args, ndim_supp, **kwargs):
+        """Initialitze a SymbolicRandomVariable class."""
         self.ndim_supp = ndim_supp
         kwargs.setdefault("inline", True)
         super().__init__(*args, **kwargs)
 
     def update(self, node: Node):
         """Symbolic update expression for input random state variables
 
@@ -596,15 +599,15 @@
         *dist_params,
         dist: Callable,
         logp: Optional[Callable] = None,
         logcdf: Optional[Callable] = None,
         moment: Optional[Callable] = None,
         ndim_supp: int = 0,
         dtype: str = "floatX",
-        class_name: str = "CustomSymbolicDist",
+        class_name: str = "CustomDist",
         **kwargs,
     ):
         dist_params = [as_tensor_variable(param) for param in dist_params]
 
         if logcdf is None:
             logcdf = default_not_implemented(class_name, "logcdf")
 
@@ -947,15 +950,15 @@
                 " Previous versions allowed passing distribution parameters as"
                 " a dictionary in ``observed``, in the current version these "
                 "parameters are positional arguments."
             )
         dist_params = cls.parse_dist_params(dist_params)
         cls.check_valid_dist_random(dist, random, dist_params)
         if dist is not None:
-            kwargs.setdefault("class_name", f"CustomSymbolicDist_{name}")
+            kwargs.setdefault("class_name", f"CustomDist_{name}")
             return _CustomSymbolicDist(
                 name,
                 *dist_params,
                 dist=dist,
                 logp=logp,
                 logcdf=logcdf,
                 moment=moment,
@@ -1143,7 +1146,149 @@
 
     def logcdf(value, c):
         return pt.switch(
             pt.lt(value, c),
             -np.inf,
             0,
         )
+
+
+class PartialObservedRV(SymbolicRandomVariable):
+    """RandomVariable with partially observed subspace, as indicated by a boolean mask.
+
+    See `create_partial_observed_rv` for more details.
+    """
+
+
+def create_partial_observed_rv(
+    rv: TensorVariable,
+    mask: Union[np.ndarray, TensorVariable],
+) -> Tuple[
+    Tuple[TensorVariable, TensorVariable], Tuple[TensorVariable, TensorVariable], TensorVariable
+]:
+    """Separate observed and unobserved components of a RandomVariable.
+
+    This function may return two independent RandomVariables or, if not possible,
+    two variables from a common `PartialObservedRV` node
+
+    Parameters
+    ----------
+    rv : TensorVariable
+    mask : tensor_like
+        Constant or variable boolean mask. True entries correspond to components of the variable that are not observed.
+
+    Returns
+    -------
+    observed_rv and mask : Tuple of TensorVariable
+        The observed component of the RV and respective indexing mask
+    unobserved_rv and mask : Tuple of TensorVariable
+        The unobserved component of the RV and respective indexing mask
+    joined_rv : TensorVariable
+        The symbolic join of the observed and unobserved components.
+    """
+    if not mask.dtype == "bool":
+        raise ValueError(
+            f"mask must be an array or tensor of boolean dtype, got dtype: {mask.dtype}"
+        )
+
+    if mask.ndim > rv.ndim:
+        raise ValueError(f"mask can't have more dims than rv, got ndim: {mask.ndim}")
+
+    antimask = ~mask
+
+    can_rewrite = False
+    # Only pure RVs can be rewritten
+    if isinstance(rv.owner.op, RandomVariable):
+        ndim_supp = rv.owner.op.ndim_supp
+
+        # All univariate RVs can be rewritten
+        if ndim_supp == 0:
+            can_rewrite = True
+
+        # Multivariate RVs can be rewritten if masking does not split within support dimensions
+        else:
+            batch_dims = rv.type.ndim - ndim_supp
+            constant_mask = getattr(as_tensor_variable(mask), "data", None)
+
+            # Indexing does not overlap with core dimensions
+            if mask.ndim <= batch_dims:
+                can_rewrite = True
+
+            # Try to handle special case where mask is constant across support dimensions,
+            # TODO: This could be done by the rewrite itself
+            elif constant_mask is not None:
+                # We check if a constant_mask that only keeps the first entry of each support dim
+                # is equivalent to the original one after re-expanding.
+                trimmed_mask = constant_mask[(...,) + (0,) * ndim_supp]
+                expanded_mask = np.broadcast_to(
+                    np.expand_dims(trimmed_mask, axis=tuple(range(-ndim_supp, 0))),
+                    shape=constant_mask.shape,
+                )
+                if np.array_equal(constant_mask, expanded_mask):
+                    mask = trimmed_mask
+                    antimask = ~trimmed_mask
+                    can_rewrite = True
+
+    if can_rewrite:
+        # Rewrite doesn't work with boolean masks. Should be fixed after https://github.com/pymc-devs/pytensor/pull/329
+        mask, antimask = mask.nonzero(), antimask.nonzero()
+
+        masked_rv = rv[mask]
+        fgraph = FunctionGraph(outputs=[masked_rv], clone=False)
+        [unobserved_rv] = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
+
+        antimasked_rv = rv[antimask]
+        fgraph = FunctionGraph(outputs=[antimasked_rv], clone=False)
+        [observed_rv] = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
+
+        # Make a clone of the observedRV, with a distinct rng so that observed and
+        # unobserved are never treated as equivalent (and mergeable) nodes by pytensor.
+        _, size, _, *inps = observed_rv.owner.inputs
+        observed_rv = observed_rv.owner.op(*inps, size=size)
+
+    # For all other cases use the more general PartialObservedRV
+    else:
+        # The symbolic graph simply splits the observed and unobserved components,
+        # so they can be given separate values.
+        dist_, mask_ = rv.type(), as_tensor_variable(mask).type()
+        observed_rv_, unobserved_rv_ = dist_[~mask_], dist_[mask_]
+
+        observed_rv, unobserved_rv = PartialObservedRV(
+            inputs=[dist_, mask_],
+            outputs=[observed_rv_, unobserved_rv_],
+            ndim_supp=rv.owner.op.ndim_supp,
+        )(rv, mask)
+
+    joined_rv = pt.empty(rv.shape, dtype=rv.type.dtype)
+    joined_rv = pt.set_subtensor(joined_rv[mask], unobserved_rv)
+    joined_rv = pt.set_subtensor(joined_rv[antimask], observed_rv)
+
+    return (observed_rv, antimask), (unobserved_rv, mask), joined_rv
+
+
+@_logprob.register(PartialObservedRV)
+def partial_observed_rv_logprob(op, values, dist, mask, **kwargs):
+    # For the logp, simply join the values
+    [obs_value, unobs_value] = values
+    antimask = ~mask
+    joined_value = pt.empty_like(dist)
+    joined_value = pt.set_subtensor(joined_value[mask], unobs_value)
+    joined_value = pt.set_subtensor(joined_value[antimask], obs_value)
+    joined_logp = logp(dist, joined_value)
+
+    # If we have a univariate RV we can split apart the logp terms
+    if op.ndim_supp == 0:
+        return joined_logp[antimask], joined_logp[mask]
+    # Otherwise, we can't (always/ easily) split apart logp terms.
+    # We return the full logp for the observed value, and a 0-nd array for the unobserved value
+    else:
+        return joined_logp.ravel(), pt.zeros((0,), dtype=joined_logp.type.dtype)
+
+
+@_moment.register(PartialObservedRV)
+def partial_observed_rv_moment(op, partial_obs_rv, rv, mask):
+    # Unobserved output
+    if partial_obs_rv.owner.outputs.index(partial_obs_rv) == 1:
+        return moment(rv)[mask]
+    # Observed output
+    else:
+        return moment(rv)[~mask]
```

### Comparing `pymc-5.5.0/pymc/distributions/mixture.py` & `pymc-5.6.0/pymc/distributions/mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,19 +609,21 @@
             pmf[1:] =  psi * pmf[1:]
             pmf /= pmf.sum()
             plt.plot(x, pmf, '-o', label='$\\psi$ = {}, $\\mu$ = {}'.format(psi, mu))
         plt.xlabel('x', fontsize=12)
         plt.ylabel('f(x)', fontsize=12)
         plt.legend(loc=1)
         plt.show()
+
     ========  ==========================
     Support   :math:`x \in \mathbb{N}_0`
     Mean      :math:`\psi\mu`
     Variance  :math:`\mu + \frac{1-\psi}{\psi}\mu^2`
     ========  ==========================
+
     Parameters
     ----------
     psi : tensor_like of float
         Expected proportion of Poisson variates (0 < psi < 1)
     mu : tensor_like of float
         Expected number of occurrences during the given interval
         (mu >= 0).
@@ -670,19 +672,21 @@
             pmf[1:] =  psi * pmf[1:]
             pmf /= pmf.sum()
             plt.plot(x, pmf, '-o', label='n = {}, p = {}, $\\psi$ = {}'.format(n, p, psi))
         plt.xlabel('x', fontsize=12)
         plt.ylabel('f(x)', fontsize=12)
         plt.legend(loc=1)
         plt.show()
+
     ========  ==========================
     Support   :math:`x \in \mathbb{N}_0`
     Mean      :math:`\psi n p`
     Variance  :math:`(1-\psi) n p [1 - p(1 - \psi n)].`
     ========  ==========================
+
     Parameters
     ----------
     psi : tensor_like of float
         Expected proportion of Binomial variates (0 < psi < 1)
     n : tensor_like of int
         Number of Bernoulli trials (n >= 0).
     p : tensor_like of float
@@ -746,14 +750,15 @@
         for a, m, psi in zip(alphas, mus, psis):
             pmf = ZeroInfNegBinom(a, m, psi, x)
             plt.plot(x, pmf, '-o', label=r'$\alpha$ = {}, $\mu$ = {}, $\psi$ = {}'.format(a, m, psi))
         plt.xlabel('x', fontsize=12)
         plt.ylabel('f(x)', fontsize=12)
         plt.legend(loc=1)
         plt.show()
+
     ========  ==========================
     Support   :math:`x \in \mathbb{N}_0`
     Mean      :math:`\psi\mu`
     Var       :math:`\psi\mu +  \left (1 + \frac{\mu}{\alpha} + \frac{1-\psi}{\mu} \right)`
     ========  ==========================
 
     The zero inflated negative binomial distribution can be parametrized
```

### Comparing `pymc-5.5.0/pymc/distributions/multivariate.py` & `pymc-5.6.0/pymc/distributions/multivariate.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,5317 +254,5324 @@
 00000fd0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
 00000fe0: 6162 6c65 2863 686f 6c29 0a20 2020 2020  able(chol).     
 00000ff0: 2020 2069 6620 6368 6f6c 2e6e 6469 6d20     if chol.ndim 
 00001000: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
 00001010: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
 00001020: 6f72 2822 6368 6f6c 206d 7573 7420 6265  or("chol must be
 00001030: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
-00001040: 2e22 290a 2020 2020 2020 2020 636f 7620  .").        cov 
-00001050: 3d20 6368 6f6c 2e64 6f74 2863 686f 6c2e  = chol.dot(chol.
-00001060: 5429 0a0a 2020 2020 7265 7475 726e 2063  T)..    return c
-00001070: 6f76 0a0a 0a64 6566 2071 7561 6464 6973  ov...def quaddis
-00001080: 745f 7061 7273 6528 7661 6c75 652c 206d  t_parse(value, m
-00001090: 752c 2063 6f76 2c20 6d61 745f 7479 7065  u, cov, mat_type
-000010a0: 3d22 636f 7622 293a 0a20 2020 2022 2222  ="cov"):.    """
-000010b0: 436f 6d70 7574 6520 2878 202d 206d 7529  Compute (x - mu)
-000010c0: 2e54 2040 2053 6967 6d61 5e2d 3120 4020  .T @ Sigma^-1 @ 
-000010d0: 2878 202d 206d 7529 2061 6e64 2074 6865  (x - mu) and the
-000010e0: 206c 6f67 6465 7420 6f66 2053 6967 6d61   logdet of Sigma
-000010f0: 2e22 2222 0a20 2020 2069 6620 7661 6c75  .""".    if valu
-00001100: 652e 6e64 696d 203e 2032 206f 7220 7661  e.ndim > 2 or va
-00001110: 6c75 652e 6e64 696d 203d 3d20 303a 0a20  lue.ndim == 0:. 
-00001120: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00001130: 7565 4572 726f 7228 2249 6e76 616c 6964  ueError("Invalid
-00001140: 2064 696d 656e 7369 6f6e 2066 6f72 2076   dimension for v
-00001150: 616c 7565 3a20 2573 2220 2520 7661 6c75  alue: %s" % valu
-00001160: 652e 6e64 696d 290a 2020 2020 6966 2076  e.ndim).    if v
-00001170: 616c 7565 2e6e 6469 6d20 3d3d 2031 3a0a  alue.ndim == 1:.
-00001180: 2020 2020 2020 2020 6f6e 6564 696d 203d          onedim =
-00001190: 2054 7275 650a 2020 2020 2020 2020 7661   True.        va
-000011a0: 6c75 6520 3d20 7661 6c75 655b 4e6f 6e65  lue = value[None
-000011b0: 2c20 3a5d 0a20 2020 2065 6c73 653a 0a20  , :].    else:. 
-000011c0: 2020 2020 2020 206f 6e65 6469 6d20 3d20         onedim = 
-000011d0: 4661 6c73 650a 0a20 2020 2064 656c 7461  False..    delta
-000011e0: 203d 2076 616c 7565 202d 206d 750a 2020   = value - mu.  
-000011f0: 2020 2320 5573 6520 7468 6973 2077 6865    # Use this whe
-00001200: 6e20 5468 6561 6e6f 2335 3930 3820 6973  n Theano#5908 is
-00001210: 2072 656c 6561 7365 642e 0a20 2020 2023   released..    #
-00001220: 2072 6574 7572 6e20 4d76 4e6f 726d 616c   return MvNormal
-00001230: 4c6f 6770 2829 2873 656c 662e 636f 762c  Logp()(self.cov,
-00001240: 2064 656c 7461 290a 2020 2020 6368 6f6c   delta).    chol
-00001250: 5f63 6f76 203d 2063 686f 6c65 736b 7928  _cov = cholesky(
-00001260: 636f 7629 0a20 2020 2069 6620 6d61 745f  cov).    if mat_
-00001270: 7479 7065 2021 3d20 2274 6175 223a 0a20  type != "tau":. 
-00001280: 2020 2020 2020 2064 6973 742c 206c 6f67         dist, log
-00001290: 6465 742c 206f 6b20 3d20 7175 6164 6469  det, ok = quaddi
-000012a0: 7374 5f63 686f 6c28 6465 6c74 612c 2063  st_chol(delta, c
-000012b0: 686f 6c5f 636f 7629 0a20 2020 2065 6c73  hol_cov).    els
-000012c0: 653a 0a20 2020 2020 2020 2064 6973 742c  e:.        dist,
-000012d0: 206c 6f67 6465 742c 206f 6b20 3d20 7175   logdet, ok = qu
-000012e0: 6164 6469 7374 5f74 6175 2864 656c 7461  addist_tau(delta
-000012f0: 2c20 6368 6f6c 5f63 6f76 290a 2020 2020  , chol_cov).    
-00001300: 6966 206f 6e65 6469 6d3a 0a20 2020 2020  if onedim:.     
-00001310: 2020 2072 6574 7572 6e20 6469 7374 5b30     return dist[0
-00001320: 5d2c 206c 6f67 6465 742c 206f 6b0a 0a20  ], logdet, ok.. 
-00001330: 2020 2072 6574 7572 6e20 6469 7374 2c20     return dist, 
-00001340: 6c6f 6764 6574 2c20 6f6b 0a0a 0a64 6566  logdet, ok...def
-00001350: 2071 7561 6464 6973 745f 6368 6f6c 2864   quaddist_chol(d
-00001360: 656c 7461 2c20 6368 6f6c 5f6d 6174 293a  elta, chol_mat):
-00001370: 0a20 2020 2064 6961 6720 3d20 7074 2e64  .    diag = pt.d
-00001380: 6961 6728 6368 6f6c 5f6d 6174 290a 2020  iag(chol_mat).  
-00001390: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
-000013a0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-000013b0: 6978 2069 7320 706f 7369 7469 7665 2064  ix is positive d
-000013c0: 6566 696e 6974 652e 0a20 2020 206f 6b20  efinite..    ok 
-000013d0: 3d20 7074 2e61 6c6c 2864 6961 6720 3e20  = pt.all(diag > 
-000013e0: 3029 0a20 2020 2023 2049 6620 6e6f 742c  0).    # If not,
-000013f0: 2072 6570 6c61 6365 2074 6865 2064 6961   replace the dia
-00001400: 676f 6e61 6c2e 2057 6520 7265 7475 726e  gonal. We return
-00001410: 202d 696e 6620 6c61 7465 722c 2062 7574   -inf later, but
-00001420: 0a20 2020 2023 206e 6565 6420 746f 2070  .    # need to p
-00001430: 7265 7665 6e74 2073 6f6c 7665 5f6c 6f77  revent solve_low
-00001440: 6572 2066 726f 6d20 7468 726f 7769 6e67  er from throwing
-00001450: 2061 6e20 6578 6365 7074 696f 6e2e 0a20   an exception.. 
-00001460: 2020 2063 686f 6c5f 636f 7620 3d20 7074     chol_cov = pt
-00001470: 2e73 7769 7463 6828 6f6b 2c20 6368 6f6c  .switch(ok, chol
-00001480: 5f6d 6174 2c20 3129 0a0a 2020 2020 6465  _mat, 1)..    de
-00001490: 6c74 615f 7472 616e 7320 3d20 736f 6c76  lta_trans = solv
-000014a0: 655f 6c6f 7765 7228 6368 6f6c 5f63 6f76  e_lower(chol_cov
-000014b0: 2c20 6465 6c74 612e 5429 2e54 0a20 2020  , delta.T).T.   
-000014c0: 2071 7561 6464 6973 7420 3d20 2864 656c   quaddist = (del
-000014d0: 7461 5f74 7261 6e73 2a2a 3229 2e73 756d  ta_trans**2).sum
-000014e0: 2861 7869 733d 2d31 290a 2020 2020 6c6f  (axis=-1).    lo
-000014f0: 6764 6574 203d 2070 742e 7375 6d28 7074  gdet = pt.sum(pt
-00001500: 2e6c 6f67 2864 6961 6729 290a 2020 2020  .log(diag)).    
-00001510: 7265 7475 726e 2071 7561 6464 6973 742c  return quaddist,
-00001520: 206c 6f67 6465 742c 206f 6b0a 0a0a 6465   logdet, ok...de
-00001530: 6620 7175 6164 6469 7374 5f74 6175 2864  f quaddist_tau(d
-00001540: 656c 7461 2c20 6368 6f6c 5f6d 6174 293a  elta, chol_mat):
-00001550: 0a20 2020 2064 6961 6720 3d20 7074 2e6e  .    diag = pt.n
-00001560: 6c69 6e61 6c67 2e64 6961 6728 6368 6f6c  linalg.diag(chol
-00001570: 5f6d 6174 290a 2020 2020 2320 4368 6563  _mat).    # Chec
-00001580: 6b20 6966 2074 6865 2070 7265 6369 7369  k if the precisi
-00001590: 6f6e 206d 6174 7269 7820 6973 2070 6f73  on matrix is pos
-000015a0: 6974 6976 6520 6465 6669 6e69 7465 2e0a  itive definite..
-000015b0: 2020 2020 6f6b 203d 2070 742e 616c 6c28      ok = pt.all(
-000015c0: 6469 6167 203e 2030 290a 2020 2020 2320  diag > 0).    # 
-000015d0: 4966 206e 6f74 2c20 7265 706c 6163 6520  If not, replace 
-000015e0: 7468 6520 6469 6167 6f6e 616c 2e20 5765  the diagonal. We
-000015f0: 2072 6574 7572 6e20 2d69 6e66 206c 6174   return -inf lat
-00001600: 6572 2c20 6275 740a 2020 2020 2320 6e65  er, but.    # ne
-00001610: 6564 2074 6f20 7072 6576 656e 7420 736f  ed to prevent so
-00001620: 6c76 655f 6c6f 7765 7220 6672 6f6d 2074  lve_lower from t
-00001630: 6872 6f77 696e 6720 616e 2065 7863 6570  hrowing an excep
-00001640: 7469 6f6e 2e0a 2020 2020 6368 6f6c 5f74  tion..    chol_t
-00001650: 6175 203d 2070 742e 7377 6974 6368 286f  au = pt.switch(o
-00001660: 6b2c 2063 686f 6c5f 6d61 742c 2031 290a  k, chol_mat, 1).
-00001670: 0a20 2020 2064 656c 7461 5f74 7261 6e73  .    delta_trans
-00001680: 203d 2070 742e 646f 7428 6465 6c74 612c   = pt.dot(delta,
-00001690: 2063 686f 6c5f 7461 7529 0a20 2020 2071   chol_tau).    q
-000016a0: 7561 6464 6973 7420 3d20 2864 656c 7461  uaddist = (delta
-000016b0: 5f74 7261 6e73 2a2a 3229 2e73 756d 2861  _trans**2).sum(a
-000016c0: 7869 733d 2d31 290a 2020 2020 6c6f 6764  xis=-1).    logd
-000016d0: 6574 203d 202d 7074 2e73 756d 2870 742e  et = -pt.sum(pt.
-000016e0: 6c6f 6728 6469 6167 2929 0a20 2020 2072  log(diag)).    r
-000016f0: 6574 7572 6e20 7175 6164 6469 7374 2c20  eturn quaddist, 
-00001700: 6c6f 6764 6574 2c20 6f6b 0a0a 0a63 6c61  logdet, ok...cla
-00001710: 7373 204d 764e 6f72 6d61 6c28 436f 6e74  ss MvNormal(Cont
-00001720: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
-00001730: 220a 2020 2020 4d75 6c74 6976 6172 6961  ".    Multivaria
-00001740: 7465 206e 6f72 6d61 6c20 6c6f 672d 6c69  te normal log-li
-00001750: 6b65 6c69 686f 6f64 2e0a 0a20 2020 202e  kelihood...    .
-00001760: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
-00001770: 2066 2878 205c 6d69 6420 5c70 692c 2054   f(x \mid \pi, T
-00001780: 2920 3d0a 2020 2020 2020 2020 2020 205c  ) =.           \
-00001790: 6672 6163 7b7c 547c 5e7b 312f 327d 7d7b  frac{|T|^{1/2}}{
-000017a0: 2832 5c70 6929 5e7b 6b2f 327d 7d0a 2020  (2\pi)^{k/2}}.  
-000017b0: 2020 2020 2020 2020 205c 6578 705c 6c65           \exp\le
-000017c0: 6674 5c7b 202d 5c66 7261 637b 317d 7b32  ft\{ -\frac{1}{2
-000017d0: 7d20 2878 2d5c 6d75 295e 7b5c 7072 696d  } (x-\mu)^{\prim
-000017e0: 657d 2054 2028 782d 5c6d 7529 205c 7269  e} T (x-\mu) \ri
-000017f0: 6768 745c 7d0a 0a20 2020 203d 3d3d 3d3d  ght\}..    =====
-00001800: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
-00001810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00001820: 2020 2020 5375 7070 6f72 7420 2020 3a6d      Support   :m
-00001830: 6174 683a 6078 205c 696e 205c 6d61 7468  ath:`x \in \math
-00001840: 6262 7b52 7d5e 6b60 0a20 2020 204d 6561  bb{R}^k`.    Mea
-00001850: 6e20 2020 2020 203a 6d61 7468 3a60 5c6d  n      :math:`\m
-00001860: 7560 0a20 2020 2056 6172 6961 6e63 6520  u`.    Variance 
-00001870: 203a 6d61 7468 3a60 545e 7b2d 317d 600a   :math:`T^{-1}`.
-00001880: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
-00001890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000018a0: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 5061  ========..    Pa
-000018b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-000018c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75 203a  -------.    mu :
-000018d0: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-000018e0: 666c 6f61 740a 2020 2020 2020 2020 5665  float.        Ve
-000018f0: 6374 6f72 206f 6620 6d65 616e 732e 0a20  ctor of means.. 
-00001900: 2020 2063 6f76 203a 2074 656e 736f 725f     cov : tensor_
-00001910: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-00001920: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00001930: 436f 7661 7269 616e 6365 206d 6174 7269  Covariance matri
-00001940: 782e 2045 7861 6374 6c79 206f 6e65 206f  x. Exactly one o
-00001950: 6620 636f 762c 2074 6175 2c20 6f72 2063  f cov, tau, or c
-00001960: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
-00001970: 2020 2074 6175 203a 2074 656e 736f 725f     tau : tensor_
-00001980: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-00001990: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-000019a0: 5072 6563 6973 696f 6e20 6d61 7472 6978  Precision matrix
-000019b0: 2e20 4578 6163 746c 7920 6f6e 6520 6f66  . Exactly one of
-000019c0: 2063 6f76 2c20 7461 752c 206f 7220 6368   cov, tau, or ch
-000019d0: 6f6c 2069 7320 6e65 6564 6564 2e0a 2020  ol is needed..  
-000019e0: 2020 6368 6f6c 203a 2074 656e 736f 725f    chol : tensor_
-000019f0: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-00001a00: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00001a10: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
-00001a20: 7369 7469 6f6e 206f 6620 636f 7661 7269  sition of covari
-00001a30: 616e 6365 206d 6174 7269 782e 2045 7861  ance matrix. Exa
-00001a40: 6374 6c79 206f 6e65 206f 6620 636f 762c  ctly one of cov,
-00001a50: 0a20 2020 2020 2020 2074 6175 2c20 6f72  .        tau, or
-00001a60: 2063 686f 6c20 6973 206e 6565 6465 642e   chol is needed.
-00001a70: 0a20 2020 206c 6f77 6572 3a20 626f 6f6c  .    lower: bool
-00001a80: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
-00001a90: 2020 2020 2020 2057 6865 7468 6572 2063         Whether c
-00001aa0: 686f 6c20 6973 2074 6865 206c 6f77 6572  hol is the lower
-00001ab0: 2074 7269 6469 6167 6f6e 616c 2063 686f   tridiagonal cho
-00001ac0: 6c65 736b 7920 6661 6374 6f72 2e0a 0a20  lesky factor... 
-00001ad0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00001ae0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
-00001af0: 696e 6520 6120 6d75 6c74 6976 6172 6961  ine a multivaria
-00001b00: 7465 206e 6f72 6d61 6c20 7661 7269 6162  te normal variab
-00001b10: 6c65 2066 6f72 2061 2067 6976 656e 2063  le for a given c
-00001b20: 6f76 6172 6961 6e63 650a 2020 2020 6d61  ovariance.    ma
-00001b30: 7472 6978 3a3a 0a0a 2020 2020 2020 2020  trix::..        
-00001b40: 636f 7620 3d20 6e70 2e61 7272 6179 285b  cov = np.array([
-00001b50: 5b31 2e2c 2030 2e35 5d2c 205b 302e 352c  [1., 0.5], [0.5,
-00001b60: 2032 5d5d 290a 2020 2020 2020 2020 6d75   2]]).        mu
-00001b70: 203d 206e 702e 7a65 726f 7328 3229 0a20   = np.zeros(2). 
-00001b80: 2020 2020 2020 2076 616c 7320 3d20 706d         vals = pm
-00001b90: 2e4d 764e 6f72 6d61 6c28 2776 616c 7327  .MvNormal('vals'
-00001ba0: 2c20 6d75 3d6d 752c 2063 6f76 3d63 6f76  , mu=mu, cov=cov
-00001bb0: 2c20 7368 6170 653d 2835 2c20 3229 290a  , shape=(5, 2)).
-00001bc0: 0a20 2020 204d 6f73 7420 6f66 2074 6865  .    Most of the
-00001bd0: 2074 696d 6520 6974 2069 7320 7072 6566   time it is pref
-00001be0: 6572 6162 6c65 2074 6f20 7370 6563 6966  erable to specif
-00001bf0: 7920 7468 6520 6368 6f6c 6573 6b79 0a20  y the cholesky. 
-00001c00: 2020 2066 6163 746f 7220 6f66 2074 6865     factor of the
-00001c10: 2063 6f76 6172 6961 6e63 6520 696e 7374   covariance inst
-00001c20: 6561 642e 2046 6f72 2065 7861 6d70 6c65  ead. For example
-00001c30: 2c20 7765 2063 6f75 6c64 0a20 2020 2066  , we could.    f
-00001c40: 6974 2061 206d 756c 7469 7661 7269 6174  it a multivariat
-00001c50: 6520 6f75 7463 6f6d 6520 6c69 6b65 2074  e outcome like t
-00001c60: 6869 7320 2873 6565 2074 6865 2064 6f63  his (see the doc
-00001c70: 7374 7269 6e67 0a20 2020 206f 6620 604c  string.    of `L
-00001c80: 4b4a 4368 6f6c 6573 6b79 436f 7660 2066  KJCholeskyCov` f
-00001c90: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00001ca0: 696f 6e20 6162 6f75 7420 7468 6973 293a  ion about this):
-00001cb0: 3a0a 0a20 2020 2020 2020 206d 7520 3d20  :..        mu = 
-00001cc0: 6e70 2e7a 6572 6f73 2833 290a 2020 2020  np.zeros(3).    
-00001cd0: 2020 2020 7472 7565 5f63 6f76 203d 206e      true_cov = n
-00001ce0: 702e 6172 7261 7928 5b5b 312e 302c 2030  p.array([[1.0, 0
-00001cf0: 2e35 2c20 302e 315d 2c0a 2020 2020 2020  .5, 0.1],.      
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2020 205b 302e 352c 2032 2e30         [0.5, 2.0
-00001d20: 2c20 302e 325d 2c0a 2020 2020 2020 2020  , 0.2],.        
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 205b 302e 312c 2030 2e32 2c20       [0.1, 0.2, 
-00001d50: 312e 305d 5d29 0a20 2020 2020 2020 2064  1.0]]).        d
-00001d60: 6174 6120 3d20 6e70 2e72 616e 646f 6d2e  ata = np.random.
-00001d70: 6d75 6c74 6976 6172 6961 7465 5f6e 6f72  multivariate_nor
-00001d80: 6d61 6c28 6d75 2c20 7472 7565 5f63 6f76  mal(mu, true_cov
-00001d90: 2c20 3130 290a 0a20 2020 2020 2020 2073  , 10)..        s
-00001da0: 645f 6469 7374 203d 2070 6d2e 4578 706f  d_dist = pm.Expo
-00001db0: 6e65 6e74 6961 6c2e 6469 7374 2831 2e30  nential.dist(1.0
-00001dc0: 2c20 7368 6170 653d 3329 0a20 2020 2020  , shape=3).     
-00001dd0: 2020 2063 686f 6c2c 2063 6f72 722c 2073     chol, corr, s
-00001de0: 7464 7320 3d20 706d 2e4c 4b4a 4368 6f6c  tds = pm.LKJChol
-00001df0: 6573 6b79 436f 7628 2763 686f 6c5f 636f  eskyCov('chol_co
-00001e00: 7627 2c20 6e3d 332c 2065 7461 3d32 2c0a  v', n=3, eta=2,.
-00001e10: 2020 2020 2020 2020 2020 2020 7364 5f64              sd_d
-00001e20: 6973 743d 7364 5f64 6973 742c 2063 6f6d  ist=sd_dist, com
-00001e30: 7075 7465 5f63 6f72 723d 5472 7565 290a  pute_corr=True).
-00001e40: 2020 2020 2020 2020 7661 6c73 203d 2070          vals = p
-00001e50: 6d2e 4d76 4e6f 726d 616c 2827 7661 6c73  m.MvNormal('vals
-00001e60: 272c 206d 753d 6d75 2c20 6368 6f6c 3d63  ', mu=mu, chol=c
-00001e70: 686f 6c2c 206f 6273 6572 7665 643d 6461  hol, observed=da
-00001e80: 7461 290a 0a20 2020 2046 6f72 2075 6e6f  ta)..    For uno
-00001e90: 6273 6572 7665 6420 7661 6c75 6573 2069  bserved values i
-00001ea0: 7420 6361 6e20 6265 2062 6574 7465 7220  t can be better 
-00001eb0: 746f 2075 7365 2061 206e 6f6e 2d63 656e  to use a non-cen
-00001ec0: 7465 7265 640a 2020 2020 7061 7261 6d65  tered.    parame
-00001ed0: 7472 697a 6174 696f 6e3a 3a0a 0a20 2020  trization::..   
-00001ee0: 2020 2020 2073 645f 6469 7374 203d 2070       sd_dist = p
-00001ef0: 6d2e 4578 706f 6e65 6e74 6961 6c2e 6469  m.Exponential.di
-00001f00: 7374 2831 2e30 2c20 7368 6170 653d 3329  st(1.0, shape=3)
-00001f10: 0a20 2020 2020 2020 2063 686f 6c2c 205f  .        chol, _
-00001f20: 2c20 5f20 3d20 706d 2e4c 4b4a 4368 6f6c  , _ = pm.LKJChol
-00001f30: 6573 6b79 436f 7628 2763 686f 6c5f 636f  eskyCov('chol_co
-00001f40: 7627 2c20 6e3d 332c 2065 7461 3d32 2c0a  v', n=3, eta=2,.
-00001f50: 2020 2020 2020 2020 2020 2020 7364 5f64              sd_d
-00001f60: 6973 743d 7364 5f64 6973 742c 2063 6f6d  ist=sd_dist, com
-00001f70: 7075 7465 5f63 6f72 723d 5472 7565 290a  pute_corr=True).
-00001f80: 2020 2020 2020 2020 7661 6c73 5f72 6177          vals_raw
-00001f90: 203d 2070 6d2e 4e6f 726d 616c 2827 7661   = pm.Normal('va
-00001fa0: 6c73 5f72 6177 272c 206d 753d 302c 2073  ls_raw', mu=0, s
-00001fb0: 6967 6d61 3d31 2c20 7368 6170 653d 2835  igma=1, shape=(5
-00001fc0: 2c20 3329 290a 2020 2020 2020 2020 7661  , 3)).        va
-00001fd0: 6c73 203d 2070 6d2e 4465 7465 726d 696e  ls = pm.Determin
-00001fe0: 6973 7469 6328 2776 616c 7327 2c20 7074  istic('vals', pt
-00001ff0: 2e64 6f74 2863 686f 6c2c 2076 616c 735f  .dot(chol, vals_
-00002000: 7261 772e 5429 2e54 290a 2020 2020 2222  raw.T).T).    ""
-00002010: 220a 2020 2020 7276 5f6f 7020 3d20 6d75  ".    rv_op = mu
-00002020: 6c74 6976 6172 6961 7465 5f6e 6f72 6d61  ltivariate_norma
-00002030: 6c0a 0a20 2020 2040 636c 6173 736d 6574  l..    @classmet
-00002040: 686f 640a 2020 2020 6465 6620 6469 7374  hod.    def dist
-00002050: 2863 6c73 2c20 6d75 2c20 636f 763d 4e6f  (cls, mu, cov=No
-00002060: 6e65 2c20 7461 753d 4e6f 6e65 2c20 6368  ne, tau=None, ch
-00002070: 6f6c 3d4e 6f6e 652c 206c 6f77 6572 3d54  ol=None, lower=T
-00002080: 7275 652c 202a 2a6b 7761 7267 7329 3a0a  rue, **kwargs):.
-00002090: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
-000020a0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-000020b0: 6c65 286d 7529 0a20 2020 2020 2020 2063  le(mu).        c
-000020c0: 6f76 203d 2071 7561 6464 6973 745f 6d61  ov = quaddist_ma
-000020d0: 7472 6978 2863 6f76 2c20 6368 6f6c 2c20  trix(cov, chol, 
-000020e0: 7461 752c 206c 6f77 6572 290a 2020 2020  tau, lower).    
-000020f0: 2020 2020 2320 5079 5465 6e73 6f72 2069      # PyTensor i
-00002100: 7320 7374 7269 6374 6572 2061 626f 7574  s stricter about
-00002110: 2074 6865 2073 6861 7065 206f 6620 6d75   the shape of mu
-00002120: 2c20 7468 616e 2050 794d 4320 7573 6564  , than PyMC used
-00002130: 2074 6f20 6265 0a20 2020 2020 2020 206d   to be.        m
-00002140: 7520 3d20 7074 2e62 726f 6164 6361 7374  u = pt.broadcast
-00002150: 5f61 7272 6179 7328 6d75 2c20 636f 765b  _arrays(mu, cov[
-00002160: 2e2e 2e2c 202d 315d 295b 305d 0a20 2020  ..., -1])[0].   
-00002170: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00002180: 7228 292e 6469 7374 285b 6d75 2c20 636f  r().dist([mu, co
-00002190: 765d 2c20 2a2a 6b77 6172 6773 290a 0a20  v], **kwargs).. 
-000021a0: 2020 2064 6566 206d 6f6d 656e 7428 7276     def moment(rv
-000021b0: 2c20 7369 7a65 2c20 6d75 2c20 636f 7629  , size, mu, cov)
-000021c0: 3a0a 2020 2020 2020 2020 6d6f 6d65 6e74  :.        moment
-000021d0: 203d 206d 750a 2020 2020 2020 2020 6966   = mu.        if
-000021e0: 206e 6f74 2072 765f 7369 7a65 5f69 735f   not rv_size_is_
-000021f0: 6e6f 6e65 2873 697a 6529 3a0a 2020 2020  none(size):.    
-00002200: 2020 2020 2020 2020 6d6f 6d65 6e74 5f73          moment_s
-00002210: 697a 6520 3d20 7074 2e63 6f6e 6361 7465  ize = pt.concate
-00002220: 6e61 7465 285b 7369 7a65 2c20 5b6d 752e  nate([size, [mu.
-00002230: 7368 6170 655b 2d31 5d5d 5d29 0a20 2020  shape[-1]]]).   
-00002240: 2020 2020 2020 2020 206d 6f6d 656e 7420           moment 
-00002250: 3d20 7074 2e66 756c 6c28 6d6f 6d65 6e74  = pt.full(moment
-00002260: 5f73 697a 652c 206d 7529 0a20 2020 2020  _size, mu).     
-00002270: 2020 2072 6574 7572 6e20 6d6f 6d65 6e74     return moment
-00002280: 0a0a 2020 2020 6465 6620 6c6f 6770 2876  ..    def logp(v
-00002290: 616c 7565 2c20 6d75 2c20 636f 7629 3a0a  alue, mu, cov):.
-000022a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000022b0: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
-000022c0: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
-000022d0: 204d 756c 7469 7661 7269 6174 6520 4e6f   Multivariate No
-000022e0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-000022f0: 6e0a 2020 2020 2020 2020 6174 2073 7065  n.        at spe
-00002300: 6369 6669 6564 2076 616c 7565 2e0a 0a20  cified value... 
-00002310: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00002320: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00002330: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
-00002340: 7565 3a20 6e75 6d65 7269 630a 2020 2020  ue: numeric.    
-00002350: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
-00002360: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
-00002370: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
-00002380: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
-00002390: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-000023a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000023b0: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
-000023c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000023d0: 2020 2071 7561 6464 6973 742c 206c 6f67     quaddist, log
-000023e0: 6465 742c 206f 6b20 3d20 7175 6164 6469  det, ok = quaddi
-000023f0: 7374 5f70 6172 7365 2876 616c 7565 2c20  st_parse(value, 
-00002400: 6d75 2c20 636f 7629 0a20 2020 2020 2020  mu, cov).       
-00002410: 206b 203d 2066 6c6f 6174 5828 7661 6c75   k = floatX(valu
-00002420: 652e 7368 6170 655b 2d31 5d29 0a20 2020  e.shape[-1]).   
-00002430: 2020 2020 206e 6f72 6d20 3d20 2d30 2e35       norm = -0.5
-00002440: 202a 206b 202a 2070 6d2e 666c 6f61 7458   * k * pm.floatX
-00002450: 286e 702e 6c6f 6728 3220 2a20 6e70 2e70  (np.log(2 * np.p
-00002460: 6929 290a 2020 2020 2020 2020 7265 7475  i)).        retu
-00002470: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
-00002480: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
-00002490: 206e 6f72 6d20 2d20 302e 3520 2a20 7175   norm - 0.5 * qu
-000024a0: 6164 6469 7374 202d 206c 6f67 6465 742c  addist - logdet,
-000024b0: 0a20 2020 2020 2020 2020 2020 206f 6b2c  .            ok,
-000024c0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-000024d0: 3d22 706f 7364 6566 222c 0a20 2020 2020  ="posdef",.     
-000024e0: 2020 2029 0a0a 0a63 6c61 7373 204d 7653     )...class MvS
-000024f0: 7475 6465 6e74 5452 5628 5261 6e64 6f6d  tudentTRV(Random
-00002500: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
-00002510: 616d 6520 3d20 226d 756c 7469 7661 7269  ame = "multivari
-00002520: 6174 655f 7374 7564 656e 7474 220a 2020  ate_studentt".  
-00002530: 2020 6e64 696d 5f73 7570 7020 3d20 310a    ndim_supp = 1.
-00002540: 2020 2020 6e64 696d 735f 7061 7261 6d73      ndims_params
-00002550: 203d 205b 302c 2031 2c20 325d 0a20 2020   = [0, 1, 2].   
-00002560: 2064 7479 7065 203d 2022 666c 6f61 7458   dtype = "floatX
-00002570: 220a 2020 2020 5f70 7269 6e74 5f6e 616d  ".    _print_nam
-00002580: 6520 3d20 2822 4d76 5374 7564 656e 7454  e = ("MvStudentT
-00002590: 222c 2022 5c5c 6f70 6572 6174 6f72 6e61  ", "\\operatorna
-000025a0: 6d65 7b4d 7653 7475 6465 6e74 547d 2229  me{MvStudentT}")
-000025b0: 0a0a 2020 2020 6465 6620 6d61 6b65 5f6e  ..    def make_n
-000025c0: 6f64 6528 7365 6c66 2c20 726e 672c 2073  ode(self, rng, s
-000025d0: 697a 652c 2064 7479 7065 2c20 6e75 2c20  ize, dtype, nu, 
-000025e0: 6d75 2c20 636f 7629 3a0a 2020 2020 2020  mu, cov):.      
-000025f0: 2020 6e75 203d 2070 742e 6173 5f74 656e    nu = pt.as_ten
-00002600: 736f 725f 7661 7269 6162 6c65 286e 7529  sor_variable(nu)
-00002610: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00002620: 6e75 2e6e 6469 6d20 3d3d 2030 3a0a 2020  nu.ndim == 0:.  
-00002630: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002640: 5661 6c75 6545 7272 6f72 2822 6e75 206d  ValueError("nu m
-00002650: 7573 7420 6265 2061 2073 6361 6c61 7220  ust be a scalar 
-00002660: 286e 6469 6d3d 3029 2e22 290a 0a20 2020  (ndim=0).")..   
-00002670: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00002680: 7228 292e 6d61 6b65 5f6e 6f64 6528 726e  r().make_node(rn
-00002690: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
-000026a0: 6e75 2c20 6d75 2c20 636f 7629 0a0a 2020  nu, mu, cov)..  
-000026b0: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
-000026c0: 656c 662c 206e 752c 206d 753d 4e6f 6e65  elf, nu, mu=None
-000026d0: 2c20 636f 763d 4e6f 6e65 2c20 7369 7a65  , cov=None, size
-000026e0: 3d4e 6f6e 652c 202a 2a6b 7761 7267 7329  =None, **kwargs)
-000026f0: 3a0a 2020 2020 2020 2020 6474 7970 6520  :.        dtype 
-00002700: 3d20 7079 7465 6e73 6f72 2e63 6f6e 6669  = pytensor.confi
-00002710: 672e 666c 6f61 7458 2069 6620 7365 6c66  g.floatX if self
-00002720: 2e64 7479 7065 203d 3d20 2266 6c6f 6174  .dtype == "float
-00002730: 5822 2065 6c73 6520 7365 6c66 2e64 7479  X" else self.dty
-00002740: 7065 0a0a 2020 2020 2020 2020 6966 206d  pe..        if m
-00002750: 7520 6973 204e 6f6e 653a 0a20 2020 2020  u is None:.     
-00002760: 2020 2020 2020 206d 7520 3d20 6e70 2e61         mu = np.a
-00002770: 7272 6179 285b 302e 305d 2c20 6474 7970  rray([0.0], dtyp
-00002780: 653d 6474 7970 6529 0a20 2020 2020 2020  e=dtype).       
-00002790: 2069 6620 636f 7620 6973 204e 6f6e 653a   if cov is None:
-000027a0: 0a20 2020 2020 2020 2020 2020 2063 6f76  .            cov
-000027b0: 203d 206e 702e 6172 7261 7928 5b5b 312e   = np.array([[1.
-000027c0: 305d 5d2c 2064 7479 7065 3d64 7479 7065  0]], dtype=dtype
-000027d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000027e0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
-000027f0: 5f28 6e75 2c20 6d75 2c20 636f 762c 2073  _(nu, mu, cov, s
-00002800: 697a 653d 7369 7a65 2c20 2a2a 6b77 6172  ize=size, **kwar
-00002810: 6773 290a 0a20 2020 2064 6566 205f 7375  gs)..    def _su
-00002820: 7070 5f73 6861 7065 5f66 726f 6d5f 7061  pp_shape_from_pa
-00002830: 7261 6d73 2873 656c 662c 2064 6973 745f  rams(self, dist_
-00002840: 7061 7261 6d73 2c20 7265 705f 7061 7261  params, rep_para
-00002850: 6d5f 6964 783d 312c 2070 6172 616d 5f73  m_idx=1, param_s
-00002860: 6861 7065 733d 4e6f 6e65 293a 0a20 2020  hapes=None):.   
-00002870: 2020 2020 2072 6574 7572 6e20 6465 6661       return defa
-00002880: 756c 745f 7375 7070 5f73 6861 7065 5f66  ult_supp_shape_f
-00002890: 726f 6d5f 7061 7261 6d73 280a 2020 2020  rom_params(.    
-000028a0: 2020 2020 2020 2020 7365 6c66 2e6e 6469          self.ndi
-000028b0: 6d5f 7375 7070 2c20 6469 7374 5f70 6172  m_supp, dist_par
-000028c0: 616d 732c 2072 6570 5f70 6172 616d 5f69  ams, rep_param_i
-000028d0: 6478 2c20 7061 7261 6d5f 7368 6170 6573  dx, param_shapes
-000028e0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000028f0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00002900: 2064 6566 2072 6e67 5f66 6e28 636c 732c   def rng_fn(cls,
-00002910: 2072 6e67 2c20 6e75 2c20 6d75 2c20 636f   rng, nu, mu, co
-00002920: 762c 2073 697a 6529 3a0a 2020 2020 2020  v, size):.      
-00002930: 2020 6d76 5f73 616d 706c 6573 203d 206d    mv_samples = m
-00002940: 756c 7469 7661 7269 6174 655f 6e6f 726d  ultivariate_norm
-00002950: 616c 2e72 6e67 5f66 6e28 726e 673d 726e  al.rng_fn(rng=rn
-00002960: 672c 206d 6561 6e3d 6e70 2e7a 6572 6f73  g, mean=np.zeros
-00002970: 5f6c 696b 6528 6d75 292c 2063 6f76 3d63  _like(mu), cov=c
-00002980: 6f76 2c20 7369 7a65 3d73 697a 6529 0a0a  ov, size=size)..
-00002990: 2020 2020 2020 2020 2320 5461 6b65 2063          # Take c
-000029a0: 6869 3220 6472 6177 7320 616e 6420 6164  hi2 draws and ad
-000029b0: 6420 616e 2061 7869 7320 6f66 206c 656e  d an axis of len
-000029c0: 6774 6820 3120 746f 2074 6865 2072 6967  gth 1 to the rig
-000029d0: 6874 2066 6f72 2063 6f72 7265 6374 2062  ht for correct b
-000029e0: 726f 6164 6361 7374 696e 6720 6265 6c6f  roadcasting belo
-000029f0: 770a 2020 2020 2020 2020 6368 6932 5f73  w.        chi2_s
-00002a00: 616d 706c 6573 203d 206e 702e 7371 7274  amples = np.sqrt
-00002a10: 2872 6e67 2e63 6869 7371 7561 7265 286e  (rng.chisquare(n
-00002a20: 752c 2073 697a 653d 7369 7a65 2920 2f20  u, size=size) / 
-00002a30: 6e75 295b 2e2e 2e2c 204e 6f6e 655d 0a0a  nu)[..., None]..
-00002a40: 2020 2020 2020 2020 6966 2073 697a 653a          if size:
-00002a50: 0a20 2020 2020 2020 2020 2020 206d 7520  .            mu 
-00002a60: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
-00002a70: 6f28 6d75 2c20 7369 7a65 202b 2028 6d75  o(mu, size + (mu
-00002a80: 2e73 6861 7065 5b2d 315d 2c29 290a 0a20  .shape[-1],)).. 
-00002a90: 2020 2020 2020 2072 6574 7572 6e20 286d         return (m
-00002aa0: 765f 7361 6d70 6c65 7320 2f20 6368 6932  v_samples / chi2
-00002ab0: 5f73 616d 706c 6573 2920 2b20 6d75 0a0a  _samples) + mu..
-00002ac0: 0a6d 765f 7374 7564 656e 7474 203d 204d  .mv_studentt = M
-00002ad0: 7653 7475 6465 6e74 5452 5628 290a 0a0a  vStudentTRV()...
-00002ae0: 636c 6173 7320 4d76 5374 7564 656e 7454  class MvStudentT
-00002af0: 2843 6f6e 7469 6e75 6f75 7329 3a0a 2020  (Continuous):.  
-00002b00: 2020 7222 2222 0a20 2020 204d 756c 7469    r""".    Multi
-00002b10: 7661 7269 6174 6520 5374 7564 656e 742d  variate Student-
-00002b20: 5420 6c6f 672d 6c69 6b65 6c69 686f 6f64  T log-likelihood
-00002b30: 2e0a 0a20 2020 202e 2e20 6d61 7468 3a3a  ...    .. math::
-00002b40: 0a20 2020 2020 2020 2066 285c 6d61 7468  .        f(\math
-00002b50: 6266 7b78 7d7c 205c 6e75 2c5c 6d75 2c5c  bf{x}| \nu,\mu,\
-00002b60: 5369 676d 6129 203d 0a20 2020 2020 2020  Sigma) =.       
-00002b70: 205c 6672 6163 0a20 2020 2020 2020 2020   \frac.         
-00002b80: 2020 207b 5c47 616d 6d61 5c6c 6566 745b     {\Gamma\left[
-00002b90: 285c 6e75 2b70 292f 325c 7269 6768 745d  (\nu+p)/2\right]
-00002ba0: 7d0a 2020 2020 2020 2020 2020 2020 7b5c  }.            {\
-00002bb0: 4761 6d6d 6128 5c6e 752f 3229 5c6e 755e  Gamma(\nu/2)\nu^
-00002bc0: 7b70 2f32 7d5c 7069 5e7b 702f 327d 0a20  {p/2}\pi^{p/2}. 
-00002bd0: 2020 2020 2020 2020 2020 2020 5c6c 6566              \lef
-00002be0: 747c 7b5c 5369 676d 617d 5c72 6967 6874  t|{\Sigma}\right
-00002bf0: 7c5e 7b31 2f32 7d0a 2020 2020 2020 2020  |^{1/2}.        
-00002c00: 2020 2020 205c 6c65 6674 5b0a 2020 2020       \left[.    
-00002c10: 2020 2020 2020 2020 2020 2031 2b5c 6672             1+\fr
-00002c20: 6163 7b31 7d7b 5c6e 757d 0a20 2020 2020  ac{1}{\nu}.     
-00002c30: 2020 2020 2020 2020 2020 287b 5c6d 6174            ({\mat
-00002c40: 6862 6620 787d 2d7b 5c6d 757d 295e 540a  hbf x}-{\mu})^T.
-00002c50: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00002c60: 5c53 6967 6d61 7d5e 7b2d 317d 287b 5c6d  \Sigma}^{-1}({\m
-00002c70: 6174 6862 6620 787d 2d7b 5c6d 757d 290a  athbf x}-{\mu}).
-00002c80: 2020 2020 2020 2020 2020 2020 205c 7269               \ri
-00002c90: 6768 745d 5e7b 2d28 5c6e 752b 7029 2f32  ght]^{-(\nu+p)/2
-00002ca0: 7d7d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  }}..    ========
-00002cb0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
-00002cc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002cd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00002ce0: 2020 2020 5375 7070 6f72 7420 2020 3a6d      Support   :m
-00002cf0: 6174 683a 6078 205c 696e 205c 6d61 7468  ath:`x \in \math
-00002d00: 6262 7b52 7d5e 7060 0a20 2020 204d 6561  bb{R}^p`.    Mea
-00002d10: 6e20 2020 2020 203a 6d61 7468 3a60 5c6d  n      :math:`\m
-00002d20: 7560 2069 6620 3a6d 6174 683a 605c 6e75  u` if :math:`\nu
-00002d30: 203e 2031 6020 656c 7365 2075 6e64 6566   > 1` else undef
-00002d40: 696e 6564 0a20 2020 2056 6172 6961 6e63  ined.    Varianc
-00002d50: 6520 203a 6d61 7468 3a60 5c66 7261 637b  e  :math:`\frac{
-00002d60: 5c6e 757d 7b5c 6d75 2d32 7d5c 5369 676d  \nu}{\mu-2}\Sigm
-00002d70: 6160 0a20 2020 2020 2020 2020 2020 2020  a`.             
-00002d80: 2020 2020 2069 6620 3a6d 6174 683a 605c       if :math:`\
-00002d90: 6e75 3e32 6020 656c 7365 2075 6e64 6566  nu>2` else undef
-00002da0: 696e 6564 0a20 2020 203d 3d3d 3d3d 3d3d  ined.    =======
-00002db0: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
-00002dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002de0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00002df0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00002e00: 2020 2020 6e75 203a 2074 656e 736f 725f      nu : tensor_
-00002e10: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-00002e20: 2020 2020 2020 4465 6772 6565 7320 6f66        Degrees of
-00002e30: 2066 7265 6564 6f6d 2c20 7368 6f75 6c64   freedom, should
-00002e40: 2062 6520 6120 706f 7369 7469 7665 2073   be a positive s
-00002e50: 6361 6c61 722e 0a20 2020 2053 6967 6d61  calar..    Sigma
-00002e60: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-00002e70: 6620 666c 6f61 742c 206f 7074 696f 6e61  f float, optiona
-00002e80: 6c0a 2020 2020 2020 2020 5363 616c 6520  l.        Scale 
-00002e90: 6d61 7472 6978 2e20 5573 6520 6073 6361  matrix. Use `sca
-00002ea0: 6c65 6020 696e 206e 6577 2063 6f64 652e  le` in new code.
-00002eb0: 0a20 2020 206d 7520 3a20 7465 6e73 6f72  .    mu : tensor
-00002ec0: 5f6c 696b 6520 6f66 2066 6c6f 6174 2c20  _like of float, 
-00002ed0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00002ee0: 2056 6563 746f 7220 6f66 206d 6561 6e73   Vector of means
-00002ef0: 2e0a 2020 2020 7363 616c 6520 3a20 7465  ..    scale : te
-00002f00: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
-00002f10: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-00002f20: 2020 2020 2054 6865 2073 6361 6c65 206d       The scale m
-00002f30: 6174 7269 782e 0a20 2020 2074 6175 203a  atrix..    tau :
-00002f40: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-00002f50: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
-00002f60: 2020 2020 2020 2020 5468 6520 7072 6563          The prec
-00002f70: 6973 696f 6e20 6d61 7472 6978 2e0a 2020  ision matrix..  
-00002f80: 2020 6368 6f6c 203a 2074 656e 736f 725f    chol : tensor_
-00002f90: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
-00002fa0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00002fb0: 5468 6520 6368 6f6c 6573 6b79 2066 6163  The cholesky fac
-00002fc0: 746f 7220 6f66 2074 6865 2073 6361 6c65  tor of the scale
-00002fd0: 206d 6174 7269 782e 0a20 2020 206c 6f77   matrix..    low
-00002fe0: 6572 203a 2062 6f6f 6c2c 2064 6566 6175  er : bool, defau
-00002ff0: 6c74 3d54 7275 650a 2020 2020 2020 2020  lt=True.        
-00003000: 5768 6574 6865 7220 7468 6520 6368 6f6c  Whether the chol
-00003010: 6573 6b79 2066 6174 636f 7220 6973 2067  esky fatcor is g
-00003020: 6976 656e 2061 7320 6120 6c6f 7765 7220  iven as a lower 
-00003030: 7472 6961 6e67 756c 6172 206d 6174 7269  triangular matri
-00003040: 782e 0a20 2020 2022 2222 0a20 2020 2072  x..    """.    r
-00003050: 765f 6f70 203d 206d 765f 7374 7564 656e  v_op = mv_studen
-00003060: 7474 0a0a 2020 2020 4063 6c61 7373 6d65  tt..    @classme
-00003070: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-00003080: 7428 636c 732c 206e 752c 2053 6967 6d61  t(cls, nu, Sigma
-00003090: 3d4e 6f6e 652c 206d 753d 4e6f 6e65 2c20  =None, mu=None, 
-000030a0: 7363 616c 653d 4e6f 6e65 2c20 7461 753d  scale=None, tau=
-000030b0: 4e6f 6e65 2c20 6368 6f6c 3d4e 6f6e 652c  None, chol=None,
-000030c0: 206c 6f77 6572 3d54 7275 652c 202a 2a6b   lower=True, **k
-000030d0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-000030e0: 636f 7620 3d20 6b77 6172 6773 2e70 6f70  cov = kwargs.pop
-000030f0: 2822 636f 7622 2c20 4e6f 6e65 290a 2020  ("cov", None).  
-00003100: 2020 2020 2020 6966 2063 6f76 2069 7320        if cov is 
-00003110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003120: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00003130: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00003140: 2020 2020 2022 5573 6520 7468 6520 7363       "Use the sc
-00003150: 616c 6520 6172 6775 6d65 6e74 2074 6f20  ale argument to 
-00003160: 7370 6563 6966 7920 7468 6520 7363 616c  specify the scal
-00003170: 6520 6d61 7472 6978 2e20 220a 2020 2020  e matrix. ".    
-00003180: 2020 2020 2020 2020 2020 2020 2263 6f76              "cov
-00003190: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
-000031a0: 2069 6e20 6675 7475 7265 2076 6572 7369   in future versi
-000031b0: 6f6e 732e 222c 0a20 2020 2020 2020 2020  ons.",.         
-000031c0: 2020 2020 2020 2046 7574 7572 6557 6172         FutureWar
-000031d0: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
-000031e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000031f0: 7363 616c 6520 3d20 636f 760a 2020 2020  scale = cov.    
-00003200: 2020 2020 6966 2053 6967 6d61 2069 7320      if Sigma is 
-00003210: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003220: 2020 2020 2020 6966 2073 6361 6c65 2069        if scale i
-00003230: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00003240: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00003250: 6520 5661 6c75 6545 7272 6f72 2822 5370  e ValueError("Sp
-00003260: 6563 6966 7920 6f6e 6c79 206f 6e65 206f  ecify only one o
-00003270: 6620 7363 616c 6520 616e 6420 5369 676d  f scale and Sigm
-00003280: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
-00003290: 7363 616c 6520 3d20 5369 676d 610a 2020  scale = Sigma.  
-000032a0: 2020 2020 2020 6e75 203d 2070 742e 6173        nu = pt.as
-000032b0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-000032c0: 2866 6c6f 6174 5828 6e75 2929 0a20 2020  (floatX(nu)).   
-000032d0: 2020 2020 206d 7520 3d20 7074 2e61 735f       mu = pt.as_
-000032e0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-000032f0: 666c 6f61 7458 286d 7529 290a 2020 2020  floatX(mu)).    
-00003300: 2020 2020 7363 616c 6520 3d20 7175 6164      scale = quad
-00003310: 6469 7374 5f6d 6174 7269 7828 7363 616c  dist_matrix(scal
-00003320: 652c 2063 686f 6c2c 2074 6175 2c20 6c6f  e, chol, tau, lo
-00003330: 7765 7229 0a20 2020 2020 2020 2023 2050  wer).        # P
-00003340: 7954 656e 736f 7220 6973 2073 7472 6963  yTensor is stric
-00003350: 7465 7220 6162 6f75 7420 7468 6520 7368  ter about the sh
-00003360: 6170 6520 6f66 206d 752c 2074 6861 6e20  ape of mu, than 
-00003370: 5079 4d43 2075 7365 6420 746f 2062 650a  PyMC used to be.
-00003380: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
-00003390: 6272 6f61 6463 6173 745f 6172 7261 7973  broadcast_arrays
-000033a0: 286d 752c 2073 6361 6c65 5b2e 2e2e 2c20  (mu, scale[..., 
-000033b0: 2d31 5d29 5b30 5d0a 0a20 2020 2020 2020  -1])[0]..       
-000033c0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-000033d0: 6469 7374 285b 6e75 2c20 6d75 2c20 7363  dist([nu, mu, sc
-000033e0: 616c 655d 2c20 2a2a 6b77 6172 6773 290a  ale], **kwargs).
-000033f0: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
-00003400: 7276 2c20 7369 7a65 2c20 6e75 2c20 6d75  rv, size, nu, mu
-00003410: 2c20 7363 616c 6529 3a0a 2020 2020 2020  , scale):.      
-00003420: 2020 6d6f 6d65 6e74 203d 206d 750a 2020    moment = mu.  
-00003430: 2020 2020 2020 6966 206e 6f74 2072 765f        if not rv_
-00003440: 7369 7a65 5f69 735f 6e6f 6e65 2873 697a  size_is_none(siz
-00003450: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003460: 6d6f 6d65 6e74 5f73 697a 6520 3d20 7074  moment_size = pt
-00003470: 2e63 6f6e 6361 7465 6e61 7465 285b 7369  .concatenate([si
-00003480: 7a65 2c20 5b6d 752e 7368 6170 655b 2d31  ze, [mu.shape[-1
-00003490: 5d5d 5d29 0a20 2020 2020 2020 2020 2020  ]]]).           
-000034a0: 206d 6f6d 656e 7420 3d20 7074 2e66 756c   moment = pt.ful
-000034b0: 6c28 6d6f 6d65 6e74 5f73 697a 652c 206d  l(moment_size, m
-000034c0: 6f6d 656e 7429 0a20 2020 2020 2020 2072  oment).        r
-000034d0: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 2020  eturn moment..  
-000034e0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
-000034f0: 2c20 6e75 2c20 6d75 2c20 7363 616c 6529  , nu, mu, scale)
-00003500: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00003510: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
-00003520: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
-00003530: 6f66 204d 756c 7469 7661 7269 6174 6520  of Multivariate 
-00003540: 5374 7564 656e 7427 7320 5420 6469 7374  Student's T dist
-00003550: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
-00003560: 2061 7420 7370 6563 6966 6965 6420 7661   at specified va
-00003570: 6c75 652e 0a0a 2020 2020 2020 2020 5061  lue...        Pa
-00003580: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00003590: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000035a0: 2020 2020 7661 6c75 653a 206e 756d 6572      value: numer
-000035b0: 6963 0a20 2020 2020 2020 2020 2020 2056  ic.            V
-000035c0: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
-000035d0: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
-000035e0: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
-000035f0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00003600: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00003610: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
-00003620: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
-00003630: 220a 2020 2020 2020 2020 7175 6164 6469  ".        quaddi
-00003640: 7374 2c20 6c6f 6764 6574 2c20 6f6b 203d  st, logdet, ok =
-00003650: 2071 7561 6464 6973 745f 7061 7273 6528   quaddist_parse(
-00003660: 7661 6c75 652c 206d 752c 2073 6361 6c65  value, mu, scale
-00003670: 290a 2020 2020 2020 2020 6b20 3d20 666c  ).        k = fl
-00003680: 6f61 7458 2876 616c 7565 2e73 6861 7065  oatX(value.shape
-00003690: 5b2d 315d 290a 0a20 2020 2020 2020 206e  [-1])..        n
-000036a0: 6f72 6d20 3d20 6761 6d6d 616c 6e28 286e  orm = gammaln((n
-000036b0: 7520 2b20 6b29 202f 2032 2e30 2920 2d20  u + k) / 2.0) - 
-000036c0: 6761 6d6d 616c 6e28 6e75 202f 2032 2e30  gammaln(nu / 2.0
-000036d0: 2920 2d20 302e 3520 2a20 6b20 2a20 7074  ) - 0.5 * k * pt
-000036e0: 2e6c 6f67 286e 7520 2a20 6e70 2e70 6929  .log(nu * np.pi)
-000036f0: 0a20 2020 2020 2020 2069 6e6e 6572 203d  .        inner =
-00003700: 202d 286e 7520 2b20 6b29 202f 2032 2e30   -(nu + k) / 2.0
-00003710: 202a 2070 742e 6c6f 6731 7028 7175 6164   * pt.log1p(quad
-00003720: 6469 7374 202f 206e 7529 0a20 2020 2020  dist / nu).     
-00003730: 2020 2072 6573 203d 206e 6f72 6d20 2b20     res = norm + 
-00003740: 696e 6e65 7220 2d20 6c6f 6764 6574 0a0a  inner - logdet..
-00003750: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00003760: 6865 636b 5f70 6172 616d 6574 6572 7328  heck_parameters(
-00003770: 7265 732c 206f 6b2c 206e 7520 3e20 302c  res, ok, nu > 0,
-00003780: 206d 7367 3d22 706f 7364 6566 2c20 6e75   msg="posdef, nu
-00003790: 203e 2030 2229 0a0a 0a63 6c61 7373 2044   > 0")...class D
-000037a0: 6972 6963 686c 6574 2853 696d 706c 6578  irichlet(Simplex
-000037b0: 436f 6e74 696e 756f 7573 293a 0a20 2020  Continuous):.   
-000037c0: 2072 2222 220a 2020 2020 4469 7269 6368   r""".    Dirich
-000037d0: 6c65 7420 6c6f 672d 6c69 6b65 6c69 686f  let log-likeliho
-000037e0: 6f64 2e0a 0a20 2020 202e 2e20 6d61 7468  od...    .. math
-000037f0: 3a3a 0a0a 2020 2020 2020 2066 285c 6d61  ::..       f(\ma
-00003800: 7468 6266 7b78 7d7c 5c6d 6174 6862 667b  thbf{x}|\mathbf{
-00003810: 617d 2920 3d0a 2020 2020 2020 2020 2020  a}) =.          
-00003820: 205c 6672 6163 7b5c 4761 6d6d 6128 5c73   \frac{\Gamma(\s
-00003830: 756d 5f7b 693d 317d 5e6b 2061 5f69 297d  um_{i=1}^k a_i)}
-00003840: 7b5c 7072 6f64 5f7b 693d 317d 5e6b 205c  {\prod_{i=1}^k \
-00003850: 4761 6d6d 6128 615f 6929 7d0a 2020 2020  Gamma(a_i)}.    
-00003860: 2020 2020 2020 205c 7072 6f64 5f7b 693d         \prod_{i=
-00003870: 317d 5e6b 2078 5f69 5e7b 615f 6920 2d20  1}^k x_i^{a_i - 
-00003880: 317d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  1}..    ========
-00003890: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
-000038a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000038b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000038c0: 3d0a 2020 2020 5375 7070 6f72 7420 2020  =.    Support   
-000038d0: 3a6d 6174 683a 6078 5f69 205c 696e 2028  :math:`x_i \in (
-000038e0: 302c 2031 2960 2066 6f72 203a 6d61 7468  0, 1)` for :math
-000038f0: 3a60 6920 5c69 6e20 5c7b 312c 205c 6c64  :`i \in \{1, \ld
-00003900: 6f74 732c 204b 5c7d 600a 2020 2020 2020  ots, K\}`.      
-00003910: 2020 2020 2020 2020 7375 6368 2074 6861          such tha
-00003920: 7420 3a6d 6174 683a 605c 7375 6d20 785f  t :math:`\sum x_
-00003930: 6920 3d20 3160 0a20 2020 204d 6561 6e20  i = 1`.    Mean 
-00003940: 2020 2020 203a 6d61 7468 3a60 5c64 6672       :math:`\dfr
-00003950: 6163 7b61 5f69 7d7b 5c73 756d 2061 5f69  ac{a_i}{\sum a_i
-00003960: 7d60 0a20 2020 2056 6172 6961 6e63 6520  }`.    Variance 
-00003970: 203a 6d61 7468 3a60 5c64 6672 6163 7b61   :math:`\dfrac{a
-00003980: 5f69 202d 205c 7375 6d20 615f 307d 7b61  _i - \sum a_0}{a
-00003990: 5f30 5e32 2028 615f 3020 2b20 3129 7d60  _0^2 (a_0 + 1)}`
-000039a0: 0a20 2020 2020 2020 2020 2020 2020 2077  .              w
-000039b0: 6865 7265 203a 6d61 7468 3a60 615f 3020  here :math:`a_0 
-000039c0: 3d20 5c73 756d 2061 5f69 600a 2020 2020  = \sum a_i`.    
-000039d0: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-000039e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000039f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003a00: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050  =========..    P
-00003a10: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00003a20: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2061 203a  --------.    a :
-00003a30: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-00003a40: 666c 6f61 740a 2020 2020 2020 2020 436f  float.        Co
-00003a50: 6e63 656e 7472 6174 696f 6e20 7061 7261  ncentration para
-00003a60: 6d65 7465 7273 2028 6120 3e20 3029 2e20  meters (a > 0). 
-00003a70: 5468 6520 6e75 6d62 6572 206f 6620 6361  The number of ca
-00003a80: 7465 676f 7269 6573 2069 7320 6769 7665  tegories is give
-00003a90: 6e20 6279 2074 6865 0a20 2020 2020 2020  n by the.       
-00003aa0: 206c 656e 6774 6820 6f66 2074 6865 206c   length of the l
-00003ab0: 6173 7420 6178 6973 2e0a 2020 2020 2222  ast axis..    ""
-00003ac0: 220a 2020 2020 7276 5f6f 7020 3d20 6469  ".    rv_op = di
-00003ad0: 7269 6368 6c65 740a 0a20 2020 2040 636c  richlet..    @cl
-00003ae0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00003af0: 6620 6469 7374 2863 6c73 2c20 612c 202a  f dist(cls, a, *
-00003b00: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00003b10: 2020 6120 3d20 7074 2e61 735f 7465 6e73    a = pt.as_tens
-00003b20: 6f72 5f76 6172 6961 626c 6528 6129 0a20  or_variable(a). 
-00003b30: 2020 2020 2020 2023 206d 6561 6e20 3d20         # mean = 
-00003b40: 6120 2f20 7074 2e73 756d 2861 290a 2020  a / pt.sum(a).  
-00003b50: 2020 2020 2020 2320 6d6f 6465 203d 2070        # mode = p
-00003b60: 742e 7377 6974 6368 2870 742e 616c 6c28  t.switch(pt.all(
-00003b70: 6120 3e20 3129 2c20 2861 202d 2031 2920  a > 1), (a - 1) 
-00003b80: 2f20 7074 2e73 756d 2861 202d 2031 292c  / pt.sum(a - 1),
-00003b90: 206e 702e 6e61 6e29 0a0a 2020 2020 2020   np.nan)..      
-00003ba0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00003bb0: 2e64 6973 7428 5b61 5d2c 202a 2a6b 7761  .dist([a], **kwa
-00003bc0: 7267 7329 0a0a 2020 2020 6465 6620 6d6f  rgs)..    def mo
-00003bd0: 6d65 6e74 2872 762c 2073 697a 652c 2061  ment(rv, size, a
-00003be0: 293a 0a20 2020 2020 2020 206e 6f72 6d5f  ):.        norm_
-00003bf0: 636f 6e73 7461 6e74 203d 2070 742e 7375  constant = pt.su
-00003c00: 6d28 612c 2061 7869 733d 2d31 295b 2e2e  m(a, axis=-1)[..
-00003c10: 2e2c 204e 6f6e 655d 0a20 2020 2020 2020  ., None].       
-00003c20: 206d 6f6d 656e 7420 3d20 6120 2f20 6e6f   moment = a / no
-00003c30: 726d 5f63 6f6e 7374 616e 740a 2020 2020  rm_constant.    
-00003c40: 2020 2020 6966 206e 6f74 2072 765f 7369      if not rv_si
-00003c50: 7a65 5f69 735f 6e6f 6e65 2873 697a 6529  ze_is_none(size)
-00003c60: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00003c70: 6d65 6e74 203d 2070 742e 6675 6c6c 2870  ment = pt.full(p
-00003c80: 742e 636f 6e63 6174 656e 6174 6528 5b73  t.concatenate([s
-00003c90: 697a 652c 205b 612e 7368 6170 655b 2d31  ize, [a.shape[-1
-00003ca0: 5d5d 5d29 2c20 6d6f 6d65 6e74 290a 2020  ]]]), moment).  
-00003cb0: 2020 2020 2020 7265 7475 726e 206d 6f6d        return mom
-00003cc0: 656e 740a 0a20 2020 2064 6566 206c 6f67  ent..    def log
-00003cd0: 7028 7661 6c75 652c 2061 293a 0a20 2020  p(value, a):.   
-00003ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003cf0: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
-00003d00: 726f 6261 6269 6c69 7479 206f 6620 4469  robability of Di
-00003d10: 7269 6368 6c65 7420 6469 7374 7269 6275  richlet distribu
-00003d20: 7469 6f6e 0a20 2020 2020 2020 2061 7420  tion.        at 
-00003d30: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
-00003d40: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00003d50: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00003d60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00003d70: 7661 6c75 653a 206e 756d 6572 6963 0a20  value: numeric. 
-00003d80: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00003d90: 2066 6f72 2077 6869 6368 206c 6f67 2d70   for which log-p
-00003da0: 726f 6261 6269 6c69 7479 2069 7320 6361  robability is ca
-00003db0: 6c63 756c 6174 6564 2e0a 0a20 2020 2020  lculated...     
-00003dc0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00003dd0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00003de0: 2020 2054 656e 736f 7256 6172 6961 626c     TensorVariabl
-00003df0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00003e00: 2020 2020 2020 2320 6f6e 6c79 2064 6566        # only def
-00003e10: 696e 6564 2066 6f72 2073 756d 2876 616c  ined for sum(val
-00003e20: 7565 2920 3d3d 2031 0a20 2020 2020 2020  ue) == 1.       
-00003e30: 2072 6573 203d 2070 742e 7375 6d28 6c6f   res = pt.sum(lo
-00003e40: 6770 6f77 2876 616c 7565 2c20 6120 2d20  gpow(value, a - 
-00003e50: 3129 202d 2067 616d 6d61 6c6e 2861 292c  1) - gammaln(a),
-00003e60: 2061 7869 733d 2d31 2920 2b20 6761 6d6d   axis=-1) + gamm
-00003e70: 616c 6e28 7074 2e73 756d 2861 2c20 6178  aln(pt.sum(a, ax
-00003e80: 6973 3d2d 3129 290a 2020 2020 2020 2020  is=-1)).        
-00003e90: 7265 7320 3d20 7074 2e73 7769 7463 6828  res = pt.switch(
-00003ea0: 0a20 2020 2020 2020 2020 2020 2070 742e  .            pt.
-00003eb0: 6f72 5f28 0a20 2020 2020 2020 2020 2020  or_(.           
-00003ec0: 2020 2020 2070 742e 616e 7928 7074 2e6c       pt.any(pt.l
-00003ed0: 7428 7661 6c75 652c 2030 292c 2061 7869  t(value, 0), axi
-00003ee0: 733d 2d31 292c 0a20 2020 2020 2020 2020  s=-1),.         
-00003ef0: 2020 2020 2020 2070 742e 616e 7928 7074         pt.any(pt
-00003f00: 2e67 7428 7661 6c75 652c 2031 292c 2061  .gt(value, 1), a
-00003f10: 7869 733d 2d31 292c 0a20 2020 2020 2020  xis=-1),.       
-00003f20: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00003f30: 2020 2020 2d6e 702e 696e 662c 0a20 2020      -np.inf,.   
-00003f40: 2020 2020 2020 2020 2072 6573 2c0a 2020           res,.  
-00003f50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003f60: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
-00003f70: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
-00003f80: 2020 2020 2072 6573 2c0a 2020 2020 2020       res,.      
-00003f90: 2020 2020 2020 6120 3e20 302c 0a20 2020        a > 0,.   
-00003fa0: 2020 2020 2020 2020 206d 7367 3d22 6120           msg="a 
-00003fb0: 3e20 3022 2c0a 2020 2020 2020 2020 290a  > 0",.        ).
-00003fc0: 0a0a 636c 6173 7320 4d75 6c74 696e 6f6d  ..class Multinom
-00003fd0: 6961 6c28 4469 7363 7265 7465 293a 0a20  ial(Discrete):. 
-00003fe0: 2020 2072 2222 220a 2020 2020 4d75 6c74     r""".    Mult
-00003ff0: 696e 6f6d 6961 6c20 6c6f 672d 6c69 6b65  inomial log-like
-00004000: 6c69 686f 6f64 2e0a 0a20 2020 2047 656e  lihood...    Gen
-00004010: 6572 616c 697a 6573 2062 696e 6f6d 6961  eralizes binomia
-00004020: 6c20 6469 7374 7269 6275 7469 6f6e 2c20  l distribution, 
-00004030: 6275 7420 696e 7374 6561 6420 6f66 2065  but instead of e
-00004040: 6163 6820 7472 6961 6c20 7265 7375 6c74  ach trial result
-00004050: 696e 670a 2020 2020 696e 2022 7375 6363  ing.    in "succ
-00004060: 6573 7322 206f 7220 2266 6169 6c75 7265  ess" or "failure
-00004070: 222c 2065 6163 6820 6f6e 6520 7265 7375  ", each one resu
-00004080: 6c74 7320 696e 2065 7861 6374 6c79 206f  lts in exactly o
-00004090: 6e65 206f 6620 736f 6d65 0a20 2020 2066  ne of some.    f
-000040a0: 6978 6564 2066 696e 6974 6520 6e75 6d62  ixed finite numb
-000040b0: 6572 206b 206f 6620 706f 7373 6962 6c65  er k of possible
-000040c0: 206f 7574 636f 6d65 7320 6f76 6572 206e   outcomes over n
-000040d0: 2069 6e64 6570 656e 6465 6e74 2074 7269   independent tri
-000040e0: 616c 732e 0a20 2020 2027 785b 695d 2720  als..    'x[i]' 
-000040f0: 696e 6469 6361 7465 7320 7468 6520 6e75  indicates the nu
-00004100: 6d62 6572 206f 6620 7469 6d65 7320 6f75  mber of times ou
-00004110: 7463 6f6d 6520 6e75 6d62 6572 2069 2077  tcome number i w
-00004120: 6173 206f 6273 6572 7665 640a 2020 2020  as observed.    
-00004130: 6f76 6572 2074 6865 206e 2074 7269 616c  over the n trial
-00004140: 732e 0a0a 2020 2020 2e2e 206d 6174 683a  s...    .. math:
-00004150: 3a0a 0a20 2020 2020 2020 6628 7820 5c6d  :..       f(x \m
-00004160: 6964 206e 2c20 7029 203d 205c 6672 6163  id n, p) = \frac
-00004170: 7b6e 217d 7b5c 7072 6f64 5f7b 693d 317d  {n!}{\prod_{i=1}
-00004180: 5e6b 2078 5f69 217d 205c 7072 6f64 5f7b  ^k x_i!} \prod_{
-00004190: 693d 317d 5e6b 2070 5f69 5e7b 785f 697d  i=1}^k p_i^{x_i}
-000041a0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ..    ==========
-000041b0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
-000041c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000041d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-000041e0: 2020 5375 7070 6f72 7420 2020 2020 3a6d    Support     :m
-000041f0: 6174 683a 6078 205c 696e 205c 7b30 2c20  ath:`x \in \{0, 
-00004200: 312c 205c 6c64 6f74 732c 206e 5c7d 6020  1, \ldots, n\}` 
-00004210: 7375 6368 2074 6861 740a 2020 2020 2020  such that.      
-00004220: 2020 2020 2020 2020 2020 3a6d 6174 683a            :math:
-00004230: 605c 7375 6d20 785f 6920 3d20 6e60 0a20  `\sum x_i = n`. 
-00004240: 2020 204d 6561 6e20 2020 2020 2020 203a     Mean        :
-00004250: 6d61 7468 3a60 6e20 705f 6960 0a20 2020  math:`n p_i`.   
-00004260: 2056 6172 6961 6e63 6520 2020 203a 6d61   Variance    :ma
-00004270: 7468 3a60 6e20 705f 6920 2831 202d 2070  th:`n p_i (1 - p
-00004280: 5f69 2960 0a20 2020 2043 6f76 6172 6961  _i)`.    Covaria
-00004290: 6e63 6520 203a 6d61 7468 3a60 2d6e 2070  nce  :math:`-n p
-000042a0: 5f69 2070 5f6a 6020 666f 7220 3a6d 6174  _i p_j` for :mat
-000042b0: 683a 6069 205c 6e65 206a 600a 2020 2020  h:`i \ne j`.    
-000042c0: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
-000042d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000042e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000042f0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
-00004300: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00004310: 2d2d 2d2d 2d2d 0a20 2020 206e 203a 2074  ------.    n : t
-00004320: 656e 736f 725f 6c69 6b65 206f 6620 696e  ensor_like of in
-00004330: 740a 2020 2020 2020 2020 546f 7461 6c20  t.        Total 
-00004340: 636f 756e 7473 2069 6e20 6561 6368 2072  counts in each r
-00004350: 6570 6c69 6361 7465 2028 6e20 3e20 3029  eplicate (n > 0)
-00004360: 2e0a 2020 2020 7020 3a20 7465 6e73 6f72  ..    p : tensor
-00004370: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-00004380: 2020 2020 2020 2050 726f 6261 6269 6c69         Probabili
-00004390: 7479 206f 6620 6561 6368 206f 6e65 206f  ty of each one o
-000043a0: 6620 7468 6520 6469 6666 6572 656e 7420  f the different 
-000043b0: 6f75 7463 6f6d 6573 2028 3020 3c3d 2070  outcomes (0 <= p
-000043c0: 203c 3d20 3129 2e20 5468 6520 6e75 6d62   <= 1). The numb
-000043d0: 6572 206f 660a 2020 2020 2020 2020 6361  er of.        ca
-000043e0: 7465 676f 7269 6573 2069 7320 6769 7665  tegories is give
-000043f0: 6e20 6279 2074 6865 206c 656e 6774 6820  n by the length 
-00004400: 6f66 2074 6865 206c 6173 7420 6178 6973  of the last axis
-00004410: 2e20 456c 656d 656e 7473 2061 7265 2065  . Elements are e
-00004420: 7870 6563 7465 6420 746f 2073 756d 0a20  xpected to sum. 
-00004430: 2020 2020 2020 2074 6f20 3120 616c 6f6e         to 1 alon
-00004440: 6720 7468 6520 6c61 7374 2061 7869 732e  g the last axis.
-00004450: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
-00004460: 6f70 203d 206d 756c 7469 6e6f 6d69 616c  op = multinomial
-00004470: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00004480: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
-00004490: 636c 732c 206e 2c20 702c 202a 6172 6773  cls, n, p, *args
-000044a0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-000044b0: 2020 2020 2070 203d 2070 742e 6173 5f74       p = pt.as_t
-000044c0: 656e 736f 725f 7661 7269 6162 6c65 2870  ensor_variable(p
-000044d0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
-000044e0: 6e73 7461 6e63 6528 702c 2054 656e 736f  nstance(p, Tenso
-000044f0: 7243 6f6e 7374 616e 7429 3a0a 2020 2020  rConstant):.    
-00004500: 2020 2020 2020 2020 705f 203d 206e 702e          p_ = np.
-00004510: 6173 6172 7261 7928 702e 6461 7461 290a  asarray(p.data).
-00004520: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00004530: 702e 616e 7928 705f 203c 2030 293a 0a20  p.any(p_ < 0):. 
-00004540: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004550: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00004560: 6622 4e65 6761 7469 7665 2060 7060 2070  f"Negative `p` p
-00004570: 6172 616d 6574 6572 7320 6172 6520 6e6f  arameters are no
-00004580: 7420 7661 6c69 642c 2067 6f74 3a20 7b70  t valid, got: {p
-00004590: 5f7d 2229 0a20 2020 2020 2020 2020 2020  _}").           
-000045a0: 2070 5f73 756d 5f20 3d20 6e70 2e73 756d   p_sum_ = np.sum
-000045b0: 285b 705f 5d2c 2061 7869 733d 2d31 290a  ([p_], axis=-1).
-000045c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000045d0: 6f74 206e 702e 616c 6c28 6e70 2e69 7363  ot np.all(np.isc
-000045e0: 6c6f 7365 2870 5f73 756d 5f2c 2031 2e30  lose(p_sum_, 1.0
-000045f0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00004600: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00004610: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00004620: 2020 2020 2020 2066 2260 7060 2070 6172         f"`p` par
-00004630: 616d 6574 6572 7320 7375 6d20 746f 207b  ameters sum to {
-00004640: 705f 7375 6d5f 7d2c 2069 6e73 7465 6164  p_sum_}, instead
-00004650: 206f 6620 312e 302e 2022 0a20 2020 2020   of 1.0. ".     
-00004660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004670: 5468 6579 2077 696c 6c20 6265 2061 7574  They will be aut
-00004680: 6f6d 6174 6963 616c 6c79 2072 6573 6361  omatically resca
-00004690: 6c65 642e 2022 0a20 2020 2020 2020 2020  led. ".         
-000046a0: 2020 2020 2020 2020 2020 2022 596f 7520             "You 
-000046b0: 6361 6e20 7265 7363 616c 6520 7468 656d  can rescale them
-000046c0: 2064 6972 6563 746c 7920 746f 2067 6574   directly to get
-000046d0: 2072 6964 206f 6620 7468 6973 2077 6172   rid of this war
-000046e0: 6e69 6e67 2e22 2c0a 2020 2020 2020 2020  ning.",.        
-000046f0: 2020 2020 2020 2020 2020 2020 5573 6572              User
-00004700: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
-00004710: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00004720: 2020 2020 2020 2020 2020 2070 5f20 3d20             p_ = 
-00004730: 705f 202f 2070 742e 7375 6d28 705f 2c20  p_ / pt.sum(p_, 
-00004740: 6178 6973 3d2d 312c 206b 6565 7064 696d  axis=-1, keepdim
-00004750: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
-00004760: 2020 2020 2020 2020 7020 3d20 7074 2e61          p = pt.a
-00004770: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-00004780: 6528 705f 290a 2020 2020 2020 2020 6e20  e(p_).        n 
-00004790: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-000047a0: 6172 6961 626c 6528 6e29 0a20 2020 2020  ariable(n).     
-000047b0: 2020 2070 203d 2070 742e 6173 5f74 656e     p = pt.as_ten
-000047c0: 736f 725f 7661 7269 6162 6c65 2870 290a  sor_variable(p).
-000047d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000047e0: 7570 6572 2829 2e64 6973 7428 5b6e 2c20  uper().dist([n, 
-000047f0: 705d 2c20 2a61 7267 732c 202a 2a6b 7761  p], *args, **kwa
-00004800: 7267 7329 0a0a 2020 2020 6465 6620 6d6f  rgs)..    def mo
-00004810: 6d65 6e74 2872 762c 2073 697a 652c 206e  ment(rv, size, n
-00004820: 2c20 7029 3a0a 2020 2020 2020 2020 6e20  , p):.        n 
-00004830: 3d20 7074 2e73 6861 7065 5f70 6164 7269  = pt.shape_padri
-00004840: 6768 7428 6e29 0a20 2020 2020 2020 206d  ght(n).        m
-00004850: 6f64 6520 3d20 7074 2e72 6f75 6e64 286e  ode = pt.round(n
-00004860: 202a 2070 290a 2020 2020 2020 2020 6469   * p).        di
-00004870: 6666 203d 206e 202d 2070 742e 7375 6d28  ff = n - pt.sum(
-00004880: 6d6f 6465 2c20 6178 6973 3d2d 312c 206b  mode, axis=-1, k
-00004890: 6565 7064 696d 733d 5472 7565 290a 2020  eepdims=True).  
-000048a0: 2020 2020 2020 696e 635f 626f 6f6c 5f61        inc_bool_a
-000048b0: 7272 203d 2070 742e 6162 7328 6469 6666  rr = pt.abs(diff
-000048c0: 2920 3e20 300a 2020 2020 2020 2020 6d6f  ) > 0.        mo
-000048d0: 6465 203d 2070 742e 696e 635f 7375 6274  de = pt.inc_subt
-000048e0: 656e 736f 7228 6d6f 6465 5b69 6e63 5f62  ensor(mode[inc_b
-000048f0: 6f6f 6c5f 6172 722e 6e6f 6e7a 6572 6f28  ool_arr.nonzero(
-00004900: 295d 2c20 6469 6666 5b69 6e63 5f62 6f6f  )], diff[inc_boo
-00004910: 6c5f 6172 722e 6e6f 6e7a 6572 6f28 295d  l_arr.nonzero()]
-00004920: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00004930: 2072 765f 7369 7a65 5f69 735f 6e6f 6e65   rv_size_is_none
-00004940: 2873 697a 6529 3a0a 2020 2020 2020 2020  (size):.        
-00004950: 2020 2020 6f75 7470 7574 5f73 697a 6520      output_size 
-00004960: 3d20 7074 2e63 6f6e 6361 7465 6e61 7465  = pt.concatenate
-00004970: 285b 7369 7a65 2c20 5b70 2e73 6861 7065  ([size, [p.shape
-00004980: 5b2d 315d 5d5d 290a 2020 2020 2020 2020  [-1]]]).        
-00004990: 2020 2020 6d6f 6465 203d 2070 742e 6675      mode = pt.fu
-000049a0: 6c6c 286f 7574 7075 745f 7369 7a65 2c20  ll(output_size, 
-000049b0: 6d6f 6465 290a 2020 2020 2020 2020 7265  mode).        re
-000049c0: 7475 726e 206d 6f64 650a 0a20 2020 2064  turn mode..    d
-000049d0: 6566 206c 6f67 7028 7661 6c75 652c 206e  ef logp(value, n
-000049e0: 2c20 7029 3a0a 2020 2020 2020 2020 2222  , p):.        ""
-000049f0: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
-00004a00: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
-00004a10: 6974 7920 6f66 204d 756c 7469 6e6f 6d69  ity of Multinomi
-00004a20: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
-00004a30: 2020 2020 2020 2020 6174 2073 7065 6369          at speci
-00004a40: 6669 6564 2076 616c 7565 2e0a 0a20 2020  fied value...   
-00004a50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00004a60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00004a70: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
-00004a80: 3a20 6e75 6d65 7269 630a 2020 2020 2020  : numeric.      
-00004a90: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
-00004aa0: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
-00004ab0: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
-00004ac0: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
-00004ad0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00004ae0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
-00004af0: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
-00004b00: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00004b10: 2020 7265 7320 3d20 6661 6374 6c6e 286e    res = factln(n
-00004b20: 2920 2b20 7074 2e73 756d 282d 6661 6374  ) + pt.sum(-fact
-00004b30: 6c6e 2876 616c 7565 2920 2b20 6c6f 6770  ln(value) + logp
-00004b40: 6f77 2870 2c20 7661 6c75 6529 2c20 6178  ow(p, value), ax
-00004b50: 6973 3d2d 3129 0a20 2020 2020 2020 2072  is=-1).        r
-00004b60: 6573 203d 2070 742e 7377 6974 6368 280a  es = pt.switch(.
-00004b70: 2020 2020 2020 2020 2020 2020 7074 2e6f              pt.o
-00004b80: 725f 2870 742e 616e 7928 7074 2e6c 7428  r_(pt.any(pt.lt(
-00004b90: 7661 6c75 652c 2030 292c 2061 7869 733d  value, 0), axis=
-00004ba0: 2d31 292c 2070 742e 6e65 7128 7074 2e73  -1), pt.neq(pt.s
-00004bb0: 756d 2876 616c 7565 2c20 6178 6973 3d2d  um(value, axis=-
-00004bc0: 3129 2c20 6e29 292c 0a20 2020 2020 2020  1), n)),.       
-00004bd0: 2020 2020 202d 6e70 2e69 6e66 2c0a 2020       -np.inf,.  
-00004be0: 2020 2020 2020 2020 2020 7265 732c 0a20            res,. 
-00004bf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004c00: 2072 6574 7572 6e20 6368 6563 6b5f 7061   return check_pa
-00004c10: 7261 6d65 7465 7273 280a 2020 2020 2020  rameters(.      
-00004c20: 2020 2020 2020 7265 732c 0a20 2020 2020        res,.     
-00004c30: 2020 2020 2020 2030 203c 3d20 702c 0a20         0 <= p,. 
-00004c40: 2020 2020 2020 2020 2020 2070 203c 3d20             p <= 
-00004c50: 312c 0a20 2020 2020 2020 2020 2020 2070  1,.            p
-00004c60: 742e 6973 636c 6f73 6528 7074 2e73 756d  t.isclose(pt.sum
-00004c70: 2870 2c20 6178 6973 3d2d 3129 2c20 3129  (p, axis=-1), 1)
-00004c80: 2c0a 2020 2020 2020 2020 2020 2020 7074  ,.            pt
-00004c90: 2e67 6528 6e2c 2030 292c 0a20 2020 2020  .ge(n, 0),.     
-00004ca0: 2020 2020 2020 206d 7367 3d22 3020 3c3d         msg="0 <=
-00004cb0: 2070 203c 3d20 312c 2073 756d 2870 2920   p <= 1, sum(p) 
-00004cc0: 3d20 312c 206e 203e 3d20 3022 2c0a 2020  = 1, n >= 0",.  
-00004cd0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-00004ce0: 4469 7269 6368 6c65 744d 756c 7469 6e6f  DirichletMultino
-00004cf0: 6d69 616c 5256 2852 616e 646f 6d56 6172  mialRV(RandomVar
-00004d00: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
-00004d10: 203d 2022 6469 7269 6368 6c65 745f 6d75   = "dirichlet_mu
-00004d20: 6c74 696e 6f6d 6961 6c22 0a20 2020 206e  ltinomial".    n
-00004d30: 6469 6d5f 7375 7070 203d 2031 0a20 2020  dim_supp = 1.   
-00004d40: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
-00004d50: 5b30 2c20 315d 0a20 2020 2064 7479 7065  [0, 1].    dtype
-00004d60: 203d 2022 696e 7436 3422 0a20 2020 205f   = "int64".    _
-00004d70: 7072 696e 745f 6e61 6d65 203d 2028 2244  print_name = ("D
-00004d80: 6972 6963 686c 6574 4d4e 222c 2022 5c5c  irichletMN", "\\
-00004d90: 6f70 6572 6174 6f72 6e61 6d65 7b44 6972  operatorname{Dir
-00004da0: 6963 686c 6574 4d4e 7d22 290a 0a20 2020  ichletMN}")..   
-00004db0: 2064 6566 205f 7375 7070 5f73 6861 7065   def _supp_shape
-00004dc0: 5f66 726f 6d5f 7061 7261 6d73 2873 656c  _from_params(sel
-00004dd0: 662c 2064 6973 745f 7061 7261 6d73 2c20  f, dist_params, 
-00004de0: 7265 705f 7061 7261 6d5f 6964 783d 312c  rep_param_idx=1,
-00004df0: 2070 6172 616d 5f73 6861 7065 733d 4e6f   param_shapes=No
-00004e00: 6e65 293a 0a20 2020 2020 2020 2072 6574  ne):.        ret
-00004e10: 7572 6e20 6465 6661 756c 745f 7375 7070  urn default_supp
-00004e20: 5f73 6861 7065 5f66 726f 6d5f 7061 7261  _shape_from_para
-00004e30: 6d73 280a 2020 2020 2020 2020 2020 2020  ms(.            
-00004e40: 7365 6c66 2e6e 6469 6d5f 7375 7070 2c20  self.ndim_supp, 
-00004e50: 6469 7374 5f70 6172 616d 732c 2072 6570  dist_params, rep
-00004e60: 5f70 6172 616d 5f69 6478 2c20 7061 7261  _param_idx, para
-00004e70: 6d5f 7368 6170 6573 0a20 2020 2020 2020  m_shapes.       
-00004e80: 2029 0a0a 2020 2020 4063 6c61 7373 6d65   )..    @classme
-00004e90: 7468 6f64 0a20 2020 2064 6566 2072 6e67  thod.    def rng
-00004ea0: 5f66 6e28 636c 732c 2072 6e67 2c20 6e2c  _fn(cls, rng, n,
-00004eb0: 2061 2c20 7369 7a65 293a 0a20 2020 2020   a, size):.     
-00004ec0: 2020 2069 6620 6e2e 6e64 696d 203e 2030     if n.ndim > 0
-00004ed0: 206f 7220 612e 6e64 696d 203e 2031 3a0a   or a.ndim > 1:.
-00004ee0: 2020 2020 2020 2020 2020 2020 6e2c 2061              n, a
-00004ef0: 203d 2062 726f 6164 6361 7374 5f70 6172   = broadcast_par
-00004f00: 616d 7328 5b6e 2c20 615d 2c20 636c 732e  ams([n, a], cls.
-00004f10: 6e64 696d 735f 7061 7261 6d73 290a 2020  ndims_params).  
-00004f20: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
-00004f30: 2074 7570 6c65 2873 697a 6520 6f72 2028   tuple(size or (
-00004f40: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00004f50: 6966 2073 697a 653a 0a20 2020 2020 2020  if size:.       
-00004f60: 2020 2020 2020 2020 206e 203d 206e 702e           n = np.
-00004f70: 6272 6f61 6463 6173 745f 746f 286e 2c20  broadcast_to(n, 
-00004f80: 7369 7a65 290a 2020 2020 2020 2020 2020  size).          
-00004f90: 2020 2020 2020 6120 3d20 6e70 2e62 726f        a = np.bro
-00004fa0: 6164 6361 7374 5f74 6f28 612c 2073 697a  adcast_to(a, siz
-00004fb0: 6520 2b20 2861 2e73 6861 7065 5b2d 315d  e + (a.shape[-1]
-00004fc0: 2c29 290a 0a20 2020 2020 2020 2020 2020  ,))..           
-00004fd0: 2072 6573 203d 206e 702e 656d 7074 7928   res = np.empty(
-00004fe0: 612e 7368 6170 6529 0a20 2020 2020 2020  a.shape).       
-00004ff0: 2020 2020 2066 6f72 2069 6478 2069 6e20       for idx in 
-00005000: 6e70 2e6e 6469 6e64 6578 2861 2e73 6861  np.ndindex(a.sha
-00005010: 7065 5b3a 2d31 5d29 3a0a 2020 2020 2020  pe[:-1]):.      
-00005020: 2020 2020 2020 2020 2020 7020 3d20 726e            p = rn
-00005030: 672e 6469 7269 6368 6c65 7428 615b 6964  g.dirichlet(a[id
-00005040: 785d 290a 2020 2020 2020 2020 2020 2020  x]).            
-00005050: 2020 2020 7265 735b 6964 785d 203d 2072      res[idx] = r
-00005060: 6e67 2e6d 756c 7469 6e6f 6d69 616c 286e  ng.multinomial(n
-00005070: 5b69 6478 5d2c 2070 290a 2020 2020 2020  [idx], p).      
-00005080: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00005090: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000050a0: 2020 2020 2020 2020 2020 2023 206e 2069             # n i
-000050b0: 7320 6120 7363 616c 6172 2c20 6120 6973  s a scalar, a is
-000050c0: 2061 2031 6420 6172 7261 790a 2020 2020   a 1d array.    
-000050d0: 2020 2020 2020 2020 7020 3d20 726e 672e          p = rng.
-000050e0: 6469 7269 6368 6c65 7428 612c 2073 697a  dirichlet(a, siz
-000050f0: 653d 7369 7a65 2920 2023 2028 7369 7a65  e=size)  # (size
-00005100: 2c20 612e 7368 6170 6529 0a0a 2020 2020  , a.shape)..    
-00005110: 2020 2020 2020 2020 7265 7320 3d20 6e70          res = np
-00005120: 2e65 6d70 7479 2870 2e73 6861 7065 290a  .empty(p.shape).
-00005130: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005140: 6964 7820 696e 206e 702e 6e64 696e 6465  idx in np.ndinde
-00005150: 7828 702e 7368 6170 655b 3a2d 315d 293a  x(p.shape[:-1]):
-00005160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005170: 2072 6573 5b69 6478 5d20 3d20 726e 672e   res[idx] = rng.
-00005180: 6d75 6c74 696e 6f6d 6961 6c28 6e2c 2070  multinomial(n, p
-00005190: 5b69 6478 5d29 0a0a 2020 2020 2020 2020  [idx])..        
-000051a0: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
-000051b0: 0a64 6972 6963 686c 6574 5f6d 756c 7469  .dirichlet_multi
-000051c0: 6e6f 6d69 616c 203d 2044 6972 6963 686c  nomial = Dirichl
-000051d0: 6574 4d75 6c74 696e 6f6d 6961 6c52 5628  etMultinomialRV(
-000051e0: 290a 0a0a 636c 6173 7320 4469 7269 6368  )...class Dirich
-000051f0: 6c65 744d 756c 7469 6e6f 6d69 616c 2844  letMultinomial(D
-00005200: 6973 6372 6574 6529 3a0a 2020 2020 7222  iscrete):.    r"
-00005210: 2222 4469 7269 6368 6c65 7420 4d75 6c74  ""Dirichlet Mult
-00005220: 696e 6f6d 6961 6c20 6c6f 672d 6c69 6b65  inomial log-like
-00005230: 6c69 686f 6f64 2e0a 0a20 2020 2044 6972  lihood...    Dir
-00005240: 6963 686c 6574 206d 6978 7475 7265 206f  ichlet mixture o
-00005250: 6620 4d75 6c74 696e 6f6d 6961 6c73 2064  f Multinomials d
-00005260: 6973 7472 6962 7574 696f 6e2c 2077 6974  istribution, wit
-00005270: 6820 6120 6d61 7267 696e 616c 697a 6564  h a marginalized
-00005280: 2050 4d46 2e0a 0a20 2020 202e 2e20 6d61   PMF...    .. ma
-00005290: 7468 3a3a 0a0a 2020 2020 2020 2020 6628  th::..        f(
-000052a0: 7820 5c6d 6964 206e 2c20 6129 203d 205c  x \mid n, a) = \
-000052b0: 6672 6163 7b5c 4761 6d6d 6128 6e20 2b20  frac{\Gamma(n + 
-000052c0: 3129 5c47 616d 6d61 285c 7375 6d20 615f  1)\Gamma(\sum a_
-000052d0: 6b29 7d0a 2020 2020 2020 2020 2020 2020  k)}.            
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 7b5c 4761 6d6d 6128 6e20 2b20 5c73    {\Gamma(n + \s
-00005300: 756d 2061 5f6b 297d 0a20 2020 2020 2020  um a_k)}.       
-00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005320: 2020 5c70 726f 645f 7b6b 3d31 7d5e 4b0a    \prod_{k=1}^K.
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2020 205c 6672 6163 7b5c           \frac{\
-00005350: 4761 6d6d 6128 785f 6b20 2b20 2061 5f6b  Gamma(x_k +  a_k
-00005360: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 207b 5c47 616d 6d61 2878 5f6b 202b 2031   {\Gamma(x_k + 1
-00005390: 295c 4761 6d6d 6128 615f 6b29 7d0a 0a20  )\Gamma(a_k)}.. 
-000053a0: 2020 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d     ==========  =
-000053b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000053c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000053d0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
-000053e0: 7570 706f 7274 2020 2020 203a 6d61 7468  upport     :math
-000053f0: 3a60 7820 5c69 6e20 5c7b 302c 2031 2c20  :`x \in \{0, 1, 
-00005400: 5c6c 646f 7473 2c20 6e5c 7d60 2073 7563  \ldots, n\}` suc
-00005410: 6820 7468 6174 0a20 2020 2020 2020 2020  h that.         
-00005420: 2020 2020 2020 203a 6d61 7468 3a60 5c73         :math:`\s
-00005430: 756d 2078 5f69 203d 206e 600a 2020 2020  um x_i = n`.    
-00005440: 4d65 616e 2020 2020 2020 2020 3a6d 6174  Mean        :mat
-00005450: 683a 606e 205c 6672 6163 7b61 5f69 7d7b  h:`n \frac{a_i}{
-00005460: 5c73 756d 7b61 5f6b 7d7d 600a 2020 2020  \sum{a_k}}`.    
-00005470: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
-00005480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000054a0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
-000054b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-000054c0: 2d2d 2d2d 2d2d 0a20 2020 206e 203a 2074  ------.    n : t
-000054d0: 656e 736f 725f 6c69 6b65 206f 6620 696e  ensor_like of in
-000054e0: 740a 2020 2020 2020 2020 546f 7461 6c20  t.        Total 
-000054f0: 636f 756e 7473 2069 6e20 6561 6368 2072  counts in each r
-00005500: 6570 6c69 6361 7465 2028 6e20 3e20 3029  eplicate (n > 0)
-00005510: 2e0a 0a20 2020 2061 203a 2074 656e 736f  ...    a : tenso
-00005520: 725f 6c69 6b65 206f 6620 666c 6f61 740a  r_like of float.
-00005530: 2020 2020 2020 2020 4469 7269 6368 6c65          Dirichle
-00005540: 7420 636f 6e63 656e 7472 6174 696f 6e20  t concentration 
-00005550: 7061 7261 6d65 7465 7273 2028 6120 3e20  parameters (a > 
-00005560: 3029 2e20 5468 6520 6e75 6d62 6572 206f  0). The number o
-00005570: 6620 6361 7465 676f 7269 6573 2069 7320  f categories is 
-00005580: 6769 7665 6e20 6279 0a20 2020 2020 2020  given by.       
-00005590: 2074 6865 206c 656e 6774 6820 6f66 2074   the length of t
-000055a0: 6865 206c 6173 7420 6178 6973 2e0a 2020  he last axis..  
-000055b0: 2020 2222 220a 2020 2020 7276 5f6f 7020    """.    rv_op 
-000055c0: 3d20 6469 7269 6368 6c65 745f 6d75 6c74  = dirichlet_mult
-000055d0: 696e 6f6d 6961 6c0a 0a20 2020 2040 636c  inomial..    @cl
-000055e0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000055f0: 6620 6469 7374 2863 6c73 2c20 6e2c 2061  f dist(cls, n, a
-00005600: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00005610: 7329 3a0a 2020 2020 2020 2020 6e20 3d20  s):.        n = 
-00005620: 696e 7458 286e 290a 2020 2020 2020 2020  intX(n).        
-00005630: 6120 3d20 666c 6f61 7458 2861 290a 0a20  a = floatX(a).. 
-00005640: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00005650: 7065 7228 292e 6469 7374 285b 6e2c 2061  per().dist([n, a
-00005660: 5d2c 202a 2a6b 7761 7267 7329 0a0a 2020  ], **kwargs)..  
-00005670: 2020 6465 6620 6d6f 6d65 6e74 2872 762c    def moment(rv,
-00005680: 2073 697a 652c 206e 2c20 6129 3a0a 2020   size, n, a):.  
-00005690: 2020 2020 2020 7020 3d20 6120 2f20 7074        p = a / pt
-000056a0: 2e73 756d 2861 2c20 6178 6973 3d2d 312c  .sum(a, axis=-1,
-000056b0: 206b 6565 7064 696d 733d 5472 7565 290a   keepdims=True).
-000056c0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-000056d0: 6f6d 656e 7428 4d75 6c74 696e 6f6d 6961  oment(Multinomia
-000056e0: 6c2e 6469 7374 286e 3d6e 2c20 703d 702c  l.dist(n=n, p=p,
-000056f0: 2073 697a 653d 7369 7a65 2929 0a0a 2020   size=size))..  
-00005700: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
-00005710: 2c20 6e2c 2061 293a 0a20 2020 2020 2020  , n, a):.       
-00005720: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
-00005730: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
-00005740: 6269 6c69 7479 206f 6620 4469 7269 6368  bility of Dirich
-00005750: 6c65 744d 756c 7469 6e6f 6d69 616c 2064  letMultinomial d
-00005760: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
-00005770: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
-00005780: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-00005790: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000057a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000057b0: 2020 2020 2020 2076 616c 7565 3a20 696e         value: in
-000057c0: 7465 6765 7220 6172 7261 790a 2020 2020  teger array.    
-000057d0: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
-000057e0: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
-000057f0: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
-00005800: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
-00005810: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00005820: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00005830: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
-00005840: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005850: 2020 2073 756d 5f61 203d 2061 2e73 756d     sum_a = a.sum
-00005860: 2861 7869 733d 2d31 290a 2020 2020 2020  (axis=-1).      
-00005870: 2020 636f 6e73 7420 3d20 2867 616d 6d61    const = (gamma
-00005880: 6c6e 286e 202b 2031 2920 2b20 6761 6d6d  ln(n + 1) + gamm
-00005890: 616c 6e28 7375 6d5f 6129 2920 2d20 6761  aln(sum_a)) - ga
-000058a0: 6d6d 616c 6e28 6e20 2b20 7375 6d5f 6129  mmaln(n + sum_a)
-000058b0: 0a20 2020 2020 2020 2073 6572 6965 7320  .        series 
-000058c0: 3d20 6761 6d6d 616c 6e28 7661 6c75 6520  = gammaln(value 
-000058d0: 2b20 6129 202d 2028 6761 6d6d 616c 6e28  + a) - (gammaln(
-000058e0: 7661 6c75 6520 2b20 3129 202b 2067 616d  value + 1) + gam
-000058f0: 6d61 6c6e 2861 2929 0a20 2020 2020 2020  maln(a)).       
-00005900: 2072 6573 203d 2063 6f6e 7374 202b 2073   res = const + s
-00005910: 6572 6965 732e 7375 6d28 6178 6973 3d2d  eries.sum(axis=-
-00005920: 3129 0a0a 2020 2020 2020 2020 7265 7320  1)..        res 
-00005930: 3d20 7074 2e73 7769 7463 6828 0a20 2020  = pt.switch(.   
-00005940: 2020 2020 2020 2020 2070 742e 6f72 5f28           pt.or_(
-00005950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005960: 2070 742e 616e 7928 7074 2e6c 7428 7661   pt.any(pt.lt(va
-00005970: 6c75 652c 2030 292c 2061 7869 733d 2d31  lue, 0), axis=-1
-00005980: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00005990: 2020 2070 742e 6e65 7128 7074 2e73 756d     pt.neq(pt.sum
-000059a0: 2876 616c 7565 2c20 6178 6973 3d2d 3129  (value, axis=-1)
-000059b0: 2c20 6e29 2c0a 2020 2020 2020 2020 2020  , n),.          
-000059c0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-000059d0: 202d 6e70 2e69 6e66 2c0a 2020 2020 2020   -np.inf,.      
-000059e0: 2020 2020 2020 7265 732c 0a20 2020 2020        res,.     
-000059f0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-00005a00: 7475 726e 2063 6865 636b 5f70 6172 616d  turn check_param
-00005a10: 6574 6572 7328 0a20 2020 2020 2020 2020  eters(.         
-00005a20: 2020 2072 6573 2c0a 2020 2020 2020 2020     res,.        
-00005a30: 2020 2020 6120 3e20 302c 0a20 2020 2020      a > 0,.     
-00005a40: 2020 2020 2020 206e 203e 3d20 302c 0a20         n >= 0,. 
-00005a50: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
-00005a60: 6120 3e20 302c 206e 203e 3d20 3022 2c0a  a > 0, n >= 0",.
-00005a70: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-00005a80: 7320 5f4f 7264 6572 6564 4d75 6c74 696e  s _OrderedMultin
-00005a90: 6f6d 6961 6c28 4d75 6c74 696e 6f6d 6961  omial(Multinomia
-00005aa0: 6c29 3a0a 2020 2020 7222 2222 0a20 2020  l):.    r""".   
-00005ab0: 2055 6e64 6572 6c79 696e 6720 636c 6173   Underlying clas
-00005ac0: 7320 666f 7220 6f72 6465 7265 6420 6d75  s for ordered mu
-00005ad0: 6c74 696e 6f6d 6961 6c20 6469 7374 7269  ltinomial distri
-00005ae0: 6275 7469 6f6e 732e 0a20 2020 2053 6565  butions..    See
-00005af0: 2064 6f63 7320 666f 7220 7468 6520 4f72   docs for the Or
+00001040: 2e22 290a 0a20 2020 2020 2020 2023 2074  .")..        # t
+00001050: 6167 2061 7320 6c6f 7765 7220 7472 6961  ag as lower tria
+00001060: 6e67 756c 6172 2074 6f20 656e 6162 6c65  ngular to enable
+00001070: 2070 7974 656e 736f 7220 7265 7772 6974   pytensor rewrit
+00001080: 6573 206f 6620 6368 6f6c 286c 2e6c 2729  es of chol(l.l')
+00001090: 202d 3e20 6c0a 2020 2020 2020 2020 6368   -> l.        ch
+000010a0: 6f6c 2e74 6167 2e6c 6f77 6572 5f74 7269  ol.tag.lower_tri
+000010b0: 616e 6775 6c61 7220 3d20 5472 7565 0a20  angular = True. 
+000010c0: 2020 2020 2020 2063 6f76 203d 2063 686f         cov = cho
+000010d0: 6c2e 646f 7428 6368 6f6c 2e54 290a 0a20  l.dot(chol.T).. 
+000010e0: 2020 2072 6574 7572 6e20 636f 760a 0a0a     return cov...
+000010f0: 6465 6620 7175 6164 6469 7374 5f70 6172  def quaddist_par
+00001100: 7365 2876 616c 7565 2c20 6d75 2c20 636f  se(value, mu, co
+00001110: 762c 206d 6174 5f74 7970 653d 2263 6f76  v, mat_type="cov
+00001120: 2229 3a0a 2020 2020 2222 2243 6f6d 7075  "):.    """Compu
+00001130: 7465 2028 7820 2d20 6d75 292e 5420 4020  te (x - mu).T @ 
+00001140: 5369 676d 615e 2d31 2040 2028 7820 2d20  Sigma^-1 @ (x - 
+00001150: 6d75 2920 616e 6420 7468 6520 6c6f 6764  mu) and the logd
+00001160: 6574 206f 6620 5369 676d 612e 2222 220a  et of Sigma.""".
+00001170: 2020 2020 6966 2076 616c 7565 2e6e 6469      if value.ndi
+00001180: 6d20 3e20 3220 6f72 2076 616c 7565 2e6e  m > 2 or value.n
+00001190: 6469 6d20 3d3d 2030 3a0a 2020 2020 2020  dim == 0:.      
+000011a0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000011b0: 6f72 2822 496e 7661 6c69 6420 6469 6d65  or("Invalid dime
+000011c0: 6e73 696f 6e20 666f 7220 7661 6c75 653a  nsion for value:
+000011d0: 2025 7322 2025 2076 616c 7565 2e6e 6469   %s" % value.ndi
+000011e0: 6d29 0a20 2020 2069 6620 7661 6c75 652e  m).    if value.
+000011f0: 6e64 696d 203d 3d20 313a 0a20 2020 2020  ndim == 1:.     
+00001200: 2020 206f 6e65 6469 6d20 3d20 5472 7565     onedim = True
+00001210: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00001220: 2076 616c 7565 5b4e 6f6e 652c 203a 5d0a   value[None, :].
+00001230: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001240: 2020 6f6e 6564 696d 203d 2046 616c 7365    onedim = False
+00001250: 0a0a 2020 2020 6465 6c74 6120 3d20 7661  ..    delta = va
+00001260: 6c75 6520 2d20 6d75 0a20 2020 2023 2055  lue - mu.    # U
+00001270: 7365 2074 6869 7320 7768 656e 2054 6865  se this when The
+00001280: 616e 6f23 3539 3038 2069 7320 7265 6c65  ano#5908 is rele
+00001290: 6173 6564 2e0a 2020 2020 2320 7265 7475  ased..    # retu
+000012a0: 726e 204d 764e 6f72 6d61 6c4c 6f67 7028  rn MvNormalLogp(
+000012b0: 2928 7365 6c66 2e63 6f76 2c20 6465 6c74  )(self.cov, delt
+000012c0: 6129 0a20 2020 2063 686f 6c5f 636f 7620  a).    chol_cov 
+000012d0: 3d20 6368 6f6c 6573 6b79 2863 6f76 290a  = cholesky(cov).
+000012e0: 2020 2020 6966 206d 6174 5f74 7970 6520      if mat_type 
+000012f0: 213d 2022 7461 7522 3a0a 2020 2020 2020  != "tau":.      
+00001300: 2020 6469 7374 2c20 6c6f 6764 6574 2c20    dist, logdet, 
+00001310: 6f6b 203d 2071 7561 6464 6973 745f 6368  ok = quaddist_ch
+00001320: 6f6c 2864 656c 7461 2c20 6368 6f6c 5f63  ol(delta, chol_c
+00001330: 6f76 290a 2020 2020 656c 7365 3a0a 2020  ov).    else:.  
+00001340: 2020 2020 2020 6469 7374 2c20 6c6f 6764        dist, logd
+00001350: 6574 2c20 6f6b 203d 2071 7561 6464 6973  et, ok = quaddis
+00001360: 745f 7461 7528 6465 6c74 612c 2063 686f  t_tau(delta, cho
+00001370: 6c5f 636f 7629 0a20 2020 2069 6620 6f6e  l_cov).    if on
+00001380: 6564 696d 3a0a 2020 2020 2020 2020 7265  edim:.        re
+00001390: 7475 726e 2064 6973 745b 305d 2c20 6c6f  turn dist[0], lo
+000013a0: 6764 6574 2c20 6f6b 0a0a 2020 2020 7265  gdet, ok..    re
+000013b0: 7475 726e 2064 6973 742c 206c 6f67 6465  turn dist, logde
+000013c0: 742c 206f 6b0a 0a0a 6465 6620 7175 6164  t, ok...def quad
+000013d0: 6469 7374 5f63 686f 6c28 6465 6c74 612c  dist_chol(delta,
+000013e0: 2063 686f 6c5f 6d61 7429 3a0a 2020 2020   chol_mat):.    
+000013f0: 6469 6167 203d 2070 742e 6469 6167 2863  diag = pt.diag(c
+00001400: 686f 6c5f 6d61 7429 0a20 2020 2023 2043  hol_mat).    # C
+00001410: 6865 636b 2069 6620 7468 6520 636f 7661  heck if the cova
+00001420: 7269 616e 6365 206d 6174 7269 7820 6973  riance matrix is
+00001430: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
+00001440: 7465 2e0a 2020 2020 6f6b 203d 2070 742e  te..    ok = pt.
+00001450: 616c 6c28 6469 6167 203e 2030 290a 2020  all(diag > 0).  
+00001460: 2020 2320 4966 206e 6f74 2c20 7265 706c    # If not, repl
+00001470: 6163 6520 7468 6520 6469 6167 6f6e 616c  ace the diagonal
+00001480: 2e20 5765 2072 6574 7572 6e20 2d69 6e66  . We return -inf
+00001490: 206c 6174 6572 2c20 6275 740a 2020 2020   later, but.    
+000014a0: 2320 6e65 6564 2074 6f20 7072 6576 656e  # need to preven
+000014b0: 7420 736f 6c76 655f 6c6f 7765 7220 6672  t solve_lower fr
+000014c0: 6f6d 2074 6872 6f77 696e 6720 616e 2065  om throwing an e
+000014d0: 7863 6570 7469 6f6e 2e0a 2020 2020 6368  xception..    ch
+000014e0: 6f6c 5f63 6f76 203d 2070 742e 7377 6974  ol_cov = pt.swit
+000014f0: 6368 286f 6b2c 2063 686f 6c5f 6d61 742c  ch(ok, chol_mat,
+00001500: 2031 290a 0a20 2020 2064 656c 7461 5f74   1)..    delta_t
+00001510: 7261 6e73 203d 2073 6f6c 7665 5f6c 6f77  rans = solve_low
+00001520: 6572 2863 686f 6c5f 636f 762c 2064 656c  er(chol_cov, del
+00001530: 7461 2e54 292e 540a 2020 2020 7175 6164  ta.T).T.    quad
+00001540: 6469 7374 203d 2028 6465 6c74 615f 7472  dist = (delta_tr
+00001550: 616e 732a 2a32 292e 7375 6d28 6178 6973  ans**2).sum(axis
+00001560: 3d2d 3129 0a20 2020 206c 6f67 6465 7420  =-1).    logdet 
+00001570: 3d20 7074 2e73 756d 2870 742e 6c6f 6728  = pt.sum(pt.log(
+00001580: 6469 6167 2929 0a20 2020 2072 6574 7572  diag)).    retur
+00001590: 6e20 7175 6164 6469 7374 2c20 6c6f 6764  n quaddist, logd
+000015a0: 6574 2c20 6f6b 0a0a 0a64 6566 2071 7561  et, ok...def qua
+000015b0: 6464 6973 745f 7461 7528 6465 6c74 612c  ddist_tau(delta,
+000015c0: 2063 686f 6c5f 6d61 7429 3a0a 2020 2020   chol_mat):.    
+000015d0: 6469 6167 203d 2070 742e 6e6c 696e 616c  diag = pt.nlinal
+000015e0: 672e 6469 6167 2863 686f 6c5f 6d61 7429  g.diag(chol_mat)
+000015f0: 0a20 2020 2023 2043 6865 636b 2069 6620  .    # Check if 
+00001600: 7468 6520 7072 6563 6973 696f 6e20 6d61  the precision ma
+00001610: 7472 6978 2069 7320 706f 7369 7469 7665  trix is positive
+00001620: 2064 6566 696e 6974 652e 0a20 2020 206f   definite..    o
+00001630: 6b20 3d20 7074 2e61 6c6c 2864 6961 6720  k = pt.all(diag 
+00001640: 3e20 3029 0a20 2020 2023 2049 6620 6e6f  > 0).    # If no
+00001650: 742c 2072 6570 6c61 6365 2074 6865 2064  t, replace the d
+00001660: 6961 676f 6e61 6c2e 2057 6520 7265 7475  iagonal. We retu
+00001670: 726e 202d 696e 6620 6c61 7465 722c 2062  rn -inf later, b
+00001680: 7574 0a20 2020 2023 206e 6565 6420 746f  ut.    # need to
+00001690: 2070 7265 7665 6e74 2073 6f6c 7665 5f6c   prevent solve_l
+000016a0: 6f77 6572 2066 726f 6d20 7468 726f 7769  ower from throwi
+000016b0: 6e67 2061 6e20 6578 6365 7074 696f 6e2e  ng an exception.
+000016c0: 0a20 2020 2063 686f 6c5f 7461 7520 3d20  .    chol_tau = 
+000016d0: 7074 2e73 7769 7463 6828 6f6b 2c20 6368  pt.switch(ok, ch
+000016e0: 6f6c 5f6d 6174 2c20 3129 0a0a 2020 2020  ol_mat, 1)..    
+000016f0: 6465 6c74 615f 7472 616e 7320 3d20 7074  delta_trans = pt
+00001700: 2e64 6f74 2864 656c 7461 2c20 6368 6f6c  .dot(delta, chol
+00001710: 5f74 6175 290a 2020 2020 7175 6164 6469  _tau).    quaddi
+00001720: 7374 203d 2028 6465 6c74 615f 7472 616e  st = (delta_tran
+00001730: 732a 2a32 292e 7375 6d28 6178 6973 3d2d  s**2).sum(axis=-
+00001740: 3129 0a20 2020 206c 6f67 6465 7420 3d20  1).    logdet = 
+00001750: 2d70 742e 7375 6d28 7074 2e6c 6f67 2864  -pt.sum(pt.log(d
+00001760: 6961 6729 290a 2020 2020 7265 7475 726e  iag)).    return
+00001770: 2071 7561 6464 6973 742c 206c 6f67 6465   quaddist, logde
+00001780: 742c 206f 6b0a 0a0a 636c 6173 7320 4d76  t, ok...class Mv
+00001790: 4e6f 726d 616c 2843 6f6e 7469 6e75 6f75  Normal(Continuou
+000017a0: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
+000017b0: 204d 756c 7469 7661 7269 6174 6520 6e6f   Multivariate no
+000017c0: 726d 616c 206c 6f67 2d6c 696b 656c 6968  rmal log-likelih
+000017d0: 6f6f 642e 0a0a 2020 2020 2e2e 206d 6174  ood...    .. mat
+000017e0: 683a 3a0a 0a20 2020 2020 2020 6628 7820  h::..       f(x 
+000017f0: 5c6d 6964 205c 7069 2c20 5429 203d 0a20  \mid \pi, T) =. 
+00001800: 2020 2020 2020 2020 2020 5c66 7261 637b            \frac{
+00001810: 7c54 7c5e 7b31 2f32 7d7d 7b28 325c 7069  |T|^{1/2}}{(2\pi
+00001820: 295e 7b6b 2f32 7d7d 0a20 2020 2020 2020  )^{k/2}}.       
+00001830: 2020 2020 5c65 7870 5c6c 6566 745c 7b20      \exp\left\{ 
+00001840: 2d5c 6672 6163 7b31 7d7b 327d 2028 782d  -\frac{1}{2} (x-
+00001850: 5c6d 7529 5e7b 5c70 7269 6d65 7d20 5420  \mu)^{\prime} T 
+00001860: 2878 2d5c 6d75 2920 5c72 6967 6874 5c7d  (x-\mu) \right\}
+00001870: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
+00001880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001890: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
+000018a0: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
+000018b0: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
+000018c0: 5e6b 600a 2020 2020 4d65 616e 2020 2020  ^k`.    Mean    
+000018d0: 2020 3a6d 6174 683a 605c 6d75 600a 2020    :math:`\mu`.  
+000018e0: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
+000018f0: 683a 6054 5e7b 2d31 7d60 0a20 2020 203d  h:`T^{-1}`.    =
+00001900: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
+00001910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001920: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
+00001930: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00001940: 2d2d 0a20 2020 206d 7520 3a20 7465 6e73  --.    mu : tens
+00001950: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00001960: 0a20 2020 2020 2020 2056 6563 746f 7220  .        Vector 
+00001970: 6f66 206d 6561 6e73 2e0a 2020 2020 636f  of means..    co
+00001980: 7620 3a20 7465 6e73 6f72 5f6c 696b 6520  v : tensor_like 
+00001990: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+000019a0: 616c 0a20 2020 2020 2020 2043 6f76 6172  al.        Covar
+000019b0: 6961 6e63 6520 6d61 7472 6978 2e20 4578  iance matrix. Ex
+000019c0: 6163 746c 7920 6f6e 6520 6f66 2063 6f76  actly one of cov
+000019d0: 2c20 7461 752c 206f 7220 6368 6f6c 2069  , tau, or chol i
+000019e0: 7320 6e65 6564 6564 2e0a 2020 2020 7461  s needed..    ta
+000019f0: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
+00001a00: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+00001a10: 616c 0a20 2020 2020 2020 2050 7265 6369  al.        Preci
+00001a20: 7369 6f6e 206d 6174 7269 782e 2045 7861  sion matrix. Exa
+00001a30: 6374 6c79 206f 6e65 206f 6620 636f 762c  ctly one of cov,
+00001a40: 2074 6175 2c20 6f72 2063 686f 6c20 6973   tau, or chol is
+00001a50: 206e 6565 6465 642e 0a20 2020 2063 686f   needed..    cho
+00001a60: 6c20 3a20 7465 6e73 6f72 5f6c 696b 6520  l : tensor_like 
+00001a70: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+00001a80: 616c 0a20 2020 2020 2020 2043 686f 6c65  al.        Chole
+00001a90: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
+00001aa0: 6e20 6f66 2063 6f76 6172 6961 6e63 6520  n of covariance 
+00001ab0: 6d61 7472 6978 2e20 4578 6163 746c 7920  matrix. Exactly 
+00001ac0: 6f6e 6520 6f66 2063 6f76 2c0a 2020 2020  one of cov,.    
+00001ad0: 2020 2020 7461 752c 206f 7220 6368 6f6c      tau, or chol
+00001ae0: 2069 7320 6e65 6564 6564 2e0a 2020 2020   is needed..    
+00001af0: 6c6f 7765 723a 2062 6f6f 6c2c 2064 6566  lower: bool, def
+00001b00: 6175 6c74 3d54 7275 650a 2020 2020 2020  ault=True.      
+00001b10: 2020 5768 6574 6865 7220 6368 6f6c 2069    Whether chol i
+00001b20: 7320 7468 6520 6c6f 7765 7220 7472 6964  s the lower trid
+00001b30: 6961 676f 6e61 6c20 6368 6f6c 6573 6b79  iagonal cholesky
+00001b40: 2066 6163 746f 722e 0a0a 2020 2020 4578   factor...    Ex
+00001b50: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00001b60: 2d2d 2d0a 2020 2020 4465 6669 6e65 2061  ---.    Define a
+00001b70: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
+00001b80: 726d 616c 2076 6172 6961 626c 6520 666f  rmal variable fo
+00001b90: 7220 6120 6769 7665 6e20 636f 7661 7269  r a given covari
+00001ba0: 616e 6365 0a20 2020 206d 6174 7269 783a  ance.    matrix:
+00001bb0: 3a0a 0a20 2020 2020 2020 2063 6f76 203d  :..        cov =
+00001bc0: 206e 702e 6172 7261 7928 5b5b 312e 2c20   np.array([[1., 
+00001bd0: 302e 355d 2c20 5b30 2e35 2c20 325d 5d29  0.5], [0.5, 2]])
+00001be0: 0a20 2020 2020 2020 206d 7520 3d20 6e70  .        mu = np
+00001bf0: 2e7a 6572 6f73 2832 290a 2020 2020 2020  .zeros(2).      
+00001c00: 2020 7661 6c73 203d 2070 6d2e 4d76 4e6f    vals = pm.MvNo
+00001c10: 726d 616c 2827 7661 6c73 272c 206d 753d  rmal('vals', mu=
+00001c20: 6d75 2c20 636f 763d 636f 762c 2073 6861  mu, cov=cov, sha
+00001c30: 7065 3d28 352c 2032 2929 0a0a 2020 2020  pe=(5, 2))..    
+00001c40: 4d6f 7374 206f 6620 7468 6520 7469 6d65  Most of the time
+00001c50: 2069 7420 6973 2070 7265 6665 7261 626c   it is preferabl
+00001c60: 6520 746f 2073 7065 6369 6679 2074 6865  e to specify the
+00001c70: 2063 686f 6c65 736b 790a 2020 2020 6661   cholesky.    fa
+00001c80: 6374 6f72 206f 6620 7468 6520 636f 7661  ctor of the cova
+00001c90: 7269 616e 6365 2069 6e73 7465 6164 2e20  riance instead. 
+00001ca0: 466f 7220 6578 616d 706c 652c 2077 6520  For example, we 
+00001cb0: 636f 756c 640a 2020 2020 6669 7420 6120  could.    fit a 
+00001cc0: 6d75 6c74 6976 6172 6961 7465 206f 7574  multivariate out
+00001cd0: 636f 6d65 206c 696b 6520 7468 6973 2028  come like this (
+00001ce0: 7365 6520 7468 6520 646f 6373 7472 696e  see the docstrin
+00001cf0: 670a 2020 2020 6f66 2060 4c4b 4a43 686f  g.    of `LKJCho
+00001d00: 6c65 736b 7943 6f76 6020 666f 7220 6d6f  leskyCov` for mo
+00001d10: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
+00001d20: 626f 7574 2074 6869 7329 3a3a 0a0a 2020  bout this)::..  
+00001d30: 2020 2020 2020 6d75 203d 206e 702e 7a65        mu = np.ze
+00001d40: 726f 7328 3329 0a20 2020 2020 2020 2074  ros(3).        t
+00001d50: 7275 655f 636f 7620 3d20 6e70 2e61 7272  rue_cov = np.arr
+00001d60: 6179 285b 5b31 2e30 2c20 302e 352c 2030  ay([[1.0, 0.5, 0
+00001d70: 2e31 5d2c 0a20 2020 2020 2020 2020 2020  .1],.           
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 5b30 2e35 2c20 322e 302c 2030 2e32    [0.5, 2.0, 0.2
+00001da0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 5b30 2e31 2c20 302e 322c 2031 2e30 5d5d  [0.1, 0.2, 1.0]]
+00001dd0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00001de0: 206e 702e 7261 6e64 6f6d 2e6d 756c 7469   np.random.multi
+00001df0: 7661 7269 6174 655f 6e6f 726d 616c 286d  variate_normal(m
+00001e00: 752c 2074 7275 655f 636f 762c 2031 3029  u, true_cov, 10)
+00001e10: 0a0a 2020 2020 2020 2020 7364 5f64 6973  ..        sd_dis
+00001e20: 7420 3d20 706d 2e45 7870 6f6e 656e 7469  t = pm.Exponenti
+00001e30: 616c 2e64 6973 7428 312e 302c 2073 6861  al.dist(1.0, sha
+00001e40: 7065 3d33 290a 2020 2020 2020 2020 6368  pe=3).        ch
+00001e50: 6f6c 2c20 636f 7272 2c20 7374 6473 203d  ol, corr, stds =
+00001e60: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
+00001e70: 6f76 2827 6368 6f6c 5f63 6f76 272c 206e  ov('chol_cov', n
+00001e80: 3d33 2c20 6574 613d 322c 0a20 2020 2020  =3, eta=2,.     
+00001e90: 2020 2020 2020 2073 645f 6469 7374 3d73         sd_dist=s
+00001ea0: 645f 6469 7374 2c20 636f 6d70 7574 655f  d_dist, compute_
+00001eb0: 636f 7272 3d54 7275 6529 0a20 2020 2020  corr=True).     
+00001ec0: 2020 2076 616c 7320 3d20 706d 2e4d 764e     vals = pm.MvN
+00001ed0: 6f72 6d61 6c28 2776 616c 7327 2c20 6d75  ormal('vals', mu
+00001ee0: 3d6d 752c 2063 686f 6c3d 6368 6f6c 2c20  =mu, chol=chol, 
+00001ef0: 6f62 7365 7276 6564 3d64 6174 6129 0a0a  observed=data)..
+00001f00: 2020 2020 466f 7220 756e 6f62 7365 7276      For unobserv
+00001f10: 6564 2076 616c 7565 7320 6974 2063 616e  ed values it can
+00001f20: 2062 6520 6265 7474 6572 2074 6f20 7573   be better to us
+00001f30: 6520 6120 6e6f 6e2d 6365 6e74 6572 6564  e a non-centered
+00001f40: 0a20 2020 2070 6172 616d 6574 7269 7a61  .    parametriza
+00001f50: 7469 6f6e 3a3a 0a0a 2020 2020 2020 2020  tion::..        
+00001f60: 7364 5f64 6973 7420 3d20 706d 2e45 7870  sd_dist = pm.Exp
+00001f70: 6f6e 656e 7469 616c 2e64 6973 7428 312e  onential.dist(1.
+00001f80: 302c 2073 6861 7065 3d33 290a 2020 2020  0, shape=3).    
+00001f90: 2020 2020 6368 6f6c 2c20 5f2c 205f 203d      chol, _, _ =
+00001fa0: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
+00001fb0: 6f76 2827 6368 6f6c 5f63 6f76 272c 206e  ov('chol_cov', n
+00001fc0: 3d33 2c20 6574 613d 322c 0a20 2020 2020  =3, eta=2,.     
+00001fd0: 2020 2020 2020 2073 645f 6469 7374 3d73         sd_dist=s
+00001fe0: 645f 6469 7374 2c20 636f 6d70 7574 655f  d_dist, compute_
+00001ff0: 636f 7272 3d54 7275 6529 0a20 2020 2020  corr=True).     
+00002000: 2020 2076 616c 735f 7261 7720 3d20 706d     vals_raw = pm
+00002010: 2e4e 6f72 6d61 6c28 2776 616c 735f 7261  .Normal('vals_ra
+00002020: 7727 2c20 6d75 3d30 2c20 7369 676d 613d  w', mu=0, sigma=
+00002030: 312c 2073 6861 7065 3d28 352c 2033 2929  1, shape=(5, 3))
+00002040: 0a20 2020 2020 2020 2076 616c 7320 3d20  .        vals = 
+00002050: 706d 2e44 6574 6572 6d69 6e69 7374 6963  pm.Deterministic
+00002060: 2827 7661 6c73 272c 2070 742e 646f 7428  ('vals', pt.dot(
+00002070: 6368 6f6c 2c20 7661 6c73 5f72 6177 2e54  chol, vals_raw.T
+00002080: 292e 5429 0a20 2020 2022 2222 0a20 2020  ).T).    """.   
+00002090: 2072 765f 6f70 203d 206d 756c 7469 7661   rv_op = multiva
+000020a0: 7269 6174 655f 6e6f 726d 616c 0a0a 2020  riate_normal..  
+000020b0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000020c0: 2020 2064 6566 2064 6973 7428 636c 732c     def dist(cls,
+000020d0: 206d 752c 2063 6f76 3d4e 6f6e 652c 2074   mu, cov=None, t
+000020e0: 6175 3d4e 6f6e 652c 2063 686f 6c3d 4e6f  au=None, chol=No
+000020f0: 6e65 2c20 6c6f 7765 723d 5472 7565 2c20  ne, lower=True, 
+00002100: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00002110: 2020 206d 7520 3d20 7074 2e61 735f 7465     mu = pt.as_te
+00002120: 6e73 6f72 5f76 6172 6961 626c 6528 6d75  nsor_variable(mu
+00002130: 290a 2020 2020 2020 2020 636f 7620 3d20  ).        cov = 
+00002140: 7175 6164 6469 7374 5f6d 6174 7269 7828  quaddist_matrix(
+00002150: 636f 762c 2063 686f 6c2c 2074 6175 2c20  cov, chol, tau, 
+00002160: 6c6f 7765 7229 0a20 2020 2020 2020 2023  lower).        #
+00002170: 2050 7954 656e 736f 7220 6973 2073 7472   PyTensor is str
+00002180: 6963 7465 7220 6162 6f75 7420 7468 6520  icter about the 
+00002190: 7368 6170 6520 6f66 206d 752c 2074 6861  shape of mu, tha
+000021a0: 6e20 5079 4d43 2075 7365 6420 746f 2062  n PyMC used to b
+000021b0: 650a 2020 2020 2020 2020 6d75 203d 2070  e.        mu = p
+000021c0: 742e 6272 6f61 6463 6173 745f 6172 7261  t.broadcast_arra
+000021d0: 7973 286d 752c 2063 6f76 5b2e 2e2e 2c20  ys(mu, cov[..., 
+000021e0: 2d31 5d29 5b30 5d0a 2020 2020 2020 2020  -1])[0].        
+000021f0: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
+00002200: 6973 7428 5b6d 752c 2063 6f76 5d2c 202a  ist([mu, cov], *
+00002210: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00002220: 6620 6d6f 6d65 6e74 2872 762c 2073 697a  f moment(rv, siz
+00002230: 652c 206d 752c 2063 6f76 293a 0a20 2020  e, mu, cov):.   
+00002240: 2020 2020 206d 6f6d 656e 7420 3d20 6d75       moment = mu
+00002250: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00002260: 7276 5f73 697a 655f 6973 5f6e 6f6e 6528  rv_size_is_none(
+00002270: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
+00002280: 2020 206d 6f6d 656e 745f 7369 7a65 203d     moment_size =
+00002290: 2070 742e 636f 6e63 6174 656e 6174 6528   pt.concatenate(
+000022a0: 5b73 697a 652c 205b 6d75 2e73 6861 7065  [size, [mu.shape
+000022b0: 5b2d 315d 5d5d 290a 2020 2020 2020 2020  [-1]]]).        
+000022c0: 2020 2020 6d6f 6d65 6e74 203d 2070 742e      moment = pt.
+000022d0: 6675 6c6c 286d 6f6d 656e 745f 7369 7a65  full(moment_size
+000022e0: 2c20 6d75 290a 2020 2020 2020 2020 7265  , mu).        re
+000022f0: 7475 726e 206d 6f6d 656e 740a 0a20 2020  turn moment..   
+00002300: 2064 6566 206c 6f67 7028 7661 6c75 652c   def logp(value,
+00002310: 206d 752c 2063 6f76 293a 0a20 2020 2020   mu, cov):.     
+00002320: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00002330: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
+00002340: 6261 6269 6c69 7479 206f 6620 4d75 6c74  bability of Mult
+00002350: 6976 6172 6961 7465 204e 6f72 6d61 6c20  ivariate Normal 
+00002360: 6469 7374 7269 6275 7469 6f6e 0a20 2020  distribution.   
+00002370: 2020 2020 2061 7420 7370 6563 6966 6965       at specifie
+00002380: 6420 7661 6c75 652e 0a0a 2020 2020 2020  d value...      
+00002390: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000023a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000023b0: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
+000023c0: 756d 6572 6963 0a20 2020 2020 2020 2020  umeric.         
+000023d0: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
+000023e0: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
+000023f0: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
+00002400: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00002410: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00002420: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
+00002430: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
+00002440: 2020 2222 220a 2020 2020 2020 2020 7175    """.        qu
+00002450: 6164 6469 7374 2c20 6c6f 6764 6574 2c20  addist, logdet, 
+00002460: 6f6b 203d 2071 7561 6464 6973 745f 7061  ok = quaddist_pa
+00002470: 7273 6528 7661 6c75 652c 206d 752c 2063  rse(value, mu, c
+00002480: 6f76 290a 2020 2020 2020 2020 6b20 3d20  ov).        k = 
+00002490: 666c 6f61 7458 2876 616c 7565 2e73 6861  floatX(value.sha
+000024a0: 7065 5b2d 315d 290a 2020 2020 2020 2020  pe[-1]).        
+000024b0: 6e6f 726d 203d 202d 302e 3520 2a20 6b20  norm = -0.5 * k 
+000024c0: 2a20 706d 2e66 6c6f 6174 5828 6e70 2e6c  * pm.floatX(np.l
+000024d0: 6f67 2832 202a 206e 702e 7069 2929 0a20  og(2 * np.pi)). 
+000024e0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+000024f0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
+00002500: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
+00002510: 202d 2030 2e35 202a 2071 7561 6464 6973   - 0.5 * quaddis
+00002520: 7420 2d20 6c6f 6764 6574 2c0a 2020 2020  t - logdet,.    
+00002530: 2020 2020 2020 2020 6f6b 2c0a 2020 2020          ok,.    
+00002540: 2020 2020 2020 2020 6d73 673d 2270 6f73          msg="pos
+00002550: 6465 6622 2c0a 2020 2020 2020 2020 290a  def",.        ).
+00002560: 0a0a 636c 6173 7320 4d76 5374 7564 656e  ..class MvStuden
+00002570: 7454 5256 2852 616e 646f 6d56 6172 6961  tTRV(RandomVaria
+00002580: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
+00002590: 2022 6d75 6c74 6976 6172 6961 7465 5f73   "multivariate_s
+000025a0: 7475 6465 6e74 7422 0a20 2020 206e 6469  tudentt".    ndi
+000025b0: 6d5f 7375 7070 203d 2031 0a20 2020 206e  m_supp = 1.    n
+000025c0: 6469 6d73 5f70 6172 616d 7320 3d20 5b30  dims_params = [0
+000025d0: 2c20 312c 2032 5d0a 2020 2020 6474 7970  , 1, 2].    dtyp
+000025e0: 6520 3d20 2266 6c6f 6174 5822 0a20 2020  e = "floatX".   
+000025f0: 205f 7072 696e 745f 6e61 6d65 203d 2028   _print_name = (
+00002600: 224d 7653 7475 6465 6e74 5422 2c20 225c  "MvStudentT", "\
+00002610: 5c6f 7065 7261 746f 726e 616d 657b 4d76  \operatorname{Mv
+00002620: 5374 7564 656e 7454 7d22 290a 0a20 2020  StudentT}")..   
+00002630: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
+00002640: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
+00002650: 6474 7970 652c 206e 752c 206d 752c 2063  dtype, nu, mu, c
+00002660: 6f76 293a 0a20 2020 2020 2020 206e 7520  ov):.        nu 
+00002670: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00002680: 6172 6961 626c 6528 6e75 290a 2020 2020  ariable(nu).    
+00002690: 2020 2020 6966 206e 6f74 206e 752e 6e64      if not nu.nd
+000026a0: 696d 203d 3d20 303a 0a20 2020 2020 2020  im == 0:.       
+000026b0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000026c0: 4572 726f 7228 226e 7520 6d75 7374 2062  Error("nu must b
+000026d0: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
+000026e0: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
+000026f0: 7265 7475 726e 2073 7570 6572 2829 2e6d  return super().m
+00002700: 616b 655f 6e6f 6465 2872 6e67 2c20 7369  ake_node(rng, si
+00002710: 7a65 2c20 6474 7970 652c 206e 752c 206d  ze, dtype, nu, m
+00002720: 752c 2063 6f76 290a 0a20 2020 2064 6566  u, cov)..    def
+00002730: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
+00002740: 6e75 2c20 6d75 3d4e 6f6e 652c 2063 6f76  nu, mu=None, cov
+00002750: 3d4e 6f6e 652c 2073 697a 653d 4e6f 6e65  =None, size=None
+00002760: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00002770: 2020 2020 2064 7479 7065 203d 2070 7974       dtype = pyt
+00002780: 656e 736f 722e 636f 6e66 6967 2e66 6c6f  ensor.config.flo
+00002790: 6174 5820 6966 2073 656c 662e 6474 7970  atX if self.dtyp
+000027a0: 6520 3d3d 2022 666c 6f61 7458 2220 656c  e == "floatX" el
+000027b0: 7365 2073 656c 662e 6474 7970 650a 0a20  se self.dtype.. 
+000027c0: 2020 2020 2020 2069 6620 6d75 2069 7320         if mu is 
+000027d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000027e0: 2020 6d75 203d 206e 702e 6172 7261 7928    mu = np.array(
+000027f0: 5b30 2e30 5d2c 2064 7479 7065 3d64 7479  [0.0], dtype=dty
+00002800: 7065 290a 2020 2020 2020 2020 6966 2063  pe).        if c
+00002810: 6f76 2069 7320 4e6f 6e65 3a0a 2020 2020  ov is None:.    
+00002820: 2020 2020 2020 2020 636f 7620 3d20 6e70          cov = np
+00002830: 2e61 7272 6179 285b 5b31 2e30 5d5d 2c20  .array([[1.0]], 
+00002840: 6474 7970 653d 6474 7970 6529 0a20 2020  dtype=dtype).   
+00002850: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00002860: 7228 292e 5f5f 6361 6c6c 5f5f 286e 752c  r().__call__(nu,
+00002870: 206d 752c 2063 6f76 2c20 7369 7a65 3d73   mu, cov, size=s
+00002880: 697a 652c 202a 2a6b 7761 7267 7329 0a0a  ize, **kwargs)..
+00002890: 2020 2020 6465 6620 5f73 7570 705f 7368      def _supp_sh
+000028a0: 6170 655f 6672 6f6d 5f70 6172 616d 7328  ape_from_params(
+000028b0: 7365 6c66 2c20 6469 7374 5f70 6172 616d  self, dist_param
+000028c0: 732c 2072 6570 5f70 6172 616d 5f69 6478  s, rep_param_idx
+000028d0: 3d31 2c20 7061 7261 6d5f 7368 6170 6573  =1, param_shapes
+000028e0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+000028f0: 7265 7475 726e 2064 6566 6175 6c74 5f73  return default_s
+00002900: 7570 705f 7368 6170 655f 6672 6f6d 5f70  upp_shape_from_p
+00002910: 6172 616d 7328 0a20 2020 2020 2020 2020  arams(.         
+00002920: 2020 2073 656c 662e 6e64 696d 5f73 7570     self.ndim_sup
+00002930: 702c 2064 6973 745f 7061 7261 6d73 2c20  p, dist_params, 
+00002940: 7265 705f 7061 7261 6d5f 6964 782c 2070  rep_param_idx, p
+00002950: 6172 616d 5f73 6861 7065 730a 2020 2020  aram_shapes.    
+00002960: 2020 2020 290a 0a20 2020 2040 636c 6173      )..    @clas
+00002970: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00002980: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
+00002990: 206e 752c 206d 752c 2063 6f76 2c20 7369   nu, mu, cov, si
+000029a0: 7a65 293a 0a20 2020 2020 2020 206d 765f  ze):.        mv_
+000029b0: 7361 6d70 6c65 7320 3d20 6d75 6c74 6976  samples = multiv
+000029c0: 6172 6961 7465 5f6e 6f72 6d61 6c2e 726e  ariate_normal.rn
+000029d0: 675f 666e 2872 6e67 3d72 6e67 2c20 6d65  g_fn(rng=rng, me
+000029e0: 616e 3d6e 702e 7a65 726f 735f 6c69 6b65  an=np.zeros_like
+000029f0: 286d 7529 2c20 636f 763d 636f 762c 2073  (mu), cov=cov, s
+00002a00: 697a 653d 7369 7a65 290a 0a20 2020 2020  ize=size)..     
+00002a10: 2020 2023 2054 616b 6520 6368 6932 2064     # Take chi2 d
+00002a20: 7261 7773 2061 6e64 2061 6464 2061 6e20  raws and add an 
+00002a30: 6178 6973 206f 6620 6c65 6e67 7468 2031  axis of length 1
+00002a40: 2074 6f20 7468 6520 7269 6768 7420 666f   to the right fo
+00002a50: 7220 636f 7272 6563 7420 6272 6f61 6463  r correct broadc
+00002a60: 6173 7469 6e67 2062 656c 6f77 0a20 2020  asting below.   
+00002a70: 2020 2020 2063 6869 325f 7361 6d70 6c65       chi2_sample
+00002a80: 7320 3d20 6e70 2e73 7172 7428 726e 672e  s = np.sqrt(rng.
+00002a90: 6368 6973 7175 6172 6528 6e75 2c20 7369  chisquare(nu, si
+00002aa0: 7a65 3d73 697a 6529 202f 206e 7529 5b2e  ze=size) / nu)[.
+00002ab0: 2e2e 2c20 4e6f 6e65 5d0a 0a20 2020 2020  .., None]..     
+00002ac0: 2020 2069 6620 7369 7a65 3a0a 2020 2020     if size:.    
+00002ad0: 2020 2020 2020 2020 6d75 203d 206e 702e          mu = np.
+00002ae0: 6272 6f61 6463 6173 745f 746f 286d 752c  broadcast_to(mu,
+00002af0: 2073 697a 6520 2b20 286d 752e 7368 6170   size + (mu.shap
+00002b00: 655b 2d31 5d2c 2929 0a0a 2020 2020 2020  e[-1],))..      
+00002b10: 2020 7265 7475 726e 2028 6d76 5f73 616d    return (mv_sam
+00002b20: 706c 6573 202f 2063 6869 325f 7361 6d70  ples / chi2_samp
+00002b30: 6c65 7329 202b 206d 750a 0a0a 6d76 5f73  les) + mu...mv_s
+00002b40: 7475 6465 6e74 7420 3d20 4d76 5374 7564  tudentt = MvStud
+00002b50: 656e 7454 5256 2829 0a0a 0a63 6c61 7373  entTRV()...class
+00002b60: 204d 7653 7475 6465 6e74 5428 436f 6e74   MvStudentT(Cont
+00002b70: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
+00002b80: 220a 2020 2020 4d75 6c74 6976 6172 6961  ".    Multivaria
+00002b90: 7465 2053 7475 6465 6e74 2d54 206c 6f67  te Student-T log
+00002ba0: 2d6c 696b 656c 6968 6f6f 642e 0a0a 2020  -likelihood...  
+00002bb0: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
+00002bc0: 2020 2020 6628 5c6d 6174 6862 667b 787d      f(\mathbf{x}
+00002bd0: 7c20 5c6e 752c 5c6d 752c 5c53 6967 6d61  | \nu,\mu,\Sigma
+00002be0: 2920 3d0a 2020 2020 2020 2020 5c66 7261  ) =.        \fra
+00002bf0: 630a 2020 2020 2020 2020 2020 2020 7b5c  c.            {\
+00002c00: 4761 6d6d 615c 6c65 6674 5b28 5c6e 752b  Gamma\left[(\nu+
+00002c10: 7029 2f32 5c72 6967 6874 5d7d 0a20 2020  p)/2\right]}.   
+00002c20: 2020 2020 2020 2020 207b 5c47 616d 6d61           {\Gamma
+00002c30: 285c 6e75 2f32 295c 6e75 5e7b 702f 327d  (\nu/2)\nu^{p/2}
+00002c40: 5c70 695e 7b70 2f32 7d0a 2020 2020 2020  \pi^{p/2}.      
+00002c50: 2020 2020 2020 205c 6c65 6674 7c7b 5c53         \left|{\S
+00002c60: 6967 6d61 7d5c 7269 6768 747c 5e7b 312f  igma}\right|^{1/
+00002c70: 327d 0a20 2020 2020 2020 2020 2020 2020  2}.             
+00002c80: 5c6c 6566 745b 0a20 2020 2020 2020 2020  \left[.         
+00002c90: 2020 2020 2020 312b 5c66 7261 637b 317d        1+\frac{1}
+00002ca0: 7b5c 6e75 7d0a 2020 2020 2020 2020 2020  {\nu}.          
+00002cb0: 2020 2020 2028 7b5c 6d61 7468 6266 2078       ({\mathbf x
+00002cc0: 7d2d 7b5c 6d75 7d29 5e54 0a20 2020 2020  }-{\mu})^T.     
+00002cd0: 2020 2020 2020 2020 2020 7b5c 5369 676d            {\Sigm
+00002ce0: 617d 5e7b 2d31 7d28 7b5c 6d61 7468 6266  a}^{-1}({\mathbf
+00002cf0: 2078 7d2d 7b5c 6d75 7d29 0a20 2020 2020   x}-{\mu}).     
+00002d00: 2020 2020 2020 2020 5c72 6967 6874 5d5e          \right]^
+00002d10: 7b2d 285c 6e75 2b70 292f 327d 7d0a 0a20  {-(\nu+p)/2}}.. 
+00002d20: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
+00002d30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002d40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002d50: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
+00002d60: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
+00002d70: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
+00002d80: 5e70 600a 2020 2020 4d65 616e 2020 2020  ^p`.    Mean    
+00002d90: 2020 3a6d 6174 683a 605c 6d75 6020 6966    :math:`\mu` if
+00002da0: 203a 6d61 7468 3a60 5c6e 7520 3e20 3160   :math:`\nu > 1`
+00002db0: 2065 6c73 6520 756e 6465 6669 6e65 640a   else undefined.
+00002dc0: 2020 2020 5661 7269 616e 6365 2020 3a6d      Variance  :m
+00002dd0: 6174 683a 605c 6672 6163 7b5c 6e75 7d7b  ath:`\frac{\nu}{
+00002de0: 5c6d 752d 327d 5c53 6967 6d61 600a 2020  \mu-2}\Sigma`.  
+00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e00: 6966 203a 6d61 7468 3a60 5c6e 753e 3260  if :math:`\nu>2`
+00002e10: 2065 6c73 6520 756e 6465 6669 6e65 640a   else undefined.
+00002e20: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+00002e30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020  ===========..   
+00002e60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00002e70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
+00002e80: 7520 3a20 7465 6e73 6f72 5f6c 696b 6520  u : tensor_like 
+00002e90: 6f66 2066 6c6f 6174 0a20 2020 2020 2020  of float.       
+00002ea0: 2044 6567 7265 6573 206f 6620 6672 6565   Degrees of free
+00002eb0: 646f 6d2c 2073 686f 756c 6420 6265 2061  dom, should be a
+00002ec0: 2070 6f73 6974 6976 6520 7363 616c 6172   positive scalar
+00002ed0: 2e0a 2020 2020 5369 676d 6120 3a20 7465  ..    Sigma : te
+00002ee0: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
+00002ef0: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
+00002f00: 2020 2020 2053 6361 6c65 206d 6174 7269       Scale matri
+00002f10: 782e 2055 7365 2060 7363 616c 6560 2069  x. Use `scale` i
+00002f20: 6e20 6e65 7720 636f 6465 2e0a 2020 2020  n new code..    
+00002f30: 6d75 203a 2074 656e 736f 725f 6c69 6b65  mu : tensor_like
+00002f40: 206f 6620 666c 6f61 742c 206f 7074 696f   of float, optio
+00002f50: 6e61 6c0a 2020 2020 2020 2020 5665 6374  nal.        Vect
+00002f60: 6f72 206f 6620 6d65 616e 732e 0a20 2020  or of means..   
+00002f70: 2073 6361 6c65 203a 2074 656e 736f 725f   scale : tensor_
+00002f80: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+00002f90: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00002fa0: 5468 6520 7363 616c 6520 6d61 7472 6978  The scale matrix
+00002fb0: 2e0a 2020 2020 7461 7520 3a20 7465 6e73  ..    tau : tens
+00002fc0: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00002fd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00002fe0: 2020 2054 6865 2070 7265 6369 7369 6f6e     The precision
+00002ff0: 206d 6174 7269 782e 0a20 2020 2063 686f   matrix..    cho
+00003000: 6c20 3a20 7465 6e73 6f72 5f6c 696b 6520  l : tensor_like 
+00003010: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+00003020: 616c 0a20 2020 2020 2020 2054 6865 2063  al.        The c
+00003030: 686f 6c65 736b 7920 6661 6374 6f72 206f  holesky factor o
+00003040: 6620 7468 6520 7363 616c 6520 6d61 7472  f the scale matr
+00003050: 6978 2e0a 2020 2020 6c6f 7765 7220 3a20  ix..    lower : 
+00003060: 626f 6f6c 2c20 6465 6661 756c 743d 5472  bool, default=Tr
+00003070: 7565 0a20 2020 2020 2020 2057 6865 7468  ue.        Wheth
+00003080: 6572 2074 6865 2063 686f 6c65 736b 7920  er the cholesky 
+00003090: 6661 7463 6f72 2069 7320 6769 7665 6e20  fatcor is given 
+000030a0: 6173 2061 206c 6f77 6572 2074 7269 616e  as a lower trian
+000030b0: 6775 6c61 7220 6d61 7472 6978 2e0a 2020  gular matrix..  
+000030c0: 2020 2222 220a 2020 2020 7276 5f6f 7020    """.    rv_op 
+000030d0: 3d20 6d76 5f73 7475 6465 6e74 740a 0a20  = mv_studentt.. 
+000030e0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000030f0: 2020 2020 6465 6620 6469 7374 2863 6c73      def dist(cls
+00003100: 2c20 6e75 2c20 5369 676d 613d 4e6f 6e65  , nu, Sigma=None
+00003110: 2c20 6d75 3d4e 6f6e 652c 2073 6361 6c65  , mu=None, scale
+00003120: 3d4e 6f6e 652c 2074 6175 3d4e 6f6e 652c  =None, tau=None,
+00003130: 2063 686f 6c3d 4e6f 6e65 2c20 6c6f 7765   chol=None, lowe
+00003140: 723d 5472 7565 2c20 2a2a 6b77 6172 6773  r=True, **kwargs
+00003150: 293a 0a20 2020 2020 2020 2063 6f76 203d  ):.        cov =
+00003160: 206b 7761 7267 732e 706f 7028 2263 6f76   kwargs.pop("cov
+00003170: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00003180: 2069 6620 636f 7620 6973 206e 6f74 204e   if cov is not N
+00003190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000031a0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031c0: 2255 7365 2074 6865 2073 6361 6c65 2061  "Use the scale a
+000031d0: 7267 756d 656e 7420 746f 2073 7065 6369  rgument to speci
+000031e0: 6679 2074 6865 2073 6361 6c65 206d 6174  fy the scale mat
+000031f0: 7269 782e 2022 0a20 2020 2020 2020 2020  rix. ".         
+00003200: 2020 2020 2020 2022 636f 7620 7769 6c6c         "cov will
+00003210: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
+00003220: 7574 7572 6520 7665 7273 696f 6e73 2e22  uture versions."
+00003230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003240: 2020 4675 7475 7265 5761 726e 696e 672c    FutureWarning,
+00003250: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00003260: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00003270: 203d 2063 6f76 0a20 2020 2020 2020 2069   = cov.        i
+00003280: 6620 5369 676d 6120 6973 206e 6f74 204e  f Sigma is not N
+00003290: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000032a0: 2069 6620 7363 616c 6520 6973 206e 6f74   if scale is not
+000032b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000032c0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000032d0: 7565 4572 726f 7228 2253 7065 6369 6679  ueError("Specify
+000032e0: 206f 6e6c 7920 6f6e 6520 6f66 2073 6361   only one of sca
+000032f0: 6c65 2061 6e64 2053 6967 6d61 2229 0a20  le and Sigma"). 
+00003300: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00003310: 203d 2053 6967 6d61 0a20 2020 2020 2020   = Sigma.       
+00003320: 206e 7520 3d20 7074 2e61 735f 7465 6e73   nu = pt.as_tens
+00003330: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
+00003340: 7458 286e 7529 290a 2020 2020 2020 2020  tX(nu)).        
+00003350: 6d75 203d 2070 742e 6173 5f74 656e 736f  mu = pt.as_tenso
+00003360: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
+00003370: 5828 6d75 2929 0a20 2020 2020 2020 2073  X(mu)).        s
+00003380: 6361 6c65 203d 2071 7561 6464 6973 745f  cale = quaddist_
+00003390: 6d61 7472 6978 2873 6361 6c65 2c20 6368  matrix(scale, ch
+000033a0: 6f6c 2c20 7461 752c 206c 6f77 6572 290a  ol, tau, lower).
+000033b0: 2020 2020 2020 2020 2320 5079 5465 6e73          # PyTens
+000033c0: 6f72 2069 7320 7374 7269 6374 6572 2061  or is stricter a
+000033d0: 626f 7574 2074 6865 2073 6861 7065 206f  bout the shape o
+000033e0: 6620 6d75 2c20 7468 616e 2050 794d 4320  f mu, than PyMC 
+000033f0: 7573 6564 2074 6f20 6265 0a20 2020 2020  used to be.     
+00003400: 2020 206d 7520 3d20 7074 2e62 726f 6164     mu = pt.broad
+00003410: 6361 7374 5f61 7272 6179 7328 6d75 2c20  cast_arrays(mu, 
+00003420: 7363 616c 655b 2e2e 2e2c 202d 315d 295b  scale[..., -1])[
+00003430: 305d 0a0a 2020 2020 2020 2020 7265 7475  0]..        retu
+00003440: 726e 2073 7570 6572 2829 2e64 6973 7428  rn super().dist(
+00003450: 5b6e 752c 206d 752c 2073 6361 6c65 5d2c  [nu, mu, scale],
+00003460: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00003470: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
+00003480: 697a 652c 206e 752c 206d 752c 2073 6361  ize, nu, mu, sca
+00003490: 6c65 293a 0a20 2020 2020 2020 206d 6f6d  le):.        mom
+000034a0: 656e 7420 3d20 6d75 0a20 2020 2020 2020  ent = mu.       
+000034b0: 2069 6620 6e6f 7420 7276 5f73 697a 655f   if not rv_size_
+000034c0: 6973 5f6e 6f6e 6528 7369 7a65 293a 0a20  is_none(size):. 
+000034d0: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
+000034e0: 745f 7369 7a65 203d 2070 742e 636f 6e63  t_size = pt.conc
+000034f0: 6174 656e 6174 6528 5b73 697a 652c 205b  atenate([size, [
+00003500: 6d75 2e73 6861 7065 5b2d 315d 5d5d 290a  mu.shape[-1]]]).
+00003510: 2020 2020 2020 2020 2020 2020 6d6f 6d65              mome
+00003520: 6e74 203d 2070 742e 6675 6c6c 286d 6f6d  nt = pt.full(mom
+00003530: 656e 745f 7369 7a65 2c20 6d6f 6d65 6e74  ent_size, moment
+00003540: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00003550: 206d 6f6d 656e 740a 0a20 2020 2064 6566   moment..    def
+00003560: 206c 6f67 7028 7661 6c75 652c 206e 752c   logp(value, nu,
+00003570: 206d 752c 2073 6361 6c65 293a 0a20 2020   mu, scale):.   
+00003580: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003590: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
+000035a0: 726f 6261 6269 6c69 7479 206f 6620 4d75  robability of Mu
+000035b0: 6c74 6976 6172 6961 7465 2053 7475 6465  ltivariate Stude
+000035c0: 6e74 2773 2054 2064 6973 7472 6962 7574  nt's T distribut
+000035d0: 696f 6e0a 2020 2020 2020 2020 6174 2073  ion.        at s
+000035e0: 7065 6369 6669 6564 2076 616c 7565 2e0a  pecified value..
+000035f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00003600: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00003610: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
+00003620: 616c 7565 3a20 6e75 6d65 7269 630a 2020  alue: numeric.  
+00003630: 2020 2020 2020 2020 2020 5661 6c75 6520            Value 
+00003640: 666f 7220 7768 6963 6820 6c6f 672d 7072  for which log-pr
+00003650: 6f62 6162 696c 6974 7920 6973 2063 616c  obability is cal
+00003660: 6375 6c61 7465 642e 0a0a 2020 2020 2020  culated...      
+00003670: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00003680: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00003690: 2020 5465 6e73 6f72 5661 7269 6162 6c65    TensorVariable
+000036a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000036b0: 2020 2020 2071 7561 6464 6973 742c 206c       quaddist, l
+000036c0: 6f67 6465 742c 206f 6b20 3d20 7175 6164  ogdet, ok = quad
+000036d0: 6469 7374 5f70 6172 7365 2876 616c 7565  dist_parse(value
+000036e0: 2c20 6d75 2c20 7363 616c 6529 0a20 2020  , mu, scale).   
+000036f0: 2020 2020 206b 203d 2066 6c6f 6174 5828       k = floatX(
+00003700: 7661 6c75 652e 7368 6170 655b 2d31 5d29  value.shape[-1])
+00003710: 0a0a 2020 2020 2020 2020 6e6f 726d 203d  ..        norm =
+00003720: 2067 616d 6d61 6c6e 2828 6e75 202b 206b   gammaln((nu + k
+00003730: 2920 2f20 322e 3029 202d 2067 616d 6d61  ) / 2.0) - gamma
+00003740: 6c6e 286e 7520 2f20 322e 3029 202d 2030  ln(nu / 2.0) - 0
+00003750: 2e35 202a 206b 202a 2070 742e 6c6f 6728  .5 * k * pt.log(
+00003760: 6e75 202a 206e 702e 7069 290a 2020 2020  nu * np.pi).    
+00003770: 2020 2020 696e 6e65 7220 3d20 2d28 6e75      inner = -(nu
+00003780: 202b 206b 2920 2f20 322e 3020 2a20 7074   + k) / 2.0 * pt
+00003790: 2e6c 6f67 3170 2871 7561 6464 6973 7420  .log1p(quaddist 
+000037a0: 2f20 6e75 290a 2020 2020 2020 2020 7265  / nu).        re
+000037b0: 7320 3d20 6e6f 726d 202b 2069 6e6e 6572  s = norm + inner
+000037c0: 202d 206c 6f67 6465 740a 0a20 2020 2020   - logdet..     
+000037d0: 2020 2072 6574 7572 6e20 6368 6563 6b5f     return check_
+000037e0: 7061 7261 6d65 7465 7273 2872 6573 2c20  parameters(res, 
+000037f0: 6f6b 2c20 6e75 203e 2030 2c20 6d73 673d  ok, nu > 0, msg=
+00003800: 2270 6f73 6465 662c 206e 7520 3e20 3022  "posdef, nu > 0"
+00003810: 290a 0a0a 636c 6173 7320 4469 7269 6368  )...class Dirich
+00003820: 6c65 7428 5369 6d70 6c65 7843 6f6e 7469  let(SimplexConti
+00003830: 6e75 6f75 7329 3a0a 2020 2020 7222 2222  nuous):.    r"""
+00003840: 0a20 2020 2044 6972 6963 686c 6574 206c  .    Dirichlet l
+00003850: 6f67 2d6c 696b 656c 6968 6f6f 642e 0a0a  og-likelihood...
+00003860: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
+00003870: 2020 2020 2020 6628 5c6d 6174 6862 667b        f(\mathbf{
+00003880: 787d 7c5c 6d61 7468 6266 7b61 7d29 203d  x}|\mathbf{a}) =
+00003890: 0a20 2020 2020 2020 2020 2020 5c66 7261  .           \fra
+000038a0: 637b 5c47 616d 6d61 285c 7375 6d5f 7b69  c{\Gamma(\sum_{i
+000038b0: 3d31 7d5e 6b20 615f 6929 7d7b 5c70 726f  =1}^k a_i)}{\pro
+000038c0: 645f 7b69 3d31 7d5e 6b20 5c47 616d 6d61  d_{i=1}^k \Gamma
+000038d0: 2861 5f69 297d 0a20 2020 2020 2020 2020  (a_i)}.         
+000038e0: 2020 5c70 726f 645f 7b69 3d31 7d5e 6b20    \prod_{i=1}^k 
+000038f0: 785f 695e 7b61 5f69 202d 2031 7d0a 0a20  x_i^{a_i - 1}.. 
+00003900: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
+00003910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
+00003940: 2053 7570 706f 7274 2020 203a 6d61 7468   Support   :math
+00003950: 3a60 785f 6920 5c69 6e20 2830 2c20 3129  :`x_i \in (0, 1)
+00003960: 6020 666f 7220 3a6d 6174 683a 6069 205c  ` for :math:`i \
+00003970: 696e 205c 7b31 2c20 5c6c 646f 7473 2c20  in \{1, \ldots, 
+00003980: 4b5c 7d60 0a20 2020 2020 2020 2020 2020  K\}`.           
+00003990: 2020 2073 7563 6820 7468 6174 203a 6d61     such that :ma
+000039a0: 7468 3a60 5c73 756d 2078 5f69 203d 2031  th:`\sum x_i = 1
+000039b0: 600a 2020 2020 4d65 616e 2020 2020 2020  `.    Mean      
+000039c0: 3a6d 6174 683a 605c 6466 7261 637b 615f  :math:`\dfrac{a_
+000039d0: 697d 7b5c 7375 6d20 615f 697d 600a 2020  i}{\sum a_i}`.  
+000039e0: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
+000039f0: 683a 605c 6466 7261 637b 615f 6920 2d20  h:`\dfrac{a_i - 
+00003a00: 5c73 756d 2061 5f30 7d7b 615f 305e 3220  \sum a_0}{a_0^2 
+00003a10: 2861 5f30 202b 2031 297d 600a 2020 2020  (a_0 + 1)}`.    
+00003a20: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+00003a30: 3a6d 6174 683a 6061 5f30 203d 205c 7375  :math:`a_0 = \su
+00003a40: 6d20 615f 6960 0a20 2020 203d 3d3d 3d3d  m a_i`.    =====
+00003a50: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00003a60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003a70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003a80: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
+00003a90: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00003aa0: 2d2d 2d0a 2020 2020 6120 3a20 7465 6e73  ---.    a : tens
+00003ab0: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+00003ac0: 0a20 2020 2020 2020 2043 6f6e 6365 6e74  .        Concent
+00003ad0: 7261 7469 6f6e 2070 6172 616d 6574 6572  ration parameter
+00003ae0: 7320 2861 203e 2030 292e 2054 6865 206e  s (a > 0). The n
+00003af0: 756d 6265 7220 6f66 2063 6174 6567 6f72  umber of categor
+00003b00: 6965 7320 6973 2067 6976 656e 2062 7920  ies is given by 
+00003b10: 7468 650a 2020 2020 2020 2020 6c65 6e67  the.        leng
+00003b20: 7468 206f 6620 7468 6520 6c61 7374 2061  th of the last a
+00003b30: 7869 732e 0a20 2020 2022 2222 0a20 2020  xis..    """.   
+00003b40: 2072 765f 6f70 203d 2064 6972 6963 686c   rv_op = dirichl
+00003b50: 6574 0a0a 2020 2020 4063 6c61 7373 6d65  et..    @classme
+00003b60: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
+00003b70: 7428 636c 732c 2061 2c20 2a2a 6b77 6172  t(cls, a, **kwar
+00003b80: 6773 293a 0a20 2020 2020 2020 2061 203d  gs):.        a =
+00003b90: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+00003ba0: 7269 6162 6c65 2861 290a 2020 2020 2020  riable(a).      
+00003bb0: 2020 2320 6d65 616e 203d 2061 202f 2070    # mean = a / p
+00003bc0: 742e 7375 6d28 6129 0a20 2020 2020 2020  t.sum(a).       
+00003bd0: 2023 206d 6f64 6520 3d20 7074 2e73 7769   # mode = pt.swi
+00003be0: 7463 6828 7074 2e61 6c6c 2861 203e 2031  tch(pt.all(a > 1
+00003bf0: 292c 2028 6120 2d20 3129 202f 2070 742e  ), (a - 1) / pt.
+00003c00: 7375 6d28 6120 2d20 3129 2c20 6e70 2e6e  sum(a - 1), np.n
+00003c10: 616e 290a 0a20 2020 2020 2020 2072 6574  an)..        ret
+00003c20: 7572 6e20 7375 7065 7228 292e 6469 7374  urn super().dist
+00003c30: 285b 615d 2c20 2a2a 6b77 6172 6773 290a  ([a], **kwargs).
+00003c40: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
+00003c50: 7276 2c20 7369 7a65 2c20 6129 3a0a 2020  rv, size, a):.  
+00003c60: 2020 2020 2020 6e6f 726d 5f63 6f6e 7374        norm_const
+00003c70: 616e 7420 3d20 7074 2e73 756d 2861 2c20  ant = pt.sum(a, 
+00003c80: 6178 6973 3d2d 3129 5b2e 2e2e 2c20 4e6f  axis=-1)[..., No
+00003c90: 6e65 5d0a 2020 2020 2020 2020 6d6f 6d65  ne].        mome
+00003ca0: 6e74 203d 2061 202f 206e 6f72 6d5f 636f  nt = a / norm_co
+00003cb0: 6e73 7461 6e74 0a20 2020 2020 2020 2069  nstant.        i
+00003cc0: 6620 6e6f 7420 7276 5f73 697a 655f 6973  f not rv_size_is
+00003cd0: 5f6e 6f6e 6528 7369 7a65 293a 0a20 2020  _none(size):.   
+00003ce0: 2020 2020 2020 2020 206d 6f6d 656e 7420           moment 
+00003cf0: 3d20 7074 2e66 756c 6c28 7074 2e63 6f6e  = pt.full(pt.con
+00003d00: 6361 7465 6e61 7465 285b 7369 7a65 2c20  catenate([size, 
+00003d10: 5b61 2e73 6861 7065 5b2d 315d 5d5d 292c  [a.shape[-1]]]),
+00003d20: 206d 6f6d 656e 7429 0a20 2020 2020 2020   moment).       
+00003d30: 2072 6574 7572 6e20 6d6f 6d65 6e74 0a0a   return moment..
+00003d40: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
+00003d50: 7565 2c20 6129 3a0a 2020 2020 2020 2020  ue, a):.        
+00003d60: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
+00003d70: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
+00003d80: 696c 6974 7920 6f66 2044 6972 6963 686c  ility of Dirichl
+00003d90: 6574 2064 6973 7472 6962 7574 696f 6e0a  et distribution.
+00003da0: 2020 2020 2020 2020 6174 2073 7065 6369          at speci
+00003db0: 6669 6564 2076 616c 7565 2e0a 0a20 2020  fied value...   
+00003dc0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00003dd0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00003de0: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
+00003df0: 3a20 6e75 6d65 7269 630a 2020 2020 2020  : numeric.      
+00003e00: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
+00003e10: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
+00003e20: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
+00003e30: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
+00003e40: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00003e50: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
+00003e60: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
+00003e70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003e80: 2023 206f 6e6c 7920 6465 6669 6e65 6420   # only defined 
+00003e90: 666f 7220 7375 6d28 7661 6c75 6529 203d  for sum(value) =
+00003ea0: 3d20 310a 2020 2020 2020 2020 7265 7320  = 1.        res 
+00003eb0: 3d20 7074 2e73 756d 286c 6f67 706f 7728  = pt.sum(logpow(
+00003ec0: 7661 6c75 652c 2061 202d 2031 2920 2d20  value, a - 1) - 
+00003ed0: 6761 6d6d 616c 6e28 6129 2c20 6178 6973  gammaln(a), axis
+00003ee0: 3d2d 3129 202b 2067 616d 6d61 6c6e 2870  =-1) + gammaln(p
+00003ef0: 742e 7375 6d28 612c 2061 7869 733d 2d31  t.sum(a, axis=-1
+00003f00: 2929 0a20 2020 2020 2020 2072 6573 203d  )).        res =
+00003f10: 2070 742e 7377 6974 6368 280a 2020 2020   pt.switch(.    
+00003f20: 2020 2020 2020 2020 7074 2e6f 725f 280a          pt.or_(.
+00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f40: 7074 2e61 6e79 2870 742e 6c74 2876 616c  pt.any(pt.lt(val
+00003f50: 7565 2c20 3029 2c20 6178 6973 3d2d 3129  ue, 0), axis=-1)
+00003f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003f70: 2020 7074 2e61 6e79 2870 742e 6774 2876    pt.any(pt.gt(v
+00003f80: 616c 7565 2c20 3129 2c20 6178 6973 3d2d  alue, 1), axis=-
+00003f90: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
+00003fa0: 292c 0a20 2020 2020 2020 2020 2020 202d  ),.            -
+00003fb0: 6e70 2e69 6e66 2c0a 2020 2020 2020 2020  np.inf,.        
+00003fc0: 2020 2020 7265 732c 0a20 2020 2020 2020      res,.       
+00003fd0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+00003fe0: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
+00003ff0: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
+00004000: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+00004010: 2061 203e 2030 2c0a 2020 2020 2020 2020   a > 0,.        
+00004020: 2020 2020 6d73 673d 2261 203e 2030 222c      msg="a > 0",
+00004030: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00004040: 7373 204d 756c 7469 6e6f 6d69 616c 2844  ss Multinomial(D
+00004050: 6973 6372 6574 6529 3a0a 2020 2020 7222  iscrete):.    r"
+00004060: 2222 0a20 2020 204d 756c 7469 6e6f 6d69  "".    Multinomi
+00004070: 616c 206c 6f67 2d6c 696b 656c 6968 6f6f  al log-likelihoo
+00004080: 642e 0a0a 2020 2020 4765 6e65 7261 6c69  d...    Generali
+00004090: 7a65 7320 6269 6e6f 6d69 616c 2064 6973  zes binomial dis
+000040a0: 7472 6962 7574 696f 6e2c 2062 7574 2069  tribution, but i
+000040b0: 6e73 7465 6164 206f 6620 6561 6368 2074  nstead of each t
+000040c0: 7269 616c 2072 6573 756c 7469 6e67 0a20  rial resulting. 
+000040d0: 2020 2069 6e20 2273 7563 6365 7373 2220     in "success" 
+000040e0: 6f72 2022 6661 696c 7572 6522 2c20 6561  or "failure", ea
+000040f0: 6368 206f 6e65 2072 6573 756c 7473 2069  ch one results i
+00004100: 6e20 6578 6163 746c 7920 6f6e 6520 6f66  n exactly one of
+00004110: 2073 6f6d 650a 2020 2020 6669 7865 6420   some.    fixed 
+00004120: 6669 6e69 7465 206e 756d 6265 7220 6b20  finite number k 
+00004130: 6f66 2070 6f73 7369 626c 6520 6f75 7463  of possible outc
+00004140: 6f6d 6573 206f 7665 7220 6e20 696e 6465  omes over n inde
+00004150: 7065 6e64 656e 7420 7472 6961 6c73 2e0a  pendent trials..
+00004160: 2020 2020 2778 5b69 5d27 2069 6e64 6963      'x[i]' indic
+00004170: 6174 6573 2074 6865 206e 756d 6265 7220  ates the number 
+00004180: 6f66 2074 696d 6573 206f 7574 636f 6d65  of times outcome
+00004190: 206e 756d 6265 7220 6920 7761 7320 6f62   number i was ob
+000041a0: 7365 7276 6564 0a20 2020 206f 7665 7220  served.    over 
+000041b0: 7468 6520 6e20 7472 6961 6c73 2e0a 0a20  the n trials... 
+000041c0: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
+000041d0: 2020 2020 2066 2878 205c 6d69 6420 6e2c       f(x \mid n,
+000041e0: 2070 2920 3d20 5c66 7261 637b 6e21 7d7b   p) = \frac{n!}{
+000041f0: 5c70 726f 645f 7b69 3d31 7d5e 6b20 785f  \prod_{i=1}^k x_
+00004200: 6921 7d20 5c70 726f 645f 7b69 3d31 7d5e  i!} \prod_{i=1}^
+00004210: 6b20 705f 695e 7b78 5f69 7d0a 0a20 2020  k p_i^{x_i}..   
+00004220: 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d   ==========  ===
+00004230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004250: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053 7570  ========.    Sup
+00004260: 706f 7274 2020 2020 203a 6d61 7468 3a60  port     :math:`
+00004270: 7820 5c69 6e20 5c7b 302c 2031 2c20 5c6c  x \in \{0, 1, \l
+00004280: 646f 7473 2c20 6e5c 7d60 2073 7563 6820  dots, n\}` such 
+00004290: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
+000042a0: 2020 2020 203a 6d61 7468 3a60 5c73 756d       :math:`\sum
+000042b0: 2078 5f69 203d 206e 600a 2020 2020 4d65   x_i = n`.    Me
+000042c0: 616e 2020 2020 2020 2020 3a6d 6174 683a  an        :math:
+000042d0: 606e 2070 5f69 600a 2020 2020 5661 7269  `n p_i`.    Vari
+000042e0: 616e 6365 2020 2020 3a6d 6174 683a 606e  ance    :math:`n
+000042f0: 2070 5f69 2028 3120 2d20 705f 6929 600a   p_i (1 - p_i)`.
+00004300: 2020 2020 436f 7661 7269 616e 6365 2020      Covariance  
+00004310: 3a6d 6174 683a 602d 6e20 705f 6920 705f  :math:`-n p_i p_
+00004320: 6a60 2066 6f72 203a 6d61 7468 3a60 6920  j` for :math:`i 
+00004330: 5c6e 6520 6a60 0a20 2020 203d 3d3d 3d3d  \ne j`.    =====
+00004340: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
+00004350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004370: 3d3d 0a0a 2020 2020 5061 7261 6d65 7465  ==..    Paramete
+00004380: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00004390: 2d0a 2020 2020 6e20 3a20 7465 6e73 6f72  -.    n : tensor
+000043a0: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
+000043b0: 2020 2020 2054 6f74 616c 2063 6f75 6e74       Total count
+000043c0: 7320 696e 2065 6163 6820 7265 706c 6963  s in each replic
+000043d0: 6174 6520 286e 203e 2030 292e 0a20 2020  ate (n > 0)..   
+000043e0: 2070 203a 2074 656e 736f 725f 6c69 6b65   p : tensor_like
+000043f0: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
+00004400: 2020 5072 6f62 6162 696c 6974 7920 6f66    Probability of
+00004410: 2065 6163 6820 6f6e 6520 6f66 2074 6865   each one of the
+00004420: 2064 6966 6665 7265 6e74 206f 7574 636f   different outco
+00004430: 6d65 7320 2830 203c 3d20 7020 3c3d 2031  mes (0 <= p <= 1
+00004440: 292e 2054 6865 206e 756d 6265 7220 6f66  ). The number of
+00004450: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
+00004460: 6965 7320 6973 2067 6976 656e 2062 7920  ies is given by 
+00004470: 7468 6520 6c65 6e67 7468 206f 6620 7468  the length of th
+00004480: 6520 6c61 7374 2061 7869 732e 2045 6c65  e last axis. Ele
+00004490: 6d65 6e74 7320 6172 6520 6578 7065 6374  ments are expect
+000044a0: 6564 2074 6f20 7375 6d0a 2020 2020 2020  ed to sum.      
+000044b0: 2020 746f 2031 2061 6c6f 6e67 2074 6865    to 1 along the
+000044c0: 206c 6173 7420 6178 6973 2e0a 2020 2020   last axis..    
+000044d0: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
+000044e0: 6d75 6c74 696e 6f6d 6961 6c0a 0a20 2020  multinomial..   
+000044f0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00004500: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
+00004510: 6e2c 2070 2c20 2a61 7267 732c 202a 2a6b  n, p, *args, **k
+00004520: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00004530: 7020 3d20 7074 2e61 735f 7465 6e73 6f72  p = pt.as_tensor
+00004540: 5f76 6172 6961 626c 6528 7029 0a20 2020  _variable(p).   
+00004550: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00004560: 6365 2870 2c20 5465 6e73 6f72 436f 6e73  ce(p, TensorCons
+00004570: 7461 6e74 293a 0a20 2020 2020 2020 2020  tant):.         
+00004580: 2020 2070 5f20 3d20 6e70 2e61 7361 7272     p_ = np.asarr
+00004590: 6179 2870 2e64 6174 6129 0a20 2020 2020  ay(p.data).     
+000045a0: 2020 2020 2020 2069 6620 6e70 2e61 6e79         if np.any
+000045b0: 2870 5f20 3c20 3029 3a0a 2020 2020 2020  (p_ < 0):.      
+000045c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000045d0: 5661 6c75 6545 7272 6f72 2866 224e 6567  ValueError(f"Neg
+000045e0: 6174 6976 6520 6070 6020 7061 7261 6d65  ative `p` parame
+000045f0: 7465 7273 2061 7265 206e 6f74 2076 616c  ters are not val
+00004600: 6964 2c20 676f 743a 207b 705f 7d22 290a  id, got: {p_}").
+00004610: 2020 2020 2020 2020 2020 2020 705f 7375              p_su
+00004620: 6d5f 203d 206e 702e 7375 6d28 5b70 5f5d  m_ = np.sum([p_]
+00004630: 2c20 6178 6973 3d2d 3129 0a20 2020 2020  , axis=-1).     
+00004640: 2020 2020 2020 2069 6620 6e6f 7420 6e70         if not np
+00004650: 2e61 6c6c 286e 702e 6973 636c 6f73 6528  .all(np.isclose(
+00004660: 705f 7375 6d5f 2c20 312e 3029 293a 0a20  p_sum_, 1.0)):. 
+00004670: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00004680: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 6622 6070 6020 7061 7261 6d65 7465    f"`p` paramete
+000046b0: 7273 2073 756d 2074 6f20 7b70 5f73 756d  rs sum to {p_sum
+000046c0: 5f7d 2c20 696e 7374 6561 6420 6f66 2031  _}, instead of 1
+000046d0: 2e30 2e20 220a 2020 2020 2020 2020 2020  .0. ".          
+000046e0: 2020 2020 2020 2020 2020 2254 6865 7920            "They 
+000046f0: 7769 6c6c 2062 6520 6175 746f 6d61 7469  will be automati
+00004700: 6361 6c6c 7920 7265 7363 616c 6564 2e20  cally rescaled. 
+00004710: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004720: 2020 2020 2020 2259 6f75 2063 616e 2072        "You can r
+00004730: 6573 6361 6c65 2074 6865 6d20 6469 7265  escale them dire
+00004740: 6374 6c79 2074 6f20 6765 7420 7269 6420  ctly to get rid 
+00004750: 6f66 2074 6869 7320 7761 726e 696e 672e  of this warning.
+00004760: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00004770: 2020 2020 2020 2055 7365 7257 6172 6e69         UserWarni
+00004780: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+00004790: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000047a0: 2020 2020 2020 705f 203d 2070 5f20 2f20        p_ = p_ / 
+000047b0: 7074 2e73 756d 2870 5f2c 2061 7869 733d  pt.sum(p_, axis=
+000047c0: 2d31 2c20 6b65 6570 6469 6d73 3d54 7275  -1, keepdims=Tru
+000047d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000047e0: 2020 2070 203d 2070 742e 6173 5f74 656e     p = pt.as_ten
+000047f0: 736f 725f 7661 7269 6162 6c65 2870 5f29  sor_variable(p_)
+00004800: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
+00004810: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00004820: 6c65 286e 290a 2020 2020 2020 2020 7020  le(n).        p 
+00004830: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00004840: 6172 6961 626c 6528 7029 0a20 2020 2020  ariable(p).     
+00004850: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00004860: 292e 6469 7374 285b 6e2c 2070 5d2c 202a  ).dist([n, p], *
+00004870: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+00004880: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
+00004890: 7276 2c20 7369 7a65 2c20 6e2c 2070 293a  rv, size, n, p):
+000048a0: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
+000048b0: 7368 6170 655f 7061 6472 6967 6874 286e  shape_padright(n
+000048c0: 290a 2020 2020 2020 2020 6d6f 6465 203d  ).        mode =
+000048d0: 2070 742e 726f 756e 6428 6e20 2a20 7029   pt.round(n * p)
+000048e0: 0a20 2020 2020 2020 2064 6966 6620 3d20  .        diff = 
+000048f0: 6e20 2d20 7074 2e73 756d 286d 6f64 652c  n - pt.sum(mode,
+00004900: 2061 7869 733d 2d31 2c20 6b65 6570 6469   axis=-1, keepdi
+00004910: 6d73 3d54 7275 6529 0a20 2020 2020 2020  ms=True).       
+00004920: 2069 6e63 5f62 6f6f 6c5f 6172 7220 3d20   inc_bool_arr = 
+00004930: 7074 2e61 6273 2864 6966 6629 203e 2030  pt.abs(diff) > 0
+00004940: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
+00004950: 7074 2e69 6e63 5f73 7562 7465 6e73 6f72  pt.inc_subtensor
+00004960: 286d 6f64 655b 696e 635f 626f 6f6c 5f61  (mode[inc_bool_a
+00004970: 7272 2e6e 6f6e 7a65 726f 2829 5d2c 2064  rr.nonzero()], d
+00004980: 6966 665b 696e 635f 626f 6f6c 5f61 7272  iff[inc_bool_arr
+00004990: 2e6e 6f6e 7a65 726f 2829 5d29 0a20 2020  .nonzero()]).   
+000049a0: 2020 2020 2069 6620 6e6f 7420 7276 5f73       if not rv_s
+000049b0: 697a 655f 6973 5f6e 6f6e 6528 7369 7a65  ize_is_none(size
+000049c0: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+000049d0: 7574 7075 745f 7369 7a65 203d 2070 742e  utput_size = pt.
+000049e0: 636f 6e63 6174 656e 6174 6528 5b73 697a  concatenate([siz
+000049f0: 652c 205b 702e 7368 6170 655b 2d31 5d5d  e, [p.shape[-1]]
+00004a00: 5d29 0a20 2020 2020 2020 2020 2020 206d  ]).            m
+00004a10: 6f64 6520 3d20 7074 2e66 756c 6c28 6f75  ode = pt.full(ou
+00004a20: 7470 7574 5f73 697a 652c 206d 6f64 6529  tput_size, mode)
+00004a30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004a40: 6d6f 6465 0a0a 2020 2020 6465 6620 6c6f  mode..    def lo
+00004a50: 6770 2876 616c 7565 2c20 6e2c 2070 293a  gp(value, n, p):
+00004a60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004a70: 2020 2020 2043 616c 6375 6c61 7465 206c       Calculate l
+00004a80: 6f67 2d70 726f 6261 6269 6c69 7479 206f  og-probability o
+00004a90: 6620 4d75 6c74 696e 6f6d 6961 6c20 6469  f Multinomial di
+00004aa0: 7374 7269 6275 7469 6f6e 0a20 2020 2020  stribution.     
+00004ab0: 2020 2061 7420 7370 6563 6966 6965 6420     at specified 
+00004ac0: 7661 6c75 652e 0a0a 2020 2020 2020 2020  value...        
+00004ad0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00004ae0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00004af0: 2020 2020 2020 7661 6c75 653a 206e 756d        value: num
+00004b00: 6572 6963 0a20 2020 2020 2020 2020 2020  eric.           
+00004b10: 2056 616c 7565 2066 6f72 2077 6869 6368   Value for which
+00004b20: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
+00004b30: 2069 7320 6361 6c63 756c 6174 6564 2e0a   is calculated..
+00004b40: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00004b50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00004b60: 0a20 2020 2020 2020 2054 656e 736f 7256  .        TensorV
+00004b70: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
+00004b80: 2222 220a 0a20 2020 2020 2020 2072 6573  """..        res
+00004b90: 203d 2066 6163 746c 6e28 6e29 202b 2070   = factln(n) + p
+00004ba0: 742e 7375 6d28 2d66 6163 746c 6e28 7661  t.sum(-factln(va
+00004bb0: 6c75 6529 202b 206c 6f67 706f 7728 702c  lue) + logpow(p,
+00004bc0: 2076 616c 7565 292c 2061 7869 733d 2d31   value), axis=-1
+00004bd0: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
+00004be0: 7074 2e73 7769 7463 6828 0a20 2020 2020  pt.switch(.     
+00004bf0: 2020 2020 2020 2070 742e 6f72 5f28 7074         pt.or_(pt
+00004c00: 2e61 6e79 2870 742e 6c74 2876 616c 7565  .any(pt.lt(value
+00004c10: 2c20 3029 2c20 6178 6973 3d2d 3129 2c20  , 0), axis=-1), 
+00004c20: 7074 2e6e 6571 2870 742e 7375 6d28 7661  pt.neq(pt.sum(va
+00004c30: 6c75 652c 2061 7869 733d 2d31 292c 206e  lue, axis=-1), n
+00004c40: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00004c50: 2d6e 702e 696e 662c 0a20 2020 2020 2020  -np.inf,.       
+00004c60: 2020 2020 2072 6573 2c0a 2020 2020 2020       res,.      
+00004c70: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+00004c80: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
+00004c90: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
+00004ca0: 2072 6573 2c0a 2020 2020 2020 2020 2020   res,.          
+00004cb0: 2020 3020 3c3d 2070 2c0a 2020 2020 2020    0 <= p,.      
+00004cc0: 2020 2020 2020 7020 3c3d 2031 2c0a 2020        p <= 1,.  
+00004cd0: 2020 2020 2020 2020 2020 7074 2e69 7363            pt.isc
+00004ce0: 6c6f 7365 2870 742e 7375 6d28 702c 2061  lose(pt.sum(p, a
+00004cf0: 7869 733d 2d31 292c 2031 292c 0a20 2020  xis=-1), 1),.   
+00004d00: 2020 2020 2020 2020 2070 742e 6765 286e           pt.ge(n
+00004d10: 2c20 3029 2c0a 2020 2020 2020 2020 2020  , 0),.          
+00004d20: 2020 6d73 673d 2230 203c 3d20 7020 3c3d    msg="0 <= p <=
+00004d30: 2031 2c20 7375 6d28 7029 203d 2031 2c20   1, sum(p) = 1, 
+00004d40: 6e20 3e3d 2030 222c 0a20 2020 2020 2020  n >= 0",.       
+00004d50: 2029 0a0a 0a63 6c61 7373 2044 6972 6963   )...class Diric
+00004d60: 686c 6574 4d75 6c74 696e 6f6d 6961 6c52  hletMultinomialR
+00004d70: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
+00004d80: 293a 0a20 2020 206e 616d 6520 3d20 2264  ):.    name = "d
+00004d90: 6972 6963 686c 6574 5f6d 756c 7469 6e6f  irichlet_multino
+00004da0: 6d69 616c 220a 2020 2020 6e64 696d 5f73  mial".    ndim_s
+00004db0: 7570 7020 3d20 310a 2020 2020 6e64 696d  upp = 1.    ndim
+00004dc0: 735f 7061 7261 6d73 203d 205b 302c 2031  s_params = [0, 1
+00004dd0: 5d0a 2020 2020 6474 7970 6520 3d20 2269  ].    dtype = "i
+00004de0: 6e74 3634 220a 2020 2020 5f70 7269 6e74  nt64".    _print
+00004df0: 5f6e 616d 6520 3d20 2822 4469 7269 6368  _name = ("Dirich
+00004e00: 6c65 744d 4e22 2c20 225c 5c6f 7065 7261  letMN", "\\opera
+00004e10: 746f 726e 616d 657b 4469 7269 6368 6c65  torname{Dirichle
+00004e20: 744d 4e7d 2229 0a0a 2020 2020 6465 6620  tMN}")..    def 
+00004e30: 5f73 7570 705f 7368 6170 655f 6672 6f6d  _supp_shape_from
+00004e40: 5f70 6172 616d 7328 7365 6c66 2c20 6469  _params(self, di
+00004e50: 7374 5f70 6172 616d 732c 2072 6570 5f70  st_params, rep_p
+00004e60: 6172 616d 5f69 6478 3d31 2c20 7061 7261  aram_idx=1, para
+00004e70: 6d5f 7368 6170 6573 3d4e 6f6e 6529 3a0a  m_shapes=None):.
+00004e80: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00004e90: 6566 6175 6c74 5f73 7570 705f 7368 6170  efault_supp_shap
+00004ea0: 655f 6672 6f6d 5f70 6172 616d 7328 0a20  e_from_params(. 
+00004eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004ec0: 6e64 696d 5f73 7570 702c 2064 6973 745f  ndim_supp, dist_
+00004ed0: 7061 7261 6d73 2c20 7265 705f 7061 7261  params, rep_para
+00004ee0: 6d5f 6964 782c 2070 6172 616d 5f73 6861  m_idx, param_sha
+00004ef0: 7065 730a 2020 2020 2020 2020 290a 0a20  pes.        ).. 
+00004f00: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00004f10: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+00004f20: 6c73 2c20 726e 672c 206e 2c20 612c 2073  ls, rng, n, a, s
+00004f30: 697a 6529 3a0a 2020 2020 2020 2020 6966  ize):.        if
+00004f40: 206e 2e6e 6469 6d20 3e20 3020 6f72 2061   n.ndim > 0 or a
+00004f50: 2e6e 6469 6d20 3e20 313a 0a20 2020 2020  .ndim > 1:.     
+00004f60: 2020 2020 2020 206e 2c20 6120 3d20 6272         n, a = br
+00004f70: 6f61 6463 6173 745f 7061 7261 6d73 285b  oadcast_params([
+00004f80: 6e2c 2061 5d2c 2063 6c73 2e6e 6469 6d73  n, a], cls.ndims
+00004f90: 5f70 6172 616d 7329 0a20 2020 2020 2020  _params).       
+00004fa0: 2020 2020 2073 697a 6520 3d20 7475 706c       size = tupl
+00004fb0: 6528 7369 7a65 206f 7220 2829 290a 0a20  e(size or ()).. 
+00004fc0: 2020 2020 2020 2020 2020 2069 6620 7369             if si
+00004fd0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+00004fe0: 2020 2020 6e20 3d20 6e70 2e62 726f 6164      n = np.broad
+00004ff0: 6361 7374 5f74 6f28 6e2c 2073 697a 6529  cast_to(n, size)
+00005000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005010: 2061 203d 206e 702e 6272 6f61 6463 6173   a = np.broadcas
+00005020: 745f 746f 2861 2c20 7369 7a65 202b 2028  t_to(a, size + (
+00005030: 612e 7368 6170 655b 2d31 5d2c 2929 0a0a  a.shape[-1],))..
+00005040: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005050: 3d20 6e70 2e65 6d70 7479 2861 2e73 6861  = np.empty(a.sha
+00005060: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+00005070: 666f 7220 6964 7820 696e 206e 702e 6e64  for idx in np.nd
+00005080: 696e 6465 7828 612e 7368 6170 655b 3a2d  index(a.shape[:-
+00005090: 315d 293a 0a20 2020 2020 2020 2020 2020  1]):.           
+000050a0: 2020 2020 2070 203d 2072 6e67 2e64 6972       p = rng.dir
+000050b0: 6963 686c 6574 2861 5b69 6478 5d29 0a20  ichlet(a[idx]). 
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000050d0: 6573 5b69 6478 5d20 3d20 726e 672e 6d75  es[idx] = rng.mu
+000050e0: 6c74 696e 6f6d 6961 6c28 6e5b 6964 785d  ltinomial(n[idx]
+000050f0: 2c20 7029 0a20 2020 2020 2020 2020 2020  , p).           
+00005100: 2072 6574 7572 6e20 7265 730a 2020 2020   return res.    
+00005110: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005120: 2020 2020 2020 2320 6e20 6973 2061 2073        # n is a s
+00005130: 6361 6c61 722c 2061 2069 7320 6120 3164  calar, a is a 1d
+00005140: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
+00005150: 2020 2070 203d 2072 6e67 2e64 6972 6963     p = rng.diric
+00005160: 686c 6574 2861 2c20 7369 7a65 3d73 697a  hlet(a, size=siz
+00005170: 6529 2020 2320 2873 697a 652c 2061 2e73  e)  # (size, a.s
+00005180: 6861 7065 290a 0a20 2020 2020 2020 2020  hape)..         
+00005190: 2020 2072 6573 203d 206e 702e 656d 7074     res = np.empt
+000051a0: 7928 702e 7368 6170 6529 0a20 2020 2020  y(p.shape).     
+000051b0: 2020 2020 2020 2066 6f72 2069 6478 2069         for idx i
+000051c0: 6e20 6e70 2e6e 6469 6e64 6578 2870 2e73  n np.ndindex(p.s
+000051d0: 6861 7065 5b3a 2d31 5d29 3a0a 2020 2020  hape[:-1]):.    
+000051e0: 2020 2020 2020 2020 2020 2020 7265 735b              res[
+000051f0: 6964 785d 203d 2072 6e67 2e6d 756c 7469  idx] = rng.multi
+00005200: 6e6f 6d69 616c 286e 2c20 705b 6964 785d  nomial(n, p[idx]
+00005210: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00005220: 6574 7572 6e20 7265 730a 0a0a 6469 7269  eturn res...diri
+00005230: 6368 6c65 745f 6d75 6c74 696e 6f6d 6961  chlet_multinomia
+00005240: 6c20 3d20 4469 7269 6368 6c65 744d 756c  l = DirichletMul
+00005250: 7469 6e6f 6d69 616c 5256 2829 0a0a 0a63  tinomialRV()...c
+00005260: 6c61 7373 2044 6972 6963 686c 6574 4d75  lass DirichletMu
+00005270: 6c74 696e 6f6d 6961 6c28 4469 7363 7265  ltinomial(Discre
+00005280: 7465 293a 0a20 2020 2072 2222 2244 6972  te):.    r"""Dir
+00005290: 6963 686c 6574 204d 756c 7469 6e6f 6d69  ichlet Multinomi
+000052a0: 616c 206c 6f67 2d6c 696b 656c 6968 6f6f  al log-likelihoo
+000052b0: 642e 0a0a 2020 2020 4469 7269 6368 6c65  d...    Dirichle
+000052c0: 7420 6d69 7874 7572 6520 6f66 204d 756c  t mixture of Mul
+000052d0: 7469 6e6f 6d69 616c 7320 6469 7374 7269  tinomials distri
+000052e0: 6275 7469 6f6e 2c20 7769 7468 2061 206d  bution, with a m
+000052f0: 6172 6769 6e61 6c69 7a65 6420 504d 462e  arginalized PMF.
+00005300: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
+00005310: 0a20 2020 2020 2020 2066 2878 205c 6d69  .        f(x \mi
+00005320: 6420 6e2c 2061 2920 3d20 5c66 7261 637b  d n, a) = \frac{
+00005330: 5c47 616d 6d61 286e 202b 2031 295c 4761  \Gamma(n + 1)\Ga
+00005340: 6d6d 6128 5c73 756d 2061 5f6b 297d 0a20  mma(\sum a_k)}. 
+00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005360: 2020 2020 2020 2020 2020 2020 207b 5c47               {\G
+00005370: 616d 6d61 286e 202b 205c 7375 6d20 615f  amma(n + \sum a_
+00005380: 6b29 7d0a 2020 2020 2020 2020 2020 2020  k)}.            
+00005390: 2020 2020 2020 2020 2020 2020 205c 7072               \pr
+000053a0: 6f64 5f7b 6b3d 317d 5e4b 0a20 2020 2020  od_{k=1}^K.     
+000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053c0: 2020 2020 5c66 7261 637b 5c47 616d 6d61      \frac{\Gamma
+000053d0: 2878 5f6b 202b 2020 615f 6b29 7d0a 2020  (x_k +  a_k)}.  
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053f0: 2020 2020 2020 2020 2020 2020 7b5c 4761              {\Ga
+00005400: 6d6d 6128 785f 6b20 2b20 3129 5c47 616d  mma(x_k + 1)\Gam
+00005410: 6d61 2861 5f6b 297d 0a0a 2020 2020 3d3d  ma(a_k)}..    ==
+00005420: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
+00005430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005450: 3d3d 3d3d 3d0a 2020 2020 5375 7070 6f72  =====.    Suppor
+00005460: 7420 2020 2020 3a6d 6174 683a 6078 205c  t     :math:`x \
+00005470: 696e 205c 7b30 2c20 312c 205c 6c64 6f74  in \{0, 1, \ldot
+00005480: 732c 206e 5c7d 6020 7375 6368 2074 6861  s, n\}` such tha
+00005490: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000054a0: 2020 3a6d 6174 683a 605c 7375 6d20 785f    :math:`\sum x_
+000054b0: 6920 3d20 6e60 0a20 2020 204d 6561 6e20  i = n`.    Mean 
+000054c0: 2020 2020 2020 203a 6d61 7468 3a60 6e20         :math:`n 
+000054d0: 5c66 7261 637b 615f 697d 7b5c 7375 6d7b  \frac{a_i}{\sum{
+000054e0: 615f 6b7d 7d60 0a20 2020 203d 3d3d 3d3d  a_k}}`.    =====
+000054f0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
+00005500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005520: 3d3d 0a0a 2020 2020 5061 7261 6d65 7465  ==..    Paramete
+00005530: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00005540: 2d0a 2020 2020 6e20 3a20 7465 6e73 6f72  -.    n : tensor
+00005550: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
+00005560: 2020 2020 2054 6f74 616c 2063 6f75 6e74       Total count
+00005570: 7320 696e 2065 6163 6820 7265 706c 6963  s in each replic
+00005580: 6174 6520 286e 203e 2030 292e 0a0a 2020  ate (n > 0)...  
+00005590: 2020 6120 3a20 7465 6e73 6f72 5f6c 696b    a : tensor_lik
+000055a0: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
+000055b0: 2020 2044 6972 6963 686c 6574 2063 6f6e     Dirichlet con
+000055c0: 6365 6e74 7261 7469 6f6e 2070 6172 616d  centration param
+000055d0: 6574 6572 7320 2861 203e 2030 292e 2054  eters (a > 0). T
+000055e0: 6865 206e 756d 6265 7220 6f66 2063 6174  he number of cat
+000055f0: 6567 6f72 6965 7320 6973 2067 6976 656e  egories is given
+00005600: 2062 790a 2020 2020 2020 2020 7468 6520   by.        the 
+00005610: 6c65 6e67 7468 206f 6620 7468 6520 6c61  length of the la
+00005620: 7374 2061 7869 732e 0a20 2020 2022 2222  st axis..    """
+00005630: 0a20 2020 2072 765f 6f70 203d 2064 6972  .    rv_op = dir
+00005640: 6963 686c 6574 5f6d 756c 7469 6e6f 6d69  ichlet_multinomi
+00005650: 616c 0a0a 2020 2020 4063 6c61 7373 6d65  al..    @classme
+00005660: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
+00005670: 7428 636c 732c 206e 2c20 612c 202a 6172  t(cls, n, a, *ar
+00005680: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+00005690: 2020 2020 2020 206e 203d 2069 6e74 5828         n = intX(
+000056a0: 6e29 0a20 2020 2020 2020 2061 203d 2066  n).        a = f
+000056b0: 6c6f 6174 5828 6129 0a0a 2020 2020 2020  loatX(a)..      
+000056c0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000056d0: 2e64 6973 7428 5b6e 2c20 615d 2c20 2a2a  .dist([n, a], **
+000056e0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+000056f0: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+00005700: 2c20 6e2c 2061 293a 0a20 2020 2020 2020  , n, a):.       
+00005710: 2070 203d 2061 202f 2070 742e 7375 6d28   p = a / pt.sum(
+00005720: 612c 2061 7869 733d 2d31 2c20 6b65 6570  a, axis=-1, keep
+00005730: 6469 6d73 3d54 7275 6529 0a20 2020 2020  dims=True).     
+00005740: 2020 2072 6574 7572 6e20 6d6f 6d65 6e74     return moment
+00005750: 284d 756c 7469 6e6f 6d69 616c 2e64 6973  (Multinomial.dis
+00005760: 7428 6e3d 6e2c 2070 3d70 2c20 7369 7a65  t(n=n, p=p, size
+00005770: 3d73 697a 6529 290a 0a20 2020 2064 6566  =size))..    def
+00005780: 206c 6f67 7028 7661 6c75 652c 206e 2c20   logp(value, n, 
+00005790: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
+000057a0: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+000057b0: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
+000057c0: 7920 6f66 2044 6972 6963 686c 6574 4d75  y of DirichletMu
+000057d0: 6c74 696e 6f6d 6961 6c20 6469 7374 7269  ltinomial distri
+000057e0: 6275 7469 6f6e 0a20 2020 2020 2020 2061  bution.        a
+000057f0: 7420 7370 6563 6966 6965 6420 7661 6c75  t specified valu
+00005800: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+00005810: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00005820: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00005830: 2020 7661 6c75 653a 2069 6e74 6567 6572    value: integer
+00005840: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
+00005850: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
+00005860: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
+00005870: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
+00005880: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005890: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+000058a0: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
+000058b0: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
+000058c0: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
+000058d0: 6d5f 6120 3d20 612e 7375 6d28 6178 6973  m_a = a.sum(axis
+000058e0: 3d2d 3129 0a20 2020 2020 2020 2063 6f6e  =-1).        con
+000058f0: 7374 203d 2028 6761 6d6d 616c 6e28 6e20  st = (gammaln(n 
+00005900: 2b20 3129 202b 2067 616d 6d61 6c6e 2873  + 1) + gammaln(s
+00005910: 756d 5f61 2929 202d 2067 616d 6d61 6c6e  um_a)) - gammaln
+00005920: 286e 202b 2073 756d 5f61 290a 2020 2020  (n + sum_a).    
+00005930: 2020 2020 7365 7269 6573 203d 2067 616d      series = gam
+00005940: 6d61 6c6e 2876 616c 7565 202b 2061 2920  maln(value + a) 
+00005950: 2d20 2867 616d 6d61 6c6e 2876 616c 7565  - (gammaln(value
+00005960: 202b 2031 2920 2b20 6761 6d6d 616c 6e28   + 1) + gammaln(
+00005970: 6129 290a 2020 2020 2020 2020 7265 7320  a)).        res 
+00005980: 3d20 636f 6e73 7420 2b20 7365 7269 6573  = const + series
+00005990: 2e73 756d 2861 7869 733d 2d31 290a 0a20  .sum(axis=-1).. 
+000059a0: 2020 2020 2020 2072 6573 203d 2070 742e         res = pt.
+000059b0: 7377 6974 6368 280a 2020 2020 2020 2020  switch(.        
+000059c0: 2020 2020 7074 2e6f 725f 280a 2020 2020      pt.or_(.    
+000059d0: 2020 2020 2020 2020 2020 2020 7074 2e61              pt.a
+000059e0: 6e79 2870 742e 6c74 2876 616c 7565 2c20  ny(pt.lt(value, 
+000059f0: 3029 2c20 6178 6973 3d2d 3129 2c0a 2020  0), axis=-1),.  
+00005a00: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00005a10: 2e6e 6571 2870 742e 7375 6d28 7661 6c75  .neq(pt.sum(valu
+00005a20: 652c 2061 7869 733d 2d31 292c 206e 292c  e, axis=-1), n),
+00005a30: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00005a40: 2020 2020 2020 2020 2020 2020 2d6e 702e              -np.
+00005a50: 696e 662c 0a20 2020 2020 2020 2020 2020  inf,.           
+00005a60: 2072 6573 2c0a 2020 2020 2020 2020 290a   res,.        ).
+00005a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005a80: 6368 6563 6b5f 7061 7261 6d65 7465 7273  check_parameters
+00005a90: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00005aa0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
+00005ab0: 203e 2030 2c0a 2020 2020 2020 2020 2020   > 0,.          
+00005ac0: 2020 6e20 3e3d 2030 2c0a 2020 2020 2020    n >= 0,.      
+00005ad0: 2020 2020 2020 6d73 673d 2261 203e 2030        msg="a > 0
+00005ae0: 2c20 6e20 3e3d 2030 222c 0a20 2020 2020  , n >= 0",.     
+00005af0: 2020 2029 0a0a 0a63 6c61 7373 205f 4f72     )...class _Or
 00005b00: 6465 7265 644d 756c 7469 6e6f 6d69 616c  deredMultinomial
-00005b10: 2077 7261 7070 6572 2063 6c61 7373 2066   wrapper class f
-00005b20: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
-00005b30: 6f6e 2068 6f77 2074 6f20 7573 6520 6974  on how to use it
-00005b40: 2069 6e20 6d6f 6465 6c73 2e0a 2020 2020   in models..    
-00005b50: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-00005b60: 6d75 6c74 696e 6f6d 6961 6c0a 0a20 2020  multinomial..   
-00005b70: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00005b80: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
-00005b90: 6574 612c 2063 7574 706f 696e 7473 2c20  eta, cutpoints, 
-00005ba0: 6e2c 202a 6172 6773 2c20 2a2a 6b77 6172  n, *args, **kwar
-00005bb0: 6773 293a 0a20 2020 2020 2020 2065 7461  gs):.        eta
-00005bc0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-00005bd0: 7661 7269 6162 6c65 2866 6c6f 6174 5828  variable(floatX(
-00005be0: 6574 6129 290a 2020 2020 2020 2020 6375  eta)).        cu
-00005bf0: 7470 6f69 6e74 7320 3d20 7074 2e61 735f  tpoints = pt.as_
-00005c00: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-00005c10: 6375 7470 6f69 6e74 7329 0a20 2020 2020  cutpoints).     
-00005c20: 2020 206e 203d 2070 742e 6173 5f74 656e     n = pt.as_ten
-00005c30: 736f 725f 7661 7269 6162 6c65 2869 6e74  sor_variable(int
-00005c40: 5828 6e29 290a 0a20 2020 2020 2020 2070  X(n))..        p
-00005c50: 6120 3d20 7369 676d 6f69 6428 6375 7470  a = sigmoid(cutp
-00005c60: 6f69 6e74 7320 2d20 7074 2e73 6861 7065  oints - pt.shape
-00005c70: 5f70 6164 7269 6768 7428 6574 6129 290a  _padright(eta)).
-00005c80: 2020 2020 2020 2020 705f 6375 6d20 3d20          p_cum = 
-00005c90: 7074 2e63 6f6e 6361 7465 6e61 7465 280a  pt.concatenate(.
-00005ca0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 7074                pt
-00005cc0: 2e7a 6572 6f73 5f6c 696b 6528 7074 2e73  .zeros_like(pt.s
-00005cd0: 6861 7065 5f70 6164 7269 6768 7428 7061  hape_padright(pa
-00005ce0: 5b2e 2e2e 2c20 305d 2929 2c0a 2020 2020  [..., 0])),.    
-00005cf0: 2020 2020 2020 2020 2020 2020 7061 2c0a              pa,.
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 7074 2e6f 6e65 735f 6c69 6b65 2870 742e  pt.ones_like(pt.
-00005d20: 7368 6170 655f 7061 6472 6967 6874 2870  shape_padright(p
-00005d30: 615b 2e2e 2e2c 2030 5d29 292c 0a20 2020  a[..., 0])),.   
-00005d40: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00005d50: 2020 2020 2020 2020 6178 6973 3d2d 312c          axis=-1,
-00005d60: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005d70: 2020 2070 203d 2070 5f63 756d 5b2e 2e2e     p = p_cum[...
-00005d80: 2c20 313a 5d20 2d20 705f 6375 6d5b 2e2e  , 1:] - p_cum[..
-00005d90: 2e2c 203a 2d31 5d0a 0a20 2020 2020 2020  ., :-1]..       
-00005da0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00005db0: 6469 7374 286e 2c20 702c 202a 6172 6773  dist(n, p, *args
-00005dc0: 2c20 2a2a 6b77 6172 6773 290a 0a0a 636c  , **kwargs)...cl
-00005dd0: 6173 7320 4f72 6465 7265 644d 756c 7469  ass OrderedMulti
-00005de0: 6e6f 6d69 616c 3a0a 2020 2020 7222 2222  nomial:.    r"""
-00005df0: 0a20 2020 2057 7261 7070 6572 2063 6c61  .    Wrapper cla
-00005e00: 7373 2066 6f72 204f 7264 6572 6564 204d  ss for Ordered M
-00005e10: 756c 7469 6e6f 6d69 616c 2064 6973 7472  ultinomial distr
-00005e20: 6962 7574 696f 6e73 2e0a 0a20 2020 2055  ibutions...    U
-00005e30: 7365 6675 6c20 666f 7220 7265 6772 6573  seful for regres
-00005e40: 7369 6f6e 206f 6e20 6f72 6469 6e61 6c20  sion on ordinal 
-00005e50: 6461 7461 2077 686f 7365 2076 616c 7565  data whose value
-00005e60: 7320 7261 6e67 650a 2020 2020 6672 6f6d  s range.    from
-00005e70: 2031 2074 6f20 4b20 6173 2061 2066 756e   1 to K as a fun
-00005e80: 6374 696f 6e20 6f66 2073 6f6d 6520 7072  ction of some pr
-00005e90: 6564 6963 746f 722c 203a 6d61 7468 3a60  edictor, :math:`
-00005ea0: 5c65 7461 602c 2062 7574 0a20 2020 2020  \eta`, but.     
-00005eb0: 7768 6963 6820 6172 6520 5f61 6767 7265  which are _aggre
-00005ec0: 6761 7465 645f 2062 7920 7472 6961 6c2c  gated_ by trial,
-00005ed0: 206c 696b 6520 6d75 6c74 696e 6f6d 6961   like multinomia
-00005ee0: 6c20 6f62 7365 7276 6174 696f 6e73 2028  l observations (
-00005ef0: 696e 0a20 2020 2020 636f 6e74 7261 7374  in.     contrast
-00005f00: 2074 6f20 6070 6d2e 4f72 6465 7265 644c   to `pm.OrderedL
-00005f10: 6f67 6973 7469 6360 2c20 7768 6963 6820  ogistic`, which 
-00005f20: 6f6e 6c79 2061 6363 6570 7473 206f 7264  only accepts ord
-00005f30: 696e 616c 2064 6174 610a 2020 2020 2069  inal data.     i
-00005f40: 6e20 6120 5f64 6973 6167 6772 6567 6174  n a _disaggregat
-00005f50: 6564 5f20 666f 726d 6174 2c20 6c69 6b65  ed_ format, like
-00005f60: 2063 6174 6567 6f72 6963 616c 206f 6273   categorical obs
-00005f70: 6572 7661 7469 6f6e 7329 2e0a 2020 2020  ervations)..    
-00005f80: 2054 6865 2063 7574 706f 696e 7473 2c20   The cutpoints, 
-00005f90: 3a6d 6174 683a 6063 602c 2073 6570 6172  :math:`c`, separ
-00005fa0: 6174 6520 7768 6963 6820 7261 6e67 6573  ate which ranges
-00005fb0: 206f 6620 3a6d 6174 683a 605c 6574 6160   of :math:`\eta`
-00005fc0: 2061 7265 0a20 2020 206d 6170 7065 6420   are.    mapped 
-00005fd0: 746f 2077 6869 6368 206f 6620 7468 6520  to which of the 
-00005fe0: 4b20 6f62 7365 7276 6564 2064 6570 656e  K observed depen
-00005ff0: 6465 6e74 2076 6172 6961 626c 6573 2e20  dent variables. 
-00006000: 5468 6520 6e75 6d62 6572 0a20 2020 206f  The number.    o
-00006010: 6620 6375 7470 6f69 6e74 7320 6973 204b  f cutpoints is K
-00006020: 202d 2031 2e20 4974 2069 7320 7265 636f   - 1. It is reco
-00006030: 6d6d 656e 6465 6420 7468 6174 2074 6865  mmended that the
-00006040: 2063 7574 706f 696e 7473 2061 7265 0a20   cutpoints are. 
-00006050: 2020 2063 6f6e 7374 7261 696e 6564 2074     constrained t
-00006060: 6f20 6265 206f 7264 6572 6564 2e0a 0a20  o be ordered... 
-00006070: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-00006080: 2020 2020 2066 286b 205c 6d69 6420 5c65       f(k \mid \e
-00006090: 7461 2c20 6329 203d 205c 6c65 6674 5c7b  ta, c) = \left\{
-000060a0: 0a20 2020 2020 2020 2020 5c62 6567 696e  .         \begin
-000060b0: 7b61 7272 6179 7d7b 6c7d 0a20 2020 2020  {array}{l}.     
-000060c0: 2020 2020 2020 3120 2d20 5c74 6578 747b        1 - \text{
-000060d0: 6c6f 6769 747d 5e7b 2d31 7d28 5c65 7461  logit}^{-1}(\eta
-000060e0: 202d 2063 5f31 290a 2020 2020 2020 2020   - c_1).        
-000060f0: 2020 2020 205c 2c2c 205c 7465 7874 7b69       \,, \text{i
-00006100: 6620 7d20 6b20 3d20 3020 5c5c 0a20 2020  f } k = 0 \\.   
-00006110: 2020 2020 2020 2020 5c74 6578 747b 6c6f          \text{lo
-00006120: 6769 747d 5e7b 2d31 7d28 5c65 7461 202d  git}^{-1}(\eta -
-00006130: 2063 5f7b 6b20 2d20 317d 2920 2d0a 2020   c_{k - 1}) -.  
-00006140: 2020 2020 2020 2020 205c 7465 7874 7b6c           \text{l
-00006150: 6f67 6974 7d5e 7b2d 317d 285c 6574 6120  ogit}^{-1}(\eta 
-00006160: 2d20 635f 7b6b 7d29 0a20 2020 2020 2020  - c_{k}).       
-00006170: 2020 2020 2020 5c2c 2c20 5c74 6578 747b        \,, \text{
-00006180: 6966 207d 2030 203c 206b 203c 204b 205c  if } 0 < k < K \
-00006190: 5c0a 2020 2020 2020 2020 2020 205c 7465  \.           \te
-000061a0: 7874 7b6c 6f67 6974 7d5e 7b2d 317d 285c  xt{logit}^{-1}(\
-000061b0: 6574 6120 2d20 635f 7b4b 202d 2031 7d29  eta - c_{K - 1})
-000061c0: 0a20 2020 2020 2020 2020 2020 2020 5c2c  .             \,
-000061d0: 2c20 5c74 6578 747b 6966 207d 206b 203d  , \text{if } k =
-000061e0: 204b 205c 5c0a 2020 2020 2020 2020 205c   K \\.         \
-000061f0: 656e 647b 6172 7261 797d 0a20 2020 2020  end{array}.     
-00006200: 2020 5c72 6967 6874 2e0a 0a20 2020 2050    \right...    P
-00006210: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00006220: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065 7461  --------.    eta
-00006230: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-00006240: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
-00006250: 5468 6520 7072 6564 6963 746f 722e 0a20  The predictor.. 
-00006260: 2020 2063 7574 706f 696e 7473 203a 2074     cutpoints : t
-00006270: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-00006280: 6f61 740a 2020 2020 2020 2020 5468 6520  oat.        The 
-00006290: 6c65 6e67 7468 204b 202d 2031 2061 7272  length K - 1 arr
-000062a0: 6179 206f 6620 6375 7470 6f69 6e74 7320  ay of cutpoints 
-000062b0: 7768 6963 6820 6272 6561 6b20 3a6d 6174  which break :mat
-000062c0: 683a 605c 6574 6160 2069 6e74 6f0a 2020  h:`\eta` into.  
-000062d0: 2020 2020 2020 7261 6e67 6573 2e20 446f        ranges. Do
-000062e0: 206e 6f74 2065 7870 6c69 6369 746c 7920   not explicitly 
-000062f0: 7365 7420 7468 6520 6669 7273 7420 616e  set the first an
-00006300: 6420 6c61 7374 2065 6c65 6d65 6e74 7320  d last elements 
-00006310: 6f66 0a20 2020 2020 2020 203a 6d61 7468  of.        :math
-00006320: 3a60 6360 2074 6f20 6e65 6761 7469 7665  :`c` to negative
-00006330: 2061 6e64 2070 6f73 6974 6976 6520 696e   and positive in
-00006340: 6669 6e69 7479 2e0a 2020 2020 6e20 3a20  finity..    n : 
-00006350: 7465 6e73 6f72 5f6c 696b 6520 6f66 2069  tensor_like of i
-00006360: 6e74 0a20 2020 2020 2020 2054 6865 2074  nt.        The t
-00006370: 6f74 616c 206e 756d 6265 7220 6f66 206d  otal number of m
-00006380: 756c 7469 6e6f 6d69 616c 2074 7269 616c  ultinomial trial
-00006390: 732e 0a20 2020 2063 6f6d 7075 7465 5f70  s..    compute_p
-000063a0: 203a 2062 6f6f 6c65 616e 2c20 6465 6661   : boolean, defa
-000063b0: 756c 743d 5472 7565 0a20 2020 2020 2020  ult=True.       
-000063c0: 2057 6865 7468 6572 2074 6f20 636f 6d70   Whether to comp
-000063d0: 7574 6520 616e 6420 7374 6f72 6520 696e  ute and store in
-000063e0: 2074 6865 2074 7261 6365 2074 6865 2069   the trace the i
-000063f0: 6e66 6572 7265 6420 7072 6f62 6162 696c  nferred probabil
-00006400: 6974 6965 7320 6f66 2065 6163 680a 2020  ities of each.  
-00006410: 2020 2020 2020 6361 7465 676f 7269 6573        categories
-00006420: 2c0a 2020 2020 2020 2020 6261 7365 6420  ,.        based 
-00006430: 6f6e 2074 6865 2063 7574 706f 696e 7473  on the cutpoints
-00006440: 2720 7661 6c75 6573 2e20 4465 6661 756c  ' values. Defaul
-00006450: 7473 2074 6f20 5472 7565 2e0a 2020 2020  ts to True..    
-00006460: 2020 2020 4d69 6768 7420 6265 2075 7365      Might be use
-00006470: 6675 6c20 746f 2064 6973 6162 6c65 2069  ful to disable i
-00006480: 7420 6966 206d 656d 6f72 7920 7573 6167  t if memory usag
-00006490: 6520 6973 206f 6620 696e 7465 7265 7374  e is of interest
-000064a0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-000064b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-000064c0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-000064d0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
-000064e0: 2023 2047 656e 6572 6174 6520 6461 7461   # Generate data
-000064f0: 2066 6f72 2061 2073 696d 706c 6520 3120   for a simple 1 
-00006500: 6469 6d65 6e73 696f 6e61 6c20 6578 616d  dimensional exam
-00006510: 706c 6520 7072 6f62 6c65 6d0a 2020 2020  ple problem.    
-00006520: 2020 2020 7472 7565 5f63 756d 5f70 203d      true_cum_p =
-00006530: 206e 702e 6172 7261 7928 5b30 2e31 2c20   np.array([0.1, 
-00006540: 302e 3135 2c20 302e 3235 2c20 302e 3530  0.15, 0.25, 0.50
-00006550: 2c20 302e 3635 2c20 302e 3930 2c20 312e  , 0.65, 0.90, 1.
-00006560: 305d 290a 2020 2020 2020 2020 7472 7565  0]).        true
-00006570: 5f70 203d 206e 702e 6873 7461 636b 285b  _p = np.hstack([
-00006580: 7472 7565 5f63 756d 5f70 5b30 5d2c 2074  true_cum_p[0], t
-00006590: 7275 655f 6375 6d5f 705b 313a 5d20 2d20  rue_cum_p[1:] - 
-000065a0: 7472 7565 5f63 756d 5f70 5b3a 2d31 5d5d  true_cum_p[:-1]]
-000065b0: 290a 2020 2020 2020 2020 6661 6b65 5f65  ).        fake_e
-000065c0: 6c65 6374 696f 6e73 203d 206e 702e 7261  lections = np.ra
-000065d0: 6e64 6f6d 2e6d 756c 7469 6e6f 6d69 616c  ndom.multinomial
-000065e0: 286e 3d31 5f30 3030 2c20 7076 616c 733d  (n=1_000, pvals=
-000065f0: 7472 7565 5f70 2c20 7369 7a65 3d36 3029  true_p, size=60)
-00006600: 0a0a 2020 2020 2020 2020 2320 4f72 6465  ..        # Orde
-00006610: 7265 6420 6d75 6c74 696e 6f6d 6961 6c20  red multinomial 
-00006620: 7265 6772 6573 7369 6f6e 0a20 2020 2020  regression.     
-00006630: 2020 2077 6974 6820 706d 2e4d 6f64 656c     with pm.Model
-00006640: 2829 2061 7320 6d6f 6465 6c3a 0a20 2020  () as model:.   
-00006650: 2020 2020 2020 2020 2063 7574 706f 696e           cutpoin
-00006660: 7473 203d 2070 6d2e 4e6f 726d 616c 280a  ts = pm.Normal(.
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2263 7574 706f 696e 7473 222c 0a20 2020  "cutpoints",.   
-00006690: 2020 2020 2020 2020 2020 2020 206d 753d               mu=
-000066a0: 6e70 2e61 7261 6e67 6528 3629 202d 2032  np.arange(6) - 2
-000066b0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
-000066c0: 2020 2020 7369 676d 613d 312e 352c 0a20      sigma=1.5,. 
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000066e0: 6e69 7476 616c 3d6e 702e 6172 616e 6765  nitval=np.arange
-000066f0: 2836 2920 2d20 322e 352c 0a20 2020 2020  (6) - 2.5,.     
-00006700: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00006710: 666f 726d 3d70 6d2e 6469 7374 7269 6275  form=pm.distribu
-00006720: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
-00006730: 2e6f 7264 6572 6564 2c0a 2020 2020 2020  .ordered,.      
-00006740: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00006750: 2020 2020 2070 6d2e 4f72 6465 7265 644d       pm.OrderedM
-00006760: 756c 7469 6e6f 6d69 616c 280a 2020 2020  ultinomial(.    
-00006770: 2020 2020 2020 2020 2020 2020 2272 6573              "res
-00006780: 756c 7473 222c 0a20 2020 2020 2020 2020  ults",.         
-00006790: 2020 2020 2020 2065 7461 3d30 2e30 2c0a         eta=0.0,.
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 6375 7470 6f69 6e74 733d 6375 7470 6f69  cutpoints=cutpoi
-000067c0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
-000067d0: 2020 2020 206e 3d66 616b 655f 656c 6563       n=fake_elec
-000067e0: 7469 6f6e 732e 7375 6d28 3129 2c0a 2020  tions.sum(1),.  
-000067f0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
-00006800: 7365 7276 6564 3d66 616b 655f 656c 6563  served=fake_elec
-00006810: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00006820: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00006830: 2020 7472 6163 6520 3d20 706d 2e73 616d    trace = pm.sam
-00006840: 706c 6528 290a 0a20 2020 2020 2020 2023  ple()..        #
-00006850: 2050 6c6f 7420 7468 6520 7265 7375 6c74   Plot the result
-00006860: 730a 2020 2020 2020 2020 6172 7669 7a2e  s.        arviz.
-00006870: 706c 6f74 5f70 6f73 7465 7269 6f72 2874  plot_posterior(t
-00006880: 7261 6365 5f31 325f 342c 2076 6172 5f6e  race_12_4, var_n
-00006890: 616d 6573 3d5b 2263 6f6d 706c 6574 655f  ames=["complete_
-000068a0: 7022 5d2c 2072 6566 5f76 616c 3d6c 6973  p"], ref_val=lis
-000068b0: 7428 7472 7565 5f70 2929 3b0a 2020 2020  t(true_p));.    
-000068c0: 2222 220a 0a20 2020 2064 6566 205f 5f6e  """..    def __n
-000068d0: 6577 5f5f 2863 6c73 2c20 6e61 6d65 2c20  ew__(cls, name, 
-000068e0: 2a61 7267 732c 2063 6f6d 7075 7465 5f70  *args, compute_p
-000068f0: 3d54 7275 652c 202a 2a6b 7761 7267 7329  =True, **kwargs)
-00006900: 3a0a 2020 2020 2020 2020 6f75 745f 7276  :.        out_rv
-00006910: 203d 205f 4f72 6465 7265 644d 756c 7469   = _OrderedMulti
-00006920: 6e6f 6d69 616c 286e 616d 652c 202a 6172  nomial(name, *ar
-00006930: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-00006940: 2020 2020 2020 6966 2063 6f6d 7075 7465        if compute
-00006950: 5f70 3a0a 2020 2020 2020 2020 2020 2020  _p:.            
-00006960: 706d 2e44 6574 6572 6d69 6e69 7374 6963  pm.Deterministic
-00006970: 2866 227b 6e61 6d65 7d5f 7072 6f62 7322  (f"{name}_probs"
-00006980: 2c20 6f75 745f 7276 2e6f 776e 6572 2e69  , out_rv.owner.i
-00006990: 6e70 7574 735b 345d 2c20 6469 6d73 3d6b  nputs[4], dims=k
-000069a0: 7761 7267 732e 6765 7428 2264 696d 7322  wargs.get("dims"
-000069b0: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-000069c0: 6e20 6f75 745f 7276 0a0a 2020 2020 4063  n out_rv..    @c
-000069d0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-000069e0: 6566 2064 6973 7428 636c 732c 202a 6172  ef dist(cls, *ar
-000069f0: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00006a00: 2020 2020 2020 2072 6574 7572 6e20 5f4f         return _O
-00006a10: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
-00006a20: 6c2e 6469 7374 282a 6172 6773 2c20 2a2a  l.dist(*args, **
-00006a30: 6b77 6172 6773 290a 0a0a 6465 6620 706f  kwargs)...def po
-00006a40: 7364 6566 2841 4129 3a0a 2020 2020 7472  sdef(AA):.    tr
-00006a50: 793a 0a20 2020 2020 2020 206c 696e 616c  y:.        linal
-00006a60: 672e 6368 6f6c 6573 6b79 2841 4129 0a20  g.cholesky(AA). 
-00006a70: 2020 2020 2020 2072 6574 7572 6e20 310a         return 1.
-00006a80: 2020 2020 6578 6365 7074 206c 696e 616c      except linal
-00006a90: 672e 4c69 6e41 6c67 4572 726f 723a 0a20  g.LinAlgError:. 
-00006aa0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
-00006ab0: 0a0a 636c 6173 7320 506f 7344 6566 4d61  ..class PosDefMa
-00006ac0: 7472 6978 284f 7029 3a0a 2020 2020 2222  trix(Op):.    ""
-00006ad0: 220a 2020 2020 4368 6563 6b20 6966 2069  ".    Check if i
-00006ae0: 6e70 7574 2069 7320 706f 7369 7469 7665  nput is positive
-00006af0: 2064 6566 696e 6974 652e 2049 6e70 7574   definite. Input
-00006b00: 2073 686f 756c 6420 6265 2061 2073 7175   should be a squ
-00006b10: 6172 6520 6d61 7472 6978 2e0a 0a20 2020  are matrix...   
-00006b20: 2022 2222 0a0a 2020 2020 2320 5072 6f70   """..    # Prop
-00006b30: 6572 7469 6573 2061 7474 7269 6275 7465  erties attribute
-00006b40: 0a20 2020 205f 5f70 726f 7073 5f5f 203d  .    __props__ =
-00006b50: 2028 290a 0a20 2020 2023 2043 6f6d 7075   ()..    # Compu
-00006b60: 6c73 6f72 7920 6966 2069 7479 7065 7320  lsory if itypes 
-00006b70: 616e 6420 6f74 7970 6573 2061 7265 206e  and otypes are n
-00006b80: 6f74 2064 6566 696e 6564 0a0a 2020 2020  ot defined..    
-00006b90: 6465 6620 6d61 6b65 5f6e 6f64 6528 7365  def make_node(se
-00006ba0: 6c66 2c20 7829 3a0a 2020 2020 2020 2020  lf, x):.        
-00006bb0: 7820 3d20 7074 2e61 735f 7465 6e73 6f72  x = pt.as_tensor
-00006bc0: 5f76 6172 6961 626c 6528 7829 0a20 2020  _variable(x).   
-00006bd0: 2020 2020 2061 7373 6572 7420 782e 6e64       assert x.nd
-00006be0: 696d 203d 3d20 320a 2020 2020 2020 2020  im == 2.        
-00006bf0: 6f20 3d20 5465 6e73 6f72 5479 7065 2864  o = TensorType(d
-00006c00: 7479 7065 3d22 696e 7438 222c 2073 6861  type="int8", sha
-00006c10: 7065 3d5b 5d29 2829 0a20 2020 2020 2020  pe=[])().       
-00006c20: 2072 6574 7572 6e20 4170 706c 7928 7365   return Apply(se
-00006c30: 6c66 2c20 5b78 5d2c 205b 6f5d 290a 0a20  lf, [x], [o]).. 
-00006c40: 2020 2023 2050 7974 686f 6e20 696d 706c     # Python impl
-00006c50: 656d 656e 7461 7469 6f6e 3a0a 2020 2020  ementation:.    
-00006c60: 6465 6620 7065 7266 6f72 6d28 7365 6c66  def perform(self
-00006c70: 2c20 6e6f 6465 2c20 696e 7075 7473 2c20  , node, inputs, 
-00006c80: 6f75 7470 7574 7329 3a0a 2020 2020 2020  outputs):.      
-00006c90: 2020 2878 2c29 203d 2069 6e70 7574 730a    (x,) = inputs.
-00006ca0: 2020 2020 2020 2020 287a 2c29 203d 206f          (z,) = o
-00006cb0: 7574 7075 7473 0a20 2020 2020 2020 2074  utputs.        t
-00006cc0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00006cd0: 7a5b 305d 203d 206e 702e 6172 7261 7928  z[0] = np.array(
-00006ce0: 706f 7364 6566 2878 292c 2064 7479 7065  posdef(x), dtype
-00006cf0: 3d22 696e 7438 2229 0a20 2020 2020 2020  ="int8").       
-00006d00: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00006d10: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
-00006d20: 6d2e 5f6c 6f67 2e65 7863 6570 7469 6f6e  m._log.exception
-00006d30: 2822 4661 696c 6564 2074 6f20 6368 6563  ("Failed to chec
-00006d40: 6b20 6966 2025 7320 706f 7369 7469 7665  k if %s positive
-00006d50: 2064 6566 696e 6974 6522 2c20 7829 0a20   definite", x). 
-00006d60: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00006d70: 0a0a 2020 2020 6465 6620 696e 6665 725f  ..    def infer_
-00006d80: 7368 6170 6528 7365 6c66 2c20 6667 7261  shape(self, fgra
-00006d90: 7068 2c20 6e6f 6465 2c20 7368 6170 6573  ph, node, shapes
-00006da0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00006db0: 6e20 5b5b 5d5d 0a0a 2020 2020 6465 6620  n [[]]..    def 
-00006dc0: 6772 6164 2873 656c 662c 2069 6e70 2c20  grad(self, inp, 
-00006dd0: 6772 6164 7329 3a0a 2020 2020 2020 2020  grads):.        
-00006de0: 2878 2c29 203d 2069 6e70 0a20 2020 2020  (x,) = inp.     
-00006df0: 2020 2072 6574 7572 6e20 5b78 2e7a 6572     return [x.zer
-00006e00: 6f73 5f6c 696b 6528 7079 7465 6e73 6f72  os_like(pytensor
-00006e10: 2e63 6f6e 6669 672e 666c 6f61 7458 295d  .config.floatX)]
-00006e20: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-00006e30: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00006e40: 2072 6574 7572 6e20 224d 6174 7269 7849   return "MatrixI
-00006e50: 7350 6f73 6974 6976 6544 6566 696e 6974  sPositiveDefinit
-00006e60: 6522 0a0a 0a6d 6174 7269 785f 706f 735f  e"...matrix_pos_
-00006e70: 6465 6620 3d20 506f 7344 6566 4d61 7472  def = PosDefMatr
-00006e80: 6978 2829 0a0a 0a63 6c61 7373 2057 6973  ix()...class Wis
-00006e90: 6861 7274 5256 2852 616e 646f 6d56 6172  hartRV(RandomVar
-00006ea0: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
-00006eb0: 203d 2022 7769 7368 6172 7422 0a20 2020   = "wishart".   
-00006ec0: 206e 6469 6d5f 7375 7070 203d 2032 0a20   ndim_supp = 2. 
-00006ed0: 2020 206e 6469 6d73 5f70 6172 616d 7320     ndims_params 
-00006ee0: 3d20 5b30 2c20 325d 0a20 2020 2064 7479  = [0, 2].    dty
-00006ef0: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
-00006f00: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
-00006f10: 2822 5769 7368 6172 7422 2c20 225c 5c6f  ("Wishart", "\\o
-00006f20: 7065 7261 746f 726e 616d 657b 5769 7368  peratorname{Wish
-00006f30: 6172 747d 2229 0a0a 2020 2020 6465 6620  art}")..    def 
-00006f40: 5f73 7570 705f 7368 6170 655f 6672 6f6d  _supp_shape_from
-00006f50: 5f70 6172 616d 7328 7365 6c66 2c20 6469  _params(self, di
-00006f60: 7374 5f70 6172 616d 732c 2072 6570 5f70  st_params, rep_p
-00006f70: 6172 616d 5f69 6478 3d31 2c20 7061 7261  aram_idx=1, para
-00006f80: 6d5f 7368 6170 6573 3d4e 6f6e 6529 3a0a  m_shapes=None):.
-00006f90: 2020 2020 2020 2020 2320 5468 6520 7368          # The sh
-00006fa0: 6170 6520 6f66 2073 6563 6f6e 6420 7061  ape of second pa
-00006fb0: 7261 6d65 7465 7220 6056 6020 6465 6669  rameter `V` defi
-00006fc0: 6e65 7320 7468 6520 7368 6170 6520 6f66  nes the shape of
-00006fd0: 2074 6865 206f 7574 7075 742e 0a20 2020   the output..   
-00006fe0: 2020 2020 2072 6574 7572 6e20 6469 7374       return dist
-00006ff0: 5f70 6172 616d 735b 315d 2e73 6861 7065  _params[1].shape
-00007000: 5b2d 323a 5d0a 0a20 2020 2040 636c 6173  [-2:]..    @clas
-00007010: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00007020: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
-00007030: 206e 752c 2056 2c20 7369 7a65 293a 0a20   nu, V, size):. 
-00007040: 2020 2020 2020 2073 6369 7079 5f73 697a         scipy_siz
-00007050: 6520 3d20 7369 7a65 2069 6620 7369 7a65  e = size if size
-00007060: 2065 6c73 6520 3120 2023 2044 6566 6175   else 1  # Defau
-00007070: 6c74 2073 697a 6520 666f 7220 5363 6970  lt size for Scip
-00007080: 7927 7320 7769 7368 6172 742e 7276 7320  y's wishart.rvs 
-00007090: 6973 2031 0a20 2020 2020 2020 2072 6573  is 1.        res
-000070a0: 756c 7420 3d20 7374 6174 732e 7769 7368  ult = stats.wish
-000070b0: 6172 742e 7276 7328 696e 7428 6e75 292c  art.rvs(int(nu),
-000070c0: 2056 2c20 7369 7a65 3d73 6369 7079 5f73   V, size=scipy_s
-000070d0: 697a 652c 2072 616e 646f 6d5f 7374 6174  ize, random_stat
-000070e0: 653d 726e 6729 0a20 2020 2020 2020 2069  e=rng).        i
-000070f0: 6620 7369 7a65 203d 3d20 2831 2c29 3a0a  f size == (1,):.
-00007100: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00007110: 726e 2072 6573 756c 745b 6e70 2e6e 6577  rn result[np.new
-00007120: 6178 6973 2c20 2e2e 2e5d 0a20 2020 2020  axis, ...].     
-00007130: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007140: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00007150: 6c74 0a0a 0a77 6973 6861 7274 203d 2057  lt...wishart = W
-00007160: 6973 6861 7274 5256 2829 0a0a 0a63 6c61  ishartRV()...cla
-00007170: 7373 2057 6973 6861 7274 2843 6f6e 7469  ss Wishart(Conti
-00007180: 6e75 6f75 7329 3a0a 2020 2020 7222 2222  nuous):.    r"""
-00007190: 0a20 2020 2057 6973 6861 7274 206c 6f67  .    Wishart log
-000071a0: 2d6c 696b 656c 6968 6f6f 642e 0a0a 2020  -likelihood...  
-000071b0: 2020 5468 6520 5769 7368 6172 7420 6469    The Wishart di
-000071c0: 7374 7269 6275 7469 6f6e 2069 7320 7468  stribution is th
-000071d0: 6520 7072 6f62 6162 696c 6974 7920 6469  e probability di
-000071e0: 7374 7269 6275 7469 6f6e 206f 6620 7468  stribution of th
-000071f0: 650a 2020 2020 6d61 7869 6d75 6d2d 6c69  e.    maximum-li
-00007200: 6b65 6c69 686f 6f64 2065 7374 696d 6174  kelihood estimat
-00007210: 6f72 2028 4d4c 4529 206f 6620 7468 6520  or (MLE) of the 
-00007220: 7072 6563 6973 696f 6e20 6d61 7472 6978  precision matrix
-00007230: 206f 6620 610a 2020 2020 6d75 6c74 6976   of a.    multiv
-00007240: 6172 6961 7465 206e 6f72 6d61 6c20 6469  ariate normal di
-00007250: 7374 7269 6275 7469 6f6e 2e20 2049 6620  stribution.  If 
-00007260: 563d 312c 2074 6865 2064 6973 7472 6962  V=1, the distrib
-00007270: 7574 696f 6e20 6973 0a20 2020 2069 6465  ution is.    ide
-00007280: 6e74 6963 616c 2074 6f20 7468 6520 6368  ntical to the ch
-00007290: 692d 7371 7561 7265 2064 6973 7472 6962  i-square distrib
-000072a0: 7574 696f 6e20 7769 7468 206e 7520 6465  ution with nu de
-000072b0: 6772 6565 7320 6f66 0a20 2020 2066 7265  grees of.    fre
-000072c0: 6564 6f6d 2e0a 0a20 2020 202e 2e20 6d61  edom...    .. ma
-000072d0: 7468 3a3a 0a0a 2020 2020 2020 2066 2858  th::..       f(X
-000072e0: 205c 6d69 6420 6e75 2c20 5429 203d 0a20   \mid nu, T) =. 
-000072f0: 2020 2020 2020 2020 2020 5c66 7261 637b            \frac{
-00007300: 7b5c 6d69 6420 5420 5c6d 6964 7d5e 7b6e  {\mid T \mid}^{n
-00007310: 752f 327d 7b5c 6d69 6420 5820 5c6d 6964  u/2}{\mid X \mid
-00007320: 7d5e 7b28 6e75 2d6b 2d31 292f 327d 7d7b  }^{(nu-k-1)/2}}{
-00007330: 325e 7b6e 7520 6b2f 327d 0a20 2020 2020  2^{nu k/2}.     
-00007340: 2020 2020 2020 5c47 616d 6d61 5f70 286e        \Gamma_p(n
-00007350: 752f 3229 7d20 5c65 7870 5c6c 6566 745c  u/2)} \exp\left\
-00007360: 7b20 2d5c 6672 6163 7b31 7d7b 327d 2054  { -\frac{1}{2} T
-00007370: 7228 5458 2920 5c72 6967 6874 5c7d 0a0a  r(TX) \right\}..
-00007380: 2020 2020 7768 6572 6520 3a6d 6174 683a      where :math:
-00007390: 606b 6020 6973 2074 6865 2072 616e 6b20  `k` is the rank 
-000073a0: 6f66 203a 6d61 7468 3a60 5860 2e0a 0a20  of :math:`X`... 
-000073b0: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
-000073c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000073d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000073e0: 3d3d 3d3d 3d3d 0a20 2020 2053 7570 706f  ======.    Suppo
-000073f0: 7274 2020 203a 6d61 7468 3a60 5828 7020  rt   :math:`X(p 
-00007400: 7820 7029 6020 706f 7369 7469 7665 2064  x p)` positive d
-00007410: 6566 696e 6974 6520 6d61 7472 6978 0a20  efinite matrix. 
-00007420: 2020 204d 6561 6e20 2020 2020 203a 6d61     Mean      :ma
-00007430: 7468 3a60 6e75 2056 600a 2020 2020 5661  th:`nu V`.    Va
-00007440: 7269 616e 6365 2020 3a6d 6174 683a 606e  riance  :math:`n
-00007450: 7520 2876 5f7b 696a 7d5e 3220 2b20 765f  u (v_{ij}^2 + v_
-00007460: 7b69 697d 2076 5f7b 6a6a 7d29 600a 2020  {ii} v_{jj})`.  
-00007470: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
-00007480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000074a0: 3d3d 3d3d 3d0a 0a20 2020 2050 6172 616d  =====..    Param
-000074b0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-000074c0: 2d2d 2d2d 0a20 2020 206e 7520 3a20 7465  ----.    nu : te
-000074d0: 6e73 6f72 5f6c 696b 6520 6f66 2069 6e74  nsor_like of int
-000074e0: 0a20 2020 2020 2020 2044 6567 7265 6573  .        Degrees
-000074f0: 206f 6620 6672 6565 646f 6d2c 203e 2030   of freedom, > 0
-00007500: 2e0a 2020 2020 5620 3a20 7465 6e73 6f72  ..    V : tensor
-00007510: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-00007520: 2020 2020 2020 2070 2078 2070 2070 6f73         p x p pos
-00007530: 6974 6976 6520 6465 6669 6e69 7465 206d  itive definite m
-00007540: 6174 7269 782e 0a0a 2020 2020 4e6f 7465  atrix...    Note
-00007550: 730a 2020 2020 2d2d 2d2d 2d0a 2020 2020  s.    -----.    
-00007560: 5468 6973 2064 6973 7472 6962 7574 696f  This distributio
-00007570: 6e20 6973 2075 6e75 7361 626c 6520 696e  n is unusable in
-00007580: 2061 2050 794d 4320 6d6f 6465 6c2e 2059   a PyMC model. Y
-00007590: 6f75 2073 686f 756c 6420 696e 7374 6561  ou should instea
-000075a0: 640a 2020 2020 7573 6520 4c4b 4a43 686f  d.    use LKJCho
-000075b0: 6c65 736b 7943 6f76 206f 7220 4c4b 4a43  leskyCov or LKJC
-000075c0: 6f72 722e 0a20 2020 2022 2222 0a20 2020  orr..    """.   
-000075d0: 2072 765f 6f70 203d 2077 6973 6861 7274   rv_op = wishart
-000075e0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-000075f0: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
-00007600: 636c 732c 206e 752c 2056 2c20 2a61 7267  cls, nu, V, *arg
-00007610: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
-00007620: 2020 2020 2020 6e75 203d 2070 742e 6173        nu = pt.as
-00007630: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00007640: 2869 6e74 5828 6e75 2929 0a20 2020 2020  (intX(nu)).     
-00007650: 2020 2056 203d 2070 742e 6173 5f74 656e     V = pt.as_ten
-00007660: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
-00007670: 6174 5828 5629 290a 0a20 2020 2020 2020  atX(V))..       
-00007680: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00007690: 2020 2020 2020 2020 2020 2020 2254 6865              "The
-000076a0: 2057 6973 6861 7274 2064 6973 7472 6962   Wishart distrib
-000076b0: 7574 696f 6e20 6361 6e20 6375 7272 656e  ution can curren
-000076c0: 746c 7920 6e6f 7420 6265 2075 7365 6420  tly not be used 
-000076d0: 220a 2020 2020 2020 2020 2020 2020 2266  ".            "f
-000076e0: 6f72 204d 434d 4320 7361 6d70 6c69 6e67  or MCMC sampling
-000076f0: 2e20 5468 6520 7072 6f62 6162 696c 6974  . The probabilit
-00007700: 7920 6f66 2073 616d 706c 696e 6720 6120  y of sampling a 
-00007710: 220a 2020 2020 2020 2020 2020 2020 2273  ".            "s
-00007720: 796d 6d65 7472 6963 206d 6174 7269 7820  ymmetric matrix 
-00007730: 6973 2062 6173 6963 616c 6c79 207a 6572  is basically zer
-00007740: 6f2e 2049 6e73 7465 6164 2c20 706c 6561  o. Instead, plea
-00007750: 7365 2022 0a20 2020 2020 2020 2020 2020  se ".           
-00007760: 2022 7573 6520 4c4b 4a43 686f 6c65 736b   "use LKJCholesk
-00007770: 7943 6f76 206f 7220 4c4b 4a43 6f72 722e  yCov or LKJCorr.
-00007780: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
-00007790: 6174 696f 6e20 220a 2020 2020 2020 2020  ation ".        
-000077a0: 2020 2020 226f 6e20 7468 6520 6973 7375      "on the issu
-000077b0: 6573 2073 7572 726f 756e 6469 6e67 2074  es surrounding t
-000077c0: 6865 2057 6973 6861 7274 2073 6565 2068  he Wishart see h
-000077d0: 6572 653a 2022 0a20 2020 2020 2020 2020  ere: ".         
-000077e0: 2020 2022 6874 7470 733a 2f2f 6769 7468     "https://gith
-000077f0: 7562 2e63 6f6d 2f70 796d 632d 6465 7673  ub.com/pymc-devs
-00007800: 2f70 796d 632f 6973 7375 6573 2f35 3338  /pymc/issues/538
-00007810: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00007820: 5573 6572 5761 726e 696e 672c 0a20 2020  UserWarning,.   
-00007830: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00007840: 2320 6d65 616e 203d 206e 7520 2a20 560a  # mean = nu * V.
-00007850: 2020 2020 2020 2020 2320 7020 3d20 562e          # p = V.
-00007860: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
-00007870: 2023 206d 6f64 6520 3d20 7074 2e73 7769   # mode = pt.swi
-00007880: 7463 6828 7074 2e67 6528 6e75 2c20 7020  tch(pt.ge(nu, p 
-00007890: 2b20 3129 2c20 286e 7520 2d20 7020 2d20  + 1), (nu - p - 
-000078a0: 3129 202a 2056 2c20 6e70 2e6e 616e 290a  1) * V, np.nan).
-000078b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000078c0: 7570 6572 2829 2e64 6973 7428 5b6e 752c  uper().dist([nu,
-000078d0: 2056 5d2c 202a 6172 6773 2c20 2a2a 6b77   V], *args, **kw
-000078e0: 6172 6773 290a 0a20 2020 2064 6566 206c  args)..    def l
-000078f0: 6f67 7028 582c 206e 752c 2056 293a 0a20  ogp(X, nu, V):. 
-00007900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007910: 2020 2043 616c 6375 6c61 7465 206c 6f67     Calculate log
-00007920: 2d70 726f 6261 6269 6c69 7479 206f 6620  -probability of 
-00007930: 5769 7368 6172 7420 6469 7374 7269 6275  Wishart distribu
-00007940: 7469 6f6e 0a20 2020 2020 2020 2061 7420  tion.        at 
-00007950: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
-00007960: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00007970: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00007980: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00007990: 583a 206e 756d 6572 6963 0a20 2020 2020  X: numeric.     
-000079a0: 2020 2020 2020 2056 616c 7565 2066 6f72         Value for
-000079b0: 2077 6869 6368 206c 6f67 2d70 726f 6261   which log-proba
-000079c0: 6269 6c69 7479 2069 7320 6361 6c63 756c  bility is calcul
-000079d0: 6174 6564 2e0a 0a20 2020 2020 2020 2052  ated...        R
-000079e0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-000079f0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
-00007a00: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
-00007a10: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00007a20: 2020 2070 203d 2056 2e73 6861 7065 5b30     p = V.shape[0
-00007a30: 5d0a 0a20 2020 2020 2020 2049 5649 203d  ]..        IVI =
-00007a40: 2064 6574 2856 290a 2020 2020 2020 2020   det(V).        
-00007a50: 4958 4920 3d20 6465 7428 5829 0a0a 2020  IXI = det(X)..  
-00007a60: 2020 2020 2020 7265 7475 726e 2063 6865        return che
-00007a70: 636b 5f70 6172 616d 6574 6572 7328 0a20  ck_parameters(. 
-00007a80: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-00007a90: 2020 2020 2020 2020 2020 2020 2028 6e75               (nu
-00007aa0: 202d 2070 202d 2031 2920 2a20 7074 2e6c   - p - 1) * pt.l
-00007ab0: 6f67 2849 5849 290a 2020 2020 2020 2020  og(IXI).        
-00007ac0: 2020 2020 2020 2020 2d20 7472 6163 6528          - trace(
-00007ad0: 6d61 7472 6978 5f69 6e76 6572 7365 2856  matrix_inverse(V
-00007ae0: 292e 646f 7428 5829 290a 2020 2020 2020  ).dot(X)).      
-00007af0: 2020 2020 2020 2020 2020 2d20 6e75 202a            - nu *
-00007b00: 2070 202a 2070 742e 6c6f 6728 3229 0a20   p * pt.log(2). 
-00007b10: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00007b20: 206e 7520 2a20 7074 2e6c 6f67 2849 5649   nu * pt.log(IVI
-00007b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007b40: 2020 2d20 3220 2a20 6d75 6c74 6967 616d    - 2 * multigam
-00007b50: 6d61 6c6e 286e 7520 2f20 322e 302c 2070  maln(nu / 2.0, p
-00007b60: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00007b70: 2020 2020 2020 2020 2020 2020 2f20 322c              / 2,
-00007b80: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
-00007b90: 7269 785f 706f 735f 6465 6628 5829 2c0a  rix_pos_def(X),.
-00007ba0: 2020 2020 2020 2020 2020 2020 7074 2e65              pt.e
-00007bb0: 7128 582c 2058 2e54 292c 0a20 2020 2020  q(X, X.T),.     
-00007bc0: 2020 2020 2020 206e 7520 3e20 2870 202d         nu > (p -
-00007bd0: 2031 292c 0a20 2020 2020 2020 2029 0a0a   1),.        )..
-00007be0: 0a64 6566 2057 6973 6861 7274 4261 7274  .def WishartBart
-00007bf0: 6c65 7474 286e 616d 652c 2053 2c20 6e75  lett(name, S, nu
-00007c00: 2c20 6973 5f63 686f 6c65 736b 793d 4661  , is_cholesky=Fa
-00007c10: 6c73 652c 2072 6574 7572 6e5f 6368 6f6c  lse, return_chol
-00007c20: 6573 6b79 3d46 616c 7365 2c20 696e 6974  esky=False, init
-00007c30: 7661 6c3d 4e6f 6e65 293a 0a20 2020 2072  val=None):.    r
-00007c40: 2222 220a 2020 2020 4261 7274 6c65 7474  """.    Bartlett
-00007c50: 2064 6563 6f6d 706f 7369 7469 6f6e 206f   decomposition o
-00007c60: 6620 7468 6520 5769 7368 6172 7420 6469  f the Wishart di
-00007c70: 7374 7269 6275 7469 6f6e 2e20 4173 2074  stribution. As t
-00007c80: 6865 2057 6973 6861 7274 0a20 2020 2064  he Wishart.    d
-00007c90: 6973 7472 6962 7574 696f 6e20 7265 7175  istribution requ
-00007ca0: 6972 6573 2074 6865 206d 6174 7269 7820  ires the matrix 
-00007cb0: 746f 2062 6520 7379 6d6d 6574 7269 6320  to be symmetric 
-00007cc0: 706f 7369 7469 7665 2073 656d 692d 6465  positive semi-de
-00007cd0: 6669 6e69 7465 0a20 2020 2069 7420 6973  finite.    it is
-00007ce0: 2069 6d70 6f73 7369 626c 6520 666f 7220   impossible for 
-00007cf0: 4d43 4d43 2074 6f20 6576 6572 2070 726f  MCMC to ever pro
-00007d00: 706f 7365 2061 6363 6570 7461 626c 6520  pose acceptable 
-00007d10: 6d61 7472 6963 6573 2e0a 0a20 2020 2049  matrices...    I
-00007d20: 6e73 7465 6164 2c20 7765 2063 616e 2075  nstead, we can u
-00007d30: 7365 2074 6865 2042 6172 6c65 7474 2064  se the Barlett d
-00007d40: 6563 6f6d 706f 7369 7469 6f6e 2077 6869  ecomposition whi
-00007d50: 6368 2073 616d 706c 6573 2061 206c 6f77  ch samples a low
-00007d60: 6572 0a20 2020 2064 6961 676f 6e61 6c20  er.    diagonal 
-00007d70: 6d61 7472 6978 2e20 5370 6563 6966 6963  matrix. Specific
-00007d80: 616c 6c79 3a0a 0a20 2020 202e 2e20 6d61  ally:..    .. ma
-00007d90: 7468 3a3a 0a20 2020 2020 2020 205c 7465  th::.        \te
-00007da0: 7874 7b49 667d 204c 205c 7369 6d20 5c62  xt{If} L \sim \b
-00007db0: 6567 696e 7b70 6d61 7472 6978 7d0a 2020  egin{pmatrix}.  
-00007dc0: 2020 2020 2020 5c73 7172 747b 635f 317d        \sqrt{c_1}
-00007dd0: 2026 2030 2026 2030 205c 5c0a 2020 2020   & 0 & 0 \\.    
-00007de0: 2020 2020 7a5f 7b32 317d 2026 205c 7371      z_{21} & \sq
-00007df0: 7274 7b63 5f32 7d20 2620 3020 5c5c 0a20  rt{c_2} & 0 \\. 
-00007e00: 2020 2020 2020 207a 5f7b 3331 7d20 2620         z_{31} & 
-00007e10: 7a5f 7b33 327d 2026 205c 7371 7274 7b63  z_{32} & \sqrt{c
-00007e20: 5f33 7d0a 2020 2020 2020 2020 5c65 6e64  _3}.        \end
-00007e30: 7b70 6d61 7472 6978 7d0a 0a20 2020 2020  {pmatrix}..     
-00007e40: 2020 205c 7465 7874 7b77 6974 687d 2063     \text{with} c
-00007e50: 5f69 205c 7369 6d20 5c63 6869 5e32 286e  _i \sim \chi^2(n
-00007e60: 2d69 2b31 2920 5c74 6578 747b 2061 6e64  -i+1) \text{ and
-00007e70: 207d 206e 5f7b 696a 7d20 5c73 696d 205c   } n_{ij} \sim \
-00007e80: 6d61 7468 6361 6c7b 4e7d 2830 2c20 3129  mathcal{N}(0, 1)
-00007e90: 2c20 5c74 6578 747b 7468 656e 7d20 5c5c  , \text{then} \\
-00007ea0: 0a20 2020 2020 2020 204c 205c 7469 6d65  .        L \time
-00007eb0: 7320 4120 5c74 696d 6573 2041 2e54 205c  s A \times A.T \
-00007ec0: 7469 6d65 7320 4c2e 5420 5c73 696d 205c  times L.T \sim \
-00007ed0: 7465 7874 7b57 6973 6861 7274 7d28 4c20  text{Wishart}(L 
-00007ee0: 5c74 696d 6573 204c 2e54 2c20 5c6e 7529  \times L.T, \nu)
-00007ef0: 0a0a 2020 2020 5365 6520 6874 7470 3a2f  ..    See http:/
-00007f00: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00007f10: 672f 7769 6b69 2f57 6973 6861 7274 5f64  g/wiki/Wishart_d
-00007f20: 6973 7472 6962 7574 696f 6e23 4261 7274  istribution#Bart
-00007f30: 6c65 7474 5f64 6563 6f6d 706f 7369 7469  lett_decompositi
-00007f40: 6f6e 0a20 2020 2066 6f72 206d 6f72 6520  on.    for more 
-00007f50: 696e 666f 726d 6174 696f 6e2e 0a0a 2020  information...  
-00007f60: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00007f70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00007f80: 5320 3a20 6e64 6172 7261 790a 2020 2020  S : ndarray.    
-00007f90: 2020 2020 7020 7820 7020 706f 7369 7469      p x p positi
-00007fa0: 7665 2064 6566 696e 6974 6520 6d61 7472  ve definite matr
-00007fb0: 6978 0a20 2020 2020 2020 204f 723a 0a20  ix.        Or:. 
-00007fc0: 2020 2020 2020 2070 2078 2070 206c 6f77         p x p low
-00007fd0: 6572 2d74 7269 616e 6775 6c61 7220 6d61  er-triangular ma
-00007fe0: 7472 6978 2074 6861 7420 6973 2074 6865  trix that is the
-00007ff0: 2043 686f 6c65 736b 7920 6661 6374 6f72   Cholesky factor
-00008000: 0a20 2020 2020 2020 206f 6620 7468 6520  .        of the 
-00008010: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00008020: 782e 0a20 2020 206e 7520 3a20 7465 6e73  x..    nu : tens
-00008030: 6f72 5f6c 696b 6520 6f66 2069 6e74 0a20  or_like of int. 
-00008040: 2020 2020 2020 2044 6567 7265 6573 206f         Degrees o
-00008050: 6620 6672 6565 646f 6d2c 203e 2064 696d  f freedom, > dim
-00008060: 2853 292e 0a20 2020 2069 735f 6368 6f6c  (S)..    is_chol
-00008070: 6573 6b79 203a 2062 6f6f 6c2c 2064 6566  esky : bool, def
-00008080: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
-00008090: 2020 2049 6e70 7574 206d 6174 7269 7820     Input matrix 
-000080a0: 5320 6973 2061 6c72 6561 6479 2043 686f  S is already Cho
-000080b0: 6c65 736b 7920 6465 636f 6d70 6f73 6564  lesky decomposed
-000080c0: 2061 7320 532e 5420 2a20 530a 2020 2020   as S.T * S.    
-000080d0: 7265 7475 726e 5f63 686f 6c65 736b 7920  return_cholesky 
-000080e0: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
-000080f0: 4661 6c73 650a 2020 2020 2020 2020 4f6e  False.        On
-00008100: 6c79 2072 6574 7572 6e20 7468 6520 4368  ly return the Ch
-00008110: 6f6c 6573 6b79 2064 6563 6f6d 706f 7365  olesky decompose
-00008120: 6420 6d61 7472 6978 2e0a 2020 2020 696e  d matrix..    in
-00008130: 6974 7661 6c20 3a20 6e64 6172 7261 790a  itval : ndarray.
-00008140: 2020 2020 2020 2020 7020 7820 7020 706f          p x p po
-00008150: 7369 7469 7665 2064 6566 696e 6974 6520  sitive definite 
-00008160: 6d61 7472 6978 2075 7365 6420 746f 2069  matrix used to i
-00008170: 6e69 7469 616c 697a 650a 0a20 2020 204e  nitialize..    N
-00008180: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
-00008190: 2020 2054 6869 7320 6973 206e 6f74 2061     This is not a
-000081a0: 2073 7461 6e64 6172 6420 4469 7374 7269   standard Distri
-000081b0: 6275 7469 6f6e 2063 6c61 7373 2062 7574  bution class but
-000081c0: 2066 6f6c 6c6f 7773 2061 2073 696d 696c   follows a simil
-000081d0: 6172 0a20 2020 2069 6e74 6572 6661 6365  ar.    interface
-000081e0: 2e20 4265 7369 6465 7320 7468 6520 5769  . Besides the Wi
-000081f0: 7368 6172 7420 6469 7374 7269 6275 7469  shart distributi
-00008200: 6f6e 2c20 6974 2077 696c 6c20 6164 6420  on, it will add 
-00008210: 5256 730a 2020 2020 6e61 6d65 5f63 2061  RVs.    name_c a
-00008220: 6e64 206e 616d 655f 7a20 746f 2079 6f75  nd name_z to you
-00008230: 7220 6d6f 6465 6c20 7768 6963 6820 6d61  r model which ma
-00008240: 6b65 2075 7020 7468 6520 6d61 7472 6978  ke up the matrix
-00008250: 2e0a 0a20 2020 2054 6869 7320 6469 7374  ...    This dist
-00008260: 7269 6275 7469 6f6e 2069 7320 7573 7561  ribution is usua
-00008270: 6c6c 7920 6120 6261 6420 6964 6561 2074  lly a bad idea t
-00008280: 6f20 7573 6520 6173 2061 2070 7269 6f72  o use as a prior
-00008290: 2066 6f72 206d 756c 7469 7661 7269 6174   for multivariat
-000082a0: 650a 2020 2020 6e6f 726d 616c 2e20 596f  e.    normal. Yo
-000082b0: 7520 7368 6f75 6c64 2069 6e73 7465 6164  u should instead
-000082c0: 2075 7365 204c 4b4a 4368 6f6c 6573 6b79   use LKJCholesky
-000082d0: 436f 7620 6f72 204c 4b4a 436f 7272 2e0a  Cov or LKJCorr..
-000082e0: 2020 2020 2222 220a 0a20 2020 204c 203d      """..    L =
-000082f0: 2053 2069 6620 6973 5f63 686f 6c65 736b   S if is_cholesk
-00008300: 7920 656c 7365 2073 6369 7079 2e6c 696e  y else scipy.lin
-00008310: 616c 672e 6368 6f6c 6573 6b79 2853 290a  alg.cholesky(S).
-00008320: 2020 2020 6469 6167 5f69 6478 203d 206e      diag_idx = n
-00008330: 702e 6469 6167 5f69 6e64 6963 6573 5f66  p.diag_indices_f
-00008340: 726f 6d28 5329 0a20 2020 2074 7269 6c5f  rom(S).    tril_
-00008350: 6964 7820 3d20 6e70 2e74 7269 6c5f 696e  idx = np.tril_in
-00008360: 6469 6365 735f 6672 6f6d 2853 2c20 6b3d  dices_from(S, k=
-00008370: 2d31 290a 2020 2020 6e5f 6469 6167 203d  -1).    n_diag =
-00008380: 206c 656e 2864 6961 675f 6964 785b 305d   len(diag_idx[0]
-00008390: 290a 2020 2020 6e5f 7472 696c 203d 206c  ).    n_tril = l
-000083a0: 656e 2874 7269 6c5f 6964 785b 305d 290a  en(tril_idx[0]).
-000083b0: 0a20 2020 2069 6620 696e 6974 7661 6c20  .    if initval 
-000083c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000083d0: 2020 2020 2023 2049 6e76 6572 7365 2074       # Inverse t
-000083e0: 7261 6e73 666f 726d 0a20 2020 2020 2020  ransform.       
-000083f0: 2069 6e69 7476 616c 203d 206e 702e 646f   initval = np.do
-00008400: 7428 6e70 2e64 6f74 286e 702e 6c69 6e61  t(np.dot(np.lina
-00008410: 6c67 2e69 6e76 284c 292c 2069 6e69 7476  lg.inv(L), initv
-00008420: 616c 292c 206e 702e 6c69 6e61 6c67 2e69  al), np.linalg.i
-00008430: 6e76 284c 2e54 2929 0a20 2020 2020 2020  nv(L.T)).       
-00008440: 2069 6e69 7476 616c 203d 206c 696e 616c   initval = linal
-00008450: 672e 6368 6f6c 6573 6b79 2869 6e69 7476  g.cholesky(initv
-00008460: 616c 2c20 6c6f 7765 723d 5472 7565 290a  al, lower=True).
-00008470: 2020 2020 2020 2020 6469 6167 5f74 6573          diag_tes
-00008480: 7476 616c 203d 2069 6e69 7476 616c 5b64  tval = initval[d
-00008490: 6961 675f 6964 785d 202a 2a20 320a 2020  iag_idx] ** 2.  
-000084a0: 2020 2020 2020 7472 696c 5f74 6573 7476        tril_testv
-000084b0: 616c 203d 2069 6e69 7476 616c 5b74 7269  al = initval[tri
-000084c0: 6c5f 6964 785d 0a20 2020 2065 6c73 653a  l_idx].    else:
-000084d0: 0a20 2020 2020 2020 2064 6961 675f 7465  .        diag_te
-000084e0: 7374 7661 6c20 3d20 4e6f 6e65 0a20 2020  stval = None.   
-000084f0: 2020 2020 2074 7269 6c5f 7465 7374 7661       tril_testva
-00008500: 6c20 3d20 4e6f 6e65 0a0a 2020 2020 6320  l = None..    c 
-00008510: 3d20 7074 2e73 7172 7428 0a20 2020 2020  = pt.sqrt(.     
-00008520: 2020 2043 6869 5371 7561 7265 6428 2225     ChiSquared("%
-00008530: 735f 6322 2025 206e 616d 652c 206e 7520  s_c" % name, nu 
-00008540: 2d20 6e70 2e61 7261 6e67 6528 322c 2032  - np.arange(2, 2
-00008550: 202b 206e 5f64 6961 6729 2c20 7368 6170   + n_diag), shap
-00008560: 653d 6e5f 6469 6167 2c20 696e 6974 7661  e=n_diag, initva
-00008570: 6c3d 6469 6167 5f74 6573 7476 616c 290a  l=diag_testval).
-00008580: 2020 2020 290a 2020 2020 706d 2e5f 6c6f      ).    pm._lo
-00008590: 672e 696e 666f 2822 4164 6465 6420 6e65  g.info("Added ne
-000085a0: 7720 7661 7269 6162 6c65 2025 735f 6320  w variable %s_c 
-000085b0: 746f 206d 6f64 656c 2064 6961 676f 6e61  to model diagona
-000085c0: 6c20 6f66 2057 6973 6861 7274 2e22 2025  l of Wishart." %
-000085d0: 206e 616d 6529 0a20 2020 207a 203d 204e   name).    z = N
-000085e0: 6f72 6d61 6c28 2225 735f 7a22 2025 206e  ormal("%s_z" % n
-000085f0: 616d 652c 2030 2e30 2c20 312e 302c 2073  ame, 0.0, 1.0, s
-00008600: 6861 7065 3d6e 5f74 7269 6c2c 2069 6e69  hape=n_tril, ini
-00008610: 7476 616c 3d74 7269 6c5f 7465 7374 7661  tval=tril_testva
-00008620: 6c29 0a20 2020 2070 6d2e 5f6c 6f67 2e69  l).    pm._log.i
-00008630: 6e66 6f28 2241 6464 6564 206e 6577 2076  nfo("Added new v
-00008640: 6172 6961 626c 6520 2573 5f7a 2074 6f20  ariable %s_z to 
-00008650: 6d6f 6465 6c20 6f66 662d 6469 6167 6f6e  model off-diagon
-00008660: 616c 7320 6f66 2057 6973 6861 7274 2e22  als of Wishart."
-00008670: 2025 206e 616d 6529 0a20 2020 2023 2043   % name).    # C
-00008680: 6f6e 7374 7275 6374 2041 206d 6174 7269  onstruct A matri
-00008690: 780a 2020 2020 4120 3d20 7074 2e7a 6572  x.    A = pt.zer
-000086a0: 6f73 2853 2e73 6861 7065 2c20 6474 7970  os(S.shape, dtyp
-000086b0: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
-000086c0: 2020 4120 3d20 7074 2e73 6574 5f73 7562    A = pt.set_sub
-000086d0: 7465 6e73 6f72 2841 5b64 6961 675f 6964  tensor(A[diag_id
-000086e0: 785d 2c20 6329 0a20 2020 2041 203d 2070  x], c).    A = p
-000086f0: 742e 7365 745f 7375 6274 656e 736f 7228  t.set_subtensor(
-00008700: 415b 7472 696c 5f69 6478 5d2c 207a 290a  A[tril_idx], z).
-00008710: 0a20 2020 2023 204c 202a 2041 202a 2041  .    # L * A * A
-00008720: 2e54 202a 204c 2e54 207e 2057 6973 6861  .T * L.T ~ Wisha
-00008730: 7274 284c 2a4c 2e54 2c20 6e75 290a 2020  rt(L*L.T, nu).  
-00008740: 2020 6966 2072 6574 7572 6e5f 6368 6f6c    if return_chol
-00008750: 6573 6b79 3a0a 2020 2020 2020 2020 7265  esky:.        re
-00008760: 7475 726e 2070 6d2e 4465 7465 726d 696e  turn pm.Determin
-00008770: 6973 7469 6328 6e61 6d65 2c20 7074 2e64  istic(name, pt.d
-00008780: 6f74 284c 2c20 4129 290a 2020 2020 656c  ot(L, A)).    el
-00008790: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-000087a0: 726e 2070 6d2e 4465 7465 726d 696e 6973  rn pm.Determinis
-000087b0: 7469 6328 6e61 6d65 2c20 7074 2e64 6f74  tic(name, pt.dot
-000087c0: 2870 742e 646f 7428 7074 2e64 6f74 284c  (pt.dot(pt.dot(L
-000087d0: 2c20 4129 2c20 412e 5429 2c20 4c2e 5429  , A), A.T), L.T)
-000087e0: 290a 0a0a 6465 6620 5f6c 6b6a 5f6e 6f72  )...def _lkj_nor
-000087f0: 6d61 6c69 7a69 6e67 5f63 6f6e 7374 616e  malizing_constan
-00008800: 7428 6574 612c 206e 293a 0a20 2020 2023  t(eta, n):.    #
-00008810: 2054 4f44 4f3a 2054 6869 7320 6973 206d   TODO: This is m
-00008820: 6978 696e 6720 7079 7468 6f6e 2062 7261  ixing python bra
-00008830: 6e63 6869 6e67 2077 6974 6820 7468 6520  nching with the 
-00008840: 706f 7465 6e74 6961 6c6c 7920 7379 6d62  potentially symb
-00008850: 6f6c 6963 206e 2061 6e64 2065 7461 2076  olic n and eta v
-00008860: 6172 6961 626c 6573 0a20 2020 2069 6620  ariables.    if 
-00008870: 6e6f 7420 6973 696e 7374 616e 6365 2865  not isinstance(e
-00008880: 7461 2c20 2869 6e74 2c20 666c 6f61 7429  ta, (int, float)
-00008890: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-000088a0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-000088b0: 7272 6f72 2822 6574 6120 6d75 7374 2062  rror("eta must b
-000088c0: 6520 616e 2069 6e74 206f 7220 666c 6f61  e an int or floa
-000088d0: 7422 290a 2020 2020 6966 206e 6f74 2069  t").    if not i
-000088e0: 7369 6e73 7461 6e63 6528 6e2c 2069 6e74  sinstance(n, int
-000088f0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00008900: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00008910: 7272 6f72 2822 6e20 6d75 7374 2062 6520  rror("n must be 
-00008920: 616e 2069 6e74 6567 6572 2229 0a20 2020  an integer").   
-00008930: 2069 6620 6574 6120 3d3d 2031 3a0a 2020   if eta == 1:.  
-00008940: 2020 2020 2020 7265 7375 6c74 203d 2067        result = g
-00008950: 616d 6d61 6c6e 2832 2e30 202a 2070 742e  ammaln(2.0 * pt.
-00008960: 6172 616e 6765 2831 2c20 696e 7428 286e  arange(1, int((n
-00008970: 202d 2031 2920 2f20 3229 202b 2031 2929   - 1) / 2) + 1))
-00008980: 2e73 756d 2829 0a20 2020 2020 2020 2069  .sum().        i
-00008990: 6620 6e20 2520 3220 3d3d 2031 3a0a 2020  f n % 2 == 1:.  
-000089a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000089b0: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
-000089c0: 2020 2020 2020 302e 3235 202a 2028 6e2a        0.25 * (n*
-000089d0: 2a32 202d 2031 2920 2a20 7074 2e6c 6f67  *2 - 1) * pt.log
-000089e0: 286e 702e 7069 290a 2020 2020 2020 2020  (np.pi).        
-000089f0: 2020 2020 2020 2020 2d20 302e 3235 202a          - 0.25 *
-00008a00: 2028 6e20 2d20 3129 202a 2a20 3220 2a20   (n - 1) ** 2 * 
-00008a10: 7074 2e6c 6f67 2832 2e30 290a 2020 2020  pt.log(2.0).    
-00008a20: 2020 2020 2020 2020 2020 2020 2d20 286e              - (n
-00008a30: 202d 2031 2920 2a20 6761 6d6d 616c 6e28   - 1) * gammaln(
-00008a40: 696e 7428 286e 202b 2031 2920 2f20 3229  int((n + 1) / 2)
-00008a50: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00008a60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008a70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008a80: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
-00008a90: 2020 2020 2020 302e 3235 202a 206e 202a        0.25 * n *
-00008aa0: 2028 6e20 2d20 3229 202a 2070 742e 6c6f   (n - 2) * pt.lo
-00008ab0: 6728 6e70 2e70 6929 0a20 2020 2020 2020  g(np.pi).       
-00008ac0: 2020 2020 2020 2020 202b 2030 2e32 3520           + 0.25 
-00008ad0: 2a20 2833 202a 206e 2a2a 3220 2d20 3420  * (3 * n**2 - 4 
-00008ae0: 2a20 6e29 202a 2070 742e 6c6f 6728 322e  * n) * pt.log(2.
-00008af0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00008b00: 2020 202b 206e 202a 2067 616d 6d61 6c6e     + n * gammaln
-00008b10: 286e 202f 2032 290a 2020 2020 2020 2020  (n / 2).        
-00008b20: 2020 2020 2020 2020 2d20 286e 202d 2031          - (n - 1
-00008b30: 2920 2a20 6761 6d6d 616c 6e28 6e29 0a20  ) * gammaln(n). 
-00008b40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008b50: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00008b60: 6573 756c 7420 3d20 2d28 6e20 2d20 3129  esult = -(n - 1)
-00008b70: 202a 2067 616d 6d61 6c6e 2865 7461 202b   * gammaln(eta +
-00008b80: 2030 2e35 202a 2028 6e20 2d20 3129 290a   0.5 * (n - 1)).
-00008b90: 2020 2020 2020 2020 6b20 3d20 7074 2e61          k = pt.a
-00008ba0: 7261 6e67 6528 312c 206e 290a 2020 2020  range(1, n).    
-00008bb0: 2020 2020 7265 7375 6c74 202b 3d20 2830      result += (0
-00008bc0: 2e35 202a 206b 202a 2070 742e 6c6f 6728  .5 * k * pt.log(
-00008bd0: 6e70 2e70 6929 202b 2067 616d 6d61 6c6e  np.pi) + gammaln
-00008be0: 2865 7461 202b 2030 2e35 202a 2028 6e20  (eta + 0.5 * (n 
-00008bf0: 2d20 3120 2d20 6b29 2929 2e73 756d 2829  - 1 - k))).sum()
-00008c00: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-00008c10: 6c74 0a0a 0a63 6c61 7373 205f 4c4b 4a43  lt...class _LKJC
-00008c20: 686f 6c65 736b 7943 6f76 4261 7365 5256  holeskyCovBaseRV
-00008c30: 2852 616e 646f 6d56 6172 6961 626c 6529  (RandomVariable)
-00008c40: 3a0a 2020 2020 6e61 6d65 203d 2022 5f6c  :.    name = "_l
-00008c50: 6b6a 6368 6f6c 6573 6b79 636f 7662 6173  kjcholeskycovbas
-00008c60: 6522 0a20 2020 206e 6469 6d5f 7375 7070  e".    ndim_supp
-00008c70: 203d 2031 0a20 2020 206e 6469 6d73 5f70   = 1.    ndims_p
-00008c80: 6172 616d 7320 3d20 5b30 2c20 302c 2031  arams = [0, 0, 1
-00008c90: 5d0a 2020 2020 6474 7970 6520 3d20 2266  ].    dtype = "f
-00008ca0: 6c6f 6174 5822 0a20 2020 205f 7072 696e  loatX".    _prin
-00008cb0: 745f 6e61 6d65 203d 2028 225f 6c6b 6a63  t_name = ("_lkjc
-00008cc0: 686f 6c65 736b 7963 6f76 6261 7365 222c  holeskycovbase",
-00008cd0: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-00008ce0: 7b5f 6c6b 6a63 686f 6c65 736b 7963 6f76  {_lkjcholeskycov
-00008cf0: 6261 7365 7d22 290a 0a20 2020 2064 6566  base}")..    def
-00008d00: 206d 616b 655f 6e6f 6465 2873 656c 662c   make_node(self,
-00008d10: 2072 6e67 2c20 7369 7a65 2c20 6474 7970   rng, size, dtyp
-00008d20: 652c 206e 2c20 6574 612c 2044 293a 0a20  e, n, eta, D):. 
-00008d30: 2020 2020 2020 206e 203d 2070 742e 6173         n = pt.as
-00008d40: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00008d50: 286e 290a 2020 2020 2020 2020 6966 206e  (n).        if n
-00008d60: 6f74 206e 2e6e 6469 6d20 3d3d 2030 3a0a  ot n.ndim == 0:.
-00008d70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008d80: 6520 5661 6c75 6545 7272 6f72 2822 6e20  e ValueError("n 
-00008d90: 6d75 7374 2062 6520 6120 7363 616c 6172  must be a scalar
-00008da0: 2028 6e64 696d 3d30 292e 2229 0a0a 2020   (ndim=0).")..  
-00008db0: 2020 2020 2020 6574 6120 3d20 7074 2e61        eta = pt.a
-00008dc0: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-00008dd0: 6528 6574 6129 0a20 2020 2020 2020 2069  e(eta).        i
-00008de0: 6620 6e6f 7420 6574 612e 6e64 696d 203d  f not eta.ndim =
-00008df0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00008e00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00008e10: 7228 2265 7461 206d 7573 7420 6265 2061  r("eta must be a
-00008e20: 2073 6361 6c61 7220 286e 6469 6d3d 3029   scalar (ndim=0)
-00008e30: 2e22 290a 0a20 2020 2020 2020 2044 203d  .")..        D =
-00008e40: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00008e50: 7269 6162 6c65 2844 290a 0a20 2020 2020  riable(D)..     
-00008e60: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-00008e70: 292e 6d61 6b65 5f6e 6f64 6528 726e 672c  ).make_node(rng,
-00008e80: 2073 697a 652c 2064 7479 7065 2c20 6e2c   size, dtype, n,
-00008e90: 2065 7461 2c20 4429 0a0a 2020 2020 6465   eta, D)..    de
-00008ea0: 6620 5f73 7570 705f 7368 6170 655f 6672  f _supp_shape_fr
-00008eb0: 6f6d 5f70 6172 616d 7328 7365 6c66 2c20  om_params(self, 
-00008ec0: 6469 7374 5f70 6172 616d 732c 2070 6172  dist_params, par
-00008ed0: 616d 5f73 6861 7065 7329 3a0a 2020 2020  am_shapes):.    
-00008ee0: 2020 2020 6e20 3d20 6469 7374 5f70 6172      n = dist_par
-00008ef0: 616d 735b 305d 0a20 2020 2020 2020 2072  ams[0].        r
-00008f00: 6574 7572 6e20 2828 6e20 2a20 286e 202b  eturn ((n * (n +
-00008f10: 2031 2929 202f 2f20 322c 290a 0a20 2020   1)) // 2,)..   
-00008f20: 2064 6566 2072 6e67 5f66 6e28 7365 6c66   def rng_fn(self
-00008f30: 2c20 726e 672c 206e 2c20 6574 612c 2044  , rng, n, eta, D
-00008f40: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
-00008f50: 2023 2057 6520 666c 6174 7465 6e20 7468   # We flatten th
-00008f60: 6520 7369 7a65 2074 6f20 6d61 6b65 206f  e size to make o
-00008f70: 7065 7261 7469 6f6e 7320 6561 7369 6572  perations easier
-00008f80: 2c20 616e 6420 7468 656e 2072 6562 7569  , and then rebui
-00008f90: 6c64 2069 740a 2020 2020 2020 2020 6966  ld it.        if
-00008fa0: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
-00008fb0: 2020 2020 2020 2020 2020 2073 697a 6520             size 
-00008fc0: 3d20 442e 7368 6170 655b 3a2d 315d 0a20  = D.shape[:-1]. 
-00008fd0: 2020 2020 2020 2066 6c61 745f 7369 7a65         flat_size
-00008fe0: 203d 206e 702e 7072 6f64 2873 697a 6529   = np.prod(size)
-00008ff0: 2e61 7374 7970 6528 696e 7429 0a0a 2020  .astype(int)..  
-00009000: 2020 2020 2020 4320 3d20 4c4b 4a43 6f72        C = LKJCor
-00009010: 7252 562e 5f72 616e 646f 6d5f 636f 7272  rRV._random_corr
-00009020: 5f6d 6174 7269 7828 726e 673d 726e 672c  _matrix(rng=rng,
-00009030: 206e 3d6e 2c20 6574 613d 6574 612c 2066   n=n, eta=eta, f
-00009040: 6c61 745f 7369 7a65 3d66 6c61 745f 7369  lat_size=flat_si
-00009050: 7a65 290a 2020 2020 2020 2020 4420 3d20  ze).        D = 
-00009060: 442e 7265 7368 6170 6528 666c 6174 5f73  D.reshape(flat_s
-00009070: 697a 652c 206e 290a 2020 2020 2020 2020  ize, n).        
-00009080: 4320 2a3d 2044 5b2e 2e2e 2c20 3a2c 206e  C *= D[..., :, n
-00009090: 702e 6e65 7761 7869 735d 202a 2044 5b2e  p.newaxis] * D[.
-000090a0: 2e2e 2c20 6e70 2e6e 6577 6178 6973 2c20  .., np.newaxis, 
-000090b0: 3a5d 0a0a 2020 2020 2020 2020 7472 696c  :]..        tril
-000090c0: 5f69 6478 203d 206e 702e 7472 696c 5f69  _idx = np.tril_i
-000090d0: 6e64 6963 6573 286e 2c20 6b3d 3029 0a20  ndices(n, k=0). 
-000090e0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
-000090f0: 206e 702e 6c69 6e61 6c67 2e63 686f 6c65   np.linalg.chole
-00009100: 736b 7928 4329 5b2e 2e2e 2c20 7472 696c  sky(C)[..., tril
-00009110: 5f69 6478 5b30 5d2c 2074 7269 6c5f 6964  _idx[0], tril_id
-00009120: 785b 315d 5d0a 0a20 2020 2020 2020 2069  x[1]]..        i
-00009130: 6620 7369 7a65 2069 7320 4e6f 6e65 3a0a  f size is None:.
-00009140: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
-00009150: 6c65 7320 3d20 7361 6d70 6c65 735b 305d  les = samples[0]
-00009160: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00009170: 2020 2020 2020 2020 2020 2064 6973 745f             dist_
-00009180: 7368 6170 6520 3d20 286e 202a 2028 6e20  shape = (n * (n 
-00009190: 2b20 3129 2920 2f2f 2032 0a20 2020 2020  + 1)) // 2.     
-000091a0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
-000091b0: 206e 702e 7265 7368 6170 6528 7361 6d70   np.reshape(samp
-000091c0: 6c65 732c 2028 2a73 697a 652c 2064 6973  les, (*size, dis
-000091d0: 745f 7368 6170 6529 290a 0a20 2020 2020  t_shape))..     
-000091e0: 2020 2072 6574 7572 6e20 7361 6d70 6c65     return sample
-000091f0: 730a 0a0a 5f6c 6a6b 5f63 686f 6c65 736b  s..._ljk_cholesk
-00009200: 795f 636f 765f 6261 7365 203d 205f 4c4b  y_cov_base = _LK
-00009210: 4a43 686f 6c65 736b 7943 6f76 4261 7365  JCholeskyCovBase
-00009220: 5256 2829 0a0a 0a23 205f 4c4b 4a43 686f  RV()...# _LKJCho
-00009230: 6c65 736b 7943 6f76 4261 7365 5256 2072  leskyCovBaseRV r
-00009240: 6571 7569 7265 7320 6120 7072 6f70 6572  equires a proper
-00009250: 6c79 2073 6861 7065 6420 6044 602c 2077  ly shaped `D`, w
-00009260: 6869 6368 206d 6561 6e73 2074 6865 2076  hich means the v
-00009270: 6172 6961 626c 6520 6361 6e27 740a 2320  ariable can't.# 
-00009280: 6265 2073 6166 656c 7920 7265 7369 7a65  be safely resize
-00009290: 642e 2042 6563 6175 7365 206f 6620 7468  d. Because of th
-000092a0: 6973 2c20 7765 2061 6464 2074 6865 2074  is, we add the t
-000092b0: 6869 6e20 5379 6d62 6f6c 6963 5261 6e64  hin SymbolicRand
-000092c0: 6f6d 5661 7269 6162 6c65 2077 7261 7070  omVariable wrapp
-000092d0: 6572 0a63 6c61 7373 205f 4c4b 4a43 686f  er.class _LKJCho
-000092e0: 6c65 736b 7943 6f76 5256 2853 796d 626f  leskyCovRV(Symbo
-000092f0: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
-00009300: 6529 3a0a 2020 2020 6465 6661 756c 745f  e):.    default_
-00009310: 6f75 7470 7574 203d 2031 0a20 2020 205f  output = 1.    _
-00009320: 7072 696e 745f 6e61 6d65 203d 2028 225f  print_name = ("_
-00009330: 6c6b 6a63 686f 6c65 736b 7963 6f76 222c  lkjcholeskycov",
-00009340: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-00009350: 7b5f 6c6b 6a63 686f 6c65 736b 7963 6f76  {_lkjcholeskycov
-00009360: 7d22 290a 0a20 2020 2064 6566 2075 7064  }")..    def upd
-00009370: 6174 6528 7365 6c66 2c20 6e6f 6465 293a  ate(self, node):
-00009380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009390: 7b6e 6f64 652e 696e 7075 7473 5b30 5d3a  {node.inputs[0]:
-000093a0: 206e 6f64 652e 6f75 7470 7574 735b 305d   node.outputs[0]
-000093b0: 7d0a 0a0a 636c 6173 7320 5f4c 4b4a 4368  }...class _LKJCh
-000093c0: 6f6c 6573 6b79 436f 7628 4469 7374 7269  oleskyCov(Distri
-000093d0: 6275 7469 6f6e 293a 0a20 2020 2072 2222  bution):.    r""
-000093e0: 2255 6e64 6572 6c79 696e 6720 636c 6173  "Underlying clas
-000093f0: 7320 666f 7220 636f 7661 7269 616e 6365  s for covariance
-00009400: 206d 6174 7269 7820 7769 7468 204c 4b4a   matrix with LKJ
-00009410: 2064 6973 7472 6962 7574 6564 2063 6f72   distributed cor
-00009420: 7265 6c61 7469 6f6e 732e 0a20 2020 2053  relations..    S
-00009430: 6565 2064 6f63 7320 666f 7220 4c4b 4a43  ee docs for LKJC
-00009440: 686f 6c65 736b 7943 6f76 2066 756e 6374  holeskyCov funct
-00009450: 696f 6e20 666f 7220 6d6f 7265 2064 6574  ion for more det
-00009460: 6169 6c73 206f 6e20 686f 7720 746f 2075  ails on how to u
-00009470: 7365 2069 7420 696e 206d 6f64 656c 732e  se it in models.
-00009480: 0a20 2020 2022 2222 0a0a 2020 2020 7276  .    """..    rv
-00009490: 5f74 7970 6520 3d20 5f4c 4b4a 4368 6f6c  _type = _LKJChol
-000094a0: 6573 6b79 436f 7652 560a 0a20 2020 2040  eskyCovRV..    @
-000094b0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-000094c0: 6465 6620 6469 7374 2863 6c73 2c20 6e2c  def dist(cls, n,
-000094d0: 2065 7461 2c20 7364 5f64 6973 742c 202a   eta, sd_dist, *
-000094e0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-000094f0: 2020 6e20 3d20 7074 2e61 735f 7465 6e73    n = pt.as_tens
-00009500: 6f72 5f76 6172 6961 626c 6528 696e 7458  or_variable(intX
-00009510: 286e 2929 0a20 2020 2020 2020 2065 7461  (n)).        eta
-00009520: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-00009530: 7661 7269 6162 6c65 2866 6c6f 6174 5828  variable(floatX(
-00009540: 6574 6129 290a 0a20 2020 2020 2020 2069  eta))..        i
-00009550: 6620 6e6f 7420 280a 2020 2020 2020 2020  f not (.        
-00009560: 2020 2020 6973 696e 7374 616e 6365 2873      isinstance(s
-00009570: 645f 6469 7374 2c20 5661 7269 6162 6c65  d_dist, Variable
-00009580: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
-00009590: 6420 7364 5f64 6973 742e 6f77 6e65 7220  d sd_dist.owner 
-000095a0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-000095b0: 2020 2020 2020 2020 616e 6420 6973 696e          and isin
-000095c0: 7374 616e 6365 2873 645f 6469 7374 2e6f  stance(sd_dist.o
-000095d0: 776e 6572 2e6f 702c 2028 5261 6e64 6f6d  wner.op, (Random
-000095e0: 5661 7269 6162 6c65 2c20 5379 6d62 6f6c  Variable, Symbol
-000095f0: 6963 5261 6e64 6f6d 5661 7269 6162 6c65  icRandomVariable
-00009600: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
-00009610: 6e64 2073 645f 6469 7374 2e6f 776e 6572  nd sd_dist.owner
-00009620: 2e6f 702e 6e64 696d 5f73 7570 7020 3c20  .op.ndim_supp < 
-00009630: 320a 2020 2020 2020 2020 293a 0a20 2020  2.        ):.   
-00009640: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00009650: 7970 6545 7272 6f72 2822 7364 5f64 6973  ypeError("sd_dis
-00009660: 7420 6d75 7374 2062 6520 6120 7363 616c  t must be a scal
-00009670: 6172 206f 7220 7665 6374 6f72 2064 6973  ar or vector dis
-00009680: 7472 6962 7574 696f 6e20 7661 7269 6162  tribution variab
-00009690: 6c65 2229 0a0a 2020 2020 2020 2020 6368  le")..        ch
-000096a0: 6563 6b5f 6469 7374 5f6e 6f74 5f72 6567  eck_dist_not_reg
-000096b0: 6973 7465 7265 6428 7364 5f64 6973 7429  istered(sd_dist)
-000096c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000096d0: 7375 7065 7228 292e 6469 7374 285b 6e2c  super().dist([n,
-000096e0: 2065 7461 2c20 7364 5f64 6973 745d 2c20   eta, sd_dist], 
-000096f0: 2a2a 6b77 6172 6773 290a 0a20 2020 2040  **kwargs)..    @
-00009700: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00009710: 6465 6620 7276 5f6f 7028 636c 732c 206e  def rv_op(cls, n
-00009720: 2c20 6574 612c 2073 645f 6469 7374 2c20  , eta, sd_dist, 
-00009730: 7369 7a65 3d4e 6f6e 6529 3a0a 2020 2020  size=None):.    
-00009740: 2020 2020 2320 5765 2072 6573 697a 6520      # We resize 
-00009750: 7468 6520 7364 5f64 6973 7420 6175 746f  the sd_dist auto
-00009760: 6d61 7469 6361 6c6c 7920 736f 2074 6861  matically so tha
-00009770: 7420 6974 2068 6173 2028 7369 7a65 2078  t it has (size x
-00009780: 206e 2920 696e 6465 7065 6e64 656e 740a   n) independent.
-00009790: 2020 2020 2020 2020 2320 6472 6177 7320          # draws 
-000097a0: 7768 6963 6820 6973 2077 6861 7420 7468  which is what th
-000097b0: 6520 605f 4c4b 4a43 686f 6c65 736b 7943  e `_LKJCholeskyC
-000097c0: 6f76 4261 7365 5256 2e72 6e67 5f66 6e60  ovBaseRV.rng_fn`
-000097d0: 2065 7870 6563 7473 2e20 5468 6973 206d   expects. This m
-000097e0: 616b 6573 2074 6865 0a20 2020 2020 2020  akes the.       
-000097f0: 2023 2072 616e 646f 6d20 616e 6420 6c6f   # random and lo
-00009800: 6770 206d 6574 686f 6473 2065 7175 6976  gp methods equiv
-00009810: 616c 656e 742c 2061 7320 7468 6520 6c61  alent, as the la
-00009820: 7474 6572 2061 6c73 6f20 6173 7375 6d65  tter also assume
-00009830: 7320 6120 756e 6971 7565 2076 616c 7565  s a unique value
-00009840: 0a20 2020 2020 2020 2023 2066 6f72 2065  .        # for e
-00009850: 6163 6820 6469 6167 6f6e 616c 2065 6c65  ach diagonal ele
-00009860: 6d65 6e74 2e0a 2020 2020 2020 2020 2320  ment..        # 
-00009870: 5369 6e63 6520 6065 7461 6020 616e 6420  Since `eta` and 
-00009880: 606e 6020 6172 6520 666f 7263 6564 2074  `n` are forced t
-00009890: 6f20 6265 2073 6361 6c61 7273 2077 6520  o be scalars we 
-000098a0: 646f 6e27 7420 6e65 6564 2074 6f20 776f  don't need to wo
-000098b0: 7272 7920 6162 6f75 740a 2020 2020 2020  rry about.      
-000098c0: 2020 2320 696d 706c 6965 6420 6261 7463    # implied batc
-000098d0: 6865 6420 6469 6d65 6e73 696f 6e73 2066  hed dimensions f
-000098e0: 726f 6d20 7468 6f73 6520 666f 7220 7468  rom those for th
-000098f0: 6520 7469 6d65 2062 6569 6e67 2e0a 2020  e time being..  
-00009900: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
-00009910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009920: 2020 2073 697a 6520 3d20 7364 5f64 6973     size = sd_dis
-00009930: 742e 7368 6170 655b 3a2d 315d 0a20 2020  t.shape[:-1].   
-00009940: 2020 2020 2073 6861 7065 203d 2074 7570       shape = tup
-00009950: 6c65 2873 697a 6529 202b 2028 6e2c 290a  le(size) + (n,).
-00009960: 2020 2020 2020 2020 6966 2073 645f 6469          if sd_di
-00009970: 7374 2e6f 776e 6572 2e6f 702e 6e64 696d  st.owner.op.ndim
-00009980: 5f73 7570 7020 3d3d 2030 3a0a 2020 2020  _supp == 0:.    
-00009990: 2020 2020 2020 2020 7364 5f64 6973 7420          sd_dist 
-000099a0: 3d20 6368 616e 6765 5f64 6973 745f 7369  = change_dist_si
-000099b0: 7a65 2873 645f 6469 7374 2c20 7368 6170  ze(sd_dist, shap
-000099c0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-000099d0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-000099e0: 6865 2073 7570 706f 7274 2073 6861 7065  he support shape
-000099f0: 206d 7573 7420 6265 2060 6e60 2062 7574   must be `n` but
-00009a00: 2077 6520 6861 7665 206e 6f20 7761 7920   we have no way 
-00009a10: 6f66 2063 6f6e 7472 6f6c 6c69 6e67 2069  of controlling i
-00009a20: 740a 2020 2020 2020 2020 2020 2020 7364  t.            sd
-00009a30: 5f64 6973 7420 3d20 6368 616e 6765 5f64  _dist = change_d
-00009a40: 6973 745f 7369 7a65 2873 645f 6469 7374  ist_size(sd_dist
-00009a50: 2c20 7368 6170 655b 3a2d 315d 290a 0a20  , shape[:-1]).. 
-00009a60: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-00009a70: 6e65 7720 726e 6720 666f 7220 7468 6520  new rng for the 
-00009a80: 5f6c 6b6a 6368 6f6c 6573 6b79 636f 7620  _lkjcholeskycov 
-00009a90: 696e 7465 726e 616c 2052 560a 2020 2020  internal RV.    
-00009aa0: 2020 2020 726e 6720 3d20 7079 7465 6e73      rng = pytens
-00009ab0: 6f72 2e73 6861 7265 6428 6e70 2e72 616e  or.shared(np.ran
-00009ac0: 646f 6d2e 6465 6661 756c 745f 726e 6728  dom.default_rng(
-00009ad0: 2929 0a0a 2020 2020 2020 2020 726e 675f  ))..        rng_
-00009ae0: 2c20 6e5f 2c20 6574 615f 2c20 7364 5f64  , n_, eta_, sd_d
-00009af0: 6973 745f 203d 2072 6e67 2e74 7970 6528  ist_ = rng.type(
-00009b00: 292c 206e 2e74 7970 6528 292c 2065 7461  ), n.type(), eta
-00009b10: 2e74 7970 6528 292c 2073 645f 6469 7374  .type(), sd_dist
-00009b20: 2e74 7970 6528 290a 2020 2020 2020 2020  .type().        
-00009b30: 6e65 7874 5f72 6e67 5f2c 206c 6b6a 636f  next_rng_, lkjco
-00009b40: 765f 203d 205f 6c6a 6b5f 6368 6f6c 6573  v_ = _ljk_choles
-00009b50: 6b79 5f63 6f76 5f62 6173 6528 6e5f 2c20  ky_cov_base(n_, 
-00009b60: 6574 615f 2c20 7364 5f64 6973 745f 2c20  eta_, sd_dist_, 
-00009b70: 726e 673d 726e 675f 292e 6f77 6e65 722e  rng=rng_).owner.
-00009b80: 6f75 7470 7574 730a 0a20 2020 2020 2020  outputs..       
-00009b90: 2072 6574 7572 6e20 5f4c 4b4a 4368 6f6c   return _LKJChol
-00009ba0: 6573 6b79 436f 7652 5628 0a20 2020 2020  eskyCovRV(.     
-00009bb0: 2020 2020 2020 2069 6e70 7574 733d 5b72         inputs=[r
-00009bc0: 6e67 5f2c 206e 5f2c 2065 7461 5f2c 2073  ng_, n_, eta_, s
-00009bd0: 645f 6469 7374 5f5d 2c0a 2020 2020 2020  d_dist_],.      
-00009be0: 2020 2020 2020 6f75 7470 7574 733d 5b6e        outputs=[n
-00009bf0: 6578 745f 726e 675f 2c20 6c6b 6a63 6f76  ext_rng_, lkjcov
-00009c00: 5f5d 2c0a 2020 2020 2020 2020 2020 2020  _],.            
-00009c10: 6e64 696d 5f73 7570 703d 312c 0a20 2020  ndim_supp=1,.   
-00009c20: 2020 2020 2029 2872 6e67 2c20 6e2c 2065       )(rng, n, e
-00009c30: 7461 2c20 7364 5f64 6973 7429 0a0a 0a40  ta, sd_dist)...@
-00009c40: 5f63 6861 6e67 655f 6469 7374 5f73 697a  _change_dist_siz
-00009c50: 652e 7265 6769 7374 6572 285f 4c4b 4a43  e.register(_LKJC
-00009c60: 686f 6c65 736b 7943 6f76 5256 290a 6465  holeskyCovRV).de
-00009c70: 6620 6368 616e 6765 5f4c 4b4a 4368 6f6c  f change_LKJChol
-00009c80: 656b 7379 436f 7652 565f 7369 7a65 286f  eksyCovRV_size(o
-00009c90: 702c 2064 6973 742c 206e 6577 5f73 697a  p, dist, new_siz
-00009ca0: 652c 2065 7870 616e 643d 4661 6c73 6529  e, expand=False)
-00009cb0: 3a0a 2020 2020 6e2c 2065 7461 2c20 7364  :.    n, eta, sd
-00009cc0: 5f64 6973 7420 3d20 6469 7374 2e6f 776e  _dist = dist.own
-00009cd0: 6572 2e69 6e70 7574 735b 313a 5d0a 0a20  er.inputs[1:].. 
-00009ce0: 2020 2069 6620 6578 7061 6e64 3a0a 2020     if expand:.  
-00009cf0: 2020 2020 2020 6f6c 645f 7369 7a65 203d        old_size =
-00009d00: 2073 645f 6469 7374 2e73 6861 7065 5b3a   sd_dist.shape[:
-00009d10: 2d31 5d0a 2020 2020 2020 2020 6e65 775f  -1].        new_
-00009d20: 7369 7a65 203d 2074 7570 6c65 286e 6577  size = tuple(new
-00009d30: 5f73 697a 6529 202b 2074 7570 6c65 286f  _size) + tuple(o
-00009d40: 6c64 5f73 697a 6529 0a0a 2020 2020 7265  ld_size)..    re
-00009d50: 7475 726e 205f 4c4b 4a43 686f 6c65 736b  turn _LKJCholesk
-00009d60: 7943 6f76 2e72 765f 6f70 286e 2c20 6574  yCov.rv_op(n, et
-00009d70: 612c 2073 645f 6469 7374 2c20 7369 7a65  a, sd_dist, size
-00009d80: 3d6e 6577 5f73 697a 6529 0a0a 0a40 5f6d  =new_size)...@_m
-00009d90: 6f6d 656e 742e 7265 6769 7374 6572 285f  oment.register(_
-00009da0: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
-00009db0: 290a 6465 6620 5f4c 4b4a 4368 6f6c 656b  ).def _LKJCholek
-00009dc0: 7379 436f 7652 565f 6d6f 6d65 6e74 286f  syCovRV_moment(o
-00009dd0: 702c 2072 762c 2072 6e67 2c20 6e2c 2065  p, rv, rng, n, e
-00009de0: 7461 2c20 7364 5f64 6973 7429 3a0a 2020  ta, sd_dist):.  
-00009df0: 2020 6469 6167 5f69 6478 7320 3d20 2870    diag_idxs = (p
-00009e00: 742e 6375 6d73 756d 2870 742e 6172 616e  t.cumsum(pt.aran
-00009e10: 6765 2831 2c20 6e20 2b20 3129 2920 2d20  ge(1, n + 1)) - 
-00009e20: 3129 2e61 7374 7970 6528 2269 6e74 3332  1).astype("int32
-00009e30: 2229 0a20 2020 206d 6f6d 656e 7420 3d20  ").    moment = 
-00009e40: 7074 2e7a 6572 6f73 5f6c 696b 6528 7276  pt.zeros_like(rv
-00009e50: 290a 2020 2020 6d6f 6d65 6e74 203d 2070  ).    moment = p
-00009e60: 742e 7365 745f 7375 6274 656e 736f 7228  t.set_subtensor(
-00009e70: 6d6f 6d65 6e74 5b2e 2e2e 2c20 6469 6167  moment[..., diag
-00009e80: 5f69 6478 735d 2c20 3129 0a20 2020 2072  _idxs], 1).    r
-00009e90: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 0a40  eturn moment...@
-00009ea0: 5f64 6566 6175 6c74 5f74 7261 6e73 666f  _default_transfo
-00009eb0: 726d 2e72 6567 6973 7465 7228 5f4c 4b4a  rm.register(_LKJ
-00009ec0: 4368 6f6c 6573 6b79 436f 7652 5629 0a64  CholeskyCovRV).d
-00009ed0: 6566 205f 4c4b 4a43 686f 6c65 6b73 7943  ef _LKJCholeksyC
-00009ee0: 6f76 5256 5f64 6566 6175 6c74 5f74 7261  ovRV_default_tra
-00009ef0: 6e73 666f 726d 286f 702c 2072 7629 3a0a  nsform(op, rv):.
-00009f00: 2020 2020 5f2c 206e 2c20 5f2c 205f 203d      _, n, _, _ =
-00009f10: 2072 762e 6f77 6e65 722e 696e 7075 7473   rv.owner.inputs
-00009f20: 0a20 2020 2072 6574 7572 6e20 7472 616e  .    return tran
-00009f30: 7366 6f72 6d73 2e43 686f 6c65 736b 7943  sforms.CholeskyC
-00009f40: 6f76 5061 636b 6564 286e 290a 0a0a 405f  ovPacked(n)...@_
-00009f50: 6c6f 6770 726f 622e 7265 6769 7374 6572  logprob.register
-00009f60: 285f 4c4b 4a43 686f 6c65 736b 7943 6f76  (_LKJCholeskyCov
-00009f70: 5256 290a 6465 6620 5f4c 4b4a 4368 6f6c  RV).def _LKJChol
-00009f80: 656b 7379 436f 7652 565f 6c6f 6770 286f  eksyCovRV_logp(o
-00009f90: 702c 2076 616c 7565 732c 2072 6e67 2c20  p, values, rng, 
-00009fa0: 6e2c 2065 7461 2c20 7364 5f64 6973 742c  n, eta, sd_dist,
-00009fb0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00009fc0: 2876 616c 7565 2c29 203d 2076 616c 7565  (value,) = value
-00009fd0: 730a 0a20 2020 2069 6620 7661 6c75 652e  s..    if value.
-00009fe0: 6e64 696d 203e 2031 3a0a 2020 2020 2020  ndim > 1:.      
-00009ff0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000a000: 6f72 2822 5f4c 4b4a 4368 6f6c 6573 6b79  or("_LKJCholesky
-0000a010: 436f 7620 6c6f 6770 2069 7320 6f6e 6c79  Cov logp is only
-0000a020: 2069 6d70 6c65 6d65 6e74 6564 2066 6f72   implemented for
-0000a030: 2076 6563 746f 7220 7661 6c75 6573 2028   vector values (
-0000a040: 6e64 696d 3d31 2922 290a 0a20 2020 2064  ndim=1)")..    d
-0000a050: 6961 675f 6964 7873 203d 2070 742e 6375  iag_idxs = pt.cu
-0000a060: 6d73 756d 2870 742e 6172 616e 6765 2831  msum(pt.arange(1
-0000a070: 2c20 6e20 2b20 3129 2920 2d20 310a 2020  , n + 1)) - 1.  
-0000a080: 2020 6375 6d73 756d 203d 2070 742e 6375    cumsum = pt.cu
-0000a090: 6d73 756d 2876 616c 7565 2a2a 3229 0a20  msum(value**2). 
-0000a0a0: 2020 2076 6172 6961 6e63 6520 3d20 7074     variance = pt
-0000a0b0: 2e7a 6572 6f73 2870 742e 6174 6c65 6173  .zeros(pt.atleas
-0000a0c0: 745f 3164 286e 2929 0a20 2020 2076 6172  t_1d(n)).    var
-0000a0d0: 6961 6e63 6520 3d20 7074 2e69 6e63 5f73  iance = pt.inc_s
-0000a0e0: 7562 7465 6e73 6f72 2876 6172 6961 6e63  ubtensor(varianc
-0000a0f0: 655b 305d 2c20 7661 6c75 655b 305d 202a  e[0], value[0] *
-0000a100: 2a20 3229 0a20 2020 2076 6172 6961 6e63  * 2).    varianc
-0000a110: 6520 3d20 7074 2e69 6e63 5f73 7562 7465  e = pt.inc_subte
-0000a120: 6e73 6f72 2876 6172 6961 6e63 655b 313a  nsor(variance[1:
-0000a130: 5d2c 2063 756d 7375 6d5b 6469 6167 5f69  ], cumsum[diag_i
-0000a140: 6478 735b 313a 5d5d 202d 2063 756d 7375  dxs[1:]] - cumsu
-0000a150: 6d5b 6469 6167 5f69 6478 735b 3a2d 315d  m[diag_idxs[:-1]
-0000a160: 5d29 0a20 2020 2073 645f 7661 6c73 203d  ]).    sd_vals =
-0000a170: 2070 742e 7371 7274 2876 6172 6961 6e63   pt.sqrt(varianc
-0000a180: 6529 0a0a 2020 2020 6c6f 6770 5f73 6420  e)..    logp_sd 
-0000a190: 3d20 706d 2e6c 6f67 7028 7364 5f64 6973  = pm.logp(sd_dis
-0000a1a0: 742c 2073 645f 7661 6c73 292e 7375 6d28  t, sd_vals).sum(
-0000a1b0: 290a 2020 2020 636f 7272 5f64 6961 6720  ).    corr_diag 
-0000a1c0: 3d20 7661 6c75 655b 6469 6167 5f69 6478  = value[diag_idx
-0000a1d0: 735d 202f 2073 645f 7661 6c73 0a0a 2020  s] / sd_vals..  
-0000a1e0: 2020 6c6f 6770 5f6c 6b6a 203d 2028 3220    logp_lkj = (2 
-0000a1f0: 2a20 6574 6120 2d20 3320 2b20 6e20 2d20  * eta - 3 + n - 
-0000a200: 7074 2e61 7261 6e67 6528 6e29 2920 2a20  pt.arange(n)) * 
-0000a210: 7074 2e6c 6f67 2863 6f72 725f 6469 6167  pt.log(corr_diag
-0000a220: 290a 2020 2020 6c6f 6770 5f6c 6b6a 203d  ).    logp_lkj =
-0000a230: 2070 742e 7375 6d28 6c6f 6770 5f6c 6b6a   pt.sum(logp_lkj
-0000a240: 290a 0a20 2020 2023 2043 6f6d 7075 7465  )..    # Compute
-0000a250: 2074 6865 206c 6f67 2064 6574 206a 6163   the log det jac
-0000a260: 6f62 6961 6e20 6f66 2074 6865 2073 6563  obian of the sec
-0000a270: 6f6e 6420 7472 616e 7366 6f72 6d61 7469  ond transformati
-0000a280: 6f6e 0a20 2020 2023 2064 6573 6372 6962  on.    # describ
-0000a290: 6564 2069 6e20 7468 6520 646f 6373 7472  ed in the docstr
-0000a2a0: 696e 672e 0a20 2020 2069 6478 203d 2070  ing..    idx = p
-0000a2b0: 742e 6172 616e 6765 286e 290a 2020 2020  t.arange(n).    
-0000a2c0: 6465 745f 696e 766a 6163 203d 2070 742e  det_invjac = pt.
-0000a2d0: 6c6f 6728 636f 7272 5f64 6961 6729 202d  log(corr_diag) -
-0000a2e0: 2069 6478 202a 2070 742e 6c6f 6728 7364   idx * pt.log(sd
-0000a2f0: 5f76 616c 7329 0a20 2020 2064 6574 5f69  _vals).    det_i
-0000a300: 6e76 6a61 6320 3d20 6465 745f 696e 766a  nvjac = det_invj
-0000a310: 6163 2e73 756d 2829 0a0a 2020 2020 2320  ac.sum()..    # 
-0000a320: 544f 444f 3a20 5f6c 6b6a 5f6e 6f72 6d61  TODO: _lkj_norma
-0000a330: 6c69 7a69 6e67 5f63 6f6e 7374 616e 7420  lizing_constant 
-0000a340: 6375 7272 656e 746c 7920 7265 7175 6972  currently requir
-0000a350: 6573 2060 6574 6160 2061 6e64 2060 6e60  es `eta` and `n`
-0000a360: 2074 6f20 6265 2063 6f6e 7374 616e 7473   to be constants
-0000a370: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
-0000a380: 7374 616e 6365 286e 2c20 436f 6e73 7461  stance(n, Consta
-0000a390: 6e74 293a 0a20 2020 2020 2020 2072 6169  nt):.        rai
-0000a3a0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-0000a3b0: 6445 7272 6f72 2822 6c6f 6770 206f 6e6c  dError("logp onl
-0000a3c0: 7920 696d 706c 656d 656e 7465 6420 666f  y implemented fo
-0000a3d0: 7220 636f 6e73 7461 6e74 2060 6e60 2229  r constant `n`")
-0000a3e0: 0a20 2020 206e 203d 2069 6e74 286e 2e64  .    n = int(n.d
-0000a3f0: 6174 6129 0a0a 2020 2020 6966 206e 6f74  ata)..    if not
-0000a400: 2069 7369 6e73 7461 6e63 6528 6574 612c   isinstance(eta,
-0000a410: 2043 6f6e 7374 616e 7429 3a0a 2020 2020   Constant):.    
-0000a420: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000a430: 6c65 6d65 6e74 6564 4572 726f 7228 226c  lementedError("l
-0000a440: 6f67 7020 6f6e 6c79 2069 6d70 6c65 6d65  ogp only impleme
-0000a450: 6e74 6564 2066 6f72 2063 6f6e 7374 616e  nted for constan
-0000a460: 7420 6065 7461 6022 290a 2020 2020 6574  t `eta`").    et
-0000a470: 6120 3d20 666c 6f61 7428 6574 612e 6461  a = float(eta.da
-0000a480: 7461 290a 0a20 2020 206e 6f72 6d20 3d20  ta)..    norm = 
-0000a490: 5f6c 6b6a 5f6e 6f72 6d61 6c69 7a69 6e67  _lkj_normalizing
-0000a4a0: 5f63 6f6e 7374 616e 7428 6574 612c 206e  _constant(eta, n
-0000a4b0: 290a 0a20 2020 2072 6574 7572 6e20 6e6f  )..    return no
-0000a4c0: 726d 202b 206c 6f67 705f 6c6b 6a20 2b20  rm + logp_lkj + 
-0000a4d0: 6c6f 6770 5f73 6420 2b20 6465 745f 696e  logp_sd + det_in
-0000a4e0: 766a 6163 0a0a 0a63 6c61 7373 204c 4b4a  vjac...class LKJ
-0000a4f0: 4368 6f6c 6573 6b79 436f 763a 0a20 2020  CholeskyCov:.   
-0000a500: 2072 2222 2257 7261 7070 6572 2063 6c61   r"""Wrapper cla
-0000a510: 7373 2066 6f72 2063 6f76 6172 6961 6e63  ss for covarianc
-0000a520: 6520 6d61 7472 6978 2077 6974 6820 4c4b  e matrix with LK
-0000a530: 4a20 6469 7374 7269 6275 7465 6420 636f  J distributed co
-0000a540: 7272 656c 6174 696f 6e73 2e0a 0a20 2020  rrelations...   
-0000a550: 2054 6869 7320 6465 6669 6e65 7320 6120   This defines a 
-0000a560: 6469 7374 7269 6275 7469 6f6e 206f 7665  distribution ove
-0000a570: 7220 4368 6f6c 6573 6b79 2064 6563 6f6d  r Cholesky decom
-0000a580: 706f 7365 6420 636f 7661 7269 616e 6365  posed covariance
-0000a590: 0a20 2020 206d 6174 7269 6365 732c 2073  .    matrices, s
-0000a5a0: 7563 6820 7468 6174 2074 6865 2075 6e64  uch that the und
-0000a5b0: 6572 6c79 696e 6720 636f 7272 656c 6174  erlying correlat
-0000a5c0: 696f 6e20 6d61 7472 6963 6573 2066 6f6c  ion matrices fol
-0000a5d0: 6c6f 7720 616e 0a20 2020 204c 4b4a 2064  low an.    LKJ d
-0000a5e0: 6973 7472 6962 7574 696f 6e20 5b31 5d20  istribution [1] 
-0000a5f0: 616e 6420 7468 6520 7374 616e 6461 7264  and the standard
-0000a600: 2064 6576 6961 7469 6f6e 7320 666f 6c6c   deviations foll
-0000a610: 6f77 2061 6e20 6172 6269 7472 6172 790a  ow an arbitrary.
-0000a620: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
-0000a630: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
-0000a640: 6520 7573 6572 2e0a 0a20 2020 2050 6172  e user...    Par
-0000a650: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0000a660: 2d2d 2d2d 2d2d 0a20 2020 206e 616d 6520  ------.    name 
-0000a670: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
-0000a680: 6520 6e61 6d65 2067 6976 656e 2074 6f20  e name given to 
-0000a690: 7468 6520 7661 7269 6162 6c65 2069 6e20  the variable in 
-0000a6a0: 7468 6520 6d6f 6465 6c2e 0a20 2020 2065  the model..    e
-0000a6b0: 7461 203a 2074 656e 736f 725f 6c69 6b65  ta : tensor_like
-0000a6c0: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
-0000a6d0: 2020 5468 6520 7368 6170 6520 7061 7261    The shape para
-0000a6e0: 6d65 7465 7220 2865 7461 203e 2030 2920  meter (eta > 0) 
-0000a6f0: 6f66 2074 6865 204c 4b4a 2064 6973 7472  of the LKJ distr
-0000a700: 6962 7574 696f 6e2e 2065 7461 203d 2031  ibution. eta = 1
-0000a710: 0a20 2020 2020 2020 2069 6d70 6c69 6573  .        implies
-0000a720: 2061 2075 6e69 666f 726d 2064 6973 7472   a uniform distr
-0000a730: 6962 7574 696f 6e20 6f66 2074 6865 2063  ibution of the c
-0000a740: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
-0000a750: 6365 733b 0a20 2020 2020 2020 206c 6172  ces;.        lar
-0000a760: 6765 7220 7661 6c75 6573 2070 7574 206d  ger values put m
-0000a770: 6f72 6520 7765 6967 6874 206f 6e20 6d61  ore weight on ma
-0000a780: 7472 6963 6573 2077 6974 6820 6665 7720  trices with few 
-0000a790: 636f 7272 656c 6174 696f 6e73 2e0a 2020  correlations..  
-0000a7a0: 2020 6e20 3a20 7465 6e73 6f72 5f6c 696b    n : tensor_lik
-0000a7b0: 6520 6f66 2069 6e74 0a20 2020 2020 2020  e of int.       
-0000a7c0: 2044 696d 656e 7369 6f6e 206f 6620 7468   Dimension of th
-0000a7d0: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
-0000a7e0: 7269 7820 286e 203e 2031 292e 0a20 2020  rix (n > 1)..   
-0000a7f0: 2073 645f 6469 7374 203a 2044 6973 7472   sd_dist : Distr
-0000a800: 6962 7574 696f 6e0a 2020 2020 2020 2020  ibution.        
-0000a810: 4120 706f 7369 7469 7665 2073 6361 6c61  A positive scala
-0000a820: 7220 6f72 2076 6563 746f 7220 6469 7374  r or vector dist
-0000a830: 7269 6275 7469 6f6e 2066 6f72 2074 6865  ribution for the
-0000a840: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-0000a850: 696f 6e73 2c20 6372 6561 7465 640a 2020  ions, created.  
-0000a860: 2020 2020 2020 7769 7468 2074 6865 2060        with the `
-0000a870: 2e64 6973 7428 2960 2041 5049 2e20 5368  .dist()` API. Sh
-0000a880: 6f75 6c64 2068 6176 6520 6073 6861 7065  ould have `shape
-0000a890: 5b2d 315d 3d6e 602e 2053 6361 6c61 7220  [-1]=n`. Scalar 
-0000a8a0: 6469 7374 7269 6275 7469 6f6e 7320 7769  distributions wi
-0000a8b0: 6c6c 2062 650a 2020 2020 2020 2020 6175  ll be.        au
-0000a8c0: 746f 6d61 7469 6361 6c6c 7920 7265 7369  tomatically resi
-0000a8d0: 7a65 6420 746f 2065 6e73 7572 6520 7468  zed to ensure th
-0000a8e0: 6973 2e0a 0a20 2020 2020 2020 202e 2e20  is...        .. 
-0000a8f0: 7761 726e 696e 673a 3a20 7364 5f64 6973  warning:: sd_dis
-0000a900: 7420 7769 6c6c 2062 6520 636c 6f6e 6564  t will be cloned
-0000a910: 2c20 7265 6e64 6572 696e 6720 6974 2069  , rendering it i
-0000a920: 6e64 6570 656e 6465 6e74 206f 6620 7468  ndependent of th
-0000a930: 6520 6f6e 6520 7061 7373 6564 2061 7320  e one passed as 
-0000a940: 696e 7075 742e 0a0a 2020 2020 636f 6d70  input...    comp
-0000a950: 7574 655f 636f 7272 203a 2062 6f6f 6c2c  ute_corr : bool,
-0000a960: 2064 6566 6175 6c74 3d54 7275 650a 2020   default=True.  
-0000a970: 2020 2020 2020 4966 2060 5472 7565 602c        If `True`,
-0000a980: 2072 6574 7572 6e73 2074 6872 6565 2076   returns three v
-0000a990: 616c 7565 733a 2074 6865 2043 686f 6c65  alues: the Chole
-0000a9a0: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
-0000a9b0: 6e2c 2074 6865 2063 6f72 7265 6c61 7469  n, the correlati
-0000a9c0: 6f6e 730a 2020 2020 2020 2020 616e 6420  ons.        and 
-0000a9d0: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
-0000a9e0: 6961 7469 6f6e 7320 6f66 2074 6865 2063  iations of the c
-0000a9f0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000aa00: 2e20 4f74 6865 7277 6973 652c 206f 6e6c  . Otherwise, onl
-0000aa10: 7920 7265 7475 726e 730a 2020 2020 2020  y returns.      
-0000aa20: 2020 7468 6520 7061 636b 6564 2043 686f    the packed Cho
-0000aa30: 6c65 736b 7920 6465 636f 6d70 6f73 6974  lesky decomposit
-0000aa40: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
-0000aa50: 2060 5472 7565 602e 0a20 2020 2020 2020   `True`..       
-0000aa60: 2063 6f6d 7061 7469 6269 6c69 7479 2e0a   compatibility..
-0000aa70: 2020 2020 7374 6f72 655f 696e 5f74 7261      store_in_tra
-0000aa80: 6365 203a 2062 6f6f 6c2c 2064 6566 6175  ce : bool, defau
-0000aa90: 6c74 3d54 7275 650a 2020 2020 2020 2020  lt=True.        
-0000aaa0: 5768 6574 6865 7220 746f 2073 746f 7265  Whether to store
-0000aab0: 2074 6865 2063 6f72 7265 6c61 7469 6f6e   the correlation
-0000aac0: 7320 616e 6420 7374 616e 6461 7264 2064  s and standard d
-0000aad0: 6576 6961 7469 6f6e 7320 6f66 2074 6865  eviations of the
-0000aae0: 2063 6f76 6172 6961 6e63 650a 2020 2020   covariance.    
-0000aaf0: 2020 2020 6d61 7472 6978 2069 6e20 7468      matrix in th
-0000ab00: 6520 706f 7374 6572 696f 7220 7472 6163  e posterior trac
-0000ab10: 652e 2049 6620 6054 7275 6560 2c20 7468  e. If `True`, th
-0000ab20: 6579 2077 696c 6c20 6175 746f 6d61 7469  ey will automati
-0000ab30: 6361 6c6c 7920 6265 206e 616d 6564 2061  cally be named a
-0000ab40: 730a 2020 2020 2020 2020 607b 6e61 6d65  s.        `{name
-0000ab50: 7d5f 636f 7272 6020 616e 6420 607b 6e61  }_corr` and `{na
-0000ab60: 6d65 7d5f 7374 6473 6020 7265 7370 6563  me}_stds` respec
-0000ab70: 7469 7665 6c79 2e20 4566 6665 6374 6976  tively. Effectiv
-0000ab80: 6520 6f6e 6c79 2077 6865 6e0a 2020 2020  e only when.    
-0000ab90: 2020 2020 6063 6f6d 7075 7465 5f63 6f72      `compute_cor
-0000aba0: 723d 5472 7565 602e 0a0a 2020 2020 5265  r=True`...    Re
-0000abb0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-0000abc0: 2d0a 2020 2020 6368 6f6c 203a 2020 5465  -.    chol :  Te
-0000abd0: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
-0000abe0: 2020 2020 2049 6620 6063 6f6d 7075 7465       If `compute
-0000abf0: 5f63 6f72 723d 5472 7565 602e 2054 6865  _corr=True`. The
-0000ac00: 2075 6e70 6163 6b65 6420 4368 6f6c 6573   unpacked Choles
-0000ac10: 6b79 2063 6f76 6172 6961 6e63 6520 6465  ky covariance de
-0000ac20: 636f 6d70 6f73 6974 696f 6e2e 0a20 2020  composition..   
-0000ac30: 2063 6f72 7220 3a20 5465 6e73 6f72 5661   corr : TensorVa
-0000ac40: 7269 6162 6c65 0a20 2020 2020 2020 2049  riable.        I
-0000ac50: 6620 6063 6f6d 7075 7465 5f63 6f72 723d  f `compute_corr=
-0000ac60: 5472 7565 602e 2054 6865 2063 6f72 7265  True`. The corre
-0000ac70: 6c61 7469 6f6e 7320 6f66 2074 6865 2063  lations of the c
-0000ac80: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000ac90: 2e0a 2020 2020 7374 6473 203a 2054 656e  ..    stds : Ten
-0000aca0: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
-0000acb0: 2020 2020 4966 2060 636f 6d70 7574 655f      If `compute_
-0000acc0: 636f 7272 3d54 7275 6560 2e20 5468 6520  corr=True`. The 
-0000acd0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0000ace0: 6f6e 7320 6f66 2074 6865 2063 6f76 6172  ons of the covar
-0000acf0: 6961 6e63 6520 6d61 7472 6978 2e0a 2020  iance matrix..  
-0000ad00: 2020 7061 636b 6564 5f63 686f 6c20 3a20    packed_chol : 
-0000ad10: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
-0000ad20: 2020 2020 2020 2049 6620 6063 6f6d 7075         If `compu
-0000ad30: 7465 5f63 6f72 723d 4661 6c73 6560 2054  te_corr=False` T
-0000ad40: 6865 2070 6163 6b65 6420 4368 6f6c 6573  he packed Choles
-0000ad50: 6b79 2063 6f76 6172 6961 6e63 6520 6465  ky covariance de
-0000ad60: 636f 6d70 6f73 6974 696f 6e2e 0a0a 2020  composition...  
-0000ad70: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-0000ad80: 2d0a 2020 2020 5369 6e63 6520 7468 6520  -.    Since the 
-0000ad90: 4368 6f6c 6573 6b79 2066 6163 746f 7220  Cholesky factor 
-0000ada0: 6973 2061 206c 6f77 6572 2074 7269 616e  is a lower trian
-0000adb0: 6775 6c61 7220 6d61 7472 6978 2c20 7765  gular matrix, we
-0000adc0: 2075 7365 2070 6163 6b65 6420 7374 6f72   use packed stor
-0000add0: 6167 6520 666f 720a 2020 2020 7468 6520  age for.    the 
-0000ade0: 6d61 7472 6978 3a20 5765 2073 746f 7265  matrix: We store
-0000adf0: 2074 6865 2076 616c 7565 7320 6f66 2074   the values of t
-0000ae00: 6865 206c 6f77 6572 2074 7269 616e 6775  he lower triangu
-0000ae10: 6c61 7220 6d61 7472 6978 2069 6e20 6120  lar matrix in a 
-0000ae20: 6f6e 652d 6469 6d65 6e73 696f 6e61 6c0a  one-dimensional.
-0000ae30: 2020 2020 6172 7261 792c 206e 756d 6265      array, numbe
-0000ae40: 7265 6420 6279 2072 6f77 3a3a 0a0a 2020  red by row::..  
-0000ae50: 2020 2020 2020 5b5b 3020 2d20 2d20 2d5d        [[0 - - -]
-0000ae60: 0a20 2020 2020 2020 2020 5b31 2032 202d  .         [1 2 -
-0000ae70: 202d 5d0a 2020 2020 2020 2020 205b 3320   -].         [3 
-0000ae80: 3420 3520 2d5d 0a20 2020 2020 2020 2020  4 5 -].         
-0000ae90: 5b36 2037 2038 2039 5d5d 0a0a 2020 2020  [6 7 8 9]]..    
-0000aea0: 5468 6520 756e 7061 636b 6564 2043 686f  The unpacked Cho
-0000aeb0: 6c65 736b 7920 636f 7661 7269 616e 6365  lesky covariance
-0000aec0: 206d 6174 7269 7820 6973 2061 7574 6f6d   matrix is autom
-0000aed0: 6174 6963 616c 6c79 2063 6f6d 7075 7465  atically compute
-0000aee0: 6420 616e 6420 7265 7475 726e 6564 2077  d and returned w
-0000aef0: 6865 6e0a 2020 2020 796f 7520 7370 6563  hen.    you spec
-0000af00: 6966 7920 6063 6f6d 7075 7465 5f63 6f72  ify `compute_cor
-0000af10: 723d 5472 7565 6020 696e 2060 706d 2e4c  r=True` in `pm.L
-0000af20: 4b4a 4368 6f6c 6573 6b79 436f 7660 2028  KJCholeskyCov` (
-0000af30: 7365 6520 6578 616d 706c 6520 6265 6c6f  see example belo
-0000af40: 7729 2e0a 2020 2020 4f74 6865 7277 6973  w)..    Otherwis
-0000af50: 652c 2079 6f75 2063 616e 2075 7365 2060  e, you can use `
-0000af60: 706d 2e65 7870 616e 645f 7061 636b 6564  pm.expand_packed
-0000af70: 5f74 7269 616e 6775 6c61 7228 7061 636b  _triangular(pack
-0000af80: 6564 5f63 6f76 2c20 6c6f 7765 723d 5472  ed_cov, lower=Tr
-0000af90: 7565 2960 0a20 2020 2074 6f20 636f 6e76  ue)`.    to conv
-0000afa0: 6572 7420 7468 6520 7061 636b 6564 2043  ert the packed C
-0000afb0: 686f 6c65 736b 7920 6d61 7472 6978 2074  holesky matrix t
-0000afc0: 6f20 6120 7265 6775 6c61 7220 7477 6f2d  o a regular two-
-0000afd0: 6469 6d65 6e73 696f 6e61 6c20 6172 7261  dimensional arra
-0000afe0: 792e 0a0a 2020 2020 4578 616d 706c 6573  y...    Examples
-0000aff0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0000b000: 2020 2e2e 2063 6f64 653a 3a20 7079 7468    .. code:: pyth
-0000b010: 6f6e 0a0a 2020 2020 2020 2020 7769 7468  on..        with
-0000b020: 2070 6d2e 4d6f 6465 6c28 2920 6173 206d   pm.Model() as m
-0000b030: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-0000b040: 2020 2320 4e6f 7465 2074 6861 7420 7765    # Note that we
-0000b050: 2061 6363 6573 7320 7468 6520 6469 7374   access the dist
-0000b060: 7269 6275 7469 6f6e 2066 6f72 2074 6865  ribution for the
-0000b070: 2073 7461 6e64 6172 640a 2020 2020 2020   standard.      
-0000b080: 2020 2020 2020 2320 6465 7669 6174 696f        # deviatio
-0000b090: 6e73 2c20 616e 6420 646f 206e 6f74 2063  ns, and do not c
-0000b0a0: 7265 6174 6520 6120 6e65 7720 7261 6e64  reate a new rand
-0000b0b0: 6f6d 2076 6172 6961 626c 652e 0a20 2020  om variable..   
-0000b0c0: 2020 2020 2020 2020 2073 645f 6469 7374           sd_dist
-0000b0d0: 203d 2070 6d2e 4578 706f 6e65 6e74 6961   = pm.Exponentia
-0000b0e0: 6c2e 6469 7374 2831 2e30 2c20 7369 7a65  l.dist(1.0, size
-0000b0f0: 3d31 3029 0a20 2020 2020 2020 2020 2020  =10).           
-0000b100: 2063 686f 6c2c 2063 6f72 722c 2073 6967   chol, corr, sig
-0000b110: 6d61 7320 3d20 706d 2e4c 4b4a 4368 6f6c  mas = pm.LKJChol
-0000b120: 6573 6b79 436f 7628 0a20 2020 2020 2020  eskyCov(.       
-0000b130: 2020 2020 2020 2020 2027 6368 6f6c 5f63           'chol_c
-0000b140: 6f76 272c 2065 7461 3d34 2c20 6e3d 3130  ov', eta=4, n=10
-0000b150: 2c20 7364 5f64 6973 743d 7364 5f64 6973  , sd_dist=sd_dis
-0000b160: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
-0000b170: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0000b180: 6620 796f 7520 6f6e 6c79 2077 616e 7420  f you only want 
-0000b190: 7468 6520 7061 636b 6564 2043 686f 6c65  the packed Chole
-0000b1a0: 736b 793a 0a20 2020 2020 2020 2020 2020  sky:.           
-0000b1b0: 2023 2070 6163 6b65 645f 6368 6f6c 203d   # packed_chol =
-0000b1c0: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
-0000b1d0: 6f76 280a 2020 2020 2020 2020 2020 2020  ov(.            
-0000b1e0: 2020 2020 2763 686f 6c5f 636f 7627 2c20      'chol_cov', 
-0000b1f0: 6574 613d 342c 206e 3d31 302c 2073 645f  eta=4, n=10, sd_
-0000b200: 6469 7374 3d73 645f 6469 7374 2c20 636f  dist=sd_dist, co
-0000b210: 6d70 7574 655f 636f 7272 3d46 616c 7365  mpute_corr=False
-0000b220: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000b230: 2020 2020 2020 2020 2020 2023 2063 686f             # cho
-0000b240: 6c20 3d20 706d 2e65 7870 616e 645f 7061  l = pm.expand_pa
-0000b250: 636b 6564 5f74 7269 616e 6775 6c61 7228  cked_triangular(
-0000b260: 3130 2c20 7061 636b 6564 5f63 686f 6c2c  10, packed_chol,
-0000b270: 206c 6f77 6572 3d54 7275 6529 0a0a 2020   lower=True)..  
-0000b280: 2020 2020 2020 2020 2020 2320 4465 6669            # Defi
-0000b290: 6e65 2061 206e 6577 204d 764e 6f72 6d61  ne a new MvNorma
-0000b2a0: 6c20 7769 7468 2074 6865 2067 6976 656e  l with the given
-0000b2b0: 2063 6f76 6172 6961 6e63 650a 2020 2020   covariance.    
-0000b2c0: 2020 2020 2020 2020 7661 6c73 203d 2070          vals = p
-0000b2d0: 6d2e 4d76 4e6f 726d 616c 2827 7661 6c73  m.MvNormal('vals
-0000b2e0: 272c 206d 753d 6e70 2e7a 6572 6f73 2831  ', mu=np.zeros(1
-0000b2f0: 3029 2c20 6368 6f6c 3d63 686f 6c2c 2073  0), chol=chol, s
-0000b300: 6861 7065 3d31 3029 0a0a 2020 2020 2020  hape=10)..      
-0000b310: 2020 2020 2020 2320 4f72 2074 7261 6e73        # Or trans
-0000b320: 666f 726d 2061 6e20 756e 636f 7272 656c  form an uncorrel
-0000b330: 6174 6564 206e 6f72 6d61 6c3a 0a20 2020  ated normal:.   
-0000b340: 2020 2020 2020 2020 2076 616c 735f 7261           vals_ra
-0000b350: 7720 3d20 706d 2e4e 6f72 6d61 6c28 2776  w = pm.Normal('v
-0000b360: 616c 735f 7261 7727 2c20 6d75 3d30 2c20  als_raw', mu=0, 
-0000b370: 7369 676d 613d 312c 2073 6861 7065 3d31  sigma=1, shape=1
-0000b380: 3029 0a20 2020 2020 2020 2020 2020 2076  0).            v
-0000b390: 616c 7320 3d20 7074 2e64 6f74 2863 686f  als = pt.dot(cho
-0000b3a0: 6c2c 2076 616c 735f 7261 7729 0a0a 2020  l, vals_raw)..  
-0000b3b0: 2020 2020 2020 2020 2020 2320 4f72 2063            # Or c
-0000b3c0: 6f6d 7075 7465 2074 6865 2063 6f76 6172  ompute the covar
-0000b3d0: 6961 6e63 6520 6d61 7472 6978 0a20 2020  iance matrix.   
-0000b3e0: 2020 2020 2020 2020 2063 6f76 203d 2070           cov = p
-0000b3f0: 742e 646f 7428 6368 6f6c 2c20 6368 6f6c  t.dot(chol, chol
-0000b400: 2e54 290a 0a20 2020 202a 2a49 6d70 6c65  .T)..    **Imple
-0000b410: 6d65 6e74 6174 696f 6e2a 2a20 496e 2074  mentation** In t
-0000b420: 6865 2075 6e63 6f6e 7374 7261 696e 6564  he unconstrained
-0000b430: 2073 7061 6365 2061 6c6c 2076 616c 7565   space all value
-0000b440: 7320 6f66 2074 6865 2063 686f 6c65 736b  s of the cholesk
-0000b450: 7920 6661 6374 6f72 0a20 2020 2061 7265  y factor.    are
-0000b460: 2073 746f 7265 6420 756e 7472 616e 7366   stored untransf
-0000b470: 6f72 6d65 642c 2065 7863 6570 7420 666f  ormed, except fo
-0000b480: 7220 7468 6520 6469 6167 6f6e 616c 2065  r the diagonal e
-0000b490: 6e74 7269 6573 2c20 7768 6572 650a 2020  ntries, where.  
-0000b4a0: 2020 7765 2075 7365 2061 206c 6f67 2d74    we use a log-t
-0000b4b0: 7261 6e73 666f 726d 2074 6f20 7265 7374  ransform to rest
-0000b4c0: 7269 6374 2074 6865 6d20 746f 2070 6f73  rict them to pos
-0000b4d0: 6974 6976 6520 7661 6c75 6573 2e0a 0a20  itive values... 
-0000b4e0: 2020 2054 6f20 636f 7272 6563 746c 7920     To correctly 
-0000b4f0: 636f 6d70 7574 6520 6c6f 672d 6c69 6b65  compute log-like
-0000b500: 6c69 686f 6f64 7320 666f 7220 7468 6520  lihoods for the 
-0000b510: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0000b520: 6f6e 730a 2020 2020 616e 6420 7468 6520  ons.    and the 
-0000b530: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
-0000b540: 6978 2073 6570 6172 6174 656c 792c 2077  ix separately, w
-0000b550: 6520 6e65 6564 2074 6f20 636f 6e73 6964  e need to consid
-0000b560: 6572 2061 0a20 2020 2073 6563 6f6e 6420  er a.    second 
-0000b570: 7472 616e 7366 6f72 6d61 7469 6f6e 3a20  transformation: 
-0000b580: 4769 7665 6e20 6120 6368 6f6c 6573 6b79  Given a cholesky
-0000b590: 2066 6163 746f 7269 7a61 7469 6f6e 0a20   factorization. 
-0000b5a0: 2020 203a 6d61 7468 3a60 4c4c 5e54 203d     :math:`LL^T =
-0000b5b0: 205c 5369 676d 6160 206f 6620 6120 636f   \Sigma` of a co
-0000b5c0: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
-0000b5d0: 7765 2063 616e 2072 6563 6f76 6572 2074  we can recover t
-0000b5e0: 6865 0a20 2020 2073 7461 6e64 6172 6420  he.    standard 
-0000b5f0: 6465 7669 6174 696f 6e73 203a 6d61 7468  deviations :math
-0000b600: 3a60 5c73 6967 6d61 6020 6173 2074 6865  :`\sigma` as the
-0000b610: 2065 7563 6c69 6465 616e 206c 656e 6774   euclidean lengt
-0000b620: 6873 206f 660a 2020 2020 7468 6520 726f  hs of.    the ro
-0000b630: 7773 206f 6620 3a6d 6174 683a 604c 602c  ws of :math:`L`,
-0000b640: 2061 6e64 2074 6865 2063 686f 6c65 736b   and the cholesk
-0000b650: 7920 6661 6374 6f72 206f 6620 7468 650a  y factor of the.
-0000b660: 2020 2020 636f 7272 656c 6174 696f 6e20      correlation 
-0000b670: 6d61 7472 6978 2061 7320 3a6d 6174 683a  matrix as :math:
-0000b680: 6055 203d 205c 7465 7874 7b64 6961 677d  `U = \text{diag}
-0000b690: 285c 7369 676d 6129 5e7b 2d31 7d4c 602e  (\sigma)^{-1}L`.
-0000b6a0: 0a20 2020 2053 696e 6365 2065 6163 6820  .    Since each 
-0000b6b0: 726f 7720 6f66 203a 6d61 7468 3a60 5560  row of :math:`U`
-0000b6c0: 2068 6173 206c 656e 6774 6820 312c 2077   has length 1, w
-0000b6d0: 6520 646f 206e 6f74 206e 6565 6420 746f  e do not need to
-0000b6e0: 0a20 2020 2073 746f 7265 2074 6865 2064  .    store the d
-0000b6f0: 6961 676f 6e61 6c2e 2057 6520 6465 6669  iagonal. We defi
-0000b700: 6e65 2061 2074 7261 6e73 666f 726d 6174  ne a transformat
-0000b710: 696f 6e20 3a6d 6174 683a 605c 7068 6960  ion :math:`\phi`
-0000b720: 0a20 2020 2073 7563 6820 7468 6174 203a  .    such that :
-0000b730: 6d61 7468 3a60 5c70 6869 284c 2960 2069  math:`\phi(L)` i
-0000b740: 7320 7468 6520 6c6f 7765 7220 7472 6961  s the lower tria
-0000b750: 6e67 756c 6172 206d 6174 7269 7820 636f  ngular matrix co
-0000b760: 6e74 6169 6e69 6e67 0a20 2020 2074 6865  ntaining.    the
-0000b770: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-0000b780: 696f 6e73 203a 6d61 7468 3a60 5c73 6967  ions :math:`\sig
-0000b790: 6d61 6020 6f6e 2074 6865 2064 6961 676f  ma` on the diago
-0000b7a0: 6e61 6c20 616e 6420 7468 650a 2020 2020  nal and the.    
-0000b7b0: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
-0000b7c0: 6978 203a 6d61 7468 3a60 5560 2062 656c  ix :math:`U` bel
-0000b7d0: 6f77 2e20 496e 2074 6869 7320 666f 726d  ow. In this form
-0000b7e0: 2077 6520 6361 6e20 6561 7369 6c79 0a20   we can easily. 
-0000b7f0: 2020 2063 6f6d 7075 7465 2074 6865 2064     compute the d
-0000b800: 6966 6665 7265 6e74 206c 696b 656c 6968  ifferent likelih
-0000b810: 6f6f 6473 2073 6570 6172 6174 656c 792c  oods separately,
-0000b820: 2061 7320 7468 6520 6c69 6b65 6c69 686f   as the likeliho
-0000b830: 6f64 0a20 2020 206f 6620 7468 6520 636f  od.    of the co
-0000b840: 7272 656c 6174 696f 6e20 6d61 7472 6978  rrelation matrix
-0000b850: 206f 6e6c 7920 6465 7065 6e64 7320 6f6e   only depends on
-0000b860: 2074 6865 2076 616c 7565 7320 6265 6c6f   the values belo
-0000b870: 7720 7468 650a 2020 2020 6469 6167 6f6e  w the.    diagon
-0000b880: 616c 2c20 616e 6420 7468 6520 6c69 6b65  al, and the like
-0000b890: 6c69 686f 6f64 206f 6620 7468 6520 7374  lihood of the st
-0000b8a0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0000b8b0: 2064 6570 656e 6473 0a20 2020 206f 6e6c   depends.    onl
-0000b8c0: 7920 6f6e 2074 6865 2064 6961 676f 6e61  y on the diagona
-0000b8d0: 6c20 7661 6c75 6573 2e0a 0a20 2020 2057  l values...    W
-0000b8e0: 6520 7374 696c 6c20 6e65 6564 2074 6865  e still need the
-0000b8f0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
-0000b900: 7468 6520 6a61 636f 6269 616e 206f 6620  the jacobian of 
-0000b910: 3a6d 6174 683a 605c 7068 695e 7b2d 317d  :math:`\phi^{-1}
-0000b920: 602e 0a20 2020 2049 6620 7765 2074 6869  `..    If we thi
-0000b930: 6e6b 206f 6620 3a6d 6174 683a 605c 7068  nk of :math:`\ph
-0000b940: 6960 2061 7320 616e 2061 7574 6f6d 6f72  i` as an automor
-0000b950: 7068 6973 6d20 6f6e 0a20 2020 203a 6d61  phism on.    :ma
-0000b960: 7468 3a60 5c6d 6174 6862 627b 527d 5e7b  th:`\mathbb{R}^{
-0000b970: 5c74 6672 6163 7b6e 286e 2b31 297d 7b32  \tfrac{n(n+1)}{2
-0000b980: 7d7d 602c 2077 6865 7265 2077 6520 6f72  }}`, where we or
-0000b990: 6465 720a 2020 2020 7468 6520 6469 6d65  der.    the dime
-0000b9a0: 6e73 696f 6e73 2061 7320 6465 7363 7269  nsions as descri
-0000b9b0: 6265 6420 696e 2074 6865 206e 6f74 6573  bed in the notes
-0000b9c0: 2061 626f 7665 2c20 7468 6520 6a61 636f   above, the jaco
-0000b9d0: 6269 616e 0a20 2020 2069 7320 6120 626c  bian.    is a bl
-0000b9e0: 6f63 6b2d 6469 6167 6f6e 616c 206d 6174  ock-diagonal mat
-0000b9f0: 7269 782c 2077 6865 7265 2065 6163 6820  rix, where each 
-0000ba00: 626c 6f63 6b20 636f 7272 6573 706f 6e64  block correspond
-0000ba10: 7320 746f 0a20 2020 206f 6e65 2072 6f77  s to.    one row
-0000ba20: 206f 6620 3a6d 6174 683a 6055 602e 2045   of :math:`U`. E
-0000ba30: 6163 6820 626c 6f63 6b20 6861 7320 6172  ach block has ar
-0000ba40: 726f 7768 6561 6420 7368 6170 652c 2061  rowhead shape, a
-0000ba50: 6e64 2077 650a 2020 2020 6361 6e20 636f  nd we.    can co
-0000ba60: 6d70 7574 6520 7468 6520 6465 7465 726d  mpute the determ
-0000ba70: 696e 616e 7420 6f66 2074 6861 7420 6173  inant of that as
-0000ba80: 2064 6573 6372 6962 6564 2069 6e20 5b32   described in [2
-0000ba90: 5d2e 2053 696e 6365 0a20 2020 2074 6865  ]. Since.    the
-0000baa0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
-0000bab0: 6120 626c 6f63 6b2d 6469 6167 6f6e 616c  a block-diagonal
-0000bac0: 206d 6174 7269 7820 6973 2074 6865 2070   matrix is the p
-0000bad0: 726f 6475 6374 0a20 2020 206f 6620 7468  roduct.    of th
-0000bae0: 6520 6465 7465 726d 696e 616e 7473 206f  e determinants o
-0000baf0: 6620 7468 6520 626c 6f63 6b73 2c20 7765  f the blocks, we
-0000bb00: 2067 6574 0a0a 2020 2020 2e2e 206d 6174   get..    .. mat
-0000bb10: 683a 3a0a 0a20 2020 2020 2020 5c74 6578  h::..       \tex
-0000bb20: 747b 6465 747d 284a 5f7b 5c70 6869 5e7b  t{det}(J_{\phi^{
-0000bb30: 2d31 7d7d 2855 2929 203d 0a20 2020 2020  -1}}(U)) =.     
-0000bb40: 2020 5c6c 6566 745b 0a20 2020 2020 2020    \left[.       
-0000bb50: 2020 5c70 726f 645f 7b69 3d32 7d5e 4e20    \prod_{i=2}^N 
-0000bb60: 755f 7b69 697d 5e7b 6920 2d20 317d 204c  u_{ii}^{i - 1} L
-0000bb70: 5f7b 6969 7d0a 2020 2020 2020 205c 7269  _{ii}.       \ri
-0000bb80: 6768 745d 5e7b 2d31 7d0a 0a20 2020 2052  ght]^{-1}..    R
-0000bb90: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
-0000bba0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
-0000bbb0: 5b31 5d20 4c65 7761 6e64 6f77 736b 692c  [1] Lewandowski,
-0000bbc0: 2044 2e2c 204b 7572 6f77 6963 6b61 2c20   D., Kurowicka, 
-0000bbd0: 442e 2061 6e64 204a 6f65 2c20 482e 2028  D. and Joe, H. (
-0000bbe0: 3230 3039 292e 0a20 2020 2020 2020 2247  2009)..       "G
-0000bbf0: 656e 6572 6174 696e 6720 7261 6e64 6f6d  enerating random
-0000bc00: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
-0000bc10: 7269 6365 7320 6261 7365 6420 6f6e 2076  rices based on v
-0000bc20: 696e 6573 2061 6e64 0a20 2020 2020 2020  ines and.       
-0000bc30: 6578 7465 6e64 6564 206f 6e69 6f6e 206d  extended onion m
-0000bc40: 6574 686f 642e 2220 4a6f 7572 6e61 6c20  ethod." Journal 
-0000bc50: 6f66 206d 756c 7469 7661 7269 6174 6520  of multivariate 
-0000bc60: 616e 616c 7973 6973 2c0a 2020 2020 2020  analysis,.      
-0000bc70: 2031 3030 2839 292c 2070 702e 3139 3839   100(9), pp.1989
-0000bc80: 2d32 3030 312e 0a0a 2020 2020 2e2e 205b  -2001...    .. [
-0000bc90: 325d 204a 2e20 4d2e 2069 736e 2774 2061  2] J. M. isn't a
-0000bca0: 206d 6174 6865 6d61 7469 6369 616e 2028   mathematician (
-0000bcb0: 6874 7470 3a2f 2f6d 6174 682e 7374 6163  http://math.stac
-0000bcc0: 6b65 7863 6861 6e67 652e 636f 6d2f 7573  kexchange.com/us
-0000bcd0: 6572 732f 3439 382f 0a20 2020 2020 2020  ers/498/.       
-0000bce0: 6a2d 6d2d 6973 6e74 2d61 2d6d 6174 6865  j-m-isnt-a-mathe
-0000bcf0: 6d61 7469 6369 616e 292c 2044 6966 6665  matician), Diffe
-0000bd00: 7265 6e74 2061 7070 726f 6163 6865 7320  rent approaches 
-0000bd10: 746f 2065 7661 6c75 6174 6520 7468 6973  to evaluate this
-0000bd20: 0a20 2020 2020 2020 6465 7465 726d 696e  .       determin
-0000bd30: 616e 742c 2055 524c 2028 7665 7273 696f  ant, URL (versio
-0000bd40: 6e3a 2032 3031 322d 3034 2d31 3429 3a0a  n: 2012-04-14):.
-0000bd50: 2020 2020 2020 2068 7474 703a 2f2f 6d61         http://ma
-0000bd60: 7468 2e73 7461 636b 6578 6368 616e 6765  th.stackexchange
-0000bd70: 2e63 6f6d 2f71 2f31 3330 3032 360a 2020  .com/q/130026.  
-0000bd80: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0000bd90: 5f6e 6577 5f5f 2863 6c73 2c20 6e61 6d65  _new__(cls, name
-0000bda0: 2c20 6574 612c 206e 2c20 7364 5f64 6973  , eta, n, sd_dis
-0000bdb0: 742c 202a 2c20 636f 6d70 7574 655f 636f  t, *, compute_co
-0000bdc0: 7272 3d54 7275 652c 2073 746f 7265 5f69  rr=True, store_i
-0000bdd0: 6e5f 7472 6163 653d 5472 7565 2c20 2a2a  n_trace=True, **
-0000bde0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-0000bdf0: 2070 6163 6b65 645f 6368 6f6c 203d 205f   packed_chol = _
-0000be00: 4c4b 4a43 686f 6c65 736b 7943 6f76 286e  LKJCholeskyCov(n
-0000be10: 616d 652c 2065 7461 3d65 7461 2c20 6e3d  ame, eta=eta, n=
-0000be20: 6e2c 2073 645f 6469 7374 3d73 645f 6469  n, sd_dist=sd_di
-0000be30: 7374 2c20 2a2a 6b77 6172 6773 290a 2020  st, **kwargs).  
-0000be40: 2020 2020 2020 6966 206e 6f74 2063 6f6d        if not com
-0000be50: 7075 7465 5f63 6f72 723a 0a20 2020 2020  pute_corr:.     
-0000be60: 2020 2020 2020 2072 6574 7572 6e20 7061         return pa
-0000be70: 636b 6564 5f63 686f 6c0a 2020 2020 2020  cked_chol.      
-0000be80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000be90: 2020 2020 6368 6f6c 2c20 636f 7272 2c20      chol, corr, 
-0000bea0: 7374 6473 203d 2063 6c73 2e68 656c 7065  stds = cls.helpe
-0000beb0: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
-0000bec0: 286e 2c20 7061 636b 6564 5f63 686f 6c29  (n, packed_chol)
-0000bed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bee0: 7374 6f72 655f 696e 5f74 7261 6365 3a0a  store_in_trace:.
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 636f 7272 203d 2070 6d2e 4465 7465 726d  corr = pm.Determ
-0000bf10: 696e 6973 7469 6328 6622 7b6e 616d 657d  inistic(f"{name}
-0000bf20: 5f63 6f72 7222 2c20 636f 7272 290a 2020  _corr", corr).  
-0000bf30: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000bf40: 6473 203d 2070 6d2e 4465 7465 726d 696e  ds = pm.Determin
-0000bf50: 6973 7469 6328 6622 7b6e 616d 657d 5f73  istic(f"{name}_s
-0000bf60: 7464 7322 2c20 7374 6473 290a 2020 2020  tds", stds).    
-0000bf70: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0000bf80: 686f 6c2c 2063 6f72 722c 2073 7464 730a  hol, corr, stds.
-0000bf90: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-0000bfa0: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
-0000bfb0: 6c73 2c20 6574 612c 206e 2c20 7364 5f64  ls, eta, n, sd_d
-0000bfc0: 6973 742c 202a 2c20 636f 6d70 7574 655f  ist, *, compute_
-0000bfd0: 636f 7272 3d54 7275 652c 202a 2a6b 7761  corr=True, **kwa
-0000bfe0: 7267 7329 3a0a 2020 2020 2020 2020 2320  rgs):.        # 
-0000bff0: 636f 6d70 7574 6520 4368 6f6c 6573 6b79  compute Cholesky
-0000c000: 2064 6563 6f6d 706f 7369 7469 6f6e 0a20   decomposition. 
-0000c010: 2020 2020 2020 2070 6163 6b65 645f 6368         packed_ch
-0000c020: 6f6c 203d 205f 4c4b 4a43 686f 6c65 736b  ol = _LKJCholesk
-0000c030: 7943 6f76 2e64 6973 7428 6574 613d 6574  yCov.dist(eta=et
-0000c040: 612c 206e 3d6e 2c20 7364 5f64 6973 743d  a, n=n, sd_dist=
-0000c050: 7364 5f64 6973 742c 202a 2a6b 7761 7267  sd_dist, **kwarg
-0000c060: 7329 0a20 2020 2020 2020 2069 6620 6e6f  s).        if no
-0000c070: 7420 636f 6d70 7574 655f 636f 7272 3a0a  t compute_corr:.
-0000c080: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c090: 726e 2070 6163 6b65 645f 6368 6f6c 0a20  rn packed_chol. 
-0000c0a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000c0b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c0c0: 636c 732e 6865 6c70 6572 5f64 6574 6572  cls.helper_deter
-0000c0d0: 6d69 6e69 7374 6963 7328 6e2c 2070 6163  ministics(n, pac
-0000c0e0: 6b65 645f 6368 6f6c 290a 0a20 2020 2040  ked_chol)..    @
-0000c0f0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-0000c100: 6465 6620 6865 6c70 6572 5f64 6574 6572  def helper_deter
-0000c110: 6d69 6e69 7374 6963 7328 636c 732c 206e  ministics(cls, n
-0000c120: 2c20 7061 636b 6564 5f63 686f 6c29 3a0a  , packed_chol):.
-0000c130: 2020 2020 2020 2020 6368 6f6c 203d 2070          chol = p
-0000c140: 6d2e 6578 7061 6e64 5f70 6163 6b65 645f  m.expand_packed_
-0000c150: 7472 6961 6e67 756c 6172 286e 2c20 7061  triangular(n, pa
-0000c160: 636b 6564 5f63 686f 6c2c 206c 6f77 6572  cked_chol, lower
-0000c170: 3d54 7275 6529 0a20 2020 2020 2020 2023  =True).        #
-0000c180: 2063 6f6d 7075 7465 2063 6f76 6172 6961   compute covaria
-0000c190: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
-0000c1a0: 2020 2063 6f76 203d 2070 742e 646f 7428     cov = pt.dot(
-0000c1b0: 6368 6f6c 2c20 6368 6f6c 2e54 290a 2020  chol, chol.T).  
-0000c1c0: 2020 2020 2020 2320 6578 7472 6163 7420        # extract 
-0000c1d0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0000c1e0: 6f6e 7320 616e 6420 7268 6f0a 2020 2020  ons and rho.    
-0000c1f0: 2020 2020 7374 6473 203d 2070 742e 7371      stds = pt.sq
-0000c200: 7274 2870 742e 6469 6167 2863 6f76 2929  rt(pt.diag(cov))
-0000c210: 0a20 2020 2020 2020 2069 6e76 5f73 7464  .        inv_std
-0000c220: 7320 3d20 3120 2f20 7374 6473 0a20 2020  s = 1 / stds.   
-0000c230: 2020 2020 2063 6f72 7220 3d20 696e 765f       corr = inv_
-0000c240: 7374 6473 5b4e 6f6e 652c 203a 5d20 2a20  stds[None, :] * 
-0000c250: 636f 7620 2a20 696e 765f 7374 6473 5b3a  cov * inv_stds[:
-0000c260: 2c20 4e6f 6e65 5d0a 2020 2020 2020 2020  , None].        
-0000c270: 7265 7475 726e 2063 686f 6c2c 2063 6f72  return chol, cor
-0000c280: 722c 2073 7464 730a 0a0a 636c 6173 7320  r, stds...class 
-0000c290: 4c4b 4a43 6f72 7252 5628 5261 6e64 6f6d  LKJCorrRV(Random
-0000c2a0: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
-0000c2b0: 616d 6520 3d20 226c 6b6a 636f 7272 220a  ame = "lkjcorr".
-0000c2c0: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
-0000c2d0: 310a 2020 2020 6e64 696d 735f 7061 7261  1.    ndims_para
-0000c2e0: 6d73 203d 205b 302c 2030 5d0a 2020 2020  ms = [0, 0].    
-0000c2f0: 6474 7970 6520 3d20 2266 6c6f 6174 5822  dtype = "floatX"
-0000c300: 0a20 2020 205f 7072 696e 745f 6e61 6d65  .    _print_name
-0000c310: 203d 2028 224c 4b4a 436f 7272 5256 222c   = ("LKJCorrRV",
-0000c320: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-0000c330: 7b4c 4b4a 436f 7272 5256 7d22 290a 0a20  {LKJCorrRV}").. 
-0000c340: 2020 2064 6566 206d 616b 655f 6e6f 6465     def make_node
-0000c350: 2873 656c 662c 2072 6e67 2c20 7369 7a65  (self, rng, size
-0000c360: 2c20 6474 7970 652c 206e 2c20 6574 6129  , dtype, n, eta)
-0000c370: 3a0a 2020 2020 2020 2020 6e20 3d20 7074  :.        n = pt
-0000c380: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
-0000c390: 626c 6528 6e29 0a20 2020 2020 2020 2069  ble(n).        i
-0000c3a0: 6620 6e6f 7420 6e2e 6e64 696d 203d 3d20  f not n.ndim == 
-0000c3b0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0000c3c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000c3d0: 226e 206d 7573 7420 6265 2061 2073 6361  "n must be a sca
-0000c3e0: 6c61 7220 286e 6469 6d3d 3029 2e22 290a  lar (ndim=0).").
-0000c3f0: 0a20 2020 2020 2020 2065 7461 203d 2070  .        eta = p
-0000c400: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-0000c410: 6162 6c65 2865 7461 290a 2020 2020 2020  able(eta).      
-0000c420: 2020 6966 206e 6f74 2065 7461 2e6e 6469    if not eta.ndi
-0000c430: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
-0000c440: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000c450: 7272 6f72 2822 6574 6120 6d75 7374 2062  rror("eta must b
-0000c460: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
-0000c470: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
-0000c480: 7265 7475 726e 2073 7570 6572 2829 2e6d  return super().m
-0000c490: 616b 655f 6e6f 6465 2872 6e67 2c20 7369  ake_node(rng, si
-0000c4a0: 7a65 2c20 6474 7970 652c 206e 2c20 6574  ze, dtype, n, et
-0000c4b0: 6129 0a0a 2020 2020 6465 6620 5f73 7570  a)..    def _sup
-0000c4c0: 705f 7368 6170 655f 6672 6f6d 5f70 6172  p_shape_from_par
-0000c4d0: 616d 7328 7365 6c66 2c20 6469 7374 5f70  ams(self, dist_p
-0000c4e0: 6172 616d 732c 202a 2a6b 7761 7267 7329  arams, **kwargs)
-0000c4f0: 3a0a 2020 2020 2020 2020 6e20 3d20 6469  :.        n = di
-0000c500: 7374 5f70 6172 616d 735b 305d 0a20 2020  st_params[0].   
-0000c510: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
-0000c520: 3d20 2828 6e20 2a20 286e 202d 2031 2929  = ((n * (n - 1))
-0000c530: 202f 2f20 322c 290a 2020 2020 2020 2020   // 2,).        
-0000c540: 7265 7475 726e 2064 6973 745f 7368 6170  return dist_shap
-0000c550: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
-0000c560: 686f 640a 2020 2020 6465 6620 726e 675f  hod.    def rng_
-0000c570: 666e 2863 6c73 2c20 726e 672c 206e 2c20  fn(cls, rng, n, 
-0000c580: 6574 612c 2073 697a 6529 3a0a 2020 2020  eta, size):.    
-0000c590: 2020 2020 2320 5765 2066 6c61 7474 656e      # We flatten
-0000c5a0: 2074 6865 2073 697a 6520 746f 206d 616b   the size to mak
-0000c5b0: 6520 6f70 6572 6174 696f 6e73 2065 6173  e operations eas
-0000c5c0: 6965 722c 2061 6e64 2074 6865 6e20 7265  ier, and then re
-0000c5d0: 6275 696c 6420 6974 0a20 2020 2020 2020  build it.       
-0000c5e0: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
-0000c5f0: 3a0a 2020 2020 2020 2020 2020 2020 666c  :.            fl
-0000c600: 6174 5f73 697a 6520 3d20 310a 2020 2020  at_size = 1.    
-0000c610: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c620: 2020 2020 2020 666c 6174 5f73 697a 6520        flat_size 
-0000c630: 3d20 6e70 2e70 726f 6428 7369 7a65 290a  = np.prod(size).
-0000c640: 0a20 2020 2020 2020 2043 203d 2063 6c73  .        C = cls
-0000c650: 2e5f 7261 6e64 6f6d 5f63 6f72 725f 6d61  ._random_corr_ma
-0000c660: 7472 6978 2872 6e67 3d72 6e67 2c20 6e3d  trix(rng=rng, n=
-0000c670: 6e2c 2065 7461 3d65 7461 2c20 666c 6174  n, eta=eta, flat
-0000c680: 5f73 697a 653d 666c 6174 5f73 697a 6529  _size=flat_size)
-0000c690: 0a0a 2020 2020 2020 2020 7472 6975 5f69  ..        triu_i
-0000c6a0: 6478 203d 206e 702e 7472 6975 5f69 6e64  dx = np.triu_ind
-0000c6b0: 6963 6573 286e 2c20 6b3d 3129 0a20 2020  ices(n, k=1).   
-0000c6c0: 2020 2020 2073 616d 706c 6573 203d 2043       samples = C
-0000c6d0: 5b2e 2e2e 2c20 7472 6975 5f69 6478 5b30  [..., triu_idx[0
-0000c6e0: 5d2c 2074 7269 755f 6964 785b 315d 5d0a  ], triu_idx[1]].
-0000c6f0: 0a20 2020 2020 2020 2069 6620 7369 7a65  .        if size
-0000c700: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000c710: 2020 2020 2020 7361 6d70 6c65 7320 3d20        samples = 
-0000c720: 7361 6d70 6c65 735b 305d 0a20 2020 2020  samples[0].     
-0000c730: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c740: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
-0000c750: 3d20 286e 202a 2028 6e20 2d20 3129 2920  = (n * (n - 1)) 
-0000c760: 2f2f 2032 0a20 2020 2020 2020 2020 2020  // 2.           
-0000c770: 2073 616d 706c 6573 203d 206e 702e 7265   samples = np.re
-0000c780: 7368 6170 6528 7361 6d70 6c65 732c 2028  shape(samples, (
-0000c790: 2a73 697a 652c 2064 6973 745f 7368 6170  *size, dist_shap
-0000c7a0: 6529 290a 2020 2020 2020 2020 7265 7475  e)).        retu
-0000c7b0: 726e 2073 616d 706c 6573 0a0a 2020 2020  rn samples..    
-0000c7c0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-0000c7d0: 2064 6566 205f 7261 6e64 6f6d 5f63 6f72   def _random_cor
-0000c7e0: 725f 6d61 7472 6978 2863 6c73 2c20 726e  r_matrix(cls, rn
-0000c7f0: 672c 206e 2c20 6574 612c 2066 6c61 745f  g, n, eta, flat_
-0000c800: 7369 7a65 293a 0a20 2020 2020 2020 2023  size):.        #
-0000c810: 206f 7269 6769 6e61 6c20 696d 706c 656d   original implem
-0000c820: 656e 7461 7469 6f6e 2069 6e20 5220 7365  entation in R se
-0000c830: 653a 0a20 2020 2020 2020 2023 2068 7474  e:.        # htt
-0000c840: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000c850: 726d 6365 6c72 6561 7468 2f72 6574 6869  rmcelreath/rethi
-0000c860: 6e6b 696e 672f 626c 6f62 2f6d 6173 7465  nking/blob/maste
-0000c870: 722f 522f 6469 7374 7269 6275 7469 6f6e  r/R/distribution
-0000c880: 732e 720a 2020 2020 2020 2020 6265 7461  s.r.        beta
-0000c890: 203d 2065 7461 202d 2031 2e30 202b 206e   = eta - 1.0 + n
-0000c8a0: 202f 2032 2e30 0a20 2020 2020 2020 2072   / 2.0.        r
-0000c8b0: 3132 203d 2032 2e30 202a 2073 7461 7473  12 = 2.0 * stats
-0000c8c0: 2e62 6574 612e 7276 7328 613d 6265 7461  .beta.rvs(a=beta
-0000c8d0: 2c20 623d 6265 7461 2c20 7369 7a65 3d66  , b=beta, size=f
-0000c8e0: 6c61 745f 7369 7a65 2c20 7261 6e64 6f6d  lat_size, random
-0000c8f0: 5f73 7461 7465 3d72 6e67 2920 2d20 312e  _state=rng) - 1.
-0000c900: 300a 2020 2020 2020 2020 5020 3d20 6e70  0.        P = np
-0000c910: 2e66 756c 6c28 2866 6c61 745f 7369 7a65  .full((flat_size
-0000c920: 2c20 6e2c 206e 292c 206e 702e 6579 6528  , n, n), np.eye(
-0000c930: 6e29 290a 2020 2020 2020 2020 505b 2e2e  n)).        P[..
-0000c940: 2e2c 2030 2c20 315d 203d 2072 3132 0a20  ., 0, 1] = r12. 
-0000c950: 2020 2020 2020 2050 5b2e 2e2e 2c20 312c         P[..., 1,
-0000c960: 2031 5d20 3d20 6e70 2e73 7172 7428 312e   1] = np.sqrt(1.
-0000c970: 3020 2d20 7231 322a 2a32 290a 2020 2020  0 - r12**2).    
-0000c980: 2020 2020 666f 7220 6d70 3120 696e 2072      for mp1 in r
-0000c990: 616e 6765 2832 2c20 6e29 3a0a 2020 2020  ange(2, n):.    
-0000c9a0: 2020 2020 2020 2020 6265 7461 202d 3d20          beta -= 
-0000c9b0: 302e 350a 2020 2020 2020 2020 2020 2020  0.5.            
-0000c9c0: 7920 3d20 7374 6174 732e 6265 7461 2e72  y = stats.beta.r
-0000c9d0: 7673 2861 3d6d 7031 202f 2032 2e30 2c20  vs(a=mp1 / 2.0, 
-0000c9e0: 623d 6265 7461 2c20 7369 7a65 3d66 6c61  b=beta, size=fla
-0000c9f0: 745f 7369 7a65 2c20 7261 6e64 6f6d 5f73  t_size, random_s
-0000ca00: 7461 7465 3d72 6e67 290a 2020 2020 2020  tate=rng).      
-0000ca10: 2020 2020 2020 7a20 3d20 7374 6174 732e        z = stats.
-0000ca20: 6e6f 726d 2e72 7673 286c 6f63 3d30 2c20  norm.rvs(loc=0, 
-0000ca30: 7363 616c 653d 312c 2073 697a 653d 2866  scale=1, size=(f
-0000ca40: 6c61 745f 7369 7a65 2c20 6d70 3129 2c20  lat_size, mp1), 
-0000ca50: 7261 6e64 6f6d 5f73 7461 7465 3d72 6e67  random_state=rng
-0000ca60: 290a 2020 2020 2020 2020 2020 2020 7a20  ).            z 
-0000ca70: 3d20 7a20 2f20 6e70 2e73 7172 7428 6e70  = z / np.sqrt(np
-0000ca80: 2e65 696e 7375 6d28 2269 6a2c 696a 2d3e  .einsum("ij,ij->
-0000ca90: 6922 2c20 7a2c 207a 2929 5b2e 2e2e 2c20  i", z, z))[..., 
-0000caa0: 6e70 2e6e 6577 6178 6973 5d0a 2020 2020  np.newaxis].    
-0000cab0: 2020 2020 2020 2020 505b 2e2e 2e2c 2030          P[..., 0
-0000cac0: 3a6d 7031 2c20 6d70 315d 203d 206e 702e  :mp1, mp1] = np.
-0000cad0: 7371 7274 2879 5b2e 2e2e 2c20 6e70 2e6e  sqrt(y[..., np.n
-0000cae0: 6577 6178 6973 5d29 202a 207a 0a20 2020  ewaxis]) * z.   
-0000caf0: 2020 2020 2020 2020 2050 5b2e 2e2e 2c20           P[..., 
-0000cb00: 6d70 312c 206d 7031 5d20 3d20 6e70 2e73  mp1, mp1] = np.s
-0000cb10: 7172 7428 312e 3020 2d20 7929 0a20 2020  qrt(1.0 - y).   
-0000cb20: 2020 2020 2043 203d 206e 702e 6569 6e73       C = np.eins
-0000cb30: 756d 2822 2e2e 2e6a 692c 2e2e 2e6a 6b2d  um("...ji,...jk-
-0000cb40: 3e2e 2e2e 696b 222c 2050 2c20 5029 0a20  >...ik", P, P). 
-0000cb50: 2020 2020 2020 2072 6574 7572 6e20 430a         return C.
-0000cb60: 0a0a 6c6b 6a63 6f72 7220 3d20 4c4b 4a43  ..lkjcorr = LKJC
-0000cb70: 6f72 7252 5628 290a 0a0a 636c 6173 7320  orrRV()...class 
-0000cb80: 4c4b 4a43 6f72 7228 426f 756e 6465 6443  LKJCorr(BoundedC
-0000cb90: 6f6e 7469 6e75 6f75 7329 3a0a 2020 2020  ontinuous):.    
-0000cba0: 7222 2222 0a20 2020 2054 6865 204c 4b4a  r""".    The LKJ
-0000cbb0: 2028 4c65 7761 6e64 6f77 736b 692c 204b   (Lewandowski, K
-0000cbc0: 7572 6f77 6963 6b61 2061 6e64 204a 6f65  urowicka and Joe
-0000cbd0: 2920 6c6f 672d 6c69 6b65 6c69 686f 6f64  ) log-likelihood
-0000cbe0: 2e0a 0a20 2020 2054 6865 204c 4b4a 2064  ...    The LKJ d
-0000cbf0: 6973 7472 6962 7574 696f 6e20 6973 2061  istribution is a
-0000cc00: 2070 7269 6f72 2064 6973 7472 6962 7574   prior distribut
-0000cc10: 696f 6e20 666f 7220 636f 7272 656c 6174  ion for correlat
-0000cc20: 696f 6e20 6d61 7472 6963 6573 2e0a 2020  ion matrices..  
-0000cc30: 2020 4966 2065 7461 203d 2031 2074 6869    If eta = 1 thi
-0000cc40: 7320 636f 7272 6573 706f 6e64 7320 746f  s corresponds to
-0000cc50: 2074 6865 2075 6e69 666f 726d 2064 6973   the uniform dis
-0000cc60: 7472 6962 7574 696f 6e20 6f76 6572 2063  tribution over c
-0000cc70: 6f72 7265 6c61 7469 6f6e 0a20 2020 206d  orrelation.    m
-0000cc80: 6174 7269 6365 732e 2046 6f72 2065 7461  atrices. For eta
-0000cc90: 202d 3e20 6f6f 2074 6865 204c 4b4a 2070   -> oo the LKJ p
-0000cca0: 7269 6f72 2061 7070 726f 6163 6865 7320  rior approaches 
-0000ccb0: 7468 6520 6964 656e 7469 7479 206d 6174  the identity mat
-0000ccc0: 7269 782e 0a0a 2020 2020 3d3d 3d3d 3d3d  rix...    ======
-0000ccd0: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
-0000cce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ccf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cd00: 3d3d 0a20 2020 2053 7570 706f 7274 2020  ==.    Support  
-0000cd10: 2055 7070 6572 2074 7269 616e 6775 6c61   Upper triangula
-0000cd20: 7220 6d61 7472 6978 2077 6974 6820 7661  r matrix with va
-0000cd30: 6c75 6573 2069 6e20 5b2d 312c 2031 5d0a  lues in [-1, 1].
-0000cd40: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+00005b10: 284d 756c 7469 6e6f 6d69 616c 293a 0a20  (Multinomial):. 
+00005b20: 2020 2072 2222 220a 2020 2020 556e 6465     r""".    Unde
+00005b30: 726c 7969 6e67 2063 6c61 7373 2066 6f72  rlying class for
+00005b40: 206f 7264 6572 6564 206d 756c 7469 6e6f   ordered multino
+00005b50: 6d69 616c 2064 6973 7472 6962 7574 696f  mial distributio
+00005b60: 6e73 2e0a 2020 2020 5365 6520 646f 6373  ns..    See docs
+00005b70: 2066 6f72 2074 6865 204f 7264 6572 6564   for the Ordered
+00005b80: 4d75 6c74 696e 6f6d 6961 6c20 7772 6170  Multinomial wrap
+00005b90: 7065 7220 636c 6173 7320 666f 7220 6d6f  per class for mo
+00005ba0: 7265 2064 6574 6169 6c73 206f 6e20 686f  re details on ho
+00005bb0: 7720 746f 2075 7365 2069 7420 696e 206d  w to use it in m
+00005bc0: 6f64 656c 732e 0a20 2020 2022 2222 0a20  odels..    """. 
+00005bd0: 2020 2072 765f 6f70 203d 206d 756c 7469     rv_op = multi
+00005be0: 6e6f 6d69 616c 0a0a 2020 2020 4063 6c61  nomial..    @cla
+00005bf0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00005c00: 2064 6973 7428 636c 732c 2065 7461 2c20   dist(cls, eta, 
+00005c10: 6375 7470 6f69 6e74 732c 206e 2c20 2a61  cutpoints, n, *a
+00005c20: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00005c30: 2020 2020 2020 2020 6574 6120 3d20 7074          eta = pt
+00005c40: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+00005c50: 626c 6528 666c 6f61 7458 2865 7461 2929  ble(floatX(eta))
+00005c60: 0a20 2020 2020 2020 2063 7574 706f 696e  .        cutpoin
+00005c70: 7473 203d 2070 742e 6173 5f74 656e 736f  ts = pt.as_tenso
+00005c80: 725f 7661 7269 6162 6c65 2863 7574 706f  r_variable(cutpo
+00005c90: 696e 7473 290a 2020 2020 2020 2020 6e20  ints).        n 
+00005ca0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00005cb0: 6172 6961 626c 6528 696e 7458 286e 2929  ariable(intX(n))
+00005cc0: 0a0a 2020 2020 2020 2020 7061 203d 2073  ..        pa = s
+00005cd0: 6967 6d6f 6964 2863 7574 706f 696e 7473  igmoid(cutpoints
+00005ce0: 202d 2070 742e 7368 6170 655f 7061 6472   - pt.shape_padr
+00005cf0: 6967 6874 2865 7461 2929 0a20 2020 2020  ight(eta)).     
+00005d00: 2020 2070 5f63 756d 203d 2070 742e 636f     p_cum = pt.co
+00005d10: 6e63 6174 656e 6174 6528 0a20 2020 2020  ncatenate(.     
+00005d20: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00005d30: 2020 2020 2020 2020 2070 742e 7a65 726f           pt.zero
+00005d40: 735f 6c69 6b65 2870 742e 7368 6170 655f  s_like(pt.shape_
+00005d50: 7061 6472 6967 6874 2870 615b 2e2e 2e2c  padright(pa[...,
+00005d60: 2030 5d29 292c 0a20 2020 2020 2020 2020   0])),.         
+00005d70: 2020 2020 2020 2070 612c 0a20 2020 2020         pa,.     
+00005d80: 2020 2020 2020 2020 2020 2070 742e 6f6e             pt.on
+00005d90: 6573 5f6c 696b 6528 7074 2e73 6861 7065  es_like(pt.shape
+00005da0: 5f70 6164 7269 6768 7428 7061 5b2e 2e2e  _padright(pa[...
+00005db0: 2c20 305d 2929 2c0a 2020 2020 2020 2020  , 0])),.        
+00005dc0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00005dd0: 2020 2061 7869 733d 2d31 2c0a 2020 2020     axis=-1,.    
+00005de0: 2020 2020 290a 2020 2020 2020 2020 7020      ).        p 
+00005df0: 3d20 705f 6375 6d5b 2e2e 2e2c 2031 3a5d  = p_cum[..., 1:]
+00005e00: 202d 2070 5f63 756d 5b2e 2e2e 2c20 3a2d   - p_cum[..., :-
+00005e10: 315d 0a0a 2020 2020 2020 2020 7265 7475  1]..        retu
+00005e20: 726e 2073 7570 6572 2829 2e64 6973 7428  rn super().dist(
+00005e30: 6e2c 2070 2c20 2a61 7267 732c 202a 2a6b  n, p, *args, **k
+00005e40: 7761 7267 7329 0a0a 0a63 6c61 7373 204f  wargs)...class O
+00005e50: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
+00005e60: 6c3a 0a20 2020 2072 2222 220a 2020 2020  l:.    r""".    
+00005e70: 5772 6170 7065 7220 636c 6173 7320 666f  Wrapper class fo
+00005e80: 7220 4f72 6465 7265 6420 4d75 6c74 696e  r Ordered Multin
+00005e90: 6f6d 6961 6c20 6469 7374 7269 6275 7469  omial distributi
+00005ea0: 6f6e 732e 0a0a 2020 2020 5573 6566 756c  ons...    Useful
+00005eb0: 2066 6f72 2072 6567 7265 7373 696f 6e20   for regression 
+00005ec0: 6f6e 206f 7264 696e 616c 2064 6174 6120  on ordinal data 
+00005ed0: 7768 6f73 6520 7661 6c75 6573 2072 616e  whose values ran
+00005ee0: 6765 0a20 2020 2066 726f 6d20 3120 746f  ge.    from 1 to
+00005ef0: 204b 2061 7320 6120 6675 6e63 7469 6f6e   K as a function
+00005f00: 206f 6620 736f 6d65 2070 7265 6469 6374   of some predict
+00005f10: 6f72 2c20 3a6d 6174 683a 605c 6574 6160  or, :math:`\eta`
+00005f20: 2c20 6275 740a 2020 2020 7768 6963 6820  , but.    which 
+00005f30: 6172 6520 5f61 6767 7265 6761 7465 645f  are _aggregated_
+00005f40: 2062 7920 7472 6961 6c2c 206c 696b 6520   by trial, like 
+00005f50: 6d75 6c74 696e 6f6d 6961 6c20 6f62 7365  multinomial obse
+00005f60: 7276 6174 696f 6e73 2028 696e 0a20 2020  rvations (in.   
+00005f70: 2063 6f6e 7472 6173 7420 746f 2060 706d   contrast to `pm
+00005f80: 2e4f 7264 6572 6564 4c6f 6769 7374 6963  .OrderedLogistic
+00005f90: 602c 2077 6869 6368 206f 6e6c 7920 6163  `, which only ac
+00005fa0: 6365 7074 7320 6f72 6469 6e61 6c20 6461  cepts ordinal da
+00005fb0: 7461 0a20 2020 2069 6e20 6120 5f64 6973  ta.    in a _dis
+00005fc0: 6167 6772 6567 6174 6564 5f20 666f 726d  aggregated_ form
+00005fd0: 6174 2c20 6c69 6b65 2063 6174 6567 6f72  at, like categor
+00005fe0: 6963 616c 206f 6273 6572 7661 7469 6f6e  ical observation
+00005ff0: 7329 2e0a 2020 2020 5468 6520 6375 7470  s)..    The cutp
+00006000: 6f69 6e74 732c 203a 6d61 7468 3a60 6360  oints, :math:`c`
+00006010: 2c20 7365 7061 7261 7465 2077 6869 6368  , separate which
+00006020: 2072 616e 6765 7320 6f66 203a 6d61 7468   ranges of :math
+00006030: 3a60 5c65 7461 6020 6172 650a 2020 2020  :`\eta` are.    
+00006040: 6d61 7070 6564 2074 6f20 7768 6963 6820  mapped to which 
+00006050: 6f66 2074 6865 204b 206f 6273 6572 7665  of the K observe
+00006060: 6420 6465 7065 6e64 656e 7420 7661 7269  d dependent vari
+00006070: 6162 6c65 732e 2054 6865 206e 756d 6265  ables. The numbe
+00006080: 720a 2020 2020 6f66 2063 7574 706f 696e  r.    of cutpoin
+00006090: 7473 2069 7320 4b20 2d20 312e 2049 7420  ts is K - 1. It 
+000060a0: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+000060b0: 6861 7420 7468 6520 6375 7470 6f69 6e74  hat the cutpoint
+000060c0: 7320 6172 650a 2020 2020 636f 6e73 7472  s are.    constr
+000060d0: 6169 6e65 6420 746f 2062 6520 6f72 6465  ained to be orde
+000060e0: 7265 642e 0a0a 2020 2020 2e2e 206d 6174  red...    .. mat
+000060f0: 683a 3a0a 0a20 2020 2020 2020 6628 6b20  h::..       f(k 
+00006100: 5c6d 6964 205c 6574 612c 2063 2920 3d20  \mid \eta, c) = 
+00006110: 5c6c 6566 745c 7b0a 2020 2020 2020 2020  \left\{.        
+00006120: 205c 6265 6769 6e7b 6172 7261 797d 7b6c   \begin{array}{l
+00006130: 7d0a 2020 2020 2020 2020 2020 2031 202d  }.           1 -
+00006140: 205c 7465 7874 7b6c 6f67 6974 7d5e 7b2d   \text{logit}^{-
+00006150: 317d 285c 6574 6120 2d20 635f 3129 0a20  1}(\eta - c_1). 
+00006160: 2020 2020 2020 2020 2020 2020 5c2c 2c20              \,, 
+00006170: 5c74 6578 747b 6966 207d 206b 203d 2030  \text{if } k = 0
+00006180: 205c 5c0a 2020 2020 2020 2020 2020 205c   \\.           \
+00006190: 7465 7874 7b6c 6f67 6974 7d5e 7b2d 317d  text{logit}^{-1}
+000061a0: 285c 6574 6120 2d20 635f 7b6b 202d 2031  (\eta - c_{k - 1
+000061b0: 7d29 202d 0a20 2020 2020 2020 2020 2020  }) -.           
+000061c0: 5c74 6578 747b 6c6f 6769 747d 5e7b 2d31  \text{logit}^{-1
+000061d0: 7d28 5c65 7461 202d 2063 5f7b 6b7d 290a  }(\eta - c_{k}).
+000061e0: 2020 2020 2020 2020 2020 2020 205c 2c2c               \,,
+000061f0: 205c 7465 7874 7b69 6620 7d20 3020 3c20   \text{if } 0 < 
+00006200: 6b20 3c20 4b20 5c5c 0a20 2020 2020 2020  k < K \\.       
+00006210: 2020 2020 5c74 6578 747b 6c6f 6769 747d      \text{logit}
+00006220: 5e7b 2d31 7d28 5c65 7461 202d 2063 5f7b  ^{-1}(\eta - c_{
+00006230: 4b20 2d20 317d 290a 2020 2020 2020 2020  K - 1}).        
+00006240: 2020 2020 205c 2c2c 205c 7465 7874 7b69       \,, \text{i
+00006250: 6620 7d20 6b20 3d20 4b20 5c5c 0a20 2020  f } k = K \\.   
+00006260: 2020 2020 2020 5c65 6e64 7b61 7272 6179        \end{array
+00006270: 7d0a 2020 2020 2020 205c 7269 6768 742e  }.       \right.
+00006280: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00006290: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000062a0: 2020 2020 6574 6120 3a20 7465 6e73 6f72      eta : tensor
+000062b0: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+000062c0: 2020 2020 2020 2054 6865 2070 7265 6469         The predi
+000062d0: 6374 6f72 2e0a 2020 2020 6375 7470 6f69  ctor..    cutpoi
+000062e0: 6e74 7320 3a20 7465 6e73 6f72 5f6c 696b  nts : tensor_lik
+000062f0: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
+00006300: 2020 2054 6865 206c 656e 6774 6820 4b20     The length K 
+00006310: 2d20 3120 6172 7261 7920 6f66 2063 7574  - 1 array of cut
+00006320: 706f 696e 7473 2077 6869 6368 2062 7265  points which bre
+00006330: 616b 203a 6d61 7468 3a60 5c65 7461 6020  ak :math:`\eta` 
+00006340: 696e 746f 0a20 2020 2020 2020 2072 616e  into.        ran
+00006350: 6765 732e 2044 6f20 6e6f 7420 6578 706c  ges. Do not expl
+00006360: 6963 6974 6c79 2073 6574 2074 6865 2066  icitly set the f
+00006370: 6972 7374 2061 6e64 206c 6173 7420 656c  irst and last el
+00006380: 656d 656e 7473 206f 660a 2020 2020 2020  ements of.      
+00006390: 2020 3a6d 6174 683a 6063 6020 746f 206e    :math:`c` to n
+000063a0: 6567 6174 6976 6520 616e 6420 706f 7369  egative and posi
+000063b0: 7469 7665 2069 6e66 696e 6974 792e 0a20  tive infinity.. 
+000063c0: 2020 206e 203a 2074 656e 736f 725f 6c69     n : tensor_li
+000063d0: 6b65 206f 6620 696e 740a 2020 2020 2020  ke of int.      
+000063e0: 2020 5468 6520 746f 7461 6c20 6e75 6d62    The total numb
+000063f0: 6572 206f 6620 6d75 6c74 696e 6f6d 6961  er of multinomia
+00006400: 6c20 7472 6961 6c73 2e0a 2020 2020 636f  l trials..    co
+00006410: 6d70 7574 655f 7020 3a20 626f 6f6c 6561  mpute_p : boolea
+00006420: 6e2c 2064 6566 6175 6c74 3d54 7275 650a  n, default=True.
+00006430: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00006440: 746f 2063 6f6d 7075 7465 2061 6e64 2073  to compute and s
+00006450: 746f 7265 2069 6e20 7468 6520 7472 6163  tore in the trac
+00006460: 6520 7468 6520 696e 6665 7272 6564 2070  e the inferred p
+00006470: 726f 6261 6269 6c69 7469 6573 206f 6620  robabilities of 
+00006480: 6561 6368 0a20 2020 2020 2020 2063 6174  each.        cat
+00006490: 6567 6f72 6965 732c 0a20 2020 2020 2020  egories,.       
+000064a0: 2062 6173 6564 206f 6e20 7468 6520 6375   based on the cu
+000064b0: 7470 6f69 6e74 7327 2076 616c 7565 732e  tpoints' values.
+000064c0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+000064d0: 652e 0a20 2020 2020 2020 204d 6967 6874  e..        Might
+000064e0: 2062 6520 7573 6566 756c 2074 6f20 6469   be useful to di
+000064f0: 7361 626c 6520 6974 2069 6620 6d65 6d6f  sable it if memo
+00006500: 7279 2075 7361 6765 2069 7320 6f66 2069  ry usage is of i
+00006510: 6e74 6572 6573 742e 0a0a 2020 2020 4578  nterest...    Ex
+00006520: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00006530: 2d2d 2d0a 2020 2020 2e2e 2063 6f64 652d  ---.    .. code-
+00006540: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00006550: 2020 2020 2020 2020 2320 4765 6e65 7261          # Genera
+00006560: 7465 2064 6174 6120 666f 7220 6120 7369  te data for a si
+00006570: 6d70 6c65 2031 2064 696d 656e 7369 6f6e  mple 1 dimension
+00006580: 616c 2065 7861 6d70 6c65 2070 726f 626c  al example probl
+00006590: 656d 0a20 2020 2020 2020 2074 7275 655f  em.        true_
+000065a0: 6375 6d5f 7020 3d20 6e70 2e61 7272 6179  cum_p = np.array
+000065b0: 285b 302e 312c 2030 2e31 352c 2030 2e32  ([0.1, 0.15, 0.2
+000065c0: 352c 2030 2e35 302c 2030 2e36 352c 2030  5, 0.50, 0.65, 0
+000065d0: 2e39 302c 2031 2e30 5d29 0a20 2020 2020  .90, 1.0]).     
+000065e0: 2020 2074 7275 655f 7020 3d20 6e70 2e68     true_p = np.h
+000065f0: 7374 6163 6b28 5b74 7275 655f 6375 6d5f  stack([true_cum_
+00006600: 705b 305d 2c20 7472 7565 5f63 756d 5f70  p[0], true_cum_p
+00006610: 5b31 3a5d 202d 2074 7275 655f 6375 6d5f  [1:] - true_cum_
+00006620: 705b 3a2d 315d 5d29 0a20 2020 2020 2020  p[:-1]]).       
+00006630: 2066 616b 655f 656c 6563 7469 6f6e 7320   fake_elections 
+00006640: 3d20 6e70 2e72 616e 646f 6d2e 6d75 6c74  = np.random.mult
+00006650: 696e 6f6d 6961 6c28 6e3d 315f 3030 302c  inomial(n=1_000,
+00006660: 2070 7661 6c73 3d74 7275 655f 702c 2073   pvals=true_p, s
+00006670: 697a 653d 3630 290a 0a20 2020 2020 2020  ize=60)..       
+00006680: 2023 204f 7264 6572 6564 206d 756c 7469   # Ordered multi
+00006690: 6e6f 6d69 616c 2072 6567 7265 7373 696f  nomial regressio
+000066a0: 6e0a 2020 2020 2020 2020 7769 7468 2070  n.        with p
+000066b0: 6d2e 4d6f 6465 6c28 2920 6173 206d 6f64  m.Model() as mod
+000066c0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+000066d0: 6375 7470 6f69 6e74 7320 3d20 706d 2e4e  cutpoints = pm.N
+000066e0: 6f72 6d61 6c28 0a20 2020 2020 2020 2020  ormal(.         
+000066f0: 2020 2020 2020 2022 6375 7470 6f69 6e74         "cutpoint
+00006700: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00006710: 2020 2020 6d75 3d6e 702e 6172 616e 6765      mu=np.arange
+00006720: 2836 2920 2d20 322e 352c 0a20 2020 2020  (6) - 2.5,.     
+00006730: 2020 2020 2020 2020 2020 2073 6967 6d61             sigma
+00006740: 3d31 2e35 2c0a 2020 2020 2020 2020 2020  =1.5,.          
+00006750: 2020 2020 2020 696e 6974 7661 6c3d 6e70        initval=np
+00006760: 2e61 7261 6e67 6528 3629 202d 2032 2e35  .arange(6) - 2.5
+00006770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006780: 2020 7472 616e 7366 6f72 6d3d 706d 2e64    transform=pm.d
+00006790: 6973 7472 6962 7574 696f 6e73 2e74 7261  istributions.tra
+000067a0: 6e73 666f 726d 732e 6f72 6465 7265 642c  nsforms.ordered,
+000067b0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+000067c0: 2020 2020 2020 2020 2020 2020 706d 2e4f              pm.O
+000067d0: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
+000067e0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+000067f0: 2020 2022 7265 7375 6c74 7322 2c0a 2020     "results",.  
+00006800: 2020 2020 2020 2020 2020 2020 2020 6574                et
+00006810: 613d 302e 302c 0a20 2020 2020 2020 2020  a=0.0,.         
+00006820: 2020 2020 2020 2063 7574 706f 696e 7473         cutpoints
+00006830: 3d63 7574 706f 696e 7473 2c0a 2020 2020  =cutpoints,.    
+00006840: 2020 2020 2020 2020 2020 2020 6e3d 6661              n=fa
+00006850: 6b65 5f65 6c65 6374 696f 6e73 2e73 756d  ke_elections.sum
+00006860: 2831 292c 0a20 2020 2020 2020 2020 2020  (1),.           
+00006870: 2020 2020 206f 6273 6572 7665 643d 6661       observed=fa
+00006880: 6b65 5f65 6c65 6374 696f 6e73 2c0a 2020  ke_elections,.  
+00006890: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000068a0: 2020 2020 2020 2020 2074 7261 6365 203d           trace =
+000068b0: 2070 6d2e 7361 6d70 6c65 2829 0a0a 2020   pm.sample()..  
+000068c0: 2020 2020 2020 2320 506c 6f74 2074 6865        # Plot the
+000068d0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+000068e0: 2061 7276 697a 2e70 6c6f 745f 706f 7374   arviz.plot_post
+000068f0: 6572 696f 7228 7472 6163 655f 3132 5f34  erior(trace_12_4
+00006900: 2c20 7661 725f 6e61 6d65 733d 5b22 636f  , var_names=["co
+00006910: 6d70 6c65 7465 5f70 225d 2c20 7265 665f  mplete_p"], ref_
+00006920: 7661 6c3d 6c69 7374 2874 7275 655f 7029  val=list(true_p)
+00006930: 293b 0a20 2020 2022 2222 0a0a 2020 2020  );.    """..    
+00006940: 6465 6620 5f5f 6e65 775f 5f28 636c 732c  def __new__(cls,
+00006950: 206e 616d 652c 202a 6172 6773 2c20 636f   name, *args, co
+00006960: 6d70 7574 655f 703d 5472 7565 2c20 2a2a  mpute_p=True, **
+00006970: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00006980: 206f 7574 5f72 7620 3d20 5f4f 7264 6572   out_rv = _Order
+00006990: 6564 4d75 6c74 696e 6f6d 6961 6c28 6e61  edMultinomial(na
+000069a0: 6d65 2c20 2a61 7267 732c 202a 2a6b 7761  me, *args, **kwa
+000069b0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
+000069c0: 636f 6d70 7574 655f 703a 0a20 2020 2020  compute_p:.     
+000069d0: 2020 2020 2020 2070 6d2e 4465 7465 726d         pm.Determ
+000069e0: 696e 6973 7469 6328 6622 7b6e 616d 657d  inistic(f"{name}
+000069f0: 5f70 726f 6273 222c 206f 7574 5f72 762e  _probs", out_rv.
+00006a00: 6f77 6e65 722e 696e 7075 7473 5b34 5d2c  owner.inputs[4],
+00006a10: 2064 696d 733d 6b77 6172 6773 2e67 6574   dims=kwargs.get
+00006a20: 2822 6469 6d73 2229 290a 2020 2020 2020  ("dims")).      
+00006a30: 2020 7265 7475 726e 206f 7574 5f72 760a    return out_rv.
+00006a40: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00006a50: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
+00006a60: 6c73 2c20 2a61 7267 732c 202a 2a6b 7761  ls, *args, **kwa
+00006a70: 7267 7329 3a0a 2020 2020 2020 2020 7265  rgs):.        re
+00006a80: 7475 726e 205f 4f72 6465 7265 644d 756c  turn _OrderedMul
+00006a90: 7469 6e6f 6d69 616c 2e64 6973 7428 2a61  tinomial.dist(*a
+00006aa0: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
+00006ab0: 0a64 6566 2070 6f73 6465 6628 4141 293a  .def posdef(AA):
+00006ac0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+00006ad0: 2020 6c69 6e61 6c67 2e63 686f 6c65 736b    linalg.cholesk
+00006ae0: 7928 4141 290a 2020 2020 2020 2020 7265  y(AA).        re
+00006af0: 7475 726e 2031 0a20 2020 2065 7863 6570  turn 1.    excep
+00006b00: 7420 6c69 6e61 6c67 2e4c 696e 416c 6745  t linalg.LinAlgE
+00006b10: 7272 6f72 3a0a 2020 2020 2020 2020 7265  rror:.        re
+00006b20: 7475 726e 2030 0a0a 0a63 6c61 7373 2050  turn 0...class P
+00006b30: 6f73 4465 664d 6174 7269 7828 4f70 293a  osDefMatrix(Op):
+00006b40: 0a20 2020 2022 2222 0a20 2020 2043 6865  .    """.    Che
+00006b50: 636b 2069 6620 696e 7075 7420 6973 2070  ck if input is p
+00006b60: 6f73 6974 6976 6520 6465 6669 6e69 7465  ositive definite
+00006b70: 2e20 496e 7075 7420 7368 6f75 6c64 2062  . Input should b
+00006b80: 6520 6120 7371 7561 7265 206d 6174 7269  e a square matri
+00006b90: 782e 0a0a 2020 2020 2222 220a 0a20 2020  x...    """..   
+00006ba0: 2023 2050 726f 7065 7274 6965 7320 6174   # Properties at
+00006bb0: 7472 6962 7574 650a 2020 2020 5f5f 7072  tribute.    __pr
+00006bc0: 6f70 735f 5f20 3d20 2829 0a0a 2020 2020  ops__ = ()..    
+00006bd0: 2320 436f 6d70 756c 736f 7279 2069 6620  # Compulsory if 
+00006be0: 6974 7970 6573 2061 6e64 206f 7479 7065  itypes and otype
+00006bf0: 7320 6172 6520 6e6f 7420 6465 6669 6e65  s are not define
+00006c00: 640a 0a20 2020 2064 6566 206d 616b 655f  d..    def make_
+00006c10: 6e6f 6465 2873 656c 662c 2078 293a 0a20  node(self, x):. 
+00006c20: 2020 2020 2020 2078 203d 2070 742e 6173         x = pt.as
+00006c30: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00006c40: 2878 290a 2020 2020 2020 2020 6173 7365  (x).        asse
+00006c50: 7274 2078 2e6e 6469 6d20 3d3d 2032 0a20  rt x.ndim == 2. 
+00006c60: 2020 2020 2020 206f 203d 2054 656e 736f         o = Tenso
+00006c70: 7254 7970 6528 6474 7970 653d 2269 6e74  rType(dtype="int
+00006c80: 3822 2c20 7368 6170 653d 5b5d 2928 290a  8", shape=[])().
+00006c90: 2020 2020 2020 2020 7265 7475 726e 2041          return A
+00006ca0: 7070 6c79 2873 656c 662c 205b 785d 2c20  pply(self, [x], 
+00006cb0: 5b6f 5d29 0a0a 2020 2020 2320 5079 7468  [o])..    # Pyth
+00006cc0: 6f6e 2069 6d70 6c65 6d65 6e74 6174 696f  on implementatio
+00006cd0: 6e3a 0a20 2020 2064 6566 2070 6572 666f  n:.    def perfo
+00006ce0: 726d 2873 656c 662c 206e 6f64 652c 2069  rm(self, node, i
+00006cf0: 6e70 7574 732c 206f 7574 7075 7473 293a  nputs, outputs):
+00006d00: 0a20 2020 2020 2020 2028 782c 2920 3d20  .        (x,) = 
+00006d10: 696e 7075 7473 0a20 2020 2020 2020 2028  inputs.        (
+00006d20: 7a2c 2920 3d20 6f75 7470 7574 730a 2020  z,) = outputs.  
+00006d30: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00006d40: 2020 2020 2020 207a 5b30 5d20 3d20 6e70         z[0] = np
+00006d50: 2e61 7272 6179 2870 6f73 6465 6628 7829  .array(posdef(x)
+00006d60: 2c20 6474 7970 653d 2269 6e74 3822 290a  , dtype="int8").
+00006d70: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00006d80: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00006d90: 2020 2020 2020 706d 2e5f 6c6f 672e 6578        pm._log.ex
+00006da0: 6365 7074 696f 6e28 2246 6169 6c65 6420  ception("Failed 
+00006db0: 746f 2063 6865 636b 2069 6620 2573 2070  to check if %s p
+00006dc0: 6f73 6974 6976 6520 6465 6669 6e69 7465  ositive definite
+00006dd0: 222c 2078 290a 2020 2020 2020 2020 2020  ", x).          
+00006de0: 2020 7261 6973 650a 0a20 2020 2064 6566    raise..    def
+00006df0: 2069 6e66 6572 5f73 6861 7065 2873 656c   infer_shape(sel
+00006e00: 662c 2066 6772 6170 682c 206e 6f64 652c  f, fgraph, node,
+00006e10: 2073 6861 7065 7329 3a0a 2020 2020 2020   shapes):.      
+00006e20: 2020 7265 7475 726e 205b 5b5d 5d0a 0a20    return [[]].. 
+00006e30: 2020 2064 6566 2067 7261 6428 7365 6c66     def grad(self
+00006e40: 2c20 696e 702c 2067 7261 6473 293a 0a20  , inp, grads):. 
+00006e50: 2020 2020 2020 2028 782c 2920 3d20 696e         (x,) = in
+00006e60: 700a 2020 2020 2020 2020 7265 7475 726e  p.        return
+00006e70: 205b 782e 7a65 726f 735f 6c69 6b65 2870   [x.zeros_like(p
+00006e80: 7974 656e 736f 722e 636f 6e66 6967 2e66  ytensor.config.f
+00006e90: 6c6f 6174 5829 5d0a 0a20 2020 2064 6566  loatX)]..    def
+00006ea0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
+00006eb0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+00006ec0: 4d61 7472 6978 4973 506f 7369 7469 7665  MatrixIsPositive
+00006ed0: 4465 6669 6e69 7465 220a 0a0a 6d61 7472  Definite"...matr
+00006ee0: 6978 5f70 6f73 5f64 6566 203d 2050 6f73  ix_pos_def = Pos
+00006ef0: 4465 664d 6174 7269 7828 290a 0a0a 636c  DefMatrix()...cl
+00006f00: 6173 7320 5769 7368 6172 7452 5628 5261  ass WishartRV(Ra
+00006f10: 6e64 6f6d 5661 7269 6162 6c65 293a 0a20  ndomVariable):. 
+00006f20: 2020 206e 616d 6520 3d20 2277 6973 6861     name = "wisha
+00006f30: 7274 220a 2020 2020 6e64 696d 5f73 7570  rt".    ndim_sup
+00006f40: 7020 3d20 320a 2020 2020 6e64 696d 735f  p = 2.    ndims_
+00006f50: 7061 7261 6d73 203d 205b 302c 2032 5d0a  params = [0, 2].
+00006f60: 2020 2020 6474 7970 6520 3d20 2266 6c6f      dtype = "flo
+00006f70: 6174 5822 0a20 2020 205f 7072 696e 745f  atX".    _print_
+00006f80: 6e61 6d65 203d 2028 2257 6973 6861 7274  name = ("Wishart
+00006f90: 222c 2022 5c5c 6f70 6572 6174 6f72 6e61  ", "\\operatorna
+00006fa0: 6d65 7b57 6973 6861 7274 7d22 290a 0a20  me{Wishart}").. 
+00006fb0: 2020 2064 6566 205f 7375 7070 5f73 6861     def _supp_sha
+00006fc0: 7065 5f66 726f 6d5f 7061 7261 6d73 2873  pe_from_params(s
+00006fd0: 656c 662c 2064 6973 745f 7061 7261 6d73  elf, dist_params
+00006fe0: 2c20 7265 705f 7061 7261 6d5f 6964 783d  , rep_param_idx=
+00006ff0: 312c 2070 6172 616d 5f73 6861 7065 733d  1, param_shapes=
+00007000: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+00007010: 2054 6865 2073 6861 7065 206f 6620 7365   The shape of se
+00007020: 636f 6e64 2070 6172 616d 6574 6572 2060  cond parameter `
+00007030: 5660 2064 6566 696e 6573 2074 6865 2073  V` defines the s
+00007040: 6861 7065 206f 6620 7468 6520 6f75 7470  hape of the outp
+00007050: 7574 2e0a 2020 2020 2020 2020 7265 7475  ut..        retu
+00007060: 726e 2064 6973 745f 7061 7261 6d73 5b31  rn dist_params[1
+00007070: 5d2e 7368 6170 655b 2d32 3a5d 0a0a 2020  ].shape[-2:]..  
+00007080: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00007090: 2020 2064 6566 2072 6e67 5f66 6e28 636c     def rng_fn(cl
+000070a0: 732c 2072 6e67 2c20 6e75 2c20 562c 2073  s, rng, nu, V, s
+000070b0: 697a 6529 3a0a 2020 2020 2020 2020 7363  ize):.        sc
+000070c0: 6970 795f 7369 7a65 203d 2073 697a 6520  ipy_size = size 
+000070d0: 6966 2073 697a 6520 656c 7365 2031 2020  if size else 1  
+000070e0: 2320 4465 6661 756c 7420 7369 7a65 2066  # Default size f
+000070f0: 6f72 2053 6369 7079 2773 2077 6973 6861  or Scipy's wisha
+00007100: 7274 2e72 7673 2069 7320 310a 2020 2020  rt.rvs is 1.    
+00007110: 2020 2020 7265 7375 6c74 203d 2073 7461      result = sta
+00007120: 7473 2e77 6973 6861 7274 2e72 7673 2869  ts.wishart.rvs(i
+00007130: 6e74 286e 7529 2c20 562c 2073 697a 653d  nt(nu), V, size=
+00007140: 7363 6970 795f 7369 7a65 2c20 7261 6e64  scipy_size, rand
+00007150: 6f6d 5f73 7461 7465 3d72 6e67 290a 2020  om_state=rng).  
+00007160: 2020 2020 2020 6966 2073 697a 6520 3d3d        if size ==
+00007170: 2028 312c 293a 0a20 2020 2020 2020 2020   (1,):.         
+00007180: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00007190: 5b6e 702e 6e65 7761 7869 732c 202e 2e2e  [np.newaxis, ...
+000071a0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+000071b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000071c0: 726e 2072 6573 756c 740a 0a0a 7769 7368  rn result...wish
+000071d0: 6172 7420 3d20 5769 7368 6172 7452 5628  art = WishartRV(
+000071e0: 290a 0a0a 636c 6173 7320 5769 7368 6172  )...class Wishar
+000071f0: 7428 436f 6e74 696e 756f 7573 293a 0a20  t(Continuous):. 
+00007200: 2020 2072 2222 220a 2020 2020 5769 7368     r""".    Wish
+00007210: 6172 7420 6c6f 672d 6c69 6b65 6c69 686f  art log-likeliho
+00007220: 6f64 2e0a 0a20 2020 2054 6865 2057 6973  od...    The Wis
+00007230: 6861 7274 2064 6973 7472 6962 7574 696f  hart distributio
+00007240: 6e20 6973 2074 6865 2070 726f 6261 6269  n is the probabi
+00007250: 6c69 7479 2064 6973 7472 6962 7574 696f  lity distributio
+00007260: 6e20 6f66 2074 6865 0a20 2020 206d 6178  n of the.    max
+00007270: 696d 756d 2d6c 696b 656c 6968 6f6f 6420  imum-likelihood 
+00007280: 6573 7469 6d61 746f 7220 284d 4c45 2920  estimator (MLE) 
+00007290: 6f66 2074 6865 2070 7265 6369 7369 6f6e  of the precision
+000072a0: 206d 6174 7269 7820 6f66 2061 0a20 2020   matrix of a.   
+000072b0: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
+000072c0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
+000072d0: 6e2e 2020 4966 2056 3d31 2c20 7468 6520  n.  If V=1, the 
+000072e0: 6469 7374 7269 6275 7469 6f6e 2069 730a  distribution is.
+000072f0: 2020 2020 6964 656e 7469 6361 6c20 746f      identical to
+00007300: 2074 6865 2063 6869 2d73 7175 6172 6520   the chi-square 
+00007310: 6469 7374 7269 6275 7469 6f6e 2077 6974  distribution wit
+00007320: 6820 6e75 2064 6567 7265 6573 206f 660a  h nu degrees of.
+00007330: 2020 2020 6672 6565 646f 6d2e 0a0a 2020      freedom...  
+00007340: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
+00007350: 2020 2020 6628 5820 5c6d 6964 206e 752c      f(X \mid nu,
+00007360: 2054 2920 3d0a 2020 2020 2020 2020 2020   T) =.          
+00007370: 205c 6672 6163 7b7b 5c6d 6964 2054 205c   \frac{{\mid T \
+00007380: 6d69 647d 5e7b 6e75 2f32 7d7b 5c6d 6964  mid}^{nu/2}{\mid
+00007390: 2058 205c 6d69 647d 5e7b 286e 752d 6b2d   X \mid}^{(nu-k-
+000073a0: 3129 2f32 7d7d 7b32 5e7b 6e75 206b 2f32  1)/2}}{2^{nu k/2
+000073b0: 7d0a 2020 2020 2020 2020 2020 205c 4761  }.           \Ga
+000073c0: 6d6d 615f 7028 6e75 2f32 297d 205c 6578  mma_p(nu/2)} \ex
+000073d0: 705c 6c65 6674 5c7b 202d 5c66 7261 637b  p\left\{ -\frac{
+000073e0: 317d 7b32 7d20 5472 2854 5829 205c 7269  1}{2} Tr(TX) \ri
+000073f0: 6768 745c 7d0a 0a20 2020 2077 6865 7265  ght\}..    where
+00007400: 203a 6d61 7468 3a60 6b60 2069 7320 7468   :math:`k` is th
+00007410: 6520 7261 6e6b 206f 6620 3a6d 6174 683a  e rank of :math:
+00007420: 6058 602e 0a0a 2020 2020 3d3d 3d3d 3d3d  `X`...    ======
+00007430: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00007440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00007460: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
+00007470: 683a 6058 2870 2078 2070 2960 2070 6f73  h:`X(p x p)` pos
+00007480: 6974 6976 6520 6465 6669 6e69 7465 206d  itive definite m
+00007490: 6174 7269 780a 2020 2020 4d65 616e 2020  atrix.    Mean  
+000074a0: 2020 2020 3a6d 6174 683a 606e 7520 5660      :math:`nu V`
+000074b0: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
+000074c0: 6d61 7468 3a60 6e75 2028 765f 7b69 6a7d  math:`nu (v_{ij}
+000074d0: 5e32 202b 2076 5f7b 6969 7d20 765f 7b6a  ^2 + v_{ii} v_{j
+000074e0: 6a7d 2960 0a20 2020 203d 3d3d 3d3d 3d3d  j})`.    =======
+000074f0: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
+00007500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
+00007520: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00007530: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00007540: 6e75 203a 2074 656e 736f 725f 6c69 6b65  nu : tensor_like
+00007550: 206f 6620 696e 740a 2020 2020 2020 2020   of int.        
+00007560: 4465 6772 6565 7320 6f66 2066 7265 6564  Degrees of freed
+00007570: 6f6d 2c20 3e20 302e 0a20 2020 2056 203a  om, > 0..    V :
+00007580: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+00007590: 666c 6f61 740a 2020 2020 2020 2020 7020  float.        p 
+000075a0: 7820 7020 706f 7369 7469 7665 2064 6566  x p positive def
+000075b0: 696e 6974 6520 6d61 7472 6978 2e0a 0a20  inite matrix... 
+000075c0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+000075d0: 2d2d 0a20 2020 2054 6869 7320 6469 7374  --.    This dist
+000075e0: 7269 6275 7469 6f6e 2069 7320 756e 7573  ribution is unus
+000075f0: 6162 6c65 2069 6e20 6120 5079 4d43 206d  able in a PyMC m
+00007600: 6f64 656c 2e20 596f 7520 7368 6f75 6c64  odel. You should
+00007610: 2069 6e73 7465 6164 0a20 2020 2075 7365   instead.    use
+00007620: 204c 4b4a 4368 6f6c 6573 6b79 436f 7620   LKJCholeskyCov 
+00007630: 6f72 204c 4b4a 436f 7272 2e0a 2020 2020  or LKJCorr..    
+00007640: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
+00007650: 7769 7368 6172 740a 0a20 2020 2040 636c  wishart..    @cl
+00007660: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00007670: 6620 6469 7374 2863 6c73 2c20 6e75 2c20  f dist(cls, nu, 
+00007680: 562c 202a 6172 6773 2c20 2a2a 6b77 6172  V, *args, **kwar
+00007690: 6773 293a 0a20 2020 2020 2020 206e 7520  gs):.        nu 
+000076a0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+000076b0: 6172 6961 626c 6528 696e 7458 286e 7529  ariable(intX(nu)
+000076c0: 290a 2020 2020 2020 2020 5620 3d20 7074  ).        V = pt
+000076d0: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+000076e0: 626c 6528 666c 6f61 7458 2856 2929 0a0a  ble(floatX(V))..
+000076f0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00007700: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
+00007710: 2020 2022 5468 6520 5769 7368 6172 7420     "The Wishart 
+00007720: 6469 7374 7269 6275 7469 6f6e 2063 616e  distribution can
+00007730: 2063 7572 7265 6e74 6c79 206e 6f74 2062   currently not b
+00007740: 6520 7573 6564 2022 0a20 2020 2020 2020  e used ".       
+00007750: 2020 2020 2022 666f 7220 4d43 4d43 2073       "for MCMC s
+00007760: 616d 706c 696e 672e 2054 6865 2070 726f  ampling. The pro
+00007770: 6261 6269 6c69 7479 206f 6620 7361 6d70  bability of samp
+00007780: 6c69 6e67 2061 2022 0a20 2020 2020 2020  ling a ".       
+00007790: 2020 2020 2022 7379 6d6d 6574 7269 6320       "symmetric 
+000077a0: 6d61 7472 6978 2069 7320 6261 7369 6361  matrix is basica
+000077b0: 6c6c 7920 7a65 726f 2e20 496e 7374 6561  lly zero. Instea
+000077c0: 642c 2070 6c65 6173 6520 220a 2020 2020  d, please ".    
+000077d0: 2020 2020 2020 2020 2275 7365 204c 4b4a          "use LKJ
+000077e0: 4368 6f6c 6573 6b79 436f 7620 6f72 204c  CholeskyCov or L
+000077f0: 4b4a 436f 7272 2e20 466f 7220 6d6f 7265  KJCorr. For more
+00007800: 2069 6e66 6f72 6d61 7469 6f6e 2022 0a20   information ". 
+00007810: 2020 2020 2020 2020 2020 2022 6f6e 2074             "on t
+00007820: 6865 2069 7373 7565 7320 7375 7272 6f75  he issues surrou
+00007830: 6e64 696e 6720 7468 6520 5769 7368 6172  nding the Wishar
+00007840: 7420 7365 6520 6865 7265 3a20 220a 2020  t see here: ".  
+00007850: 2020 2020 2020 2020 2020 2268 7474 7073            "https
+00007860: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
+00007870: 6d63 2d64 6576 732f 7079 6d63 2f69 7373  mc-devs/pymc/iss
+00007880: 7565 732f 3533 382e 222c 0a20 2020 2020  ues/538.",.     
+00007890: 2020 2020 2020 2055 7365 7257 6172 6e69         UserWarni
+000078a0: 6e67 2c0a 2020 2020 2020 2020 290a 0a20  ng,.        ).. 
+000078b0: 2020 2020 2020 2023 206d 6561 6e20 3d20         # mean = 
+000078c0: 6e75 202a 2056 0a20 2020 2020 2020 2023  nu * V.        #
+000078d0: 2070 203d 2056 2e73 6861 7065 5b30 5d0a   p = V.shape[0].
+000078e0: 2020 2020 2020 2020 2320 6d6f 6465 203d          # mode =
+000078f0: 2070 742e 7377 6974 6368 2870 742e 6765   pt.switch(pt.ge
+00007900: 286e 752c 2070 202b 2031 292c 2028 6e75  (nu, p + 1), (nu
+00007910: 202d 2070 202d 2031 2920 2a20 562c 206e   - p - 1) * V, n
+00007920: 702e 6e61 6e29 0a20 2020 2020 2020 2072  p.nan).        r
+00007930: 6574 7572 6e20 7375 7065 7228 292e 6469  eturn super().di
+00007940: 7374 285b 6e75 2c20 565d 2c20 2a61 7267  st([nu, V], *arg
+00007950: 732c 202a 2a6b 7761 7267 7329 0a0a 2020  s, **kwargs)..  
+00007960: 2020 6465 6620 6c6f 6770 2858 2c20 6e75    def logp(X, nu
+00007970: 2c20 5629 3a0a 2020 2020 2020 2020 2222  , V):.        ""
+00007980: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
+00007990: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
+000079a0: 6974 7920 6f66 2057 6973 6861 7274 2064  ity of Wishart d
+000079b0: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
+000079c0: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
+000079d0: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+000079e0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000079f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00007a00: 2020 2020 2020 2058 3a20 6e75 6d65 7269         X: numeri
+00007a10: 630a 2020 2020 2020 2020 2020 2020 5661  c.            Va
+00007a20: 6c75 6520 666f 7220 7768 6963 6820 6c6f  lue for which lo
+00007a30: 672d 7072 6f62 6162 696c 6974 7920 6973  g-probability is
+00007a40: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
+00007a50: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00007a60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00007a70: 2020 2020 2020 5465 6e73 6f72 5661 7269        TensorVari
+00007a80: 6162 6c65 0a20 2020 2020 2020 2022 2222  able.        """
+00007a90: 0a0a 2020 2020 2020 2020 7020 3d20 562e  ..        p = V.
+00007aa0: 7368 6170 655b 305d 0a0a 2020 2020 2020  shape[0]..      
+00007ab0: 2020 4956 4920 3d20 6465 7428 5629 0a20    IVI = det(V). 
+00007ac0: 2020 2020 2020 2049 5849 203d 2064 6574         IXI = det
+00007ad0: 2858 290a 0a20 2020 2020 2020 2072 6574  (X)..        ret
+00007ae0: 7572 6e20 6368 6563 6b5f 7061 7261 6d65  urn check_parame
+00007af0: 7465 7273 280a 2020 2020 2020 2020 2020  ters(.          
+00007b00: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+00007b10: 2020 2020 286e 7520 2d20 7020 2d20 3129      (nu - p - 1)
+00007b20: 202a 2070 742e 6c6f 6728 4958 4929 0a20   * pt.log(IXI). 
+00007b30: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00007b40: 2074 7261 6365 286d 6174 7269 785f 696e   trace(matrix_in
+00007b50: 7665 7273 6528 5629 2e64 6f74 2858 2929  verse(V).dot(X))
+00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b70: 202d 206e 7520 2a20 7020 2a20 7074 2e6c   - nu * p * pt.l
+00007b80: 6f67 2832 290a 2020 2020 2020 2020 2020  og(2).          
+00007b90: 2020 2020 2020 2d20 6e75 202a 2070 742e        - nu * pt.
+00007ba0: 6c6f 6728 4956 4929 0a20 2020 2020 2020  log(IVI).       
+00007bb0: 2020 2020 2020 2020 202d 2032 202a 206d           - 2 * m
+00007bc0: 756c 7469 6761 6d6d 616c 6e28 6e75 202f  ultigammaln(nu /
+00007bd0: 2032 2e30 2c20 7029 0a20 2020 2020 2020   2.0, p).       
+00007be0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00007bf0: 2020 202f 2032 2c0a 2020 2020 2020 2020     / 2,.        
+00007c00: 2020 2020 6d61 7472 6978 5f70 6f73 5f64      matrix_pos_d
+00007c10: 6566 2858 292c 0a20 2020 2020 2020 2020  ef(X),.         
+00007c20: 2020 2070 742e 6571 2858 2c20 582e 5429     pt.eq(X, X.T)
+00007c30: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+00007c40: 203e 2028 7020 2d20 3129 2c0a 2020 2020   > (p - 1),.    
+00007c50: 2020 2020 290a 0a0a 6465 6620 5769 7368      )...def Wish
+00007c60: 6172 7442 6172 746c 6574 7428 6e61 6d65  artBartlett(name
+00007c70: 2c20 532c 206e 752c 2069 735f 6368 6f6c  , S, nu, is_chol
+00007c80: 6573 6b79 3d46 616c 7365 2c20 7265 7475  esky=False, retu
+00007c90: 726e 5f63 686f 6c65 736b 793d 4661 6c73  rn_cholesky=Fals
+00007ca0: 652c 2069 6e69 7476 616c 3d4e 6f6e 6529  e, initval=None)
+00007cb0: 3a0a 2020 2020 7222 2222 0a20 2020 2042  :.    r""".    B
+00007cc0: 6172 746c 6574 7420 6465 636f 6d70 6f73  artlett decompos
+00007cd0: 6974 696f 6e20 6f66 2074 6865 2057 6973  ition of the Wis
+00007ce0: 6861 7274 2064 6973 7472 6962 7574 696f  hart distributio
+00007cf0: 6e2e 2041 7320 7468 6520 5769 7368 6172  n. As the Wishar
+00007d00: 740a 2020 2020 6469 7374 7269 6275 7469  t.    distributi
+00007d10: 6f6e 2072 6571 7569 7265 7320 7468 6520  on requires the 
+00007d20: 6d61 7472 6978 2074 6f20 6265 2073 796d  matrix to be sym
+00007d30: 6d65 7472 6963 2070 6f73 6974 6976 6520  metric positive 
+00007d40: 7365 6d69 2d64 6566 696e 6974 650a 2020  semi-definite.  
+00007d50: 2020 6974 2069 7320 696d 706f 7373 6962    it is impossib
+00007d60: 6c65 2066 6f72 204d 434d 4320 746f 2065  le for MCMC to e
+00007d70: 7665 7220 7072 6f70 6f73 6520 6163 6365  ver propose acce
+00007d80: 7074 6162 6c65 206d 6174 7269 6365 732e  ptable matrices.
+00007d90: 0a0a 2020 2020 496e 7374 6561 642c 2077  ..    Instead, w
+00007da0: 6520 6361 6e20 7573 6520 7468 6520 4261  e can use the Ba
+00007db0: 726c 6574 7420 6465 636f 6d70 6f73 6974  rlett decomposit
+00007dc0: 696f 6e20 7768 6963 6820 7361 6d70 6c65  ion which sample
+00007dd0: 7320 6120 6c6f 7765 720a 2020 2020 6469  s a lower.    di
+00007de0: 6167 6f6e 616c 206d 6174 7269 782e 2053  agonal matrix. S
+00007df0: 7065 6369 6669 6361 6c6c 793a 0a0a 2020  pecifically:..  
+00007e00: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
+00007e10: 2020 2020 5c74 6578 747b 4966 7d20 4c20      \text{If} L 
+00007e20: 5c73 696d 205c 6265 6769 6e7b 706d 6174  \sim \begin{pmat
+00007e30: 7269 787d 0a20 2020 2020 2020 205c 7371  rix}.        \sq
+00007e40: 7274 7b63 5f31 7d20 2620 3020 2620 3020  rt{c_1} & 0 & 0 
+00007e50: 5c5c 0a20 2020 2020 2020 207a 5f7b 3231  \\.        z_{21
+00007e60: 7d20 2620 5c73 7172 747b 635f 327d 2026  } & \sqrt{c_2} &
+00007e70: 2030 205c 5c0a 2020 2020 2020 2020 7a5f   0 \\.        z_
+00007e80: 7b33 317d 2026 207a 5f7b 3332 7d20 2620  {31} & z_{32} & 
+00007e90: 5c73 7172 747b 635f 337d 0a20 2020 2020  \sqrt{c_3}.     
+00007ea0: 2020 205c 656e 647b 706d 6174 7269 787d     \end{pmatrix}
+00007eb0: 0a0a 2020 2020 2020 2020 5c74 6578 747b  ..        \text{
+00007ec0: 7769 7468 7d20 635f 6920 5c73 696d 205c  with} c_i \sim \
+00007ed0: 6368 695e 3228 6e2d 692b 3129 205c 7465  chi^2(n-i+1) \te
+00007ee0: 7874 7b20 616e 6420 7d20 6e5f 7b69 6a7d  xt{ and } n_{ij}
+00007ef0: 205c 7369 6d20 5c6d 6174 6863 616c 7b4e   \sim \mathcal{N
+00007f00: 7d28 302c 2031 292c 205c 7465 7874 7b74  }(0, 1), \text{t
+00007f10: 6865 6e7d 205c 5c0a 2020 2020 2020 2020  hen} \\.        
+00007f20: 4c20 5c74 696d 6573 2041 205c 7469 6d65  L \times A \time
+00007f30: 7320 412e 5420 5c74 696d 6573 204c 2e54  s A.T \times L.T
+00007f40: 205c 7369 6d20 5c74 6578 747b 5769 7368   \sim \text{Wish
+00007f50: 6172 747d 284c 205c 7469 6d65 7320 4c2e  art}(L \times L.
+00007f60: 542c 205c 6e75 290a 0a20 2020 2053 6565  T, \nu)..    See
+00007f70: 2068 7474 703a 2f2f 656e 2e77 696b 6970   http://en.wikip
+00007f80: 6564 6961 2e6f 7267 2f77 696b 692f 5769  edia.org/wiki/Wi
+00007f90: 7368 6172 745f 6469 7374 7269 6275 7469  shart_distributi
+00007fa0: 6f6e 2342 6172 746c 6574 745f 6465 636f  on#Bartlett_deco
+00007fb0: 6d70 6f73 6974 696f 6e0a 2020 2020 666f  mposition.    fo
+00007fc0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00007fd0: 6f6e 2e0a 0a20 2020 2050 6172 616d 6574  on...    Paramet
+00007fe0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00007ff0: 2d2d 0a20 2020 2053 203a 206e 6461 7272  --.    S : ndarr
+00008000: 6179 0a20 2020 2020 2020 2070 2078 2070  ay.        p x p
+00008010: 2070 6f73 6974 6976 6520 6465 6669 6e69   positive defini
+00008020: 7465 206d 6174 7269 780a 2020 2020 2020  te matrix.      
+00008030: 2020 4f72 3a0a 2020 2020 2020 2020 7020    Or:.        p 
+00008040: 7820 7020 6c6f 7765 722d 7472 6961 6e67  x p lower-triang
+00008050: 756c 6172 206d 6174 7269 7820 7468 6174  ular matrix that
+00008060: 2069 7320 7468 6520 4368 6f6c 6573 6b79   is the Cholesky
+00008070: 2066 6163 746f 720a 2020 2020 2020 2020   factor.        
+00008080: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
+00008090: 6520 6d61 7472 6978 2e0a 2020 2020 6e75  e matrix..    nu
+000080a0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+000080b0: 6620 696e 740a 2020 2020 2020 2020 4465  f int.        De
+000080c0: 6772 6565 7320 6f66 2066 7265 6564 6f6d  grees of freedom
+000080d0: 2c20 3e20 6469 6d28 5329 2e0a 2020 2020  , > dim(S)..    
+000080e0: 6973 5f63 686f 6c65 736b 7920 3a20 626f  is_cholesky : bo
+000080f0: 6f6c 2c20 6465 6661 756c 743d 4661 6c73  ol, default=Fals
+00008100: 650a 2020 2020 2020 2020 496e 7075 7420  e.        Input 
+00008110: 6d61 7472 6978 2053 2069 7320 616c 7265  matrix S is alre
+00008120: 6164 7920 4368 6f6c 6573 6b79 2064 6563  ady Cholesky dec
+00008130: 6f6d 706f 7365 6420 6173 2053 2e54 202a  omposed as S.T *
+00008140: 2053 0a20 2020 2072 6574 7572 6e5f 6368   S.    return_ch
+00008150: 6f6c 6573 6b79 203a 2062 6f6f 6c2c 2064  olesky : bool, d
+00008160: 6566 6175 6c74 3d46 616c 7365 0a20 2020  efault=False.   
+00008170: 2020 2020 204f 6e6c 7920 7265 7475 726e       Only return
+00008180: 2074 6865 2043 686f 6c65 736b 7920 6465   the Cholesky de
+00008190: 636f 6d70 6f73 6564 206d 6174 7269 782e  composed matrix.
+000081a0: 0a20 2020 2069 6e69 7476 616c 203a 206e  .    initval : n
+000081b0: 6461 7272 6179 0a20 2020 2020 2020 2070  darray.        p
+000081c0: 2078 2070 2070 6f73 6974 6976 6520 6465   x p positive de
+000081d0: 6669 6e69 7465 206d 6174 7269 7820 7573  finite matrix us
+000081e0: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
+000081f0: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+00008200: 2d2d 2d2d 2d0a 2020 2020 5468 6973 2069  -----.    This i
+00008210: 7320 6e6f 7420 6120 7374 616e 6461 7264  s not a standard
+00008220: 2044 6973 7472 6962 7574 696f 6e20 636c   Distribution cl
+00008230: 6173 7320 6275 7420 666f 6c6c 6f77 7320  ass but follows 
+00008240: 6120 7369 6d69 6c61 720a 2020 2020 696e  a similar.    in
+00008250: 7465 7266 6163 652e 2042 6573 6964 6573  terface. Besides
+00008260: 2074 6865 2057 6973 6861 7274 2064 6973   the Wishart dis
+00008270: 7472 6962 7574 696f 6e2c 2069 7420 7769  tribution, it wi
+00008280: 6c6c 2061 6464 2052 5673 0a20 2020 206e  ll add RVs.    n
+00008290: 616d 655f 6320 616e 6420 6e61 6d65 5f7a  ame_c and name_z
+000082a0: 2074 6f20 796f 7572 206d 6f64 656c 2077   to your model w
+000082b0: 6869 6368 206d 616b 6520 7570 2074 6865  hich make up the
+000082c0: 206d 6174 7269 782e 0a0a 2020 2020 5468   matrix...    Th
+000082d0: 6973 2064 6973 7472 6962 7574 696f 6e20  is distribution 
+000082e0: 6973 2075 7375 616c 6c79 2061 2062 6164  is usually a bad
+000082f0: 2069 6465 6120 746f 2075 7365 2061 7320   idea to use as 
+00008300: 6120 7072 696f 7220 666f 7220 6d75 6c74  a prior for mult
+00008310: 6976 6172 6961 7465 0a20 2020 206e 6f72  ivariate.    nor
+00008320: 6d61 6c2e 2059 6f75 2073 686f 756c 6420  mal. You should 
+00008330: 696e 7374 6561 6420 7573 6520 4c4b 4a43  instead use LKJC
+00008340: 686f 6c65 736b 7943 6f76 206f 7220 4c4b  holeskyCov or LK
+00008350: 4a43 6f72 722e 0a20 2020 2022 2222 0a0a  JCorr..    """..
+00008360: 2020 2020 4c20 3d20 5320 6966 2069 735f      L = S if is_
+00008370: 6368 6f6c 6573 6b79 2065 6c73 6520 7363  cholesky else sc
+00008380: 6970 792e 6c69 6e61 6c67 2e63 686f 6c65  ipy.linalg.chole
+00008390: 736b 7928 5329 0a20 2020 2064 6961 675f  sky(S).    diag_
+000083a0: 6964 7820 3d20 6e70 2e64 6961 675f 696e  idx = np.diag_in
+000083b0: 6469 6365 735f 6672 6f6d 2853 290a 2020  dices_from(S).  
+000083c0: 2020 7472 696c 5f69 6478 203d 206e 702e    tril_idx = np.
+000083d0: 7472 696c 5f69 6e64 6963 6573 5f66 726f  tril_indices_fro
+000083e0: 6d28 532c 206b 3d2d 3129 0a20 2020 206e  m(S, k=-1).    n
+000083f0: 5f64 6961 6720 3d20 6c65 6e28 6469 6167  _diag = len(diag
+00008400: 5f69 6478 5b30 5d29 0a20 2020 206e 5f74  _idx[0]).    n_t
+00008410: 7269 6c20 3d20 6c65 6e28 7472 696c 5f69  ril = len(tril_i
+00008420: 6478 5b30 5d29 0a0a 2020 2020 6966 2069  dx[0])..    if i
+00008430: 6e69 7476 616c 2069 7320 6e6f 7420 4e6f  nitval is not No
+00008440: 6e65 3a0a 2020 2020 2020 2020 2320 496e  ne:.        # In
+00008450: 7665 7273 6520 7472 616e 7366 6f72 6d0a  verse transform.
+00008460: 2020 2020 2020 2020 696e 6974 7661 6c20          initval 
+00008470: 3d20 6e70 2e64 6f74 286e 702e 646f 7428  = np.dot(np.dot(
+00008480: 6e70 2e6c 696e 616c 672e 696e 7628 4c29  np.linalg.inv(L)
+00008490: 2c20 696e 6974 7661 6c29 2c20 6e70 2e6c  , initval), np.l
+000084a0: 696e 616c 672e 696e 7628 4c2e 5429 290a  inalg.inv(L.T)).
+000084b0: 2020 2020 2020 2020 696e 6974 7661 6c20          initval 
+000084c0: 3d20 6c69 6e61 6c67 2e63 686f 6c65 736b  = linalg.cholesk
+000084d0: 7928 696e 6974 7661 6c2c 206c 6f77 6572  y(initval, lower
+000084e0: 3d54 7275 6529 0a20 2020 2020 2020 2064  =True).        d
+000084f0: 6961 675f 7465 7374 7661 6c20 3d20 696e  iag_testval = in
+00008500: 6974 7661 6c5b 6469 6167 5f69 6478 5d20  itval[diag_idx] 
+00008510: 2a2a 2032 0a20 2020 2020 2020 2074 7269  ** 2.        tri
+00008520: 6c5f 7465 7374 7661 6c20 3d20 696e 6974  l_testval = init
+00008530: 7661 6c5b 7472 696c 5f69 6478 5d0a 2020  val[tril_idx].  
+00008540: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008550: 6469 6167 5f74 6573 7476 616c 203d 204e  diag_testval = N
+00008560: 6f6e 650a 2020 2020 2020 2020 7472 696c  one.        tril
+00008570: 5f74 6573 7476 616c 203d 204e 6f6e 650a  _testval = None.
+00008580: 0a20 2020 2063 203d 2070 742e 7371 7274  .    c = pt.sqrt
+00008590: 280a 2020 2020 2020 2020 4368 6953 7175  (.        ChiSqu
+000085a0: 6172 6564 2822 2573 5f63 2220 2520 6e61  ared("%s_c" % na
+000085b0: 6d65 2c20 6e75 202d 206e 702e 6172 616e  me, nu - np.aran
+000085c0: 6765 2832 2c20 3220 2b20 6e5f 6469 6167  ge(2, 2 + n_diag
+000085d0: 292c 2073 6861 7065 3d6e 5f64 6961 672c  ), shape=n_diag,
+000085e0: 2069 6e69 7476 616c 3d64 6961 675f 7465   initval=diag_te
+000085f0: 7374 7661 6c29 0a20 2020 2029 0a20 2020  stval).    ).   
+00008600: 2070 6d2e 5f6c 6f67 2e69 6e66 6f28 2241   pm._log.info("A
+00008610: 6464 6564 206e 6577 2076 6172 6961 626c  dded new variabl
+00008620: 6520 2573 5f63 2074 6f20 6d6f 6465 6c20  e %s_c to model 
+00008630: 6469 6167 6f6e 616c 206f 6620 5769 7368  diagonal of Wish
+00008640: 6172 742e 2220 2520 6e61 6d65 290a 2020  art." % name).  
+00008650: 2020 7a20 3d20 4e6f 726d 616c 2822 2573    z = Normal("%s
+00008660: 5f7a 2220 2520 6e61 6d65 2c20 302e 302c  _z" % name, 0.0,
+00008670: 2031 2e30 2c20 7368 6170 653d 6e5f 7472   1.0, shape=n_tr
+00008680: 696c 2c20 696e 6974 7661 6c3d 7472 696c  il, initval=tril
+00008690: 5f74 6573 7476 616c 290a 2020 2020 706d  _testval).    pm
+000086a0: 2e5f 6c6f 672e 696e 666f 2822 4164 6465  ._log.info("Adde
+000086b0: 6420 6e65 7720 7661 7269 6162 6c65 2025  d new variable %
+000086c0: 735f 7a20 746f 206d 6f64 656c 206f 6666  s_z to model off
+000086d0: 2d64 6961 676f 6e61 6c73 206f 6620 5769  -diagonals of Wi
+000086e0: 7368 6172 742e 2220 2520 6e61 6d65 290a  shart." % name).
+000086f0: 2020 2020 2320 436f 6e73 7472 7563 7420      # Construct 
+00008700: 4120 6d61 7472 6978 0a20 2020 2041 203d  A matrix.    A =
+00008710: 2070 742e 7a65 726f 7328 532e 7368 6170   pt.zeros(S.shap
+00008720: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00008730: 7433 3229 0a20 2020 2041 203d 2070 742e  t32).    A = pt.
+00008740: 7365 745f 7375 6274 656e 736f 7228 415b  set_subtensor(A[
+00008750: 6469 6167 5f69 6478 5d2c 2063 290a 2020  diag_idx], c).  
+00008760: 2020 4120 3d20 7074 2e73 6574 5f73 7562    A = pt.set_sub
+00008770: 7465 6e73 6f72 2841 5b74 7269 6c5f 6964  tensor(A[tril_id
+00008780: 785d 2c20 7a29 0a0a 2020 2020 2320 4c20  x], z)..    # L 
+00008790: 2a20 4120 2a20 412e 5420 2a20 4c2e 5420  * A * A.T * L.T 
+000087a0: 7e20 5769 7368 6172 7428 4c2a 4c2e 542c  ~ Wishart(L*L.T,
+000087b0: 206e 7529 0a20 2020 2069 6620 7265 7475   nu).    if retu
+000087c0: 726e 5f63 686f 6c65 736b 793a 0a20 2020  rn_cholesky:.   
+000087d0: 2020 2020 2072 6574 7572 6e20 706d 2e44       return pm.D
+000087e0: 6574 6572 6d69 6e69 7374 6963 286e 616d  eterministic(nam
+000087f0: 652c 2070 742e 646f 7428 4c2c 2041 2929  e, pt.dot(L, A))
+00008800: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00008810: 2020 2072 6574 7572 6e20 706d 2e44 6574     return pm.Det
+00008820: 6572 6d69 6e69 7374 6963 286e 616d 652c  erministic(name,
+00008830: 2070 742e 646f 7428 7074 2e64 6f74 2870   pt.dot(pt.dot(p
+00008840: 742e 646f 7428 4c2c 2041 292c 2041 2e54  t.dot(L, A), A.T
+00008850: 292c 204c 2e54 2929 0a0a 0a64 6566 205f  ), L.T))...def _
+00008860: 6c6b 6a5f 6e6f 726d 616c 697a 696e 675f  lkj_normalizing_
+00008870: 636f 6e73 7461 6e74 2865 7461 2c20 6e29  constant(eta, n)
+00008880: 3a0a 2020 2020 2320 544f 444f 3a20 5468  :.    # TODO: Th
+00008890: 6973 2069 7320 6d69 7869 6e67 2070 7974  is is mixing pyt
+000088a0: 686f 6e20 6272 616e 6368 696e 6720 7769  hon branching wi
+000088b0: 7468 2074 6865 2070 6f74 656e 7469 616c  th the potential
+000088c0: 6c79 2073 796d 626f 6c69 6320 6e20 616e  ly symbolic n an
+000088d0: 6420 6574 6120 7661 7269 6162 6c65 730a  d eta variables.
+000088e0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+000088f0: 7461 6e63 6528 6574 612c 2028 696e 742c  tance(eta, (int,
+00008900: 2066 6c6f 6174 2929 3a0a 2020 2020 2020   float)):.      
+00008910: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00008920: 6d65 6e74 6564 4572 726f 7228 2265 7461  mentedError("eta
+00008930: 206d 7573 7420 6265 2061 6e20 696e 7420   must be an int 
+00008940: 6f72 2066 6c6f 6174 2229 0a20 2020 2069  or float").    i
+00008950: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00008960: 286e 2c20 696e 7429 3a0a 2020 2020 2020  (n, int):.      
+00008970: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00008980: 6d65 6e74 6564 4572 726f 7228 226e 206d  mentedError("n m
+00008990: 7573 7420 6265 2061 6e20 696e 7465 6765  ust be an intege
+000089a0: 7222 290a 2020 2020 6966 2065 7461 203d  r").    if eta =
+000089b0: 3d20 313a 0a20 2020 2020 2020 2072 6573  = 1:.        res
+000089c0: 756c 7420 3d20 6761 6d6d 616c 6e28 322e  ult = gammaln(2.
+000089d0: 3020 2a20 7074 2e61 7261 6e67 6528 312c  0 * pt.arange(1,
+000089e0: 2069 6e74 2828 6e20 2d20 3129 202f 2032   int((n - 1) / 2
+000089f0: 2920 2b20 3129 292e 7375 6d28 290a 2020  ) + 1)).sum().  
+00008a00: 2020 2020 2020 6966 206e 2025 2032 203d        if n % 2 =
+00008a10: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00008a20: 2072 6573 756c 7420 2b3d 2028 0a20 2020   result += (.   
+00008a30: 2020 2020 2020 2020 2020 2020 2030 2e32               0.2
+00008a40: 3520 2a20 286e 2a2a 3220 2d20 3129 202a  5 * (n**2 - 1) *
+00008a50: 2070 742e 6c6f 6728 6e70 2e70 6929 0a20   pt.log(np.pi). 
+00008a60: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00008a70: 2030 2e32 3520 2a20 286e 202d 2031 2920   0.25 * (n - 1) 
+00008a80: 2a2a 2032 202a 2070 742e 6c6f 6728 322e  ** 2 * pt.log(2.
+00008a90: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00008aa0: 2020 202d 2028 6e20 2d20 3129 202a 2067     - (n - 1) * g
+00008ab0: 616d 6d61 6c6e 2869 6e74 2828 6e20 2b20  ammaln(int((n + 
+00008ac0: 3129 202f 2032 2929 0a20 2020 2020 2020  1) / 2)).       
+00008ad0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00008ae0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00008af0: 2072 6573 756c 7420 2b3d 2028 0a20 2020   result += (.   
+00008b00: 2020 2020 2020 2020 2020 2020 2030 2e32               0.2
+00008b10: 3520 2a20 6e20 2a20 286e 202d 2032 2920  5 * n * (n - 2) 
+00008b20: 2a20 7074 2e6c 6f67 286e 702e 7069 290a  * pt.log(np.pi).
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2b20 302e 3235 202a 2028 3320 2a20 6e2a  + 0.25 * (3 * n*
+00008b50: 2a32 202d 2034 202a 206e 2920 2a20 7074  *2 - 4 * n) * pt
+00008b60: 2e6c 6f67 2832 2e30 290a 2020 2020 2020  .log(2.0).      
+00008b70: 2020 2020 2020 2020 2020 2b20 6e20 2a20            + n * 
+00008b80: 6761 6d6d 616c 6e28 6e20 2f20 3229 0a20  gammaln(n / 2). 
+00008b90: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00008ba0: 2028 6e20 2d20 3129 202a 2067 616d 6d61   (n - 1) * gamma
+00008bb0: 6c6e 286e 290a 2020 2020 2020 2020 2020  ln(n).          
+00008bc0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+00008bd0: 2020 2020 2020 7265 7375 6c74 203d 202d        result = -
+00008be0: 286e 202d 2031 2920 2a20 6761 6d6d 616c  (n - 1) * gammal
+00008bf0: 6e28 6574 6120 2b20 302e 3520 2a20 286e  n(eta + 0.5 * (n
+00008c00: 202d 2031 2929 0a20 2020 2020 2020 206b   - 1)).        k
+00008c10: 203d 2070 742e 6172 616e 6765 2831 2c20   = pt.arange(1, 
+00008c20: 6e29 0a20 2020 2020 2020 2072 6573 756c  n).        resul
+00008c30: 7420 2b3d 2028 302e 3520 2a20 6b20 2a20  t += (0.5 * k * 
+00008c40: 7074 2e6c 6f67 286e 702e 7069 2920 2b20  pt.log(np.pi) + 
+00008c50: 6761 6d6d 616c 6e28 6574 6120 2b20 302e  gammaln(eta + 0.
+00008c60: 3520 2a20 286e 202d 2031 202d 206b 2929  5 * (n - 1 - k))
+00008c70: 292e 7375 6d28 290a 2020 2020 7265 7475  ).sum().    retu
+00008c80: 726e 2072 6573 756c 740a 0a0a 636c 6173  rn result...clas
+00008c90: 7320 5f4c 4b4a 4368 6f6c 6573 6b79 436f  s _LKJCholeskyCo
+00008ca0: 7642 6173 6552 5628 5261 6e64 6f6d 5661  vBaseRV(RandomVa
+00008cb0: 7269 6162 6c65 293a 0a20 2020 206e 616d  riable):.    nam
+00008cc0: 6520 3d20 225f 6c6b 6a63 686f 6c65 736b  e = "_lkjcholesk
+00008cd0: 7963 6f76 6261 7365 220a 2020 2020 6e64  ycovbase".    nd
+00008ce0: 696d 5f73 7570 7020 3d20 310a 2020 2020  im_supp = 1.    
+00008cf0: 6e64 696d 735f 7061 7261 6d73 203d 205b  ndims_params = [
+00008d00: 302c 2030 2c20 315d 0a20 2020 2064 7479  0, 0, 1].    dty
+00008d10: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
+00008d20: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
+00008d30: 2822 5f6c 6b6a 6368 6f6c 6573 6b79 636f  ("_lkjcholeskyco
+00008d40: 7662 6173 6522 2c20 225c 5c6f 7065 7261  vbase", "\\opera
+00008d50: 746f 726e 616d 657b 5f6c 6b6a 6368 6f6c  torname{_lkjchol
+00008d60: 6573 6b79 636f 7662 6173 657d 2229 0a0a  eskycovbase}")..
+00008d70: 2020 2020 6465 6620 6d61 6b65 5f6e 6f64      def make_nod
+00008d80: 6528 7365 6c66 2c20 726e 672c 2073 697a  e(self, rng, siz
+00008d90: 652c 2064 7479 7065 2c20 6e2c 2065 7461  e, dtype, n, eta
+00008da0: 2c20 4429 3a0a 2020 2020 2020 2020 6e20  , D):.        n 
+00008db0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00008dc0: 6172 6961 626c 6528 6e29 0a20 2020 2020  ariable(n).     
+00008dd0: 2020 2069 6620 6e6f 7420 6e2e 6e64 696d     if not n.ndim
+00008de0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00008df0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00008e00: 726f 7228 226e 206d 7573 7420 6265 2061  ror("n must be a
+00008e10: 2073 6361 6c61 7220 286e 6469 6d3d 3029   scalar (ndim=0)
+00008e20: 2e22 290a 0a20 2020 2020 2020 2065 7461  .")..        eta
+00008e30: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+00008e40: 7661 7269 6162 6c65 2865 7461 290a 2020  variable(eta).  
+00008e50: 2020 2020 2020 6966 206e 6f74 2065 7461        if not eta
+00008e60: 2e6e 6469 6d20 3d3d 2030 3a0a 2020 2020  .ndim == 0:.    
+00008e70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00008e80: 6c75 6545 7272 6f72 2822 6574 6120 6d75  lueError("eta mu
+00008e90: 7374 2062 6520 6120 7363 616c 6172 2028  st be a scalar (
+00008ea0: 6e64 696d 3d30 292e 2229 0a0a 2020 2020  ndim=0).")..    
+00008eb0: 2020 2020 4420 3d20 7074 2e61 735f 7465      D = pt.as_te
+00008ec0: 6e73 6f72 5f76 6172 6961 626c 6528 4429  nsor_variable(D)
+00008ed0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00008ee0: 2073 7570 6572 2829 2e6d 616b 655f 6e6f   super().make_no
+00008ef0: 6465 2872 6e67 2c20 7369 7a65 2c20 6474  de(rng, size, dt
+00008f00: 7970 652c 206e 2c20 6574 612c 2044 290a  ype, n, eta, D).
+00008f10: 0a20 2020 2064 6566 205f 7375 7070 5f73  .    def _supp_s
+00008f20: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
+00008f30: 2873 656c 662c 2064 6973 745f 7061 7261  (self, dist_para
+00008f40: 6d73 2c20 7061 7261 6d5f 7368 6170 6573  ms, param_shapes
+00008f50: 293a 0a20 2020 2020 2020 206e 203d 2064  ):.        n = d
+00008f60: 6973 745f 7061 7261 6d73 5b30 5d0a 2020  ist_params[0].  
+00008f70: 2020 2020 2020 7265 7475 726e 2028 286e        return ((n
+00008f80: 202a 2028 6e20 2b20 3129 2920 2f2f 2032   * (n + 1)) // 2
+00008f90: 2c29 0a0a 2020 2020 6465 6620 726e 675f  ,)..    def rng_
+00008fa0: 666e 2873 656c 662c 2072 6e67 2c20 6e2c  fn(self, rng, n,
+00008fb0: 2065 7461 2c20 442c 2073 697a 6529 3a0a   eta, D, size):.
+00008fc0: 2020 2020 2020 2020 2320 5765 2066 6c61          # We fla
+00008fd0: 7474 656e 2074 6865 2073 697a 6520 746f  tten the size to
+00008fe0: 206d 616b 6520 6f70 6572 6174 696f 6e73   make operations
+00008ff0: 2065 6173 6965 722c 2061 6e64 2074 6865   easier, and the
+00009000: 6e20 7265 6275 696c 6420 6974 0a20 2020  n rebuild it.   
+00009010: 2020 2020 2069 6620 7369 7a65 2069 7320       if size is 
+00009020: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009030: 2020 7369 7a65 203d 2044 2e73 6861 7065    size = D.shape
+00009040: 5b3a 2d31 5d0a 2020 2020 2020 2020 666c  [:-1].        fl
+00009050: 6174 5f73 697a 6520 3d20 6e70 2e70 726f  at_size = np.pro
+00009060: 6428 7369 7a65 292e 6173 7479 7065 2869  d(size).astype(i
+00009070: 6e74 290a 0a20 2020 2020 2020 2043 203d  nt)..        C =
+00009080: 204c 4b4a 436f 7272 5256 2e5f 7261 6e64   LKJCorrRV._rand
+00009090: 6f6d 5f63 6f72 725f 6d61 7472 6978 2872  om_corr_matrix(r
+000090a0: 6e67 3d72 6e67 2c20 6e3d 6e2c 2065 7461  ng=rng, n=n, eta
+000090b0: 3d65 7461 2c20 666c 6174 5f73 697a 653d  =eta, flat_size=
+000090c0: 666c 6174 5f73 697a 6529 0a20 2020 2020  flat_size).     
+000090d0: 2020 2044 203d 2044 2e72 6573 6861 7065     D = D.reshape
+000090e0: 2866 6c61 745f 7369 7a65 2c20 6e29 0a20  (flat_size, n). 
+000090f0: 2020 2020 2020 2043 202a 3d20 445b 2e2e         C *= D[..
+00009100: 2e2c 203a 2c20 6e70 2e6e 6577 6178 6973  ., :, np.newaxis
+00009110: 5d20 2a20 445b 2e2e 2e2c 206e 702e 6e65  ] * D[..., np.ne
+00009120: 7761 7869 732c 203a 5d0a 0a20 2020 2020  waxis, :]..     
+00009130: 2020 2074 7269 6c5f 6964 7820 3d20 6e70     tril_idx = np
+00009140: 2e74 7269 6c5f 696e 6469 6365 7328 6e2c  .tril_indices(n,
+00009150: 206b 3d30 290a 2020 2020 2020 2020 7361   k=0).        sa
+00009160: 6d70 6c65 7320 3d20 6e70 2e6c 696e 616c  mples = np.linal
+00009170: 672e 6368 6f6c 6573 6b79 2843 295b 2e2e  g.cholesky(C)[..
+00009180: 2e2c 2074 7269 6c5f 6964 785b 305d 2c20  ., tril_idx[0], 
+00009190: 7472 696c 5f69 6478 5b31 5d5d 0a0a 2020  tril_idx[1]]..  
+000091a0: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
+000091b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000091c0: 2020 2073 616d 706c 6573 203d 2073 616d     samples = sam
+000091d0: 706c 6573 5b30 5d0a 2020 2020 2020 2020  ples[0].        
+000091e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000091f0: 2020 6469 7374 5f73 6861 7065 203d 2028    dist_shape = (
+00009200: 6e20 2a20 286e 202b 2031 2929 202f 2f20  n * (n + 1)) // 
+00009210: 320a 2020 2020 2020 2020 2020 2020 7361  2.            sa
+00009220: 6d70 6c65 7320 3d20 6e70 2e72 6573 6861  mples = np.resha
+00009230: 7065 2873 616d 706c 6573 2c20 282a 7369  pe(samples, (*si
+00009240: 7a65 2c20 6469 7374 5f73 6861 7065 2929  ze, dist_shape))
+00009250: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00009260: 2073 616d 706c 6573 0a0a 0a5f 6c6a 6b5f   samples..._ljk_
+00009270: 6368 6f6c 6573 6b79 5f63 6f76 5f62 6173  cholesky_cov_bas
+00009280: 6520 3d20 5f4c 4b4a 4368 6f6c 6573 6b79  e = _LKJCholesky
+00009290: 436f 7642 6173 6552 5628 290a 0a0a 2320  CovBaseRV()...# 
+000092a0: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7642  _LKJCholeskyCovB
+000092b0: 6173 6552 5620 7265 7175 6972 6573 2061  aseRV requires a
+000092c0: 2070 726f 7065 726c 7920 7368 6170 6564   properly shaped
+000092d0: 2060 4460 2c20 7768 6963 6820 6d65 616e   `D`, which mean
+000092e0: 7320 7468 6520 7661 7269 6162 6c65 2063  s the variable c
+000092f0: 616e 2774 0a23 2062 6520 7361 6665 6c79  an't.# be safely
+00009300: 2072 6573 697a 6564 2e20 4265 6361 7573   resized. Becaus
+00009310: 6520 6f66 2074 6869 732c 2077 6520 6164  e of this, we ad
+00009320: 6420 7468 6520 7468 696e 2053 796d 626f  d the thin Symbo
+00009330: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
+00009340: 6520 7772 6170 7065 720a 636c 6173 7320  e wrapper.class 
+00009350: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7652  _LKJCholeskyCovR
+00009360: 5628 5379 6d62 6f6c 6963 5261 6e64 6f6d  V(SymbolicRandom
+00009370: 5661 7269 6162 6c65 293a 0a20 2020 2064  Variable):.    d
+00009380: 6566 6175 6c74 5f6f 7574 7075 7420 3d20  efault_output = 
+00009390: 310a 2020 2020 5f70 7269 6e74 5f6e 616d  1.    _print_nam
+000093a0: 6520 3d20 2822 5f6c 6b6a 6368 6f6c 6573  e = ("_lkjcholes
+000093b0: 6b79 636f 7622 2c20 225c 5c6f 7065 7261  kycov", "\\opera
+000093c0: 746f 726e 616d 657b 5f6c 6b6a 6368 6f6c  torname{_lkjchol
+000093d0: 6573 6b79 636f 767d 2229 0a0a 2020 2020  eskycov}")..    
+000093e0: 6465 6620 7570 6461 7465 2873 656c 662c  def update(self,
+000093f0: 206e 6f64 6529 3a0a 2020 2020 2020 2020   node):.        
+00009400: 7265 7475 726e 207b 6e6f 6465 2e69 6e70  return {node.inp
+00009410: 7574 735b 305d 3a20 6e6f 6465 2e6f 7574  uts[0]: node.out
+00009420: 7075 7473 5b30 5d7d 0a0a 0a63 6c61 7373  puts[0]}...class
+00009430: 205f 4c4b 4a43 686f 6c65 736b 7943 6f76   _LKJCholeskyCov
+00009440: 2844 6973 7472 6962 7574 696f 6e29 3a0a  (Distribution):.
+00009450: 2020 2020 7222 2222 556e 6465 726c 7969      r"""Underlyi
+00009460: 6e67 2063 6c61 7373 2066 6f72 2063 6f76  ng class for cov
+00009470: 6172 6961 6e63 6520 6d61 7472 6978 2077  ariance matrix w
+00009480: 6974 6820 4c4b 4a20 6469 7374 7269 6275  ith LKJ distribu
+00009490: 7465 6420 636f 7272 656c 6174 696f 6e73  ted correlations
+000094a0: 2e0a 2020 2020 5365 6520 646f 6373 2066  ..    See docs f
+000094b0: 6f72 204c 4b4a 4368 6f6c 6573 6b79 436f  or LKJCholeskyCo
+000094c0: 7620 6675 6e63 7469 6f6e 2066 6f72 206d  v function for m
+000094d0: 6f72 6520 6465 7461 696c 7320 6f6e 2068  ore details on h
+000094e0: 6f77 2074 6f20 7573 6520 6974 2069 6e20  ow to use it in 
+000094f0: 6d6f 6465 6c73 2e0a 2020 2020 2222 220a  models..    """.
+00009500: 0a20 2020 2072 765f 7479 7065 203d 205f  .    rv_type = _
+00009510: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
+00009520: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00009530: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
+00009540: 636c 732c 206e 2c20 6574 612c 2073 645f  cls, n, eta, sd_
+00009550: 6469 7374 2c20 2a2a 6b77 6172 6773 293a  dist, **kwargs):
+00009560: 0a20 2020 2020 2020 206e 203d 2070 742e  .        n = pt.
+00009570: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00009580: 6c65 2869 6e74 5828 6e29 290a 2020 2020  le(intX(n)).    
+00009590: 2020 2020 6574 6120 3d20 7074 2e61 735f      eta = pt.as_
+000095a0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+000095b0: 666c 6f61 7458 2865 7461 2929 0a0a 2020  floatX(eta))..  
+000095c0: 2020 2020 2020 6966 206e 6f74 2028 0a20        if not (. 
+000095d0: 2020 2020 2020 2020 2020 2069 7369 6e73             isins
+000095e0: 7461 6e63 6528 7364 5f64 6973 742c 2056  tance(sd_dist, V
+000095f0: 6172 6961 626c 6529 0a20 2020 2020 2020  ariable).       
+00009600: 2020 2020 2061 6e64 2073 645f 6469 7374       and sd_dist
+00009610: 2e6f 776e 6572 2069 7320 6e6f 7420 4e6f  .owner is not No
+00009620: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
+00009630: 6e64 2069 7369 6e73 7461 6e63 6528 7364  nd isinstance(sd
+00009640: 5f64 6973 742e 6f77 6e65 722e 6f70 2c20  _dist.owner.op, 
+00009650: 2852 616e 646f 6d56 6172 6961 626c 652c  (RandomVariable,
+00009660: 2053 796d 626f 6c69 6352 616e 646f 6d56   SymbolicRandomV
+00009670: 6172 6961 626c 6529 290a 2020 2020 2020  ariable)).      
+00009680: 2020 2020 2020 616e 6420 7364 5f64 6973        and sd_dis
+00009690: 742e 6f77 6e65 722e 6f70 2e6e 6469 6d5f  t.owner.op.ndim_
+000096a0: 7375 7070 203c 2032 0a20 2020 2020 2020  supp < 2.       
+000096b0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000096c0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+000096d0: 2273 645f 6469 7374 206d 7573 7420 6265  "sd_dist must be
+000096e0: 2061 2073 6361 6c61 7220 6f72 2076 6563   a scalar or vec
+000096f0: 746f 7220 6469 7374 7269 6275 7469 6f6e  tor distribution
+00009700: 2076 6172 6961 626c 6522 290a 0a20 2020   variable")..   
+00009710: 2020 2020 2063 6865 636b 5f64 6973 745f       check_dist_
+00009720: 6e6f 745f 7265 6769 7374 6572 6564 2873  not_registered(s
+00009730: 645f 6469 7374 290a 2020 2020 2020 2020  d_dist).        
+00009740: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
+00009750: 6973 7428 5b6e 2c20 6574 612c 2073 645f  ist([n, eta, sd_
+00009760: 6469 7374 5d2c 202a 2a6b 7761 7267 7329  dist], **kwargs)
+00009770: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00009780: 6f64 0a20 2020 2064 6566 2072 765f 6f70  od.    def rv_op
+00009790: 2863 6c73 2c20 6e2c 2065 7461 2c20 7364  (cls, n, eta, sd
+000097a0: 5f64 6973 742c 2073 697a 653d 4e6f 6e65  _dist, size=None
+000097b0: 293a 0a20 2020 2020 2020 2023 2057 6520  ):.        # We 
+000097c0: 7265 7369 7a65 2074 6865 2073 645f 6469  resize the sd_di
+000097d0: 7374 2061 7574 6f6d 6174 6963 616c 6c79  st automatically
+000097e0: 2073 6f20 7468 6174 2069 7420 6861 7320   so that it has 
+000097f0: 2873 697a 6520 7820 6e29 2069 6e64 6570  (size x n) indep
+00009800: 656e 6465 6e74 0a20 2020 2020 2020 2023  endent.        #
+00009810: 2064 7261 7773 2077 6869 6368 2069 7320   draws which is 
+00009820: 7768 6174 2074 6865 2060 5f4c 4b4a 4368  what the `_LKJCh
+00009830: 6f6c 6573 6b79 436f 7642 6173 6552 562e  oleskyCovBaseRV.
+00009840: 726e 675f 666e 6020 6578 7065 6374 732e  rng_fn` expects.
+00009850: 2054 6869 7320 6d61 6b65 7320 7468 650a   This makes the.
+00009860: 2020 2020 2020 2020 2320 7261 6e64 6f6d          # random
+00009870: 2061 6e64 206c 6f67 7020 6d65 7468 6f64   and logp method
+00009880: 7320 6571 7569 7661 6c65 6e74 2c20 6173  s equivalent, as
+00009890: 2074 6865 206c 6174 7465 7220 616c 736f   the latter also
+000098a0: 2061 7373 756d 6573 2061 2075 6e69 7175   assumes a uniqu
+000098b0: 6520 7661 6c75 650a 2020 2020 2020 2020  e value.        
+000098c0: 2320 666f 7220 6561 6368 2064 6961 676f  # for each diago
+000098d0: 6e61 6c20 656c 656d 656e 742e 0a20 2020  nal element..   
+000098e0: 2020 2020 2023 2053 696e 6365 2060 6574       # Since `et
+000098f0: 6160 2061 6e64 2060 6e60 2061 7265 2066  a` and `n` are f
+00009900: 6f72 6365 6420 746f 2062 6520 7363 616c  orced to be scal
+00009910: 6172 7320 7765 2064 6f6e 2774 206e 6565  ars we don't nee
+00009920: 6420 746f 2077 6f72 7279 2061 626f 7574  d to worry about
+00009930: 0a20 2020 2020 2020 2023 2069 6d70 6c69  .        # impli
+00009940: 6564 2062 6174 6368 6564 2064 696d 656e  ed batched dimen
+00009950: 7369 6f6e 7320 6672 6f6d 2074 686f 7365  sions from those
+00009960: 2066 6f72 2074 6865 2074 696d 6520 6265   for the time be
+00009970: 696e 672e 0a20 2020 2020 2020 2069 6620  ing..        if 
+00009980: 7369 7a65 2069 7320 4e6f 6e65 3a0a 2020  size is None:.  
+00009990: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
+000099a0: 2073 645f 6469 7374 2e73 6861 7065 5b3a   sd_dist.shape[:
+000099b0: 2d31 5d0a 2020 2020 2020 2020 7368 6170  -1].        shap
+000099c0: 6520 3d20 7475 706c 6528 7369 7a65 2920  e = tuple(size) 
+000099d0: 2b20 286e 2c29 0a20 2020 2020 2020 2069  + (n,).        i
+000099e0: 6620 7364 5f64 6973 742e 6f77 6e65 722e  f sd_dist.owner.
+000099f0: 6f70 2e6e 6469 6d5f 7375 7070 203d 3d20  op.ndim_supp == 
+00009a00: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
+00009a10: 645f 6469 7374 203d 2063 6861 6e67 655f  d_dist = change_
+00009a20: 6469 7374 5f73 697a 6528 7364 5f64 6973  dist_size(sd_dis
+00009a30: 742c 2073 6861 7065 290a 2020 2020 2020  t, shape).      
+00009a40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009a50: 2020 2020 2320 5468 6520 7375 7070 6f72      # The suppor
+00009a60: 7420 7368 6170 6520 6d75 7374 2062 6520  t shape must be 
+00009a70: 606e 6020 6275 7420 7765 2068 6176 6520  `n` but we have 
+00009a80: 6e6f 2077 6179 206f 6620 636f 6e74 726f  no way of contro
+00009a90: 6c6c 696e 6720 6974 0a20 2020 2020 2020  lling it.       
+00009aa0: 2020 2020 2073 645f 6469 7374 203d 2063       sd_dist = c
+00009ab0: 6861 6e67 655f 6469 7374 5f73 697a 6528  hange_dist_size(
+00009ac0: 7364 5f64 6973 742c 2073 6861 7065 5b3a  sd_dist, shape[:
+00009ad0: 2d31 5d29 0a0a 2020 2020 2020 2020 2320  -1])..        # 
+00009ae0: 4372 6561 7465 206e 6577 2072 6e67 2066  Create new rng f
+00009af0: 6f72 2074 6865 205f 6c6b 6a63 686f 6c65  or the _lkjchole
+00009b00: 736b 7963 6f76 2069 6e74 6572 6e61 6c20  skycov internal 
+00009b10: 5256 0a20 2020 2020 2020 2072 6e67 203d  RV.        rng =
+00009b20: 2070 7974 656e 736f 722e 7368 6172 6564   pytensor.shared
+00009b30: 286e 702e 7261 6e64 6f6d 2e64 6566 6175  (np.random.defau
+00009b40: 6c74 5f72 6e67 2829 290a 0a20 2020 2020  lt_rng())..     
+00009b50: 2020 2072 6e67 5f2c 206e 5f2c 2065 7461     rng_, n_, eta
+00009b60: 5f2c 2073 645f 6469 7374 5f20 3d20 726e  _, sd_dist_ = rn
+00009b70: 672e 7479 7065 2829 2c20 6e2e 7479 7065  g.type(), n.type
+00009b80: 2829 2c20 6574 612e 7479 7065 2829 2c20  (), eta.type(), 
+00009b90: 7364 5f64 6973 742e 7479 7065 2829 0a20  sd_dist.type(). 
+00009ba0: 2020 2020 2020 206e 6578 745f 726e 675f         next_rng_
+00009bb0: 2c20 6c6b 6a63 6f76 5f20 3d20 5f6c 6a6b  , lkjcov_ = _ljk
+00009bc0: 5f63 686f 6c65 736b 795f 636f 765f 6261  _cholesky_cov_ba
+00009bd0: 7365 286e 5f2c 2065 7461 5f2c 2073 645f  se(n_, eta_, sd_
+00009be0: 6469 7374 5f2c 2072 6e67 3d72 6e67 5f29  dist_, rng=rng_)
+00009bf0: 2e6f 776e 6572 2e6f 7574 7075 7473 0a0a  .owner.outputs..
+00009c00: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00009c10: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
+00009c20: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+00009c30: 7075 7473 3d5b 726e 675f 2c20 6e5f 2c20  puts=[rng_, n_, 
+00009c40: 6574 615f 2c20 7364 5f64 6973 745f 5d2c  eta_, sd_dist_],
+00009c50: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00009c60: 7075 7473 3d5b 6e65 7874 5f72 6e67 5f2c  puts=[next_rng_,
+00009c70: 206c 6b6a 636f 765f 5d2c 0a20 2020 2020   lkjcov_],.     
+00009c80: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
+00009c90: 3d31 2c0a 2020 2020 2020 2020 2928 726e  =1,.        )(rn
+00009ca0: 672c 206e 2c20 6574 612c 2073 645f 6469  g, n, eta, sd_di
+00009cb0: 7374 290a 0a0a 405f 6368 616e 6765 5f64  st)...@_change_d
+00009cc0: 6973 745f 7369 7a65 2e72 6567 6973 7465  ist_size.registe
+00009cd0: 7228 5f4c 4b4a 4368 6f6c 6573 6b79 436f  r(_LKJCholeskyCo
+00009ce0: 7652 5629 0a64 6566 2063 6861 6e67 655f  vRV).def change_
+00009cf0: 4c4b 4a43 686f 6c65 6b73 7943 6f76 5256  LKJCholeksyCovRV
+00009d00: 5f73 697a 6528 6f70 2c20 6469 7374 2c20  _size(op, dist, 
+00009d10: 6e65 775f 7369 7a65 2c20 6578 7061 6e64  new_size, expand
+00009d20: 3d46 616c 7365 293a 0a20 2020 206e 2c20  =False):.    n, 
+00009d30: 6574 612c 2073 645f 6469 7374 203d 2064  eta, sd_dist = d
+00009d40: 6973 742e 6f77 6e65 722e 696e 7075 7473  ist.owner.inputs
+00009d50: 5b31 3a5d 0a0a 2020 2020 6966 2065 7870  [1:]..    if exp
+00009d60: 616e 643a 0a20 2020 2020 2020 206f 6c64  and:.        old
+00009d70: 5f73 697a 6520 3d20 7364 5f64 6973 742e  _size = sd_dist.
+00009d80: 7368 6170 655b 3a2d 315d 0a20 2020 2020  shape[:-1].     
+00009d90: 2020 206e 6577 5f73 697a 6520 3d20 7475     new_size = tu
+00009da0: 706c 6528 6e65 775f 7369 7a65 2920 2b20  ple(new_size) + 
+00009db0: 7475 706c 6528 6f6c 645f 7369 7a65 290a  tuple(old_size).
+00009dc0: 0a20 2020 2072 6574 7572 6e20 5f4c 4b4a  .    return _LKJ
+00009dd0: 4368 6f6c 6573 6b79 436f 762e 7276 5f6f  CholeskyCov.rv_o
+00009de0: 7028 6e2c 2065 7461 2c20 7364 5f64 6973  p(n, eta, sd_dis
+00009df0: 742c 2073 697a 653d 6e65 775f 7369 7a65  t, size=new_size
+00009e00: 290a 0a0a 405f 6d6f 6d65 6e74 2e72 6567  )...@_moment.reg
+00009e10: 6973 7465 7228 5f4c 4b4a 4368 6f6c 6573  ister(_LKJCholes
+00009e20: 6b79 436f 7652 5629 0a64 6566 205f 4c4b  kyCovRV).def _LK
+00009e30: 4a43 686f 6c65 6b73 7943 6f76 5256 5f6d  JCholeksyCovRV_m
+00009e40: 6f6d 656e 7428 6f70 2c20 7276 2c20 726e  oment(op, rv, rn
+00009e50: 672c 206e 2c20 6574 612c 2073 645f 6469  g, n, eta, sd_di
+00009e60: 7374 293a 0a20 2020 2064 6961 675f 6964  st):.    diag_id
+00009e70: 7873 203d 2028 7074 2e63 756d 7375 6d28  xs = (pt.cumsum(
+00009e80: 7074 2e61 7261 6e67 6528 312c 206e 202b  pt.arange(1, n +
+00009e90: 2031 2929 202d 2031 292e 6173 7479 7065   1)) - 1).astype
+00009ea0: 2822 696e 7433 3222 290a 2020 2020 6d6f  ("int32").    mo
+00009eb0: 6d65 6e74 203d 2070 742e 7a65 726f 735f  ment = pt.zeros_
+00009ec0: 6c69 6b65 2872 7629 0a20 2020 206d 6f6d  like(rv).    mom
+00009ed0: 656e 7420 3d20 7074 2e73 6574 5f73 7562  ent = pt.set_sub
+00009ee0: 7465 6e73 6f72 286d 6f6d 656e 745b 2e2e  tensor(moment[..
+00009ef0: 2e2c 2064 6961 675f 6964 7873 5d2c 2031  ., diag_idxs], 1
+00009f00: 290a 2020 2020 7265 7475 726e 206d 6f6d  ).    return mom
+00009f10: 656e 740a 0a0a 405f 6465 6661 756c 745f  ent...@_default_
+00009f20: 7472 616e 7366 6f72 6d2e 7265 6769 7374  transform.regist
+00009f30: 6572 285f 4c4b 4a43 686f 6c65 736b 7943  er(_LKJCholeskyC
+00009f40: 6f76 5256 290a 6465 6620 5f4c 4b4a 4368  ovRV).def _LKJCh
+00009f50: 6f6c 656b 7379 436f 7652 565f 6465 6661  oleksyCovRV_defa
+00009f60: 756c 745f 7472 616e 7366 6f72 6d28 6f70  ult_transform(op
+00009f70: 2c20 7276 293a 0a20 2020 205f 2c20 6e2c  , rv):.    _, n,
+00009f80: 205f 2c20 5f20 3d20 7276 2e6f 776e 6572   _, _ = rv.owner
+00009f90: 2e69 6e70 7574 730a 2020 2020 7265 7475  .inputs.    retu
+00009fa0: 726e 2074 7261 6e73 666f 726d 732e 4368  rn transforms.Ch
+00009fb0: 6f6c 6573 6b79 436f 7650 6163 6b65 6428  oleskyCovPacked(
+00009fc0: 6e29 0a0a 0a40 5f6c 6f67 7072 6f62 2e72  n)...@_logprob.r
+00009fd0: 6567 6973 7465 7228 5f4c 4b4a 4368 6f6c  egister(_LKJChol
+00009fe0: 6573 6b79 436f 7652 5629 0a64 6566 205f  eskyCovRV).def _
+00009ff0: 4c4b 4a43 686f 6c65 6b73 7943 6f76 5256  LKJCholeksyCovRV
+0000a000: 5f6c 6f67 7028 6f70 2c20 7661 6c75 6573  _logp(op, values
+0000a010: 2c20 726e 672c 206e 2c20 6574 612c 2073  , rng, n, eta, s
+0000a020: 645f 6469 7374 2c20 2a2a 6b77 6172 6773  d_dist, **kwargs
+0000a030: 293a 0a20 2020 2028 7661 6c75 652c 2920  ):.    (value,) 
+0000a040: 3d20 7661 6c75 6573 0a0a 2020 2020 6966  = values..    if
+0000a050: 2076 616c 7565 2e6e 6469 6d20 3e20 313a   value.ndim > 1:
+0000a060: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+0000a070: 616c 7565 4572 726f 7228 225f 4c4b 4a43  alueError("_LKJC
+0000a080: 686f 6c65 736b 7943 6f76 206c 6f67 7020  holeskyCov logp 
+0000a090: 6973 206f 6e6c 7920 696d 706c 656d 656e  is only implemen
+0000a0a0: 7465 6420 666f 7220 7665 6374 6f72 2076  ted for vector v
+0000a0b0: 616c 7565 7320 286e 6469 6d3d 3129 2229  alues (ndim=1)")
+0000a0c0: 0a0a 2020 2020 6469 6167 5f69 6478 7320  ..    diag_idxs 
+0000a0d0: 3d20 7074 2e63 756d 7375 6d28 7074 2e61  = pt.cumsum(pt.a
+0000a0e0: 7261 6e67 6528 312c 206e 202b 2031 2929  range(1, n + 1))
+0000a0f0: 202d 2031 0a20 2020 2063 756d 7375 6d20   - 1.    cumsum 
+0000a100: 3d20 7074 2e63 756d 7375 6d28 7661 6c75  = pt.cumsum(valu
+0000a110: 652a 2a32 290a 2020 2020 7661 7269 616e  e**2).    varian
+0000a120: 6365 203d 2070 742e 7a65 726f 7328 7074  ce = pt.zeros(pt
+0000a130: 2e61 746c 6561 7374 5f31 6428 6e29 290a  .atleast_1d(n)).
+0000a140: 2020 2020 7661 7269 616e 6365 203d 2070      variance = p
+0000a150: 742e 696e 635f 7375 6274 656e 736f 7228  t.inc_subtensor(
+0000a160: 7661 7269 616e 6365 5b30 5d2c 2076 616c  variance[0], val
+0000a170: 7565 5b30 5d20 2a2a 2032 290a 2020 2020  ue[0] ** 2).    
+0000a180: 7661 7269 616e 6365 203d 2070 742e 696e  variance = pt.in
+0000a190: 635f 7375 6274 656e 736f 7228 7661 7269  c_subtensor(vari
+0000a1a0: 616e 6365 5b31 3a5d 2c20 6375 6d73 756d  ance[1:], cumsum
+0000a1b0: 5b64 6961 675f 6964 7873 5b31 3a5d 5d20  [diag_idxs[1:]] 
+0000a1c0: 2d20 6375 6d73 756d 5b64 6961 675f 6964  - cumsum[diag_id
+0000a1d0: 7873 5b3a 2d31 5d5d 290a 2020 2020 7364  xs[:-1]]).    sd
+0000a1e0: 5f76 616c 7320 3d20 7074 2e73 7172 7428  _vals = pt.sqrt(
+0000a1f0: 7661 7269 616e 6365 290a 0a20 2020 206c  variance)..    l
+0000a200: 6f67 705f 7364 203d 2070 6d2e 6c6f 6770  ogp_sd = pm.logp
+0000a210: 2873 645f 6469 7374 2c20 7364 5f76 616c  (sd_dist, sd_val
+0000a220: 7329 2e73 756d 2829 0a20 2020 2063 6f72  s).sum().    cor
+0000a230: 725f 6469 6167 203d 2076 616c 7565 5b64  r_diag = value[d
+0000a240: 6961 675f 6964 7873 5d20 2f20 7364 5f76  iag_idxs] / sd_v
+0000a250: 616c 730a 0a20 2020 206c 6f67 705f 6c6b  als..    logp_lk
+0000a260: 6a20 3d20 2832 202a 2065 7461 202d 2033  j = (2 * eta - 3
+0000a270: 202b 206e 202d 2070 742e 6172 616e 6765   + n - pt.arange
+0000a280: 286e 2929 202a 2070 742e 6c6f 6728 636f  (n)) * pt.log(co
+0000a290: 7272 5f64 6961 6729 0a20 2020 206c 6f67  rr_diag).    log
+0000a2a0: 705f 6c6b 6a20 3d20 7074 2e73 756d 286c  p_lkj = pt.sum(l
+0000a2b0: 6f67 705f 6c6b 6a29 0a0a 2020 2020 2320  ogp_lkj)..    # 
+0000a2c0: 436f 6d70 7574 6520 7468 6520 6c6f 6720  Compute the log 
+0000a2d0: 6465 7420 6a61 636f 6269 616e 206f 6620  det jacobian of 
+0000a2e0: 7468 6520 7365 636f 6e64 2074 7261 6e73  the second trans
+0000a2f0: 666f 726d 6174 696f 6e0a 2020 2020 2320  formation.    # 
+0000a300: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
+0000a310: 2064 6f63 7374 7269 6e67 2e0a 2020 2020   docstring..    
+0000a320: 6964 7820 3d20 7074 2e61 7261 6e67 6528  idx = pt.arange(
+0000a330: 6e29 0a20 2020 2064 6574 5f69 6e76 6a61  n).    det_invja
+0000a340: 6320 3d20 7074 2e6c 6f67 2863 6f72 725f  c = pt.log(corr_
+0000a350: 6469 6167 2920 2d20 6964 7820 2a20 7074  diag) - idx * pt
+0000a360: 2e6c 6f67 2873 645f 7661 6c73 290a 2020  .log(sd_vals).  
+0000a370: 2020 6465 745f 696e 766a 6163 203d 2064    det_invjac = d
+0000a380: 6574 5f69 6e76 6a61 632e 7375 6d28 290a  et_invjac.sum().
+0000a390: 0a20 2020 2023 2054 4f44 4f3a 205f 6c6b  .    # TODO: _lk
+0000a3a0: 6a5f 6e6f 726d 616c 697a 696e 675f 636f  j_normalizing_co
+0000a3b0: 6e73 7461 6e74 2063 7572 7265 6e74 6c79  nstant currently
+0000a3c0: 2072 6571 7569 7265 7320 6065 7461 6020   requires `eta` 
+0000a3d0: 616e 6420 606e 6020 746f 2062 6520 636f  and `n` to be co
+0000a3e0: 6e73 7461 6e74 730a 2020 2020 6966 206e  nstants.    if n
+0000a3f0: 6f74 2069 7369 6e73 7461 6e63 6528 6e2c  ot isinstance(n,
+0000a400: 2043 6f6e 7374 616e 7429 3a0a 2020 2020   Constant):.    
+0000a410: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+0000a420: 6c65 6d65 6e74 6564 4572 726f 7228 226c  lementedError("l
+0000a430: 6f67 7020 6f6e 6c79 2069 6d70 6c65 6d65  ogp only impleme
+0000a440: 6e74 6564 2066 6f72 2063 6f6e 7374 616e  nted for constan
+0000a450: 7420 606e 6022 290a 2020 2020 6e20 3d20  t `n`").    n = 
+0000a460: 696e 7428 6e2e 6461 7461 290a 0a20 2020  int(n.data)..   
+0000a470: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000a480: 6365 2865 7461 2c20 436f 6e73 7461 6e74  ce(eta, Constant
+0000a490: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+0000a4a0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+0000a4b0: 7272 6f72 2822 6c6f 6770 206f 6e6c 7920  rror("logp only 
+0000a4c0: 696d 706c 656d 656e 7465 6420 666f 7220  implemented for 
+0000a4d0: 636f 6e73 7461 6e74 2060 6574 6160 2229  constant `eta`")
+0000a4e0: 0a20 2020 2065 7461 203d 2066 6c6f 6174  .    eta = float
+0000a4f0: 2865 7461 2e64 6174 6129 0a0a 2020 2020  (eta.data)..    
+0000a500: 6e6f 726d 203d 205f 6c6b 6a5f 6e6f 726d  norm = _lkj_norm
+0000a510: 616c 697a 696e 675f 636f 6e73 7461 6e74  alizing_constant
+0000a520: 2865 7461 2c20 6e29 0a0a 2020 2020 7265  (eta, n)..    re
+0000a530: 7475 726e 206e 6f72 6d20 2b20 6c6f 6770  turn norm + logp
+0000a540: 5f6c 6b6a 202b 206c 6f67 705f 7364 202b  _lkj + logp_sd +
+0000a550: 2064 6574 5f69 6e76 6a61 630a 0a0a 636c   det_invjac...cl
+0000a560: 6173 7320 4c4b 4a43 686f 6c65 736b 7943  ass LKJCholeskyC
+0000a570: 6f76 3a0a 2020 2020 7222 2222 5772 6170  ov:.    r"""Wrap
+0000a580: 7065 7220 636c 6173 7320 666f 7220 636f  per class for co
+0000a590: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+0000a5a0: 7769 7468 204c 4b4a 2064 6973 7472 6962  with LKJ distrib
+0000a5b0: 7574 6564 2063 6f72 7265 6c61 7469 6f6e  uted correlation
+0000a5c0: 732e 0a0a 2020 2020 5468 6973 2064 6566  s...    This def
+0000a5d0: 696e 6573 2061 2064 6973 7472 6962 7574  ines a distribut
+0000a5e0: 696f 6e20 6f76 6572 2043 686f 6c65 736b  ion over Cholesk
+0000a5f0: 7920 6465 636f 6d70 6f73 6564 2063 6f76  y decomposed cov
+0000a600: 6172 6961 6e63 650a 2020 2020 6d61 7472  ariance.    matr
+0000a610: 6963 6573 2c20 7375 6368 2074 6861 7420  ices, such that 
+0000a620: 7468 6520 756e 6465 726c 7969 6e67 2063  the underlying c
+0000a630: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+0000a640: 6365 7320 666f 6c6c 6f77 2061 6e0a 2020  ces follow an.  
+0000a650: 2020 4c4b 4a20 6469 7374 7269 6275 7469    LKJ distributi
+0000a660: 6f6e 205b 315d 2061 6e64 2074 6865 2073  on [1] and the s
+0000a670: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
+0000a680: 6e73 2066 6f6c 6c6f 7720 616e 2061 7262  ns follow an arb
+0000a690: 6974 7261 7279 0a20 2020 2064 6973 7472  itrary.    distr
+0000a6a0: 6962 7574 696f 6e20 7370 6563 6966 6965  ibution specifie
+0000a6b0: 6420 6279 2074 6865 2075 7365 722e 0a0a  d by the user...
+0000a6c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000a6d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000a6e0: 2020 6e61 6d65 203a 2073 7472 0a20 2020    name : str.   
+0000a6f0: 2020 2020 2054 6865 206e 616d 6520 6769       The name gi
+0000a700: 7665 6e20 746f 2074 6865 2076 6172 6961  ven to the varia
+0000a710: 626c 6520 696e 2074 6865 206d 6f64 656c  ble in the model
+0000a720: 2e0a 2020 2020 6574 6120 3a20 7465 6e73  ..    eta : tens
+0000a730: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+0000a740: 0a20 2020 2020 2020 2054 6865 2073 6861  .        The sha
+0000a750: 7065 2070 6172 616d 6574 6572 2028 6574  pe parameter (et
+0000a760: 6120 3e20 3029 206f 6620 7468 6520 4c4b  a > 0) of the LK
+0000a770: 4a20 6469 7374 7269 6275 7469 6f6e 2e20  J distribution. 
+0000a780: 6574 6120 3d20 310a 2020 2020 2020 2020  eta = 1.        
+0000a790: 696d 706c 6965 7320 6120 756e 6966 6f72  implies a unifor
+0000a7a0: 6d20 6469 7374 7269 6275 7469 6f6e 206f  m distribution o
+0000a7b0: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
+0000a7c0: 6e20 6d61 7472 6963 6573 3b0a 2020 2020  n matrices;.    
+0000a7d0: 2020 2020 6c61 7267 6572 2076 616c 7565      larger value
+0000a7e0: 7320 7075 7420 6d6f 7265 2077 6569 6768  s put more weigh
+0000a7f0: 7420 6f6e 206d 6174 7269 6365 7320 7769  t on matrices wi
+0000a800: 7468 2066 6577 2063 6f72 7265 6c61 7469  th few correlati
+0000a810: 6f6e 732e 0a20 2020 206e 203a 2074 656e  ons..    n : ten
+0000a820: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
+0000a830: 2020 2020 2020 2020 4469 6d65 6e73 696f          Dimensio
+0000a840: 6e20 6f66 2074 6865 2063 6f76 6172 6961  n of the covaria
+0000a850: 6e63 6520 6d61 7472 6978 2028 6e20 3e20  nce matrix (n > 
+0000a860: 3129 2e0a 2020 2020 7364 5f64 6973 7420  1)..    sd_dist 
+0000a870: 3a20 4469 7374 7269 6275 7469 6f6e 0a20  : Distribution. 
+0000a880: 2020 2020 2020 2041 2070 6f73 6974 6976         A positiv
+0000a890: 6520 7363 616c 6172 206f 7220 7665 6374  e scalar or vect
+0000a8a0: 6f72 2064 6973 7472 6962 7574 696f 6e20  or distribution 
+0000a8b0: 666f 7220 7468 6520 7374 616e 6461 7264  for the standard
+0000a8c0: 2064 6576 6961 7469 6f6e 732c 2063 7265   deviations, cre
+0000a8d0: 6174 6564 0a20 2020 2020 2020 2077 6974  ated.        wit
+0000a8e0: 6820 7468 6520 602e 6469 7374 2829 6020  h the `.dist()` 
+0000a8f0: 4150 492e 2053 686f 756c 6420 6861 7665  API. Should have
+0000a900: 2060 7368 6170 655b 2d31 5d3d 6e60 2e20   `shape[-1]=n`. 
+0000a910: 5363 616c 6172 2064 6973 7472 6962 7574  Scalar distribut
+0000a920: 696f 6e73 2077 696c 6c20 6265 0a20 2020  ions will be.   
+0000a930: 2020 2020 2061 7574 6f6d 6174 6963 616c       automatical
+0000a940: 6c79 2072 6573 697a 6564 2074 6f20 656e  ly resized to en
+0000a950: 7375 7265 2074 6869 732e 0a0a 2020 2020  sure this...    
+0000a960: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
+0000a970: 2073 645f 6469 7374 2077 696c 6c20 6265   sd_dist will be
+0000a980: 2063 6c6f 6e65 642c 2072 656e 6465 7269   cloned, renderi
+0000a990: 6e67 2069 7420 696e 6465 7065 6e64 656e  ng it independen
+0000a9a0: 7420 6f66 2074 6865 206f 6e65 2070 6173  t of the one pas
+0000a9b0: 7365 6420 6173 2069 6e70 7574 2e0a 0a20  sed as input... 
+0000a9c0: 2020 2063 6f6d 7075 7465 5f63 6f72 7220     compute_corr 
+0000a9d0: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
+0000a9e0: 5472 7565 0a20 2020 2020 2020 2049 6620  True.        If 
+0000a9f0: 6054 7275 6560 2c20 7265 7475 726e 7320  `True`, returns 
+0000aa00: 7468 7265 6520 7661 6c75 6573 3a20 7468  three values: th
+0000aa10: 6520 4368 6f6c 6573 6b79 2064 6563 6f6d  e Cholesky decom
+0000aa20: 706f 7369 7469 6f6e 2c20 7468 6520 636f  position, the co
+0000aa30: 7272 656c 6174 696f 6e73 0a20 2020 2020  rrelations.     
+0000aa40: 2020 2061 6e64 2074 6865 2073 7461 6e64     and the stand
+0000aa50: 6172 6420 6465 7669 6174 696f 6e73 206f  ard deviations o
+0000aa60: 6620 7468 6520 636f 7661 7269 616e 6365  f the covariance
+0000aa70: 206d 6174 7269 782e 204f 7468 6572 7769   matrix. Otherwi
+0000aa80: 7365 2c20 6f6e 6c79 2072 6574 7572 6e73  se, only returns
+0000aa90: 0a20 2020 2020 2020 2074 6865 2070 6163  .        the pac
+0000aaa0: 6b65 6420 4368 6f6c 6573 6b79 2064 6563  ked Cholesky dec
+0000aab0: 6f6d 706f 7369 7469 6f6e 2e20 4465 6661  omposition. Defa
+0000aac0: 756c 7473 2074 6f20 6054 7275 6560 2e0a  ults to `True`..
+0000aad0: 2020 2020 2020 2020 636f 6d70 6174 6962          compatib
+0000aae0: 696c 6974 792e 0a20 2020 2073 746f 7265  ility..    store
+0000aaf0: 5f69 6e5f 7472 6163 6520 3a20 626f 6f6c  _in_trace : bool
+0000ab00: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
+0000ab10: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+0000ab20: 6f20 7374 6f72 6520 7468 6520 636f 7272  o store the corr
+0000ab30: 656c 6174 696f 6e73 2061 6e64 2073 7461  elations and sta
+0000ab40: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
+0000ab50: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
+0000ab60: 6365 0a20 2020 2020 2020 206d 6174 7269  ce.        matri
+0000ab70: 7820 696e 2074 6865 2070 6f73 7465 7269  x in the posteri
+0000ab80: 6f72 2074 7261 6365 2e20 4966 2060 5472  or trace. If `Tr
+0000ab90: 7565 602c 2074 6865 7920 7769 6c6c 2061  ue`, they will a
+0000aba0: 7574 6f6d 6174 6963 616c 6c79 2062 6520  utomatically be 
+0000abb0: 6e61 6d65 6420 6173 0a20 2020 2020 2020  named as.       
+0000abc0: 2060 7b6e 616d 657d 5f63 6f72 7260 2061   `{name}_corr` a
+0000abd0: 6e64 2060 7b6e 616d 657d 5f73 7464 7360  nd `{name}_stds`
+0000abe0: 2072 6573 7065 6374 6976 656c 792e 2045   respectively. E
+0000abf0: 6666 6563 7469 7665 206f 6e6c 7920 7768  ffective only wh
+0000ac00: 656e 0a20 2020 2020 2020 2060 636f 6d70  en.        `comp
+0000ac10: 7574 655f 636f 7272 3d54 7275 6560 2e0a  ute_corr=True`..
+0000ac20: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0000ac30: 202d 2d2d 2d2d 2d2d 0a20 2020 2063 686f   -------.    cho
+0000ac40: 6c20 3a20 2054 656e 736f 7256 6172 6961  l :  TensorVaria
+0000ac50: 626c 650a 2020 2020 2020 2020 4966 2060  ble.        If `
+0000ac60: 636f 6d70 7574 655f 636f 7272 3d54 7275  compute_corr=Tru
+0000ac70: 6560 2e20 5468 6520 756e 7061 636b 6564  e`. The unpacked
+0000ac80: 2043 686f 6c65 736b 7920 636f 7661 7269   Cholesky covari
+0000ac90: 616e 6365 2064 6563 6f6d 706f 7369 7469  ance decompositi
+0000aca0: 6f6e 2e0a 2020 2020 636f 7272 203a 2054  on..    corr : T
+0000acb0: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
+0000acc0: 2020 2020 2020 4966 2060 636f 6d70 7574        If `comput
+0000acd0: 655f 636f 7272 3d54 7275 6560 2e20 5468  e_corr=True`. Th
+0000ace0: 6520 636f 7272 656c 6174 696f 6e73 206f  e correlations o
+0000acf0: 6620 7468 6520 636f 7661 7269 616e 6365  f the covariance
+0000ad00: 206d 6174 7269 782e 0a20 2020 2073 7464   matrix..    std
+0000ad10: 7320 3a20 5465 6e73 6f72 5661 7269 6162  s : TensorVariab
+0000ad20: 6c65 0a20 2020 2020 2020 2049 6620 6063  le.        If `c
+0000ad30: 6f6d 7075 7465 5f63 6f72 723d 5472 7565  ompute_corr=True
+0000ad40: 602e 2054 6865 2073 7461 6e64 6172 6420  `. The standard 
+0000ad50: 6465 7669 6174 696f 6e73 206f 6620 7468  deviations of th
+0000ad60: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
+0000ad70: 7269 782e 0a20 2020 2070 6163 6b65 645f  rix..    packed_
+0000ad80: 6368 6f6c 203a 2054 656e 736f 7256 6172  chol : TensorVar
+0000ad90: 6961 626c 650a 2020 2020 2020 2020 4966  iable.        If
+0000ada0: 2060 636f 6d70 7574 655f 636f 7272 3d46   `compute_corr=F
+0000adb0: 616c 7365 6020 5468 6520 7061 636b 6564  alse` The packed
+0000adc0: 2043 686f 6c65 736b 7920 636f 7661 7269   Cholesky covari
+0000add0: 616e 6365 2064 6563 6f6d 706f 7369 7469  ance decompositi
+0000ade0: 6f6e 2e0a 0a20 2020 204e 6f74 6573 0a20  on...    Notes. 
+0000adf0: 2020 202d 2d2d 2d2d 0a20 2020 2053 696e     -----.    Sin
+0000ae00: 6365 2074 6865 2043 686f 6c65 736b 7920  ce the Cholesky 
+0000ae10: 6661 6374 6f72 2069 7320 6120 6c6f 7765  factor is a lowe
+0000ae20: 7220 7472 6961 6e67 756c 6172 206d 6174  r triangular mat
+0000ae30: 7269 782c 2077 6520 7573 6520 7061 636b  rix, we use pack
+0000ae40: 6564 2073 746f 7261 6765 2066 6f72 0a20  ed storage for. 
+0000ae50: 2020 2074 6865 206d 6174 7269 783a 2057     the matrix: W
+0000ae60: 6520 7374 6f72 6520 7468 6520 7661 6c75  e store the valu
+0000ae70: 6573 206f 6620 7468 6520 6c6f 7765 7220  es of the lower 
+0000ae80: 7472 6961 6e67 756c 6172 206d 6174 7269  triangular matri
+0000ae90: 7820 696e 2061 206f 6e65 2d64 696d 656e  x in a one-dimen
+0000aea0: 7369 6f6e 616c 0a20 2020 2061 7272 6179  sional.    array
+0000aeb0: 2c20 6e75 6d62 6572 6564 2062 7920 726f  , numbered by ro
+0000aec0: 773a 3a0a 0a20 2020 2020 2020 205b 5b30  w::..        [[0
+0000aed0: 202d 202d 202d 5d0a 2020 2020 2020 2020   - - -].        
+0000aee0: 205b 3120 3220 2d20 2d5d 0a20 2020 2020   [1 2 - -].     
+0000aef0: 2020 2020 5b33 2034 2035 202d 5d0a 2020      [3 4 5 -].  
+0000af00: 2020 2020 2020 205b 3620 3720 3820 395d         [6 7 8 9]
+0000af10: 5d0a 0a20 2020 2054 6865 2075 6e70 6163  ]..    The unpac
+0000af20: 6b65 6420 4368 6f6c 6573 6b79 2063 6f76  ked Cholesky cov
+0000af30: 6172 6961 6e63 6520 6d61 7472 6978 2069  ariance matrix i
+0000af40: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
+0000af50: 636f 6d70 7574 6564 2061 6e64 2072 6574  computed and ret
+0000af60: 7572 6e65 6420 7768 656e 0a20 2020 2079  urned when.    y
+0000af70: 6f75 2073 7065 6369 6679 2060 636f 6d70  ou specify `comp
+0000af80: 7574 655f 636f 7272 3d54 7275 6560 2069  ute_corr=True` i
+0000af90: 6e20 6070 6d2e 4c4b 4a43 686f 6c65 736b  n `pm.LKJCholesk
+0000afa0: 7943 6f76 6020 2873 6565 2065 7861 6d70  yCov` (see examp
+0000afb0: 6c65 2062 656c 6f77 292e 0a20 2020 204f  le below)..    O
+0000afc0: 7468 6572 7769 7365 2c20 796f 7520 6361  therwise, you ca
+0000afd0: 6e20 7573 6520 6070 6d2e 6578 7061 6e64  n use `pm.expand
+0000afe0: 5f70 6163 6b65 645f 7472 6961 6e67 756c  _packed_triangul
+0000aff0: 6172 2870 6163 6b65 645f 636f 762c 206c  ar(packed_cov, l
+0000b000: 6f77 6572 3d54 7275 6529 600a 2020 2020  ower=True)`.    
+0000b010: 746f 2063 6f6e 7665 7274 2074 6865 2070  to convert the p
+0000b020: 6163 6b65 6420 4368 6f6c 6573 6b79 206d  acked Cholesky m
+0000b030: 6174 7269 7820 746f 2061 2072 6567 756c  atrix to a regul
+0000b040: 6172 2074 776f 2d64 696d 656e 7369 6f6e  ar two-dimension
+0000b050: 616c 2061 7272 6179 2e0a 0a20 2020 2045  al array...    E
+0000b060: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+0000b070: 2d2d 2d2d 0a20 2020 202e 2e20 636f 6465  ----.    .. code
+0000b080: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0000b090: 2020 2077 6974 6820 706d 2e4d 6f64 656c     with pm.Model
+0000b0a0: 2829 2061 7320 6d6f 6465 6c3a 0a20 2020  () as model:.   
+0000b0b0: 2020 2020 2020 2020 2023 204e 6f74 6520           # Note 
+0000b0c0: 7468 6174 2077 6520 6163 6365 7373 2074  that we access t
+0000b0d0: 6865 2064 6973 7472 6962 7574 696f 6e20  he distribution 
+0000b0e0: 666f 7220 7468 6520 7374 616e 6461 7264  for the standard
+0000b0f0: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+0000b100: 6576 6961 7469 6f6e 732c 2061 6e64 2064  eviations, and d
+0000b110: 6f20 6e6f 7420 6372 6561 7465 2061 206e  o not create a n
+0000b120: 6577 2072 616e 646f 6d20 7661 7269 6162  ew random variab
+0000b130: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+0000b140: 7364 5f64 6973 7420 3d20 706d 2e45 7870  sd_dist = pm.Exp
+0000b150: 6f6e 656e 7469 616c 2e64 6973 7428 312e  onential.dist(1.
+0000b160: 302c 2073 697a 653d 3130 290a 2020 2020  0, size=10).    
+0000b170: 2020 2020 2020 2020 6368 6f6c 2c20 636f          chol, co
+0000b180: 7272 2c20 7369 676d 6173 203d 2070 6d2e  rr, sigmas = pm.
+0000b190: 4c4b 4a43 686f 6c65 736b 7943 6f76 280a  LKJCholeskyCov(.
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2763 686f 6c5f 636f 7627 2c20 6574 613d  'chol_cov', eta=
+0000b1c0: 342c 206e 3d31 302c 2073 645f 6469 7374  4, n=10, sd_dist
+0000b1d0: 3d73 645f 6469 7374 0a20 2020 2020 2020  =sd_dist.       
+0000b1e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b1f0: 2020 2020 2320 6966 2079 6f75 206f 6e6c      # if you onl
+0000b200: 7920 7761 6e74 2074 6865 2070 6163 6b65  y want the packe
+0000b210: 6420 4368 6f6c 6573 6b79 3a0a 2020 2020  d Cholesky:.    
+0000b220: 2020 2020 2020 2020 2320 7061 636b 6564          # packed
+0000b230: 5f63 686f 6c20 3d20 706d 2e4c 4b4a 4368  _chol = pm.LKJCh
+0000b240: 6f6c 6573 6b79 436f 7628 0a20 2020 2020  oleskyCov(.     
+0000b250: 2020 2020 2020 2020 2020 2027 6368 6f6c             'chol
+0000b260: 5f63 6f76 272c 2065 7461 3d34 2c20 6e3d  _cov', eta=4, n=
+0000b270: 3130 2c20 7364 5f64 6973 743d 7364 5f64  10, sd_dist=sd_d
+0000b280: 6973 742c 2063 6f6d 7075 7465 5f63 6f72  ist, compute_cor
+0000b290: 723d 4661 6c73 650a 2020 2020 2020 2020  r=False.        
+0000b2a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000b2b0: 2020 2320 6368 6f6c 203d 2070 6d2e 6578    # chol = pm.ex
+0000b2c0: 7061 6e64 5f70 6163 6b65 645f 7472 6961  pand_packed_tria
+0000b2d0: 6e67 756c 6172 2831 302c 2070 6163 6b65  ngular(10, packe
+0000b2e0: 645f 6368 6f6c 2c20 6c6f 7765 723d 5472  d_chol, lower=Tr
+0000b2f0: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
+0000b300: 2023 2044 6566 696e 6520 6120 6e65 7720   # Define a new 
+0000b310: 4d76 4e6f 726d 616c 2077 6974 6820 7468  MvNormal with th
+0000b320: 6520 6769 7665 6e20 636f 7661 7269 616e  e given covarian
+0000b330: 6365 0a20 2020 2020 2020 2020 2020 2076  ce.            v
+0000b340: 616c 7320 3d20 706d 2e4d 764e 6f72 6d61  als = pm.MvNorma
+0000b350: 6c28 2776 616c 7327 2c20 6d75 3d6e 702e  l('vals', mu=np.
+0000b360: 7a65 726f 7328 3130 292c 2063 686f 6c3d  zeros(10), chol=
+0000b370: 6368 6f6c 2c20 7368 6170 653d 3130 290a  chol, shape=10).
+0000b380: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
+0000b390: 7220 7472 616e 7366 6f72 6d20 616e 2075  r transform an u
+0000b3a0: 6e63 6f72 7265 6c61 7465 6420 6e6f 726d  ncorrelated norm
+0000b3b0: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
+0000b3c0: 7661 6c73 5f72 6177 203d 2070 6d2e 4e6f  vals_raw = pm.No
+0000b3d0: 726d 616c 2827 7661 6c73 5f72 6177 272c  rmal('vals_raw',
+0000b3e0: 206d 753d 302c 2073 6967 6d61 3d31 2c20   mu=0, sigma=1, 
+0000b3f0: 7368 6170 653d 3130 290a 2020 2020 2020  shape=10).      
+0000b400: 2020 2020 2020 7661 6c73 203d 2070 742e        vals = pt.
+0000b410: 646f 7428 6368 6f6c 2c20 7661 6c73 5f72  dot(chol, vals_r
+0000b420: 6177 290a 0a20 2020 2020 2020 2020 2020  aw)..           
+0000b430: 2023 204f 7220 636f 6d70 7574 6520 7468   # Or compute th
+0000b440: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
+0000b450: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
+0000b460: 636f 7620 3d20 7074 2e64 6f74 2863 686f  cov = pt.dot(cho
+0000b470: 6c2c 2063 686f 6c2e 5429 0a0a 2020 2020  l, chol.T)..    
+0000b480: 2a2a 496d 706c 656d 656e 7461 7469 6f6e  **Implementation
+0000b490: 2a2a 2049 6e20 7468 6520 756e 636f 6e73  ** In the uncons
+0000b4a0: 7472 6169 6e65 6420 7370 6163 6520 616c  trained space al
+0000b4b0: 6c20 7661 6c75 6573 206f 6620 7468 6520  l values of the 
+0000b4c0: 6368 6f6c 6573 6b79 2066 6163 746f 720a  cholesky factor.
+0000b4d0: 2020 2020 6172 6520 7374 6f72 6564 2075      are stored u
+0000b4e0: 6e74 7261 6e73 666f 726d 6564 2c20 6578  ntransformed, ex
+0000b4f0: 6365 7074 2066 6f72 2074 6865 2064 6961  cept for the dia
+0000b500: 676f 6e61 6c20 656e 7472 6965 732c 2077  gonal entries, w
+0000b510: 6865 7265 0a20 2020 2077 6520 7573 6520  here.    we use 
+0000b520: 6120 6c6f 672d 7472 616e 7366 6f72 6d20  a log-transform 
+0000b530: 746f 2072 6573 7472 6963 7420 7468 656d  to restrict them
+0000b540: 2074 6f20 706f 7369 7469 7665 2076 616c   to positive val
+0000b550: 7565 732e 0a0a 2020 2020 546f 2063 6f72  ues...    To cor
+0000b560: 7265 6374 6c79 2063 6f6d 7075 7465 206c  rectly compute l
+0000b570: 6f67 2d6c 696b 656c 6968 6f6f 6473 2066  og-likelihoods f
+0000b580: 6f72 2074 6865 2073 7461 6e64 6172 6420  or the standard 
+0000b590: 6465 7669 6174 696f 6e73 0a20 2020 2061  deviations.    a
+0000b5a0: 6e64 2074 6865 2063 6f72 7265 6c61 7469  nd the correlati
+0000b5b0: 6f6e 206d 6174 7269 7820 7365 7061 7261  on matrix separa
+0000b5c0: 7465 6c79 2c20 7765 206e 6565 6420 746f  tely, we need to
+0000b5d0: 2063 6f6e 7369 6465 7220 610a 2020 2020   consider a.    
+0000b5e0: 7365 636f 6e64 2074 7261 6e73 666f 726d  second transform
+0000b5f0: 6174 696f 6e3a 2047 6976 656e 2061 2063  ation: Given a c
+0000b600: 686f 6c65 736b 7920 6661 6374 6f72 697a  holesky factoriz
+0000b610: 6174 696f 6e0a 2020 2020 3a6d 6174 683a  ation.    :math:
+0000b620: 604c 4c5e 5420 3d20 5c53 6967 6d61 6020  `LL^T = \Sigma` 
+0000b630: 6f66 2061 2063 6f76 6172 6961 6e63 6520  of a covariance 
+0000b640: 6d61 7472 6978 2077 6520 6361 6e20 7265  matrix we can re
+0000b650: 636f 7665 7220 7468 650a 2020 2020 7374  cover the.    st
+0000b660: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+0000b670: 7320 3a6d 6174 683a 605c 7369 676d 6160  s :math:`\sigma`
+0000b680: 2061 7320 7468 6520 6575 636c 6964 6561   as the euclidea
+0000b690: 6e20 6c65 6e67 7468 7320 6f66 0a20 2020  n lengths of.   
+0000b6a0: 2074 6865 2072 6f77 7320 6f66 203a 6d61   the rows of :ma
+0000b6b0: 7468 3a60 4c60 2c20 616e 6420 7468 6520  th:`L`, and the 
+0000b6c0: 6368 6f6c 6573 6b79 2066 6163 746f 7220  cholesky factor 
+0000b6d0: 6f66 2074 6865 0a20 2020 2063 6f72 7265  of the.    corre
+0000b6e0: 6c61 7469 6f6e 206d 6174 7269 7820 6173  lation matrix as
+0000b6f0: 203a 6d61 7468 3a60 5520 3d20 5c74 6578   :math:`U = \tex
+0000b700: 747b 6469 6167 7d28 5c73 6967 6d61 295e  t{diag}(\sigma)^
+0000b710: 7b2d 317d 4c60 2e0a 2020 2020 5369 6e63  {-1}L`..    Sinc
+0000b720: 6520 6561 6368 2072 6f77 206f 6620 3a6d  e each row of :m
+0000b730: 6174 683a 6055 6020 6861 7320 6c65 6e67  ath:`U` has leng
+0000b740: 7468 2031 2c20 7765 2064 6f20 6e6f 7420  th 1, we do not 
+0000b750: 6e65 6564 2074 6f0a 2020 2020 7374 6f72  need to.    stor
+0000b760: 6520 7468 6520 6469 6167 6f6e 616c 2e20  e the diagonal. 
+0000b770: 5765 2064 6566 696e 6520 6120 7472 616e  We define a tran
+0000b780: 7366 6f72 6d61 7469 6f6e 203a 6d61 7468  sformation :math
+0000b790: 3a60 5c70 6869 600a 2020 2020 7375 6368  :`\phi`.    such
+0000b7a0: 2074 6861 7420 3a6d 6174 683a 605c 7068   that :math:`\ph
+0000b7b0: 6928 4c29 6020 6973 2074 6865 206c 6f77  i(L)` is the low
+0000b7c0: 6572 2074 7269 616e 6775 6c61 7220 6d61  er triangular ma
+0000b7d0: 7472 6978 2063 6f6e 7461 696e 696e 670a  trix containing.
+0000b7e0: 2020 2020 7468 6520 7374 616e 6461 7264      the standard
+0000b7f0: 2064 6576 6961 7469 6f6e 7320 3a6d 6174   deviations :mat
+0000b800: 683a 605c 7369 676d 6160 206f 6e20 7468  h:`\sigma` on th
+0000b810: 6520 6469 6167 6f6e 616c 2061 6e64 2074  e diagonal and t
+0000b820: 6865 0a20 2020 2063 6f72 7265 6c61 7469  he.    correlati
+0000b830: 6f6e 206d 6174 7269 7820 3a6d 6174 683a  on matrix :math:
+0000b840: 6055 6020 6265 6c6f 772e 2049 6e20 7468  `U` below. In th
+0000b850: 6973 2066 6f72 6d20 7765 2063 616e 2065  is form we can e
+0000b860: 6173 696c 790a 2020 2020 636f 6d70 7574  asily.    comput
+0000b870: 6520 7468 6520 6469 6666 6572 656e 7420  e the different 
+0000b880: 6c69 6b65 6c69 686f 6f64 7320 7365 7061  likelihoods sepa
+0000b890: 7261 7465 6c79 2c20 6173 2074 6865 206c  rately, as the l
+0000b8a0: 696b 656c 6968 6f6f 640a 2020 2020 6f66  ikelihood.    of
+0000b8b0: 2074 6865 2063 6f72 7265 6c61 7469 6f6e   the correlation
+0000b8c0: 206d 6174 7269 7820 6f6e 6c79 2064 6570   matrix only dep
+0000b8d0: 656e 6473 206f 6e20 7468 6520 7661 6c75  ends on the valu
+0000b8e0: 6573 2062 656c 6f77 2074 6865 0a20 2020  es below the.   
+0000b8f0: 2064 6961 676f 6e61 6c2c 2061 6e64 2074   diagonal, and t
+0000b900: 6865 206c 696b 656c 6968 6f6f 6420 6f66  he likelihood of
+0000b910: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
+0000b920: 7669 6174 696f 6e20 6465 7065 6e64 730a  viation depends.
+0000b930: 2020 2020 6f6e 6c79 206f 6e20 7468 6520      only on the 
+0000b940: 6469 6167 6f6e 616c 2076 616c 7565 732e  diagonal values.
+0000b950: 0a0a 2020 2020 5765 2073 7469 6c6c 206e  ..    We still n
+0000b960: 6565 6420 7468 6520 6465 7465 726d 696e  eed the determin
+0000b970: 616e 7420 6f66 2074 6865 206a 6163 6f62  ant of the jacob
+0000b980: 6961 6e20 6f66 203a 6d61 7468 3a60 5c70  ian of :math:`\p
+0000b990: 6869 5e7b 2d31 7d60 2e0a 2020 2020 4966  hi^{-1}`..    If
+0000b9a0: 2077 6520 7468 696e 6b20 6f66 203a 6d61   we think of :ma
+0000b9b0: 7468 3a60 5c70 6869 6020 6173 2061 6e20  th:`\phi` as an 
+0000b9c0: 6175 746f 6d6f 7270 6869 736d 206f 6e0a  automorphism on.
+0000b9d0: 2020 2020 3a6d 6174 683a 605c 6d61 7468      :math:`\math
+0000b9e0: 6262 7b52 7d5e 7b5c 7466 7261 637b 6e28  bb{R}^{\tfrac{n(
+0000b9f0: 6e2b 3129 7d7b 327d 7d60 2c20 7768 6572  n+1)}{2}}`, wher
+0000ba00: 6520 7765 206f 7264 6572 0a20 2020 2074  e we order.    t
+0000ba10: 6865 2064 696d 656e 7369 6f6e 7320 6173  he dimensions as
+0000ba20: 2064 6573 6372 6962 6564 2069 6e20 7468   described in th
+0000ba30: 6520 6e6f 7465 7320 6162 6f76 652c 2074  e notes above, t
+0000ba40: 6865 206a 6163 6f62 6961 6e0a 2020 2020  he jacobian.    
+0000ba50: 6973 2061 2062 6c6f 636b 2d64 6961 676f  is a block-diago
+0000ba60: 6e61 6c20 6d61 7472 6978 2c20 7768 6572  nal matrix, wher
+0000ba70: 6520 6561 6368 2062 6c6f 636b 2063 6f72  e each block cor
+0000ba80: 7265 7370 6f6e 6473 2074 6f0a 2020 2020  responds to.    
+0000ba90: 6f6e 6520 726f 7720 6f66 203a 6d61 7468  one row of :math
+0000baa0: 3a60 5560 2e20 4561 6368 2062 6c6f 636b  :`U`. Each block
+0000bab0: 2068 6173 2061 7272 6f77 6865 6164 2073   has arrowhead s
+0000bac0: 6861 7065 2c20 616e 6420 7765 0a20 2020  hape, and we.   
+0000bad0: 2063 616e 2063 6f6d 7075 7465 2074 6865   can compute the
+0000bae0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
+0000baf0: 7468 6174 2061 7320 6465 7363 7269 6265  that as describe
+0000bb00: 6420 696e 205b 325d 2e20 5369 6e63 650a  d in [2]. Since.
+0000bb10: 2020 2020 7468 6520 6465 7465 726d 696e      the determin
+0000bb20: 616e 7420 6f66 2061 2062 6c6f 636b 2d64  ant of a block-d
+0000bb30: 6961 676f 6e61 6c20 6d61 7472 6978 2069  iagonal matrix i
+0000bb40: 7320 7468 6520 7072 6f64 7563 740a 2020  s the product.  
+0000bb50: 2020 6f66 2074 6865 2064 6574 6572 6d69    of the determi
+0000bb60: 6e61 6e74 7320 6f66 2074 6865 2062 6c6f  nants of the blo
+0000bb70: 636b 732c 2077 6520 6765 740a 0a20 2020  cks, we get..   
+0000bb80: 202e 2e20 6d61 7468 3a3a 0a0a 2020 2020   .. math::..    
+0000bb90: 2020 205c 7465 7874 7b64 6574 7d28 4a5f     \text{det}(J_
+0000bba0: 7b5c 7068 695e 7b2d 317d 7d28 5529 2920  {\phi^{-1}}(U)) 
+0000bbb0: 3d0a 2020 2020 2020 205c 6c65 6674 5b0a  =.       \left[.
+0000bbc0: 2020 2020 2020 2020 205c 7072 6f64 5f7b           \prod_{
+0000bbd0: 693d 327d 5e4e 2075 5f7b 6969 7d5e 7b69  i=2}^N u_{ii}^{i
+0000bbe0: 202d 2031 7d20 4c5f 7b69 697d 0a20 2020   - 1} L_{ii}.   
+0000bbf0: 2020 2020 5c72 6967 6874 5d5e 7b2d 317d      \right]^{-1}
+0000bc00: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
+0000bc10: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0000bc20: 2020 2020 2e2e 205b 315d 204c 6577 616e      .. [1] Lewan
+0000bc30: 646f 7773 6b69 2c20 442e 2c20 4b75 726f  dowski, D., Kuro
+0000bc40: 7769 636b 612c 2044 2e20 616e 6420 4a6f  wicka, D. and Jo
+0000bc50: 652c 2048 2e20 2832 3030 3929 2e0a 2020  e, H. (2009)..  
+0000bc60: 2020 2020 2022 4765 6e65 7261 7469 6e67       "Generating
+0000bc70: 2072 616e 646f 6d20 636f 7272 656c 6174   random correlat
+0000bc80: 696f 6e20 6d61 7472 6963 6573 2062 6173  ion matrices bas
+0000bc90: 6564 206f 6e20 7669 6e65 7320 616e 640a  ed on vines and.
+0000bca0: 2020 2020 2020 2065 7874 656e 6465 6420         extended 
+0000bcb0: 6f6e 696f 6e20 6d65 7468 6f64 2e22 204a  onion method." J
+0000bcc0: 6f75 726e 616c 206f 6620 6d75 6c74 6976  ournal of multiv
+0000bcd0: 6172 6961 7465 2061 6e61 6c79 7369 732c  ariate analysis,
+0000bce0: 0a20 2020 2020 2020 3130 3028 3929 2c20  .       100(9), 
+0000bcf0: 7070 2e31 3938 392d 3230 3031 2e0a 0a20  pp.1989-2001... 
+0000bd00: 2020 202e 2e20 5b32 5d20 4a2e 204d 2e20     .. [2] J. M. 
+0000bd10: 6973 6e27 7420 6120 6d61 7468 656d 6174  isn't a mathemat
+0000bd20: 6963 6961 6e20 2868 7474 703a 2f2f 6d61  ician (http://ma
+0000bd30: 7468 2e73 7461 636b 6578 6368 616e 6765  th.stackexchange
+0000bd40: 2e63 6f6d 2f75 7365 7273 2f34 3938 2f0a  .com/users/498/.
+0000bd50: 2020 2020 2020 206a 2d6d 2d69 736e 742d         j-m-isnt-
+0000bd60: 612d 6d61 7468 656d 6174 6963 6961 6e29  a-mathematician)
+0000bd70: 2c20 4469 6666 6572 656e 7420 6170 7072  , Different appr
+0000bd80: 6f61 6368 6573 2074 6f20 6576 616c 7561  oaches to evalua
+0000bd90: 7465 2074 6869 730a 2020 2020 2020 2064  te this.       d
+0000bda0: 6574 6572 6d69 6e61 6e74 2c20 5552 4c20  eterminant, URL 
+0000bdb0: 2876 6572 7369 6f6e 3a20 3230 3132 2d30  (version: 2012-0
+0000bdc0: 342d 3134 293a 0a20 2020 2020 2020 6874  4-14):.       ht
+0000bdd0: 7470 3a2f 2f6d 6174 682e 7374 6163 6b65  tp://math.stacke
+0000bde0: 7863 6861 6e67 652e 636f 6d2f 712f 3133  xchange.com/q/13
+0000bdf0: 3030 3236 0a20 2020 2022 2222 0a0a 2020  0026.    """..  
+0000be00: 2020 6465 6620 5f5f 6e65 775f 5f28 636c    def __new__(cl
+0000be10: 732c 206e 616d 652c 2065 7461 2c20 6e2c  s, name, eta, n,
+0000be20: 2073 645f 6469 7374 2c20 2a2c 2063 6f6d   sd_dist, *, com
+0000be30: 7075 7465 5f63 6f72 723d 5472 7565 2c20  pute_corr=True, 
+0000be40: 7374 6f72 655f 696e 5f74 7261 6365 3d54  store_in_trace=T
+0000be50: 7275 652c 202a 2a6b 7761 7267 7329 3a0a  rue, **kwargs):.
+0000be60: 2020 2020 2020 2020 7061 636b 6564 5f63          packed_c
+0000be70: 686f 6c20 3d20 5f4c 4b4a 4368 6f6c 6573  hol = _LKJCholes
+0000be80: 6b79 436f 7628 6e61 6d65 2c20 6574 613d  kyCov(name, eta=
+0000be90: 6574 612c 206e 3d6e 2c20 7364 5f64 6973  eta, n=n, sd_dis
+0000bea0: 743d 7364 5f64 6973 742c 202a 2a6b 7761  t=sd_dist, **kwa
+0000beb0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
+0000bec0: 6e6f 7420 636f 6d70 7574 655f 636f 7272  not compute_corr
+0000bed0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000bee0: 7475 726e 2070 6163 6b65 645f 6368 6f6c  turn packed_chol
+0000bef0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000bf00: 2020 2020 2020 2020 2020 2063 686f 6c2c             chol,
+0000bf10: 2063 6f72 722c 2073 7464 7320 3d20 636c   corr, stds = cl
+0000bf20: 732e 6865 6c70 6572 5f64 6574 6572 6d69  s.helper_determi
+0000bf30: 6e69 7374 6963 7328 6e2c 2070 6163 6b65  nistics(n, packe
+0000bf40: 645f 6368 6f6c 290a 2020 2020 2020 2020  d_chol).        
+0000bf50: 2020 2020 6966 2073 746f 7265 5f69 6e5f      if store_in_
+0000bf60: 7472 6163 653a 0a20 2020 2020 2020 2020  trace:.         
+0000bf70: 2020 2020 2020 2063 6f72 7220 3d20 706d         corr = pm
+0000bf80: 2e44 6574 6572 6d69 6e69 7374 6963 2866  .Deterministic(f
+0000bf90: 227b 6e61 6d65 7d5f 636f 7272 222c 2063  "{name}_corr", c
+0000bfa0: 6f72 7229 0a20 2020 2020 2020 2020 2020  orr).           
+0000bfb0: 2020 2020 2073 7464 7320 3d20 706d 2e44       stds = pm.D
+0000bfc0: 6574 6572 6d69 6e69 7374 6963 2866 227b  eterministic(f"{
+0000bfd0: 6e61 6d65 7d5f 7374 6473 222c 2073 7464  name}_stds", std
+0000bfe0: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
+0000bff0: 6574 7572 6e20 6368 6f6c 2c20 636f 7272  eturn chol, corr
+0000c000: 2c20 7374 6473 0a0a 2020 2020 4063 6c61  , stds..    @cla
+0000c010: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+0000c020: 2064 6973 7428 636c 732c 2065 7461 2c20   dist(cls, eta, 
+0000c030: 6e2c 2073 645f 6469 7374 2c20 2a2c 2063  n, sd_dist, *, c
+0000c040: 6f6d 7075 7465 5f63 6f72 723d 5472 7565  ompute_corr=True
+0000c050: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+0000c060: 2020 2020 2023 2063 6f6d 7075 7465 2043       # compute C
+0000c070: 686f 6c65 736b 7920 6465 636f 6d70 6f73  holesky decompos
+0000c080: 6974 696f 6e0a 2020 2020 2020 2020 7061  ition.        pa
+0000c090: 636b 6564 5f63 686f 6c20 3d20 5f4c 4b4a  cked_chol = _LKJ
+0000c0a0: 4368 6f6c 6573 6b79 436f 762e 6469 7374  CholeskyCov.dist
+0000c0b0: 2865 7461 3d65 7461 2c20 6e3d 6e2c 2073  (eta=eta, n=n, s
+0000c0c0: 645f 6469 7374 3d73 645f 6469 7374 2c20  d_dist=sd_dist, 
+0000c0d0: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
+0000c0e0: 2020 6966 206e 6f74 2063 6f6d 7075 7465    if not compute
+0000c0f0: 5f63 6f72 723a 0a20 2020 2020 2020 2020  _corr:.         
+0000c100: 2020 2072 6574 7572 6e20 7061 636b 6564     return packed
+0000c110: 5f63 686f 6c0a 2020 2020 2020 2020 656c  _chol.        el
+0000c120: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c130: 7265 7475 726e 2063 6c73 2e68 656c 7065  return cls.helpe
+0000c140: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
+0000c150: 286e 2c20 7061 636b 6564 5f63 686f 6c29  (n, packed_chol)
+0000c160: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+0000c170: 6f64 0a20 2020 2064 6566 2068 656c 7065  od.    def helpe
+0000c180: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
+0000c190: 2863 6c73 2c20 6e2c 2070 6163 6b65 645f  (cls, n, packed_
+0000c1a0: 6368 6f6c 293a 0a20 2020 2020 2020 2063  chol):.        c
+0000c1b0: 686f 6c20 3d20 706d 2e65 7870 616e 645f  hol = pm.expand_
+0000c1c0: 7061 636b 6564 5f74 7269 616e 6775 6c61  packed_triangula
+0000c1d0: 7228 6e2c 2070 6163 6b65 645f 6368 6f6c  r(n, packed_chol
+0000c1e0: 2c20 6c6f 7765 723d 5472 7565 290a 2020  , lower=True).  
+0000c1f0: 2020 2020 2020 2320 636f 6d70 7574 6520        # compute 
+0000c200: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000c210: 780a 2020 2020 2020 2020 636f 7620 3d20  x.        cov = 
+0000c220: 7074 2e64 6f74 2863 686f 6c2c 2063 686f  pt.dot(chol, cho
+0000c230: 6c2e 5429 0a20 2020 2020 2020 2023 2065  l.T).        # e
+0000c240: 7874 7261 6374 2073 7461 6e64 6172 6420  xtract standard 
+0000c250: 6465 7669 6174 696f 6e73 2061 6e64 2072  deviations and r
+0000c260: 686f 0a20 2020 2020 2020 2073 7464 7320  ho.        stds 
+0000c270: 3d20 7074 2e73 7172 7428 7074 2e64 6961  = pt.sqrt(pt.dia
+0000c280: 6728 636f 7629 290a 2020 2020 2020 2020  g(cov)).        
+0000c290: 696e 765f 7374 6473 203d 2031 202f 2073  inv_stds = 1 / s
+0000c2a0: 7464 730a 2020 2020 2020 2020 636f 7272  tds.        corr
+0000c2b0: 203d 2069 6e76 5f73 7464 735b 4e6f 6e65   = inv_stds[None
+0000c2c0: 2c20 3a5d 202a 2063 6f76 202a 2069 6e76  , :] * cov * inv
+0000c2d0: 5f73 7464 735b 3a2c 204e 6f6e 655d 0a20  _stds[:, None]. 
+0000c2e0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+0000c2f0: 6f6c 2c20 636f 7272 2c20 7374 6473 0a0a  ol, corr, stds..
+0000c300: 0a63 6c61 7373 204c 4b4a 436f 7272 5256  .class LKJCorrRV
+0000c310: 2852 616e 646f 6d56 6172 6961 626c 6529  (RandomVariable)
+0000c320: 3a0a 2020 2020 6e61 6d65 203d 2022 6c6b  :.    name = "lk
+0000c330: 6a63 6f72 7222 0a20 2020 206e 6469 6d5f  jcorr".    ndim_
+0000c340: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
+0000c350: 6d73 5f70 6172 616d 7320 3d20 5b30 2c20  ms_params = [0, 
+0000c360: 305d 0a20 2020 2064 7479 7065 203d 2022  0].    dtype = "
+0000c370: 666c 6f61 7458 220a 2020 2020 5f70 7269  floatX".    _pri
+0000c380: 6e74 5f6e 616d 6520 3d20 2822 4c4b 4a43  nt_name = ("LKJC
+0000c390: 6f72 7252 5622 2c20 225c 5c6f 7065 7261  orrRV", "\\opera
+0000c3a0: 746f 726e 616d 657b 4c4b 4a43 6f72 7252  torname{LKJCorrR
+0000c3b0: 567d 2229 0a0a 2020 2020 6465 6620 6d61  V}")..    def ma
+0000c3c0: 6b65 5f6e 6f64 6528 7365 6c66 2c20 726e  ke_node(self, rn
+0000c3d0: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
+0000c3e0: 6e2c 2065 7461 293a 0a20 2020 2020 2020  n, eta):.       
+0000c3f0: 206e 203d 2070 742e 6173 5f74 656e 736f   n = pt.as_tenso
+0000c400: 725f 7661 7269 6162 6c65 286e 290a 2020  r_variable(n).  
+0000c410: 2020 2020 2020 6966 206e 6f74 206e 2e6e        if not n.n
+0000c420: 6469 6d20 3d3d 2030 3a0a 2020 2020 2020  dim == 0:.      
+0000c430: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000c440: 6545 7272 6f72 2822 6e20 6d75 7374 2062  eError("n must b
+0000c450: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
+0000c460: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
+0000c470: 6574 6120 3d20 7074 2e61 735f 7465 6e73  eta = pt.as_tens
+0000c480: 6f72 5f76 6172 6961 626c 6528 6574 6129  or_variable(eta)
+0000c490: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c4a0: 6574 612e 6e64 696d 203d 3d20 303a 0a20  eta.ndim == 0:. 
+0000c4b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000c4c0: 2056 616c 7565 4572 726f 7228 2265 7461   ValueError("eta
+0000c4d0: 206d 7573 7420 6265 2061 2073 6361 6c61   must be a scala
+0000c4e0: 7220 286e 6469 6d3d 3029 2e22 290a 0a20  r (ndim=0).").. 
+0000c4f0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+0000c500: 7065 7228 292e 6d61 6b65 5f6e 6f64 6528  per().make_node(
+0000c510: 726e 672c 2073 697a 652c 2064 7479 7065  rng, size, dtype
+0000c520: 2c20 6e2c 2065 7461 290a 0a20 2020 2064  , n, eta)..    d
+0000c530: 6566 205f 7375 7070 5f73 6861 7065 5f66  ef _supp_shape_f
+0000c540: 726f 6d5f 7061 7261 6d73 2873 656c 662c  rom_params(self,
+0000c550: 2064 6973 745f 7061 7261 6d73 2c20 2a2a   dist_params, **
+0000c560: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+0000c570: 206e 203d 2064 6973 745f 7061 7261 6d73   n = dist_params
+0000c580: 5b30 5d0a 2020 2020 2020 2020 6469 7374  [0].        dist
+0000c590: 5f73 6861 7065 203d 2028 286e 202a 2028  _shape = ((n * (
+0000c5a0: 6e20 2d20 3129 2920 2f2f 2032 2c29 0a20  n - 1)) // 2,). 
+0000c5b0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
+0000c5c0: 7374 5f73 6861 7065 0a0a 2020 2020 4063  st_shape..    @c
+0000c5d0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+0000c5e0: 6566 2072 6e67 5f66 6e28 636c 732c 2072  ef rng_fn(cls, r
+0000c5f0: 6e67 2c20 6e2c 2065 7461 2c20 7369 7a65  ng, n, eta, size
+0000c600: 293a 0a20 2020 2020 2020 2023 2057 6520  ):.        # We 
+0000c610: 666c 6174 7465 6e20 7468 6520 7369 7a65  flatten the size
+0000c620: 2074 6f20 6d61 6b65 206f 7065 7261 7469   to make operati
+0000c630: 6f6e 7320 6561 7369 6572 2c20 616e 6420  ons easier, and 
+0000c640: 7468 656e 2072 6562 7569 6c64 2069 740a  then rebuild it.
+0000c650: 2020 2020 2020 2020 6966 2073 697a 6520          if size 
+0000c660: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000c670: 2020 2020 2066 6c61 745f 7369 7a65 203d       flat_size =
+0000c680: 2031 0a20 2020 2020 2020 2065 6c73 653a   1.        else:
+0000c690: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
+0000c6a0: 745f 7369 7a65 203d 206e 702e 7072 6f64  t_size = np.prod
+0000c6b0: 2873 697a 6529 0a0a 2020 2020 2020 2020  (size)..        
+0000c6c0: 4320 3d20 636c 732e 5f72 616e 646f 6d5f  C = cls._random_
+0000c6d0: 636f 7272 5f6d 6174 7269 7828 726e 673d  corr_matrix(rng=
+0000c6e0: 726e 672c 206e 3d6e 2c20 6574 613d 6574  rng, n=n, eta=et
+0000c6f0: 612c 2066 6c61 745f 7369 7a65 3d66 6c61  a, flat_size=fla
+0000c700: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+0000c710: 2074 7269 755f 6964 7820 3d20 6e70 2e74   triu_idx = np.t
+0000c720: 7269 755f 696e 6469 6365 7328 6e2c 206b  riu_indices(n, k
+0000c730: 3d31 290a 2020 2020 2020 2020 7361 6d70  =1).        samp
+0000c740: 6c65 7320 3d20 435b 2e2e 2e2c 2074 7269  les = C[..., tri
+0000c750: 755f 6964 785b 305d 2c20 7472 6975 5f69  u_idx[0], triu_i
+0000c760: 6478 5b31 5d5d 0a0a 2020 2020 2020 2020  dx[1]]..        
+0000c770: 6966 2073 697a 6520 6973 204e 6f6e 653a  if size is None:
+0000c780: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
+0000c790: 706c 6573 203d 2073 616d 706c 6573 5b30  ples = samples[0
+0000c7a0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+0000c7b0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+0000c7c0: 5f73 6861 7065 203d 2028 6e20 2a20 286e  _shape = (n * (n
+0000c7d0: 202d 2031 2929 202f 2f20 320a 2020 2020   - 1)) // 2.    
+0000c7e0: 2020 2020 2020 2020 7361 6d70 6c65 7320          samples 
+0000c7f0: 3d20 6e70 2e72 6573 6861 7065 2873 616d  = np.reshape(sam
+0000c800: 706c 6573 2c20 282a 7369 7a65 2c20 6469  ples, (*size, di
+0000c810: 7374 5f73 6861 7065 2929 0a20 2020 2020  st_shape)).     
+0000c820: 2020 2072 6574 7572 6e20 7361 6d70 6c65     return sample
+0000c830: 730a 0a20 2020 2040 636c 6173 736d 6574  s..    @classmet
+0000c840: 686f 640a 2020 2020 6465 6620 5f72 616e  hod.    def _ran
+0000c850: 646f 6d5f 636f 7272 5f6d 6174 7269 7828  dom_corr_matrix(
+0000c860: 636c 732c 2072 6e67 2c20 6e2c 2065 7461  cls, rng, n, eta
+0000c870: 2c20 666c 6174 5f73 697a 6529 3a0a 2020  , flat_size):.  
+0000c880: 2020 2020 2020 2320 6f72 6967 696e 616c        # original
+0000c890: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+0000c8a0: 696e 2052 2073 6565 3a0a 2020 2020 2020  in R see:.      
+0000c8b0: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
+0000c8c0: 7562 2e63 6f6d 2f72 6d63 656c 7265 6174  ub.com/rmcelreat
+0000c8d0: 682f 7265 7468 696e 6b69 6e67 2f62 6c6f  h/rethinking/blo
+0000c8e0: 622f 6d61 7374 6572 2f52 2f64 6973 7472  b/master/R/distr
+0000c8f0: 6962 7574 696f 6e73 2e72 0a20 2020 2020  ibutions.r.     
+0000c900: 2020 2062 6574 6120 3d20 6574 6120 2d20     beta = eta - 
+0000c910: 312e 3020 2b20 6e20 2f20 322e 300a 2020  1.0 + n / 2.0.  
+0000c920: 2020 2020 2020 7231 3220 3d20 322e 3020        r12 = 2.0 
+0000c930: 2a20 7374 6174 732e 6265 7461 2e72 7673  * stats.beta.rvs
+0000c940: 2861 3d62 6574 612c 2062 3d62 6574 612c  (a=beta, b=beta,
+0000c950: 2073 697a 653d 666c 6174 5f73 697a 652c   size=flat_size,
+0000c960: 2072 616e 646f 6d5f 7374 6174 653d 726e   random_state=rn
+0000c970: 6729 202d 2031 2e30 0a20 2020 2020 2020  g) - 1.0.       
+0000c980: 2050 203d 206e 702e 6675 6c6c 2828 666c   P = np.full((fl
+0000c990: 6174 5f73 697a 652c 206e 2c20 6e29 2c20  at_size, n, n), 
+0000c9a0: 6e70 2e65 7965 286e 2929 0a20 2020 2020  np.eye(n)).     
+0000c9b0: 2020 2050 5b2e 2e2e 2c20 302c 2031 5d20     P[..., 0, 1] 
+0000c9c0: 3d20 7231 320a 2020 2020 2020 2020 505b  = r12.        P[
+0000c9d0: 2e2e 2e2c 2031 2c20 315d 203d 206e 702e  ..., 1, 1] = np.
+0000c9e0: 7371 7274 2831 2e30 202d 2072 3132 2a2a  sqrt(1.0 - r12**
+0000c9f0: 3229 0a20 2020 2020 2020 2066 6f72 206d  2).        for m
+0000ca00: 7031 2069 6e20 7261 6e67 6528 322c 206e  p1 in range(2, n
+0000ca10: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
+0000ca20: 6574 6120 2d3d 2030 2e35 0a20 2020 2020  eta -= 0.5.     
+0000ca30: 2020 2020 2020 2079 203d 2073 7461 7473         y = stats
+0000ca40: 2e62 6574 612e 7276 7328 613d 6d70 3120  .beta.rvs(a=mp1 
+0000ca50: 2f20 322e 302c 2062 3d62 6574 612c 2073  / 2.0, b=beta, s
+0000ca60: 697a 653d 666c 6174 5f73 697a 652c 2072  ize=flat_size, r
+0000ca70: 616e 646f 6d5f 7374 6174 653d 726e 6729  andom_state=rng)
+0000ca80: 0a20 2020 2020 2020 2020 2020 207a 203d  .            z =
+0000ca90: 2073 7461 7473 2e6e 6f72 6d2e 7276 7328   stats.norm.rvs(
+0000caa0: 6c6f 633d 302c 2073 6361 6c65 3d31 2c20  loc=0, scale=1, 
+0000cab0: 7369 7a65 3d28 666c 6174 5f73 697a 652c  size=(flat_size,
+0000cac0: 206d 7031 292c 2072 616e 646f 6d5f 7374   mp1), random_st
+0000cad0: 6174 653d 726e 6729 0a20 2020 2020 2020  ate=rng).       
+0000cae0: 2020 2020 207a 203d 207a 202f 206e 702e       z = z / np.
+0000caf0: 7371 7274 286e 702e 6569 6e73 756d 2822  sqrt(np.einsum("
+0000cb00: 696a 2c69 6a2d 3e69 222c 207a 2c20 7a29  ij,ij->i", z, z)
+0000cb10: 295b 2e2e 2e2c 206e 702e 6e65 7761 7869  )[..., np.newaxi
+0000cb20: 735d 0a20 2020 2020 2020 2020 2020 2050  s].            P
+0000cb30: 5b2e 2e2e 2c20 303a 6d70 312c 206d 7031  [..., 0:mp1, mp1
+0000cb40: 5d20 3d20 6e70 2e73 7172 7428 795b 2e2e  ] = np.sqrt(y[..
+0000cb50: 2e2c 206e 702e 6e65 7761 7869 735d 2920  ., np.newaxis]) 
+0000cb60: 2a20 7a0a 2020 2020 2020 2020 2020 2020  * z.            
+0000cb70: 505b 2e2e 2e2c 206d 7031 2c20 6d70 315d  P[..., mp1, mp1]
+0000cb80: 203d 206e 702e 7371 7274 2831 2e30 202d   = np.sqrt(1.0 -
+0000cb90: 2079 290a 2020 2020 2020 2020 4320 3d20   y).        C = 
+0000cba0: 6e70 2e65 696e 7375 6d28 222e 2e2e 6a69  np.einsum("...ji
+0000cbb0: 2c2e 2e2e 6a6b 2d3e 2e2e 2e69 6b22 2c20  ,...jk->...ik", 
+0000cbc0: 502c 2050 290a 2020 2020 2020 2020 7265  P, P).        re
+0000cbd0: 7475 726e 2043 0a0a 0a6c 6b6a 636f 7272  turn C...lkjcorr
+0000cbe0: 203d 204c 4b4a 436f 7272 5256 2829 0a0a   = LKJCorrRV()..
+0000cbf0: 0a63 6c61 7373 204c 4b4a 436f 7272 2842  .class LKJCorr(B
+0000cc00: 6f75 6e64 6564 436f 6e74 696e 756f 7573  oundedContinuous
+0000cc10: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+0000cc20: 5468 6520 4c4b 4a20 284c 6577 616e 646f  The LKJ (Lewando
+0000cc30: 7773 6b69 2c20 4b75 726f 7769 636b 6120  wski, Kurowicka 
+0000cc40: 616e 6420 4a6f 6529 206c 6f67 2d6c 696b  and Joe) log-lik
+0000cc50: 656c 6968 6f6f 642e 0a0a 2020 2020 5468  elihood...    Th
+0000cc60: 6520 4c4b 4a20 6469 7374 7269 6275 7469  e LKJ distributi
+0000cc70: 6f6e 2069 7320 6120 7072 696f 7220 6469  on is a prior di
+0000cc80: 7374 7269 6275 7469 6f6e 2066 6f72 2063  stribution for c
+0000cc90: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+0000cca0: 6365 732e 0a20 2020 2049 6620 6574 6120  ces..    If eta 
+0000ccb0: 3d20 3120 7468 6973 2063 6f72 7265 7370  = 1 this corresp
+0000ccc0: 6f6e 6473 2074 6f20 7468 6520 756e 6966  onds to the unif
+0000ccd0: 6f72 6d20 6469 7374 7269 6275 7469 6f6e  orm distribution
+0000cce0: 206f 7665 7220 636f 7272 656c 6174 696f   over correlatio
+0000ccf0: 6e0a 2020 2020 6d61 7472 6963 6573 2e20  n.    matrices. 
+0000cd00: 466f 7220 6574 6120 2d3e 206f 6f20 7468  For eta -> oo th
+0000cd10: 6520 4c4b 4a20 7072 696f 7220 6170 7072  e LKJ prior appr
+0000cd20: 6f61 6368 6573 2074 6865 2069 6465 6e74  oaches the ident
+0000cd30: 6974 7920 6d61 7472 6978 2e0a 0a20 2020  ity matrix...   
+0000cd40: 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d   ========  =====
 0000cd50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000cd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
-0000cd80: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000cd90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000cda0: 6e20 3a20 7465 6e73 6f72 5f6c 696b 6520  n : tensor_like 
-0000cdb0: 6f66 2069 6e74 0a20 2020 2020 2020 2044  of int.        D
-0000cdc0: 696d 656e 7369 6f6e 206f 6620 7468 6520  imension of the 
-0000cdd0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000cde0: 7820 286e 203e 2031 292e 0a20 2020 2065  x (n > 1)..    e
-0000cdf0: 7461 203a 2074 656e 736f 725f 6c69 6b65  ta : tensor_like
-0000ce00: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
-0000ce10: 2020 5468 6520 7368 6170 6520 7061 7261    The shape para
-0000ce20: 6d65 7465 7220 2865 7461 203e 2030 2920  meter (eta > 0) 
-0000ce30: 6f66 2074 6865 204c 4b4a 2064 6973 7472  of the LKJ distr
-0000ce40: 6962 7574 696f 6e2e 2065 7461 203d 2031  ibution. eta = 1
-0000ce50: 0a20 2020 2020 2020 2069 6d70 6c69 6573  .        implies
-0000ce60: 2061 2075 6e69 666f 726d 2064 6973 7472   a uniform distr
-0000ce70: 6962 7574 696f 6e20 6f66 2074 6865 2063  ibution of the c
-0000ce80: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
-0000ce90: 6365 733b 0a20 2020 2020 2020 206c 6172  ces;.        lar
-0000cea0: 6765 7220 7661 6c75 6573 2070 7574 206d  ger values put m
-0000ceb0: 6f72 6520 7765 6967 6874 206f 6e20 6d61  ore weight on ma
-0000cec0: 7472 6963 6573 2077 6974 6820 6665 7720  trices with few 
-0000ced0: 636f 7272 656c 6174 696f 6e73 2e0a 0a20  correlations... 
-0000cee0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-0000cef0: 2d2d 0a20 2020 2054 6869 7320 696d 706c  --.    This impl
-0000cf00: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
-0000cf10: 7265 7475 726e 7320 7468 6520 7661 6c75  returns the valu
-0000cf20: 6573 206f 6620 7468 6520 7570 7065 7220  es of the upper 
-0000cf30: 7472 6961 6e67 756c 6172 0a20 2020 206d  triangular.    m
-0000cf40: 6174 7269 7820 6578 636c 7564 696e 6720  atrix excluding 
-0000cf50: 7468 6520 6469 6167 6f6e 616c 2e20 4865  the diagonal. He
-0000cf60: 7265 2069 7320 6120 7363 6865 6d61 7469  re is a schemati
-0000cf70: 6320 666f 7220 6e20 3d20 352c 2073 686f  c for n = 5, sho
-0000cf80: 7769 6e67 0a20 2020 2074 6865 2069 6e64  wing.    the ind
-0000cf90: 6578 6573 206f 6620 7468 6520 656c 656d  exes of the elem
-0000cfa0: 656e 7473 3a3a 0a0a 2020 2020 2020 2020  ents::..        
-0000cfb0: 5b5b 2d20 3020 3120 3220 335d 0a20 2020  [[- 0 1 2 3].   
-0000cfc0: 2020 2020 2020 5b2d 202d 2034 2035 2036        [- - 4 5 6
-0000cfd0: 5d0a 2020 2020 2020 2020 205b 2d20 2d20  ].         [- - 
-0000cfe0: 2d20 3720 385d 0a20 2020 2020 2020 2020  - 7 8].         
-0000cff0: 5b2d 202d 202d 202d 2039 5d0a 2020 2020  [- - - - 9].    
-0000d000: 2020 2020 205b 2d20 2d20 2d20 2d20 2d5d       [- - - - -]
-0000d010: 5d0a 0a0a 2020 2020 5265 6665 7265 6e63  ]...    Referenc
-0000d020: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
-0000d030: 2d0a 2020 2020 2e2e 205b 4c4b 4a32 3030  -.    .. [LKJ200
-0000d040: 395d 204c 6577 616e 646f 7773 6b69 2c20  9] Lewandowski, 
-0000d050: 442e 2c20 4b75 726f 7769 636b 612c 2044  D., Kurowicka, D
-0000d060: 2e20 616e 6420 4a6f 652c 2048 2e20 2832  . and Joe, H. (2
-0000d070: 3030 3929 2e0a 2020 2020 2020 2020 2247  009)..        "G
-0000d080: 656e 6572 6174 696e 6720 7261 6e64 6f6d  enerating random
-0000d090: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
-0000d0a0: 7269 6365 7320 6261 7365 6420 6f6e 2076  rices based on v
-0000d0b0: 696e 6573 2061 6e64 0a20 2020 2020 2020  ines and.       
-0000d0c0: 2065 7874 656e 6465 6420 6f6e 696f 6e20   extended onion 
-0000d0d0: 6d65 7468 6f64 2e22 204a 6f75 726e 616c  method." Journal
-0000d0e0: 206f 6620 6d75 6c74 6976 6172 6961 7465   of multivariate
-0000d0f0: 2061 6e61 6c79 7369 732c 0a20 2020 2020   analysis,.     
-0000d100: 2020 2031 3030 2839 292c 2070 702e 3139     100(9), pp.19
-0000d110: 3839 2d32 3030 312e 0a20 2020 2022 2222  89-2001..    """
-0000d120: 0a0a 2020 2020 7276 5f6f 7020 3d20 6c6b  ..    rv_op = lk
-0000d130: 6a63 6f72 720a 0a20 2020 2040 636c 6173  jcorr..    @clas
-0000d140: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-0000d150: 6469 7374 2863 6c73 2c20 6e2c 2065 7461  dist(cls, n, eta
-0000d160: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-0000d170: 2020 2020 206e 203d 2070 742e 6173 5f74       n = pt.as_t
-0000d180: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
-0000d190: 6e74 5828 6e29 290a 2020 2020 2020 2020  ntX(n)).        
-0000d1a0: 6574 6120 3d20 7074 2e61 735f 7465 6e73  eta = pt.as_tens
-0000d1b0: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
-0000d1c0: 7458 2865 7461 2929 0a20 2020 2020 2020  tX(eta)).       
-0000d1d0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-0000d1e0: 6469 7374 285b 6e2c 2065 7461 5d2c 202a  dist([n, eta], *
-0000d1f0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-0000d200: 6620 6d6f 6d65 6e74 2872 762c 202a 6172  f moment(rv, *ar
-0000d210: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
-0000d220: 7572 6e20 7074 2e7a 6572 6f73 5f6c 696b  urn pt.zeros_lik
-0000d230: 6528 7276 290a 0a20 2020 2064 6566 206c  e(rv)..    def l
-0000d240: 6f67 7028 7661 6c75 652c 206e 2c20 6574  ogp(value, n, et
-0000d250: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
-0000d260: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-0000d270: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
-0000d280: 7920 6f66 204c 4b4a 2064 6973 7472 6962  y of LKJ distrib
-0000d290: 7574 696f 6e20 6174 2073 7065 6369 6669  ution at specifi
-0000d2a0: 6564 0a20 2020 2020 2020 2076 616c 7565  ed.        value
-0000d2b0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000d2c0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0000d2d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000d2e0: 2076 616c 7565 3a20 6e75 6d65 7269 630a   value: numeric.
-0000d2f0: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-0000d300: 6520 666f 7220 7768 6963 6820 6c6f 672d  e for which log-
-0000d310: 7072 6f62 6162 696c 6974 7920 6973 2063  probability is c
-0000d320: 616c 6375 6c61 7465 642e 0a0a 2020 2020  alculated...    
-0000d330: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000d340: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000d350: 2020 2020 5465 6e73 6f72 5661 7269 6162      TensorVariab
-0000d360: 6c65 0a20 2020 2020 2020 2022 2222 0a0a  le.        """..
-0000d370: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-0000d380: 5079 5465 6e73 6f72 2064 6f65 7320 6e6f  PyTensor does no
-0000d390: 7420 6861 7665 2061 2060 7472 6975 5f69  t have a `triu_i
-0000d3a0: 6e64 6963 6573 602c 2073 6f20 7765 2063  ndices`, so we c
-0000d3b0: 616e 206f 6e6c 7920 776f 726b 2077 6974  an only work wit
-0000d3c0: 6820 636f 6e73 7461 6e74 0a20 2020 2020  h constant.     
-0000d3d0: 2020 2023 2020 6e20 286f 7220 656c 7365     #  n (or else
-0000d3e0: 2066 696e 6420 6120 6469 6666 6572 656e   find a differen
-0000d3f0: 7420 6578 7072 6573 7369 6f6e 290a 2020  t expression).  
-0000d400: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000d410: 6e73 7461 6e63 6528 6e2c 2043 6f6e 7374  nstance(n, Const
-0000d420: 616e 7429 3a0a 2020 2020 2020 2020 2020  ant):.          
-0000d430: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000d440: 6d65 6e74 6564 4572 726f 7228 226c 6f67  mentedError("log
-0000d450: 7020 6f6e 6c79 2069 6d70 6c65 6d65 6e74  p only implement
-0000d460: 6564 2066 6f72 2063 6f6e 7374 616e 7420  ed for constant 
-0000d470: 606e 6022 290a 0a20 2020 2020 2020 206e  `n`")..        n
-0000d480: 203d 2069 6e74 286e 2e64 6174 6129 0a20   = int(n.data). 
-0000d490: 2020 2020 2020 2073 6861 7065 203d 206e         shape = n
-0000d4a0: 202a 2028 6e20 2d20 3129 202f 2f20 320a   * (n - 1) // 2.
-0000d4b0: 2020 2020 2020 2020 7472 695f 696e 6465          tri_inde
-0000d4c0: 7820 3d20 6e70 2e7a 6572 6f73 2828 6e2c  x = np.zeros((n,
-0000d4d0: 206e 292c 2064 7479 7065 3d22 696e 7433   n), dtype="int3
-0000d4e0: 3222 290a 2020 2020 2020 2020 7472 695f  2").        tri_
-0000d4f0: 696e 6465 785b 6e70 2e74 7269 755f 696e  index[np.triu_in
-0000d500: 6469 6365 7328 6e2c 206b 3d31 295d 203d  dices(n, k=1)] =
-0000d510: 206e 702e 6172 616e 6765 2873 6861 7065   np.arange(shape
-0000d520: 290a 2020 2020 2020 2020 7472 695f 696e  ).        tri_in
-0000d530: 6465 785b 6e70 2e74 7269 755f 696e 6469  dex[np.triu_indi
-0000d540: 6365 7328 6e2c 206b 3d31 295b 3a3a 2d31  ces(n, k=1)[::-1
-0000d550: 5d5d 203d 206e 702e 6172 616e 6765 2873  ]] = np.arange(s
-0000d560: 6861 7065 290a 0a20 2020 2020 2020 2076  hape)..        v
-0000d570: 616c 7565 203d 2070 742e 7461 6b65 2876  alue = pt.take(v
-0000d580: 616c 7565 2c20 7472 695f 696e 6465 7829  alue, tri_index)
-0000d590: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
-0000d5a0: 2070 742e 6669 6c6c 5f64 6961 676f 6e61   pt.fill_diagona
-0000d5b0: 6c28 7661 6c75 652c 2031 290a 0a20 2020  l(value, 1)..   
-0000d5c0: 2020 2020 2023 2054 4f44 4f3a 205f 6c6b       # TODO: _lk
-0000d5d0: 6a5f 6e6f 726d 616c 697a 696e 675f 636f  j_normalizing_co
-0000d5e0: 6e73 7461 6e74 2063 7572 7265 6e74 6c79  nstant currently
-0000d5f0: 2072 6571 7569 7265 7320 6065 7461 6020   requires `eta` 
-0000d600: 616e 6420 606e 6020 746f 2062 6520 636f  and `n` to be co
-0000d610: 6e73 7461 6e74 730a 2020 2020 2020 2020  nstants.        
-0000d620: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-0000d630: 6528 6574 612c 2043 6f6e 7374 616e 7429  e(eta, Constant)
-0000d640: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000d650: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-0000d660: 6564 4572 726f 7228 226c 6f67 7020 6f6e  edError("logp on
-0000d670: 6c79 2069 6d70 6c65 6d65 6e74 6564 2066  ly implemented f
-0000d680: 6f72 2063 6f6e 7374 616e 7420 6065 7461  or constant `eta
-0000d690: 6022 290a 2020 2020 2020 2020 6574 6120  `").        eta 
-0000d6a0: 3d20 666c 6f61 7428 6574 612e 6461 7461  = float(eta.data
-0000d6b0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-0000d6c0: 203d 205f 6c6b 6a5f 6e6f 726d 616c 697a   = _lkj_normaliz
-0000d6d0: 696e 675f 636f 6e73 7461 6e74 2865 7461  ing_constant(eta
-0000d6e0: 2c20 6e29 0a20 2020 2020 2020 2072 6573  , n).        res
-0000d6f0: 756c 7420 2b3d 2028 6574 6120 2d20 312e  ult += (eta - 1.
-0000d700: 3029 202a 2070 742e 6c6f 6728 6465 7428  0) * pt.log(det(
-0000d710: 7661 6c75 6529 290a 2020 2020 2020 2020  value)).        
-0000d720: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
-0000d730: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
-0000d740: 2020 2020 2072 6573 756c 742c 0a20 2020       result,.   
-0000d750: 2020 2020 2020 2020 2076 616c 7565 203e           value >
-0000d760: 3d20 2d31 2c0a 2020 2020 2020 2020 2020  = -1,.          
-0000d770: 2020 7661 6c75 6520 3c3d 2031 2c0a 2020    value <= 1,.  
-0000d780: 2020 2020 2020 2020 2020 6d61 7472 6978            matrix
-0000d790: 5f70 6f73 5f64 6566 2876 616c 7565 292c  _pos_def(value),
-0000d7a0: 0a20 2020 2020 2020 2020 2020 2065 7461  .            eta
-0000d7b0: 203e 2030 2c0a 2020 2020 2020 2020 290a   > 0,.        ).
-0000d7c0: 0a0a 405f 6465 6661 756c 745f 7472 616e  ..@_default_tran
-0000d7d0: 7366 6f72 6d2e 7265 6769 7374 6572 284c  sform.register(L
-0000d7e0: 4b4a 436f 7272 290a 6465 6620 6c6b 6a63  KJCorr).def lkjc
-0000d7f0: 6f72 725f 6465 6661 756c 745f 7472 616e  orr_default_tran
-0000d800: 7366 6f72 6d28 6f70 2c20 7276 293a 0a20  sform(op, rv):. 
-0000d810: 2020 2072 6574 7572 6e20 496e 7465 7276     return Interv
-0000d820: 616c 2866 6c6f 6174 5828 2d31 2e30 292c  al(floatX(-1.0),
-0000d830: 2066 6c6f 6174 5828 312e 3029 290a 0a0a   floatX(1.0))...
-0000d840: 636c 6173 7320 4d61 7472 6978 4e6f 726d  class MatrixNorm
-0000d850: 616c 5256 2852 616e 646f 6d56 6172 6961  alRV(RandomVaria
-0000d860: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
-0000d870: 2022 6d61 7472 6978 6e6f 726d 616c 220a   "matrixnormal".
-0000d880: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
-0000d890: 320a 2020 2020 6e64 696d 735f 7061 7261  2.    ndims_para
-0000d8a0: 6d73 203d 205b 322c 2032 2c20 325d 0a20  ms = [2, 2, 2]. 
-0000d8b0: 2020 2064 7479 7065 203d 2022 666c 6f61     dtype = "floa
-0000d8c0: 7458 220a 2020 2020 5f70 7269 6e74 5f6e  tX".    _print_n
-0000d8d0: 616d 6520 3d20 2822 4d61 7472 6978 4e6f  ame = ("MatrixNo
-0000d8e0: 726d 616c 222c 2022 5c5c 6f70 6572 6174  rmal", "\\operat
-0000d8f0: 6f72 6e61 6d65 7b4d 6174 7269 784e 6f72  orname{MatrixNor
-0000d900: 6d61 6c7d 2229 0a0a 2020 2020 6465 6620  mal}")..    def 
-0000d910: 5f69 6e66 6572 5f73 6861 7065 2873 656c  _infer_shape(sel
-0000d920: 662c 2073 697a 652c 2064 6973 745f 7061  f, size, dist_pa
-0000d930: 7261 6d73 2c20 7061 7261 6d5f 7368 6170  rams, param_shap
-0000d940: 6573 3d4e 6f6e 6529 3a0a 2020 2020 2020  es=None):.      
-0000d950: 2020 7368 6170 6520 3d20 7475 706c 6528    shape = tuple(
-0000d960: 7369 7a65 2920 2b20 7475 706c 6528 6469  size) + tuple(di
-0000d970: 7374 5f70 6172 616d 735b 305d 2e73 6861  st_params[0].sha
-0000d980: 7065 5b2d 323a 5d29 0a20 2020 2020 2020  pe[-2:]).       
-0000d990: 2072 6574 7572 6e20 7368 6170 650a 0a20   return shape.. 
-0000d9a0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000d9b0: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
-0000d9c0: 6c73 2c20 726e 672c 206d 752c 2072 6f77  ls, rng, mu, row
-0000d9d0: 6368 6f6c 2c20 636f 6c63 686f 6c2c 2073  chol, colchol, s
-0000d9e0: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
-0000d9f0: 2020 2073 697a 6520 3d20 746f 5f74 7570     size = to_tup
-0000da00: 6c65 2873 697a 6529 0a20 2020 2020 2020  le(size).       
-0000da10: 2064 6973 745f 7368 6170 6520 3d20 746f   dist_shape = to
-0000da20: 5f74 7570 6c65 285b 726f 7763 686f 6c2e  _tuple([rowchol.
-0000da30: 7368 6170 655b 305d 2c20 636f 6c63 686f  shape[0], colcho
-0000da40: 6c2e 7368 6170 655b 305d 5d29 0a20 2020  l.shape[0]]).   
-0000da50: 2020 2020 206f 7574 7075 745f 7368 6170       output_shap
-0000da60: 6520 3d20 7369 7a65 202b 2064 6973 745f  e = size + dist_
-0000da70: 7368 6170 650a 0a20 2020 2020 2020 2023  shape..        #
-0000da80: 2042 726f 6164 6361 7374 696e 6720 616c   Broadcasting al
-0000da90: 6c20 7061 7261 6d65 7465 7273 0a20 2020  l parameters.   
-0000daa0: 2020 2020 2073 6861 7065 7320 3d20 5b6d       shapes = [m
-0000dab0: 752e 7368 6170 652c 206f 7574 7075 745f  u.shape, output_
-0000dac0: 7368 6170 655d 0a20 2020 2020 2020 2062  shape].        b
-0000dad0: 726f 6164 6361 7374 6162 6c65 5f73 6861  roadcastable_sha
-0000dae0: 7065 203d 2062 726f 6164 6361 7374 5f64  pe = broadcast_d
-0000daf0: 6973 745f 7361 6d70 6c65 735f 7368 6170  ist_samples_shap
-0000db00: 6528 7368 6170 6573 2c20 7369 7a65 3d73  e(shapes, size=s
-0000db10: 697a 6529 0a20 2020 2020 2020 206d 7520  ize).        mu 
-0000db20: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
-0000db30: 6f28 6d75 2c20 7368 6170 653d 6272 6f61  o(mu, shape=broa
-0000db40: 6463 6173 7461 626c 655f 7368 6170 6529  dcastable_shape)
-0000db50: 0a20 2020 2020 2020 2072 6f77 6368 6f6c  .        rowchol
-0000db60: 203d 206e 702e 6272 6f61 6463 6173 745f   = np.broadcast_
-0000db70: 746f 2872 6f77 6368 6f6c 2c20 7368 6170  to(rowchol, shap
-0000db80: 653d 7369 7a65 202b 2072 6f77 6368 6f6c  e=size + rowchol
-0000db90: 2e73 6861 7065 5b2d 323a 5d29 0a0a 2020  .shape[-2:])..  
-0000dba0: 2020 2020 2020 636f 6c63 686f 6c20 3d20        colchol = 
-0000dbb0: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
-0000dbc0: 636f 6c63 686f 6c2c 2073 6861 7065 3d73  colchol, shape=s
-0000dbd0: 697a 6520 2b20 636f 6c63 686f 6c2e 7368  ize + colchol.sh
-0000dbe0: 6170 655b 2d32 3a5d 290a 2020 2020 2020  ape[-2:]).      
-0000dbf0: 2020 636f 6c63 686f 6c20 3d20 6e70 2e73    colchol = np.s
-0000dc00: 7761 7061 7865 7328 636f 6c63 686f 6c2c  wapaxes(colchol,
-0000dc10: 202d 312c 202d 3229 2020 2320 5461 6b65   -1, -2)  # Take
-0000dc20: 2074 7261 6e73 706f 7365 0a0a 2020 2020   transpose..    
-0000dc30: 2020 2020 7374 616e 6461 7264 5f6e 6f72      standard_nor
-0000dc40: 6d61 6c20 3d20 726e 672e 7374 616e 6461  mal = rng.standa
-0000dc50: 7264 5f6e 6f72 6d61 6c28 6f75 7470 7574  rd_normal(output
-0000dc60: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
-0000dc70: 7361 6d70 6c65 7320 3d20 6d75 202b 206e  samples = mu + n
-0000dc80: 702e 6d61 746d 756c 2872 6f77 6368 6f6c  p.matmul(rowchol
-0000dc90: 2c20 6e70 2e6d 6174 6d75 6c28 7374 616e  , np.matmul(stan
-0000dca0: 6461 7264 5f6e 6f72 6d61 6c2c 2063 6f6c  dard_normal, col
-0000dcb0: 6368 6f6c 2929 0a0a 2020 2020 2020 2020  chol))..        
-0000dcc0: 7265 7475 726e 2073 616d 706c 6573 0a0a  return samples..
-0000dcd0: 0a6d 6174 7269 786e 6f72 6d61 6c20 3d20  .matrixnormal = 
-0000dce0: 4d61 7472 6978 4e6f 726d 616c 5256 2829  MatrixNormalRV()
-0000dcf0: 0a0a 0a63 6c61 7373 204d 6174 7269 784e  ...class MatrixN
-0000dd00: 6f72 6d61 6c28 436f 6e74 696e 756f 7573  ormal(Continuous
-0000dd10: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
-0000dd20: 4d61 7472 6978 2d76 616c 7565 6420 6e6f  Matrix-valued no
-0000dd30: 726d 616c 206c 6f67 2d6c 696b 656c 6968  rmal log-likelih
-0000dd40: 6f6f 642e 0a0a 2020 2020 2e2e 206d 6174  ood...    .. mat
-0000dd50: 683a 3a0a 2020 2020 2020 2066 2878 205c  h::.       f(x \
-0000dd60: 6d69 6420 5c6d 752c 2055 2c20 5629 203d  mid \mu, U, V) =
-0000dd70: 0a20 2020 2020 2020 2020 2020 5c66 7261  .           \fra
-0000dd80: 637b 317d 7b28 325c 7069 5e7b 6d20 6e7d  c{1}{(2\pi^{m n}
-0000dd90: 207c 557c 5e6e 207c 567c 5e6d 295e 7b31   |U|^n |V|^m)^{1
-0000dda0: 2f32 7d7d 0a20 2020 2020 2020 2020 2020  /2}}.           
-0000ddb0: 5c65 7870 5c6c 6566 745c 7b0a 2020 2020  \exp\left\{.    
-0000ddc0: 2020 2020 2020 2020 2020 2020 2d5c 6672              -\fr
-0000ddd0: 6163 7b31 7d7b 327d 205c 6d61 7468 726d  ac{1}{2} \mathrm
-0000dde0: 7b54 727d 5b20 565e 7b2d 317d 2028 782d  {Tr}[ V^{-1} (x-
-0000ddf0: 5c6d 7529 5e7b 5c70 7269 6d65 7d20 555e  \mu)^{\prime} U^
-0000de00: 7b2d 317d 2028 782d 5c6d 7529 5d0a 2020  {-1} (x-\mu)].  
-0000de10: 2020 2020 2020 2020 2020 5c72 6967 6874            \right
-0000de20: 5c7d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  \}..    ========
-0000de30: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
-0000de40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000de50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
-0000de60: 2020 2053 7570 706f 7274 2020 2020 2020     Support      
-0000de70: 2020 2020 3a6d 6174 683a 6078 205c 696e      :math:`x \in
-0000de80: 205c 6d61 7468 6262 7b52 7d5e 7b6d 205c   \mathbb{R}^{m \
-0000de90: 7469 6d65 7320 6e7d 600a 2020 2020 4d65  times n}`.    Me
-0000dea0: 616e 2020 2020 2020 2020 2020 2020 203a  an             :
-0000deb0: 6d61 7468 3a60 5c6d 7560 0a20 2020 2052  math:`\mu`.    R
-0000dec0: 6f77 2056 6172 6961 6e63 6520 2020 2020  ow Variance     
-0000ded0: 3a6d 6174 683a 6055 600a 2020 2020 436f  :math:`U`.    Co
-0000dee0: 6c75 6d6e 2056 6172 6961 6e63 6520 203a  lumn Variance  :
-0000def0: 6d61 7468 3a60 5660 0a20 2020 203d 3d3d  math:`V`.    ===
-0000df00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d  ============  ==
-0000df10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000df20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000df30: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
-0000df40: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0000df50: 2d2d 0a20 2020 206d 7520 3a20 7465 6e73  --.    mu : tens
-0000df60: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-0000df70: 0a20 2020 2020 2020 2041 7272 6179 206f  .        Array o
-0000df80: 6620 6d65 616e 732e 204d 7573 7420 6265  f means. Must be
-0000df90: 2062 726f 6164 6361 7374 6162 6c65 2077   broadcastable w
-0000dfa0: 6974 6820 7468 6520 7261 6e64 6f6d 2076  ith the random v
-0000dfb0: 6172 6961 626c 6520 5820 7375 6368 0a20  ariable X such. 
-0000dfc0: 2020 2020 2020 2074 6861 7420 7468 6520         that the 
-0000dfd0: 7368 6170 6520 6f66 206d 7520 2b20 5820  shape of mu + X 
-0000dfe0: 6973 2028 4d2c 204e 292e 0a20 2020 2072  is (M, N)..    r
-0000dff0: 6f77 636f 7620 3a20 284d 2c20 4d29 2074  owcov : (M, M) t
-0000e000: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-0000e010: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-0000e020: 2020 2020 2020 416d 6f6e 672d 726f 7720        Among-row 
-0000e030: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000e040: 782e 2044 6566 696e 6573 2076 6172 6961  x. Defines varia
-0000e050: 6e63 6520 7769 7468 696e 0a20 2020 2020  nce within.     
-0000e060: 2020 2063 6f6c 756d 6e73 2e20 4578 6163     columns. Exac
-0000e070: 746c 7920 6f6e 6520 6f66 2072 6f77 636f  tly one of rowco
-0000e080: 7620 6f72 2072 6f77 6368 6f6c 2069 7320  v or rowchol is 
-0000e090: 6e65 6564 6564 2e0a 2020 2020 726f 7763  needed..    rowc
-0000e0a0: 686f 6c20 3a20 284d 2c20 4d29 2074 656e  hol : (M, M) ten
-0000e0b0: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
-0000e0c0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-0000e0d0: 2020 2020 4368 6f6c 6573 6b79 2064 6563      Cholesky dec
-0000e0e0: 6f6d 706f 7369 7469 6f6e 206f 6620 616d  omposition of am
-0000e0f0: 6f6e 672d 726f 7720 636f 7661 7269 616e  ong-row covarian
-0000e100: 6365 206d 6174 7269 782e 2045 7861 6374  ce matrix. Exact
-0000e110: 6c79 206f 6e65 206f 660a 2020 2020 2020  ly one of.      
-0000e120: 2020 726f 7763 6f76 206f 7220 726f 7763    rowcov or rowc
-0000e130: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
-0000e140: 2020 2063 6f6c 636f 7620 3a20 284e 2c20     colcov : (N, 
-0000e150: 4e29 2074 656e 736f 725f 6c69 6b65 206f  N) tensor_like o
-0000e160: 6620 666c 6f61 742c 206f 7074 696f 6e61  f float, optiona
-0000e170: 6c0a 2020 2020 2020 2020 416d 6f6e 672d  l.        Among-
-0000e180: 636f 6c75 6d6e 2063 6f76 6172 6961 6e63  column covarianc
-0000e190: 6520 6d61 7472 6978 2e20 4966 2072 6f77  e matrix. If row
-0000e1a0: 636f 7620 6973 2074 6865 2069 6465 6e74  cov is the ident
-0000e1b0: 6974 7920 6d61 7472 6978 2c0a 2020 2020  ity matrix,.    
-0000e1c0: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-0000e1d0: 6e73 2061 7320 6063 6f76 6020 696e 204d  ns as `cov` in M
-0000e1e0: 764e 6f72 6d61 6c2e 0a20 2020 2020 2020  vNormal..       
-0000e1f0: 2045 7861 6374 6c79 206f 6e65 206f 6620   Exactly one of 
-0000e200: 636f 6c63 6f76 206f 7220 636f 6c63 686f  colcov or colcho
-0000e210: 6c20 6973 206e 6565 6465 642e 0a20 2020  l is needed..   
-0000e220: 2063 6f6c 6368 6f6c 203a 2028 4e2c 204e   colchol : (N, N
-0000e230: 2920 7465 6e73 6f72 5f6c 696b 6520 6f66  ) tensor_like of
-0000e240: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-0000e250: 0a20 2020 2020 2020 2043 686f 6c65 736b  .        Cholesk
-0000e260: 7920 6465 636f 6d70 6f73 6974 696f 6e20  y decomposition 
-0000e270: 6f66 2061 6d6f 6e67 2d63 6f6c 756d 6e20  of among-column 
-0000e280: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000e290: 782e 2045 7861 6374 6c79 206f 6e65 0a20  x. Exactly one. 
-0000e2a0: 2020 2020 2020 206f 6620 636f 6c63 6f76         of colcov
-0000e2b0: 206f 7220 636f 6c63 686f 6c20 6973 206e   or colchol is n
-0000e2c0: 6565 6465 642e 0a0a 2020 2020 4578 616d  eeded...    Exam
-0000e2d0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-0000e2e0: 2d0a 2020 2020 4465 6669 6e65 2061 206d  -.    Define a m
-0000e2f0: 6174 7269 7876 6172 6961 7465 206e 6f72  atrixvariate nor
-0000e300: 6d61 6c20 7661 7269 6162 6c65 2066 6f72  mal variable for
-0000e310: 2067 6976 656e 2072 6f77 2061 6e64 2063   given row and c
-0000e320: 6f6c 756d 6e20 636f 7661 7269 616e 6365  olumn covariance
-0000e330: 0a20 2020 206d 6174 7269 6365 733a 3a0a  .    matrices::.
-0000e340: 0a20 2020 2020 2020 2063 6f6c 636f 7620  .        colcov 
-0000e350: 3d20 6e70 2e61 7272 6179 285b 5b31 2e2c  = np.array([[1.,
-0000e360: 2030 2e35 5d2c 205b 302e 352c 2032 5d5d   0.5], [0.5, 2]]
-0000e370: 290a 2020 2020 2020 2020 726f 7763 6f76  ).        rowcov
-0000e380: 203d 206e 702e 6172 7261 7928 5b5b 312c   = np.array([[1,
-0000e390: 2030 2c20 305d 2c20 5b30 2c20 342c 2030   0, 0], [0, 4, 0
-0000e3a0: 5d2c 205b 302c 2030 2c20 3136 5d5d 290a  ], [0, 0, 16]]).
-0000e3b0: 2020 2020 2020 2020 6d20 3d20 726f 7763          m = rowc
-0000e3c0: 6f76 2e73 6861 7065 5b30 5d0a 2020 2020  ov.shape[0].    
-0000e3d0: 2020 2020 6e20 3d20 636f 6c63 6f76 2e73      n = colcov.s
-0000e3e0: 6861 7065 5b30 5d0a 2020 2020 2020 2020  hape[0].        
-0000e3f0: 6d75 203d 206e 702e 7a65 726f 7328 286d  mu = np.zeros((m
-0000e400: 2c20 6e29 290a 2020 2020 2020 2020 7661  , n)).        va
-0000e410: 6c73 203d 2070 6d2e 4d61 7472 6978 4e6f  ls = pm.MatrixNo
-0000e420: 726d 616c 2827 7661 6c73 272c 206d 753d  rmal('vals', mu=
-0000e430: 6d75 2c20 636f 6c63 6f76 3d63 6f6c 636f  mu, colcov=colco
-0000e440: 762c 0a20 2020 2020 2020 2020 2020 2020  v,.             
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 726f 7763 6f76 3d72 6f77 636f 7629    rowcov=rowcov)
-0000e470: 0a0a 2020 2020 4162 6f76 652c 2074 6865  ..    Above, the
-0000e480: 2069 7468 2072 6f77 2069 6e20 7661 6c73   ith row in vals
-0000e490: 2068 6173 2061 2076 6172 6961 6e63 6520   has a variance 
-0000e4a0: 7468 6174 2069 7320 7363 616c 6564 2062  that is scaled b
-0000e4b0: 7920 345e 692e 0a20 2020 2041 6c74 6572  y 4^i..    Alter
-0000e4c0: 6e61 7469 7665 6c79 2c20 726f 7720 6f72  natively, row or
-0000e4d0: 2063 6f6c 756d 6e20 6368 6f6c 6573 6b79   column cholesky
-0000e4e0: 206d 6174 7269 6365 7320 636f 756c 6420   matrices could 
-0000e4f0: 6265 2073 7562 7374 6974 7574 6564 2066  be substituted f
-0000e500: 6f72 0a20 2020 2065 6974 6865 7220 636f  or.    either co
-0000e510: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
-0000e520: 2054 6865 204d 6174 7269 784e 6f72 6d61   The MatrixNorma
-0000e530: 6c20 6973 2071 7569 636b 6572 2077 6179  l is quicker way
-0000e540: 2063 6f6d 7075 7465 0a20 2020 204d 764e   compute.    MvN
-0000e550: 6f72 6d61 6c28 6d75 2c20 6e70 2e6b 726f  ormal(mu, np.kro
-0000e560: 6e28 726f 7763 6f76 2c20 636f 6c63 6f76  n(rowcov, colcov
-0000e570: 2929 2074 6861 7420 7461 6b65 7320 6164  )) that takes ad
-0000e580: 7661 6e74 6167 6520 6f66 206b 726f 6e65  vantage of krone
-0000e590: 636b 6572 2070 726f 6475 6374 0a20 2020  cker product.   
-0000e5a0: 2070 726f 7065 7274 6965 7320 666f 7220   properties for 
-0000e5b0: 696e 7665 7273 696f 6e2e 2046 6f72 2065  inversion. For e
-0000e5c0: 7861 6d70 6c65 2c20 6966 2064 7261 7773  xample, if draws
-0000e5d0: 2066 726f 6d20 4d76 4e6f 726d 616c 2068   from MvNormal h
-0000e5e0: 6164 2074 6865 2073 616d 650a 2020 2020  ad the same.    
-0000e5f0: 636f 7661 7269 616e 6365 2073 7472 7563  covariance struc
-0000e600: 7475 7265 2c20 6275 7420 7765 7265 2073  ture, but were s
-0000e610: 6361 6c65 6420 6279 2064 6966 6665 7265  caled by differe
-0000e620: 6e74 2070 6f77 6572 7320 6f66 2061 6e20  nt powers of an 
-0000e630: 756e 6b6e 6f77 6e0a 2020 2020 636f 6e73  unknown.    cons
-0000e640: 7461 6e74 2c20 626f 7468 2074 6865 2063  tant, both the c
-0000e650: 6f76 6172 6961 6e63 6520 616e 6420 7363  ovariance and sc
-0000e660: 616c 696e 6720 636f 756c 6420 6265 206c  aling could be l
-0000e670: 6561 726e 6564 2061 7320 666f 6c6c 6f77  earned as follow
-0000e680: 730a 2020 2020 2873 6565 2074 6865 2064  s.    (see the d
-0000e690: 6f63 7374 7269 6e67 206f 6620 604c 4b4a  ocstring of `LKJ
-0000e6a0: 4368 6f6c 6573 6b79 436f 7660 2066 6f72  CholeskyCov` for
-0000e6b0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-0000e6c0: 6e20 6162 6f75 7420 7468 6973 290a 0a20  n about this).. 
-0000e6d0: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
-0000e6e0: 686f 6e0a 0a20 2020 2020 2020 2023 2053  hon..        # S
-0000e6f0: 6574 7570 2064 6174 610a 2020 2020 2020  etup data.      
-0000e700: 2020 7472 7565 5f63 6f6c 636f 7620 3d20    true_colcov = 
-0000e710: 6e70 2e61 7272 6179 285b 5b31 2e30 2c20  np.array([[1.0, 
-0000e720: 302e 352c 2030 2e31 5d2c 0a20 2020 2020  0.5, 0.1],.     
-0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 2020 2020 2020 2020 205b 302e 352c             [0.5,
-0000e750: 2031 2e30 2c20 302e 325d 2c0a 2020 2020   1.0, 0.2],.    
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 2020 2020 2020 2020 2020 2020 5b30 2e31              [0.1
-0000e780: 2c20 302e 322c 2031 2e30 5d5d 290a 2020  , 0.2, 1.0]]).  
-0000e790: 2020 2020 2020 6d20 3d20 330a 2020 2020        m = 3.    
-0000e7a0: 2020 2020 6e20 3d20 7472 7565 5f63 6f6c      n = true_col
-0000e7b0: 636f 762e 7368 6170 655b 305d 0a20 2020  cov.shape[0].   
-0000e7c0: 2020 2020 2074 7275 655f 7363 616c 6520       true_scale 
-0000e7d0: 3d20 330a 2020 2020 2020 2020 7472 7565  = 3.        true
-0000e7e0: 5f72 6f77 636f 7620 3d20 6e70 2e64 6961  _rowcov = np.dia
-0000e7f0: 6728 5b74 7275 655f 7363 616c 652a 2a28  g([true_scale**(
-0000e800: 322a 6929 2066 6f72 2069 2069 6e20 7261  2*i) for i in ra
-0000e810: 6e67 6528 6d29 5d29 0a20 2020 2020 2020  nge(m)]).       
-0000e820: 206d 7520 3d20 6e70 2e7a 6572 6f73 2828   mu = np.zeros((
-0000e830: 6d2c 206e 2929 0a20 2020 2020 2020 2074  m, n)).        t
-0000e840: 7275 655f 6b72 6f6e 203d 206e 702e 6b72  rue_kron = np.kr
-0000e850: 6f6e 2874 7275 655f 726f 7763 6f76 2c20  on(true_rowcov, 
-0000e860: 7472 7565 5f63 6f6c 636f 7629 0a20 2020  true_colcov).   
-0000e870: 2020 2020 2064 6174 6120 3d20 6e70 2e72       data = np.r
-0000e880: 616e 646f 6d2e 6d75 6c74 6976 6172 6961  andom.multivaria
-0000e890: 7465 5f6e 6f72 6d61 6c28 6d75 2e66 6c61  te_normal(mu.fla
-0000e8a0: 7474 656e 2829 2c20 7472 7565 5f6b 726f  tten(), true_kro
-0000e8b0: 6e29 0a20 2020 2020 2020 2064 6174 6120  n).        data 
-0000e8c0: 3d20 6461 7461 2e72 6573 6861 7065 286d  = data.reshape(m
-0000e8d0: 2c20 6e29 0a0a 2020 2020 2020 2020 7769  , n)..        wi
-0000e8e0: 7468 2070 6d2e 4d6f 6465 6c28 2920 6173  th pm.Model() as
-0000e8f0: 206d 6f64 656c 3a0a 2020 2020 2020 2020   model:.        
-0000e900: 2020 2020 2320 5365 7475 7020 7269 6768      # Setup righ
-0000e910: 7420 6368 6f6c 6573 6b79 206d 6174 7269  t cholesky matri
-0000e920: 780a 2020 2020 2020 2020 2020 2020 7364  x.            sd
-0000e930: 5f64 6973 7420 3d20 706d 2e48 616c 6643  _dist = pm.HalfC
-0000e940: 6175 6368 792e 6469 7374 2862 6574 613d  auchy.dist(beta=
-0000e950: 322e 352c 2073 6861 7065 3d33 290a 2020  2.5, shape=3).  
-0000e960: 2020 2020 2020 2020 2020 636f 6c63 686f            colcho
-0000e970: 6c5f 7061 636b 6564 203d 2070 6d2e 4c4b  l_packed = pm.LK
-0000e980: 4a43 686f 6c65 736b 7943 6f76 2827 636f  JCholeskyCov('co
-0000e990: 6c63 686f 6c70 6163 6b65 6427 2c20 6e3d  lcholpacked', n=
-0000e9a0: 332c 2065 7461 3d32 2c0a 2020 2020 2020  3, eta=2,.      
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2020 2020 2020 2073 645f 6469 7374           sd_dist
-0000e9e0: 3d73 645f 6469 7374 290a 2020 2020 2020  =sd_dist).      
-0000e9f0: 2020 2020 2020 636f 6c63 686f 6c20 3d20        colchol = 
-0000ea00: 706d 2e65 7870 616e 645f 7061 636b 6564  pm.expand_packed
-0000ea10: 5f74 7269 616e 6775 6c61 7228 332c 2063  _triangular(3, c
-0000ea20: 6f6c 6368 6f6c 5f70 6163 6b65 6429 0a0a  olchol_packed)..
-0000ea30: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
-0000ea40: 7475 7020 6c65 6674 2063 6f76 6172 6961  tup left covaria
-0000ea50: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
-0000ea60: 2020 2020 2020 2073 6361 6c65 203d 2070         scale = p
-0000ea70: 6d2e 4c6f 674e 6f72 6d61 6c28 2773 6361  m.LogNormal('sca
-0000ea80: 6c65 272c 206d 753d 6e70 2e6c 6f67 2874  le', mu=np.log(t
-0000ea90: 7275 655f 7363 616c 6529 2c20 7369 676d  rue_scale), sigm
-0000eaa0: 613d 302e 3529 0a20 2020 2020 2020 2020  a=0.5).         
-0000eab0: 2020 2072 6f77 636f 7620 3d20 7074 2e64     rowcov = pt.d
-0000eac0: 6961 6728 5b73 6361 6c65 2a2a 2832 2a69  iag([scale**(2*i
-0000ead0: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
-0000eae0: 286d 295d 290a 0a20 2020 2020 2020 2020  (m)])..         
-0000eaf0: 2020 2076 616c 7320 3d20 706d 2e4d 6174     vals = pm.Mat
-0000eb00: 7269 784e 6f72 6d61 6c28 2776 616c 7327  rixNormal('vals'
-0000eb10: 2c20 6d75 3d6d 752c 2063 6f6c 6368 6f6c  , mu=mu, colchol
-0000eb20: 3d63 6f6c 6368 6f6c 2c20 726f 7763 6f76  =colchol, rowcov
-0000eb30: 3d72 6f77 636f 762c 0a20 2020 2020 2020  =rowcov,.       
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 2020 2020 2020 2020 2020 2020 6f62 7365              obse
-0000eb60: 7276 6564 3d64 6174 6129 0a20 2020 2022  rved=data).    "
-0000eb70: 2222 0a20 2020 2072 765f 6f70 203d 206d  "".    rv_op = m
-0000eb80: 6174 7269 786e 6f72 6d61 6c0a 0a20 2020  atrixnormal..   
-0000eb90: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-0000eba0: 2020 6465 6620 6469 7374 280a 2020 2020    def dist(.    
-0000ebb0: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
-0000ebc0: 206d 752c 0a20 2020 2020 2020 2072 6f77   mu,.        row
-0000ebd0: 636f 763d 4e6f 6e65 2c0a 2020 2020 2020  cov=None,.      
-0000ebe0: 2020 726f 7763 686f 6c3d 4e6f 6e65 2c0a    rowchol=None,.
-0000ebf0: 2020 2020 2020 2020 636f 6c63 6f76 3d4e          colcov=N
-0000ec00: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
-0000ec10: 6368 6f6c 3d4e 6f6e 652c 0a20 2020 2020  chol=None,.     
-0000ec20: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
-0000ec30: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-0000ec40: 293a 0a20 2020 2020 2020 2063 686f 6c65  ):.        chole
-0000ec50: 736b 7920 3d20 4368 6f6c 6573 6b79 286c  sky = Cholesky(l
-0000ec60: 6f77 6572 3d54 7275 652c 206f 6e5f 6572  ower=True, on_er
-0000ec70: 726f 723d 2272 6169 7365 2229 0a0a 2020  ror="raise")..  
-0000ec80: 2020 2020 2020 2320 416d 6f6e 672d 726f        # Among-ro
-0000ec90: 7720 6d61 7472 6963 6573 0a20 2020 2020  w matrices.     
-0000eca0: 2020 2069 6620 6c65 6e28 5b69 2066 6f72     if len([i for
-0000ecb0: 2069 2069 6e20 5b72 6f77 636f 762c 2072   i in [rowcov, r
-0000ecc0: 6f77 6368 6f6c 5d20 6966 2069 2069 7320  owchol] if i is 
-0000ecd0: 6e6f 7420 4e6f 6e65 5d29 2021 3d20 313a  not None]) != 1:
-0000ece0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000ecf0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000ed10: 496e 636f 6d70 6174 6962 6c65 2070 6172  Incompatible par
-0000ed20: 616d 6574 6572 697a 6174 696f 6e2e 2053  ameterization. S
-0000ed30: 7065 6369 6679 2065 7861 6374 6c79 206f  pecify exactly o
-0000ed40: 6e65 206f 6620 726f 7763 6f76 2c20 6f72  ne of rowcov, or
-0000ed50: 2072 6f77 6368 6f6c 2e22 0a20 2020 2020   rowchol.".     
-0000ed60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000ed70: 2069 6620 726f 7763 6f76 2069 7320 6e6f   if rowcov is no
-0000ed80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ed90: 2020 2020 6966 2072 6f77 636f 762e 6e64      if rowcov.nd
-0000eda0: 696d 2021 3d20 323a 0a20 2020 2020 2020  im != 2:.       
-0000edb0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000edc0: 616c 7565 4572 726f 7228 2272 6f77 636f  alueError("rowco
-0000edd0: 7620 6d75 7374 2062 6520 7477 6f20 6469  v must be two di
-0000ede0: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
-0000edf0: 2020 2020 2020 2020 2072 6f77 6368 6f6c           rowchol
-0000ee00: 5f63 6f76 203d 2063 686f 6c65 736b 7928  _cov = cholesky(
-0000ee10: 726f 7763 6f76 290a 2020 2020 2020 2020  rowcov).        
-0000ee20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000ee30: 2020 6966 2072 6f77 6368 6f6c 2e6e 6469    if rowchol.ndi
-0000ee40: 6d20 213d 2032 3a0a 2020 2020 2020 2020  m != 2:.        
-0000ee50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000ee60: 6c75 6545 7272 6f72 2822 726f 7763 686f  lueError("rowcho
-0000ee70: 6c20 6d75 7374 2062 6520 7477 6f20 6469  l must be two di
-0000ee80: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
-0000ee90: 2020 2020 2020 2020 2072 6f77 6368 6f6c           rowchol
-0000eea0: 5f63 6f76 203d 2070 742e 6173 5f74 656e  _cov = pt.as_ten
-0000eeb0: 736f 725f 7661 7269 6162 6c65 2872 6f77  sor_variable(row
-0000eec0: 6368 6f6c 290a 0a20 2020 2020 2020 2023  chol)..        #
-0000eed0: 2041 6d6f 6e67 2d63 6f6c 756d 6e20 6d61   Among-column ma
-0000eee0: 7472 6963 6573 0a20 2020 2020 2020 2069  trices.        i
-0000eef0: 6620 6c65 6e28 5b69 2066 6f72 2069 2069  f len([i for i i
-0000ef00: 6e20 5b63 6f6c 636f 762c 2063 6f6c 6368  n [colcov, colch
-0000ef10: 6f6c 5d20 6966 2069 2069 7320 6e6f 7420  ol] if i is not 
-0000ef20: 4e6f 6e65 5d29 2021 3d20 313a 0a20 2020  None]) != 1:.   
-0000ef30: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000ef40: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0000ef50: 2020 2020 2020 2020 2020 2022 496e 636f             "Inco
-0000ef60: 6d70 6174 6962 6c65 2070 6172 616d 6574  mpatible paramet
-0000ef70: 6572 697a 6174 696f 6e2e 2053 7065 6369  erization. Speci
-0000ef80: 6679 2065 7861 6374 6c79 206f 6e65 206f  fy exactly one o
-0000ef90: 6620 636f 6c63 6f76 2c20 6f72 2063 6f6c  f colcov, or col
-0000efa0: 6368 6f6c 2e22 0a20 2020 2020 2020 2020  chol.".         
-0000efb0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-0000efc0: 636f 6c63 6f76 2069 7320 6e6f 7420 4e6f  colcov is not No
-0000efd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000efe0: 636f 6c63 6f76 203d 2070 742e 6173 5f74  colcov = pt.as_t
-0000eff0: 656e 736f 725f 7661 7269 6162 6c65 2863  ensor_variable(c
-0000f000: 6f6c 636f 7629 0a20 2020 2020 2020 2020  olcov).         
-0000f010: 2020 2069 6620 636f 6c63 6f76 2e6e 6469     if colcov.ndi
-0000f020: 6d20 213d 2032 3a0a 2020 2020 2020 2020  m != 2:.        
-0000f030: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000f040: 6c75 6545 7272 6f72 2822 636f 6c63 6f76  lueError("colcov
-0000f050: 206d 7573 7420 6265 2074 776f 2064 696d   must be two dim
-0000f060: 656e 7369 6f6e 616c 2e22 290a 2020 2020  ensional.").    
-0000f070: 2020 2020 2020 2020 636f 6c63 686f 6c5f          colchol_
-0000f080: 636f 7620 3d20 6368 6f6c 6573 6b79 2863  cov = cholesky(c
-0000f090: 6f6c 636f 7629 0a20 2020 2020 2020 2065  olcov).        e
-0000f0a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f0b0: 2069 6620 636f 6c63 686f 6c2e 6e64 696d   if colchol.ndim
-0000f0c0: 2021 3d20 323a 0a20 2020 2020 2020 2020   != 2:.         
-0000f0d0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0000f0e0: 7565 4572 726f 7228 2263 6f6c 6368 6f6c  ueError("colchol
-0000f0f0: 206d 7573 7420 6265 2074 776f 2064 696d   must be two dim
-0000f100: 656e 7369 6f6e 616c 2e22 290a 2020 2020  ensional.").    
-0000f110: 2020 2020 2020 2020 636f 6c63 686f 6c5f          colchol_
-0000f120: 636f 7620 3d20 7074 2e61 735f 7465 6e73  cov = pt.as_tens
-0000f130: 6f72 5f76 6172 6961 626c 6528 636f 6c63  or_variable(colc
-0000f140: 686f 6c29 0a0a 2020 2020 2020 2020 6469  hol)..        di
-0000f150: 7374 5f73 6861 7065 203d 2028 726f 7763  st_shape = (rowc
-0000f160: 686f 6c5f 636f 762e 7368 6170 655b 2d31  hol_cov.shape[-1
-0000f170: 5d2c 2063 6f6c 6368 6f6c 5f63 6f76 2e73  ], colchol_cov.s
-0000f180: 6861 7065 5b2d 315d 290a 0a20 2020 2020  hape[-1])..     
-0000f190: 2020 2023 2042 726f 6164 6361 7374 696e     # Broadcastin
-0000f1a0: 6720 6d75 0a20 2020 2020 2020 206d 7520  g mu.        mu 
-0000f1b0: 3d20 7074 2e65 7874 7261 5f6f 7073 2e62  = pt.extra_ops.b
-0000f1c0: 726f 6164 6361 7374 5f74 6f28 6d75 2c20  roadcast_to(mu, 
-0000f1d0: 7368 6170 653d 6469 7374 5f73 6861 7065  shape=dist_shape
-0000f1e0: 290a 2020 2020 2020 2020 6d75 203d 2070  ).        mu = p
-0000f1f0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-0000f200: 6162 6c65 2866 6c6f 6174 5828 6d75 2929  able(floatX(mu))
-0000f210: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000f220: 2073 7570 6572 2829 2e64 6973 7428 5b6d   super().dist([m
-0000f230: 752c 2072 6f77 6368 6f6c 5f63 6f76 2c20  u, rowchol_cov, 
-0000f240: 636f 6c63 686f 6c5f 636f 765d 2c20 2a2a  colchol_cov], **
-0000f250: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-0000f260: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
-0000f270: 2c20 6d75 2c20 726f 7763 686f 6c2c 2063  , mu, rowchol, c
-0000f280: 6f6c 6368 6f6c 293a 0a20 2020 2020 2020  olchol):.       
-0000f290: 2072 6574 7572 6e20 7074 2e66 756c 6c5f   return pt.full_
-0000f2a0: 6c69 6b65 2872 762c 206d 7529 0a0a 2020  like(rv, mu)..  
-0000f2b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
-0000f2c0: 2c20 6d75 2c20 726f 7763 686f 6c2c 2063  , mu, rowchol, c
-0000f2d0: 6f6c 6368 6f6c 293a 0a20 2020 2020 2020  olchol):.       
-0000f2e0: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
-0000f2f0: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
-0000f300: 6269 6c69 7479 206f 6620 4d61 7472 6978  bility of Matrix
-0000f310: 2d76 616c 7565 6420 4e6f 726d 616c 2064  -valued Normal d
-0000f320: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
-0000f330: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
-0000f340: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-0000f350: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000f360: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000f370: 2020 2020 2020 2076 616c 7565 3a20 6e75         value: nu
-0000f380: 6d65 7269 630a 2020 2020 2020 2020 2020  meric.          
-0000f390: 2020 5661 6c75 6520 666f 7220 7768 6963    Value for whic
-0000f3a0: 6820 6c6f 672d 7072 6f62 6162 696c 6974  h log-probabilit
-0000f3b0: 7920 6973 2063 616c 6375 6c61 7465 642e  y is calculated.
-0000f3c0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000f3d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000f3e0: 2d0a 2020 2020 2020 2020 5465 6e73 6f72  -.        Tensor
-0000f3f0: 5661 7269 6162 6c65 0a20 2020 2020 2020  Variable.       
-0000f400: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-0000f410: 2076 616c 7565 2e6e 6469 6d20 213d 2032   value.ndim != 2
-0000f420: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000f430: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0000f440: 5661 6c75 6520 6d75 7374 2062 6520 7477  Value must be tw
-0000f450: 6f20 6469 6d65 6e73 696f 6e61 6c2e 2229  o dimensional.")
-0000f460: 0a0a 2020 2020 2020 2020 2320 436f 6d70  ..        # Comp
-0000f470: 7574 6520 5472 5b63 6f6c 636f 765e 2d31  ute Tr[colcov^-1
-0000f480: 2040 2028 7820 2d20 6d75 292e 5420 4020   @ (x - mu).T @ 
-0000f490: 726f 7763 6f76 5e2d 3120 4020 2878 202d  rowcov^-1 @ (x -
-0000f4a0: 206d 7529 5d20 616e 640a 2020 2020 2020   mu)] and.      
-0000f4b0: 2020 2320 7468 6520 6c6f 6764 6574 206f    # the logdet o
-0000f4c0: 6620 636f 6c63 6f76 2061 6e64 2072 6f77  f colcov and row
-0000f4d0: 636f 762e 0a20 2020 2020 2020 2064 656c  cov..        del
-0000f4e0: 7461 203d 2076 616c 7565 202d 206d 750a  ta = value - mu.
-0000f4f0: 0a20 2020 2020 2020 2023 2046 696e 6420  .        # Find 
-0000f500: 6578 706f 6e65 6e74 2070 6965 6365 2062  exponent piece b
-0000f510: 7920 7069 6563 650a 2020 2020 2020 2020  y piece.        
-0000f520: 7269 6768 745f 7175 6164 6469 7374 203d  right_quaddist =
-0000f530: 2073 6f6c 7665 5f6c 6f77 6572 2872 6f77   solve_lower(row
-0000f540: 6368 6f6c 2c20 6465 6c74 6129 0a20 2020  chol, delta).   
-0000f550: 2020 2020 2071 7561 6464 6973 7420 3d20       quaddist = 
-0000f560: 7074 2e6e 6c69 6e61 6c67 2e6d 6174 7269  pt.nlinalg.matri
-0000f570: 785f 646f 7428 7269 6768 745f 7175 6164  x_dot(right_quad
-0000f580: 6469 7374 2e54 2c20 7269 6768 745f 7175  dist.T, right_qu
-0000f590: 6164 6469 7374 290a 2020 2020 2020 2020  addist).        
-0000f5a0: 7175 6164 6469 7374 203d 2073 6f6c 7665  quaddist = solve
-0000f5b0: 5f6c 6f77 6572 2863 6f6c 6368 6f6c 2c20  _lower(colchol, 
-0000f5c0: 7175 6164 6469 7374 290a 2020 2020 2020  quaddist).      
-0000f5d0: 2020 7175 6164 6469 7374 203d 2073 6f6c    quaddist = sol
-0000f5e0: 7665 5f75 7070 6572 2863 6f6c 6368 6f6c  ve_upper(colchol
-0000f5f0: 2e54 2c20 7175 6164 6469 7374 290a 2020  .T, quaddist).  
-0000f600: 2020 2020 2020 7472 7175 6164 6469 7374        trquaddist
-0000f610: 203d 2070 742e 6e6c 696e 616c 672e 7472   = pt.nlinalg.tr
-0000f620: 6163 6528 7175 6164 6469 7374 290a 0a20  ace(quaddist).. 
-0000f630: 2020 2020 2020 2063 6f6c 6469 6167 203d         coldiag =
-0000f640: 2070 742e 6469 6167 2863 6f6c 6368 6f6c   pt.diag(colchol
-0000f650: 290a 2020 2020 2020 2020 726f 7764 6961  ).        rowdia
-0000f660: 6720 3d20 7074 2e64 6961 6728 726f 7763  g = pt.diag(rowc
-0000f670: 686f 6c29 0a20 2020 2020 2020 2068 616c  hol).        hal
-0000f680: 665f 636f 6c6c 6f67 6465 7420 3d20 7074  f_collogdet = pt
-0000f690: 2e73 756d 2870 742e 6c6f 6728 636f 6c64  .sum(pt.log(cold
-0000f6a0: 6961 6729 2920 2023 206c 6f67 6465 7428  iag))  # logdet(
-0000f6b0: 4d29 203d 2032 2a54 7228 6c6f 6728 4c29  M) = 2*Tr(log(L)
-0000f6c0: 290a 2020 2020 2020 2020 6861 6c66 5f72  ).        half_r
-0000f6d0: 6f77 6c6f 6764 6574 203d 2070 742e 7375  owlogdet = pt.su
-0000f6e0: 6d28 7074 2e6c 6f67 2872 6f77 6469 6167  m(pt.log(rowdiag
-0000f6f0: 2929 2020 2320 5573 696e 6720 4368 6f6c  ))  # Using Chol
-0000f700: 6573 6b79 3a20 4d20 3d20 4c20 4c5e 540a  esky: M = L L^T.
-0000f710: 0a20 2020 2020 2020 206d 203d 2072 6f77  .        m = row
-0000f720: 6368 6f6c 2e73 6861 7065 5b30 5d0a 2020  chol.shape[0].  
-0000f730: 2020 2020 2020 6e20 3d20 636f 6c63 686f        n = colcho
-0000f740: 6c2e 7368 6170 655b 305d 0a0a 2020 2020  l.shape[0]..    
-0000f750: 2020 2020 6e6f 726d 203d 202d 302e 3520      norm = -0.5 
-0000f760: 2a20 6d20 2a20 6e20 2a20 706d 2e66 6c6f  * m * n * pm.flo
-0000f770: 6174 5828 6e70 2e6c 6f67 2832 202a 206e  atX(np.log(2 * n
-0000f780: 702e 7069 2929 0a20 2020 2020 2020 2072  p.pi)).        r
-0000f790: 6574 7572 6e20 6e6f 726d 202d 2030 2e35  eturn norm - 0.5
-0000f7a0: 202a 2074 7271 7561 6464 6973 7420 2d20   * trquaddist - 
-0000f7b0: 6d20 2a20 6861 6c66 5f63 6f6c 6c6f 6764  m * half_collogd
-0000f7c0: 6574 202d 206e 202a 2068 616c 665f 726f  et - n * half_ro
-0000f7d0: 776c 6f67 6465 740a 0a0a 636c 6173 7320  wlogdet...class 
-0000f7e0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c52  KroneckerNormalR
-0000f7f0: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
-0000f800: 293a 0a20 2020 206e 616d 6520 3d20 226b  ):.    name = "k
-0000f810: 726f 6e65 636b 6572 6e6f 726d 616c 220a  roneckernormal".
-0000f820: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
-0000f830: 310a 2020 2020 6e64 696d 735f 7061 7261  1.    ndims_para
-0000f840: 6d73 203d 205b 312c 2030 2c20 325d 0a20  ms = [1, 0, 2]. 
-0000f850: 2020 2064 7479 7065 203d 2022 666c 6f61     dtype = "floa
-0000f860: 7458 220a 2020 2020 5f70 7269 6e74 5f6e  tX".    _print_n
-0000f870: 616d 6520 3d20 2822 4b72 6f6e 6563 6b65  ame = ("Kronecke
-0000f880: 724e 6f72 6d61 6c22 2c20 225c 5c6f 7065  rNormal", "\\ope
-0000f890: 7261 746f 726e 616d 657b 4b72 6f6e 6563  ratorname{Kronec
-0000f8a0: 6b65 724e 6f72 6d61 6c7d 2229 0a0a 2020  kerNormal}")..  
-0000f8b0: 2020 6465 6620 726e 675f 666e 2873 656c    def rng_fn(sel
-0000f8c0: 662c 2072 6e67 2c20 6d75 2c20 7369 676d  f, rng, mu, sigm
-0000f8d0: 612c 202a 636f 7673 2c20 7369 7a65 3d4e  a, *covs, size=N
-0000f8e0: 6f6e 6529 3a0a 2020 2020 2020 2020 7369  one):.        si
-0000f8f0: 7a65 203d 2073 697a 6520 6966 2073 697a  ze = size if siz
-0000f900: 6520 656c 7365 2063 6f76 735b 2d31 5d0a  e else covs[-1].
-0000f910: 2020 2020 2020 2020 636f 7673 203d 2063          covs = c
-0000f920: 6f76 735b 3a2d 315d 2069 6620 636f 7673  ovs[:-1] if covs
-0000f930: 5b2d 315d 203d 3d20 7369 7a65 2065 6c73  [-1] == size els
-0000f940: 6520 636f 7673 0a0a 2020 2020 2020 2020  e covs..        
-0000f950: 636f 7620 3d20 7265 6475 6365 286c 696e  cov = reduce(lin
-0000f960: 616c 672e 6b72 6f6e 2c20 636f 7673 290a  alg.kron, covs).
-0000f970: 0a20 2020 2020 2020 2069 6620 7369 676d  .        if sigm
-0000f980: 613a 0a20 2020 2020 2020 2020 2020 2063  a:.            c
-0000f990: 6f76 203d 2063 6f76 202b 2073 6967 6d61  ov = cov + sigma
-0000f9a0: 2a2a 3220 2a20 6e70 2e65 7965 2863 6f76  **2 * np.eye(cov
-0000f9b0: 2e73 6861 7065 5b30 5d29 0a0a 2020 2020  .shape[0])..    
-0000f9c0: 2020 2020 7820 3d20 6d75 6c74 6976 6172      x = multivar
-0000f9d0: 6961 7465 5f6e 6f72 6d61 6c2e 726e 675f  iate_normal.rng_
-0000f9e0: 666e 2872 6e67 3d72 6e67 2c20 6d65 616e  fn(rng=rng, mean
-0000f9f0: 3d6d 752c 2063 6f76 3d63 6f76 2c20 7369  =mu, cov=cov, si
-0000fa00: 7a65 3d73 697a 6529 0a20 2020 2020 2020  ze=size).       
-0000fa10: 2072 6574 7572 6e20 780a 0a0a 6b72 6f6e   return x...kron
-0000fa20: 6563 6b65 726e 6f72 6d61 6c20 3d20 4b72  eckernormal = Kr
-0000fa30: 6f6e 6563 6b65 724e 6f72 6d61 6c52 5628  oneckerNormalRV(
-0000fa40: 290a 0a0a 636c 6173 7320 4b72 6f6e 6563  )...class Kronec
-0000fa50: 6b65 724e 6f72 6d61 6c28 436f 6e74 696e  kerNormal(Contin
-0000fa60: 756f 7573 293a 0a20 2020 2072 2222 220a  uous):.    r""".
-0000fa70: 2020 2020 4d75 6c74 6976 6172 6961 7465      Multivariate
-0000fa80: 206e 6f72 6d61 6c20 6c6f 672d 6c69 6b65   normal log-like
-0000fa90: 6c69 686f 6f64 2077 6974 6820 4b72 6f6e  lihood with Kron
-0000faa0: 6563 6b65 722d 7374 7275 6374 7572 6564  ecker-structured
-0000fab0: 2063 6f76 6172 6961 6e63 652e 0a0a 2020   covariance...  
-0000fac0: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
-0000fad0: 2020 2020 6628 7820 5c6d 6964 205c 6d75      f(x \mid \mu
-0000fae0: 2c20 4b29 203d 0a20 2020 2020 2020 2020  , K) =.         
-0000faf0: 2020 5c66 7261 637b 317d 7b28 325c 7069    \frac{1}{(2\pi
-0000fb00: 207c 4b7c 295e 7b31 2f32 7d7d 0a20 2020   |K|)^{1/2}}.   
-0000fb10: 2020 2020 2020 2020 5c65 7870 5c6c 6566          \exp\lef
-0000fb20: 745c 7b20 2d5c 6672 6163 7b31 7d7b 327d  t\{ -\frac{1}{2}
-0000fb30: 2028 782d 5c6d 7529 5e7b 5c70 7269 6d65   (x-\mu)^{\prime
-0000fb40: 7d20 4b5e 7b2d 317d 2028 782d 5c6d 7529  } K^{-1} (x-\mu)
-0000fb50: 205c 7269 6768 745c 7d0a 0a20 2020 203d   \right\}..    =
-0000fb60: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
-0000fb70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fb80: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
-0000fb90: 2020 3a6d 6174 683a 6078 205c 696e 205c    :math:`x \in \
-0000fba0: 6d61 7468 6262 7b52 7d5e 4e60 0a20 2020  mathbb{R}^N`.   
-0000fbb0: 204d 6561 6e20 2020 2020 203a 6d61 7468   Mean      :math
-0000fbc0: 3a60 5c6d 7560 0a20 2020 2056 6172 6961  :`\mu`.    Varia
-0000fbd0: 6e63 6520 203a 6d61 7468 3a60 4b20 3d20  nce  :math:`K = 
-0000fbe0: 5c62 6967 6f74 696d 6573 204b 5f69 202b  \bigotimes K_i +
-0000fbf0: 205c 7369 676d 615e 3220 495f 4e60 0a20   \sigma^2 I_N`. 
-0000fc00: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
-0000fc10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fc20: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
-0000fc30: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0000fc40: 2d2d 2d2d 2d2d 0a20 2020 206d 7520 3a20  ------.    mu : 
-0000fc50: 7465 6e73 6f72 5f6c 696b 6520 6f66 2066  tensor_like of f
-0000fc60: 6c6f 6174 0a20 2020 2020 2020 2056 6563  loat.        Vec
-0000fc70: 746f 7220 6f66 206d 6561 6e73 2c20 6a75  tor of means, ju
-0000fc80: 7374 2061 7320 696e 2060 4d76 4e6f 726d  st as in `MvNorm
-0000fc90: 616c 602e 0a20 2020 2063 6f76 7320 3a20  al`..    covs : 
-0000fca0: 6c69 7374 206f 6620 6172 7261 7973 0a20  list of arrays. 
-0000fcb0: 2020 2020 2020 2054 6865 2073 6574 206f         The set o
-0000fcc0: 6620 636f 7661 7269 616e 6365 206d 6174  f covariance mat
-0000fcd0: 7269 6365 7320 3a6d 6174 683a 605b 4b5f  rices :math:`[K_
-0000fce0: 312c 204b 5f32 2c20 2e2e 2e5d 6020 746f  1, K_2, ...]` to
-0000fcf0: 2062 650a 2020 2020 2020 2020 4b72 6f6e   be.        Kron
-0000fd00: 6563 6b65 7265 6420 696e 2074 6865 206f  eckered in the o
-0000fd10: 7264 6572 2070 726f 7669 6465 6420 3a6d  rder provided :m
-0000fd20: 6174 683a 605c 6269 676f 7469 6d65 7320  ath:`\bigotimes 
-0000fd30: 4b5f 6960 2e0a 2020 2020 6368 6f6c 7320  K_i`..    chols 
-0000fd40: 3a20 6c69 7374 206f 6620 6172 7261 7973  : list of arrays
-0000fd50: 0a20 2020 2020 2020 2054 6865 2073 6574  .        The set
-0000fd60: 206f 6620 6c6f 7765 7220 6368 6f6c 6573   of lower choles
-0000fd70: 6b79 206d 6174 7269 6365 7320 3a6d 6174  ky matrices :mat
-0000fd80: 683a 605b 4c5f 312c 204c 5f32 2c20 2e2e  h:`[L_1, L_2, ..
-0000fd90: 2e5d 6020 7375 6368 2074 6861 740a 2020  .]` such that.  
-0000fda0: 2020 2020 2020 3a6d 6174 683a 604b 5f69        :math:`K_i
-0000fdb0: 203d 204c 5f69 204c 5f69 2760 2e0a 2020   = L_i L_i'`..  
-0000fdc0: 2020 6576 6473 203a 206c 6973 7420 6f66    evds : list of
-0000fdd0: 2074 7570 6c65 730a 2020 2020 2020 2020   tuples.        
-0000fde0: 5468 6520 7365 7420 6f66 2065 6967 656e  The set of eigen
-0000fdf0: 7661 6c75 652d 7665 6374 6f72 2c20 6569  value-vector, ei
-0000fe00: 6765 6e76 6563 746f 722d 6d61 7472 6978  genvector-matrix
-0000fe10: 2070 6169 7273 0a20 2020 2020 2020 203a   pairs.        :
-0000fe20: 6d61 7468 3a60 5b28 765f 312c 2051 5f31  math:`[(v_1, Q_1
-0000fe30: 292c 2028 765f 322c 2051 5f32 292c 202e  ), (v_2, Q_2), .
-0000fe40: 2e2e 5d60 2073 7563 6820 7468 6174 0a20  ..]` such that. 
-0000fe50: 2020 2020 2020 203a 6d61 7468 3a60 4b5f         :math:`K_
-0000fe60: 6920 3d20 515f 6920 5c74 6578 747b 6469  i = Q_i \text{di
-0000fe70: 6167 7d28 765f 6929 2051 5f69 2760 2e20  ag}(v_i) Q_i'`. 
-0000fe80: 466f 7220 6578 616d 706c 653a 3a0a 0a20  For example::.. 
-0000fe90: 2020 2020 2020 2020 2020 2076 5f69 2c20             v_i, 
-0000fea0: 515f 6920 3d20 7074 2e6e 6c69 6e61 6c67  Q_i = pt.nlinalg
-0000feb0: 2e65 6967 6828 4b5f 6929 0a20 2020 2073  .eigh(K_i).    s
-0000fec0: 6967 6d61 203a 2073 6361 6c61 722c 206f  igma : scalar, o
-0000fed0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000fee0: 5374 616e 6461 7264 2064 6576 6961 7469  Standard deviati
-0000fef0: 6f6e 206f 6620 7468 6520 4761 7573 7369  on of the Gaussi
-0000ff00: 616e 2077 6869 7465 206e 6f69 7365 2e0a  an white noise..
-0000ff10: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-0000ff20: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044    --------.    D
-0000ff30: 6566 696e 6520 6120 6d75 6c74 6976 6172  efine a multivar
-0000ff40: 6961 7465 206e 6f72 6d61 6c20 7661 7269  iate normal vari
-0000ff50: 6162 6c65 2077 6974 6820 6120 636f 7661  able with a cova
-0000ff60: 7269 616e 6365 0a20 2020 203a 6d61 7468  riance.    :math
-0000ff70: 3a60 4b20 3d20 4b5f 3120 5c6f 7469 6d65  :`K = K_1 \otime
-0000ff80: 7320 4b5f 3260 0a0a 2020 2020 2e2e 2063  s K_2`..    .. c
-0000ff90: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-0000ffa0: 2020 2020 2020 4b31 203d 206e 702e 6172        K1 = np.ar
-0000ffb0: 7261 7928 5b5b 312e 2c20 302e 355d 2c20  ray([[1., 0.5], 
-0000ffc0: 5b30 2e35 2c20 325d 5d29 0a20 2020 2020  [0.5, 2]]).     
-0000ffd0: 2020 204b 3220 3d20 6e70 2e61 7272 6179     K2 = np.array
-0000ffe0: 285b 5b31 2e2c 2030 2e34 2c20 302e 325d  ([[1., 0.4, 0.2]
-0000fff0: 2c20 5b30 2e34 2c20 322c 2030 2e33 5d2c  , [0.4, 2, 0.3],
-00010000: 205b 302e 322c 2030 2e33 2c20 315d 5d29   [0.2, 0.3, 1]])
-00010010: 0a20 2020 2020 2020 2063 6f76 7320 3d20  .        covs = 
-00010020: 5b4b 312c 204b 325d 0a20 2020 2020 2020  [K1, K2].       
-00010030: 204e 203d 2036 0a20 2020 2020 2020 206d   N = 6.        m
-00010040: 7520 3d20 6e70 2e7a 6572 6f73 284e 290a  u = np.zeros(N).
-00010050: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
-00010060: 4d6f 6465 6c28 2920 6173 206d 6f64 656c  Model() as model
-00010070: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
-00010080: 6c73 203d 2070 6d2e 4b72 6f6e 6563 6b65  ls = pm.Kronecke
-00010090: 724e 6f72 6d61 6c28 2776 616c 7327 2c20  rNormal('vals', 
-000100a0: 6d75 3d6d 752c 2063 6f76 733d 636f 7673  mu=mu, covs=covs
-000100b0: 2c20 7368 6170 653d 4e29 0a0a 2020 2020  , shape=N)..    
-000100c0: 4566 6669 6369 656e 6379 2067 6169 6e73  Efficiency gains
-000100d0: 2061 7265 206d 6164 6520 6279 2063 686f   are made by cho
-000100e0: 6c65 736b 7920 6465 636f 6d70 6f73 696e  lesky decomposin
-000100f0: 6720 3a6d 6174 683a 604b 5f31 6020 616e  g :math:`K_1` an
-00010100: 640a 2020 2020 3a6d 6174 683a 604b 5f32  d.    :math:`K_2
-00010110: 6020 696e 6469 7669 6475 616c 6c79 2072  ` individually r
-00010120: 6174 6865 7220 7468 616e 2074 6865 206c  ather than the l
-00010130: 6172 6765 7220 3a6d 6174 683a 604b 6020  arger :math:`K` 
-00010140: 6d61 7472 6978 2e20 416c 7468 6f75 6768  matrix. Although
-00010150: 0a20 2020 206f 6e6c 7920 7477 6f20 6d61  .    only two ma
-00010160: 7472 6963 6573 203a 6d61 7468 3a60 4b5f  trices :math:`K_
-00010170: 3160 2061 6e64 203a 6d61 7468 3a60 4b5f  1` and :math:`K_
-00010180: 3260 2061 7265 2073 686f 776e 2068 6572  2` are shown her
-00010190: 652c 2061 6e20 6172 6269 7472 6172 790a  e, an arbitrary.
-000101a0: 2020 2020 6e75 6d62 6572 206f 6620 7375      number of su
-000101b0: 626d 6174 7269 6365 7320 6361 6e20 6265  bmatrices can be
-000101c0: 2063 6f6d 6269 6e65 6420 696e 2074 6869   combined in thi
-000101d0: 7320 7761 792e 2043 686f 6c65 736b 7973  s way. Choleskys
-000101e0: 2061 6e64 0a20 2020 2065 6967 656e 6465   and.    eigende
-000101f0: 636f 6d70 6f73 6974 696f 6e73 2063 616e  compositions can
-00010200: 2062 6520 7072 6f76 6964 6564 2069 6e73   be provided ins
-00010210: 7465 6164 0a0a 2020 2020 2e2e 2063 6f64  tead..    .. cod
-00010220: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00010230: 2020 2020 6368 6f6c 7320 3d20 5b6e 702e      chols = [np.
-00010240: 6c69 6e61 6c67 2e63 686f 6c65 736b 7928  linalg.cholesky(
-00010250: 4b69 2920 666f 7220 4b69 2069 6e20 636f  Ki) for Ki in co
-00010260: 7673 5d0a 2020 2020 2020 2020 6576 6473  vs].        evds
-00010270: 203d 205b 6e70 2e6c 696e 616c 672e 6569   = [np.linalg.ei
-00010280: 6768 284b 6929 2066 6f72 204b 6920 696e  gh(Ki) for Ki in
-00010290: 2063 6f76 735d 0a20 2020 2020 2020 2077   covs].        w
-000102a0: 6974 6820 706d 2e4d 6f64 656c 2829 2061  ith pm.Model() a
-000102b0: 7320 6d6f 6465 6c3a 0a20 2020 2020 2020  s model:.       
-000102c0: 2020 2020 2076 616c 7332 203d 2070 6d2e       vals2 = pm.
-000102d0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c28  KroneckerNormal(
-000102e0: 2776 616c 7332 272c 206d 753d 6d75 2c20  'vals2', mu=mu, 
-000102f0: 6368 6f6c 733d 6368 6f6c 732c 2073 6861  chols=chols, sha
-00010300: 7065 3d4e 290a 2020 2020 2020 2020 2020  pe=N).          
-00010310: 2020 2320 6f72 0a20 2020 2020 2020 2020    # or.         
-00010320: 2020 2076 616c 7333 203d 2070 6d2e 4b72     vals3 = pm.Kr
-00010330: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
-00010340: 616c 7333 272c 206d 753d 6d75 2c20 6576  als3', mu=mu, ev
-00010350: 6473 3d65 7664 732c 2073 6861 7065 3d4e  ds=evds, shape=N
-00010360: 290a 0a20 2020 206e 6569 7468 6572 206f  )..    neither o
-00010370: 6620 7768 6963 6820 7769 6c6c 2062 6520  f which will be 
-00010380: 636f 6e76 6572 7465 642e 2044 6961 676f  converted. Diago
-00010390: 6e61 6c20 6e6f 6973 6520 6361 6e20 616c  nal noise can al
-000103a0: 736f 2062 6520 6164 6465 6420 746f 0a20  so be added to. 
-000103b0: 2020 2074 6865 2063 6f76 6172 6961 6e63     the covarianc
-000103c0: 6520 6d61 7472 6978 2c20 3a6d 6174 683a  e matrix, :math:
-000103d0: 604b 203d 204b 5f31 205c 6f74 696d 6573  `K = K_1 \otimes
-000103e0: 204b 5f32 202b 205c 7369 676d 615e 3220   K_2 + \sigma^2 
-000103f0: 495f 4e60 2e0a 2020 2020 4465 7370 6974  I_N`..    Despit
-00010400: 6520 7468 6520 6e6f 6973 6520 7265 6d6f  e the noise remo
-00010410: 7669 6e67 2074 6865 206f 7665 7261 6c6c  ving the overall
-00010420: 204b 726f 6e65 636b 6572 2073 7472 7563   Kronecker struc
-00010430: 7475 7265 206f 6620 7468 6520 6d61 7472  ture of the matr
-00010440: 6978 2c0a 2020 2020 604b 726f 6e65 636b  ix,.    `Kroneck
-00010450: 6572 4e6f 726d 616c 6020 6361 6e20 636f  erNormal` can co
-00010460: 6e74 696e 7565 2074 6f20 6d61 6b65 2065  ntinue to make e
-00010470: 6666 6963 6965 6e74 2063 616c 6375 6c61  fficient calcula
-00010480: 7469 6f6e 7320 6279 0a20 2020 2075 7469  tions by.    uti
-00010490: 6c69 7a69 6e67 2065 6967 656e 6465 636f  lizing eigendeco
-000104a0: 6d70 6f73 6974 6f6e 7320 6f66 2074 6865  mpositons of the
-000104b0: 2073 7562 6d61 7472 6963 6573 2062 6568   submatrices beh
-000104c0: 696e 6420 7468 6520 7363 656e 6573 205b  ind the scenes [
-000104d0: 315d 2e0a 2020 2020 5468 7573 2c0a 0a20  1]..    Thus,.. 
-000104e0: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
-000104f0: 686f 6e0a 0a20 2020 2020 2020 2073 6967  hon..        sig
-00010500: 6d61 203d 2030 2e31 0a20 2020 2020 2020  ma = 0.1.       
-00010510: 2077 6974 6820 706d 2e4d 6f64 656c 2829   with pm.Model()
-00010520: 2061 7320 6e6f 6973 655f 6d6f 6465 6c3a   as noise_model:
-00010530: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00010540: 7320 3d20 706d 2e4b 726f 6e65 636b 6572  s = pm.Kronecker
-00010550: 4e6f 726d 616c 2827 7661 6c73 272c 206d  Normal('vals', m
-00010560: 753d 6d75 2c20 636f 7673 3d63 6f76 732c  u=mu, covs=covs,
-00010570: 2073 6967 6d61 3d73 6967 6d61 2c20 7368   sigma=sigma, sh
-00010580: 6170 653d 4e29 0a20 2020 2020 2020 2020  ape=N).         
-00010590: 2020 2076 616c 7332 203d 2070 6d2e 4b72     vals2 = pm.Kr
-000105a0: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
-000105b0: 616c 7332 272c 206d 753d 6d75 2c20 6368  als2', mu=mu, ch
-000105c0: 6f6c 733d 6368 6f6c 732c 2073 6967 6d61  ols=chols, sigma
-000105d0: 3d73 6967 6d61 2c20 7368 6170 653d 4e29  =sigma, shape=N)
-000105e0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000105f0: 7333 203d 2070 6d2e 4b72 6f6e 6563 6b65  s3 = pm.Kronecke
-00010600: 724e 6f72 6d61 6c28 2776 616c 7333 272c  rNormal('vals3',
-00010610: 206d 753d 6d75 2c20 6576 6473 3d65 7664   mu=mu, evds=evd
-00010620: 732c 2073 6967 6d61 3d73 6967 6d61 2c20  s, sigma=sigma, 
-00010630: 7368 6170 653d 4e29 0a0a 2020 2020 6172  shape=N)..    ar
-00010640: 6520 6964 656e 7469 6361 6c2c 2077 6974  e identical, wit
-00010650: 6820 6063 6f76 7360 2061 6e64 2060 6368  h `covs` and `ch
-00010660: 6f6c 7360 2065 6163 6820 636f 6e76 6572  ols` each conver
-00010670: 7465 6420 746f 0a20 2020 2065 6967 656e  ted to.    eigen
-00010680: 6465 636f 6d70 6f73 6974 696f 6e73 2e0a  decompositions..
-00010690: 0a20 2020 2052 6566 6572 656e 6365 730a  .    References.
-000106a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000106b0: 2020 202e 2e20 5b31 5d20 5361 6174 6368     .. [1] Saatch
-000106c0: 692c 2059 2e20 2832 3031 3129 2e20 2253  i, Y. (2011). "S
-000106d0: 6361 6c61 626c 6520 696e 6665 7265 6e63  calable inferenc
-000106e0: 6520 666f 7220 7374 7275 6374 7572 6564  e for structured
-000106f0: 2047 6175 7373 6961 6e20 7072 6f63 6573   Gaussian proces
-00010700: 7320 6d6f 6465 6c73 220a 2020 2020 2222  s models".    ""
-00010710: 220a 2020 2020 7276 5f6f 7020 3d20 6b72  ".    rv_op = kr
-00010720: 6f6e 6563 6b65 726e 6f72 6d61 6c0a 0a20  oneckernormal.. 
-00010730: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00010740: 2020 2020 6465 6620 6469 7374 2863 6c73      def dist(cls
-00010750: 2c20 6d75 2c20 636f 7673 3d4e 6f6e 652c  , mu, covs=None,
-00010760: 2063 686f 6c73 3d4e 6f6e 652c 2065 7664   chols=None, evd
-00010770: 733d 4e6f 6e65 2c20 7369 676d 613d 4e6f  s=None, sigma=No
-00010780: 6e65 2c20 2a61 7267 732c 202a 2a6b 7761  ne, *args, **kwa
-00010790: 7267 7329 3a0a 2020 2020 2020 2020 6966  rgs):.        if
-000107a0: 206c 656e 285b 6920 666f 7220 6920 696e   len([i for i in
-000107b0: 205b 636f 7673 2c20 6368 6f6c 732c 2065   [covs, chols, e
-000107c0: 7664 735d 2069 6620 6920 6973 206e 6f74  vds] if i is not
-000107d0: 204e 6f6e 655d 2920 213d 2031 3a0a 2020   None]) != 1:.  
-000107e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000107f0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00010800: 2020 2020 2020 2020 2020 2020 2249 6e63              "Inc
-00010810: 6f6d 7061 7469 626c 6520 7061 7261 6d65  ompatible parame
-00010820: 7465 7269 7a61 7469 6f6e 2e20 5370 6563  terization. Spec
-00010830: 6966 7920 6578 6163 746c 7920 6f6e 6520  ify exactly one 
-00010840: 6f66 2063 6f76 732c 2063 686f 6c73 2c20  of covs, chols, 
-00010850: 6f72 2065 7664 732e 220a 2020 2020 2020  or evds.".      
-00010860: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00010870: 2073 6967 6d61 203d 2073 6967 6d61 2069   sigma = sigma i
-00010880: 6620 7369 676d 6120 656c 7365 2030 0a0a  f sigma else 0..
-00010890: 2020 2020 2020 2020 6966 2063 686f 6c73          if chols
-000108a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000108b0: 2020 2020 2020 2020 2020 636f 7673 203d            covs =
-000108c0: 205b 6368 6f6c 2e64 6f74 2863 686f 6c2e   [chol.dot(chol.
-000108d0: 5429 2066 6f72 2063 686f 6c20 696e 2063  T) for chol in c
-000108e0: 686f 6c73 5d0a 2020 2020 2020 2020 656c  hols].        el
-000108f0: 6966 2065 7664 7320 6973 206e 6f74 204e  if evds is not N
-00010900: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00010910: 2065 6967 685f 6974 6572 6162 6c65 203d   eigh_iterable =
-00010920: 2065 7664 730a 2020 2020 2020 2020 2020   evds.          
-00010930: 2020 636f 7673 203d 205b 5d0a 2020 2020    covs = [].    
-00010940: 2020 2020 2020 2020 6569 6773 5f73 6570          eigs_sep
-00010950: 2c20 5173 203d 207a 6970 282a 6569 6768  , Qs = zip(*eigh
-00010960: 5f69 7465 7261 626c 6529 2020 2320 556e  _iterable)  # Un
-00010970: 7a69 700a 2020 2020 2020 2020 2020 2020  zip.            
-00010980: 666f 7220 6569 672c 2051 2069 6e20 7a69  for eig, Q in zi
-00010990: 7028 6569 6773 5f73 6570 2c20 5173 293a  p(eigs_sep, Qs):
-000109a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000109b0: 2063 6f76 5f69 203d 2070 742e 646f 7428   cov_i = pt.dot(
-000109c0: 512c 2070 742e 646f 7428 7074 2e64 6961  Q, pt.dot(pt.dia
-000109d0: 6728 6569 6729 2c20 512e 5429 290a 2020  g(eig), Q.T)).  
-000109e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000109f0: 7673 2e61 7070 656e 6428 636f 765f 6929  vs.append(cov_i)
-00010a00: 0a0a 2020 2020 2020 2020 6d75 203d 2070  ..        mu = p
-00010a10: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00010a20: 6162 6c65 286d 7529 0a0a 2020 2020 2020  able(mu)..      
-00010a30: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00010a40: 2e64 6973 7428 5b6d 752c 2073 6967 6d61  .dist([mu, sigma
-00010a50: 2c20 2a63 6f76 735d 2c20 2a2a 6b77 6172  , *covs], **kwar
-00010a60: 6773 290a 0a20 2020 2064 6566 206d 6f6d  gs)..    def mom
-00010a70: 656e 7428 7276 2c20 7369 7a65 2c20 6d75  ent(rv, size, mu
-00010a80: 2c20 636f 7673 2c20 6368 6f6c 732c 2065  , covs, chols, e
-00010a90: 7664 7329 3a0a 2020 2020 2020 2020 6d65  vds):.        me
-00010aa0: 616e 203d 206d 750a 2020 2020 2020 2020  an = mu.        
-00010ab0: 6966 206e 6f74 2072 765f 7369 7a65 5f69  if not rv_size_i
-00010ac0: 735f 6e6f 6e65 2873 697a 6529 3a0a 2020  s_none(size):.  
-00010ad0: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
-00010ae0: 5f73 697a 6520 3d20 7074 2e63 6f6e 6361  _size = pt.conca
-00010af0: 7465 6e61 7465 285b 7369 7a65 2c20 6d75  tenate([size, mu
-00010b00: 2e73 6861 7065 5d29 0a20 2020 2020 2020  .shape]).       
-00010b10: 2020 2020 206d 6561 6e20 3d20 7074 2e66       mean = pt.f
-00010b20: 756c 6c28 6d6f 6d65 6e74 5f73 697a 652c  ull(moment_size,
-00010b30: 206d 7529 0a20 2020 2020 2020 2072 6574   mu).        ret
-00010b40: 7572 6e20 6d65 616e 0a0a 2020 2020 6465  urn mean..    de
-00010b50: 6620 6c6f 6770 2876 616c 7565 2c20 6d75  f logp(value, mu
-00010b60: 2c20 7369 676d 612c 202a 636f 7673 293a  , sigma, *covs):
-00010b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010b80: 2020 2020 2043 616c 6375 6c61 7465 206c       Calculate l
-00010b90: 6f67 2d70 726f 6261 6269 6c69 7479 206f  og-probability o
-00010ba0: 6620 4d75 6c74 6976 6172 6961 7465 204e  f Multivariate N
-00010bb0: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
-00010bc0: 6f6e 0a20 2020 2020 2020 2077 6974 6820  on.        with 
-00010bd0: 4b72 6f6e 6563 6b65 722d 7374 7275 6374  Kronecker-struct
-00010be0: 7572 6564 2063 6f76 6172 6961 6e63 6520  ured covariance 
-00010bf0: 6174 2073 7065 6369 6669 6564 2076 616c  at specified val
-00010c00: 7565 2e0a 0a20 2020 2020 2020 2050 6172  ue...        Par
-00010c10: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00010c20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00010c30: 2020 2076 616c 7565 3a20 6e75 6d65 7269     value: numeri
-00010c40: 630a 2020 2020 2020 2020 2020 2020 5661  c.            Va
-00010c50: 6c75 6520 666f 7220 7768 6963 6820 6c6f  lue for which lo
-00010c60: 672d 7072 6f62 6162 696c 6974 7920 6973  g-probability is
-00010c70: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
-00010c80: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00010c90: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00010ca0: 2020 2020 2020 5465 6e73 6f72 5661 7269        TensorVari
-00010cb0: 6162 6c65 0a20 2020 2020 2020 2022 2222  able.        """
-00010cc0: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
-00010cd0: 7465 7320 7468 6520 7175 6164 7261 7469  tes the quadrati
-00010ce0: 6320 2878 2d6d 7529 5e54 2040 204b 5e2d  c (x-mu)^T @ K^-
-00010cf0: 3120 4020 2878 2d6d 7529 2061 6e64 206c  1 @ (x-mu) and l
-00010d00: 6f67 2864 6574 284b 2929 0a20 2020 2020  og(det(K)).     
-00010d10: 2020 2069 6620 7661 6c75 652e 6e64 696d     if value.ndim
-00010d20: 203e 2032 206f 7220 7661 6c75 652e 6e64   > 2 or value.nd
-00010d30: 696d 203d 3d20 303a 0a20 2020 2020 2020  im == 0:.       
-00010d40: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00010d50: 4572 726f 7228 6622 496e 7661 6c69 6420  Error(f"Invalid 
-00010d60: 6469 6d65 6e73 696f 6e20 666f 7220 7661  dimension for va
-00010d70: 6c75 653a 207b 7661 6c75 652e 6e64 696d  lue: {value.ndim
-00010d80: 7d22 290a 2020 2020 2020 2020 6966 2076  }").        if v
-00010d90: 616c 7565 2e6e 6469 6d20 3d3d 2031 3a0a  alue.ndim == 1:.
-00010da0: 2020 2020 2020 2020 2020 2020 6f6e 6564              oned
-00010db0: 696d 203d 2054 7275 650a 2020 2020 2020  im = True.      
-00010dc0: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
-00010dd0: 6c75 655b 4e6f 6e65 2c20 3a5d 0a20 2020  lue[None, :].   
-00010de0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010df0: 2020 2020 2020 206f 6e65 6469 6d20 3d20         onedim = 
-00010e00: 4661 6c73 650a 0a20 2020 2020 2020 2064  False..        d
-00010e10: 656c 7461 203d 2076 616c 7565 202d 206d  elta = value - m
-00010e20: 750a 0a20 2020 2020 2020 2065 6967 685f  u..        eigh_
-00010e30: 6974 6572 6162 6c65 203d 206d 6170 2865  iterable = map(e
-00010e40: 6967 682c 2063 6f76 7329 0a20 2020 2020  igh, covs).     
-00010e50: 2020 2065 6967 735f 7365 702c 2051 7320     eigs_sep, Qs 
-00010e60: 3d20 7a69 7028 2a65 6967 685f 6974 6572  = zip(*eigh_iter
-00010e70: 6162 6c65 2920 2023 2055 6e7a 6970 0a20  able)  # Unzip. 
-00010e80: 2020 2020 2020 2051 7320 3d20 6c69 7374         Qs = list
-00010e90: 286d 6170 2870 742e 6173 5f74 656e 736f  (map(pt.as_tenso
-00010ea0: 725f 7661 7269 6162 6c65 2c20 5173 2929  r_variable, Qs))
-00010eb0: 0a20 2020 2020 2020 2051 5473 203d 206c  .        QTs = l
-00010ec0: 6973 7428 6d61 7028 7074 2e74 7261 6e73  ist(map(pt.trans
-00010ed0: 706f 7365 2c20 5173 2929 0a0a 2020 2020  pose, Qs))..    
-00010ee0: 2020 2020 6569 6773 5f73 6570 203d 206c      eigs_sep = l
-00010ef0: 6973 7428 6d61 7028 7074 2e61 735f 7465  ist(map(pt.as_te
-00010f00: 6e73 6f72 5f76 6172 6961 626c 652c 2065  nsor_variable, e
-00010f10: 6967 735f 7365 7029 290a 2020 2020 2020  igs_sep)).      
-00010f20: 2020 6569 6773 203d 206b 726f 6e5f 6469    eigs = kron_di
-00010f30: 6167 282a 6569 6773 5f73 6570 2920 2023  ag(*eigs_sep)  #
-00010f40: 2043 6f6d 6269 6e65 2073 6570 6172 6174   Combine separat
-00010f50: 6520 6569 6773 0a20 2020 2020 2020 2065  e eigs.        e
-00010f60: 6967 7320 2b3d 2073 6967 6d61 2a2a 320a  igs += sigma**2.
-00010f70: 2020 2020 2020 2020 4e20 3d20 6569 6773          N = eigs
-00010f80: 2e73 6861 7065 5b30 5d0a 0a20 2020 2020  .shape[0]..     
-00010f90: 2020 2073 7172 745f 7175 6164 203d 206b     sqrt_quad = k
-00010fa0: 726f 6e5f 646f 7428 5154 732c 2064 656c  ron_dot(QTs, del
-00010fb0: 7461 2e54 290a 2020 2020 2020 2020 7371  ta.T).        sq
-00010fc0: 7274 5f71 7561 6420 3d20 7371 7274 5f71  rt_quad = sqrt_q
-00010fd0: 7561 6420 2f20 7074 2e73 7172 7428 6569  uad / pt.sqrt(ei
-00010fe0: 6773 5b3a 2c20 4e6f 6e65 5d29 0a20 2020  gs[:, None]).   
-00010ff0: 2020 2020 206c 6f67 6465 7420 3d20 7074       logdet = pt
-00011000: 2e73 756d 2870 742e 6c6f 6728 6569 6773  .sum(pt.log(eigs
-00011010: 2929 0a0a 2020 2020 2020 2020 2320 5371  ))..        # Sq
-00011020: 7561 7265 2065 6163 6820 7361 6d70 6c65  uare each sample
-00011030: 0a20 2020 2020 2020 2071 7561 6420 3d20  .        quad = 
-00011040: 7074 2e62 6174 6368 6564 5f64 6f74 2873  pt.batched_dot(s
-00011050: 7172 745f 7175 6164 2e54 2c20 7371 7274  qrt_quad.T, sqrt
-00011060: 5f71 7561 642e 5429 0a20 2020 2020 2020  _quad.T).       
-00011070: 2069 6620 6f6e 6564 696d 3a0a 2020 2020   if onedim:.    
-00011080: 2020 2020 2020 2020 7175 6164 203d 2071          quad = q
-00011090: 7561 645b 305d 0a0a 2020 2020 2020 2020  uad[0]..        
-000110a0: 6120 3d20 2d28 7175 6164 202b 206c 6f67  a = -(quad + log
-000110b0: 6465 7420 2b20 4e20 2a20 7074 2e6c 6f67  det + N * pt.log
-000110c0: 2832 202a 206e 702e 7069 2929 202f 2032  (2 * np.pi)) / 2
-000110d0: 2e30 0a20 2020 2020 2020 2072 6574 7572  .0.        retur
-000110e0: 6e20 610a 0a0a 636c 6173 7320 4341 5252  n a...class CARR
-000110f0: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
-00011100: 293a 0a20 2020 206e 616d 6520 3d20 2263  ):.    name = "c
-00011110: 6172 220a 2020 2020 6e64 696d 5f73 7570  ar".    ndim_sup
-00011120: 7020 3d20 310a 2020 2020 6e64 696d 735f  p = 1.    ndims_
-00011130: 7061 7261 6d73 203d 205b 312c 2032 2c20  params = [1, 2, 
-00011140: 302c 2030 5d0a 2020 2020 6474 7970 6520  0, 0].    dtype 
-00011150: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
-00011160: 7072 696e 745f 6e61 6d65 203d 2028 2243  print_name = ("C
-00011170: 4152 222c 2022 5c5c 6f70 6572 6174 6f72  AR", "\\operator
-00011180: 6e61 6d65 7b43 4152 7d22 290a 0a20 2020  name{CAR}")..   
-00011190: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
-000111a0: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
-000111b0: 6474 7970 652c 206d 752c 2057 2c20 616c  dtype, mu, W, al
-000111c0: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
-000111d0: 2020 206d 7520 3d20 7074 2e61 735f 7465     mu = pt.as_te
-000111e0: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
-000111f0: 6f61 7458 286d 7529 290a 0a20 2020 2020  oatX(mu))..     
-00011200: 2020 2057 203d 2070 7974 656e 736f 722e     W = pytensor.
-00011210: 7370 6172 7365 2e61 735f 7370 6172 7365  sparse.as_sparse
-00011220: 5f6f 725f 7465 6e73 6f72 5f76 6172 6961  _or_tensor_varia
-00011230: 626c 6528 666c 6f61 7458 2857 2929 0a20  ble(floatX(W)). 
-00011240: 2020 2020 2020 2069 6620 6e6f 7420 572e         if not W.
-00011250: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
-00011260: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00011270: 7565 4572 726f 7228 2257 206d 7573 7420  ueError("W must 
-00011280: 6265 2061 206d 6174 7269 7820 286e 6469  be a matrix (ndi
-00011290: 6d3d 3229 2e22 290a 0a20 2020 2020 2020  m=2).")..       
-000112a0: 2073 7061 7273 6520 3d20 6973 696e 7374   sparse = isinst
-000112b0: 616e 6365 2857 2c20 7079 7465 6e73 6f72  ance(W, pytensor
-000112c0: 2e73 7061 7273 652e 5370 6172 7365 5661  .sparse.SparseVa
-000112d0: 7269 6162 6c65 290a 2020 2020 2020 2020  riable).        
-000112e0: 6d73 6720 3d20 2257 206d 7573 7420 6265  msg = "W must be
-000112f0: 2061 2073 796d 6d65 7472 6963 2061 646a   a symmetric adj
-00011300: 6163 656e 6379 206d 6174 7269 782e 220a  acency matrix.".
-00011310: 2020 2020 2020 2020 6966 2073 7061 7273          if spars
-00011320: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-00011330: 6273 5f64 6966 6620 3d20 7079 7465 6e73  bs_diff = pytens
-00011340: 6f72 2e73 7061 7273 652e 6261 7369 632e  or.sparse.basic.
-00011350: 6d75 6c28 7079 7465 6e73 6f72 2e73 7061  mul(pytensor.spa
-00011360: 7273 652e 7369 676e 2857 202d 2057 2e54  rse.sign(W - W.T
-00011370: 292c 2057 202d 2057 2e54 290a 2020 2020  ), W - W.T).    
-00011380: 2020 2020 2020 2020 5720 3d20 4173 7365          W = Asse
-00011390: 7274 286d 7367 2928 572c 2070 742e 6973  rt(msg)(W, pt.is
-000113a0: 636c 6f73 6528 7079 7465 6e73 6f72 2e73  close(pytensor.s
-000113b0: 7061 7273 652e 7370 5f73 756d 2861 6273  parse.sp_sum(abs
-000113c0: 5f64 6966 6629 2c20 3029 290a 2020 2020  _diff), 0)).    
-000113d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000113e0: 2020 2020 2020 5720 3d20 4173 7365 7274        W = Assert
-000113f0: 286d 7367 2928 572c 2070 742e 616c 6c63  (msg)(W, pt.allc
-00011400: 6c6f 7365 2857 2c20 572e 5429 290a 0a20  lose(W, W.T)).. 
-00011410: 2020 2020 2020 2074 6175 203d 2070 742e         tau = pt.
-00011420: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-00011430: 6c65 2866 6c6f 6174 5828 7461 7529 290a  le(floatX(tau)).
-00011440: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
-00011450: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-00011460: 6961 626c 6528 666c 6f61 7458 2861 6c70  iable(floatX(alp
-00011470: 6861 2929 0a0a 2020 2020 2020 2020 7265  ha))..        re
-00011480: 7475 726e 2073 7570 6572 2829 2e6d 616b  turn super().mak
-00011490: 655f 6e6f 6465 2872 6e67 2c20 7369 7a65  e_node(rng, size
-000114a0: 2c20 6474 7970 652c 206d 752c 2057 2c20  , dtype, mu, W, 
-000114b0: 616c 7068 612c 2074 6175 290a 0a20 2020  alpha, tau)..   
-000114c0: 2064 6566 205f 696e 6665 725f 7368 6170   def _infer_shap
-000114d0: 6528 7365 6c66 2c20 7369 7a65 2c20 6469  e(self, size, di
-000114e0: 7374 5f70 6172 616d 732c 2070 6172 616d  st_params, param
-000114f0: 5f73 6861 7065 733d 4e6f 6e65 293a 0a20  _shapes=None):. 
-00011500: 2020 2020 2020 2073 6861 7065 203d 2074         shape = t
-00011510: 7570 6c65 2873 697a 6529 202b 2028 6469  uple(size) + (di
-00011520: 7374 5f70 6172 616d 735b 305d 2e73 6861  st_params[0].sha
-00011530: 7065 5b2d 315d 2c29 0a20 2020 2020 2020  pe[-1],).       
-00011540: 2072 6574 7572 6e20 7368 6170 650a 0a20   return shape.. 
-00011550: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00011560: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
-00011570: 6c73 2c20 726e 673a 206e 702e 7261 6e64  ls, rng: np.rand
-00011580: 6f6d 2e52 616e 646f 6d53 7461 7465 2c20  om.RandomState, 
-00011590: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
-000115a0: 752c 2073 697a 6529 3a0a 2020 2020 2020  u, size):.      
-000115b0: 2020 2222 220a 2020 2020 2020 2020 496d    """.        Im
-000115c0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-000115d0: 616c 676f 7269 7468 6d20 6672 6f6d 2070  algorithm from p
-000115e0: 6170 6572 0a20 2020 2020 2020 2048 6176  aper.        Hav
-000115f0: 6172 6420 5275 652c 2032 3030 312e 2022  ard Rue, 2001. "
-00011600: 4661 7374 2073 616d 706c 696e 6720 6f66  Fast sampling of
-00011610: 2047 6175 7373 6961 6e20 4d61 726b 6f76   Gaussian Markov
-00011620: 2072 616e 646f 6d20 6669 656c 6473 2c22   random fields,"
-00011630: 0a20 2020 2020 2020 204a 6f75 726e 616c  .        Journal
-00011640: 206f 6620 7468 6520 526f 7961 6c20 5374   of the Royal St
-00011650: 6174 6973 7469 6361 6c20 536f 6369 6574  atistical Societ
-00011660: 7920 5365 7269 6573 2042 2c20 526f 7961  y Series B, Roya
-00011670: 6c20 5374 6174 6973 7469 6361 6c20 536f  l Statistical So
-00011680: 6369 6574 792c 0a20 2020 2020 2020 2076  ciety,.        v
-00011690: 6f6c 2e20 3633 2832 292c 2070 6167 6573  ol. 63(2), pages
-000116a0: 2033 3235 2d33 3338 2e20 444f 493a 2031   325-338. DOI: 1
-000116b0: 302e 3131 3131 2f31 3436 372d 3938 3638  0.1111/1467-9868
-000116c0: 2e30 3032 3838 0a20 2020 2020 2020 2022  .00288.        "
-000116d0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000116e0: 7420 7363 6970 792e 7370 6172 7365 2e69  t scipy.sparse.i
-000116f0: 7373 7061 7273 6528 5729 3a0a 2020 2020  ssparse(W):.    
-00011700: 2020 2020 2020 2020 5720 3d20 7363 6970          W = scip
-00011710: 792e 7370 6172 7365 2e63 7372 5f6d 6174  y.sparse.csr_mat
-00011720: 7269 7828 5729 0a20 2020 2020 2020 2073  rix(W).        s
-00011730: 203d 206e 702e 6173 6172 7261 7928 572e   = np.asarray(W.
-00011740: 7375 6d28 6178 6973 3d30 2929 5b30 5d0a  sum(axis=0))[0].
-00011750: 2020 2020 2020 2020 4420 3d20 7363 6970          D = scip
-00011760: 792e 7370 6172 7365 2e64 6961 6773 2873  y.sparse.diags(s
-00011770: 290a 2020 2020 2020 2020 7461 7520 3d20  ).        tau = 
-00011780: 7363 6970 792e 7370 6172 7365 2e63 7372  scipy.sparse.csr
-00011790: 5f6d 6174 7269 7828 7461 7529 0a20 2020  _matrix(tau).   
-000117a0: 2020 2020 2061 6c70 6861 203d 2073 6369       alpha = sci
-000117b0: 7079 2e73 7061 7273 652e 6373 725f 6d61  py.sparse.csr_ma
-000117c0: 7472 6978 2861 6c70 6861 290a 0a20 2020  trix(alpha)..   
-000117d0: 2020 2020 2051 203d 2074 6175 2e6d 756c       Q = tau.mul
-000117e0: 7469 706c 7928 4420 2d20 616c 7068 612e  tiply(D - alpha.
-000117f0: 6d75 6c74 6970 6c79 2857 2929 0a0a 2020  multiply(W))..  
-00011800: 2020 2020 2020 7065 726d 5f61 7272 6179        perm_array
-00011810: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
-00011820: 6373 6772 6170 682e 7265 7665 7273 655f  csgraph.reverse_
-00011830: 6375 7468 696c 6c5f 6d63 6b65 6528 512c  cuthill_mckee(Q,
-00011840: 2073 796d 6d65 7472 6963 5f6d 6f64 653d   symmetric_mode=
-00011850: 5472 7565 290a 2020 2020 2020 2020 696e  True).        in
-00011860: 765f 7065 726d 203d 206e 702e 6172 6773  v_perm = np.args
-00011870: 6f72 7428 7065 726d 5f61 7272 6179 290a  ort(perm_array).
-00011880: 0a20 2020 2020 2020 2051 203d 2051 5b70  .        Q = Q[p
-00011890: 6572 6d5f 6172 7261 792c 203a 5d5b 3a2c  erm_array, :][:,
-000118a0: 2070 6572 6d5f 6172 7261 795d 0a0a 2020   perm_array]..  
-000118b0: 2020 2020 2020 5162 203d 2051 2e64 6961        Qb = Q.dia
-000118c0: 676f 6e61 6c28 290a 2020 2020 2020 2020  gonal().        
-000118d0: 7520 3d20 310a 2020 2020 2020 2020 7768  u = 1.        wh
-000118e0: 696c 6520 6e70 2e63 6f75 6e74 5f6e 6f6e  ile np.count_non
-000118f0: 7a65 726f 2851 2e64 6961 676f 6e61 6c28  zero(Q.diagonal(
-00011900: 7529 2920 3e20 303a 0a20 2020 2020 2020  u)) > 0:.       
-00011910: 2020 2020 2051 6220 3d20 6e70 2e76 7374       Qb = np.vst
-00011920: 6163 6b28 286e 702e 7061 6428 512e 6469  ack((np.pad(Q.di
-00011930: 6167 6f6e 616c 2875 292c 2028 752c 2030  agonal(u), (u, 0
-00011940: 292c 2063 6f6e 7374 616e 745f 7661 6c75  ), constant_valu
-00011950: 6573 3d28 302c 2030 2929 2c20 5162 2929  es=(0, 0)), Qb))
-00011960: 0a20 2020 2020 2020 2020 2020 2075 202b  .            u +
-00011970: 3d20 310a 0a20 2020 2020 2020 204c 203d  = 1..        L =
-00011980: 2073 6369 7079 2e6c 696e 616c 672e 6368   scipy.linalg.ch
-00011990: 6f6c 6573 6b79 5f62 616e 6465 6428 5162  olesky_banded(Qb
-000119a0: 2c20 6c6f 7765 723d 4661 6c73 6529 0a0a  , lower=False)..
-000119b0: 2020 2020 2020 2020 7369 7a65 203d 2074          size = t
-000119c0: 7570 6c65 2873 697a 6520 6f72 2028 2929  uple(size or ())
-000119d0: 0a20 2020 2020 2020 2069 6620 7369 7a65  .        if size
-000119e0: 3a0a 2020 2020 2020 2020 2020 2020 6d75  :.            mu
-000119f0: 203d 206e 702e 6272 6f61 6463 6173 745f   = np.broadcast_
-00011a00: 746f 286d 752c 2073 697a 6520 2b20 286d  to(mu, size + (m
-00011a10: 752e 7368 6170 655b 2d31 5d2c 2929 0a20  u.shape[-1],)). 
-00011a20: 2020 2020 2020 207a 203d 2072 6e67 2e6e         z = rng.n
-00011a30: 6f72 6d61 6c28 7369 7a65 3d6d 752e 7368  ormal(size=mu.sh
-00011a40: 6170 6529 0a20 2020 2020 2020 2073 616d  ape).        sam
-00011a50: 706c 6573 203d 206e 702e 656d 7074 7928  ples = np.empty(
-00011a60: 7a2e 7368 6170 6529 0a20 2020 2020 2020  z.shape).       
-00011a70: 2066 6f72 2069 6478 2069 6e20 6e70 2e6e   for idx in np.n
-00011a80: 6469 6e64 6578 286d 752e 7368 6170 655b  dindex(mu.shape[
-00011a90: 3a2d 315d 293a 0a20 2020 2020 2020 2020  :-1]):.         
-00011aa0: 2020 2073 616d 706c 6573 5b69 6478 5d20     samples[idx] 
-00011ab0: 3d20 7363 6970 792e 6c69 6e61 6c67 2e63  = scipy.linalg.c
-00011ac0: 686f 5f73 6f6c 7665 5f62 616e 6465 6428  ho_solve_banded(
-00011ad0: 284c 2c20 4661 6c73 6529 2c20 7a5b 6964  (L, False), z[id
-00011ae0: 785d 2920 2b20 6d75 5b69 6478 5d5b 7065  x]) + mu[idx][pe
-00011af0: 726d 5f61 7272 6179 5d0a 2020 2020 2020  rm_array].      
-00011b00: 2020 7361 6d70 6c65 7320 3d20 7361 6d70    samples = samp
-00011b10: 6c65 735b 2e2e 2e2c 2069 6e76 5f70 6572  les[..., inv_per
-00011b20: 6d5d 0a20 2020 2020 2020 2072 6574 7572  m].        retur
-00011b30: 6e20 7361 6d70 6c65 730a 0a0a 6361 7220  n samples...car 
-00011b40: 3d20 4341 5252 5628 290a 0a0a 636c 6173  = CARRV()...clas
-00011b50: 7320 4341 5228 436f 6e74 696e 756f 7573  s CAR(Continuous
-00011b60: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
-00011b70: 4c69 6b65 6c69 686f 6f64 2066 6f72 2061  Likelihood for a
-00011b80: 2063 6f6e 6469 7469 6f6e 616c 2061 7574   conditional aut
-00011b90: 6f72 6567 7265 7373 696f 6e2e 2054 6869  oregression. Thi
-00011ba0: 7320 6973 2061 2073 7065 6369 616c 2063  s is a special c
-00011bb0: 6173 6520 6f66 2074 6865 0a20 2020 206d  ase of the.    m
-00011bc0: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
-00011bd0: 616c 2077 6974 6820 616e 2061 646a 6163  al with an adjac
-00011be0: 656e 6379 2d73 7472 7563 7475 7265 6420  ency-structured 
-00011bf0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00011c00: 782e 0a0a 2020 2020 2e2e 206d 6174 683a  x...    .. math:
-00011c10: 3a0a 0a20 2020 2020 2020 6628 7820 5c6d  :..       f(x \m
-00011c20: 6964 2057 2c20 5c61 6c70 6861 2c20 5c74  id W, \alpha, \t
-00011c30: 6175 2920 3d0a 2020 2020 2020 2020 2020  au) =.          
-00011c40: 205c 6672 6163 7b7c 547c 5e7b 312f 327d   \frac{|T|^{1/2}
-00011c50: 7d7b 2832 5c70 6929 5e7b 6b2f 327d 7d0a  }{(2\pi)^{k/2}}.
-00011c60: 2020 2020 2020 2020 2020 205c 6578 705c             \exp\
-00011c70: 6c65 6674 5c7b 202d 5c66 7261 637b 317d  left\{ -\frac{1}
-00011c80: 7b32 7d20 2878 2d5c 6d75 295e 7b5c 7072  {2} (x-\mu)^{\pr
-00011c90: 696d 657d 2054 5e7b 2d31 7d20 2878 2d5c  ime} T^{-1} (x-\
-00011ca0: 6d75 2920 5c72 6967 6874 5c7d 0a0a 2020  mu) \right\}..  
-00011cb0: 2020 7768 6572 6520 3a6d 6174 683a 6054    where :math:`T
-00011cc0: 203d 2028 5c74 6175 2044 2849 2d5c 616c   = (\tau D(I-\al
-00011cd0: 7068 6120 5729 295e 7b2d 317d 6020 616e  pha W))^{-1}` an
-00011ce0: 6420 3a6d 6174 683a 6044 203d 2064 6961  d :math:`D = dia
-00011cf0: 6728 5c73 756d 5f69 2057 5f7b 696a 7d29  g(\sum_i W_{ij})
-00011d00: 602e 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  `...    ========
-00011d10: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
-00011d20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
-00011d30: 2053 7570 706f 7274 2020 203a 6d61 7468   Support   :math
-00011d40: 3a60 7820 5c69 6e20 5c6d 6174 6862 627b  :`x \in \mathbb{
-00011d50: 527d 5e6b 600a 2020 2020 4d65 616e 2020  R}^k`.    Mean  
-00011d60: 2020 2020 3a6d 6174 683a 605c 6d75 205c      :math:`\mu \
-00011d70: 696e 205c 6d61 7468 6262 7b52 7d5e 6b60  in \mathbb{R}^k`
-00011d80: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
-00011d90: 6d61 7468 3a60 285c 7461 7520 4428 492d  math:`(\tau D(I-
-00011da0: 5c61 6c70 6861 2057 2929 5e7b 2d31 7d60  \alpha W))^{-1}`
-00011db0: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
-00011dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011dd0: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050  =========..    P
-00011de0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00011df0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d 7520  --------.    mu 
-00011e00: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
-00011e10: 2066 6c6f 6174 0a20 2020 2020 2020 2052   float.        R
-00011e20: 6561 6c2d 7661 6c75 6564 206d 6561 6e20  eal-valued mean 
-00011e30: 7665 6374 6f72 0a20 2020 2057 203a 2028  vector.    W : (
-00011e40: 4d2c 204d 2920 7465 6e73 6f72 5f6c 696b  M, M) tensor_lik
-00011e50: 6520 6f66 2069 6e74 0a20 2020 2020 2020  e of int.       
-00011e60: 2053 796d 6d65 7472 6963 2061 646a 6163   Symmetric adjac
-00011e70: 656e 6379 206d 6174 7269 7820 6f66 2031  ency matrix of 1
-00011e80: 7320 616e 6420 3073 2069 6e64 6963 6174  s and 0s indicat
-00011e90: 696e 670a 2020 2020 2020 2020 6164 6a61  ing.        adja
-00011ea0: 6365 6e63 7920 6265 7477 6565 6e20 656c  cency between el
-00011eb0: 656d 656e 7473 2e20 4966 2070 6f73 7369  ements. If possi
-00011ec0: 626c 652c 202a 572a 2069 7320 636f 6e76  ble, *W* is conv
-00011ed0: 6572 7465 640a 2020 2020 2020 2020 746f  erted.        to
-00011ee0: 2061 2073 7061 7273 6520 6d61 7472 6978   a sparse matrix
-00011ef0: 2c20 6661 6c6c 696e 6720 6261 636b 2074  , falling back t
-00011f00: 6f20 6120 6465 6e73 6520 7661 7269 6162  o a dense variab
-00011f10: 6c65 2e0a 2020 2020 2020 2020 3a66 756e  le..        :fun
-00011f20: 633a 607e 7079 7465 6e73 6f72 2e73 7061  c:`~pytensor.spa
-00011f30: 7273 652e 6261 7369 632e 6173 5f73 7061  rse.basic.as_spa
-00011f40: 7273 655f 6f72 5f74 656e 736f 725f 7661  rse_or_tensor_va
-00011f50: 7269 6162 6c65 6020 6973 0a20 2020 2020  riable` is.     
-00011f60: 2020 2075 7365 6420 666f 7220 7468 6973     used for this
-00011f70: 2073 7061 7273 6520 6f72 2074 656e 736f   sparse or tenso
-00011f80: 7276 6172 6961 626c 6520 636f 6e76 6572  rvariable conver
-00011f90: 7369 6f6e 2e0a 2020 2020 616c 7068 6120  sion..    alpha 
-00011fa0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
-00011fb0: 2066 6c6f 6174 0a20 2020 2020 2020 2041   float.        A
-00011fc0: 7574 6f72 6567 7265 7373 696f 6e20 7061  utoregression pa
-00011fd0: 7261 6d65 7465 7220 7461 6b69 6e67 2076  rameter taking v
-00011fe0: 616c 7565 7320 6265 7477 6565 6e20 2d31  alues between -1
-00011ff0: 2061 6e64 2031 2e20 5661 6c75 6573 2063   and 1. Values c
-00012000: 6c6f 7365 7220 746f 2030 2069 6e64 6963  loser to 0 indic
-00012010: 6174 6520 7765 616b 6572 0a20 2020 2020  ate weaker.     
-00012020: 2020 2063 6f72 7265 6c61 7469 6f6e 2061     correlation a
-00012030: 6e64 2076 616c 7565 7320 636c 6f73 6572  nd values closer
-00012040: 2074 6f20 3120 696e 6469 6361 7465 2068   to 1 indicate h
-00012050: 6967 6865 7220 6175 746f 636f 7272 656c  igher autocorrel
-00012060: 6174 696f 6e2e 2046 6f72 206d 6f73 7420  ation. For most 
-00012070: 7573 6520 6361 7365 732c 2074 6865 0a20  use cases, the. 
-00012080: 2020 2020 2020 2073 7570 706f 7274 206f         support o
-00012090: 6620 616c 7068 6120 7368 6f75 6c64 2062  f alpha should b
-000120a0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-000120b0: 2830 2c20 3129 2e0a 2020 2020 7461 7520  (0, 1)..    tau 
-000120c0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
-000120d0: 2066 6c6f 6174 0a20 2020 2020 2020 2050   float.        P
-000120e0: 6f73 6974 6976 6520 7072 6563 6973 696f  ositive precisio
-000120f0: 6e20 7661 7269 6162 6c65 2063 6f6e 7472  n variable contr
-00012100: 6f6c 6c69 6e67 2074 6865 2073 6361 6c65  olling the scale
-00012110: 206f 6620 7468 6520 756e 6465 726c 7969   of the underlyi
-00012120: 6e67 206e 6f72 6d61 6c20 7661 7269 6174  ng normal variat
-00012130: 6573 2e0a 0a20 2020 2052 6566 6572 656e  es...    Referen
-00012140: 6365 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ces.    --------
-00012150: 2d2d 0a20 2020 202e 2e20 204a 696e 2c20  --.    ..  Jin, 
-00012160: 582e 2c20 4361 726c 696e 2c20 422e 2c20  X., Carlin, B., 
-00012170: 4261 6e65 726a 6565 2c20 532e 0a20 2020  Banerjee, S..   
-00012180: 2020 2020 2022 4765 6e65 7261 6c69 7a65       "Generalize
-00012190: 6420 4869 6572 6172 6368 6963 616c 204d  d Hierarchical M
-000121a0: 756c 7469 7661 7269 6174 6520 4341 5220  ultivariate CAR 
-000121b0: 4d6f 6465 6c73 2066 6f72 2041 7265 616c  Models for Areal
-000121c0: 2044 6174 6122 0a20 2020 2020 2020 2042   Data".        B
-000121d0: 696f 6d65 7472 6963 732c 2056 6f6c 2e20  iometrics, Vol. 
-000121e0: 3631 2c20 4e6f 2e20 3420 2844 6563 2e2c  61, No. 4 (Dec.,
-000121f0: 2032 3030 3529 2c20 7070 2e20 3935 302d   2005), pp. 950-
-00012200: 3936 310a 2020 2020 2222 220a 2020 2020  961.    """.    
-00012210: 7276 5f6f 7020 3d20 6361 720a 0a20 2020  rv_op = car..   
-00012220: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00012230: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
-00012240: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
-00012250: 752c 202a 6172 6773 2c20 2a2a 6b77 6172  u, *args, **kwar
-00012260: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
-00012270: 7572 6e20 7375 7065 7228 292e 6469 7374  urn super().dist
-00012280: 285b 6d75 2c20 572c 2061 6c70 6861 2c20  ([mu, W, alpha, 
-00012290: 7461 755d 2c20 2a2a 6b77 6172 6773 290a  tau], **kwargs).
-000122a0: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
-000122b0: 7276 2c20 7369 7a65 2c20 6d75 2c20 572c  rv, size, mu, W,
-000122c0: 2061 6c70 6861 2c20 7461 7529 3a0a 2020   alpha, tau):.  
-000122d0: 2020 2020 2020 7265 7475 726e 2070 742e        return pt.
-000122e0: 6675 6c6c 5f6c 696b 6528 7276 2c20 6d75  full_like(rv, mu
-000122f0: 290a 0a20 2020 2064 6566 206c 6f67 7028  )..    def logp(
-00012300: 7661 6c75 652c 206d 752c 2057 2c20 616c  value, mu, W, al
-00012310: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
-00012320: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00012330: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
-00012340: 6261 6269 6c69 7479 206f 6620 6120 4341  bability of a CA
-00012350: 522d 6469 7374 7269 6275 7465 6420 7665  R-distributed ve
-00012360: 6374 6f72 0a20 2020 2020 2020 2061 7420  ctor.        at 
-00012370: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
-00012380: 2054 6869 7320 6c6f 6720 7072 6f62 6162   This log probab
-00012390: 696c 6974 7920 6675 6e63 7469 6f6e 2064  ility function d
-000123a0: 6966 6665 7273 2066 726f 6d0a 2020 2020  iffers from.    
-000123b0: 2020 2020 7468 6520 7472 7565 2043 4152      the true CAR
-000123c0: 206c 6f67 2064 656e 7369 7479 2028 414b   log density (AK
-000123d0: 4120 6120 6d75 6c74 6976 6172 6961 7465  A a multivariate
-000123e0: 206e 6f72 6d61 6c20 7769 7468 2043 4152   normal with CAR
-000123f0: 2d73 7472 7563 7475 7265 640a 2020 2020  -structured.    
-00012400: 2020 2020 636f 7661 7269 616e 6365 206d      covariance m
-00012410: 6174 7269 7829 2062 7920 616e 2061 6464  atrix) by an add
-00012420: 6974 6976 6520 636f 6e73 7461 6e74 2e0a  itive constant..
-00012430: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00012440: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00012450: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
-00012460: 616c 7565 3a20 6172 7261 790a 2020 2020  alue: array.    
-00012470: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
-00012480: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
-00012490: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
-000124a0: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
-000124b0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-000124c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000124d0: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
-000124e0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000124f0: 2020 2020 7370 6172 7365 203d 2069 7369      sparse = isi
-00012500: 6e73 7461 6e63 6528 572c 2028 7079 7465  nstance(W, (pyte
-00012510: 6e73 6f72 2e73 7061 7273 652e 5370 6172  nsor.sparse.Spar
-00012520: 7365 436f 6e73 7461 6e74 2c20 7079 7465  seConstant, pyte
-00012530: 6e73 6f72 2e73 7061 7273 652e 5370 6172  nsor.sparse.Spar
-00012540: 7365 5661 7269 6162 6c65 2929 0a0a 2020  seVariable))..  
-00012550: 2020 2020 2020 6966 2073 7061 7273 653a        if sparse:
-00012560: 0a20 2020 2020 2020 2020 2020 2044 203d  .            D =
-00012570: 2073 705f 7375 6d28 572c 2061 7869 733d   sp_sum(W, axis=
-00012580: 3029 0a20 2020 2020 2020 2020 2020 2044  0).            D
-00012590: 696e 765f 7371 7274 203d 2070 742e 6469  inv_sqrt = pt.di
-000125a0: 6167 2831 202f 2070 742e 7371 7274 2844  ag(1 / pt.sqrt(D
-000125b0: 2929 0a20 2020 2020 2020 2020 2020 2044  )).            D
-000125c0: 5744 203d 2070 742e 646f 7428 7079 7465  WD = pt.dot(pyte
-000125d0: 6e73 6f72 2e73 7061 7273 652e 646f 7428  nsor.sparse.dot(
-000125e0: 4469 6e76 5f73 7172 742c 2057 292c 2044  Dinv_sqrt, W), D
-000125f0: 696e 765f 7371 7274 290a 2020 2020 2020  inv_sqrt).      
-00012600: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012610: 2020 2020 4420 3d20 572e 7375 6d28 6178      D = W.sum(ax
-00012620: 6973 3d30 290a 2020 2020 2020 2020 2020  is=0).          
-00012630: 2020 4469 6e76 5f73 7172 7420 3d20 7074    Dinv_sqrt = pt
-00012640: 2e64 6961 6728 3120 2f20 7074 2e73 7172  .diag(1 / pt.sqr
-00012650: 7428 4429 290a 2020 2020 2020 2020 2020  t(D)).          
-00012660: 2020 4457 4420 3d20 7074 2e64 6f74 2870    DWD = pt.dot(p
-00012670: 742e 646f 7428 4469 6e76 5f73 7172 742c  t.dot(Dinv_sqrt,
-00012680: 2057 292c 2044 696e 765f 7371 7274 290a   W), Dinv_sqrt).
-00012690: 2020 2020 2020 2020 6c61 6d20 3d20 7074          lam = pt
-000126a0: 2e73 6c69 6e61 6c67 2e65 6967 7661 6c73  .slinalg.eigvals
-000126b0: 6828 4457 442c 2070 742e 6579 6528 4457  h(DWD, pt.eye(DW
-000126c0: 442e 7368 6170 655b 305d 2929 0a0a 2020  D.shape[0]))..  
-000126d0: 2020 2020 2020 642c 205f 203d 2057 2e73        d, _ = W.s
-000126e0: 6861 7065 0a0a 2020 2020 2020 2020 6966  hape..        if
-000126f0: 2076 616c 7565 2e6e 6469 6d20 3d3d 2031   value.ndim == 1
-00012700: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
-00012710: 6c75 6520 3d20 7661 6c75 655b 4e6f 6e65  lue = value[None
-00012720: 2c20 3a5d 0a0a 2020 2020 2020 2020 6c6f  , :]..        lo
-00012730: 6774 6175 203d 2064 202a 2070 742e 6c6f  gtau = d * pt.lo
-00012740: 6728 7461 7529 2e73 756d 2829 0a20 2020  g(tau).sum().   
-00012750: 2020 2020 206c 6f67 6465 7420 3d20 7074       logdet = pt
-00012760: 2e6c 6f67 2831 202d 2061 6c70 6861 2e54  .log(1 - alpha.T
-00012770: 202a 206c 616d 5b3a 2c20 4e6f 6e65 5d29   * lam[:, None])
-00012780: 2e73 756d 2829 0a20 2020 2020 2020 2064  .sum().        d
-00012790: 656c 7461 203d 2076 616c 7565 202d 206d  elta = value - m
-000127a0: 750a 0a20 2020 2020 2020 2069 6620 7370  u..        if sp
-000127b0: 6172 7365 3a0a 2020 2020 2020 2020 2020  arse:.          
-000127c0: 2020 5764 656c 7461 203d 2070 7974 656e    Wdelta = pyten
-000127d0: 736f 722e 7370 6172 7365 2e64 6f74 2864  sor.sparse.dot(d
-000127e0: 656c 7461 2c20 5729 0a20 2020 2020 2020  elta, W).       
-000127f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00012800: 2020 2057 6465 6c74 6120 3d20 7074 2e64     Wdelta = pt.d
-00012810: 6f74 2864 656c 7461 2c20 5729 0a0a 2020  ot(delta, W)..  
-00012820: 2020 2020 2020 7461 755f 646f 745f 6465        tau_dot_de
-00012830: 6c74 6120 3d20 445b 4e6f 6e65 2c20 3a5d  lta = D[None, :]
-00012840: 202a 2064 656c 7461 202d 2061 6c70 6861   * delta - alpha
-00012850: 202a 2057 6465 6c74 610a 2020 2020 2020   * Wdelta.      
-00012860: 2020 6c6f 6771 7561 6420 3d20 2874 6175    logquad = (tau
-00012870: 202a 2064 656c 7461 202a 2074 6175 5f64   * delta * tau_d
-00012880: 6f74 5f64 656c 7461 292e 7375 6d28 6178  ot_delta).sum(ax
-00012890: 6973 3d2d 3129 0a20 2020 2020 2020 2072  is=-1).        r
-000128a0: 6574 7572 6e20 6368 6563 6b5f 7061 7261  eturn check_para
-000128b0: 6d65 7465 7273 280a 2020 2020 2020 2020  meters(.        
-000128c0: 2020 2020 302e 3520 2a20 286c 6f67 7461      0.5 * (logta
-000128d0: 7520 2b20 6c6f 6764 6574 202d 206c 6f67  u + logdet - log
-000128e0: 7175 6164 292c 0a20 2020 2020 2020 2020  quad),.         
-000128f0: 2020 202d 3120 3c3d 2061 6c70 6861 2c0a     -1 <= alpha,.
-00012900: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-00012910: 6120 3c3d 2031 2c0a 2020 2020 2020 2020  a <= 1,.        
-00012920: 2020 2020 7461 7520 3e20 302c 0a20 2020      tau > 0,.   
-00012930: 2020 2020 2020 2020 206d 7367 3d22 2d31           msg="-1
-00012940: 203c 3d20 616c 7068 6120 3c3d 2031 2c20   <= alpha <= 1, 
-00012950: 7461 7520 3e20 3022 2c0a 2020 2020 2020  tau > 0",.      
-00012960: 2020 290a 0a0a 636c 6173 7320 5374 6963    )...class Stic
-00012970: 6b42 7265 616b 696e 6757 6569 6768 7473  kBreakingWeights
-00012980: 5256 2852 616e 646f 6d56 6172 6961 626c  RV(RandomVariabl
-00012990: 6529 3a0a 2020 2020 6e61 6d65 203d 2022  e):.    name = "
-000129a0: 7374 6963 6b5f 6272 6561 6b69 6e67 5f77  stick_breaking_w
-000129b0: 6569 6768 7473 220a 2020 2020 6e64 696d  eights".    ndim
-000129c0: 5f73 7570 7020 3d20 310a 2020 2020 6e64  _supp = 1.    nd
-000129d0: 696d 735f 7061 7261 6d73 203d 205b 302c  ims_params = [0,
-000129e0: 2030 5d0a 2020 2020 6474 7970 6520 3d20   0].    dtype = 
-000129f0: 2266 6c6f 6174 5822 0a20 2020 205f 7072  "floatX".    _pr
-00012a00: 696e 745f 6e61 6d65 203d 2028 2253 7469  int_name = ("Sti
-00012a10: 636b 4272 6561 6b69 6e67 5765 6967 6874  ckBreakingWeight
-00012a20: 7322 2c20 225c 5c6f 7065 7261 746f 726e  s", "\\operatorn
-00012a30: 616d 657b 5374 6963 6b42 7265 616b 696e  ame{StickBreakin
-00012a40: 6757 6569 6768 7473 7d22 290a 0a20 2020  gWeights}")..   
-00012a50: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
-00012a60: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
-00012a70: 6474 7970 652c 2061 6c70 6861 2c20 4b29  dtype, alpha, K)
-00012a80: 3a0a 2020 2020 2020 2020 616c 7068 6120  :.        alpha 
-00012a90: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00012aa0: 6172 6961 626c 6528 616c 7068 6129 0a20  ariable(alpha). 
-00012ab0: 2020 2020 2020 204b 203d 2070 742e 6173         K = pt.as
-00012ac0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00012ad0: 2869 6e74 5828 4b29 290a 0a20 2020 2020  (intX(K))..     
-00012ae0: 2020 2069 6620 4b2e 6e64 696d 203e 2030     if K.ndim > 0
-00012af0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00012b00: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00012b10: 4b20 6d75 7374 2062 6520 6120 7363 616c  K must be a scal
-00012b20: 6172 2e22 290a 0a20 2020 2020 2020 2072  ar.")..        r
-00012b30: 6574 7572 6e20 7375 7065 7228 292e 6d61  eturn super().ma
-00012b40: 6b65 5f6e 6f64 6528 726e 672c 2073 697a  ke_node(rng, siz
-00012b50: 652c 2064 7479 7065 2c20 616c 7068 612c  e, dtype, alpha,
-00012b60: 204b 290a 0a20 2020 2064 6566 205f 7375   K)..    def _su
-00012b70: 7070 5f73 6861 7065 5f66 726f 6d5f 7061  pp_shape_from_pa
-00012b80: 7261 6d73 2873 656c 662c 2064 6973 745f  rams(self, dist_
-00012b90: 7061 7261 6d73 2c20 2a2a 6b77 6172 6773  params, **kwargs
-00012ba0: 293a 0a20 2020 2020 2020 204b 203d 2064  ):.        K = d
-00012bb0: 6973 745f 7061 7261 6d73 5b31 5d0a 2020  ist_params[1].  
-00012bc0: 2020 2020 2020 7265 7475 726e 2028 4b20        return (K 
-00012bd0: 2b20 312c 290a 0a20 2020 2040 636c 6173  + 1,)..    @clas
-00012be0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00012bf0: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
-00012c00: 2061 6c70 6861 2c20 4b2c 2073 697a 6529   alpha, K, size)
-00012c10: 3a0a 2020 2020 2020 2020 6966 204b 203c  :.        if K <
-00012c20: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00012c30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00012c40: 2822 4b20 6e65 6564 7320 746f 2062 6520  ("K needs to be 
-00012c50: 706f 7369 7469 7665 2e22 290a 0a20 2020  positive.")..   
-00012c60: 2020 2020 2073 697a 6520 3d20 746f 5f74       size = to_t
-00012c70: 7570 6c65 2873 697a 6529 2069 6620 7369  uple(size) if si
-00012c80: 7a65 2069 7320 6e6f 7420 4e6f 6e65 2065  ze is not None e
-00012c90: 6c73 6520 616c 7068 612e 7368 6170 650a  lse alpha.shape.
-00012ca0: 2020 2020 2020 2020 7369 7a65 203d 2073          size = s
-00012cb0: 697a 6520 2b20 284b 2c29 0a20 2020 2020  ize + (K,).     
-00012cc0: 2020 2061 6c70 6861 203d 2061 6c70 6861     alpha = alpha
-00012cd0: 5b2e 2e2e 2c20 6e70 2e6e 6577 6178 6973  [..., np.newaxis
-00012ce0: 5d0a 0a20 2020 2020 2020 2062 6574 6173  ]..        betas
-00012cf0: 203d 2072 6e67 2e62 6574 6128 312c 2061   = rng.beta(1, a
-00012d00: 6c70 6861 2c20 7369 7a65 3d73 697a 6529  lpha, size=size)
-00012d10: 0a0a 2020 2020 2020 2020 7374 6963 6b73  ..        sticks
-00012d20: 203d 206e 702e 636f 6e63 6174 656e 6174   = np.concatenat
-00012d30: 6528 0a20 2020 2020 2020 2020 2020 2028  e(.            (
-00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d50: 206e 702e 6f6e 6573 2873 6861 7065 3d28   np.ones(shape=(
-00012d60: 7369 7a65 5b3a 2d31 5d20 2b20 2831 2c29  size[:-1] + (1,)
-00012d70: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00012d80: 2020 2020 6e70 2e63 756d 7072 6f64 2831      np.cumprod(1
-00012d90: 202d 2062 6574 6173 5b2e 2e2e 2c20 3a2d   - betas[..., :-
-00012da0: 315d 2c20 6178 6973 3d2d 3129 2c0a 2020  1], axis=-1),.  
-00012db0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00012dc0: 2020 2020 2020 2020 2061 7869 733d 2d31           axis=-1
-00012dd0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00012de0: 2020 2020 2077 6569 6768 7473 203d 2073       weights = s
-00012df0: 7469 636b 7320 2a20 6265 7461 730a 2020  ticks * betas.  
-00012e00: 2020 2020 2020 7765 6967 6874 7320 3d20        weights = 
-00012e10: 6e70 2e63 6f6e 6361 7465 6e61 7465 280a  np.concatenate(.
-00012e20: 2020 2020 2020 2020 2020 2020 2877 6569              (wei
-00012e30: 6768 7473 2c20 3120 2d20 7765 6967 6874  ghts, 1 - weight
-00012e40: 732e 7375 6d28 6178 6973 3d2d 3129 5b2e  s.sum(axis=-1)[.
-00012e50: 2e2e 2c20 6e70 2e6e 6577 6178 6973 5d29  .., np.newaxis])
-00012e60: 2c0a 2020 2020 2020 2020 2020 2020 6178  ,.            ax
-00012e70: 6973 3d2d 312c 0a20 2020 2020 2020 2029  is=-1,.        )
-00012e80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00012e90: 2077 6569 6768 7473 0a0a 0a73 7469 636b   weights...stick
-00012ea0: 6272 6561 6b69 6e67 7765 6967 6874 7320  breakingweights 
-00012eb0: 3d20 5374 6963 6b42 7265 616b 696e 6757  = StickBreakingW
-00012ec0: 6569 6768 7473 5256 2829 0a0a 0a63 6c61  eightsRV()...cla
-00012ed0: 7373 2053 7469 636b 4272 6561 6b69 6e67  ss StickBreaking
-00012ee0: 5765 6967 6874 7328 5369 6d70 6c65 7843  Weights(SimplexC
-00012ef0: 6f6e 7469 6e75 6f75 7329 3a0a 2020 2020  ontinuous):.    
-00012f00: 7222 2222 0a20 2020 204c 696b 656c 6968  r""".    Likelih
-00012f10: 6f6f 6420 6f66 2074 7275 6e63 6174 6564  ood of truncated
-00012f20: 2073 7469 636b 2d62 7265 616b 696e 6720   stick-breaking 
-00012f30: 7765 6967 6874 732e 2054 6865 2077 6569  weights. The wei
-00012f40: 6768 7473 2061 7265 2067 656e 6572 6174  ghts are generat
-00012f50: 6564 2066 726f 6d20 610a 2020 2020 7374  ed from a.    st
-00012f60: 6963 6b2d 6272 6561 6b69 6e67 2070 726f  ick-breaking pro
-00012f70: 6365 6475 6365 2077 6865 7265 203a 6d61  ceduce where :ma
-00012f80: 7468 3a60 785f 6b20 3d20 765f 6b20 5c70  th:`x_k = v_k \p
-00012f90: 726f 645f 7b5c 656c 6c20 3c20 6b7d 2028  rod_{\ell < k} (
-00012fa0: 3120 2d20 765f 5c65 6c6c 2960 2066 6f72  1 - v_\ell)` for
-00012fb0: 0a20 2020 203a 6d61 7468 3a60 6b20 5c69  .    :math:`k \i
-00012fc0: 6e20 5c7b 312c 205c 6c64 6f74 732c 204b  n \{1, \ldots, K
-00012fd0: 5c7d 6020 616e 6420 3a6d 6174 683a 6078  \}` and :math:`x
-00012fe0: 5f4b 203d 205c 7072 6f64 5f7b 5c65 6c6c  _K = \prod_{\ell
-00012ff0: 203d 2031 7d5e 7b4b 7d20 2831 202d 2076   = 1}^{K} (1 - v
-00013000: 5f5c 656c 6c29 203d 2031 202d 205c 7375  _\ell) = 1 - \su
-00013010: 6d5f 7b5c 656c 6c3d 317d 5e4b 2078 5f5c  m_{\ell=1}^K x_\
-00013020: 656c 6c60 0a20 2020 2077 6974 6820 3a6d  ell`.    with :m
-00013030: 6174 683a 6076 5f6b 205c 7374 6163 6b72  ath:`v_k \stackr
-00013040: 656c 7b5c 7465 7874 7b69 2e69 2e64 2e7d  el{\text{i.i.d.}
-00013050: 7d7b 5c73 696d 7d20 5c74 6578 747b 4265  }{\sim} \text{Be
-00013060: 7461 7d28 312c 205c 616c 7068 6129 602e  ta}(1, \alpha)`.
-00013070: 0a0a 2020 2020 2e2e 206d 6174 683a 0a0a  ..    .. math:..
-00013080: 2020 2020 2020 2020 6628 5c6d 6174 6862          f(\mathb
-00013090: 667b 787d 7c5c 616c 7068 612c 204b 2920  f{x}|\alpha, K) 
-000130a0: 3d0a 2020 2020 2020 2020 2020 2020 4228  =.            B(
-000130b0: 312c 205c 616c 7068 6129 5e7b 2d4b 7d78  1, \alpha)^{-K}x
-000130c0: 5f7b 4b2b 317d 5e5c 616c 7068 6120 5c70  _{K+1}^\alpha \p
-000130d0: 726f 645f 7b6b 3d31 7d5e 7b4b 2b31 7d5c  rod_{k=1}^{K+1}\
-000130e0: 6c65 6674 5c7b 5c73 756d 5f7b 6a3d 6b7d  left\{\sum_{j=k}
-000130f0: 5e7b 4b2b 317d 2078 5f6a 5c72 6967 6874  ^{K+1} x_j\right
-00013100: 5c7d 5e7b 2d31 7d0a 0a20 2020 203d 3d3d  \}^{-1}..    ===
-00013110: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
-00013120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013140: 3d3d 3d3d 3d3d 0a20 2020 2053 7570 706f  ======.    Suppo
-00013150: 7274 2020 203a 6d61 7468 3a60 785f 6b20  rt   :math:`x_k 
-00013160: 5c69 6e20 2830 2c20 3129 6020 666f 7220  \in (0, 1)` for 
-00013170: 3a6d 6174 683a 606b 205c 696e 205c 7b31  :math:`k \in \{1
-00013180: 2c20 5c6c 646f 7473 2c20 4b2b 315c 7d60  , \ldots, K+1\}`
-00013190: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
-000131a0: 7563 6820 7468 6174 203a 6d61 7468 3a60  uch that :math:`
-000131b0: 5c73 756d 2078 5f6b 203d 2031 600a 2020  \sum x_k = 1`.  
-000131c0: 2020 4d65 616e 2020 2020 2020 3a6d 6174    Mean      :mat
-000131d0: 683a 605c 6d61 7468 6262 7b45 7d5b 785f  h:`\mathbb{E}[x_
-000131e0: 6b5d 203d 205c 6466 7261 637b 317d 7b31  k] = \dfrac{1}{1
-000131f0: 202b 205c 616c 7068 617d 5c6c 6566 7428   + \alpha}\left(
-00013200: 5c64 6672 6163 7b5c 616c 7068 617d 7b31  \dfrac{\alpha}{1
-00013210: 202b 205c 616c 7068 617d 5c72 6967 6874   + \alpha}\right
-00013220: 295e 7b6b 202d 2031 7d60 0a20 2020 2020  )^{k - 1}`.     
-00013230: 2020 2020 2020 2020 2066 6f72 203a 6d61           for :ma
-00013240: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
-00013250: 6c64 6f74 732c 204b 5c7d 6020 616e 6420  ldots, K\}` and 
-00013260: 3a6d 6174 683a 605c 6d61 7468 6262 7b45  :math:`\mathbb{E
-00013270: 7d5b 785f 7b4b 2b31 7d5d 203d 205c 6c65  }[x_{K+1}] = \le
-00013280: 6674 285c 6466 7261 637b 5c61 6c70 6861  ft(\dfrac{\alpha
-00013290: 7d7b 3120 2b20 5c61 6c70 6861 7d5c 7269  }{1 + \alpha}\ri
-000132a0: 6768 7429 5e7b 4b7d 600a 2020 2020 3d3d  ght)^{K}`.    ==
-000132b0: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
-000132c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000132d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000132e0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
-000132f0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00013300: 2d2d 2d2d 2d2d 0a20 2020 2061 6c70 6861  ------.    alpha
-00013310: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-00013320: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
-00013330: 436f 6e63 656e 7472 6174 696f 6e20 7061  Concentration pa
-00013340: 7261 6d65 7465 7220 2861 6c70 6861 203e  rameter (alpha >
-00013350: 2030 292e 0a20 2020 204b 203a 2074 656e   0)..    K : ten
-00013360: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
-00013370: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
-00013380: 6572 206f 6620 2273 7469 636b 7322 2074  er of "sticks" t
-00013390: 6f20 6272 6561 6b20 6f66 6620 6672 6f6d  o break off from
-000133a0: 2061 6e20 696e 6974 6961 6c20 6f6e 652d   an initial one-
-000133b0: 756e 6974 2073 7469 636b 2e20 5468 6520  unit stick. The 
-000133c0: 6c65 6e67 7468 206f 6620 7468 6520 7765  length of the we
-000133d0: 6967 6874 0a20 2020 2020 2020 2076 6563  ight.        vec
-000133e0: 746f 7220 6973 204b 202b 2031 2c20 7768  tor is K + 1, wh
-000133f0: 6572 6520 7468 6520 6c61 7374 2077 6569  ere the last wei
-00013400: 6768 7420 6973 206f 6e65 206d 696e 7573  ght is one minus
-00013410: 2074 6865 2073 756d 206f 6620 616c 6c20   the sum of all 
-00013420: 7468 6520 6669 7273 7420 7374 6963 6b73  the first sticks
-00013430: 2e0a 0a20 2020 2052 6566 6572 656e 6365  ...    Reference
-00013440: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00013450: 0a20 2020 202e 2e20 5b31 5d20 4973 6877  .    .. [1] Ishw
-00013460: 6172 616e 2c20 482e 2c20 2620 4a61 6d65  aran, H., & Jame
-00013470: 732c 204c 2e20 462e 2028 3230 3031 292e  s, L. F. (2001).
-00013480: 2047 6962 6273 2073 616d 706c 696e 6720   Gibbs sampling 
-00013490: 6d65 7468 6f64 7320 666f 7220 7374 6963  methods for stic
-000134a0: 6b2d 6272 6561 6b69 6e67 2070 7269 6f72  k-breaking prior
-000134b0: 732e 0a20 2020 2020 2020 2020 2020 4a6f  s..           Jo
-000134c0: 7572 6e61 6c20 6f66 2074 6865 2041 6d65  urnal of the Ame
-000134d0: 7269 6361 6e20 5374 6174 6973 7469 6361  rican Statistica
-000134e0: 6c20 4173 736f 6369 6174 696f 6e2c 2039  l Association, 9
-000134f0: 3628 3435 3329 2c20 3136 312d 3137 332e  6(453), 161-173.
-00013500: 0a0a 2020 2020 2e2e 205b 325d 204d c3bc  ..    .. [2] M..
-00013510: 6c6c 6572 2c20 502e 2c20 5175 696e 7461  ller, P., Quinta
-00013520: 6e61 2c20 462e 2041 2e2c 204a 6172 612c  na, F. A., Jara,
-00013530: 2041 2e2c 2026 2048 616e 736f 6e2c 2054   A., & Hanson, T
-00013540: 2e20 2832 3031 3529 2e20 4261 7965 7369  . (2015). Bayesi
-00013550: 616e 206e 6f6e 7061 7261 6d65 7472 6963  an nonparametric
-00013560: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
-00013570: 2061 6e61 6c79 7369 732e 204e 6577 2059   analysis. New Y
-00013580: 6f72 6b3a 2053 7072 696e 6765 722e 0a20  ork: Springer.. 
-00013590: 2020 2022 2222 0a20 2020 2072 765f 6f70     """.    rv_op
-000135a0: 203d 2073 7469 636b 6272 6561 6b69 6e67   = stickbreaking
-000135b0: 7765 6967 6874 730a 0a20 2020 2040 636c  weights..    @cl
-000135c0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000135d0: 6620 6469 7374 2863 6c73 2c20 616c 7068  f dist(cls, alph
-000135e0: 612c 204b 2c20 2a61 7267 732c 202a 2a6b  a, K, *args, **k
-000135f0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00013600: 616c 7068 6120 3d20 7074 2e61 735f 7465  alpha = pt.as_te
-00013610: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
-00013620: 6f61 7458 2861 6c70 6861 2929 0a20 2020  oatX(alpha)).   
-00013630: 2020 2020 204b 203d 2070 742e 6173 5f74       K = pt.as_t
-00013640: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
-00013650: 6e74 5828 4b29 290a 0a20 2020 2020 2020  ntX(K))..       
-00013660: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00013670: 6469 7374 285b 616c 7068 612c 204b 5d2c  dist([alpha, K],
-00013680: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00013690: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
-000136a0: 697a 652c 2061 6c70 6861 2c20 4b29 3a0a  ize, alpha, K):.
-000136b0: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
-000136c0: 616c 7068 615b 2e2e 2e2c 206e 702e 6e65  alpha[..., np.ne
-000136d0: 7761 7869 735d 0a20 2020 2020 2020 206d  waxis].        m
-000136e0: 6f6d 656e 7420 3d20 2861 6c70 6861 202f  oment = (alpha /
-000136f0: 2028 3120 2b20 616c 7068 6129 2920 2a2a   (1 + alpha)) **
-00013700: 2070 742e 6172 616e 6765 284b 290a 2020   pt.arange(K).  
-00013710: 2020 2020 2020 6d6f 6d65 6e74 202a 3d20        moment *= 
-00013720: 3120 2f20 2831 202b 2061 6c70 6861 290a  1 / (1 + alpha).
-00013730: 2020 2020 2020 2020 6d6f 6d65 6e74 203d          moment =
-00013740: 2070 742e 636f 6e63 6174 656e 6174 6528   pt.concatenate(
-00013750: 5b6d 6f6d 656e 742c 2028 616c 7068 6120  [moment, (alpha 
-00013760: 2f20 2831 202b 2061 6c70 6861 2929 202a  / (1 + alpha)) *
-00013770: 2a20 4b5d 2c20 6178 6973 3d2d 3129 0a20  * K], axis=-1). 
-00013780: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
-00013790: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
-000137a0: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
-000137b0: 206d 6f6d 656e 745f 7369 7a65 203d 2070   moment_size = p
-000137c0: 742e 636f 6e63 6174 656e 6174 6528 0a20  t.concatenate(. 
-000137d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000137e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137f0: 2020 2020 2073 697a 652c 0a20 2020 2020       size,.     
-00013800: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00013810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013820: 2020 2020 2020 2020 204b 202b 2031 2c0a           K + 1,.
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00013850: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00013860: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00013870: 2020 206d 6f6d 656e 7420 3d20 7074 2e66     moment = pt.f
-00013880: 756c 6c28 6d6f 6d65 6e74 5f73 697a 652c  ull(moment_size,
-00013890: 206d 6f6d 656e 7429 0a0a 2020 2020 2020   moment)..      
-000138a0: 2020 7265 7475 726e 206d 6f6d 656e 740a    return moment.
-000138b0: 0a20 2020 2064 6566 206c 6f67 7028 7661  .    def logp(va
-000138c0: 6c75 652c 2061 6c70 6861 2c20 4b29 3a0a  lue, alpha, K):.
-000138d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000138e0: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
-000138f0: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
-00013900: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
-00013910: 6e20 696e 6475 6365 6420 6672 6f6d 2074  n induced from t
-00013920: 6865 2073 7469 636b 2d62 7265 616b 696e  he stick-breakin
-00013930: 6720 7072 6f63 6573 730a 2020 2020 2020  g process.      
-00013940: 2020 6174 2073 7065 6369 6669 6564 2076    at specified v
-00013950: 616c 7565 2e0a 0a20 2020 2020 2020 2050  alue...        P
-00013960: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00013970: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00013980: 2020 2020 2076 616c 7565 3a20 6e75 6d65       value: nume
-00013990: 7269 630a 2020 2020 2020 2020 2020 2020  ric.            
-000139a0: 5661 6c75 6520 666f 7220 7768 6963 6820  Value for which 
-000139b0: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
-000139c0: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
-000139d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000139e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000139f0: 2020 2020 2020 2020 5465 6e73 6f72 5661          TensorVa
-00013a00: 7269 6162 6c65 0a20 2020 2020 2020 2022  riable.        "
-00013a10: 2222 0a20 2020 2020 2020 206c 6f67 7020  "".        logp 
-00013a20: 3d20 2d70 742e 7375 6d28 0a20 2020 2020  = -pt.sum(.     
-00013a30: 2020 2020 2020 2070 742e 6c6f 6728 0a20         pt.log(. 
-00013a40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013a50: 742e 6375 6d73 756d 280a 2020 2020 2020  t.cumsum(.      
-00013a60: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00013a70: 6c75 655b 2e2e 2e2c 203a 3a2d 315d 2c0a  lue[..., ::-1],.
-00013a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a90: 2020 2020 6178 6973 3d2d 312c 0a20 2020      axis=-1,.   
-00013aa0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00013ab0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00013ac0: 2020 2020 2020 2020 2020 6178 6973 3d2d            axis=-
-00013ad0: 312c 0a20 2020 2020 2020 2029 0a20 2020  1,.        ).   
-00013ae0: 2020 2020 206c 6f67 7020 2b3d 202d 4b20       logp += -K 
-00013af0: 2a20 6265 7461 6c6e 2831 2c20 616c 7068  * betaln(1, alph
-00013b00: 6129 0a20 2020 2020 2020 206c 6f67 7020  a).        logp 
-00013b10: 2b3d 2061 6c70 6861 202a 2070 742e 6c6f  += alpha * pt.lo
-00013b20: 6728 7661 6c75 655b 2e2e 2e2c 202d 315d  g(value[..., -1]
-00013b30: 290a 0a20 2020 2020 2020 206c 6f67 7020  )..        logp 
-00013b40: 3d20 7074 2e73 7769 7463 6828 0a20 2020  = pt.switch(.   
-00013b50: 2020 2020 2020 2020 2070 742e 6f72 5f28           pt.or_(
-00013b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b70: 2070 742e 616e 7928 0a20 2020 2020 2020   pt.any(.       
-00013b80: 2020 2020 2020 2020 2020 2020 2070 742e               pt.
-00013b90: 616e 645f 2870 742e 6c65 2876 616c 7565  and_(pt.le(value
-00013ba0: 2c20 3029 2c20 7074 2e67 6528 7661 6c75  , 0), pt.ge(valu
-00013bb0: 652c 2031 2929 2c0a 2020 2020 2020 2020  e, 1)),.        
-00013bc0: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00013bd0: 3d2d 312c 0a20 2020 2020 2020 2020 2020  =-1,.           
-00013be0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00013bf0: 2020 2020 2020 2020 7074 2e6f 725f 280a          pt.or_(.
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 2020 2020 7074 2e62 6974 7769 7365 5f6e      pt.bitwise_n
-00013c20: 6f74 2870 742e 616c 6c63 6c6f 7365 2876  ot(pt.allclose(v
-00013c30: 616c 7565 2e73 756d 282d 3129 2c20 3129  alue.sum(-1), 1)
-00013c40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00013c50: 2020 2020 2020 2070 742e 6e65 7128 7661         pt.neq(va
-00013c60: 6c75 652e 7368 6170 655b 2d31 5d2c 204b  lue.shape[-1], K
-00013c70: 202b 2031 292c 0a20 2020 2020 2020 2020   + 1),.         
-00013c80: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00013c90: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00013ca0: 2020 2020 202d 6e70 2e69 6e66 2c0a 2020       -np.inf,.  
-00013cb0: 2020 2020 2020 2020 2020 6c6f 6770 2c0a            logp,.
-00013cc0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00013cd0: 2020 2072 6574 7572 6e20 6368 6563 6b5f     return check_
-00013ce0: 7061 7261 6d65 7465 7273 280a 2020 2020  parameters(.    
-00013cf0: 2020 2020 2020 2020 6c6f 6770 2c0a 2020          logp,.  
-00013d00: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
-00013d10: 3e20 302c 0a20 2020 2020 2020 2020 2020  > 0,.           
-00013d20: 204b 203e 2030 2c0a 2020 2020 2020 2020   K > 0,.        
-00013d30: 2020 2020 6d73 673d 2261 6c70 6861 203e      msg="alpha >
-00013d40: 2030 2c20 4b20 3e20 3022 2c0a 2020 2020   0, K > 0",.    
-00013d50: 2020 2020 290a 0a0a 636c 6173 7320 5a65      )...class Ze
-00013d60: 726f 5375 6d4e 6f72 6d61 6c52 5628 5379  roSumNormalRV(Sy
-00013d70: 6d62 6f6c 6963 5261 6e64 6f6d 5661 7269  mbolicRandomVari
-00013d80: 6162 6c65 293a 0a20 2020 2022 2222 5a65  able):.    """Ze
-00013d90: 726f 5375 6d4e 6f72 6d61 6c20 7261 6e64  roSumNormal rand
-00013da0: 6f6d 2076 6172 6961 626c 6522 2222 0a0a  om variable"""..
-00013db0: 2020 2020 5f70 7269 6e74 5f6e 616d 6520      _print_name 
-00013dc0: 3d20 2822 5a65 726f 5375 6d4e 6f72 6d61  = ("ZeroSumNorma
-00013dd0: 6c22 2c20 225c 5c6f 7065 7261 746f 726e  l", "\\operatorn
-00013de0: 616d 657b 5a65 726f 5375 6d4e 6f72 6d61  ame{ZeroSumNorma
-00013df0: 6c7d 2229 0a20 2020 2064 6566 6175 6c74  l}").    default
-00013e00: 5f6f 7574 7075 7420 3d20 300a 0a0a 636c  _output = 0...cl
-00013e10: 6173 7320 5a65 726f 5375 6d4e 6f72 6d61  ass ZeroSumNorma
-00013e20: 6c28 4469 7374 7269 6275 7469 6f6e 293a  l(Distribution):
-00013e30: 0a20 2020 2072 2222 220a 2020 2020 5a65  .    r""".    Ze
-00013e40: 726f 5375 6d4e 6f72 6d61 6c20 6469 7374  roSumNormal dist
-00013e50: 7269 6275 7469 6f6e 2c20 692e 6520 4e6f  ribution, i.e No
-00013e60: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-00013e70: 6e20 7768 6572 6520 6f6e 6520 6f72 0a20  n where one or. 
-00013e80: 2020 2073 6576 6572 616c 2061 7865 7320     several axes 
-00013e90: 6172 6520 636f 6e73 7472 6169 6e65 6420  are constrained 
-00013ea0: 746f 2073 756d 2074 6f20 7a65 726f 2e0a  to sum to zero..
-00013eb0: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
-00013ec0: 7468 6520 6c61 7374 2061 7869 7320 6973  the last axis is
-00013ed0: 2063 6f6e 7374 7261 696e 6564 2074 6f20   constrained to 
-00013ee0: 7375 6d20 746f 207a 6572 6f2e 0a20 2020  sum to zero..   
-00013ef0: 2053 6565 2060 6e5f 7a65 726f 7375 6d5f   See `n_zerosum_
-00013f00: 6178 6573 6020 6b77 6172 6720 666f 7220  axes` kwarg for 
-00013f10: 6d6f 7265 2064 6574 6169 6c73 2e0a 0a20  more details... 
-00013f20: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-00013f30: 2020 2020 2020 5c62 6567 696e 7b61 6c69        \begin{ali
-00013f40: 676e 2a7d 0a20 2020 2020 2020 2020 2020  gn*}.           
-00013f50: 205a 534e 285c 7369 676d 6129 203d 204e   ZSN(\sigma) = N
-00013f60: 205c 4269 6728 2030 2c20 5c73 6967 6d61   \Big( 0, \sigma
-00013f70: 5e32 2028 4920 2d20 5c74 6672 6163 7b31  ^2 (I - \tfrac{1
-00013f80: 7d7b 6e7d 4a29 205c 4269 6729 205c 5c0a  }{n}J) \Big) \\.
-00013f90: 2020 2020 2020 2020 2020 2020 5c74 6578              \tex
-00013fa0: 747b 7768 6572 657d 205c 207e 204a 5f7b  t{where} \ ~ J_{
-00013fb0: 696a 7d20 3d20 3120 5c20 7e20 5c74 6578  ij} = 1 \ ~ \tex
-00013fc0: 747b 616e 647d 205c 5c0a 2020 2020 2020  t{and} \\.      
-00013fd0: 2020 2020 2020 6e20 3d20 5c74 6578 747b        n = \text{
-00013fe0: 6e62 7220 6f66 207a 6572 6f2d 7375 6d20  nbr of zero-sum 
-00013ff0: 6178 6573 7d0a 2020 2020 2020 2020 5c65  axes}.        \e
-00014000: 6e64 7b61 6c69 676e 2a7d 0a0a 2020 2020  nd{align*}..    
-00014010: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00014020: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7369  ---------.    si
-00014030: 676d 6120 3a20 7465 6e73 6f72 5f6c 696b  gma : tensor_lik
-00014040: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
-00014050: 2020 2053 6361 6c65 2070 6172 616d 6574     Scale paramet
-00014060: 6572 2028 7369 676d 6120 3e20 3029 2e0a  er (sigma > 0)..
-00014070: 2020 2020 2020 2020 4974 2773 2061 6374          It's act
-00014080: 7561 6c6c 7920 7468 6520 7374 616e 6461  ually the standa
-00014090: 7264 2064 6576 6961 7469 6f6e 206f 6620  rd deviation of 
-000140a0: 7468 6520 756e 6465 726c 7969 6e67 2c20  the underlying, 
-000140b0: 756e 636f 6e73 7472 6169 6e65 6420 4e6f  unconstrained No
-000140c0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-000140d0: 6e2e 0a20 2020 2020 2020 2044 6566 6175  n..        Defau
-000140e0: 6c74 7320 746f 2031 2069 6620 6e6f 7420  lts to 1 if not 
-000140f0: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
-00014100: 2020 2046 6f72 206e 6f77 2c20 6060 7369     For now, ``si
-00014110: 676d 6160 6020 6861 7320 746f 2062 6520  gma`` has to be 
-00014120: 6120 7363 616c 6172 2c20 746f 2065 6e73  a scalar, to ens
-00014130: 7572 6520 7468 6520 7a65 726f 2d73 756d  ure the zero-sum
-00014140: 2063 6f6e 7374 7261 696e 742e 0a20 2020   constraint..   
-00014150: 206e 5f7a 6572 6f73 756d 5f61 7865 733a   n_zerosum_axes:
-00014160: 2069 6e74 2c20 6465 6661 756c 7473 2074   int, defaults t
-00014170: 6f20 310a 2020 2020 2020 2020 4e75 6d62  o 1.        Numb
-00014180: 6572 206f 6620 6178 6573 2061 6c6f 6e67  er of axes along
-00014190: 2077 6869 6368 2074 6865 207a 6572 6f2d   which the zero-
-000141a0: 7375 6d20 636f 6e73 7472 6169 6e74 2069  sum constraint i
-000141b0: 7320 656e 666f 7263 6564 2c20 7374 6172  s enforced, star
-000141c0: 7469 6e67 2066 726f 6d20 7468 6520 7269  ting from the ri
-000141d0: 6768 746d 6f73 7420 706f 7369 7469 6f6e  ghtmost position
-000141e0: 2e0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
-000141f0: 7473 2074 6f20 312c 2069 2e65 2074 6865  ts to 1, i.e the
-00014200: 2072 6967 6874 6d6f 7374 2061 7869 732e   rightmost axis.
-00014210: 0a20 2020 207a 6572 6f73 756d 5f61 7865  .    zerosum_axe
-00014220: 733a 2069 6e74 2c20 6465 7072 6563 6174  s: int, deprecat
-00014230: 6564 2070 6c65 6173 6520 7573 6520 6e5f  ed please use n_
-00014240: 7a65 726f 7375 6d5f 6178 6573 2061 7320  zerosum_axes as 
-00014250: 6974 7320 7375 6363 6573 736f 720a 2020  its successor.  
-00014260: 2020 6469 6d73 3a20 7365 7175 656e 6365    dims: sequence
-00014270: 206f 6620 7374 7269 6e67 732c 206f 7074   of strings, opt
-00014280: 696f 6e61 6c0a 2020 2020 2020 2020 4469  ional.        Di
-00014290: 6d65 6e73 696f 6e20 6e61 6d65 7320 6f66  mension names of
-000142a0: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
-000142b0: 6e2e 2057 6f72 6b73 2074 6865 2073 616d  n. Works the sam
-000142c0: 6520 6173 2066 6f72 206f 7468 6572 2050  e as for other P
-000142d0: 794d 4320 6469 7374 7269 6275 7469 6f6e  yMC distribution
-000142e0: 732e 0a20 2020 2020 2020 204e 6563 6573  s..        Neces
-000142f0: 7361 7279 2069 6620 6060 7368 6170 6560  sary if ``shape`
-00014300: 6020 6973 206e 6f74 2070 6173 7365 642e  ` is not passed.
-00014310: 0a20 2020 2073 6861 7065 3a20 7475 706c  .    shape: tupl
-00014320: 6520 6f66 2069 6e74 6567 6572 732c 206f  e of integers, o
-00014330: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00014340: 5368 6170 6520 6f66 2074 6865 2064 6973  Shape of the dis
-00014350: 7472 6962 7574 696f 6e2e 2057 6f72 6b73  tribution. Works
-00014360: 2074 6865 2073 616d 6520 6173 2066 6f72   the same as for
-00014370: 206f 7468 6572 2050 794d 4320 6469 7374   other PyMC dist
-00014380: 7269 6275 7469 6f6e 732e 0a20 2020 2020  ributions..     
-00014390: 2020 204e 6563 6573 7361 7279 2069 6620     Necessary if 
-000143a0: 6060 6469 6d73 6060 206f 7220 6060 6f62  ``dims`` or ``ob
-000143b0: 7365 7276 6564 6060 2069 7320 6e6f 7420  served`` is not 
-000143c0: 7061 7373 6564 2e0a 0a20 2020 2057 6172  passed...    War
-000143d0: 6e69 6e67 730a 2020 2020 2d2d 2d2d 2d2d  nings.    ------
-000143e0: 2d2d 0a20 2020 2060 6073 6967 6d61 6060  --.    ``sigma``
-000143f0: 2068 6173 2074 6f20 6265 2061 2073 6361   has to be a sca
-00014400: 6c61 722c 2074 6f20 656e 7375 7265 2074  lar, to ensure t
-00014410: 6865 207a 6572 6f2d 7375 6d20 636f 6e73  he zero-sum cons
-00014420: 7472 6169 6e74 2e0a 2020 2020 5468 6520  traint..    The 
-00014430: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
-00014440: 6679 2061 2076 6563 746f 7220 6f66 2060  fy a vector of `
-00014450: 6073 6967 6d61 6060 206d 6179 2062 6520  `sigma`` may be 
-00014460: 6164 6465 6420 696e 2066 7574 7572 6520  added in future 
-00014470: 7665 7273 696f 6e73 2e0a 0a20 2020 2060  versions...    `
-00014480: 606e 5f7a 6572 6f73 756d 5f61 7865 7360  `n_zerosum_axes`
-00014490: 6020 6861 7320 746f 2062 6520 3e20 302e  ` has to be > 0.
-000144a0: 2049 6620 796f 7520 7761 6e74 2074 6865   If you want the
-000144b0: 2062 6568 6176 696f 7220 6f66 2060 606e   behavior of ``n
-000144c0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
-000144d0: 3060 602c 0a20 2020 206a 7573 7420 7573  0``,.    just us
-000144e0: 6520 6060 706d 2e4e 6f72 6d61 6c60 602e  e ``pm.Normal``.
-000144f0: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
-00014500: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-00014510: 4465 6669 6e65 2061 2060 5a65 726f 5375  Define a `ZeroSu
-00014520: 6d4e 6f72 6d61 6c60 2076 6172 6961 626c  mNormal` variabl
-00014530: 652c 2077 6974 6820 6073 6967 6d61 3d31  e, with `sigma=1
-00014540: 6020 616e 640a 2020 2020 606e 5f7a 6572  ` and.    `n_zer
-00014550: 6f73 756d 5f61 7865 733d 3160 2020 6279  osum_axes=1`  by
-00014560: 2064 6566 6175 6c74 3a3a 0a0a 2020 2020   default::..    
-00014570: 2020 2020 434f 4f52 4453 203d 207b 0a20      COORDS = {. 
-00014580: 2020 2020 2020 2020 2020 2022 7265 6769             "regi
-00014590: 6f6e 7322 3a20 5b22 6122 2c20 2262 222c  ons": ["a", "b",
-000145a0: 2022 6322 5d2c 0a20 2020 2020 2020 2020   "c"],.         
-000145b0: 2020 2022 616e 7377 6572 7322 3a20 5b22     "answers": ["
-000145c0: 7965 7322 2c20 226e 6f22 2c20 2277 6861  yes", "no", "wha
-000145d0: 7465 7665 7222 2c20 2264 6f6e 2774 2075  tever", "don't u
-000145e0: 6e64 6572 7374 616e 6420 7175 6573 7469  nderstand questi
-000145f0: 6f6e 225d 2c0a 2020 2020 2020 2020 7d0a  on"],.        }.
-00014600: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
-00014610: 4d6f 6465 6c28 636f 6f72 6473 3d43 4f4f  Model(coords=COO
-00014620: 5244 5329 2061 7320 6d3a 0a20 2020 2020  RDS) as m:.     
-00014630: 2020 2020 2020 2023 2074 6865 207a 6572         # the zer
-00014640: 6f20 7375 6d20 6178 6973 2077 696c 6c20  o sum axis will 
-00014650: 6265 2027 616e 7377 6572 7327 0a20 2020  be 'answers'.   
-00014660: 2020 2020 2020 2020 2076 203d 2070 6d2e           v = pm.
-00014670: 5a65 726f 5375 6d4e 6f72 6d61 6c28 2276  ZeroSumNormal("v
-00014680: 222c 2064 696d 733d 2822 7265 6769 6f6e  ", dims=("region
-00014690: 7322 2c20 2261 6e73 7765 7273 2229 290a  s", "answers")).
-000146a0: 0a20 2020 2020 2020 2077 6974 6820 706d  .        with pm
-000146b0: 2e4d 6f64 656c 2863 6f6f 7264 733d 434f  .Model(coords=CO
-000146c0: 4f52 4453 2920 6173 206d 3a0a 2020 2020  ORDS) as m:.    
-000146d0: 2020 2020 2020 2020 2320 7468 6520 7a65          # the ze
-000146e0: 726f 2073 756d 2061 7865 7320 7769 6c6c  ro sum axes will
-000146f0: 2062 6520 2761 6e73 7765 7273 2720 616e   be 'answers' an
-00014700: 6420 2772 6567 696f 6e73 270a 2020 2020  d 'regions'.    
-00014710: 2020 2020 2020 2020 7620 3d20 706d 2e5a          v = pm.Z
-00014720: 6572 6f53 756d 4e6f 726d 616c 2822 7622  eroSumNormal("v"
-00014730: 2c20 6469 6d73 3d28 2272 6567 696f 6e73  , dims=("regions
-00014740: 222c 2022 616e 7377 6572 7322 292c 206e  ", "answers"), n
-00014750: 5f7a 6572 6f73 756d 5f61 7865 733d 3229  _zerosum_axes=2)
-00014760: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
-00014770: 6d2e 4d6f 6465 6c28 636f 6f72 6473 3d43  m.Model(coords=C
-00014780: 4f4f 5244 5329 2061 7320 6d3a 0a20 2020  OORDS) as m:.   
-00014790: 2020 2020 2020 2020 2023 2074 6865 207a           # the z
-000147a0: 6572 6f20 7375 6d20 6178 6573 2077 696c  ero sum axes wil
-000147b0: 6c20 6265 2074 6865 206c 6173 7420 7477  l be the last tw
-000147c0: 6f0a 2020 2020 2020 2020 2020 2020 7620  o.            v 
-000147d0: 3d20 706d 2e5a 6572 6f53 756d 4e6f 726d  = pm.ZeroSumNorm
-000147e0: 616c 2822 7622 2c20 7368 6170 653d 2833  al("v", shape=(3
-000147f0: 2c20 342c 2035 292c 206e 5f7a 6572 6f73  , 4, 5), n_zeros
-00014800: 756d 5f61 7865 733d 3229 0a20 2020 2022  um_axes=2).    "
-00014810: 2222 0a20 2020 2072 765f 7479 7065 203d  "".    rv_type =
-00014820: 205a 6572 6f53 756d 4e6f 726d 616c 5256   ZeroSumNormalRV
-00014830: 0a0a 2020 2020 6465 6620 5f5f 6e65 775f  ..    def __new_
-00014840: 5f28 0a20 2020 2020 2020 2063 6c73 2c20  _(.        cls, 
-00014850: 2a61 7267 732c 207a 6572 6f73 756d 5f61  *args, zerosum_a
-00014860: 7865 733d 4e6f 6e65 2c20 6e5f 7a65 726f  xes=None, n_zero
-00014870: 7375 6d5f 6178 6573 3d4e 6f6e 652c 2073  sum_axes=None, s
-00014880: 7570 706f 7274 5f73 6861 7065 3d4e 6f6e  upport_shape=Non
-00014890: 652c 2064 696d 733d 4e6f 6e65 2c20 2a2a  e, dims=None, **
-000148a0: 6b77 6172 6773 0a20 2020 2029 3a0a 2020  kwargs.    ):.  
-000148b0: 2020 2020 2020 6966 207a 6572 6f73 756d        if zerosum
-000148c0: 5f61 7865 7320 6973 206e 6f74 204e 6f6e  _axes is not Non
-000148d0: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-000148e0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
-000148f0: 7a65 726f 7375 6d5f 6178 6573 0a20 2020  zerosum_axes.   
-00014900: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-00014910: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-00014920: 2020 2020 2020 2020 2254 6865 2027 7a65          "The 'ze
-00014930: 726f 7375 6d5f 6178 6573 2720 7061 7261  rosum_axes' para
-00014940: 6d65 7465 7220 6973 2064 6570 7265 6361  meter is depreca
-00014950: 7465 642e 2055 7365 2027 6e5f 7a65 726f  ted. Use 'n_zero
-00014960: 7375 6d5f 6178 6573 2720 696e 7374 6561  sum_axes' instea
-00014970: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
-00014980: 2020 2020 2044 6570 7265 6361 7469 6f6e       Deprecation
-00014990: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
-000149a0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-000149b0: 6620 6469 6d73 2069 7320 6e6f 7420 4e6f  f dims is not No
-000149c0: 6e65 206f 7220 6b77 6172 6773 2e67 6574  ne or kwargs.get
-000149d0: 2822 6f62 7365 7276 6564 2229 2069 7320  ("observed") is 
-000149e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000149f0: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
-00014a00: 6178 6573 203d 2063 6c73 2e63 6865 636b  axes = cls.check
-00014a10: 5f7a 6572 6f73 756d 5f61 7865 7328 6e5f  _zerosum_axes(n_
-00014a20: 7a65 726f 7375 6d5f 6178 6573 290a 0a20  zerosum_axes).. 
-00014a30: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00014a40: 7274 5f73 6861 7065 203d 2067 6574 5f73  rt_shape = get_s
-00014a50: 7570 706f 7274 5f73 6861 7065 280a 2020  upport_shape(.  
-00014a60: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00014a70: 7070 6f72 745f 7368 6170 653d 7375 7070  pport_shape=supp
-00014a80: 6f72 745f 7368 6170 652c 0a20 2020 2020  ort_shape,.     
-00014a90: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00014aa0: 3d4e 6f6e 652c 2020 2320 5368 6170 6520  =None,  # Shape 
-00014ab0: 7769 6c6c 2062 6520 6368 6563 6b65 6420  will be checked 
-00014ac0: 696e 2060 636c 732e 6469 7374 600a 2020  in `cls.dist`.  
-00014ad0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00014ae0: 6d73 3d64 696d 732c 0a20 2020 2020 2020  ms=dims,.       
-00014af0: 2020 2020 2020 2020 206f 6273 6572 7665           observe
-00014b00: 643d 6b77 6172 6773 2e67 6574 2822 6f62  d=kwargs.get("ob
-00014b10: 7365 7276 6564 222c 204e 6f6e 6529 2c0a  served", None),.
-00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b30: 6e64 696d 5f73 7570 703d 6e5f 7a65 726f  ndim_supp=n_zero
-00014b40: 7375 6d5f 6178 6573 2c0a 2020 2020 2020  sum_axes,.      
-00014b50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00014b60: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00014b70: 5f5f 6e65 775f 5f28 0a20 2020 2020 2020  __new__(.       
-00014b80: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
-00014b90: 2020 2020 2020 2a61 7267 732c 0a20 2020        *args,.   
-00014ba0: 2020 2020 2020 2020 206e 5f7a 6572 6f73           n_zeros
-00014bb0: 756d 5f61 7865 733d 6e5f 7a65 726f 7375  um_axes=n_zerosu
-00014bc0: 6d5f 6178 6573 2c0a 2020 2020 2020 2020  m_axes,.        
-00014bd0: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
-00014be0: 653d 7375 7070 6f72 745f 7368 6170 652c  e=support_shape,
-00014bf0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
-00014c00: 733d 6469 6d73 2c0a 2020 2020 2020 2020  s=dims,.        
-00014c10: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
-00014c20: 2020 2020 2020 290a 0a20 2020 2040 636c        )..    @cl
-00014c30: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00014c40: 6620 6469 7374 2863 6c73 2c20 7369 676d  f dist(cls, sigm
-00014c50: 613d 312c 206e 5f7a 6572 6f73 756d 5f61  a=1, n_zerosum_a
-00014c60: 7865 733d 4e6f 6e65 2c20 7375 7070 6f72  xes=None, suppor
-00014c70: 745f 7368 6170 653d 4e6f 6e65 2c20 2a2a  t_shape=None, **
-00014c80: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00014c90: 206e 5f7a 6572 6f73 756d 5f61 7865 7320   n_zerosum_axes 
-00014ca0: 3d20 636c 732e 6368 6563 6b5f 7a65 726f  = cls.check_zero
-00014cb0: 7375 6d5f 6178 6573 286e 5f7a 6572 6f73  sum_axes(n_zeros
-00014cc0: 756d 5f61 7865 7329 0a0a 2020 2020 2020  um_axes)..      
-00014cd0: 2020 7369 676d 6120 3d20 7074 2e61 735f    sigma = pt.as_
-00014ce0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-00014cf0: 666c 6f61 7458 2873 6967 6d61 2929 0a20  floatX(sigma)). 
-00014d00: 2020 2020 2020 2069 6620 7369 676d 612e         if sigma.
-00014d10: 6e64 696d 203e 2030 3a0a 2020 2020 2020  ndim > 0:.      
-00014d20: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00014d30: 6545 7272 6f72 2822 7369 676d 6120 6861  eError("sigma ha
-00014d40: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
-00014d50: 2229 0a0a 2020 2020 2020 2020 7375 7070  ")..        supp
-00014d60: 6f72 745f 7368 6170 6520 3d20 6765 745f  ort_shape = get_
-00014d70: 7375 7070 6f72 745f 7368 6170 6528 0a20  support_shape(. 
-00014d80: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00014d90: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
-00014da0: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
-00014db0: 2020 2020 7368 6170 653d 6b77 6172 6773      shape=kwargs
-00014dc0: 2e67 6574 2822 7368 6170 6522 292c 0a20  .get("shape"),. 
-00014dd0: 2020 2020 2020 2020 2020 206e 6469 6d5f             ndim_
-00014de0: 7375 7070 3d6e 5f7a 6572 6f73 756d 5f61  supp=n_zerosum_a
-00014df0: 7865 732c 0a20 2020 2020 2020 2029 0a0a  xes,.        )..
-00014e00: 2020 2020 2020 2020 6966 2073 7570 706f          if suppo
-00014e10: 7274 5f73 6861 7065 2069 7320 4e6f 6e65  rt_shape is None
-00014e20: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014e30: 206e 5f7a 6572 6f73 756d 5f61 7865 7320   n_zerosum_axes 
-00014e40: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00014e50: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00014e60: 4572 726f 7228 2259 6f75 206d 7573 7420  Error("You must 
-00014e70: 7370 6563 6966 7920 6469 6d73 2c20 7368  specify dims, sh
-00014e80: 6170 6520 6f72 2073 7570 706f 7274 5f73  ape or support_s
-00014e90: 6861 7065 2070 6172 616d 6574 6572 2229  hape parameter")
-00014ea0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00014eb0: 4f44 4f3a 2065 6467 652d 6361 7365 2064  ODO: edge-case d
-00014ec0: 6f65 736e 2774 2077 6f72 6b20 666f 7220  oesn't work for 
-00014ed0: 6e6f 772c 2062 6563 6175 7365 2070 742e  now, because pt.
-00014ee0: 7374 6163 6b20 696e 2067 6574 5f73 7570  stack in get_sup
-00014ef0: 706f 7274 5f73 6861 7065 2066 6169 6c73  port_shape fails
-00014f00: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
-00014f10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014f20: 2023 2020 2020 2073 7570 706f 7274 5f73   #     support_s
-00014f30: 6861 7065 203d 2028 2920 2320 6265 6361  hape = () # beca
-00014f40: 7573 6520 6974 2773 206a 7573 7420 6120  use it's just a 
-00014f50: 4e6f 726d 616c 2069 6e20 7468 6174 2063  Normal in that c
-00014f60: 6173 650a 2020 2020 2020 2020 7375 7070  ase.        supp
-00014f70: 6f72 745f 7368 6170 6520 3d20 7074 2e61  ort_shape = pt.a
-00014f80: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-00014f90: 6528 696e 7458 2873 7570 706f 7274 5f73  e(intX(support_s
-00014fa0: 6861 7065 2929 0a0a 2020 2020 2020 2020  hape))..        
-00014fb0: 6173 7365 7274 206e 5f7a 6572 6f73 756d  assert n_zerosum
-00014fc0: 5f61 7865 7320 3d3d 2070 742e 6765 745f  _axes == pt.get_
-00014fd0: 7665 6374 6f72 5f6c 656e 6774 6828 0a20  vector_length(. 
-00014fe0: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00014ff0: 7274 5f73 6861 7065 0a20 2020 2020 2020  rt_shape.       
-00015000: 2029 2c20 2273 7570 706f 7274 5f73 6861   ), "support_sha
-00015010: 7065 2068 6173 2074 6f20 6265 2061 7320  pe has to be as 
-00015020: 6c6f 6e67 2061 7320 6e5f 7a65 726f 7375  long as n_zerosu
-00015030: 6d5f 6178 6573 220a 0a20 2020 2020 2020  m_axes"..       
-00015040: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00015050: 6469 7374 280a 2020 2020 2020 2020 2020  dist(.          
-00015060: 2020 5b73 6967 6d61 5d2c 206e 5f7a 6572    [sigma], n_zer
-00015070: 6f73 756d 5f61 7865 733d 6e5f 7a65 726f  osum_axes=n_zero
-00015080: 7375 6d5f 6178 6573 2c20 7375 7070 6f72  sum_axes, suppor
-00015090: 745f 7368 6170 653d 7375 7070 6f72 745f  t_shape=support_
-000150a0: 7368 6170 652c 202a 2a6b 7761 7267 730a  shape, **kwargs.
-000150b0: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-000150c0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-000150d0: 6465 6620 6368 6563 6b5f 7a65 726f 7375  def check_zerosu
-000150e0: 6d5f 6178 6573 2863 6c73 2c20 6e5f 7a65  m_axes(cls, n_ze
-000150f0: 726f 7375 6d5f 6178 6573 3a20 4f70 7469  rosum_axes: Opti
-00015100: 6f6e 616c 5b69 6e74 5d29 202d 3e20 696e  onal[int]) -> in
-00015110: 743a 0a20 2020 2020 2020 2069 6620 6e5f  t:.        if n_
-00015120: 7a65 726f 7375 6d5f 6178 6573 2069 7320  zerosum_axes is 
-00015130: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00015140: 2020 6e5f 7a65 726f 7375 6d5f 6178 6573    n_zerosum_axes
-00015150: 203d 2031 0a20 2020 2020 2020 2069 6620   = 1.        if 
-00015160: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
-00015170: 5f7a 6572 6f73 756d 5f61 7865 732c 2069  _zerosum_axes, i
-00015180: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00015190: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000151a0: 2822 6e5f 7a65 726f 7375 6d5f 6178 6573  ("n_zerosum_axes
-000151b0: 2068 6173 2074 6f20 6265 2061 6e20 696e   has to be an in
-000151c0: 7465 6765 7222 290a 2020 2020 2020 2020  teger").        
-000151d0: 6966 206e 6f74 206e 5f7a 6572 6f73 756d  if not n_zerosum
-000151e0: 5f61 7865 7320 3e20 303a 0a20 2020 2020  _axes > 0:.     
-000151f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00015200: 7565 4572 726f 7228 226e 5f7a 6572 6f73  ueError("n_zeros
-00015210: 756d 5f61 7865 7320 6861 7320 746f 2062  um_axes has to b
-00015220: 6520 3e20 3022 290a 2020 2020 2020 2020  e > 0").        
-00015230: 7265 7475 726e 206e 5f7a 6572 6f73 756d  return n_zerosum
-00015240: 5f61 7865 730a 0a20 2020 2040 636c 6173  _axes..    @clas
-00015250: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00015260: 7276 5f6f 7028 636c 732c 2073 6967 6d61  rv_op(cls, sigma
-00015270: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
-00015280: 2c20 7375 7070 6f72 745f 7368 6170 652c  , support_shape,
-00015290: 2073 697a 653d 4e6f 6e65 293a 0a20 2020   size=None):.   
-000152a0: 2020 2020 2073 6861 7065 203d 2074 6f5f       shape = to_
-000152b0: 7475 706c 6528 7369 7a65 2920 2b20 7475  tuple(size) + tu
-000152c0: 706c 6528 7375 7070 6f72 745f 7368 6170  ple(support_shap
-000152d0: 6529 0a20 2020 2020 2020 206e 6f72 6d61  e).        norma
-000152e0: 6c5f 6469 7374 203d 2070 6d2e 4e6f 726d  l_dist = pm.Norm
-000152f0: 616c 2e64 6973 7428 7369 676d 613d 7369  al.dist(sigma=si
-00015300: 676d 612c 2073 6861 7065 3d73 6861 7065  gma, shape=shape
-00015310: 290a 0a20 2020 2020 2020 2069 6620 6e5f  )..        if n_
-00015320: 7a65 726f 7375 6d5f 6178 6573 203e 206e  zerosum_axes > n
-00015330: 6f72 6d61 6c5f 6469 7374 2e6e 6469 6d3a  ormal_dist.ndim:
-00015340: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00015350: 7365 2056 616c 7565 4572 726f 7228 2253  se ValueError("S
-00015360: 6861 7065 206f 6620 6469 7374 7269 6275  hape of distribu
-00015370: 7469 6f6e 2069 7320 746f 6f20 736d 616c  tion is too smal
-00015380: 6c20 666f 7220 7468 6520 6e75 6d62 6572  l for the number
-00015390: 206f 6620 7a65 726f 7375 6d20 6178 6573   of zerosum axes
-000153a0: 2229 0a0a 2020 2020 2020 2020 6e6f 726d  ")..        norm
-000153b0: 616c 5f64 6973 745f 2c20 7369 676d 615f  al_dist_, sigma_
-000153c0: 2c20 7375 7070 6f72 745f 7368 6170 655f  , support_shape_
-000153d0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000153e0: 206e 6f72 6d61 6c5f 6469 7374 2e74 7970   normal_dist.typ
-000153f0: 6528 292c 0a20 2020 2020 2020 2020 2020  e(),.           
-00015400: 2073 6967 6d61 2e74 7970 6528 292c 0a20   sigma.type(),. 
-00015410: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00015420: 7274 5f73 6861 7065 2e74 7970 6528 292c  rt_shape.type(),
-00015430: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00015440: 2020 2020 2320 5a65 726f 7375 6d2d 6e6f      # Zerosum-no
-00015450: 726d 616c 696e 6720 6973 2061 6368 6965  rmaling is achie
-00015460: 7665 6420 6279 2073 7562 7472 6163 7469  ved by subtracti
-00015470: 6e67 2074 6865 206d 6561 6e20 616c 6f6e  ng the mean alon
-00015480: 6720 7468 6520 6769 7665 6e20 6e5f 7a65  g the given n_ze
-00015490: 726f 7375 6d5f 6178 6573 0a20 2020 2020  rosum_axes.     
-000154a0: 2020 207a 6572 6f73 756d 5f72 765f 203d     zerosum_rv_ =
-000154b0: 206e 6f72 6d61 6c5f 6469 7374 5f0a 2020   normal_dist_.  
-000154c0: 2020 2020 2020 666f 7220 6178 6973 2069        for axis i
-000154d0: 6e20 7261 6e67 6528 6e5f 7a65 726f 7375  n range(n_zerosu
-000154e0: 6d5f 6178 6573 293a 0a20 2020 2020 2020  m_axes):.       
-000154f0: 2020 2020 207a 6572 6f73 756d 5f72 765f       zerosum_rv_
-00015500: 202d 3d20 7a65 726f 7375 6d5f 7276 5f2e   -= zerosum_rv_.
-00015510: 6d65 616e 2861 7869 733d 2d61 7869 7320  mean(axis=-axis 
-00015520: 2d20 312c 206b 6565 7064 696d 733d 5472  - 1, keepdims=Tr
-00015530: 7565 290a 0a20 2020 2020 2020 2072 6574  ue)..        ret
-00015540: 7572 6e20 5a65 726f 5375 6d4e 6f72 6d61  urn ZeroSumNorma
-00015550: 6c52 5628 0a20 2020 2020 2020 2020 2020  lRV(.           
-00015560: 2069 6e70 7574 733d 5b6e 6f72 6d61 6c5f   inputs=[normal_
-00015570: 6469 7374 5f2c 2073 6967 6d61 5f2c 2073  dist_, sigma_, s
-00015580: 7570 706f 7274 5f73 6861 7065 5f5d 2c0a  upport_shape_],.
-00015590: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-000155a0: 7574 733d 5b7a 6572 6f73 756d 5f72 765f  uts=[zerosum_rv_
-000155b0: 2c20 7375 7070 6f72 745f 7368 6170 655f  , support_shape_
-000155c0: 5d2c 0a20 2020 2020 2020 2020 2020 206e  ],.            n
-000155d0: 6469 6d5f 7375 7070 3d6e 5f7a 6572 6f73  dim_supp=n_zeros
-000155e0: 756d 5f61 7865 732c 0a20 2020 2020 2020  um_axes,.       
-000155f0: 2029 286e 6f72 6d61 6c5f 6469 7374 2c20   )(normal_dist, 
-00015600: 7369 676d 612c 2073 7570 706f 7274 5f73  sigma, support_s
-00015610: 6861 7065 290a 0a0a 405f 6368 616e 6765  hape)...@_change
-00015620: 5f64 6973 745f 7369 7a65 2e72 6567 6973  _dist_size.regis
-00015630: 7465 7228 5a65 726f 5375 6d4e 6f72 6d61  ter(ZeroSumNorma
-00015640: 6c52 5629 0a64 6566 2063 6861 6e67 655f  lRV).def change_
-00015650: 7a65 726f 7375 6d5f 7369 7a65 286f 702c  zerosum_size(op,
-00015660: 206e 6f72 6d61 6c5f 6469 7374 2c20 6e65   normal_dist, ne
-00015670: 775f 7369 7a65 2c20 6578 7061 6e64 3d46  w_size, expand=F
-00015680: 616c 7365 293a 0a20 2020 206e 6f72 6d61  alse):.    norma
-00015690: 6c5f 6469 7374 2c20 7369 676d 612c 2073  l_dist, sigma, s
-000156a0: 7570 706f 7274 5f73 6861 7065 203d 206e  upport_shape = n
-000156b0: 6f72 6d61 6c5f 6469 7374 2e6f 776e 6572  ormal_dist.owner
-000156c0: 2e69 6e70 7574 730a 0a20 2020 2069 6620  .inputs..    if 
-000156d0: 6578 7061 6e64 3a0a 2020 2020 2020 2020  expand:.        
-000156e0: 6f72 6967 696e 616c 5f73 6861 7065 203d  original_shape =
-000156f0: 2074 7570 6c65 286e 6f72 6d61 6c5f 6469   tuple(normal_di
-00015700: 7374 2e73 6861 7065 290a 2020 2020 2020  st.shape).      
-00015710: 2020 6f6c 645f 7369 7a65 203d 206f 7269    old_size = ori
-00015720: 6769 6e61 6c5f 7368 6170 655b 3a20 6c65  ginal_shape[: le
-00015730: 6e28 6f72 6967 696e 616c 5f73 6861 7065  n(original_shape
-00015740: 2920 2d20 6f70 2e6e 6469 6d5f 7375 7070  ) - op.ndim_supp
-00015750: 5d0a 2020 2020 2020 2020 6e65 775f 7369  ].        new_si
-00015760: 7a65 203d 2074 7570 6c65 286e 6577 5f73  ze = tuple(new_s
-00015770: 697a 6529 202b 206f 6c64 5f73 697a 650a  ize) + old_size.
-00015780: 0a20 2020 2072 6574 7572 6e20 5a65 726f  .    return Zero
-00015790: 5375 6d4e 6f72 6d61 6c2e 7276 5f6f 7028  SumNormal.rv_op(
-000157a0: 0a20 2020 2020 2020 2073 6967 6d61 3d73  .        sigma=s
-000157b0: 6967 6d61 2c20 6e5f 7a65 726f 7375 6d5f  igma, n_zerosum_
-000157c0: 6178 6573 3d6f 702e 6e64 696d 5f73 7570  axes=op.ndim_sup
-000157d0: 702c 2073 7570 706f 7274 5f73 6861 7065  p, support_shape
-000157e0: 3d73 7570 706f 7274 5f73 6861 7065 2c20  =support_shape, 
-000157f0: 7369 7a65 3d6e 6577 5f73 697a 650a 2020  size=new_size.  
-00015800: 2020 290a 0a0a 405f 6d6f 6d65 6e74 2e72    )...@_moment.r
-00015810: 6567 6973 7465 7228 5a65 726f 5375 6d4e  egister(ZeroSumN
-00015820: 6f72 6d61 6c52 5629 0a64 6566 207a 6572  ormalRV).def zer
-00015830: 6f73 756d 6e6f 726d 616c 5f6d 6f6d 656e  osumnormal_momen
-00015840: 7428 6f70 2c20 7276 2c20 2a72 765f 696e  t(op, rv, *rv_in
-00015850: 7075 7473 293a 0a20 2020 2072 6574 7572  puts):.    retur
-00015860: 6e20 7074 2e7a 6572 6f73 5f6c 696b 6528  n pt.zeros_like(
-00015870: 7276 290a 0a0a 405f 6465 6661 756c 745f  rv)...@_default_
-00015880: 7472 616e 7366 6f72 6d2e 7265 6769 7374  transform.regist
-00015890: 6572 285a 6572 6f53 756d 4e6f 726d 616c  er(ZeroSumNormal
-000158a0: 5256 290a 6465 6620 7a65 726f 7375 6d5f  RV).def zerosum_
-000158b0: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
-000158c0: 6d28 6f70 2c20 7276 293a 0a20 2020 206e  m(op, rv):.    n
-000158d0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
-000158e0: 7475 706c 6528 6e70 2e61 7261 6e67 6528  tuple(np.arange(
-000158f0: 2d6f 702e 6e64 696d 5f73 7570 702c 2030  -op.ndim_supp, 0
-00015900: 2929 0a20 2020 2072 6574 7572 6e20 5a65  )).    return Ze
-00015910: 726f 5375 6d54 7261 6e73 666f 726d 286e  roSumTransform(n
-00015920: 5f7a 6572 6f73 756d 5f61 7865 7329 0a0a  _zerosum_axes)..
-00015930: 0a40 5f6c 6f67 7072 6f62 2e72 6567 6973  .@_logprob.regis
-00015940: 7465 7228 5a65 726f 5375 6d4e 6f72 6d61  ter(ZeroSumNorma
-00015950: 6c52 5629 0a64 6566 207a 6572 6f73 756d  lRV).def zerosum
-00015960: 6e6f 726d 616c 5f6c 6f67 7028 6f70 2c20  normal_logp(op, 
-00015970: 7661 6c75 6573 2c20 6e6f 726d 616c 5f64  values, normal_d
-00015980: 6973 742c 2073 6967 6d61 2c20 7375 7070  ist, sigma, supp
-00015990: 6f72 745f 7368 6170 652c 202a 2a6b 7761  ort_shape, **kwa
-000159a0: 7267 7329 3a0a 2020 2020 2876 616c 7565  rgs):.    (value
-000159b0: 2c29 203d 2076 616c 7565 730a 2020 2020  ,) = values.    
-000159c0: 7368 6170 6520 3d20 7661 6c75 652e 7368  shape = value.sh
-000159d0: 6170 650a 2020 2020 6e5f 7a65 726f 7375  ape.    n_zerosu
-000159e0: 6d5f 6178 6573 203d 206f 702e 6e64 696d  m_axes = op.ndim
-000159f0: 5f73 7570 700a 0a20 2020 205f 6465 675f  _supp..    _deg_
-00015a00: 6672 6565 5f73 7570 706f 7274 5f73 6861  free_support_sha
-00015a10: 7065 203d 2070 742e 696e 635f 7375 6274  pe = pt.inc_subt
-00015a20: 656e 736f 7228 7368 6170 655b 2d6e 5f7a  ensor(shape[-n_z
-00015a30: 6572 6f73 756d 5f61 7865 733a 5d2c 202d  erosum_axes:], -
-00015a40: 3129 0a20 2020 205f 6675 6c6c 5f73 697a  1).    _full_siz
-00015a50: 6520 3d20 7074 2e70 726f 6428 7368 6170  e = pt.prod(shap
-00015a60: 6529 0a20 2020 205f 6465 6772 6565 735f  e).    _degrees_
-00015a70: 6f66 5f66 7265 6564 6f6d 203d 2070 742e  of_freedom = pt.
-00015a80: 7072 6f64 285f 6465 675f 6672 6565 5f73  prod(_deg_free_s
-00015a90: 7570 706f 7274 5f73 6861 7065 290a 0a20  upport_shape).. 
-00015aa0: 2020 207a 6572 6f73 756d 7320 3d20 5b0a     zerosums = [.
-00015ab0: 2020 2020 2020 2020 7074 2e61 6c6c 2870          pt.all(p
-00015ac0: 742e 6973 636c 6f73 6528 7074 2e6d 6561  t.isclose(pt.mea
-00015ad0: 6e28 7661 6c75 652c 2061 7869 733d 2d61  n(value, axis=-a
-00015ae0: 7869 7320 2d20 3129 2c20 302c 2061 746f  xis - 1), 0, ato
-00015af0: 6c3d 3165 2d39 2929 0a20 2020 2020 2020  l=1e-9)).       
-00015b00: 2066 6f72 2061 7869 7320 696e 2072 616e   for axis in ran
-00015b10: 6765 286e 5f7a 6572 6f73 756d 5f61 7865  ge(n_zerosum_axe
-00015b20: 7329 0a20 2020 205d 0a0a 2020 2020 6f75  s).    ]..    ou
-00015b30: 7420 3d20 7074 2e73 756d 280a 2020 2020  t = pt.sum(.    
-00015b40: 2020 2020 706d 2e6c 6f67 7028 6e6f 726d      pm.logp(norm
-00015b50: 616c 5f64 6973 742c 2076 616c 7565 2920  al_dist, value) 
-00015b60: 2a20 5f64 6567 7265 6573 5f6f 665f 6672  * _degrees_of_fr
-00015b70: 6565 646f 6d20 2f20 5f66 756c 6c5f 7369  eedom / _full_si
-00015b80: 7a65 2c0a 2020 2020 2020 2020 6178 6973  ze,.        axis
-00015b90: 3d74 7570 6c65 286e 702e 6172 616e 6765  =tuple(np.arange
-00015ba0: 282d 6e5f 7a65 726f 7375 6d5f 6178 6573  (-n_zerosum_axes
-00015bb0: 2c20 3029 292c 0a20 2020 2029 0a0a 2020  , 0)),.    )..  
-00015bc0: 2020 7265 7475 726e 2063 6865 636b 5f70    return check_p
-00015bd0: 6172 616d 6574 6572 7328 6f75 742c 202a  arameters(out, *
-00015be0: 7a65 726f 7375 6d73 2c20 6d73 673d 226d  zerosums, msg="m
-00015bf0: 6561 6e28 7661 6c75 652c 2061 7869 733d  ean(value, axis=
-00015c00: 6e5f 7a65 726f 7375 6d5f 6178 6573 2920  n_zerosum_axes) 
-00015c10: 3d20 3022 290a                           = 0").
+0000cd70: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 5375  =========.    Su
+0000cd80: 7070 6f72 7420 2020 5570 7065 7220 7472  pport   Upper tr
+0000cd90: 6961 6e67 756c 6172 206d 6174 7269 7820  iangular matrix 
+0000cda0: 7769 7468 2076 616c 7565 7320 696e 205b  with values in [
+0000cdb0: 2d31 2c20 315d 0a20 2020 203d 3d3d 3d3d  -1, 1].    =====
+0000cdc0: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+0000cdd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cde0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cdf0: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
+0000ce00: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+0000ce10: 2d2d 0a20 2020 206e 203a 2074 656e 736f  --.    n : tenso
+0000ce20: 725f 6c69 6b65 206f 6620 696e 740a 2020  r_like of int.  
+0000ce30: 2020 2020 2020 4469 6d65 6e73 696f 6e20        Dimension 
+0000ce40: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
+0000ce50: 6520 6d61 7472 6978 2028 6e20 3e20 3129  e matrix (n > 1)
+0000ce60: 2e0a 2020 2020 6574 6120 3a20 7465 6e73  ..    eta : tens
+0000ce70: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+0000ce80: 0a20 2020 2020 2020 2054 6865 2073 6861  .        The sha
+0000ce90: 7065 2070 6172 616d 6574 6572 2028 6574  pe parameter (et
+0000cea0: 6120 3e20 3029 206f 6620 7468 6520 4c4b  a > 0) of the LK
+0000ceb0: 4a20 6469 7374 7269 6275 7469 6f6e 2e20  J distribution. 
+0000cec0: 6574 6120 3d20 310a 2020 2020 2020 2020  eta = 1.        
+0000ced0: 696d 706c 6965 7320 6120 756e 6966 6f72  implies a unifor
+0000cee0: 6d20 6469 7374 7269 6275 7469 6f6e 206f  m distribution o
+0000cef0: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
+0000cf00: 6e20 6d61 7472 6963 6573 3b0a 2020 2020  n matrices;.    
+0000cf10: 2020 2020 6c61 7267 6572 2076 616c 7565      larger value
+0000cf20: 7320 7075 7420 6d6f 7265 2077 6569 6768  s put more weigh
+0000cf30: 7420 6f6e 206d 6174 7269 6365 7320 7769  t on matrices wi
+0000cf40: 7468 2066 6577 2063 6f72 7265 6c61 7469  th few correlati
+0000cf50: 6f6e 732e 0a0a 2020 2020 4e6f 7465 730a  ons...    Notes.
+0000cf60: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
+0000cf70: 6973 2069 6d70 6c65 6d65 6e74 6174 696f  is implementatio
+0000cf80: 6e20 6f6e 6c79 2072 6574 7572 6e73 2074  n only returns t
+0000cf90: 6865 2076 616c 7565 7320 6f66 2074 6865  he values of the
+0000cfa0: 2075 7070 6572 2074 7269 616e 6775 6c61   upper triangula
+0000cfb0: 720a 2020 2020 6d61 7472 6978 2065 7863  r.    matrix exc
+0000cfc0: 6c75 6469 6e67 2074 6865 2064 6961 676f  luding the diago
+0000cfd0: 6e61 6c2e 2048 6572 6520 6973 2061 2073  nal. Here is a s
+0000cfe0: 6368 656d 6174 6963 2066 6f72 206e 203d  chematic for n =
+0000cff0: 2035 2c20 7368 6f77 696e 670a 2020 2020   5, showing.    
+0000d000: 7468 6520 696e 6465 7865 7320 6f66 2074  the indexes of t
+0000d010: 6865 2065 6c65 6d65 6e74 733a 3a0a 0a20  he elements::.. 
+0000d020: 2020 2020 2020 205b 5b2d 2030 2031 2032         [[- 0 1 2
+0000d030: 2033 5d0a 2020 2020 2020 2020 205b 2d20   3].         [- 
+0000d040: 2d20 3420 3520 365d 0a20 2020 2020 2020  - 4 5 6].       
+0000d050: 2020 5b2d 202d 202d 2037 2038 5d0a 2020    [- - - 7 8].  
+0000d060: 2020 2020 2020 205b 2d20 2d20 2d20 2d20         [- - - - 
+0000d070: 395d 0a20 2020 2020 2020 2020 5b2d 202d  9].         [- -
+0000d080: 202d 202d 202d 5d5d 0a0a 0a20 2020 2052   - - -]]...    R
+0000d090: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
+0000d0a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
+0000d0b0: 5b4c 4b4a 3230 3039 5d20 4c65 7761 6e64  [LKJ2009] Lewand
+0000d0c0: 6f77 736b 692c 2044 2e2c 204b 7572 6f77  owski, D., Kurow
+0000d0d0: 6963 6b61 2c20 442e 2061 6e64 204a 6f65  icka, D. and Joe
+0000d0e0: 2c20 482e 2028 3230 3039 292e 0a20 2020  , H. (2009)..   
+0000d0f0: 2020 2020 2022 4765 6e65 7261 7469 6e67       "Generating
+0000d100: 2072 616e 646f 6d20 636f 7272 656c 6174   random correlat
+0000d110: 696f 6e20 6d61 7472 6963 6573 2062 6173  ion matrices bas
+0000d120: 6564 206f 6e20 7669 6e65 7320 616e 640a  ed on vines and.
+0000d130: 2020 2020 2020 2020 6578 7465 6e64 6564          extended
+0000d140: 206f 6e69 6f6e 206d 6574 686f 642e 2220   onion method." 
+0000d150: 4a6f 7572 6e61 6c20 6f66 206d 756c 7469  Journal of multi
+0000d160: 7661 7269 6174 6520 616e 616c 7973 6973  variate analysis
+0000d170: 2c0a 2020 2020 2020 2020 3130 3028 3929  ,.        100(9)
+0000d180: 2c20 7070 2e31 3938 392d 3230 3031 2e0a  , pp.1989-2001..
+0000d190: 2020 2020 2222 220a 0a20 2020 2072 765f      """..    rv_
+0000d1a0: 6f70 203d 206c 6b6a 636f 7272 0a0a 2020  op = lkjcorr..  
+0000d1b0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+0000d1c0: 2020 2064 6566 2064 6973 7428 636c 732c     def dist(cls,
+0000d1d0: 206e 2c20 6574 612c 202a 2a6b 7761 7267   n, eta, **kwarg
+0000d1e0: 7329 3a0a 2020 2020 2020 2020 6e20 3d20  s):.        n = 
+0000d1f0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+0000d200: 6961 626c 6528 696e 7458 286e 2929 0a20  iable(intX(n)). 
+0000d210: 2020 2020 2020 2065 7461 203d 2070 742e         eta = pt.
+0000d220: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+0000d230: 6c65 2866 6c6f 6174 5828 6574 6129 290a  le(floatX(eta)).
+0000d240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d250: 7570 6572 2829 2e64 6973 7428 5b6e 2c20  uper().dist([n, 
+0000d260: 6574 615d 2c20 2a2a 6b77 6172 6773 290a  eta], **kwargs).
+0000d270: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
+0000d280: 7276 2c20 2a61 7267 7329 3a0a 2020 2020  rv, *args):.    
+0000d290: 2020 2020 7265 7475 726e 2070 742e 7a65      return pt.ze
+0000d2a0: 726f 735f 6c69 6b65 2872 7629 0a0a 2020  ros_like(rv)..  
+0000d2b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+0000d2c0: 2c20 6e2c 2065 7461 293a 0a20 2020 2020  , n, eta):.     
+0000d2d0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000d2e0: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
+0000d2f0: 6261 6269 6c69 7479 206f 6620 4c4b 4a20  bability of LKJ 
+0000d300: 6469 7374 7269 6275 7469 6f6e 2061 7420  distribution at 
+0000d310: 7370 6563 6966 6965 640a 2020 2020 2020  specified.      
+0000d320: 2020 7661 6c75 652e 0a0a 2020 2020 2020    value...      
+0000d330: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000d340: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000d350: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
+0000d360: 756d 6572 6963 0a20 2020 2020 2020 2020  umeric.         
+0000d370: 2020 2056 616c 7565 2066 6f72 2077 6869     Value for whi
+0000d380: 6368 206c 6f67 2d70 726f 6261 6269 6c69  ch log-probabili
+0000d390: 7479 2069 7320 6361 6c63 756c 6174 6564  ty is calculated
+0000d3a0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000d3b0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000d3c0: 2d2d 0a20 2020 2020 2020 2054 656e 736f  --.        Tenso
+0000d3d0: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
+0000d3e0: 2020 2222 220a 0a20 2020 2020 2020 2023    """..        #
+0000d3f0: 2054 4f44 4f3a 2050 7954 656e 736f 7220   TODO: PyTensor 
+0000d400: 646f 6573 206e 6f74 2068 6176 6520 6120  does not have a 
+0000d410: 6074 7269 755f 696e 6469 6365 7360 2c20  `triu_indices`, 
+0000d420: 736f 2077 6520 6361 6e20 6f6e 6c79 2077  so we can only w
+0000d430: 6f72 6b20 7769 7468 2063 6f6e 7374 616e  ork with constan
+0000d440: 740a 2020 2020 2020 2020 2320 206e 2028  t.        #  n (
+0000d450: 6f72 2065 6c73 6520 6669 6e64 2061 2064  or else find a d
+0000d460: 6966 6665 7265 6e74 2065 7870 7265 7373  ifferent express
+0000d470: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+0000d480: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
+0000d490: 2c20 436f 6e73 7461 6e74 293a 0a20 2020  , Constant):.   
+0000d4a0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+0000d4b0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+0000d4c0: 6f72 2822 6c6f 6770 206f 6e6c 7920 696d  or("logp only im
+0000d4d0: 706c 656d 656e 7465 6420 666f 7220 636f  plemented for co
+0000d4e0: 6e73 7461 6e74 2060 6e60 2229 0a0a 2020  nstant `n`")..  
+0000d4f0: 2020 2020 2020 6e20 3d20 696e 7428 6e2e        n = int(n.
+0000d500: 6461 7461 290a 2020 2020 2020 2020 7368  data).        sh
+0000d510: 6170 6520 3d20 6e20 2a20 286e 202d 2031  ape = n * (n - 1
+0000d520: 2920 2f2f 2032 0a20 2020 2020 2020 2074  ) // 2.        t
+0000d530: 7269 5f69 6e64 6578 203d 206e 702e 7a65  ri_index = np.ze
+0000d540: 726f 7328 286e 2c20 6e29 2c20 6474 7970  ros((n, n), dtyp
+0000d550: 653d 2269 6e74 3332 2229 0a20 2020 2020  e="int32").     
+0000d560: 2020 2074 7269 5f69 6e64 6578 5b6e 702e     tri_index[np.
+0000d570: 7472 6975 5f69 6e64 6963 6573 286e 2c20  triu_indices(n, 
+0000d580: 6b3d 3129 5d20 3d20 6e70 2e61 7261 6e67  k=1)] = np.arang
+0000d590: 6528 7368 6170 6529 0a20 2020 2020 2020  e(shape).       
+0000d5a0: 2074 7269 5f69 6e64 6578 5b6e 702e 7472   tri_index[np.tr
+0000d5b0: 6975 5f69 6e64 6963 6573 286e 2c20 6b3d  iu_indices(n, k=
+0000d5c0: 3129 5b3a 3a2d 315d 5d20 3d20 6e70 2e61  1)[::-1]] = np.a
+0000d5d0: 7261 6e67 6528 7368 6170 6529 0a0a 2020  range(shape)..  
+0000d5e0: 2020 2020 2020 7661 6c75 6520 3d20 7074        value = pt
+0000d5f0: 2e74 616b 6528 7661 6c75 652c 2074 7269  .take(value, tri
+0000d600: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
+0000d610: 7661 6c75 6520 3d20 7074 2e66 696c 6c5f  value = pt.fill_
+0000d620: 6469 6167 6f6e 616c 2876 616c 7565 2c20  diagonal(value, 
+0000d630: 3129 0a0a 2020 2020 2020 2020 2320 544f  1)..        # TO
+0000d640: 444f 3a20 5f6c 6b6a 5f6e 6f72 6d61 6c69  DO: _lkj_normali
+0000d650: 7a69 6e67 5f63 6f6e 7374 616e 7420 6375  zing_constant cu
+0000d660: 7272 656e 746c 7920 7265 7175 6972 6573  rrently requires
+0000d670: 2060 6574 6160 2061 6e64 2060 6e60 2074   `eta` and `n` t
+0000d680: 6f20 6265 2063 6f6e 7374 616e 7473 0a20  o be constants. 
+0000d690: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000d6a0: 696e 7374 616e 6365 2865 7461 2c20 436f  instance(eta, Co
+0000d6b0: 6e73 7461 6e74 293a 0a20 2020 2020 2020  nstant):.       
+0000d6c0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+0000d6d0: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
+0000d6e0: 6c6f 6770 206f 6e6c 7920 696d 706c 656d  logp only implem
+0000d6f0: 656e 7465 6420 666f 7220 636f 6e73 7461  ented for consta
+0000d700: 6e74 2060 6574 6160 2229 0a20 2020 2020  nt `eta`").     
+0000d710: 2020 2065 7461 203d 2066 6c6f 6174 2865     eta = float(e
+0000d720: 7461 2e64 6174 6129 0a20 2020 2020 2020  ta.data).       
+0000d730: 2072 6573 756c 7420 3d20 5f6c 6b6a 5f6e   result = _lkj_n
+0000d740: 6f72 6d61 6c69 7a69 6e67 5f63 6f6e 7374  ormalizing_const
+0000d750: 616e 7428 6574 612c 206e 290a 2020 2020  ant(eta, n).    
+0000d760: 2020 2020 7265 7375 6c74 202b 3d20 2865      result += (e
+0000d770: 7461 202d 2031 2e30 2920 2a20 7074 2e6c  ta - 1.0) * pt.l
+0000d780: 6f67 2864 6574 2876 616c 7565 2929 0a20  og(det(value)). 
+0000d790: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+0000d7a0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
+0000d7b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000d7c0: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
+0000d7d0: 7661 6c75 6520 3e3d 202d 312c 0a20 2020  value >= -1,.   
+0000d7e0: 2020 2020 2020 2020 2076 616c 7565 203c           value <
+0000d7f0: 3d20 312c 0a20 2020 2020 2020 2020 2020  = 1,.           
+0000d800: 206d 6174 7269 785f 706f 735f 6465 6628   matrix_pos_def(
+0000d810: 7661 6c75 6529 2c0a 2020 2020 2020 2020  value),.        
+0000d820: 2020 2020 6574 6120 3e20 302c 0a20 2020      eta > 0,.   
+0000d830: 2020 2020 2029 0a0a 0a40 5f64 6566 6175       )...@_defau
+0000d840: 6c74 5f74 7261 6e73 666f 726d 2e72 6567  lt_transform.reg
+0000d850: 6973 7465 7228 4c4b 4a43 6f72 7229 0a64  ister(LKJCorr).d
+0000d860: 6566 206c 6b6a 636f 7272 5f64 6566 6175  ef lkjcorr_defau
+0000d870: 6c74 5f74 7261 6e73 666f 726d 286f 702c  lt_transform(op,
+0000d880: 2072 7629 3a0a 2020 2020 7265 7475 726e   rv):.    return
+0000d890: 2049 6e74 6572 7661 6c28 666c 6f61 7458   Interval(floatX
+0000d8a0: 282d 312e 3029 2c20 666c 6f61 7458 2831  (-1.0), floatX(1
+0000d8b0: 2e30 2929 0a0a 0a63 6c61 7373 204d 6174  .0))...class Mat
+0000d8c0: 7269 784e 6f72 6d61 6c52 5628 5261 6e64  rixNormalRV(Rand
+0000d8d0: 6f6d 5661 7269 6162 6c65 293a 0a20 2020  omVariable):.   
+0000d8e0: 206e 616d 6520 3d20 226d 6174 7269 786e   name = "matrixn
+0000d8f0: 6f72 6d61 6c22 0a20 2020 206e 6469 6d5f  ormal".    ndim_
+0000d900: 7375 7070 203d 2032 0a20 2020 206e 6469  supp = 2.    ndi
+0000d910: 6d73 5f70 6172 616d 7320 3d20 5b32 2c20  ms_params = [2, 
+0000d920: 322c 2032 5d0a 2020 2020 6474 7970 6520  2, 2].    dtype 
+0000d930: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
+0000d940: 7072 696e 745f 6e61 6d65 203d 2028 224d  print_name = ("M
+0000d950: 6174 7269 784e 6f72 6d61 6c22 2c20 225c  atrixNormal", "\
+0000d960: 5c6f 7065 7261 746f 726e 616d 657b 4d61  \operatorname{Ma
+0000d970: 7472 6978 4e6f 726d 616c 7d22 290a 0a20  trixNormal}").. 
+0000d980: 2020 2064 6566 205f 696e 6665 725f 7368     def _infer_sh
+0000d990: 6170 6528 7365 6c66 2c20 7369 7a65 2c20  ape(self, size, 
+0000d9a0: 6469 7374 5f70 6172 616d 732c 2070 6172  dist_params, par
+0000d9b0: 616d 5f73 6861 7065 733d 4e6f 6e65 293a  am_shapes=None):
+0000d9c0: 0a20 2020 2020 2020 2073 6861 7065 203d  .        shape =
+0000d9d0: 2074 7570 6c65 2873 697a 6529 202b 2074   tuple(size) + t
+0000d9e0: 7570 6c65 2864 6973 745f 7061 7261 6d73  uple(dist_params
+0000d9f0: 5b30 5d2e 7368 6170 655b 2d32 3a5d 290a  [0].shape[-2:]).
+0000da00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000da10: 6861 7065 0a0a 2020 2020 4063 6c61 7373  hape..    @class
+0000da20: 6d65 7468 6f64 0a20 2020 2064 6566 2072  method.    def r
+0000da30: 6e67 5f66 6e28 636c 732c 2072 6e67 2c20  ng_fn(cls, rng, 
+0000da40: 6d75 2c20 726f 7763 686f 6c2c 2063 6f6c  mu, rowchol, col
+0000da50: 6368 6f6c 2c20 7369 7a65 3d4e 6f6e 6529  chol, size=None)
+0000da60: 3a0a 2020 2020 2020 2020 7369 7a65 203d  :.        size =
+0000da70: 2074 6f5f 7475 706c 6528 7369 7a65 290a   to_tuple(size).
+0000da80: 2020 2020 2020 2020 6469 7374 5f73 6861          dist_sha
+0000da90: 7065 203d 2074 6f5f 7475 706c 6528 5b72  pe = to_tuple([r
+0000daa0: 6f77 6368 6f6c 2e73 6861 7065 5b30 5d2c  owchol.shape[0],
+0000dab0: 2063 6f6c 6368 6f6c 2e73 6861 7065 5b30   colchol.shape[0
+0000dac0: 5d5d 290a 2020 2020 2020 2020 6f75 7470  ]]).        outp
+0000dad0: 7574 5f73 6861 7065 203d 2073 697a 6520  ut_shape = size 
+0000dae0: 2b20 6469 7374 5f73 6861 7065 0a0a 2020  + dist_shape..  
+0000daf0: 2020 2020 2020 2320 4272 6f61 6463 6173        # Broadcas
+0000db00: 7469 6e67 2061 6c6c 2070 6172 616d 6574  ting all paramet
+0000db10: 6572 730a 2020 2020 2020 2020 7368 6170  ers.        shap
+0000db20: 6573 203d 205b 6d75 2e73 6861 7065 2c20  es = [mu.shape, 
+0000db30: 6f75 7470 7574 5f73 6861 7065 5d0a 2020  output_shape].  
+0000db40: 2020 2020 2020 6272 6f61 6463 6173 7461        broadcasta
+0000db50: 626c 655f 7368 6170 6520 3d20 6272 6f61  ble_shape = broa
+0000db60: 6463 6173 745f 6469 7374 5f73 616d 706c  dcast_dist_sampl
+0000db70: 6573 5f73 6861 7065 2873 6861 7065 732c  es_shape(shapes,
+0000db80: 2073 697a 653d 7369 7a65 290a 2020 2020   size=size).    
+0000db90: 2020 2020 6d75 203d 206e 702e 6272 6f61      mu = np.broa
+0000dba0: 6463 6173 745f 746f 286d 752c 2073 6861  dcast_to(mu, sha
+0000dbb0: 7065 3d62 726f 6164 6361 7374 6162 6c65  pe=broadcastable
+0000dbc0: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
+0000dbd0: 726f 7763 686f 6c20 3d20 6e70 2e62 726f  rowchol = np.bro
+0000dbe0: 6164 6361 7374 5f74 6f28 726f 7763 686f  adcast_to(rowcho
+0000dbf0: 6c2c 2073 6861 7065 3d73 697a 6520 2b20  l, shape=size + 
+0000dc00: 726f 7763 686f 6c2e 7368 6170 655b 2d32  rowchol.shape[-2
+0000dc10: 3a5d 290a 0a20 2020 2020 2020 2063 6f6c  :])..        col
+0000dc20: 6368 6f6c 203d 206e 702e 6272 6f61 6463  chol = np.broadc
+0000dc30: 6173 745f 746f 2863 6f6c 6368 6f6c 2c20  ast_to(colchol, 
+0000dc40: 7368 6170 653d 7369 7a65 202b 2063 6f6c  shape=size + col
+0000dc50: 6368 6f6c 2e73 6861 7065 5b2d 323a 5d29  chol.shape[-2:])
+0000dc60: 0a20 2020 2020 2020 2063 6f6c 6368 6f6c  .        colchol
+0000dc70: 203d 206e 702e 7377 6170 6178 6573 2863   = np.swapaxes(c
+0000dc80: 6f6c 6368 6f6c 2c20 2d31 2c20 2d32 2920  olchol, -1, -2) 
+0000dc90: 2023 2054 616b 6520 7472 616e 7370 6f73   # Take transpos
+0000dca0: 650a 0a20 2020 2020 2020 2073 7461 6e64  e..        stand
+0000dcb0: 6172 645f 6e6f 726d 616c 203d 2072 6e67  ard_normal = rng
+0000dcc0: 2e73 7461 6e64 6172 645f 6e6f 726d 616c  .standard_normal
+0000dcd0: 286f 7574 7075 745f 7368 6170 6529 0a20  (output_shape). 
+0000dce0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
+0000dcf0: 206d 7520 2b20 6e70 2e6d 6174 6d75 6c28   mu + np.matmul(
+0000dd00: 726f 7763 686f 6c2c 206e 702e 6d61 746d  rowchol, np.matm
+0000dd10: 756c 2873 7461 6e64 6172 645f 6e6f 726d  ul(standard_norm
+0000dd20: 616c 2c20 636f 6c63 686f 6c29 290a 0a20  al, colchol)).. 
+0000dd30: 2020 2020 2020 2072 6574 7572 6e20 7361         return sa
+0000dd40: 6d70 6c65 730a 0a0a 6d61 7472 6978 6e6f  mples...matrixno
+0000dd50: 726d 616c 203d 204d 6174 7269 784e 6f72  rmal = MatrixNor
+0000dd60: 6d61 6c52 5628 290a 0a0a 636c 6173 7320  malRV()...class 
+0000dd70: 4d61 7472 6978 4e6f 726d 616c 2843 6f6e  MatrixNormal(Con
+0000dd80: 7469 6e75 6f75 7329 3a0a 2020 2020 7222  tinuous):.    r"
+0000dd90: 2222 0a20 2020 204d 6174 7269 782d 7661  "".    Matrix-va
+0000dda0: 6c75 6564 206e 6f72 6d61 6c20 6c6f 672d  lued normal log-
+0000ddb0: 6c69 6b65 6c69 686f 6f64 2e0a 0a20 2020  likelihood...   
+0000ddc0: 202e 2e20 6d61 7468 3a3a 0a20 2020 2020   .. math::.     
+0000ddd0: 2020 6628 7820 5c6d 6964 205c 6d75 2c20    f(x \mid \mu, 
+0000dde0: 552c 2056 2920 3d0a 2020 2020 2020 2020  U, V) =.        
+0000ddf0: 2020 205c 6672 6163 7b31 7d7b 2832 5c70     \frac{1}{(2\p
+0000de00: 695e 7b6d 206e 7d20 7c55 7c5e 6e20 7c56  i^{m n} |U|^n |V
+0000de10: 7c5e 6d29 5e7b 312f 327d 7d0a 2020 2020  |^m)^{1/2}}.    
+0000de20: 2020 2020 2020 205c 6578 705c 6c65 6674         \exp\left
+0000de30: 5c7b 0a20 2020 2020 2020 2020 2020 2020  \{.             
+0000de40: 2020 202d 5c66 7261 637b 317d 7b32 7d20     -\frac{1}{2} 
+0000de50: 5c6d 6174 6872 6d7b 5472 7d5b 2056 5e7b  \mathrm{Tr}[ V^{
+0000de60: 2d31 7d20 2878 2d5c 6d75 295e 7b5c 7072  -1} (x-\mu)^{\pr
+0000de70: 696d 657d 2055 5e7b 2d31 7d20 2878 2d5c  ime} U^{-1} (x-\
+0000de80: 6d75 295d 0a20 2020 2020 2020 2020 2020  mu)].           
+0000de90: 205c 7269 6768 745c 7d0a 0a20 2020 203d   \right\}..    =
+0000dea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020  ==============  
+0000deb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000dec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ded0: 3d3d 3d3d 3d0a 2020 2020 5375 7070 6f72  =====.    Suppor
+0000dee0: 7420 2020 2020 2020 2020 203a 6d61 7468  t          :math
+0000def0: 3a60 7820 5c69 6e20 5c6d 6174 6862 627b  :`x \in \mathbb{
+0000df00: 527d 5e7b 6d20 5c74 696d 6573 206e 7d60  R}^{m \times n}`
+0000df10: 0a20 2020 204d 6561 6e20 2020 2020 2020  .    Mean       
+0000df20: 2020 2020 2020 3a6d 6174 683a 605c 6d75        :math:`\mu
+0000df30: 600a 2020 2020 526f 7720 5661 7269 616e  `.    Row Varian
+0000df40: 6365 2020 2020 203a 6d61 7468 3a60 5560  ce     :math:`U`
+0000df50: 0a20 2020 2043 6f6c 756d 6e20 5661 7269  .    Column Vari
+0000df60: 616e 6365 2020 3a6d 6174 683a 6056 600a  ance  :math:`V`.
+0000df70: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
+0000df80: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+0000df90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000dfa0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+0000dfb0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000dfc0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75  ---------.    mu
+0000dfd0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+0000dfe0: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+0000dff0: 4172 7261 7920 6f66 206d 6561 6e73 2e20  Array of means. 
+0000e000: 4d75 7374 2062 6520 6272 6f61 6463 6173  Must be broadcas
+0000e010: 7461 626c 6520 7769 7468 2074 6865 2072  table with the r
+0000e020: 616e 646f 6d20 7661 7269 6162 6c65 2058  andom variable X
+0000e030: 2073 7563 680a 2020 2020 2020 2020 7468   such.        th
+0000e040: 6174 2074 6865 2073 6861 7065 206f 6620  at the shape of 
+0000e050: 6d75 202b 2058 2069 7320 284d 2c20 4e29  mu + X is (M, N)
+0000e060: 2e0a 2020 2020 726f 7763 6f76 203a 2028  ..    rowcov : (
+0000e070: 4d2c 204d 2920 7465 6e73 6f72 5f6c 696b  M, M) tensor_lik
+0000e080: 6520 6f66 2066 6c6f 6174 2c20 6f70 7469  e of float, opti
+0000e090: 6f6e 616c 0a20 2020 2020 2020 2041 6d6f  onal.        Amo
+0000e0a0: 6e67 2d72 6f77 2063 6f76 6172 6961 6e63  ng-row covarianc
+0000e0b0: 6520 6d61 7472 6978 2e20 4465 6669 6e65  e matrix. Define
+0000e0c0: 7320 7661 7269 616e 6365 2077 6974 6869  s variance withi
+0000e0d0: 6e0a 2020 2020 2020 2020 636f 6c75 6d6e  n.        column
+0000e0e0: 732e 2045 7861 6374 6c79 206f 6e65 206f  s. Exactly one o
+0000e0f0: 6620 726f 7763 6f76 206f 7220 726f 7763  f rowcov or rowc
+0000e100: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
+0000e110: 2020 2072 6f77 6368 6f6c 203a 2028 4d2c     rowchol : (M,
+0000e120: 204d 2920 7465 6e73 6f72 5f6c 696b 6520   M) tensor_like 
+0000e130: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+0000e140: 616c 0a20 2020 2020 2020 2043 686f 6c65  al.        Chole
+0000e150: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
+0000e160: 6e20 6f66 2061 6d6f 6e67 2d72 6f77 2063  n of among-row c
+0000e170: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000e180: 2e20 4578 6163 746c 7920 6f6e 6520 6f66  . Exactly one of
+0000e190: 0a20 2020 2020 2020 2072 6f77 636f 7620  .        rowcov 
+0000e1a0: 6f72 2072 6f77 6368 6f6c 2069 7320 6e65  or rowchol is ne
+0000e1b0: 6564 6564 2e0a 2020 2020 636f 6c63 6f76  eded..    colcov
+0000e1c0: 203a 2028 4e2c 204e 2920 7465 6e73 6f72   : (N, N) tensor
+0000e1d0: 5f6c 696b 6520 6f66 2066 6c6f 6174 2c20  _like of float, 
+0000e1e0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000e1f0: 2041 6d6f 6e67 2d63 6f6c 756d 6e20 636f   Among-column co
+0000e200: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
+0000e210: 2049 6620 726f 7763 6f76 2069 7320 7468   If rowcov is th
+0000e220: 6520 6964 656e 7469 7479 206d 6174 7269  e identity matri
+0000e230: 782c 0a20 2020 2020 2020 2074 6869 7320  x,.        this 
+0000e240: 6675 6e63 7469 6f6e 7320 6173 2060 636f  functions as `co
+0000e250: 7660 2069 6e20 4d76 4e6f 726d 616c 2e0a  v` in MvNormal..
+0000e260: 2020 2020 2020 2020 4578 6163 746c 7920          Exactly 
+0000e270: 6f6e 6520 6f66 2063 6f6c 636f 7620 6f72  one of colcov or
+0000e280: 2063 6f6c 6368 6f6c 2069 7320 6e65 6564   colchol is need
+0000e290: 6564 2e0a 2020 2020 636f 6c63 686f 6c20  ed..    colchol 
+0000e2a0: 3a20 284e 2c20 4e29 2074 656e 736f 725f  : (N, N) tensor_
+0000e2b0: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+0000e2c0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000e2d0: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
+0000e2e0: 7369 7469 6f6e 206f 6620 616d 6f6e 672d  sition of among-
+0000e2f0: 636f 6c75 6d6e 2063 6f76 6172 6961 6e63  column covarianc
+0000e300: 6520 6d61 7472 6978 2e20 4578 6163 746c  e matrix. Exactl
+0000e310: 7920 6f6e 650a 2020 2020 2020 2020 6f66  y one.        of
+0000e320: 2063 6f6c 636f 7620 6f72 2063 6f6c 6368   colcov or colch
+0000e330: 6f6c 2069 7320 6e65 6564 6564 2e0a 0a20  ol is needed... 
+0000e340: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+0000e350: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
+0000e360: 696e 6520 6120 6d61 7472 6978 7661 7269  ine a matrixvari
+0000e370: 6174 6520 6e6f 726d 616c 2076 6172 6961  ate normal varia
+0000e380: 626c 6520 666f 7220 6769 7665 6e20 726f  ble for given ro
+0000e390: 7720 616e 6420 636f 6c75 6d6e 2063 6f76  w and column cov
+0000e3a0: 6172 6961 6e63 650a 2020 2020 6d61 7472  ariance.    matr
+0000e3b0: 6963 6573 3a3a 0a0a 2020 2020 2020 2020  ices::..        
+0000e3c0: 636f 6c63 6f76 203d 206e 702e 6172 7261  colcov = np.arra
+0000e3d0: 7928 5b5b 312e 2c20 302e 355d 2c20 5b30  y([[1., 0.5], [0
+0000e3e0: 2e35 2c20 325d 5d29 0a20 2020 2020 2020  .5, 2]]).       
+0000e3f0: 2072 6f77 636f 7620 3d20 6e70 2e61 7272   rowcov = np.arr
+0000e400: 6179 285b 5b31 2c20 302c 2030 5d2c 205b  ay([[1, 0, 0], [
+0000e410: 302c 2034 2c20 305d 2c20 5b30 2c20 302c  0, 4, 0], [0, 0,
+0000e420: 2031 365d 5d29 0a20 2020 2020 2020 206d   16]]).        m
+0000e430: 203d 2072 6f77 636f 762e 7368 6170 655b   = rowcov.shape[
+0000e440: 305d 0a20 2020 2020 2020 206e 203d 2063  0].        n = c
+0000e450: 6f6c 636f 762e 7368 6170 655b 305d 0a20  olcov.shape[0]. 
+0000e460: 2020 2020 2020 206d 7520 3d20 6e70 2e7a         mu = np.z
+0000e470: 6572 6f73 2828 6d2c 206e 2929 0a20 2020  eros((m, n)).   
+0000e480: 2020 2020 2076 616c 7320 3d20 706d 2e4d       vals = pm.M
+0000e490: 6174 7269 784e 6f72 6d61 6c28 2776 616c  atrixNormal('val
+0000e4a0: 7327 2c20 6d75 3d6d 752c 2063 6f6c 636f  s', mu=mu, colco
+0000e4b0: 763d 636f 6c63 6f76 2c0a 2020 2020 2020  v=colcov,.      
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 2020 2020 2020 2020 2072 6f77 636f 763d           rowcov=
+0000e4e0: 726f 7763 6f76 290a 0a20 2020 2041 626f  rowcov)..    Abo
+0000e4f0: 7665 2c20 7468 6520 6974 6820 726f 7720  ve, the ith row 
+0000e500: 696e 2076 616c 7320 6861 7320 6120 7661  in vals has a va
+0000e510: 7269 616e 6365 2074 6861 7420 6973 2073  riance that is s
+0000e520: 6361 6c65 6420 6279 2034 5e69 2e0a 2020  caled by 4^i..  
+0000e530: 2020 416c 7465 726e 6174 6976 656c 792c    Alternatively,
+0000e540: 2072 6f77 206f 7220 636f 6c75 6d6e 2063   row or column c
+0000e550: 686f 6c65 736b 7920 6d61 7472 6963 6573  holesky matrices
+0000e560: 2063 6f75 6c64 2062 6520 7375 6273 7469   could be substi
+0000e570: 7475 7465 6420 666f 720a 2020 2020 6569  tuted for.    ei
+0000e580: 7468 6572 2063 6f76 6172 6961 6e63 6520  ther covariance 
+0000e590: 6d61 7472 6978 2e20 5468 6520 4d61 7472  matrix. The Matr
+0000e5a0: 6978 4e6f 726d 616c 2069 7320 7175 6963  ixNormal is quic
+0000e5b0: 6b65 7220 7761 7920 636f 6d70 7574 650a  ker way compute.
+0000e5c0: 2020 2020 4d76 4e6f 726d 616c 286d 752c      MvNormal(mu,
+0000e5d0: 206e 702e 6b72 6f6e 2872 6f77 636f 762c   np.kron(rowcov,
+0000e5e0: 2063 6f6c 636f 7629 2920 7468 6174 2074   colcov)) that t
+0000e5f0: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
+0000e600: 6620 6b72 6f6e 6563 6b65 7220 7072 6f64  f kronecker prod
+0000e610: 7563 740a 2020 2020 7072 6f70 6572 7469  uct.    properti
+0000e620: 6573 2066 6f72 2069 6e76 6572 7369 6f6e  es for inversion
+0000e630: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
+0000e640: 6620 6472 6177 7320 6672 6f6d 204d 764e  f draws from MvN
+0000e650: 6f72 6d61 6c20 6861 6420 7468 6520 7361  ormal had the sa
+0000e660: 6d65 0a20 2020 2063 6f76 6172 6961 6e63  me.    covarianc
+0000e670: 6520 7374 7275 6374 7572 652c 2062 7574  e structure, but
+0000e680: 2077 6572 6520 7363 616c 6564 2062 7920   were scaled by 
+0000e690: 6469 6666 6572 656e 7420 706f 7765 7273  different powers
+0000e6a0: 206f 6620 616e 2075 6e6b 6e6f 776e 0a20   of an unknown. 
+0000e6b0: 2020 2063 6f6e 7374 616e 742c 2062 6f74     constant, bot
+0000e6c0: 6820 7468 6520 636f 7661 7269 616e 6365  h the covariance
+0000e6d0: 2061 6e64 2073 6361 6c69 6e67 2063 6f75   and scaling cou
+0000e6e0: 6c64 2062 6520 6c65 6172 6e65 6420 6173  ld be learned as
+0000e6f0: 2066 6f6c 6c6f 7773 0a20 2020 2028 7365   follows.    (se
+0000e700: 6520 7468 6520 646f 6373 7472 696e 6720  e the docstring 
+0000e710: 6f66 2060 4c4b 4a43 686f 6c65 736b 7943  of `LKJCholeskyC
+0000e720: 6f76 6020 666f 7220 6d6f 7265 2069 6e66  ov` for more inf
+0000e730: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
+0000e740: 6869 7329 0a0a 2020 2020 2e2e 2063 6f64  his)..    .. cod
+0000e750: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+0000e760: 2020 2020 2320 5365 7475 7020 6461 7461      # Setup data
+0000e770: 0a20 2020 2020 2020 2074 7275 655f 636f  .        true_co
+0000e780: 6c63 6f76 203d 206e 702e 6172 7261 7928  lcov = np.array(
+0000e790: 5b5b 312e 302c 2030 2e35 2c20 302e 315d  [[1.0, 0.5, 0.1]
+0000e7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 5b30 2e35 2c20 312e 302c 2030 2e32    [0.5, 1.0, 0.2
+0000e7d0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7f0: 2020 205b 302e 312c 2030 2e32 2c20 312e     [0.1, 0.2, 1.
+0000e800: 305d 5d29 0a20 2020 2020 2020 206d 203d  0]]).        m =
+0000e810: 2033 0a20 2020 2020 2020 206e 203d 2074   3.        n = t
+0000e820: 7275 655f 636f 6c63 6f76 2e73 6861 7065  rue_colcov.shape
+0000e830: 5b30 5d0a 2020 2020 2020 2020 7472 7565  [0].        true
+0000e840: 5f73 6361 6c65 203d 2033 0a20 2020 2020  _scale = 3.     
+0000e850: 2020 2074 7275 655f 726f 7763 6f76 203d     true_rowcov =
+0000e860: 206e 702e 6469 6167 285b 7472 7565 5f73   np.diag([true_s
+0000e870: 6361 6c65 2a2a 2832 2a69 2920 666f 7220  cale**(2*i) for 
+0000e880: 6920 696e 2072 616e 6765 286d 295d 290a  i in range(m)]).
+0000e890: 2020 2020 2020 2020 6d75 203d 206e 702e          mu = np.
+0000e8a0: 7a65 726f 7328 286d 2c20 6e29 290a 2020  zeros((m, n)).  
+0000e8b0: 2020 2020 2020 7472 7565 5f6b 726f 6e20        true_kron 
+0000e8c0: 3d20 6e70 2e6b 726f 6e28 7472 7565 5f72  = np.kron(true_r
+0000e8d0: 6f77 636f 762c 2074 7275 655f 636f 6c63  owcov, true_colc
+0000e8e0: 6f76 290a 2020 2020 2020 2020 6461 7461  ov).        data
+0000e8f0: 203d 206e 702e 7261 6e64 6f6d 2e6d 756c   = np.random.mul
+0000e900: 7469 7661 7269 6174 655f 6e6f 726d 616c  tivariate_normal
+0000e910: 286d 752e 666c 6174 7465 6e28 292c 2074  (mu.flatten(), t
+0000e920: 7275 655f 6b72 6f6e 290a 2020 2020 2020  rue_kron).      
+0000e930: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0000e940: 7368 6170 6528 6d2c 206e 290a 0a20 2020  shape(m, n)..   
+0000e950: 2020 2020 2077 6974 6820 706d 2e4d 6f64       with pm.Mod
+0000e960: 656c 2829 2061 7320 6d6f 6465 6c3a 0a20  el() as model:. 
+0000e970: 2020 2020 2020 2020 2020 2023 2053 6574             # Set
+0000e980: 7570 2072 6967 6874 2063 686f 6c65 736b  up right cholesk
+0000e990: 7920 6d61 7472 6978 0a20 2020 2020 2020  y matrix.       
+0000e9a0: 2020 2020 2073 645f 6469 7374 203d 2070       sd_dist = p
+0000e9b0: 6d2e 4861 6c66 4361 7563 6879 2e64 6973  m.HalfCauchy.dis
+0000e9c0: 7428 6265 7461 3d32 2e35 2c20 7368 6170  t(beta=2.5, shap
+0000e9d0: 653d 3329 0a20 2020 2020 2020 2020 2020  e=3).           
+0000e9e0: 2063 6f6c 6368 6f6c 5f70 6163 6b65 6420   colchol_packed 
+0000e9f0: 3d20 706d 2e4c 4b4a 4368 6f6c 6573 6b79  = pm.LKJCholesky
+0000ea00: 436f 7628 2763 6f6c 6368 6f6c 7061 636b  Cov('colcholpack
+0000ea10: 6564 272c 206e 3d33 2c20 6574 613d 322c  ed', n=3, eta=2,
+0000ea20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 7364 5f64 6973 743d 7364 5f64 6973 7429  sd_dist=sd_dist)
+0000ea60: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+0000ea70: 6368 6f6c 203d 2070 6d2e 6578 7061 6e64  chol = pm.expand
+0000ea80: 5f70 6163 6b65 645f 7472 6961 6e67 756c  _packed_triangul
+0000ea90: 6172 2833 2c20 636f 6c63 686f 6c5f 7061  ar(3, colchol_pa
+0000eaa0: 636b 6564 290a 0a20 2020 2020 2020 2020  cked)..         
+0000eab0: 2020 2023 2053 6574 7570 206c 6566 7420     # Setup left 
+0000eac0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000ead0: 780a 2020 2020 2020 2020 2020 2020 7363  x.            sc
+0000eae0: 616c 6520 3d20 706d 2e4c 6f67 4e6f 726d  ale = pm.LogNorm
+0000eaf0: 616c 2827 7363 616c 6527 2c20 6d75 3d6e  al('scale', mu=n
+0000eb00: 702e 6c6f 6728 7472 7565 5f73 6361 6c65  p.log(true_scale
+0000eb10: 292c 2073 6967 6d61 3d30 2e35 290a 2020  ), sigma=0.5).  
+0000eb20: 2020 2020 2020 2020 2020 726f 7763 6f76            rowcov
+0000eb30: 203d 2070 742e 6469 6167 285b 7363 616c   = pt.diag([scal
+0000eb40: 652a 2a28 322a 6929 2066 6f72 2069 2069  e**(2*i) for i i
+0000eb50: 6e20 7261 6e67 6528 6d29 5d29 0a0a 2020  n range(m)])..  
+0000eb60: 2020 2020 2020 2020 2020 7661 6c73 203d            vals =
+0000eb70: 2070 6d2e 4d61 7472 6978 4e6f 726d 616c   pm.MatrixNormal
+0000eb80: 2827 7661 6c73 272c 206d 753d 6d75 2c20  ('vals', mu=mu, 
+0000eb90: 636f 6c63 686f 6c3d 636f 6c63 686f 6c2c  colchol=colchol,
+0000eba0: 2072 6f77 636f 763d 726f 7763 6f76 2c0a   rowcov=rowcov,.
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebd0: 2020 206f 6273 6572 7665 643d 6461 7461     observed=data
+0000ebe0: 290a 2020 2020 2222 220a 2020 2020 7276  ).    """.    rv
+0000ebf0: 5f6f 7020 3d20 6d61 7472 6978 6e6f 726d  _op = matrixnorm
+0000ec00: 616c 0a0a 2020 2020 4063 6c61 7373 6d65  al..    @classme
+0000ec10: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
+0000ec20: 7428 0a20 2020 2020 2020 2063 6c73 2c0a  t(.        cls,.
+0000ec30: 2020 2020 2020 2020 6d75 2c0a 2020 2020          mu,.    
+0000ec40: 2020 2020 726f 7763 6f76 3d4e 6f6e 652c      rowcov=None,
+0000ec50: 0a20 2020 2020 2020 2072 6f77 6368 6f6c  .        rowchol
+0000ec60: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
+0000ec70: 6f6c 636f 763d 4e6f 6e65 2c0a 2020 2020  olcov=None,.    
+0000ec80: 2020 2020 636f 6c63 686f 6c3d 4e6f 6e65      colchol=None
+0000ec90: 2c0a 2020 2020 2020 2020 2a61 7267 732c  ,.        *args,
+0000eca0: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+0000ecb0: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
+0000ecc0: 2020 6368 6f6c 6573 6b79 203d 2043 686f    cholesky = Cho
+0000ecd0: 6c65 736b 7928 6c6f 7765 723d 5472 7565  lesky(lower=True
+0000ece0: 2c20 6f6e 5f65 7272 6f72 3d22 7261 6973  , on_error="rais
+0000ecf0: 6522 290a 0a20 2020 2020 2020 2023 2041  e")..        # A
+0000ed00: 6d6f 6e67 2d72 6f77 206d 6174 7269 6365  mong-row matrice
+0000ed10: 730a 2020 2020 2020 2020 6966 206c 656e  s.        if len
+0000ed20: 285b 6920 666f 7220 6920 696e 205b 726f  ([i for i in [ro
+0000ed30: 7763 6f76 2c20 726f 7763 686f 6c5d 2069  wcov, rowchol] i
+0000ed40: 6620 6920 6973 206e 6f74 204e 6f6e 655d  f i is not None]
+0000ed50: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
+0000ed60: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000ed70: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000ed80: 2020 2020 2020 2249 6e63 6f6d 7061 7469        "Incompati
+0000ed90: 626c 6520 7061 7261 6d65 7465 7269 7a61  ble parameteriza
+0000eda0: 7469 6f6e 2e20 5370 6563 6966 7920 6578  tion. Specify ex
+0000edb0: 6163 746c 7920 6f6e 6520 6f66 2072 6f77  actly one of row
+0000edc0: 636f 762c 206f 7220 726f 7763 686f 6c2e  cov, or rowchol.
+0000edd0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000ede0: 2020 2020 2020 2020 6966 2072 6f77 636f          if rowco
+0000edf0: 7620 6973 206e 6f74 204e 6f6e 653a 0a20  v is not None:. 
+0000ee00: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+0000ee10: 7763 6f76 2e6e 6469 6d20 213d 2032 3a0a  wcov.ndim != 2:.
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000ee40: 2822 726f 7763 6f76 206d 7573 7420 6265  ("rowcov must be
+0000ee50: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
+0000ee60: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+0000ee70: 726f 7763 686f 6c5f 636f 7620 3d20 6368  rowchol_cov = ch
+0000ee80: 6f6c 6573 6b79 2872 6f77 636f 7629 0a20  olesky(rowcov). 
+0000ee90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000eea0: 2020 2020 2020 2020 2069 6620 726f 7763           if rowc
+0000eeb0: 686f 6c2e 6e64 696d 2021 3d20 323a 0a20  hol.ndim != 2:. 
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000eed0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000eee0: 2272 6f77 6368 6f6c 206d 7573 7420 6265  "rowchol must be
+0000eef0: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
+0000ef00: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+0000ef10: 726f 7763 686f 6c5f 636f 7620 3d20 7074  rowchol_cov = pt
+0000ef20: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+0000ef30: 626c 6528 726f 7763 686f 6c29 0a0a 2020  ble(rowchol)..  
+0000ef40: 2020 2020 2020 2320 416d 6f6e 672d 636f        # Among-co
+0000ef50: 6c75 6d6e 206d 6174 7269 6365 730a 2020  lumn matrices.  
+0000ef60: 2020 2020 2020 6966 206c 656e 285b 6920        if len([i 
+0000ef70: 666f 7220 6920 696e 205b 636f 6c63 6f76  for i in [colcov
+0000ef80: 2c20 636f 6c63 686f 6c5d 2069 6620 6920  , colchol] if i 
+0000ef90: 6973 206e 6f74 204e 6f6e 655d 2920 213d  is not None]) !=
+0000efa0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000efb0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000efc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000efd0: 2020 2249 6e63 6f6d 7061 7469 626c 6520    "Incompatible 
+0000efe0: 7061 7261 6d65 7465 7269 7a61 7469 6f6e  parameterization
+0000eff0: 2e20 5370 6563 6966 7920 6578 6163 746c  . Specify exactl
+0000f000: 7920 6f6e 6520 6f66 2063 6f6c 636f 762c  y one of colcov,
+0000f010: 206f 7220 636f 6c63 686f 6c2e 220a 2020   or colchol.".  
+0000f020: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f030: 2020 2020 6966 2063 6f6c 636f 7620 6973      if colcov is
+0000f040: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000f050: 2020 2020 2020 2063 6f6c 636f 7620 3d20         colcov = 
+0000f060: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+0000f070: 6961 626c 6528 636f 6c63 6f76 290a 2020  iable(colcov).  
+0000f080: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
+0000f090: 636f 762e 6e64 696d 2021 3d20 323a 0a20  cov.ndim != 2:. 
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f0b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000f0c0: 2263 6f6c 636f 7620 6d75 7374 2062 6520  "colcov must be 
+0000f0d0: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
+0000f0e0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+0000f0f0: 6f6c 6368 6f6c 5f63 6f76 203d 2063 686f  olchol_cov = cho
+0000f100: 6c65 736b 7928 636f 6c63 6f76 290a 2020  lesky(colcov).  
+0000f110: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000f120: 2020 2020 2020 2020 6966 2063 6f6c 6368          if colch
+0000f130: 6f6c 2e6e 6469 6d20 213d 2032 3a0a 2020  ol.ndim != 2:.  
+0000f140: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000f150: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0000f160: 636f 6c63 686f 6c20 6d75 7374 2062 6520  colchol must be 
+0000f170: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
+0000f180: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+0000f190: 6f6c 6368 6f6c 5f63 6f76 203d 2070 742e  olchol_cov = pt.
+0000f1a0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+0000f1b0: 6c65 2863 6f6c 6368 6f6c 290a 0a20 2020  le(colchol)..   
+0000f1c0: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
+0000f1d0: 3d20 2872 6f77 6368 6f6c 5f63 6f76 2e73  = (rowchol_cov.s
+0000f1e0: 6861 7065 5b2d 315d 2c20 636f 6c63 686f  hape[-1], colcho
+0000f1f0: 6c5f 636f 762e 7368 6170 655b 2d31 5d29  l_cov.shape[-1])
+0000f200: 0a0a 2020 2020 2020 2020 2320 4272 6f61  ..        # Broa
+0000f210: 6463 6173 7469 6e67 206d 750a 2020 2020  dcasting mu.    
+0000f220: 2020 2020 6d75 203d 2070 742e 6578 7472      mu = pt.extr
+0000f230: 615f 6f70 732e 6272 6f61 6463 6173 745f  a_ops.broadcast_
+0000f240: 746f 286d 752c 2073 6861 7065 3d64 6973  to(mu, shape=dis
+0000f250: 745f 7368 6170 6529 0a20 2020 2020 2020  t_shape).       
+0000f260: 206d 7520 3d20 7074 2e61 735f 7465 6e73   mu = pt.as_tens
+0000f270: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
+0000f280: 7458 286d 7529 290a 0a20 2020 2020 2020  tX(mu))..       
+0000f290: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+0000f2a0: 6469 7374 285b 6d75 2c20 726f 7763 686f  dist([mu, rowcho
+0000f2b0: 6c5f 636f 762c 2063 6f6c 6368 6f6c 5f63  l_cov, colchol_c
+0000f2c0: 6f76 5d2c 202a 2a6b 7761 7267 7329 0a0a  ov], **kwargs)..
+0000f2d0: 2020 2020 6465 6620 6d6f 6d65 6e74 2872      def moment(r
+0000f2e0: 762c 2073 697a 652c 206d 752c 2072 6f77  v, size, mu, row
+0000f2f0: 6368 6f6c 2c20 636f 6c63 686f 6c29 3a0a  chol, colchol):.
+0000f300: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+0000f310: 742e 6675 6c6c 5f6c 696b 6528 7276 2c20  t.full_like(rv, 
+0000f320: 6d75 290a 0a20 2020 2064 6566 206c 6f67  mu)..    def log
+0000f330: 7028 7661 6c75 652c 206d 752c 2072 6f77  p(value, mu, row
+0000f340: 6368 6f6c 2c20 636f 6c63 686f 6c29 3a0a  chol, colchol):.
+0000f350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f360: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
+0000f370: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
+0000f380: 204d 6174 7269 782d 7661 6c75 6564 204e   Matrix-valued N
+0000f390: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+0000f3a0: 6f6e 0a20 2020 2020 2020 2061 7420 7370  on.        at sp
+0000f3b0: 6563 6966 6965 6420 7661 6c75 652e 0a0a  ecified value...
+0000f3c0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000f3d0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000f3e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
+0000f3f0: 6c75 653a 206e 756d 6572 6963 0a20 2020  lue: numeric.   
+0000f400: 2020 2020 2020 2020 2056 616c 7565 2066           Value f
+0000f410: 6f72 2077 6869 6368 206c 6f67 2d70 726f  or which log-pro
+0000f420: 6261 6269 6c69 7479 2069 7320 6361 6c63  bability is calc
+0000f430: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
+0000f440: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0000f450: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0000f460: 2054 656e 736f 7256 6172 6961 626c 650a   TensorVariable.
+0000f470: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000f480: 2020 2020 2069 6620 7661 6c75 652e 6e64       if value.nd
+0000f490: 696d 2021 3d20 323a 0a20 2020 2020 2020  im != 2:.       
+0000f4a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000f4b0: 4572 726f 7228 2256 616c 7565 206d 7573  Error("Value mus
+0000f4c0: 7420 6265 2074 776f 2064 696d 656e 7369  t be two dimensi
+0000f4d0: 6f6e 616c 2e22 290a 0a20 2020 2020 2020  onal.")..       
+0000f4e0: 2023 2043 6f6d 7075 7465 2054 725b 636f   # Compute Tr[co
+0000f4f0: 6c63 6f76 5e2d 3120 4020 2878 202d 206d  lcov^-1 @ (x - m
+0000f500: 7529 2e54 2040 2072 6f77 636f 765e 2d31  u).T @ rowcov^-1
+0000f510: 2040 2028 7820 2d20 6d75 295d 2061 6e64   @ (x - mu)] and
+0000f520: 0a20 2020 2020 2020 2023 2074 6865 206c  .        # the l
+0000f530: 6f67 6465 7420 6f66 2063 6f6c 636f 7620  ogdet of colcov 
+0000f540: 616e 6420 726f 7763 6f76 2e0a 2020 2020  and rowcov..    
+0000f550: 2020 2020 6465 6c74 6120 3d20 7661 6c75      delta = valu
+0000f560: 6520 2d20 6d75 0a0a 2020 2020 2020 2020  e - mu..        
+0000f570: 2320 4669 6e64 2065 7870 6f6e 656e 7420  # Find exponent 
+0000f580: 7069 6563 6520 6279 2070 6965 6365 0a20  piece by piece. 
+0000f590: 2020 2020 2020 2072 6967 6874 5f71 7561         right_qua
+0000f5a0: 6464 6973 7420 3d20 736f 6c76 655f 6c6f  ddist = solve_lo
+0000f5b0: 7765 7228 726f 7763 686f 6c2c 2064 656c  wer(rowchol, del
+0000f5c0: 7461 290a 2020 2020 2020 2020 7175 6164  ta).        quad
+0000f5d0: 6469 7374 203d 2070 742e 6e6c 696e 616c  dist = pt.nlinal
+0000f5e0: 672e 6d61 7472 6978 5f64 6f74 2872 6967  g.matrix_dot(rig
+0000f5f0: 6874 5f71 7561 6464 6973 742e 542c 2072  ht_quaddist.T, r
+0000f600: 6967 6874 5f71 7561 6464 6973 7429 0a20  ight_quaddist). 
+0000f610: 2020 2020 2020 2071 7561 6464 6973 7420         quaddist 
+0000f620: 3d20 736f 6c76 655f 6c6f 7765 7228 636f  = solve_lower(co
+0000f630: 6c63 686f 6c2c 2071 7561 6464 6973 7429  lchol, quaddist)
+0000f640: 0a20 2020 2020 2020 2071 7561 6464 6973  .        quaddis
+0000f650: 7420 3d20 736f 6c76 655f 7570 7065 7228  t = solve_upper(
+0000f660: 636f 6c63 686f 6c2e 542c 2071 7561 6464  colchol.T, quadd
+0000f670: 6973 7429 0a20 2020 2020 2020 2074 7271  ist).        trq
+0000f680: 7561 6464 6973 7420 3d20 7074 2e6e 6c69  uaddist = pt.nli
+0000f690: 6e61 6c67 2e74 7261 6365 2871 7561 6464  nalg.trace(quadd
+0000f6a0: 6973 7429 0a0a 2020 2020 2020 2020 636f  ist)..        co
+0000f6b0: 6c64 6961 6720 3d20 7074 2e64 6961 6728  ldiag = pt.diag(
+0000f6c0: 636f 6c63 686f 6c29 0a20 2020 2020 2020  colchol).       
+0000f6d0: 2072 6f77 6469 6167 203d 2070 742e 6469   rowdiag = pt.di
+0000f6e0: 6167 2872 6f77 6368 6f6c 290a 2020 2020  ag(rowchol).    
+0000f6f0: 2020 2020 6861 6c66 5f63 6f6c 6c6f 6764      half_collogd
+0000f700: 6574 203d 2070 742e 7375 6d28 7074 2e6c  et = pt.sum(pt.l
+0000f710: 6f67 2863 6f6c 6469 6167 2929 2020 2320  og(coldiag))  # 
+0000f720: 6c6f 6764 6574 284d 2920 3d20 322a 5472  logdet(M) = 2*Tr
+0000f730: 286c 6f67 284c 2929 0a20 2020 2020 2020  (log(L)).       
+0000f740: 2068 616c 665f 726f 776c 6f67 6465 7420   half_rowlogdet 
+0000f750: 3d20 7074 2e73 756d 2870 742e 6c6f 6728  = pt.sum(pt.log(
+0000f760: 726f 7764 6961 6729 2920 2023 2055 7369  rowdiag))  # Usi
+0000f770: 6e67 2043 686f 6c65 736b 793a 204d 203d  ng Cholesky: M =
+0000f780: 204c 204c 5e54 0a0a 2020 2020 2020 2020   L L^T..        
+0000f790: 6d20 3d20 726f 7763 686f 6c2e 7368 6170  m = rowchol.shap
+0000f7a0: 655b 305d 0a20 2020 2020 2020 206e 203d  e[0].        n =
+0000f7b0: 2063 6f6c 6368 6f6c 2e73 6861 7065 5b30   colchol.shape[0
+0000f7c0: 5d0a 0a20 2020 2020 2020 206e 6f72 6d20  ]..        norm 
+0000f7d0: 3d20 2d30 2e35 202a 206d 202a 206e 202a  = -0.5 * m * n *
+0000f7e0: 2070 6d2e 666c 6f61 7458 286e 702e 6c6f   pm.floatX(np.lo
+0000f7f0: 6728 3220 2a20 6e70 2e70 6929 290a 2020  g(2 * np.pi)).  
+0000f800: 2020 2020 2020 7265 7475 726e 206e 6f72        return nor
+0000f810: 6d20 2d20 302e 3520 2a20 7472 7175 6164  m - 0.5 * trquad
+0000f820: 6469 7374 202d 206d 202a 2068 616c 665f  dist - m * half_
+0000f830: 636f 6c6c 6f67 6465 7420 2d20 6e20 2a20  collogdet - n * 
+0000f840: 6861 6c66 5f72 6f77 6c6f 6764 6574 0a0a  half_rowlogdet..
+0000f850: 0a63 6c61 7373 204b 726f 6e65 636b 6572  .class Kronecker
+0000f860: 4e6f 726d 616c 5256 2852 616e 646f 6d56  NormalRV(RandomV
+0000f870: 6172 6961 626c 6529 3a0a 2020 2020 6e61  ariable):.    na
+0000f880: 6d65 203d 2022 6b72 6f6e 6563 6b65 726e  me = "kroneckern
+0000f890: 6f72 6d61 6c22 0a20 2020 206e 6469 6d5f  ormal".    ndim_
+0000f8a0: 7375 7070 203d 2031 0a20 2020 206e 6469  supp = 1.    ndi
+0000f8b0: 6d73 5f70 6172 616d 7320 3d20 5b31 2c20  ms_params = [1, 
+0000f8c0: 302c 2032 5d0a 2020 2020 6474 7970 6520  0, 2].    dtype 
+0000f8d0: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
+0000f8e0: 7072 696e 745f 6e61 6d65 203d 2028 224b  print_name = ("K
+0000f8f0: 726f 6e65 636b 6572 4e6f 726d 616c 222c  roneckerNormal",
+0000f900: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+0000f910: 7b4b 726f 6e65 636b 6572 4e6f 726d 616c  {KroneckerNormal
+0000f920: 7d22 290a 0a20 2020 2064 6566 2072 6e67  }")..    def rng
+0000f930: 5f66 6e28 7365 6c66 2c20 726e 672c 206d  _fn(self, rng, m
+0000f940: 752c 2073 6967 6d61 2c20 2a63 6f76 732c  u, sigma, *covs,
+0000f950: 2073 697a 653d 4e6f 6e65 293a 0a20 2020   size=None):.   
+0000f960: 2020 2020 2073 697a 6520 3d20 7369 7a65       size = size
+0000f970: 2069 6620 7369 7a65 2065 6c73 6520 636f   if size else co
+0000f980: 7673 5b2d 315d 0a20 2020 2020 2020 2063  vs[-1].        c
+0000f990: 6f76 7320 3d20 636f 7673 5b3a 2d31 5d20  ovs = covs[:-1] 
+0000f9a0: 6966 2063 6f76 735b 2d31 5d20 3d3d 2073  if covs[-1] == s
+0000f9b0: 697a 6520 656c 7365 2063 6f76 730a 0a20  ize else covs.. 
+0000f9c0: 2020 2020 2020 2063 6f76 203d 2072 6564         cov = red
+0000f9d0: 7563 6528 6c69 6e61 6c67 2e6b 726f 6e2c  uce(linalg.kron,
+0000f9e0: 2063 6f76 7329 0a0a 2020 2020 2020 2020   covs)..        
+0000f9f0: 6966 2073 6967 6d61 3a0a 2020 2020 2020  if sigma:.      
+0000fa00: 2020 2020 2020 636f 7620 3d20 636f 7620        cov = cov 
+0000fa10: 2b20 7369 676d 612a 2a32 202a 206e 702e  + sigma**2 * np.
+0000fa20: 6579 6528 636f 762e 7368 6170 655b 305d  eye(cov.shape[0]
+0000fa30: 290a 0a20 2020 2020 2020 2078 203d 206d  )..        x = m
+0000fa40: 756c 7469 7661 7269 6174 655f 6e6f 726d  ultivariate_norm
+0000fa50: 616c 2e72 6e67 5f66 6e28 726e 673d 726e  al.rng_fn(rng=rn
+0000fa60: 672c 206d 6561 6e3d 6d75 2c20 636f 763d  g, mean=mu, cov=
+0000fa70: 636f 762c 2073 697a 653d 7369 7a65 290a  cov, size=size).
+0000fa80: 2020 2020 2020 2020 7265 7475 726e 2078          return x
+0000fa90: 0a0a 0a6b 726f 6e65 636b 6572 6e6f 726d  ...kroneckernorm
+0000faa0: 616c 203d 204b 726f 6e65 636b 6572 4e6f  al = KroneckerNo
+0000fab0: 726d 616c 5256 2829 0a0a 0a63 6c61 7373  rmalRV()...class
+0000fac0: 204b 726f 6e65 636b 6572 4e6f 726d 616c   KroneckerNormal
+0000fad0: 2843 6f6e 7469 6e75 6f75 7329 3a0a 2020  (Continuous):.  
+0000fae0: 2020 7222 2222 0a20 2020 204d 756c 7469    r""".    Multi
+0000faf0: 7661 7269 6174 6520 6e6f 726d 616c 206c  variate normal l
+0000fb00: 6f67 2d6c 696b 656c 6968 6f6f 6420 7769  og-likelihood wi
+0000fb10: 7468 204b 726f 6e65 636b 6572 2d73 7472  th Kronecker-str
+0000fb20: 7563 7475 7265 6420 636f 7661 7269 616e  uctured covarian
+0000fb30: 6365 2e0a 0a20 2020 202e 2e20 6d61 7468  ce...    .. math
+0000fb40: 3a3a 0a0a 2020 2020 2020 2066 2878 205c  ::..       f(x \
+0000fb50: 6d69 6420 5c6d 752c 204b 2920 3d0a 2020  mid \mu, K) =.  
+0000fb60: 2020 2020 2020 2020 205c 6672 6163 7b31           \frac{1
+0000fb70: 7d7b 2832 5c70 6920 7c4b 7c29 5e7b 312f  }{(2\pi |K|)^{1/
+0000fb80: 327d 7d0a 2020 2020 2020 2020 2020 205c  2}}.           \
+0000fb90: 6578 705c 6c65 6674 5c7b 202d 5c66 7261  exp\left\{ -\fra
+0000fba0: 637b 317d 7b32 7d20 2878 2d5c 6d75 295e  c{1}{2} (x-\mu)^
+0000fbb0: 7b5c 7072 696d 657d 204b 5e7b 2d31 7d20  {\prime} K^{-1} 
+0000fbc0: 2878 2d5c 6d75 2920 5c72 6967 6874 5c7d  (x-\mu) \right\}
+0000fbd0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
+0000fbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fbf0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
+0000fc00: 7570 706f 7274 2020 203a 6d61 7468 3a60  upport   :math:`
+0000fc10: 7820 5c69 6e20 5c6d 6174 6862 627b 527d  x \in \mathbb{R}
+0000fc20: 5e4e 600a 2020 2020 4d65 616e 2020 2020  ^N`.    Mean    
+0000fc30: 2020 3a6d 6174 683a 605c 6d75 600a 2020    :math:`\mu`.  
+0000fc40: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
+0000fc50: 683a 604b 203d 205c 6269 676f 7469 6d65  h:`K = \bigotime
+0000fc60: 7320 4b5f 6920 2b20 5c73 6967 6d61 5e32  s K_i + \sigma^2
+0000fc70: 2049 5f4e 600a 2020 2020 3d3d 3d3d 3d3d   I_N`.    ======
+0000fc80: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+0000fc90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+0000fca0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000fcb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000fcc0: 2020 6d75 203a 2074 656e 736f 725f 6c69    mu : tensor_li
+0000fcd0: 6b65 206f 6620 666c 6f61 740a 2020 2020  ke of float.    
+0000fce0: 2020 2020 5665 6374 6f72 206f 6620 6d65      Vector of me
+0000fcf0: 616e 732c 206a 7573 7420 6173 2069 6e20  ans, just as in 
+0000fd00: 604d 764e 6f72 6d61 6c60 2e0a 2020 2020  `MvNormal`..    
+0000fd10: 636f 7673 203a 206c 6973 7420 6f66 2061  covs : list of a
+0000fd20: 7272 6179 730a 2020 2020 2020 2020 5468  rrays.        Th
+0000fd30: 6520 7365 7420 6f66 2063 6f76 6172 6961  e set of covaria
+0000fd40: 6e63 6520 6d61 7472 6963 6573 203a 6d61  nce matrices :ma
+0000fd50: 7468 3a60 5b4b 5f31 2c20 4b5f 322c 202e  th:`[K_1, K_2, .
+0000fd60: 2e2e 5d60 2074 6f20 6265 0a20 2020 2020  ..]` to be.     
+0000fd70: 2020 204b 726f 6e65 636b 6572 6564 2069     Kroneckered i
+0000fd80: 6e20 7468 6520 6f72 6465 7220 7072 6f76  n the order prov
+0000fd90: 6964 6564 203a 6d61 7468 3a60 5c62 6967  ided :math:`\big
+0000fda0: 6f74 696d 6573 204b 5f69 602e 0a20 2020  otimes K_i`..   
+0000fdb0: 2063 686f 6c73 203a 206c 6973 7420 6f66   chols : list of
+0000fdc0: 2061 7272 6179 730a 2020 2020 2020 2020   arrays.        
+0000fdd0: 5468 6520 7365 7420 6f66 206c 6f77 6572  The set of lower
+0000fde0: 2063 686f 6c65 736b 7920 6d61 7472 6963   cholesky matric
+0000fdf0: 6573 203a 6d61 7468 3a60 5b4c 5f31 2c20  es :math:`[L_1, 
+0000fe00: 4c5f 322c 202e 2e2e 5d60 2073 7563 6820  L_2, ...]` such 
+0000fe10: 7468 6174 0a20 2020 2020 2020 203a 6d61  that.        :ma
+0000fe20: 7468 3a60 4b5f 6920 3d20 4c5f 6920 4c5f  th:`K_i = L_i L_
+0000fe30: 6927 602e 0a20 2020 2065 7664 7320 3a20  i'`..    evds : 
+0000fe40: 6c69 7374 206f 6620 7475 706c 6573 0a20  list of tuples. 
+0000fe50: 2020 2020 2020 2054 6865 2073 6574 206f         The set o
+0000fe60: 6620 6569 6765 6e76 616c 7565 2d76 6563  f eigenvalue-vec
+0000fe70: 746f 722c 2065 6967 656e 7665 6374 6f72  tor, eigenvector
+0000fe80: 2d6d 6174 7269 7820 7061 6972 730a 2020  -matrix pairs.  
+0000fe90: 2020 2020 2020 3a6d 6174 683a 605b 2876        :math:`[(v
+0000fea0: 5f31 2c20 515f 3129 2c20 2876 5f32 2c20  _1, Q_1), (v_2, 
+0000feb0: 515f 3229 2c20 2e2e 2e5d 6020 7375 6368  Q_2), ...]` such
+0000fec0: 2074 6861 740a 2020 2020 2020 2020 3a6d   that.        :m
+0000fed0: 6174 683a 604b 5f69 203d 2051 5f69 205c  ath:`K_i = Q_i \
+0000fee0: 7465 7874 7b64 6961 677d 2876 5f69 2920  text{diag}(v_i) 
+0000fef0: 515f 6927 602e 2046 6f72 2065 7861 6d70  Q_i'`. For examp
+0000ff00: 6c65 3a3a 0a0a 2020 2020 2020 2020 2020  le::..          
+0000ff10: 2020 765f 692c 2051 5f69 203d 2070 742e    v_i, Q_i = pt.
+0000ff20: 6e6c 696e 616c 672e 6569 6768 284b 5f69  nlinalg.eigh(K_i
+0000ff30: 290a 2020 2020 7369 676d 6120 3a20 7363  ).    sigma : sc
+0000ff40: 616c 6172 2c20 6f70 7469 6f6e 616c 0a20  alar, optional. 
+0000ff50: 2020 2020 2020 2053 7461 6e64 6172 6420         Standard 
+0000ff60: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
+0000ff70: 2047 6175 7373 6961 6e20 7768 6974 6520   Gaussian white 
+0000ff80: 6e6f 6973 652e 0a0a 2020 2020 4578 616d  noise...    Exam
+0000ff90: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0000ffa0: 2d0a 2020 2020 4465 6669 6e65 2061 206d  -.    Define a m
+0000ffb0: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
+0000ffc0: 616c 2076 6172 6961 626c 6520 7769 7468  al variable with
+0000ffd0: 2061 2063 6f76 6172 6961 6e63 650a 2020   a covariance.  
+0000ffe0: 2020 3a6d 6174 683a 604b 203d 204b 5f31    :math:`K = K_1
+0000fff0: 205c 6f74 696d 6573 204b 5f32 600a 0a20   \otimes K_2`.. 
+00010000: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
+00010010: 686f 6e0a 0a20 2020 2020 2020 204b 3120  hon..        K1 
+00010020: 3d20 6e70 2e61 7272 6179 285b 5b31 2e2c  = np.array([[1.,
+00010030: 2030 2e35 5d2c 205b 302e 352c 2032 5d5d   0.5], [0.5, 2]]
+00010040: 290a 2020 2020 2020 2020 4b32 203d 206e  ).        K2 = n
+00010050: 702e 6172 7261 7928 5b5b 312e 2c20 302e  p.array([[1., 0.
+00010060: 342c 2030 2e32 5d2c 205b 302e 342c 2032  4, 0.2], [0.4, 2
+00010070: 2c20 302e 335d 2c20 5b30 2e32 2c20 302e  , 0.3], [0.2, 0.
+00010080: 332c 2031 5d5d 290a 2020 2020 2020 2020  3, 1]]).        
+00010090: 636f 7673 203d 205b 4b31 2c20 4b32 5d0a  covs = [K1, K2].
+000100a0: 2020 2020 2020 2020 4e20 3d20 360a 2020          N = 6.  
+000100b0: 2020 2020 2020 6d75 203d 206e 702e 7a65        mu = np.ze
+000100c0: 726f 7328 4e29 0a20 2020 2020 2020 2077  ros(N).        w
+000100d0: 6974 6820 706d 2e4d 6f64 656c 2829 2061  ith pm.Model() a
+000100e0: 7320 6d6f 6465 6c3a 0a20 2020 2020 2020  s model:.       
+000100f0: 2020 2020 2076 616c 7320 3d20 706d 2e4b       vals = pm.K
+00010100: 726f 6e65 636b 6572 4e6f 726d 616c 2827  roneckerNormal('
+00010110: 7661 6c73 272c 206d 753d 6d75 2c20 636f  vals', mu=mu, co
+00010120: 7673 3d63 6f76 732c 2073 6861 7065 3d4e  vs=covs, shape=N
+00010130: 290a 0a20 2020 2045 6666 6963 6965 6e63  )..    Efficienc
+00010140: 7920 6761 696e 7320 6172 6520 6d61 6465  y gains are made
+00010150: 2062 7920 6368 6f6c 6573 6b79 2064 6563   by cholesky dec
+00010160: 6f6d 706f 7369 6e67 203a 6d61 7468 3a60  omposing :math:`
+00010170: 4b5f 3160 2061 6e64 0a20 2020 203a 6d61  K_1` and.    :ma
+00010180: 7468 3a60 4b5f 3260 2069 6e64 6976 6964  th:`K_2` individ
+00010190: 7561 6c6c 7920 7261 7468 6572 2074 6861  ually rather tha
+000101a0: 6e20 7468 6520 6c61 7267 6572 203a 6d61  n the larger :ma
+000101b0: 7468 3a60 4b60 206d 6174 7269 782e 2041  th:`K` matrix. A
+000101c0: 6c74 686f 7567 680a 2020 2020 6f6e 6c79  lthough.    only
+000101d0: 2074 776f 206d 6174 7269 6365 7320 3a6d   two matrices :m
+000101e0: 6174 683a 604b 5f31 6020 616e 6420 3a6d  ath:`K_1` and :m
+000101f0: 6174 683a 604b 5f32 6020 6172 6520 7368  ath:`K_2` are sh
+00010200: 6f77 6e20 6865 7265 2c20 616e 2061 7262  own here, an arb
+00010210: 6974 7261 7279 0a20 2020 206e 756d 6265  itrary.    numbe
+00010220: 7220 6f66 2073 7562 6d61 7472 6963 6573  r of submatrices
+00010230: 2063 616e 2062 6520 636f 6d62 696e 6564   can be combined
+00010240: 2069 6e20 7468 6973 2077 6179 2e20 4368   in this way. Ch
+00010250: 6f6c 6573 6b79 7320 616e 640a 2020 2020  oleskys and.    
+00010260: 6569 6765 6e64 6563 6f6d 706f 7369 7469  eigendecompositi
+00010270: 6f6e 7320 6361 6e20 6265 2070 726f 7669  ons can be provi
+00010280: 6465 6420 696e 7374 6561 640a 0a20 2020  ded instead..   
+00010290: 202e 2e20 636f 6465 3a3a 2070 7974 686f   .. code:: pytho
+000102a0: 6e0a 0a20 2020 2020 2020 2063 686f 6c73  n..        chols
+000102b0: 203d 205b 6e70 2e6c 696e 616c 672e 6368   = [np.linalg.ch
+000102c0: 6f6c 6573 6b79 284b 6929 2066 6f72 204b  olesky(Ki) for K
+000102d0: 6920 696e 2063 6f76 735d 0a20 2020 2020  i in covs].     
+000102e0: 2020 2065 7664 7320 3d20 5b6e 702e 6c69     evds = [np.li
+000102f0: 6e61 6c67 2e65 6967 6828 4b69 2920 666f  nalg.eigh(Ki) fo
+00010300: 7220 4b69 2069 6e20 636f 7673 5d0a 2020  r Ki in covs].  
+00010310: 2020 2020 2020 7769 7468 2070 6d2e 4d6f        with pm.Mo
+00010320: 6465 6c28 2920 6173 206d 6f64 656c 3a0a  del() as model:.
+00010330: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
+00010340: 3220 3d20 706d 2e4b 726f 6e65 636b 6572  2 = pm.Kronecker
+00010350: 4e6f 726d 616c 2827 7661 6c73 3227 2c20  Normal('vals2', 
+00010360: 6d75 3d6d 752c 2063 686f 6c73 3d63 686f  mu=mu, chols=cho
+00010370: 6c73 2c20 7368 6170 653d 4e29 0a20 2020  ls, shape=N).   
+00010380: 2020 2020 2020 2020 2023 206f 720a 2020           # or.  
+00010390: 2020 2020 2020 2020 2020 7661 6c73 3320            vals3 
+000103a0: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
+000103b0: 726d 616c 2827 7661 6c73 3327 2c20 6d75  rmal('vals3', mu
+000103c0: 3d6d 752c 2065 7664 733d 6576 6473 2c20  =mu, evds=evds, 
+000103d0: 7368 6170 653d 4e29 0a0a 2020 2020 6e65  shape=N)..    ne
+000103e0: 6974 6865 7220 6f66 2077 6869 6368 2077  ither of which w
+000103f0: 696c 6c20 6265 2063 6f6e 7665 7274 6564  ill be converted
+00010400: 2e20 4469 6167 6f6e 616c 206e 6f69 7365  . Diagonal noise
+00010410: 2063 616e 2061 6c73 6f20 6265 2061 6464   can also be add
+00010420: 6564 2074 6f0a 2020 2020 7468 6520 636f  ed to.    the co
+00010430: 7661 7269 616e 6365 206d 6174 7269 782c  variance matrix,
+00010440: 203a 6d61 7468 3a60 4b20 3d20 4b5f 3120   :math:`K = K_1 
+00010450: 5c6f 7469 6d65 7320 4b5f 3220 2b20 5c73  \otimes K_2 + \s
+00010460: 6967 6d61 5e32 2049 5f4e 602e 0a20 2020  igma^2 I_N`..   
+00010470: 2044 6573 7069 7465 2074 6865 206e 6f69   Despite the noi
+00010480: 7365 2072 656d 6f76 696e 6720 7468 6520  se removing the 
+00010490: 6f76 6572 616c 6c20 4b72 6f6e 6563 6b65  overall Kronecke
+000104a0: 7220 7374 7275 6374 7572 6520 6f66 2074  r structure of t
+000104b0: 6865 206d 6174 7269 782c 0a20 2020 2060  he matrix,.    `
+000104c0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c60  KroneckerNormal`
+000104d0: 2063 616e 2063 6f6e 7469 6e75 6520 746f   can continue to
+000104e0: 206d 616b 6520 6566 6669 6369 656e 7420   make efficient 
+000104f0: 6361 6c63 756c 6174 696f 6e73 2062 790a  calculations by.
+00010500: 2020 2020 7574 696c 697a 696e 6720 6569      utilizing ei
+00010510: 6765 6e64 6563 6f6d 706f 7369 746f 6e73  gendecompositons
+00010520: 206f 6620 7468 6520 7375 626d 6174 7269   of the submatri
+00010530: 6365 7320 6265 6869 6e64 2074 6865 2073  ces behind the s
+00010540: 6365 6e65 7320 5b31 5d2e 0a20 2020 2054  cenes [1]..    T
+00010550: 6875 732c 0a0a 2020 2020 2e2e 2063 6f64  hus,..    .. cod
+00010560: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00010570: 2020 2020 7369 676d 6120 3d20 302e 310a      sigma = 0.1.
+00010580: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
+00010590: 4d6f 6465 6c28 2920 6173 206e 6f69 7365  Model() as noise
+000105a0: 5f6d 6f64 656c 3a0a 2020 2020 2020 2020  _model:.        
+000105b0: 2020 2020 7661 6c73 203d 2070 6d2e 4b72      vals = pm.Kr
+000105c0: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
+000105d0: 616c 7327 2c20 6d75 3d6d 752c 2063 6f76  als', mu=mu, cov
+000105e0: 733d 636f 7673 2c20 7369 676d 613d 7369  s=covs, sigma=si
+000105f0: 676d 612c 2073 6861 7065 3d4e 290a 2020  gma, shape=N).  
+00010600: 2020 2020 2020 2020 2020 7661 6c73 3220            vals2 
+00010610: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
+00010620: 726d 616c 2827 7661 6c73 3227 2c20 6d75  rmal('vals2', mu
+00010630: 3d6d 752c 2063 686f 6c73 3d63 686f 6c73  =mu, chols=chols
+00010640: 2c20 7369 676d 613d 7369 676d 612c 2073  , sigma=sigma, s
+00010650: 6861 7065 3d4e 290a 2020 2020 2020 2020  hape=N).        
+00010660: 2020 2020 7661 6c73 3320 3d20 706d 2e4b      vals3 = pm.K
+00010670: 726f 6e65 636b 6572 4e6f 726d 616c 2827  roneckerNormal('
+00010680: 7661 6c73 3327 2c20 6d75 3d6d 752c 2065  vals3', mu=mu, e
+00010690: 7664 733d 6576 6473 2c20 7369 676d 613d  vds=evds, sigma=
+000106a0: 7369 676d 612c 2073 6861 7065 3d4e 290a  sigma, shape=N).
+000106b0: 0a20 2020 2061 7265 2069 6465 6e74 6963  .    are identic
+000106c0: 616c 2c20 7769 7468 2060 636f 7673 6020  al, with `covs` 
+000106d0: 616e 6420 6063 686f 6c73 6020 6561 6368  and `chols` each
+000106e0: 2063 6f6e 7665 7274 6564 2074 6f0a 2020   converted to.  
+000106f0: 2020 6569 6765 6e64 6563 6f6d 706f 7369    eigendecomposi
+00010700: 7469 6f6e 732e 0a0a 2020 2020 5265 6665  tions...    Refe
+00010710: 7265 6e63 6573 0a20 2020 202d 2d2d 2d2d  rences.    -----
+00010720: 2d2d 2d2d 2d0a 2020 2020 2e2e 205b 315d  -----.    .. [1]
+00010730: 2053 6161 7463 6869 2c20 592e 2028 3230   Saatchi, Y. (20
+00010740: 3131 292e 2022 5363 616c 6162 6c65 2069  11). "Scalable i
+00010750: 6e66 6572 656e 6365 2066 6f72 2073 7472  nference for str
+00010760: 7563 7475 7265 6420 4761 7573 7369 616e  uctured Gaussian
+00010770: 2070 726f 6365 7373 206d 6f64 656c 7322   process models"
+00010780: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
+00010790: 6f70 203d 206b 726f 6e65 636b 6572 6e6f  op = kroneckerno
+000107a0: 726d 616c 0a0a 2020 2020 4063 6c61 7373  rmal..    @class
+000107b0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+000107c0: 6973 7428 636c 732c 206d 752c 2063 6f76  ist(cls, mu, cov
+000107d0: 733d 4e6f 6e65 2c20 6368 6f6c 733d 4e6f  s=None, chols=No
+000107e0: 6e65 2c20 6576 6473 3d4e 6f6e 652c 2073  ne, evds=None, s
+000107f0: 6967 6d61 3d4e 6f6e 652c 202a 6172 6773  igma=None, *args
+00010800: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00010810: 2020 2020 2069 6620 6c65 6e28 5b69 2066       if len([i f
+00010820: 6f72 2069 2069 6e20 5b63 6f76 732c 2063  or i in [covs, c
+00010830: 686f 6c73 2c20 6576 6473 5d20 6966 2069  hols, evds] if i
+00010840: 2069 7320 6e6f 7420 4e6f 6e65 5d29 2021   is not None]) !
+00010850: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00010860: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00010870: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00010880: 2020 2022 496e 636f 6d70 6174 6962 6c65     "Incompatible
+00010890: 2070 6172 616d 6574 6572 697a 6174 696f   parameterizatio
+000108a0: 6e2e 2053 7065 6369 6679 2065 7861 6374  n. Specify exact
+000108b0: 6c79 206f 6e65 206f 6620 636f 7673 2c20  ly one of covs, 
+000108c0: 6368 6f6c 732c 206f 7220 6576 6473 2e22  chols, or evds."
+000108d0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+000108e0: 2020 2020 2020 2020 7369 676d 6120 3d20          sigma = 
+000108f0: 7369 676d 6120 6966 2073 6967 6d61 2065  sigma if sigma e
+00010900: 6c73 6520 300a 0a20 2020 2020 2020 2069  lse 0..        i
+00010910: 6620 6368 6f6c 7320 6973 206e 6f74 204e  f chols is not N
+00010920: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010930: 2063 6f76 7320 3d20 5b63 686f 6c2e 646f   covs = [chol.do
+00010940: 7428 6368 6f6c 2e54 2920 666f 7220 6368  t(chol.T) for ch
+00010950: 6f6c 2069 6e20 6368 6f6c 735d 0a20 2020  ol in chols].   
+00010960: 2020 2020 2065 6c69 6620 6576 6473 2069       elif evds i
+00010970: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00010980: 2020 2020 2020 2020 6569 6768 5f69 7465          eigh_ite
+00010990: 7261 626c 6520 3d20 6576 6473 0a20 2020  rable = evds.   
+000109a0: 2020 2020 2020 2020 2063 6f76 7320 3d20           covs = 
+000109b0: 5b5d 0a20 2020 2020 2020 2020 2020 2065  [].            e
+000109c0: 6967 735f 7365 702c 2051 7320 3d20 7a69  igs_sep, Qs = zi
+000109d0: 7028 2a65 6967 685f 6974 6572 6162 6c65  p(*eigh_iterable
+000109e0: 2920 2023 2055 6e7a 6970 0a20 2020 2020  )  # Unzip.     
+000109f0: 2020 2020 2020 2066 6f72 2065 6967 2c20         for eig, 
+00010a00: 5120 696e 207a 6970 2865 6967 735f 7365  Q in zip(eigs_se
+00010a10: 702c 2051 7329 3a0a 2020 2020 2020 2020  p, Qs):.        
+00010a20: 2020 2020 2020 2020 636f 765f 6920 3d20          cov_i = 
+00010a30: 7074 2e64 6f74 2851 2c20 7074 2e64 6f74  pt.dot(Q, pt.dot
+00010a40: 2870 742e 6469 6167 2865 6967 292c 2051  (pt.diag(eig), Q
+00010a50: 2e54 2929 0a20 2020 2020 2020 2020 2020  .T)).           
+00010a60: 2020 2020 2063 6f76 732e 6170 7065 6e64       covs.append
+00010a70: 2863 6f76 5f69 290a 0a20 2020 2020 2020  (cov_i)..       
+00010a80: 206d 7520 3d20 7074 2e61 735f 7465 6e73   mu = pt.as_tens
+00010a90: 6f72 5f76 6172 6961 626c 6528 6d75 290a  or_variable(mu).
+00010aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010ab0: 7375 7065 7228 292e 6469 7374 285b 6d75  super().dist([mu
+00010ac0: 2c20 7369 676d 612c 202a 636f 7673 5d2c  , sigma, *covs],
+00010ad0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00010ae0: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
+00010af0: 697a 652c 206d 752c 2063 6f76 732c 2063  ize, mu, covs, c
+00010b00: 686f 6c73 2c20 6576 6473 293a 0a20 2020  hols, evds):.   
+00010b10: 2020 2020 206d 6561 6e20 3d20 6d75 0a20       mean = mu. 
+00010b20: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
+00010b30: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
+00010b40: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
+00010b50: 206d 6f6d 656e 745f 7369 7a65 203d 2070   moment_size = p
+00010b60: 742e 636f 6e63 6174 656e 6174 6528 5b73  t.concatenate([s
+00010b70: 697a 652c 206d 752e 7368 6170 655d 290a  ize, mu.shape]).
+00010b80: 2020 2020 2020 2020 2020 2020 6d65 616e              mean
+00010b90: 203d 2070 742e 6675 6c6c 286d 6f6d 656e   = pt.full(momen
+00010ba0: 745f 7369 7a65 2c20 6d75 290a 2020 2020  t_size, mu).    
+00010bb0: 2020 2020 7265 7475 726e 206d 6561 6e0a      return mean.
+00010bc0: 0a20 2020 2064 6566 206c 6f67 7028 7661  .    def logp(va
+00010bd0: 6c75 652c 206d 752c 2073 6967 6d61 2c20  lue, mu, sigma, 
+00010be0: 2a63 6f76 7329 3a0a 2020 2020 2020 2020  *covs):.        
+00010bf0: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
+00010c00: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
+00010c10: 696c 6974 7920 6f66 204d 756c 7469 7661  ility of Multiva
+00010c20: 7269 6174 6520 4e6f 726d 616c 2064 6973  riate Normal dis
+00010c30: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
+00010c40: 2020 7769 7468 204b 726f 6e65 636b 6572    with Kronecker
+00010c50: 2d73 7472 7563 7475 7265 6420 636f 7661  -structured cova
+00010c60: 7269 616e 6365 2061 7420 7370 6563 6966  riance at specif
+00010c70: 6965 6420 7661 6c75 652e 0a0a 2020 2020  ied value...    
+00010c80: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00010c90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00010ca0: 2d0a 2020 2020 2020 2020 7661 6c75 653a  -.        value:
+00010cb0: 206e 756d 6572 6963 0a20 2020 2020 2020   numeric.       
+00010cc0: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
+00010cd0: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
+00010ce0: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
+00010cf0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+00010d00: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00010d10: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
+00010d20: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
+00010d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010d40: 2320 436f 6d70 7574 6573 2074 6865 2071  # Computes the q
+00010d50: 7561 6472 6174 6963 2028 782d 6d75 295e  uadratic (x-mu)^
+00010d60: 5420 4020 4b5e 2d31 2040 2028 782d 6d75  T @ K^-1 @ (x-mu
+00010d70: 2920 616e 6420 6c6f 6728 6465 7428 4b29  ) and log(det(K)
+00010d80: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
+00010d90: 7565 2e6e 6469 6d20 3e20 3220 6f72 2076  ue.ndim > 2 or v
+00010da0: 616c 7565 2e6e 6469 6d20 3d3d 2030 3a0a  alue.ndim == 0:.
+00010db0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00010dc0: 6520 5661 6c75 6545 7272 6f72 2866 2249  e ValueError(f"I
+00010dd0: 6e76 616c 6964 2064 696d 656e 7369 6f6e  nvalid dimension
+00010de0: 2066 6f72 2076 616c 7565 3a20 7b76 616c   for value: {val
+00010df0: 7565 2e6e 6469 6d7d 2229 0a20 2020 2020  ue.ndim}").     
+00010e00: 2020 2069 6620 7661 6c75 652e 6e64 696d     if value.ndim
+00010e10: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00010e20: 2020 206f 6e65 6469 6d20 3d20 5472 7565     onedim = True
+00010e30: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00010e40: 7565 203d 2076 616c 7565 5b4e 6f6e 652c  ue = value[None,
+00010e50: 203a 5d0a 2020 2020 2020 2020 656c 7365   :].        else
+00010e60: 3a0a 2020 2020 2020 2020 2020 2020 6f6e  :.            on
+00010e70: 6564 696d 203d 2046 616c 7365 0a0a 2020  edim = False..  
+00010e80: 2020 2020 2020 6465 6c74 6120 3d20 7661        delta = va
+00010e90: 6c75 6520 2d20 6d75 0a0a 2020 2020 2020  lue - mu..      
+00010ea0: 2020 6569 6768 5f69 7465 7261 626c 6520    eigh_iterable 
+00010eb0: 3d20 6d61 7028 6569 6768 2c20 636f 7673  = map(eigh, covs
+00010ec0: 290a 2020 2020 2020 2020 6569 6773 5f73  ).        eigs_s
+00010ed0: 6570 2c20 5173 203d 207a 6970 282a 6569  ep, Qs = zip(*ei
+00010ee0: 6768 5f69 7465 7261 626c 6529 2020 2320  gh_iterable)  # 
+00010ef0: 556e 7a69 700a 2020 2020 2020 2020 5173  Unzip.        Qs
+00010f00: 203d 206c 6973 7428 6d61 7028 7074 2e61   = list(map(pt.a
+00010f10: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
+00010f20: 652c 2051 7329 290a 2020 2020 2020 2020  e, Qs)).        
+00010f30: 5154 7320 3d20 6c69 7374 286d 6170 2870  QTs = list(map(p
+00010f40: 742e 7472 616e 7370 6f73 652c 2051 7329  t.transpose, Qs)
+00010f50: 290a 0a20 2020 2020 2020 2065 6967 735f  )..        eigs_
+00010f60: 7365 7020 3d20 6c69 7374 286d 6170 2870  sep = list(map(p
+00010f70: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00010f80: 6162 6c65 2c20 6569 6773 5f73 6570 2929  able, eigs_sep))
+00010f90: 0a20 2020 2020 2020 2065 6967 7320 3d20  .        eigs = 
+00010fa0: 6b72 6f6e 5f64 6961 6728 2a65 6967 735f  kron_diag(*eigs_
+00010fb0: 7365 7029 2020 2320 436f 6d62 696e 6520  sep)  # Combine 
+00010fc0: 7365 7061 7261 7465 2065 6967 730a 2020  separate eigs.  
+00010fd0: 2020 2020 2020 6569 6773 202b 3d20 7369        eigs += si
+00010fe0: 676d 612a 2a32 0a20 2020 2020 2020 204e  gma**2.        N
+00010ff0: 203d 2065 6967 732e 7368 6170 655b 305d   = eigs.shape[0]
+00011000: 0a0a 2020 2020 2020 2020 7371 7274 5f71  ..        sqrt_q
+00011010: 7561 6420 3d20 6b72 6f6e 5f64 6f74 2851  uad = kron_dot(Q
+00011020: 5473 2c20 6465 6c74 612e 5429 0a20 2020  Ts, delta.T).   
+00011030: 2020 2020 2073 7172 745f 7175 6164 203d       sqrt_quad =
+00011040: 2073 7172 745f 7175 6164 202f 2070 742e   sqrt_quad / pt.
+00011050: 7371 7274 2865 6967 735b 3a2c 204e 6f6e  sqrt(eigs[:, Non
+00011060: 655d 290a 2020 2020 2020 2020 6c6f 6764  e]).        logd
+00011070: 6574 203d 2070 742e 7375 6d28 7074 2e6c  et = pt.sum(pt.l
+00011080: 6f67 2865 6967 7329 290a 0a20 2020 2020  og(eigs))..     
+00011090: 2020 2023 2053 7175 6172 6520 6561 6368     # Square each
+000110a0: 2073 616d 706c 650a 2020 2020 2020 2020   sample.        
+000110b0: 7175 6164 203d 2070 742e 6261 7463 6865  quad = pt.batche
+000110c0: 645f 646f 7428 7371 7274 5f71 7561 642e  d_dot(sqrt_quad.
+000110d0: 542c 2073 7172 745f 7175 6164 2e54 290a  T, sqrt_quad.T).
+000110e0: 2020 2020 2020 2020 6966 206f 6e65 6469          if onedi
+000110f0: 6d3a 0a20 2020 2020 2020 2020 2020 2071  m:.            q
+00011100: 7561 6420 3d20 7175 6164 5b30 5d0a 0a20  uad = quad[0].. 
+00011110: 2020 2020 2020 2061 203d 202d 2871 7561         a = -(qua
+00011120: 6420 2b20 6c6f 6764 6574 202b 204e 202a  d + logdet + N *
+00011130: 2070 742e 6c6f 6728 3220 2a20 6e70 2e70   pt.log(2 * np.p
+00011140: 6929 2920 2f20 322e 300a 2020 2020 2020  i)) / 2.0.      
+00011150: 2020 7265 7475 726e 2061 0a0a 0a63 6c61    return a...cla
+00011160: 7373 2043 4152 5256 2852 616e 646f 6d56  ss CARRV(RandomV
+00011170: 6172 6961 626c 6529 3a0a 2020 2020 6e61  ariable):.    na
+00011180: 6d65 203d 2022 6361 7222 0a20 2020 206e  me = "car".    n
+00011190: 6469 6d5f 7375 7070 203d 2031 0a20 2020  dim_supp = 1.   
+000111a0: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
+000111b0: 5b31 2c20 322c 2030 2c20 305d 0a20 2020  [1, 2, 0, 0].   
+000111c0: 2064 7479 7065 203d 2022 666c 6f61 7458   dtype = "floatX
+000111d0: 220a 2020 2020 5f70 7269 6e74 5f6e 616d  ".    _print_nam
+000111e0: 6520 3d20 2822 4341 5222 2c20 225c 5c6f  e = ("CAR", "\\o
+000111f0: 7065 7261 746f 726e 616d 657b 4341 527d  peratorname{CAR}
+00011200: 2229 0a0a 2020 2020 6465 6620 6d61 6b65  ")..    def make
+00011210: 5f6e 6f64 6528 7365 6c66 2c20 726e 672c  _node(self, rng,
+00011220: 2073 697a 652c 2064 7479 7065 2c20 6d75   size, dtype, mu
+00011230: 2c20 572c 2061 6c70 6861 2c20 7461 7529  , W, alpha, tau)
+00011240: 3a0a 2020 2020 2020 2020 6d75 203d 2070  :.        mu = p
+00011250: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00011260: 6162 6c65 2866 6c6f 6174 5828 6d75 2929  able(floatX(mu))
+00011270: 0a0a 2020 2020 2020 2020 5720 3d20 7079  ..        W = py
+00011280: 7465 6e73 6f72 2e73 7061 7273 652e 6173  tensor.sparse.as
+00011290: 5f73 7061 7273 655f 6f72 5f74 656e 736f  _sparse_or_tenso
+000112a0: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
+000112b0: 5828 5729 290a 2020 2020 2020 2020 6966  X(W)).        if
+000112c0: 206e 6f74 2057 2e6e 6469 6d20 3d3d 2032   not W.ndim == 2
+000112d0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000112e0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+000112f0: 5720 6d75 7374 2062 6520 6120 6d61 7472  W must be a matr
+00011300: 6978 2028 6e64 696d 3d32 292e 2229 0a0a  ix (ndim=2).")..
+00011310: 2020 2020 2020 2020 7370 6172 7365 203d          sparse =
+00011320: 2069 7369 6e73 7461 6e63 6528 572c 2070   isinstance(W, p
+00011330: 7974 656e 736f 722e 7370 6172 7365 2e53  ytensor.sparse.S
+00011340: 7061 7273 6556 6172 6961 626c 6529 0a20  parseVariable). 
+00011350: 2020 2020 2020 206d 7367 203d 2022 5720         msg = "W 
+00011360: 6d75 7374 2062 6520 6120 7379 6d6d 6574  must be a symmet
+00011370: 7269 6320 6164 6a61 6365 6e63 7920 6d61  ric adjacency ma
+00011380: 7472 6978 2e22 0a20 2020 2020 2020 2069  trix.".        i
+00011390: 6620 7370 6172 7365 3a0a 2020 2020 2020  f sparse:.      
+000113a0: 2020 2020 2020 6162 735f 6469 6666 203d        abs_diff =
+000113b0: 2070 7974 656e 736f 722e 7370 6172 7365   pytensor.sparse
+000113c0: 2e62 6173 6963 2e6d 756c 2870 7974 656e  .basic.mul(pyten
+000113d0: 736f 722e 7370 6172 7365 2e73 6967 6e28  sor.sparse.sign(
+000113e0: 5720 2d20 572e 5429 2c20 5720 2d20 572e  W - W.T), W - W.
+000113f0: 5429 0a20 2020 2020 2020 2020 2020 2057  T).            W
+00011400: 203d 2041 7373 6572 7428 6d73 6729 2857   = Assert(msg)(W
+00011410: 2c20 7074 2e69 7363 6c6f 7365 2870 7974  , pt.isclose(pyt
+00011420: 656e 736f 722e 7370 6172 7365 2e73 705f  ensor.sparse.sp_
+00011430: 7375 6d28 6162 735f 6469 6666 292c 2030  sum(abs_diff), 0
+00011440: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
+00011450: 0a20 2020 2020 2020 2020 2020 2057 203d  .            W =
+00011460: 2041 7373 6572 7428 6d73 6729 2857 2c20   Assert(msg)(W, 
+00011470: 7074 2e61 6c6c 636c 6f73 6528 572c 2057  pt.allclose(W, W
+00011480: 2e54 2929 0a0a 2020 2020 2020 2020 7461  .T))..        ta
+00011490: 7520 3d20 7074 2e61 735f 7465 6e73 6f72  u = pt.as_tensor
+000114a0: 5f76 6172 6961 626c 6528 666c 6f61 7458  _variable(floatX
+000114b0: 2874 6175 2929 0a20 2020 2020 2020 2061  (tau)).        a
+000114c0: 6c70 6861 203d 2070 742e 6173 5f74 656e  lpha = pt.as_ten
+000114d0: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
+000114e0: 6174 5828 616c 7068 6129 290a 0a20 2020  atX(alpha))..   
+000114f0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00011500: 7228 292e 6d61 6b65 5f6e 6f64 6528 726e  r().make_node(rn
+00011510: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
+00011520: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
+00011530: 7529 0a0a 2020 2020 6465 6620 5f69 6e66  u)..    def _inf
+00011540: 6572 5f73 6861 7065 2873 656c 662c 2073  er_shape(self, s
+00011550: 697a 652c 2064 6973 745f 7061 7261 6d73  ize, dist_params
+00011560: 2c20 7061 7261 6d5f 7368 6170 6573 3d4e  , param_shapes=N
+00011570: 6f6e 6529 3a0a 2020 2020 2020 2020 7368  one):.        sh
+00011580: 6170 6520 3d20 7475 706c 6528 7369 7a65  ape = tuple(size
+00011590: 2920 2b20 2864 6973 745f 7061 7261 6d73  ) + (dist_params
+000115a0: 5b30 5d2e 7368 6170 655b 2d31 5d2c 290a  [0].shape[-1],).
+000115b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000115c0: 6861 7065 0a0a 2020 2020 4063 6c61 7373  hape..    @class
+000115d0: 6d65 7468 6f64 0a20 2020 2064 6566 2072  method.    def r
+000115e0: 6e67 5f66 6e28 636c 732c 2072 6e67 3a20  ng_fn(cls, rng: 
+000115f0: 6e70 2e72 616e 646f 6d2e 5261 6e64 6f6d  np.random.Random
+00011600: 5374 6174 652c 206d 752c 2057 2c20 616c  State, mu, W, al
+00011610: 7068 612c 2074 6175 2c20 7369 7a65 293a  pha, tau, size):
+00011620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011630: 2020 2020 2049 6d70 6c65 6d65 6e74 6174       Implementat
+00011640: 696f 6e20 6f66 2061 6c67 6f72 6974 686d  ion of algorithm
+00011650: 2066 726f 6d20 7061 7065 720a 2020 2020   from paper.    
+00011660: 2020 2020 4861 7661 7264 2052 7565 2c20      Havard Rue, 
+00011670: 3230 3031 2e20 2246 6173 7420 7361 6d70  2001. "Fast samp
+00011680: 6c69 6e67 206f 6620 4761 7573 7369 616e  ling of Gaussian
+00011690: 204d 6172 6b6f 7620 7261 6e64 6f6d 2066   Markov random f
+000116a0: 6965 6c64 732c 220a 2020 2020 2020 2020  ields,".        
+000116b0: 4a6f 7572 6e61 6c20 6f66 2074 6865 2052  Journal of the R
+000116c0: 6f79 616c 2053 7461 7469 7374 6963 616c  oyal Statistical
+000116d0: 2053 6f63 6965 7479 2053 6572 6965 7320   Society Series 
+000116e0: 422c 2052 6f79 616c 2053 7461 7469 7374  B, Royal Statist
+000116f0: 6963 616c 2053 6f63 6965 7479 2c0a 2020  ical Society,.  
+00011700: 2020 2020 2020 766f 6c2e 2036 3328 3229        vol. 63(2)
+00011710: 2c20 7061 6765 7320 3332 352d 3333 382e  , pages 325-338.
+00011720: 2044 4f49 3a20 3130 2e31 3131 312f 3134   DOI: 10.1111/14
+00011730: 3637 2d39 3836 382e 3030 3238 380a 2020  67-9868.00288.  
+00011740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011750: 2020 6966 206e 6f74 2073 6369 7079 2e73    if not scipy.s
+00011760: 7061 7273 652e 6973 7370 6172 7365 2857  parse.issparse(W
+00011770: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
+00011780: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
+00011790: 6373 725f 6d61 7472 6978 2857 290a 2020  csr_matrix(W).  
+000117a0: 2020 2020 2020 7320 3d20 6e70 2e61 7361        s = np.asa
+000117b0: 7272 6179 2857 2e73 756d 2861 7869 733d  rray(W.sum(axis=
+000117c0: 3029 295b 305d 0a20 2020 2020 2020 2044  0))[0].        D
+000117d0: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
+000117e0: 6469 6167 7328 7329 0a20 2020 2020 2020  diags(s).       
+000117f0: 2074 6175 203d 2073 6369 7079 2e73 7061   tau = scipy.spa
+00011800: 7273 652e 6373 725f 6d61 7472 6978 2874  rse.csr_matrix(t
+00011810: 6175 290a 2020 2020 2020 2020 616c 7068  au).        alph
+00011820: 6120 3d20 7363 6970 792e 7370 6172 7365  a = scipy.sparse
+00011830: 2e63 7372 5f6d 6174 7269 7828 616c 7068  .csr_matrix(alph
+00011840: 6129 0a0a 2020 2020 2020 2020 5120 3d20  a)..        Q = 
+00011850: 7461 752e 6d75 6c74 6970 6c79 2844 202d  tau.multiply(D -
+00011860: 2061 6c70 6861 2e6d 756c 7469 706c 7928   alpha.multiply(
+00011870: 5729 290a 0a20 2020 2020 2020 2070 6572  W))..        per
+00011880: 6d5f 6172 7261 7920 3d20 7363 6970 792e  m_array = scipy.
+00011890: 7370 6172 7365 2e63 7367 7261 7068 2e72  sparse.csgraph.r
+000118a0: 6576 6572 7365 5f63 7574 6869 6c6c 5f6d  everse_cuthill_m
+000118b0: 636b 6565 2851 2c20 7379 6d6d 6574 7269  ckee(Q, symmetri
+000118c0: 635f 6d6f 6465 3d54 7275 6529 0a20 2020  c_mode=True).   
+000118d0: 2020 2020 2069 6e76 5f70 6572 6d20 3d20       inv_perm = 
+000118e0: 6e70 2e61 7267 736f 7274 2870 6572 6d5f  np.argsort(perm_
+000118f0: 6172 7261 7929 0a0a 2020 2020 2020 2020  array)..        
+00011900: 5120 3d20 515b 7065 726d 5f61 7272 6179  Q = Q[perm_array
+00011910: 2c20 3a5d 5b3a 2c20 7065 726d 5f61 7272  , :][:, perm_arr
+00011920: 6179 5d0a 0a20 2020 2020 2020 2051 6220  ay]..        Qb 
+00011930: 3d20 512e 6469 6167 6f6e 616c 2829 0a20  = Q.diagonal(). 
+00011940: 2020 2020 2020 2075 203d 2031 0a20 2020         u = 1.   
+00011950: 2020 2020 2077 6869 6c65 206e 702e 636f       while np.co
+00011960: 756e 745f 6e6f 6e7a 6572 6f28 512e 6469  unt_nonzero(Q.di
+00011970: 6167 6f6e 616c 2875 2929 203e 2030 3a0a  agonal(u)) > 0:.
+00011980: 2020 2020 2020 2020 2020 2020 5162 203d              Qb =
+00011990: 206e 702e 7673 7461 636b 2828 6e70 2e70   np.vstack((np.p
+000119a0: 6164 2851 2e64 6961 676f 6e61 6c28 7529  ad(Q.diagonal(u)
+000119b0: 2c20 2875 2c20 3029 2c20 636f 6e73 7461  , (u, 0), consta
+000119c0: 6e74 5f76 616c 7565 733d 2830 2c20 3029  nt_values=(0, 0)
+000119d0: 292c 2051 6229 290a 2020 2020 2020 2020  ), Qb)).        
+000119e0: 2020 2020 7520 2b3d 2031 0a0a 2020 2020      u += 1..    
+000119f0: 2020 2020 4c20 3d20 7363 6970 792e 6c69      L = scipy.li
+00011a00: 6e61 6c67 2e63 686f 6c65 736b 795f 6261  nalg.cholesky_ba
+00011a10: 6e64 6564 2851 622c 206c 6f77 6572 3d46  nded(Qb, lower=F
+00011a20: 616c 7365 290a 0a20 2020 2020 2020 2073  alse)..        s
+00011a30: 697a 6520 3d20 7475 706c 6528 7369 7a65  ize = tuple(size
+00011a40: 206f 7220 2829 290a 2020 2020 2020 2020   or ()).        
+00011a50: 6966 2073 697a 653a 0a20 2020 2020 2020  if size:.       
+00011a60: 2020 2020 206d 7520 3d20 6e70 2e62 726f       mu = np.bro
+00011a70: 6164 6361 7374 5f74 6f28 6d75 2c20 7369  adcast_to(mu, si
+00011a80: 7a65 202b 2028 6d75 2e73 6861 7065 5b2d  ze + (mu.shape[-
+00011a90: 315d 2c29 290a 2020 2020 2020 2020 7a20  1],)).        z 
+00011aa0: 3d20 726e 672e 6e6f 726d 616c 2873 697a  = rng.normal(siz
+00011ab0: 653d 6d75 2e73 6861 7065 290a 2020 2020  e=mu.shape).    
+00011ac0: 2020 2020 7361 6d70 6c65 7320 3d20 6e70      samples = np
+00011ad0: 2e65 6d70 7479 287a 2e73 6861 7065 290a  .empty(z.shape).
+00011ae0: 2020 2020 2020 2020 666f 7220 6964 7820          for idx 
+00011af0: 696e 206e 702e 6e64 696e 6465 7828 6d75  in np.ndindex(mu
+00011b00: 2e73 6861 7065 5b3a 2d31 5d29 3a0a 2020  .shape[:-1]):.  
+00011b10: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+00011b20: 735b 6964 785d 203d 2073 6369 7079 2e6c  s[idx] = scipy.l
+00011b30: 696e 616c 672e 6368 6f5f 736f 6c76 655f  inalg.cho_solve_
+00011b40: 6261 6e64 6564 2828 4c2c 2046 616c 7365  banded((L, False
+00011b50: 292c 207a 5b69 6478 5d29 202b 206d 755b  ), z[idx]) + mu[
+00011b60: 6964 785d 5b70 6572 6d5f 6172 7261 795d  idx][perm_array]
+00011b70: 0a20 2020 2020 2020 2073 616d 706c 6573  .        samples
+00011b80: 203d 2073 616d 706c 6573 5b2e 2e2e 2c20   = samples[..., 
+00011b90: 696e 765f 7065 726d 5d0a 2020 2020 2020  inv_perm].      
+00011ba0: 2020 7265 7475 726e 2073 616d 706c 6573    return samples
+00011bb0: 0a0a 0a63 6172 203d 2043 4152 5256 2829  ...car = CARRV()
+00011bc0: 0a0a 0a63 6c61 7373 2043 4152 2843 6f6e  ...class CAR(Con
+00011bd0: 7469 6e75 6f75 7329 3a0a 2020 2020 7222  tinuous):.    r"
+00011be0: 2222 0a20 2020 204c 696b 656c 6968 6f6f  "".    Likelihoo
+00011bf0: 6420 666f 7220 6120 636f 6e64 6974 696f  d for a conditio
+00011c00: 6e61 6c20 6175 746f 7265 6772 6573 7369  nal autoregressi
+00011c10: 6f6e 2e20 5468 6973 2069 7320 6120 7370  on. This is a sp
+00011c20: 6563 6961 6c20 6361 7365 206f 6620 7468  ecial case of th
+00011c30: 650a 2020 2020 6d75 6c74 6976 6172 6961  e.    multivaria
+00011c40: 7465 206e 6f72 6d61 6c20 7769 7468 2061  te normal with a
+00011c50: 6e20 6164 6a61 6365 6e63 792d 7374 7275  n adjacency-stru
+00011c60: 6374 7572 6564 2063 6f76 6172 6961 6e63  ctured covarianc
+00011c70: 6520 6d61 7472 6978 2e0a 0a20 2020 202e  e matrix...    .
+00011c80: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
+00011c90: 2066 2878 205c 6d69 6420 572c 205c 616c   f(x \mid W, \al
+00011ca0: 7068 612c 205c 7461 7529 203d 0a20 2020  pha, \tau) =.   
+00011cb0: 2020 2020 2020 2020 5c66 7261 637b 7c54          \frac{|T
+00011cc0: 7c5e 7b31 2f32 7d7d 7b28 325c 7069 295e  |^{1/2}}{(2\pi)^
+00011cd0: 7b6b 2f32 7d7d 0a20 2020 2020 2020 2020  {k/2}}.         
+00011ce0: 2020 5c65 7870 5c6c 6566 745c 7b20 2d5c    \exp\left\{ -\
+00011cf0: 6672 6163 7b31 7d7b 327d 2028 782d 5c6d  frac{1}{2} (x-\m
+00011d00: 7529 5e7b 5c70 7269 6d65 7d20 545e 7b2d  u)^{\prime} T^{-
+00011d10: 317d 2028 782d 5c6d 7529 205c 7269 6768  1} (x-\mu) \righ
+00011d20: 745c 7d0a 0a20 2020 2077 6865 7265 203a  t\}..    where :
+00011d30: 6d61 7468 3a60 5420 3d20 285c 7461 7520  math:`T = (\tau 
+00011d40: 4428 492d 5c61 6c70 6861 2057 2929 5e7b  D(I-\alpha W))^{
+00011d50: 2d31 7d60 2061 6e64 203a 6d61 7468 3a60  -1}` and :math:`
+00011d60: 4420 3d20 6469 6167 285c 7375 6d5f 6920  D = diag(\sum_i 
+00011d70: 575f 7b69 6a7d 2960 2e0a 0a20 2020 203d  W_{ij})`...    =
+00011d80: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
+00011d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011da0: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
+00011db0: 2020 3a6d 6174 683a 6078 205c 696e 205c    :math:`x \in \
+00011dc0: 6d61 7468 6262 7b52 7d5e 6b60 0a20 2020  mathbb{R}^k`.   
+00011dd0: 204d 6561 6e20 2020 2020 203a 6d61 7468   Mean      :math
+00011de0: 3a60 5c6d 7520 5c69 6e20 5c6d 6174 6862  :`\mu \in \mathb
+00011df0: 627b 527d 5e6b 600a 2020 2020 5661 7269  b{R}^k`.    Vari
+00011e00: 616e 6365 2020 3a6d 6174 683a 6028 5c74  ance  :math:`(\t
+00011e10: 6175 2044 2849 2d5c 616c 7068 6120 5729  au D(I-\alpha W)
+00011e20: 295e 7b2d 317d 600a 2020 2020 3d3d 3d3d  )^{-1}`.    ====
+00011e30: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00011e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011e50: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00011e60: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00011e70: 2020 2020 6d75 203a 2074 656e 736f 725f      mu : tensor_
+00011e80: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
+00011e90: 2020 2020 2020 5265 616c 2d76 616c 7565        Real-value
+00011ea0: 6420 6d65 616e 2076 6563 746f 720a 2020  d mean vector.  
+00011eb0: 2020 5720 3a20 284d 2c20 4d29 2074 656e    W : (M, M) ten
+00011ec0: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
+00011ed0: 2020 2020 2020 2020 5379 6d6d 6574 7269          Symmetri
+00011ee0: 6320 6164 6a61 6365 6e63 7920 6d61 7472  c adjacency matr
+00011ef0: 6978 206f 6620 3173 2061 6e64 2030 7320  ix of 1s and 0s 
+00011f00: 696e 6469 6361 7469 6e67 0a20 2020 2020  indicating.     
+00011f10: 2020 2061 646a 6163 656e 6379 2062 6574     adjacency bet
+00011f20: 7765 656e 2065 6c65 6d65 6e74 732e 2049  ween elements. I
+00011f30: 6620 706f 7373 6962 6c65 2c20 2a57 2a20  f possible, *W* 
+00011f40: 6973 2063 6f6e 7665 7274 6564 0a20 2020  is converted.   
+00011f50: 2020 2020 2074 6f20 6120 7370 6172 7365       to a sparse
+00011f60: 206d 6174 7269 782c 2066 616c 6c69 6e67   matrix, falling
+00011f70: 2062 6163 6b20 746f 2061 2064 656e 7365   back to a dense
+00011f80: 2076 6172 6961 626c 652e 0a20 2020 2020   variable..     
+00011f90: 2020 203a 6675 6e63 3a60 7e70 7974 656e     :func:`~pyten
+00011fa0: 736f 722e 7370 6172 7365 2e62 6173 6963  sor.sparse.basic
+00011fb0: 2e61 735f 7370 6172 7365 5f6f 725f 7465  .as_sparse_or_te
+00011fc0: 6e73 6f72 5f76 6172 6961 626c 6560 2069  nsor_variable` i
+00011fd0: 730a 2020 2020 2020 2020 7573 6564 2066  s.        used f
+00011fe0: 6f72 2074 6869 7320 7370 6172 7365 206f  or this sparse o
+00011ff0: 7220 7465 6e73 6f72 7661 7269 6162 6c65  r tensorvariable
+00012000: 2063 6f6e 7665 7273 696f 6e2e 0a20 2020   conversion..   
+00012010: 2061 6c70 6861 203a 2074 656e 736f 725f   alpha : tensor_
+00012020: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
+00012030: 2020 2020 2020 4175 746f 7265 6772 6573        Autoregres
+00012040: 7369 6f6e 2070 6172 616d 6574 6572 2074  sion parameter t
+00012050: 616b 696e 6720 7661 6c75 6573 2062 6574  aking values bet
+00012060: 7765 656e 202d 3120 616e 6420 312e 2056  ween -1 and 1. V
+00012070: 616c 7565 7320 636c 6f73 6572 2074 6f20  alues closer to 
+00012080: 3020 696e 6469 6361 7465 2077 6561 6b65  0 indicate weake
+00012090: 720a 2020 2020 2020 2020 636f 7272 656c  r.        correl
+000120a0: 6174 696f 6e20 616e 6420 7661 6c75 6573  ation and values
+000120b0: 2063 6c6f 7365 7220 746f 2031 2069 6e64   closer to 1 ind
+000120c0: 6963 6174 6520 6869 6768 6572 2061 7574  icate higher aut
+000120d0: 6f63 6f72 7265 6c61 7469 6f6e 2e20 466f  ocorrelation. Fo
+000120e0: 7220 6d6f 7374 2075 7365 2063 6173 6573  r most use cases
+000120f0: 2c20 7468 650a 2020 2020 2020 2020 7375  , the.        su
+00012100: 7070 6f72 7420 6f66 2061 6c70 6861 2073  pport of alpha s
+00012110: 686f 756c 6420 6265 2072 6573 7472 6963  hould be restric
+00012120: 7465 6420 746f 2028 302c 2031 292e 0a20  ted to (0, 1).. 
+00012130: 2020 2074 6175 203a 2074 656e 736f 725f     tau : tensor_
+00012140: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
+00012150: 2020 2020 2020 506f 7369 7469 7665 2070        Positive p
+00012160: 7265 6369 7369 6f6e 2076 6172 6961 626c  recision variabl
+00012170: 6520 636f 6e74 726f 6c6c 696e 6720 7468  e controlling th
+00012180: 6520 7363 616c 6520 6f66 2074 6865 2075  e scale of the u
+00012190: 6e64 6572 6c79 696e 6720 6e6f 726d 616c  nderlying normal
+000121a0: 2076 6172 6961 7465 732e 0a0a 2020 2020   variates...    
+000121b0: 5265 6665 7265 6e63 6573 0a20 2020 202d  References.    -
+000121c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e  ---------.    ..
+000121d0: 2020 4a69 6e2c 2058 2e2c 2043 6172 6c69    Jin, X., Carli
+000121e0: 6e2c 2042 2e2c 2042 616e 6572 6a65 652c  n, B., Banerjee,
+000121f0: 2053 2e0a 2020 2020 2020 2020 2247 656e   S..        "Gen
+00012200: 6572 616c 697a 6564 2048 6965 7261 7263  eralized Hierarc
+00012210: 6869 6361 6c20 4d75 6c74 6976 6172 6961  hical Multivaria
+00012220: 7465 2043 4152 204d 6f64 656c 7320 666f  te CAR Models fo
+00012230: 7220 4172 6561 6c20 4461 7461 220a 2020  r Areal Data".  
+00012240: 2020 2020 2020 4269 6f6d 6574 7269 6373        Biometrics
+00012250: 2c20 566f 6c2e 2036 312c 204e 6f2e 2034  , Vol. 61, No. 4
+00012260: 2028 4465 632e 2c20 3230 3035 292c 2070   (Dec., 2005), p
+00012270: 702e 2039 3530 2d39 3631 0a20 2020 2022  p. 950-961.    "
+00012280: 2222 0a20 2020 2072 765f 6f70 203d 2063  "".    rv_op = c
+00012290: 6172 0a0a 2020 2020 4063 6c61 7373 6d65  ar..    @classme
+000122a0: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
+000122b0: 7428 636c 732c 206d 752c 2057 2c20 616c  t(cls, mu, W, al
+000122c0: 7068 612c 2074 6175 2c20 2a61 7267 732c  pha, tau, *args,
+000122d0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+000122e0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+000122f0: 2829 2e64 6973 7428 5b6d 752c 2057 2c20  ().dist([mu, W, 
+00012300: 616c 7068 612c 2074 6175 5d2c 202a 2a6b  alpha, tau], **k
+00012310: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00012320: 6d6f 6d65 6e74 2872 762c 2073 697a 652c  moment(rv, size,
+00012330: 206d 752c 2057 2c20 616c 7068 612c 2074   mu, W, alpha, t
+00012340: 6175 293a 0a20 2020 2020 2020 2072 6574  au):.        ret
+00012350: 7572 6e20 7074 2e66 756c 6c5f 6c69 6b65  urn pt.full_like
+00012360: 2872 762c 206d 7529 0a0a 2020 2020 6465  (rv, mu)..    de
+00012370: 6620 6c6f 6770 2876 616c 7565 2c20 6d75  f logp(value, mu
+00012380: 2c20 572c 2061 6c70 6861 2c20 7461 7529  , W, alpha, tau)
+00012390: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000123a0: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
+000123b0: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
+000123c0: 6f66 2061 2043 4152 2d64 6973 7472 6962  of a CAR-distrib
+000123d0: 7574 6564 2076 6563 746f 720a 2020 2020  uted vector.    
+000123e0: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
+000123f0: 2076 616c 7565 2e20 5468 6973 206c 6f67   value. This log
+00012400: 2070 726f 6261 6269 6c69 7479 2066 756e   probability fun
+00012410: 6374 696f 6e20 6469 6666 6572 7320 6672  ction differs fr
+00012420: 6f6d 0a20 2020 2020 2020 2074 6865 2074  om.        the t
+00012430: 7275 6520 4341 5220 6c6f 6720 6465 6e73  rue CAR log dens
+00012440: 6974 7920 2841 4b41 2061 206d 756c 7469  ity (AKA a multi
+00012450: 7661 7269 6174 6520 6e6f 726d 616c 2077  variate normal w
+00012460: 6974 6820 4341 522d 7374 7275 6374 7572  ith CAR-structur
+00012470: 6564 0a20 2020 2020 2020 2063 6f76 6172  ed.        covar
+00012480: 6961 6e63 6520 6d61 7472 6978 2920 6279  iance matrix) by
+00012490: 2061 6e20 6164 6469 7469 7665 2063 6f6e   an additive con
+000124a0: 7374 616e 742e 0a0a 2020 2020 2020 2020  stant...        
+000124b0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000124c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000124d0: 2020 2020 2020 7661 6c75 653a 2061 7272        value: arr
+000124e0: 6179 0a20 2020 2020 2020 2020 2020 2056  ay.            V
+000124f0: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
+00012500: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
+00012510: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
+00012520: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00012530: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00012540: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
+00012550: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
+00012560: 220a 0a20 2020 2020 2020 2073 7061 7273  "..        spars
+00012570: 6520 3d20 6973 696e 7374 616e 6365 2857  e = isinstance(W
+00012580: 2c20 2870 7974 656e 736f 722e 7370 6172  , (pytensor.spar
+00012590: 7365 2e53 7061 7273 6543 6f6e 7374 616e  se.SparseConstan
+000125a0: 742c 2070 7974 656e 736f 722e 7370 6172  t, pytensor.spar
+000125b0: 7365 2e53 7061 7273 6556 6172 6961 626c  se.SparseVariabl
+000125c0: 6529 290a 0a20 2020 2020 2020 2069 6620  e))..        if 
+000125d0: 7370 6172 7365 3a0a 2020 2020 2020 2020  sparse:.        
+000125e0: 2020 2020 4420 3d20 7370 5f73 756d 2857      D = sp_sum(W
+000125f0: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
+00012600: 2020 2020 2020 4469 6e76 5f73 7172 7420        Dinv_sqrt 
+00012610: 3d20 7074 2e64 6961 6728 3120 2f20 7074  = pt.diag(1 / pt
+00012620: 2e73 7172 7428 4429 290a 2020 2020 2020  .sqrt(D)).      
+00012630: 2020 2020 2020 4457 4420 3d20 7074 2e64        DWD = pt.d
+00012640: 6f74 2870 7974 656e 736f 722e 7370 6172  ot(pytensor.spar
+00012650: 7365 2e64 6f74 2844 696e 765f 7371 7274  se.dot(Dinv_sqrt
+00012660: 2c20 5729 2c20 4469 6e76 5f73 7172 7429  , W), Dinv_sqrt)
+00012670: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00012680: 2020 2020 2020 2020 2020 2044 203d 2057             D = W
+00012690: 2e73 756d 2861 7869 733d 3029 0a20 2020  .sum(axis=0).   
+000126a0: 2020 2020 2020 2020 2044 696e 765f 7371           Dinv_sq
+000126b0: 7274 203d 2070 742e 6469 6167 2831 202f  rt = pt.diag(1 /
+000126c0: 2070 742e 7371 7274 2844 2929 0a20 2020   pt.sqrt(D)).   
+000126d0: 2020 2020 2020 2020 2044 5744 203d 2070           DWD = p
+000126e0: 742e 646f 7428 7074 2e64 6f74 2844 696e  t.dot(pt.dot(Din
+000126f0: 765f 7371 7274 2c20 5729 2c20 4469 6e76  v_sqrt, W), Dinv
+00012700: 5f73 7172 7429 0a20 2020 2020 2020 206c  _sqrt).        l
+00012710: 616d 203d 2070 742e 736c 696e 616c 672e  am = pt.slinalg.
+00012720: 6569 6776 616c 7368 2844 5744 2c20 7074  eigvalsh(DWD, pt
+00012730: 2e65 7965 2844 5744 2e73 6861 7065 5b30  .eye(DWD.shape[0
+00012740: 5d29 290a 0a20 2020 2020 2020 2064 2c20  ]))..        d, 
+00012750: 5f20 3d20 572e 7368 6170 650a 0a20 2020  _ = W.shape..   
+00012760: 2020 2020 2069 6620 7661 6c75 652e 6e64       if value.nd
+00012770: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00012780: 2020 2020 2076 616c 7565 203d 2076 616c       value = val
+00012790: 7565 5b4e 6f6e 652c 203a 5d0a 0a20 2020  ue[None, :]..   
+000127a0: 2020 2020 206c 6f67 7461 7520 3d20 6420       logtau = d 
+000127b0: 2a20 7074 2e6c 6f67 2874 6175 292e 7375  * pt.log(tau).su
+000127c0: 6d28 290a 2020 2020 2020 2020 6c6f 6764  m().        logd
+000127d0: 6574 203d 2070 742e 6c6f 6728 3120 2d20  et = pt.log(1 - 
+000127e0: 616c 7068 612e 5420 2a20 6c61 6d5b 3a2c  alpha.T * lam[:,
+000127f0: 204e 6f6e 655d 292e 7375 6d28 290a 2020   None]).sum().  
+00012800: 2020 2020 2020 6465 6c74 6120 3d20 7661        delta = va
+00012810: 6c75 6520 2d20 6d75 0a0a 2020 2020 2020  lue - mu..      
+00012820: 2020 6966 2073 7061 7273 653a 0a20 2020    if sparse:.   
+00012830: 2020 2020 2020 2020 2057 6465 6c74 6120           Wdelta 
+00012840: 3d20 7079 7465 6e73 6f72 2e73 7061 7273  = pytensor.spars
+00012850: 652e 646f 7428 6465 6c74 612c 2057 290a  e.dot(delta, W).
+00012860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00012870: 2020 2020 2020 2020 2020 5764 656c 7461            Wdelta
+00012880: 203d 2070 742e 646f 7428 6465 6c74 612c   = pt.dot(delta,
+00012890: 2057 290a 0a20 2020 2020 2020 2074 6175   W)..        tau
+000128a0: 5f64 6f74 5f64 656c 7461 203d 2044 5b4e  _dot_delta = D[N
+000128b0: 6f6e 652c 203a 5d20 2a20 6465 6c74 6120  one, :] * delta 
+000128c0: 2d20 616c 7068 6120 2a20 5764 656c 7461  - alpha * Wdelta
+000128d0: 0a20 2020 2020 2020 206c 6f67 7175 6164  .        logquad
+000128e0: 203d 2028 7461 7520 2a20 6465 6c74 6120   = (tau * delta 
+000128f0: 2a20 7461 755f 646f 745f 6465 6c74 6129  * tau_dot_delta)
+00012900: 2e73 756d 2861 7869 733d 2d31 290a 2020  .sum(axis=-1).  
+00012910: 2020 2020 2020 7265 7475 726e 2063 6865        return che
+00012920: 636b 5f70 6172 616d 6574 6572 7328 0a20  ck_parameters(. 
+00012930: 2020 2020 2020 2020 2020 2030 2e35 202a             0.5 *
+00012940: 2028 6c6f 6774 6175 202b 206c 6f67 6465   (logtau + logde
+00012950: 7420 2d20 6c6f 6771 7561 6429 2c0a 2020  t - logquad),.  
+00012960: 2020 2020 2020 2020 2020 2d31 203c 3d20            -1 <= 
+00012970: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
+00012980: 2020 2061 6c70 6861 203c 3d20 312c 0a20     alpha <= 1,. 
+00012990: 2020 2020 2020 2020 2020 2074 6175 203e             tau >
+000129a0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+000129b0: 6d73 673d 222d 3120 3c3d 2061 6c70 6861  msg="-1 <= alpha
+000129c0: 203c 3d20 312c 2074 6175 203e 2030 222c   <= 1, tau > 0",
+000129d0: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+000129e0: 7373 2053 7469 636b 4272 6561 6b69 6e67  ss StickBreaking
+000129f0: 5765 6967 6874 7352 5628 5261 6e64 6f6d  WeightsRV(Random
+00012a00: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
+00012a10: 616d 6520 3d20 2273 7469 636b 5f62 7265  ame = "stick_bre
+00012a20: 616b 696e 675f 7765 6967 6874 7322 0a20  aking_weights". 
+00012a30: 2020 206e 6469 6d5f 7375 7070 203d 2031     ndim_supp = 1
+00012a40: 0a20 2020 206e 6469 6d73 5f70 6172 616d  .    ndims_param
+00012a50: 7320 3d20 5b30 2c20 305d 0a20 2020 2064  s = [0, 0].    d
+00012a60: 7479 7065 203d 2022 666c 6f61 7458 220a  type = "floatX".
+00012a70: 2020 2020 5f70 7269 6e74 5f6e 616d 6520      _print_name 
+00012a80: 3d20 2822 5374 6963 6b42 7265 616b 696e  = ("StickBreakin
+00012a90: 6757 6569 6768 7473 222c 2022 5c5c 6f70  gWeights", "\\op
+00012aa0: 6572 6174 6f72 6e61 6d65 7b53 7469 636b  eratorname{Stick
+00012ab0: 4272 6561 6b69 6e67 5765 6967 6874 737d  BreakingWeights}
+00012ac0: 2229 0a0a 2020 2020 6465 6620 6d61 6b65  ")..    def make
+00012ad0: 5f6e 6f64 6528 7365 6c66 2c20 726e 672c  _node(self, rng,
+00012ae0: 2073 697a 652c 2064 7479 7065 2c20 616c   size, dtype, al
+00012af0: 7068 612c 204b 293a 0a20 2020 2020 2020  pha, K):.       
+00012b00: 2061 6c70 6861 203d 2070 742e 6173 5f74   alpha = pt.as_t
+00012b10: 656e 736f 725f 7661 7269 6162 6c65 2861  ensor_variable(a
+00012b20: 6c70 6861 290a 2020 2020 2020 2020 4b20  lpha).        K 
+00012b30: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00012b40: 6172 6961 626c 6528 696e 7458 284b 2929  ariable(intX(K))
+00012b50: 0a0a 2020 2020 2020 2020 6966 204b 2e6e  ..        if K.n
+00012b60: 6469 6d20 3e20 303a 0a20 2020 2020 2020  dim > 0:.       
+00012b70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00012b80: 4572 726f 7228 224b 206d 7573 7420 6265  Error("K must be
+00012b90: 2061 2073 6361 6c61 722e 2229 0a0a 2020   a scalar.")..  
+00012ba0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+00012bb0: 6572 2829 2e6d 616b 655f 6e6f 6465 2872  er().make_node(r
+00012bc0: 6e67 2c20 7369 7a65 2c20 6474 7970 652c  ng, size, dtype,
+00012bd0: 2061 6c70 6861 2c20 4b29 0a0a 2020 2020   alpha, K)..    
+00012be0: 6465 6620 5f73 7570 705f 7368 6170 655f  def _supp_shape_
+00012bf0: 6672 6f6d 5f70 6172 616d 7328 7365 6c66  from_params(self
+00012c00: 2c20 6469 7374 5f70 6172 616d 732c 202a  , dist_params, *
+00012c10: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00012c20: 2020 4b20 3d20 6469 7374 5f70 6172 616d    K = dist_param
+00012c30: 735b 315d 0a20 2020 2020 2020 2072 6574  s[1].        ret
+00012c40: 7572 6e20 284b 202b 2031 2c29 0a0a 2020  urn (K + 1,)..  
+00012c50: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00012c60: 2020 2064 6566 2072 6e67 5f66 6e28 636c     def rng_fn(cl
+00012c70: 732c 2072 6e67 2c20 616c 7068 612c 204b  s, rng, alpha, K
+00012c80: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
+00012c90: 2069 6620 4b20 3c20 303a 0a20 2020 2020   if K < 0:.     
+00012ca0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00012cb0: 7565 4572 726f 7228 224b 206e 6565 6473  ueError("K needs
+00012cc0: 2074 6f20 6265 2070 6f73 6974 6976 652e   to be positive.
+00012cd0: 2229 0a0a 2020 2020 2020 2020 7369 7a65  ")..        size
+00012ce0: 203d 2074 6f5f 7475 706c 6528 7369 7a65   = to_tuple(size
+00012cf0: 2920 6966 2073 697a 6520 6973 206e 6f74  ) if size is not
+00012d00: 204e 6f6e 6520 656c 7365 2061 6c70 6861   None else alpha
+00012d10: 2e73 6861 7065 0a20 2020 2020 2020 2073  .shape.        s
+00012d20: 697a 6520 3d20 7369 7a65 202b 2028 4b2c  ize = size + (K,
+00012d30: 290a 2020 2020 2020 2020 616c 7068 6120  ).        alpha 
+00012d40: 3d20 616c 7068 615b 2e2e 2e2c 206e 702e  = alpha[..., np.
+00012d50: 6e65 7761 7869 735d 0a0a 2020 2020 2020  newaxis]..      
+00012d60: 2020 6265 7461 7320 3d20 726e 672e 6265    betas = rng.be
+00012d70: 7461 2831 2c20 616c 7068 612c 2073 697a  ta(1, alpha, siz
+00012d80: 653d 7369 7a65 290a 0a20 2020 2020 2020  e=size)..       
+00012d90: 2073 7469 636b 7320 3d20 6e70 2e63 6f6e   sticks = np.con
+00012da0: 6361 7465 6e61 7465 280a 2020 2020 2020  catenate(.      
+00012db0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00012dc0: 2020 2020 2020 2020 6e70 2e6f 6e65 7328          np.ones(
+00012dd0: 7368 6170 653d 2873 697a 655b 3a2d 315d  shape=(size[:-1]
+00012de0: 202b 2028 312c 2929 292c 0a20 2020 2020   + (1,))),.     
+00012df0: 2020 2020 2020 2020 2020 206e 702e 6375             np.cu
+00012e00: 6d70 726f 6428 3120 2d20 6265 7461 735b  mprod(1 - betas[
+00012e10: 2e2e 2e2c 203a 2d31 5d2c 2061 7869 733d  ..., :-1], axis=
+00012e20: 2d31 292c 0a20 2020 2020 2020 2020 2020  -1),.           
+00012e30: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00012e40: 6178 6973 3d2d 312c 0a20 2020 2020 2020  axis=-1,.       
+00012e50: 2029 0a0a 2020 2020 2020 2020 7765 6967   )..        weig
+00012e60: 6874 7320 3d20 7374 6963 6b73 202a 2062  hts = sticks * b
+00012e70: 6574 6173 0a20 2020 2020 2020 2077 6569  etas.        wei
+00012e80: 6768 7473 203d 206e 702e 636f 6e63 6174  ghts = np.concat
+00012e90: 656e 6174 6528 0a20 2020 2020 2020 2020  enate(.         
+00012ea0: 2020 2028 7765 6967 6874 732c 2031 202d     (weights, 1 -
+00012eb0: 2077 6569 6768 7473 2e73 756d 2861 7869   weights.sum(axi
+00012ec0: 733d 2d31 295b 2e2e 2e2c 206e 702e 6e65  s=-1)[..., np.ne
+00012ed0: 7761 7869 735d 292c 0a20 2020 2020 2020  waxis]),.       
+00012ee0: 2020 2020 2061 7869 733d 2d31 2c0a 2020       axis=-1,.  
+00012ef0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00012f00: 2072 6574 7572 6e20 7765 6967 6874 730a   return weights.
+00012f10: 0a0a 7374 6963 6b62 7265 616b 696e 6777  ..stickbreakingw
+00012f20: 6569 6768 7473 203d 2053 7469 636b 4272  eights = StickBr
+00012f30: 6561 6b69 6e67 5765 6967 6874 7352 5628  eakingWeightsRV(
+00012f40: 290a 0a0a 636c 6173 7320 5374 6963 6b42  )...class StickB
+00012f50: 7265 616b 696e 6757 6569 6768 7473 2853  reakingWeights(S
+00012f60: 696d 706c 6578 436f 6e74 696e 756f 7573  implexContinuous
+00012f70: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+00012f80: 4c69 6b65 6c69 686f 6f64 206f 6620 7472  Likelihood of tr
+00012f90: 756e 6361 7465 6420 7374 6963 6b2d 6272  uncated stick-br
+00012fa0: 6561 6b69 6e67 2077 6569 6768 7473 2e20  eaking weights. 
+00012fb0: 5468 6520 7765 6967 6874 7320 6172 6520  The weights are 
+00012fc0: 6765 6e65 7261 7465 6420 6672 6f6d 2061  generated from a
+00012fd0: 0a20 2020 2073 7469 636b 2d62 7265 616b  .    stick-break
+00012fe0: 696e 6720 7072 6f63 6564 7563 6520 7768  ing proceduce wh
+00012ff0: 6572 6520 3a6d 6174 683a 6078 5f6b 203d  ere :math:`x_k =
+00013000: 2076 5f6b 205c 7072 6f64 5f7b 5c65 6c6c   v_k \prod_{\ell
+00013010: 203c 206b 7d20 2831 202d 2076 5f5c 656c   < k} (1 - v_\el
+00013020: 6c29 6020 666f 720a 2020 2020 3a6d 6174  l)` for.    :mat
+00013030: 683a 606b 205c 696e 205c 7b31 2c20 5c6c  h:`k \in \{1, \l
+00013040: 646f 7473 2c20 4b5c 7d60 2061 6e64 203a  dots, K\}` and :
+00013050: 6d61 7468 3a60 785f 4b20 3d20 5c70 726f  math:`x_K = \pro
+00013060: 645f 7b5c 656c 6c20 3d20 317d 5e7b 4b7d  d_{\ell = 1}^{K}
+00013070: 2028 3120 2d20 765f 5c65 6c6c 2920 3d20   (1 - v_\ell) = 
+00013080: 3120 2d20 5c73 756d 5f7b 5c65 6c6c 3d31  1 - \sum_{\ell=1
+00013090: 7d5e 4b20 785f 5c65 6c6c 600a 2020 2020  }^K x_\ell`.    
+000130a0: 7769 7468 203a 6d61 7468 3a60 765f 6b20  with :math:`v_k 
+000130b0: 5c73 7461 636b 7265 6c7b 5c74 6578 747b  \stackrel{\text{
+000130c0: 692e 692e 642e 7d7d 7b5c 7369 6d7d 205c  i.i.d.}}{\sim} \
+000130d0: 7465 7874 7b42 6574 617d 2831 2c20 5c61  text{Beta}(1, \a
+000130e0: 6c70 6861 2960 2e0a 0a20 2020 202e 2e20  lpha)`...    .. 
+000130f0: 6d61 7468 3a0a 0a20 2020 2020 2020 2066  math:..        f
+00013100: 285c 6d61 7468 6266 7b78 7d7c 5c61 6c70  (\mathbf{x}|\alp
+00013110: 6861 2c20 4b29 203d 0a20 2020 2020 2020  ha, K) =.       
+00013120: 2020 2020 2042 2831 2c20 5c61 6c70 6861       B(1, \alpha
+00013130: 295e 7b2d 4b7d 785f 7b4b 2b31 7d5e 5c61  )^{-K}x_{K+1}^\a
+00013140: 6c70 6861 205c 7072 6f64 5f7b 6b3d 317d  lpha \prod_{k=1}
+00013150: 5e7b 4b2b 317d 5c6c 6566 745c 7b5c 7375  ^{K+1}\left\{\su
+00013160: 6d5f 7b6a 3d6b 7d5e 7b4b 2b31 7d20 785f  m_{j=k}^{K+1} x_
+00013170: 6a5c 7269 6768 745c 7d5e 7b2d 317d 0a0a  j\right\}^{-1}..
+00013180: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+00013190: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000131a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000131b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+000131c0: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
+000131d0: 683a 6078 5f6b 205c 696e 2028 302c 2031  h:`x_k \in (0, 1
+000131e0: 2960 2066 6f72 203a 6d61 7468 3a60 6b20  )` for :math:`k 
+000131f0: 5c69 6e20 5c7b 312c 205c 6c64 6f74 732c  \in \{1, \ldots,
+00013200: 204b 2b31 5c7d 600a 2020 2020 2020 2020   K+1\}`.        
+00013210: 2020 2020 2020 7375 6368 2074 6861 7420        such that 
+00013220: 3a6d 6174 683a 605c 7375 6d20 785f 6b20  :math:`\sum x_k 
+00013230: 3d20 3160 0a20 2020 204d 6561 6e20 2020  = 1`.    Mean   
+00013240: 2020 203a 6d61 7468 3a60 5c6d 6174 6862     :math:`\mathb
+00013250: 627b 457d 5b78 5f6b 5d20 3d20 5c64 6672  b{E}[x_k] = \dfr
+00013260: 6163 7b31 7d7b 3120 2b20 5c61 6c70 6861  ac{1}{1 + \alpha
+00013270: 7d5c 6c65 6674 285c 6466 7261 637b 5c61  }\left(\dfrac{\a
+00013280: 6c70 6861 7d7b 3120 2b20 5c61 6c70 6861  lpha}{1 + \alpha
+00013290: 7d5c 7269 6768 7429 5e7b 6b20 2d20 317d  }\right)^{k - 1}
+000132a0: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
+000132b0: 666f 7220 3a6d 6174 683a 606b 205c 696e  for :math:`k \in
+000132c0: 205c 7b31 2c20 5c6c 646f 7473 2c20 4b5c   \{1, \ldots, K\
+000132d0: 7d60 2061 6e64 203a 6d61 7468 3a60 5c6d  }` and :math:`\m
+000132e0: 6174 6862 627b 457d 5b78 5f7b 4b2b 317d  athbb{E}[x_{K+1}
+000132f0: 5d20 3d20 5c6c 6566 7428 5c64 6672 6163  ] = \left(\dfrac
+00013300: 7b5c 616c 7068 617d 7b31 202b 205c 616c  {\alpha}{1 + \al
+00013310: 7068 617d 5c72 6967 6874 295e 7b4b 7d60  pha}\right)^{K}`
+00013320: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
+00013330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+00013360: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00013370: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00013380: 2020 616c 7068 6120 3a20 7465 6e73 6f72    alpha : tensor
+00013390: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+000133a0: 2020 2020 2020 2043 6f6e 6365 6e74 7261         Concentra
+000133b0: 7469 6f6e 2070 6172 616d 6574 6572 2028  tion parameter (
+000133c0: 616c 7068 6120 3e20 3029 2e0a 2020 2020  alpha > 0)..    
+000133d0: 4b20 3a20 7465 6e73 6f72 5f6c 696b 6520  K : tensor_like 
+000133e0: 6f66 2069 6e74 0a20 2020 2020 2020 2054  of int.        T
+000133f0: 6865 206e 756d 6265 7220 6f66 2022 7374  he number of "st
+00013400: 6963 6b73 2220 746f 2062 7265 616b 206f  icks" to break o
+00013410: 6666 2066 726f 6d20 616e 2069 6e69 7469  ff from an initi
+00013420: 616c 206f 6e65 2d75 6e69 7420 7374 6963  al one-unit stic
+00013430: 6b2e 2054 6865 206c 656e 6774 6820 6f66  k. The length of
+00013440: 2074 6865 2077 6569 6768 740a 2020 2020   the weight.    
+00013450: 2020 2020 7665 6374 6f72 2069 7320 4b20      vector is K 
+00013460: 2b20 312c 2077 6865 7265 2074 6865 206c  + 1, where the l
+00013470: 6173 7420 7765 6967 6874 2069 7320 6f6e  ast weight is on
+00013480: 6520 6d69 6e75 7320 7468 6520 7375 6d20  e minus the sum 
+00013490: 6f66 2061 6c6c 2074 6865 2066 6972 7374  of all the first
+000134a0: 2073 7469 636b 732e 0a0a 2020 2020 5265   sticks...    Re
+000134b0: 6665 7265 6e63 6573 0a20 2020 202d 2d2d  ferences.    ---
+000134c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e 205b  -------.    .. [
+000134d0: 315d 2049 7368 7761 7261 6e2c 2048 2e2c  1] Ishwaran, H.,
+000134e0: 2026 204a 616d 6573 2c20 4c2e 2046 2e20   & James, L. F. 
+000134f0: 2832 3030 3129 2e20 4769 6262 7320 7361  (2001). Gibbs sa
+00013500: 6d70 6c69 6e67 206d 6574 686f 6473 2066  mpling methods f
+00013510: 6f72 2073 7469 636b 2d62 7265 616b 696e  or stick-breakin
+00013520: 6720 7072 696f 7273 2e0a 2020 2020 2020  g priors..      
+00013530: 2020 2020 204a 6f75 726e 616c 206f 6620       Journal of 
+00013540: 7468 6520 416d 6572 6963 616e 2053 7461  the American Sta
+00013550: 7469 7374 6963 616c 2041 7373 6f63 6961  tistical Associa
+00013560: 7469 6f6e 2c20 3936 2834 3533 292c 2031  tion, 96(453), 1
+00013570: 3631 2d31 3733 2e0a 0a20 2020 202e 2e20  61-173...    .. 
+00013580: 5b32 5d20 4dc3 bc6c 6c65 722c 2050 2e2c  [2] M..ller, P.,
+00013590: 2051 7569 6e74 616e 612c 2046 2e20 412e   Quintana, F. A.
+000135a0: 2c20 4a61 7261 2c20 412e 2c20 2620 4861  , Jara, A., & Ha
+000135b0: 6e73 6f6e 2c20 542e 2028 3230 3135 292e  nson, T. (2015).
+000135c0: 2042 6179 6573 6961 6e20 6e6f 6e70 6172   Bayesian nonpar
+000135d0: 616d 6574 7269 6320 6461 7461 0a20 2020  ametric data.   
+000135e0: 2020 2020 2020 2020 616e 616c 7973 6973          analysis
+000135f0: 2e20 4e65 7720 596f 726b 3a20 5370 7269  . New York: Spri
+00013600: 6e67 6572 2e0a 2020 2020 2222 220a 2020  nger..    """.  
+00013610: 2020 7276 5f6f 7020 3d20 7374 6963 6b62    rv_op = stickb
+00013620: 7265 616b 696e 6777 6569 6768 7473 0a0a  reakingweights..
+00013630: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00013640: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
+00013650: 732c 2061 6c70 6861 2c20 4b2c 202a 6172  s, alpha, K, *ar
+00013660: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+00013670: 2020 2020 2020 2061 6c70 6861 203d 2070         alpha = p
+00013680: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00013690: 6162 6c65 2866 6c6f 6174 5828 616c 7068  able(floatX(alph
+000136a0: 6129 290a 2020 2020 2020 2020 4b20 3d20  a)).        K = 
+000136b0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+000136c0: 6961 626c 6528 696e 7458 284b 2929 0a0a  iable(intX(K))..
+000136d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000136e0: 7570 6572 2829 2e64 6973 7428 5b61 6c70  uper().dist([alp
+000136f0: 6861 2c20 4b5d 2c20 2a2a 6b77 6172 6773  ha, K], **kwargs
+00013700: 290a 0a20 2020 2064 6566 206d 6f6d 656e  )..    def momen
+00013710: 7428 7276 2c20 7369 7a65 2c20 616c 7068  t(rv, size, alph
+00013720: 612c 204b 293a 0a20 2020 2020 2020 2061  a, K):.        a
+00013730: 6c70 6861 203d 2061 6c70 6861 5b2e 2e2e  lpha = alpha[...
+00013740: 2c20 6e70 2e6e 6577 6178 6973 5d0a 2020  , np.newaxis].  
+00013750: 2020 2020 2020 6d6f 6d65 6e74 203d 2028        moment = (
+00013760: 616c 7068 6120 2f20 2831 202b 2061 6c70  alpha / (1 + alp
+00013770: 6861 2929 202a 2a20 7074 2e61 7261 6e67  ha)) ** pt.arang
+00013780: 6528 4b29 0a20 2020 2020 2020 206d 6f6d  e(K).        mom
+00013790: 656e 7420 2a3d 2031 202f 2028 3120 2b20  ent *= 1 / (1 + 
+000137a0: 616c 7068 6129 0a20 2020 2020 2020 206d  alpha).        m
+000137b0: 6f6d 656e 7420 3d20 7074 2e63 6f6e 6361  oment = pt.conca
+000137c0: 7465 6e61 7465 285b 6d6f 6d65 6e74 2c20  tenate([moment, 
+000137d0: 2861 6c70 6861 202f 2028 3120 2b20 616c  (alpha / (1 + al
+000137e0: 7068 6129 2920 2a2a 204b 5d2c 2061 7869  pha)) ** K], axi
+000137f0: 733d 2d31 290a 2020 2020 2020 2020 6966  s=-1).        if
+00013800: 206e 6f74 2072 765f 7369 7a65 5f69 735f   not rv_size_is_
+00013810: 6e6f 6e65 2873 697a 6529 3a0a 2020 2020  none(size):.    
+00013820: 2020 2020 2020 2020 6d6f 6d65 6e74 5f73          moment_s
+00013830: 697a 6520 3d20 7074 2e63 6f6e 6361 7465  ize = pt.concate
+00013840: 6e61 7465 280a 2020 2020 2020 2020 2020  nate(.          
+00013850: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00013860: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00013870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013880: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138a0: 4b20 2b20 312c 0a20 2020 2020 2020 2020  K + 1,.         
+000138b0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000138c0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+000138d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000138e0: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
+000138f0: 203d 2070 742e 6675 6c6c 286d 6f6d 656e   = pt.full(momen
+00013900: 745f 7369 7a65 2c20 6d6f 6d65 6e74 290a  t_size, moment).
+00013910: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013920: 6d6f 6d65 6e74 0a0a 2020 2020 6465 6620  moment..    def 
+00013930: 6c6f 6770 2876 616c 7565 2c20 616c 7068  logp(value, alph
+00013940: 612c 204b 293a 0a20 2020 2020 2020 2022  a, K):.        "
+00013950: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+00013960: 6c61 7465 206c 6f67 2d70 726f 6261 6269  late log-probabi
+00013970: 6c69 7479 206f 6620 7468 6520 6469 7374  lity of the dist
+00013980: 7269 6275 7469 6f6e 2069 6e64 7563 6564  ribution induced
+00013990: 2066 726f 6d20 7468 6520 7374 6963 6b2d   from the stick-
+000139a0: 6272 6561 6b69 6e67 2070 726f 6365 7373  breaking process
+000139b0: 0a20 2020 2020 2020 2061 7420 7370 6563  .        at spec
+000139c0: 6966 6965 6420 7661 6c75 652e 0a0a 2020  ified value...  
+000139d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000139e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000139f0: 2d2d 2d0a 2020 2020 2020 2020 7661 6c75  ---.        valu
+00013a00: 653a 206e 756d 6572 6963 0a20 2020 2020  e: numeric.     
+00013a10: 2020 2020 2020 2056 616c 7565 2066 6f72         Value for
+00013a20: 2077 6869 6368 206c 6f67 2d70 726f 6261   which log-proba
+00013a30: 6269 6c69 7479 2069 7320 6361 6c63 756c  bility is calcul
+00013a40: 6174 6564 2e0a 0a20 2020 2020 2020 2052  ated...        R
+00013a50: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00013a60: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+00013a70: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
+00013a80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013a90: 2020 6c6f 6770 203d 202d 7074 2e73 756d    logp = -pt.sum
+00013aa0: 280a 2020 2020 2020 2020 2020 2020 7074  (.            pt
+00013ab0: 2e6c 6f67 280a 2020 2020 2020 2020 2020  .log(.          
+00013ac0: 2020 2020 2020 7074 2e63 756d 7375 6d28        pt.cumsum(
+00013ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ae0: 2020 2020 2076 616c 7565 5b2e 2e2e 2c20       value[..., 
+00013af0: 3a3a 2d31 5d2c 0a20 2020 2020 2020 2020  ::-1],.         
+00013b00: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
+00013b10: 2d31 2c0a 2020 2020 2020 2020 2020 2020  -1,.            
+00013b20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00013b30: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00013b40: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
+00013b50: 2020 290a 2020 2020 2020 2020 6c6f 6770    ).        logp
+00013b60: 202b 3d20 2d4b 202a 2062 6574 616c 6e28   += -K * betaln(
+00013b70: 312c 2061 6c70 6861 290a 2020 2020 2020  1, alpha).      
+00013b80: 2020 6c6f 6770 202b 3d20 616c 7068 6120    logp += alpha 
+00013b90: 2a20 7074 2e6c 6f67 2876 616c 7565 5b2e  * pt.log(value[.
+00013ba0: 2e2e 2c20 2d31 5d29 0a0a 2020 2020 2020  .., -1])..      
+00013bb0: 2020 6c6f 6770 203d 2070 742e 7377 6974    logp = pt.swit
+00013bc0: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
+00013bd0: 7074 2e6f 725f 280a 2020 2020 2020 2020  pt.or_(.        
+00013be0: 2020 2020 2020 2020 7074 2e61 6e79 280a          pt.any(.
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 2020 7074 2e61 6e64 5f28 7074 2e6c      pt.and_(pt.l
+00013c10: 6528 7661 6c75 652c 2030 292c 2070 742e  e(value, 0), pt.
+00013c20: 6765 2876 616c 7565 2c20 3129 292c 0a20  ge(value, 1)),. 
+00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c40: 2020 2061 7869 733d 2d31 2c0a 2020 2020     axis=-1,.    
+00013c50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00013c70: 742e 6f72 5f28 0a20 2020 2020 2020 2020  t.or_(.         
+00013c80: 2020 2020 2020 2020 2020 2070 742e 6269             pt.bi
+00013c90: 7477 6973 655f 6e6f 7428 7074 2e61 6c6c  twise_not(pt.all
+00013ca0: 636c 6f73 6528 7661 6c75 652e 7375 6d28  close(value.sum(
+00013cb0: 2d31 292c 2031 2929 2c0a 2020 2020 2020  -1), 1)),.      
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00013cd0: 2e6e 6571 2876 616c 7565 2e73 6861 7065  .neq(value.shape
+00013ce0: 5b2d 315d 2c20 4b20 2b20 3129 2c0a 2020  [-1], K + 1),.  
+00013cf0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00013d00: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00013d10: 2020 2020 2020 2020 2020 2020 2d6e 702e              -np.
+00013d20: 696e 662c 0a20 2020 2020 2020 2020 2020  inf,.           
+00013d30: 206c 6f67 702c 0a20 2020 2020 2020 2029   logp,.        )
+00013d40: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013d50: 2063 6865 636b 5f70 6172 616d 6574 6572   check_parameter
+00013d60: 7328 0a20 2020 2020 2020 2020 2020 206c  s(.            l
+00013d70: 6f67 702c 0a20 2020 2020 2020 2020 2020  ogp,.           
+00013d80: 2061 6c70 6861 203e 2030 2c0a 2020 2020   alpha > 0,.    
+00013d90: 2020 2020 2020 2020 4b20 3e20 302c 0a20          K > 0,. 
+00013da0: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
+00013db0: 616c 7068 6120 3e20 302c 204b 203e 2030  alpha > 0, K > 0
+00013dc0: 222c 0a20 2020 2020 2020 2029 0a0a 0a63  ",.        )...c
+00013dd0: 6c61 7373 205a 6572 6f53 756d 4e6f 726d  lass ZeroSumNorm
+00013de0: 616c 5256 2853 796d 626f 6c69 6352 616e  alRV(SymbolicRan
+00013df0: 646f 6d56 6172 6961 626c 6529 3a0a 2020  domVariable):.  
+00013e00: 2020 2222 225a 6572 6f53 756d 4e6f 726d    """ZeroSumNorm
+00013e10: 616c 2072 616e 646f 6d20 7661 7269 6162  al random variab
+00013e20: 6c65 2222 220a 0a20 2020 205f 7072 696e  le"""..    _prin
+00013e30: 745f 6e61 6d65 203d 2028 225a 6572 6f53  t_name = ("ZeroS
+00013e40: 756d 4e6f 726d 616c 222c 2022 5c5c 6f70  umNormal", "\\op
+00013e50: 6572 6174 6f72 6e61 6d65 7b5a 6572 6f53  eratorname{ZeroS
+00013e60: 756d 4e6f 726d 616c 7d22 290a 2020 2020  umNormal}").    
+00013e70: 6465 6661 756c 745f 6f75 7470 7574 203d  default_output =
+00013e80: 2030 0a0a 0a63 6c61 7373 205a 6572 6f53   0...class ZeroS
+00013e90: 756d 4e6f 726d 616c 2844 6973 7472 6962  umNormal(Distrib
+00013ea0: 7574 696f 6e29 3a0a 2020 2020 7222 2222  ution):.    r"""
+00013eb0: 0a20 2020 205a 6572 6f53 756d 4e6f 726d  .    ZeroSumNorm
+00013ec0: 616c 2064 6973 7472 6962 7574 696f 6e2c  al distribution,
+00013ed0: 2069 2e65 204e 6f72 6d61 6c20 6469 7374   i.e Normal dist
+00013ee0: 7269 6275 7469 6f6e 2077 6865 7265 206f  ribution where o
+00013ef0: 6e65 206f 720a 2020 2020 7365 7665 7261  ne or.    severa
+00013f00: 6c20 6178 6573 2061 7265 2063 6f6e 7374  l axes are const
+00013f10: 7261 696e 6564 2074 6f20 7375 6d20 746f  rained to sum to
+00013f20: 207a 6572 6f2e 0a20 2020 2042 7920 6465   zero..    By de
+00013f30: 6661 756c 742c 2074 6865 206c 6173 7420  fault, the last 
+00013f40: 6178 6973 2069 7320 636f 6e73 7472 6169  axis is constrai
+00013f50: 6e65 6420 746f 2073 756d 2074 6f20 7a65  ned to sum to ze
+00013f60: 726f 2e0a 2020 2020 5365 6520 606e 5f7a  ro..    See `n_z
+00013f70: 6572 6f73 756d 5f61 7865 7360 206b 7761  erosum_axes` kwa
+00013f80: 7267 2066 6f72 206d 6f72 6520 6465 7461  rg for more deta
+00013f90: 696c 732e 0a0a 2020 2020 2e2e 206d 6174  ils...    .. mat
+00013fa0: 683a 3a0a 0a20 2020 2020 2020 205c 6265  h::..        \be
+00013fb0: 6769 6e7b 616c 6967 6e2a 7d0a 2020 2020  gin{align*}.    
+00013fc0: 2020 2020 2020 2020 5a53 4e28 5c73 6967          ZSN(\sig
+00013fd0: 6d61 2920 3d20 4e20 5c42 6967 2820 302c  ma) = N \Big( 0,
+00013fe0: 205c 7369 676d 615e 3220 2849 202d 205c   \sigma^2 (I - \
+00013ff0: 7466 7261 637b 317d 7b6e 7d4a 2920 5c42  tfrac{1}{n}J) \B
+00014000: 6967 2920 5c5c 0a20 2020 2020 2020 2020  ig) \\.         
+00014010: 2020 205c 7465 7874 7b77 6865 7265 7d20     \text{where} 
+00014020: 5c20 7e20 4a5f 7b69 6a7d 203d 2031 205c  \ ~ J_{ij} = 1 \
+00014030: 207e 205c 7465 7874 7b61 6e64 7d20 5c5c   ~ \text{and} \\
+00014040: 0a20 2020 2020 2020 2020 2020 206e 203d  .            n =
+00014050: 205c 7465 7874 7b6e 6272 206f 6620 7a65   \text{nbr of ze
+00014060: 726f 2d73 756d 2061 7865 737d 0a20 2020  ro-sum axes}.   
+00014070: 2020 2020 205c 656e 647b 616c 6967 6e2a       \end{align*
+00014080: 7d0a 0a20 2020 2050 6172 616d 6574 6572  }..    Parameter
+00014090: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+000140a0: 0a20 2020 2073 6967 6d61 203a 2074 656e  .    sigma : ten
+000140b0: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+000140c0: 740a 2020 2020 2020 2020 5363 616c 6520  t.        Scale 
+000140d0: 7061 7261 6d65 7465 7220 2873 6967 6d61  parameter (sigma
+000140e0: 203e 2030 292e 0a20 2020 2020 2020 2049   > 0)..        I
+000140f0: 7427 7320 6163 7475 616c 6c79 2074 6865  t's actually the
+00014100: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00014110: 696f 6e20 6f66 2074 6865 2075 6e64 6572  ion of the under
+00014120: 6c79 696e 672c 2075 6e63 6f6e 7374 7261  lying, unconstra
+00014130: 696e 6564 204e 6f72 6d61 6c20 6469 7374  ined Normal dist
+00014140: 7269 6275 7469 6f6e 2e0a 2020 2020 2020  ribution..      
+00014150: 2020 4465 6661 756c 7473 2074 6f20 3120    Defaults to 1 
+00014160: 6966 206e 6f74 2073 7065 6369 6669 6564  if not specified
+00014170: 2e0a 2020 2020 2020 2020 466f 7220 6e6f  ..        For no
+00014180: 772c 2060 6073 6967 6d61 6060 2068 6173  w, ``sigma`` has
+00014190: 2074 6f20 6265 2061 2073 6361 6c61 722c   to be a scalar,
+000141a0: 2074 6f20 656e 7375 7265 2074 6865 207a   to ensure the z
+000141b0: 6572 6f2d 7375 6d20 636f 6e73 7472 6169  ero-sum constrai
+000141c0: 6e74 2e0a 2020 2020 6e5f 7a65 726f 7375  nt..    n_zerosu
+000141d0: 6d5f 6178 6573 3a20 696e 742c 2064 6566  m_axes: int, def
+000141e0: 6175 6c74 7320 746f 2031 0a20 2020 2020  aults to 1.     
+000141f0: 2020 204e 756d 6265 7220 6f66 2061 7865     Number of axe
+00014200: 7320 616c 6f6e 6720 7768 6963 6820 7468  s along which th
+00014210: 6520 7a65 726f 2d73 756d 2063 6f6e 7374  e zero-sum const
+00014220: 7261 696e 7420 6973 2065 6e66 6f72 6365  raint is enforce
+00014230: 642c 2073 7461 7274 696e 6720 6672 6f6d  d, starting from
+00014240: 2074 6865 2072 6967 6874 6d6f 7374 2070   the rightmost p
+00014250: 6f73 6974 696f 6e2e 0a20 2020 2020 2020  osition..       
+00014260: 2044 6566 6175 6c74 7320 746f 2031 2c20   Defaults to 1, 
+00014270: 692e 6520 7468 6520 7269 6768 746d 6f73  i.e the rightmos
+00014280: 7420 6178 6973 2e0a 2020 2020 7a65 726f  t axis..    zero
+00014290: 7375 6d5f 6178 6573 3a20 696e 742c 2064  sum_axes: int, d
+000142a0: 6570 7265 6361 7465 6420 706c 6561 7365  eprecated please
+000142b0: 2075 7365 206e 5f7a 6572 6f73 756d 5f61   use n_zerosum_a
+000142c0: 7865 7320 6173 2069 7473 2073 7563 6365  xes as its succe
+000142d0: 7373 6f72 0a20 2020 2064 696d 733a 2073  ssor.    dims: s
+000142e0: 6571 7565 6e63 6520 6f66 2073 7472 696e  equence of strin
+000142f0: 6773 2c20 6f70 7469 6f6e 616c 0a20 2020  gs, optional.   
+00014300: 2020 2020 2044 696d 656e 7369 6f6e 206e       Dimension n
+00014310: 616d 6573 206f 6620 7468 6520 6469 7374  ames of the dist
+00014320: 7269 6275 7469 6f6e 2e20 576f 726b 7320  ribution. Works 
+00014330: 7468 6520 7361 6d65 2061 7320 666f 7220  the same as for 
+00014340: 6f74 6865 7220 5079 4d43 2064 6973 7472  other PyMC distr
+00014350: 6962 7574 696f 6e73 2e0a 2020 2020 2020  ibutions..      
+00014360: 2020 4e65 6365 7373 6172 7920 6966 2060    Necessary if `
+00014370: 6073 6861 7065 6060 2069 7320 6e6f 7420  `shape`` is not 
+00014380: 7061 7373 6564 2e0a 2020 2020 7368 6170  passed..    shap
+00014390: 653a 2074 7570 6c65 206f 6620 696e 7465  e: tuple of inte
+000143a0: 6765 7273 2c20 6f70 7469 6f6e 616c 0a20  gers, optional. 
+000143b0: 2020 2020 2020 2053 6861 7065 206f 6620         Shape of 
+000143c0: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+000143d0: 2e20 576f 726b 7320 7468 6520 7361 6d65  . Works the same
+000143e0: 2061 7320 666f 7220 6f74 6865 7220 5079   as for other Py
+000143f0: 4d43 2064 6973 7472 6962 7574 696f 6e73  MC distributions
+00014400: 2e0a 2020 2020 2020 2020 4e65 6365 7373  ..        Necess
+00014410: 6172 7920 6966 2060 6064 696d 7360 6020  ary if ``dims`` 
+00014420: 6f72 2060 606f 6273 6572 7665 6460 6020  or ``observed`` 
+00014430: 6973 206e 6f74 2070 6173 7365 642e 0a0a  is not passed...
+00014440: 2020 2020 5761 726e 696e 6773 0a20 2020      Warnings.   
+00014450: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 6060   --------.    ``
+00014460: 7369 676d 6160 6020 6861 7320 746f 2062  sigma`` has to b
+00014470: 6520 6120 7363 616c 6172 2c20 746f 2065  e a scalar, to e
+00014480: 6e73 7572 6520 7468 6520 7a65 726f 2d73  nsure the zero-s
+00014490: 756d 2063 6f6e 7374 7261 696e 742e 0a20  um constraint.. 
+000144a0: 2020 2054 6865 2061 6269 6c69 7479 2074     The ability t
+000144b0: 6f20 7370 6563 6966 7920 6120 7665 6374  o specify a vect
+000144c0: 6f72 206f 6620 6060 7369 676d 6160 6020  or of ``sigma`` 
+000144d0: 6d61 7920 6265 2061 6464 6564 2069 6e20  may be added in 
+000144e0: 6675 7475 7265 2076 6572 7369 6f6e 732e  future versions.
+000144f0: 0a0a 2020 2020 6060 6e5f 7a65 726f 7375  ..    ``n_zerosu
+00014500: 6d5f 6178 6573 6060 2068 6173 2074 6f20  m_axes`` has to 
+00014510: 6265 203e 2030 2e20 4966 2079 6f75 2077  be > 0. If you w
+00014520: 616e 7420 7468 6520 6265 6861 7669 6f72  ant the behavior
+00014530: 206f 6620 6060 6e5f 7a65 726f 7375 6d5f   of ``n_zerosum_
+00014540: 6178 6573 203d 2030 6060 2c0a 2020 2020  axes = 0``,.    
+00014550: 6a75 7374 2075 7365 2060 6070 6d2e 4e6f  just use ``pm.No
+00014560: 726d 616c 6060 2e0a 0a20 2020 2045 7861  rmal``...    Exa
+00014570: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00014580: 2d2d 0a20 2020 2044 6566 696e 6520 6120  --.    Define a 
+00014590: 605a 6572 6f53 756d 4e6f 726d 616c 6020  `ZeroSumNormal` 
+000145a0: 7661 7269 6162 6c65 2c20 7769 7468 2060  variable, with `
+000145b0: 7369 676d 613d 3160 2061 6e64 0a20 2020  sigma=1` and.   
+000145c0: 2060 6e5f 7a65 726f 7375 6d5f 6178 6573   `n_zerosum_axes
+000145d0: 3d31 6020 2062 7920 6465 6661 756c 743a  =1`  by default:
+000145e0: 3a0a 0a20 2020 2020 2020 2043 4f4f 5244  :..        COORD
+000145f0: 5320 3d20 7b0a 2020 2020 2020 2020 2020  S = {.          
+00014600: 2020 2272 6567 696f 6e73 223a 205b 2261    "regions": ["a
+00014610: 222c 2022 6222 2c20 2263 225d 2c0a 2020  ", "b", "c"],.  
+00014620: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
+00014630: 7273 223a 205b 2279 6573 222c 2022 6e6f  rs": ["yes", "no
+00014640: 222c 2022 7768 6174 6576 6572 222c 2022  ", "whatever", "
+00014650: 646f 6e27 7420 756e 6465 7273 7461 6e64  don't understand
+00014660: 2071 7565 7374 696f 6e22 5d2c 0a20 2020   question"],.   
+00014670: 2020 2020 207d 0a20 2020 2020 2020 2077       }.        w
+00014680: 6974 6820 706d 2e4d 6f64 656c 2863 6f6f  ith pm.Model(coo
+00014690: 7264 733d 434f 4f52 4453 2920 6173 206d  rds=COORDS) as m
+000146a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000146b0: 7468 6520 7a65 726f 2073 756d 2061 7869  the zero sum axi
+000146c0: 7320 7769 6c6c 2062 6520 2761 6e73 7765  s will be 'answe
+000146d0: 7273 270a 2020 2020 2020 2020 2020 2020  rs'.            
+000146e0: 7620 3d20 706d 2e5a 6572 6f53 756d 4e6f  v = pm.ZeroSumNo
+000146f0: 726d 616c 2822 7622 2c20 6469 6d73 3d28  rmal("v", dims=(
+00014700: 2272 6567 696f 6e73 222c 2022 616e 7377  "regions", "answ
+00014710: 6572 7322 2929 0a0a 2020 2020 2020 2020  ers"))..        
+00014720: 7769 7468 2070 6d2e 4d6f 6465 6c28 636f  with pm.Model(co
+00014730: 6f72 6473 3d43 4f4f 5244 5329 2061 7320  ords=COORDS) as 
+00014740: 6d3a 0a20 2020 2020 2020 2020 2020 2023  m:.            #
+00014750: 2074 6865 207a 6572 6f20 7375 6d20 6178   the zero sum ax
+00014760: 6573 2077 696c 6c20 6265 2027 616e 7377  es will be 'answ
+00014770: 6572 7327 2061 6e64 2027 7265 6769 6f6e  ers' and 'region
+00014780: 7327 0a20 2020 2020 2020 2020 2020 2076  s'.            v
+00014790: 203d 2070 6d2e 5a65 726f 5375 6d4e 6f72   = pm.ZeroSumNor
+000147a0: 6d61 6c28 2276 222c 2064 696d 733d 2822  mal("v", dims=("
+000147b0: 7265 6769 6f6e 7322 2c20 2261 6e73 7765  regions", "answe
+000147c0: 7273 2229 2c20 6e5f 7a65 726f 7375 6d5f  rs"), n_zerosum_
+000147d0: 6178 6573 3d32 290a 0a20 2020 2020 2020  axes=2)..       
+000147e0: 2077 6974 6820 706d 2e4d 6f64 656c 2863   with pm.Model(c
+000147f0: 6f6f 7264 733d 434f 4f52 4453 2920 6173  oords=COORDS) as
+00014800: 206d 3a0a 2020 2020 2020 2020 2020 2020   m:.            
+00014810: 2320 7468 6520 7a65 726f 2073 756d 2061  # the zero sum a
+00014820: 7865 7320 7769 6c6c 2062 6520 7468 6520  xes will be the 
+00014830: 6c61 7374 2074 776f 0a20 2020 2020 2020  last two.       
+00014840: 2020 2020 2076 203d 2070 6d2e 5a65 726f       v = pm.Zero
+00014850: 5375 6d4e 6f72 6d61 6c28 2276 222c 2073  SumNormal("v", s
+00014860: 6861 7065 3d28 332c 2034 2c20 3529 2c20  hape=(3, 4, 5), 
+00014870: 6e5f 7a65 726f 7375 6d5f 6178 6573 3d32  n_zerosum_axes=2
+00014880: 290a 2020 2020 2222 220a 2020 2020 7276  ).    """.    rv
+00014890: 5f74 7970 6520 3d20 5a65 726f 5375 6d4e  _type = ZeroSumN
+000148a0: 6f72 6d61 6c52 560a 0a20 2020 2064 6566  ormalRV..    def
+000148b0: 205f 5f6e 6577 5f5f 280a 2020 2020 2020   __new__(.      
+000148c0: 2020 636c 732c 202a 6172 6773 2c20 7a65    cls, *args, ze
+000148d0: 726f 7375 6d5f 6178 6573 3d4e 6f6e 652c  rosum_axes=None,
+000148e0: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
+000148f0: 4e6f 6e65 2c20 7375 7070 6f72 745f 7368  None, support_sh
+00014900: 6170 653d 4e6f 6e65 2c20 6469 6d73 3d4e  ape=None, dims=N
+00014910: 6f6e 652c 202a 2a6b 7761 7267 730a 2020  one, **kwargs.  
+00014920: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
+00014930: 7a65 726f 7375 6d5f 6178 6573 2069 7320  zerosum_axes is 
+00014940: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014950: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
+00014960: 6178 6573 203d 207a 6572 6f73 756d 5f61  axes = zerosum_a
+00014970: 7865 730a 2020 2020 2020 2020 2020 2020  xes.            
+00014980: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+00014990: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000149a0: 5468 6520 277a 6572 6f73 756d 5f61 7865  The 'zerosum_axe
+000149b0: 7327 2070 6172 616d 6574 6572 2069 7320  s' parameter is 
+000149c0: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
+000149d0: 276e 5f7a 6572 6f73 756d 5f61 7865 7327  'n_zerosum_axes'
+000149e0: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
+000149f0: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
+00014a00: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
+00014a10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00014a20: 2020 2020 2020 6966 2064 696d 7320 6973        if dims is
+00014a30: 206e 6f74 204e 6f6e 6520 6f72 206b 7761   not None or kwa
+00014a40: 7267 732e 6765 7428 226f 6273 6572 7665  rgs.get("observe
+00014a50: 6422 2920 6973 206e 6f74 204e 6f6e 653a  d") is not None:
+00014a60: 0a20 2020 2020 2020 2020 2020 206e 5f7a  .            n_z
+00014a70: 6572 6f73 756d 5f61 7865 7320 3d20 636c  erosum_axes = cl
+00014a80: 732e 6368 6563 6b5f 7a65 726f 7375 6d5f  s.check_zerosum_
+00014a90: 6178 6573 286e 5f7a 6572 6f73 756d 5f61  axes(n_zerosum_a
+00014aa0: 7865 7329 0a0a 2020 2020 2020 2020 2020  xes)..          
+00014ab0: 2020 7375 7070 6f72 745f 7368 6170 6520    support_shape 
+00014ac0: 3d20 6765 745f 7375 7070 6f72 745f 7368  = get_support_sh
+00014ad0: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
+00014ae0: 2020 2020 2073 7570 706f 7274 5f73 6861       support_sha
+00014af0: 7065 3d73 7570 706f 7274 5f73 6861 7065  pe=support_shape
+00014b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014b10: 2020 7368 6170 653d 4e6f 6e65 2c20 2023    shape=None,  #
+00014b20: 2053 6861 7065 2077 696c 6c20 6265 2063   Shape will be c
+00014b30: 6865 636b 6564 2069 6e20 6063 6c73 2e64  hecked in `cls.d
+00014b40: 6973 7460 0a20 2020 2020 2020 2020 2020  ist`.           
+00014b50: 2020 2020 2064 696d 733d 6469 6d73 2c0a       dims=dims,.
+00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b70: 6f62 7365 7276 6564 3d6b 7761 7267 732e  observed=kwargs.
+00014b80: 6765 7428 226f 6273 6572 7665 6422 2c20  get("observed", 
+00014b90: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
+00014ba0: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
+00014bb0: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
+00014bc0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00014bd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00014be0: 7570 6572 2829 2e5f 5f6e 6577 5f5f 280a  uper().__new__(.
+00014bf0: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
+00014c00: 0a20 2020 2020 2020 2020 2020 202a 6172  .            *ar
+00014c10: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00014c20: 6e5f 7a65 726f 7375 6d5f 6178 6573 3d6e  n_zerosum_axes=n
+00014c30: 5f7a 6572 6f73 756d 5f61 7865 732c 0a20  _zerosum_axes,. 
+00014c40: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00014c50: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
+00014c60: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
+00014c70: 2020 2020 6469 6d73 3d64 696d 732c 0a20      dims=dims,. 
+00014c80: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00014c90: 7267 732c 0a20 2020 2020 2020 2029 0a0a  rgs,.        )..
+00014ca0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00014cb0: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
+00014cc0: 732c 2073 6967 6d61 3d31 2c20 6e5f 7a65  s, sigma=1, n_ze
+00014cd0: 726f 7375 6d5f 6178 6573 3d4e 6f6e 652c  rosum_axes=None,
+00014ce0: 2073 7570 706f 7274 5f73 6861 7065 3d4e   support_shape=N
+00014cf0: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
+00014d00: 2020 2020 2020 2020 6e5f 7a65 726f 7375          n_zerosu
+00014d10: 6d5f 6178 6573 203d 2063 6c73 2e63 6865  m_axes = cls.che
+00014d20: 636b 5f7a 6572 6f73 756d 5f61 7865 7328  ck_zerosum_axes(
+00014d30: 6e5f 7a65 726f 7375 6d5f 6178 6573 290a  n_zerosum_axes).
+00014d40: 0a20 2020 2020 2020 2073 6967 6d61 203d  .        sigma =
+00014d50: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+00014d60: 7269 6162 6c65 2866 6c6f 6174 5828 7369  riable(floatX(si
+00014d70: 676d 6129 290a 2020 2020 2020 2020 6966  gma)).        if
+00014d80: 2073 6967 6d61 2e6e 6469 6d20 3e20 303a   sigma.ndim > 0:
+00014d90: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00014da0: 7365 2056 616c 7565 4572 726f 7228 2273  se ValueError("s
+00014db0: 6967 6d61 2068 6173 2074 6f20 6265 2061  igma has to be a
+00014dc0: 2073 6361 6c61 7222 290a 0a20 2020 2020   scalar")..     
+00014dd0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+00014de0: 203d 2067 6574 5f73 7570 706f 7274 5f73   = get_support_s
+00014df0: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
+00014e00: 2020 7375 7070 6f72 745f 7368 6170 653d    support_shape=
+00014e10: 7375 7070 6f72 745f 7368 6170 652c 0a20  support_shape,. 
+00014e20: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00014e30: 3d6b 7761 7267 732e 6765 7428 2273 6861  =kwargs.get("sha
+00014e40: 7065 2229 2c0a 2020 2020 2020 2020 2020  pe"),.          
+00014e50: 2020 6e64 696d 5f73 7570 703d 6e5f 7a65    ndim_supp=n_ze
+00014e60: 726f 7375 6d5f 6178 6573 2c0a 2020 2020  rosum_axes,.    
+00014e70: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+00014e80: 6620 7375 7070 6f72 745f 7368 6170 6520  f support_shape 
+00014e90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00014ea0: 2020 2020 2069 6620 6e5f 7a65 726f 7375       if n_zerosu
+00014eb0: 6d5f 6178 6573 203e 2030 3a0a 2020 2020  m_axes > 0:.    
+00014ec0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00014ed0: 6520 5661 6c75 6545 7272 6f72 2822 596f  e ValueError("Yo
+00014ee0: 7520 6d75 7374 2073 7065 6369 6679 2064  u must specify d
+00014ef0: 696d 732c 2073 6861 7065 206f 7220 7375  ims, shape or su
+00014f00: 7070 6f72 745f 7368 6170 6520 7061 7261  pport_shape para
+00014f10: 6d65 7465 7222 290a 2020 2020 2020 2020  meter").        
+00014f20: 2020 2020 2320 544f 444f 3a20 6564 6765      # TODO: edge
+00014f30: 2d63 6173 6520 646f 6573 6e27 7420 776f  -case doesn't wo
+00014f40: 726b 2066 6f72 206e 6f77 2c20 6265 6361  rk for now, beca
+00014f50: 7573 6520 7074 2e73 7461 636b 2069 6e20  use pt.stack in 
+00014f60: 6765 745f 7375 7070 6f72 745f 7368 6170  get_support_shap
+00014f70: 6520 6661 696c 730a 2020 2020 2020 2020  e fails.        
+00014f80: 2020 2020 2320 656c 7365 3a0a 2020 2020      # else:.    
+00014f90: 2020 2020 2020 2020 2320 2020 2020 7375          #     su
+00014fa0: 7070 6f72 745f 7368 6170 6520 3d20 2829  pport_shape = ()
+00014fb0: 2023 2062 6563 6175 7365 2069 7427 7320   # because it's 
+00014fc0: 6a75 7374 2061 204e 6f72 6d61 6c20 696e  just a Normal in
+00014fd0: 2074 6861 7420 6361 7365 0a20 2020 2020   that case.     
+00014fe0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
+00014ff0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+00015000: 7661 7269 6162 6c65 2869 6e74 5828 7375  variable(intX(su
+00015010: 7070 6f72 745f 7368 6170 6529 290a 0a20  pport_shape)).. 
+00015020: 2020 2020 2020 2061 7373 6572 7420 6e5f         assert n_
+00015030: 7a65 726f 7375 6d5f 6178 6573 203d 3d20  zerosum_axes == 
+00015040: 7074 2e67 6574 5f76 6563 746f 725f 6c65  pt.get_vector_le
+00015050: 6e67 7468 280a 2020 2020 2020 2020 2020  ngth(.          
+00015060: 2020 7375 7070 6f72 745f 7368 6170 650a    support_shape.
+00015070: 2020 2020 2020 2020 292c 2022 7375 7070          ), "supp
+00015080: 6f72 745f 7368 6170 6520 6861 7320 746f  ort_shape has to
+00015090: 2062 6520 6173 206c 6f6e 6720 6173 206e   be as long as n
+000150a0: 5f7a 6572 6f73 756d 5f61 7865 7322 0a0a  _zerosum_axes"..
+000150b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000150c0: 7570 6572 2829 2e64 6973 7428 0a20 2020  uper().dist(.   
+000150d0: 2020 2020 2020 2020 205b 7369 676d 615d           [sigma]
+000150e0: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
+000150f0: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
+00015100: 2073 7570 706f 7274 5f73 6861 7065 3d73   support_shape=s
+00015110: 7570 706f 7274 5f73 6861 7065 2c20 2a2a  upport_shape, **
+00015120: 6b77 6172 6773 0a20 2020 2020 2020 2029  kwargs.        )
+00015130: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00015140: 6f64 0a20 2020 2064 6566 2063 6865 636b  od.    def check
+00015150: 5f7a 6572 6f73 756d 5f61 7865 7328 636c  _zerosum_axes(cl
+00015160: 732c 206e 5f7a 6572 6f73 756d 5f61 7865  s, n_zerosum_axe
+00015170: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
+00015180: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00015190: 2020 6966 206e 5f7a 6572 6f73 756d 5f61    if n_zerosum_a
+000151a0: 7865 7320 6973 204e 6f6e 653a 0a20 2020  xes is None:.   
+000151b0: 2020 2020 2020 2020 206e 5f7a 6572 6f73           n_zeros
+000151c0: 756d 5f61 7865 7320 3d20 310a 2020 2020  um_axes = 1.    
+000151d0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+000151e0: 7461 6e63 6528 6e5f 7a65 726f 7375 6d5f  tance(n_zerosum_
+000151f0: 6178 6573 2c20 696e 7429 3a0a 2020 2020  axes, int):.    
+00015200: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00015210: 7065 4572 726f 7228 226e 5f7a 6572 6f73  peError("n_zeros
+00015220: 756d 5f61 7865 7320 6861 7320 746f 2062  um_axes has to b
+00015230: 6520 616e 2069 6e74 6567 6572 2229 0a20  e an integer"). 
+00015240: 2020 2020 2020 2069 6620 6e6f 7420 6e5f         if not n_
+00015250: 7a65 726f 7375 6d5f 6178 6573 203e 2030  zerosum_axes > 0
+00015260: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00015270: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00015280: 6e5f 7a65 726f 7375 6d5f 6178 6573 2068  n_zerosum_axes h
+00015290: 6173 2074 6f20 6265 203e 2030 2229 0a20  as to be > 0"). 
+000152a0: 2020 2020 2020 2072 6574 7572 6e20 6e5f         return n_
+000152b0: 7a65 726f 7375 6d5f 6178 6573 0a0a 2020  zerosum_axes..  
+000152c0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000152d0: 2020 2064 6566 2072 765f 6f70 2863 6c73     def rv_op(cls
+000152e0: 2c20 7369 676d 612c 206e 5f7a 6572 6f73  , sigma, n_zeros
+000152f0: 756d 5f61 7865 732c 2073 7570 706f 7274  um_axes, support
+00015300: 5f73 6861 7065 2c20 7369 7a65 3d4e 6f6e  _shape, size=Non
+00015310: 6529 3a0a 2020 2020 2020 2020 7368 6170  e):.        shap
+00015320: 6520 3d20 746f 5f74 7570 6c65 2873 697a  e = to_tuple(siz
+00015330: 6529 202b 2074 7570 6c65 2873 7570 706f  e) + tuple(suppo
+00015340: 7274 5f73 6861 7065 290a 2020 2020 2020  rt_shape).      
+00015350: 2020 6e6f 726d 616c 5f64 6973 7420 3d20    normal_dist = 
+00015360: 706d 2e4e 6f72 6d61 6c2e 6469 7374 2873  pm.Normal.dist(s
+00015370: 6967 6d61 3d73 6967 6d61 2c20 7368 6170  igma=sigma, shap
+00015380: 653d 7368 6170 6529 0a0a 2020 2020 2020  e=shape)..      
+00015390: 2020 6966 206e 5f7a 6572 6f73 756d 5f61    if n_zerosum_a
+000153a0: 7865 7320 3e20 6e6f 726d 616c 5f64 6973  xes > normal_dis
+000153b0: 742e 6e64 696d 3a0a 2020 2020 2020 2020  t.ndim:.        
+000153c0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000153d0: 7272 6f72 2822 5368 6170 6520 6f66 2064  rror("Shape of d
+000153e0: 6973 7472 6962 7574 696f 6e20 6973 2074  istribution is t
+000153f0: 6f6f 2073 6d61 6c6c 2066 6f72 2074 6865  oo small for the
+00015400: 206e 756d 6265 7220 6f66 207a 6572 6f73   number of zeros
+00015410: 756d 2061 7865 7322 290a 0a20 2020 2020  um axes")..     
+00015420: 2020 206e 6f72 6d61 6c5f 6469 7374 5f2c     normal_dist_,
+00015430: 2073 6967 6d61 5f2c 2073 7570 706f 7274   sigma_, support
+00015440: 5f73 6861 7065 5f20 3d20 280a 2020 2020  _shape_ = (.    
+00015450: 2020 2020 2020 2020 6e6f 726d 616c 5f64          normal_d
+00015460: 6973 742e 7479 7065 2829 2c0a 2020 2020  ist.type(),.    
+00015470: 2020 2020 2020 2020 7369 676d 612e 7479          sigma.ty
+00015480: 7065 2829 2c0a 2020 2020 2020 2020 2020  pe(),.          
+00015490: 2020 7375 7070 6f72 745f 7368 6170 652e    support_shape.
+000154a0: 7479 7065 2829 2c0a 2020 2020 2020 2020  type(),.        
+000154b0: 290a 0a20 2020 2020 2020 2023 205a 6572  )..        # Zer
+000154c0: 6f73 756d 2d6e 6f72 6d61 6c69 6e67 2069  osum-normaling i
+000154d0: 7320 6163 6869 6576 6564 2062 7920 7375  s achieved by su
+000154e0: 6274 7261 6374 696e 6720 7468 6520 6d65  btracting the me
+000154f0: 616e 2061 6c6f 6e67 2074 6865 2067 6976  an along the giv
+00015500: 656e 206e 5f7a 6572 6f73 756d 5f61 7865  en n_zerosum_axe
+00015510: 730a 2020 2020 2020 2020 7a65 726f 7375  s.        zerosu
+00015520: 6d5f 7276 5f20 3d20 6e6f 726d 616c 5f64  m_rv_ = normal_d
+00015530: 6973 745f 0a20 2020 2020 2020 2066 6f72  ist_.        for
+00015540: 2061 7869 7320 696e 2072 616e 6765 286e   axis in range(n
+00015550: 5f7a 6572 6f73 756d 5f61 7865 7329 3a0a  _zerosum_axes):.
+00015560: 2020 2020 2020 2020 2020 2020 7a65 726f              zero
+00015570: 7375 6d5f 7276 5f20 2d3d 207a 6572 6f73  sum_rv_ -= zeros
+00015580: 756d 5f72 765f 2e6d 6561 6e28 6178 6973  um_rv_.mean(axis
+00015590: 3d2d 6178 6973 202d 2031 2c20 6b65 6570  =-axis - 1, keep
+000155a0: 6469 6d73 3d54 7275 6529 0a0a 2020 2020  dims=True)..    
+000155b0: 2020 2020 7265 7475 726e 205a 6572 6f53      return ZeroS
+000155c0: 756d 4e6f 726d 616c 5256 280a 2020 2020  umNormalRV(.    
+000155d0: 2020 2020 2020 2020 696e 7075 7473 3d5b          inputs=[
+000155e0: 6e6f 726d 616c 5f64 6973 745f 2c20 7369  normal_dist_, si
+000155f0: 676d 615f 2c20 7375 7070 6f72 745f 7368  gma_, support_sh
+00015600: 6170 655f 5d2c 0a20 2020 2020 2020 2020  ape_],.         
+00015610: 2020 206f 7574 7075 7473 3d5b 7a65 726f     outputs=[zero
+00015620: 7375 6d5f 7276 5f2c 2073 7570 706f 7274  sum_rv_, support
+00015630: 5f73 6861 7065 5f5d 2c0a 2020 2020 2020  _shape_],.      
+00015640: 2020 2020 2020 6e64 696d 5f73 7570 703d        ndim_supp=
+00015650: 6e5f 7a65 726f 7375 6d5f 6178 6573 2c0a  n_zerosum_axes,.
+00015660: 2020 2020 2020 2020 2928 6e6f 726d 616c          )(normal
+00015670: 5f64 6973 742c 2073 6967 6d61 2c20 7375  _dist, sigma, su
+00015680: 7070 6f72 745f 7368 6170 6529 0a0a 0a40  pport_shape)...@
+00015690: 5f63 6861 6e67 655f 6469 7374 5f73 697a  _change_dist_siz
+000156a0: 652e 7265 6769 7374 6572 285a 6572 6f53  e.register(ZeroS
+000156b0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
+000156c0: 6368 616e 6765 5f7a 6572 6f73 756d 5f73  change_zerosum_s
+000156d0: 697a 6528 6f70 2c20 6e6f 726d 616c 5f64  ize(op, normal_d
+000156e0: 6973 742c 206e 6577 5f73 697a 652c 2065  ist, new_size, e
+000156f0: 7870 616e 643d 4661 6c73 6529 3a0a 2020  xpand=False):.  
+00015700: 2020 6e6f 726d 616c 5f64 6973 742c 2073    normal_dist, s
+00015710: 6967 6d61 2c20 7375 7070 6f72 745f 7368  igma, support_sh
+00015720: 6170 6520 3d20 6e6f 726d 616c 5f64 6973  ape = normal_dis
+00015730: 742e 6f77 6e65 722e 696e 7075 7473 0a0a  t.owner.inputs..
+00015740: 2020 2020 6966 2065 7870 616e 643a 0a20      if expand:. 
+00015750: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
+00015760: 7368 6170 6520 3d20 7475 706c 6528 6e6f  shape = tuple(no
+00015770: 726d 616c 5f64 6973 742e 7368 6170 6529  rmal_dist.shape)
+00015780: 0a20 2020 2020 2020 206f 6c64 5f73 697a  .        old_siz
+00015790: 6520 3d20 6f72 6967 696e 616c 5f73 6861  e = original_sha
+000157a0: 7065 5b3a 206c 656e 286f 7269 6769 6e61  pe[: len(origina
+000157b0: 6c5f 7368 6170 6529 202d 206f 702e 6e64  l_shape) - op.nd
+000157c0: 696d 5f73 7570 705d 0a20 2020 2020 2020  im_supp].       
+000157d0: 206e 6577 5f73 697a 6520 3d20 7475 706c   new_size = tupl
+000157e0: 6528 6e65 775f 7369 7a65 2920 2b20 6f6c  e(new_size) + ol
+000157f0: 645f 7369 7a65 0a0a 2020 2020 7265 7475  d_size..    retu
+00015800: 726e 205a 6572 6f53 756d 4e6f 726d 616c  rn ZeroSumNormal
+00015810: 2e72 765f 6f70 280a 2020 2020 2020 2020  .rv_op(.        
+00015820: 7369 676d 613d 7369 676d 612c 206e 5f7a  sigma=sigma, n_z
+00015830: 6572 6f73 756d 5f61 7865 733d 6f70 2e6e  erosum_axes=op.n
+00015840: 6469 6d5f 7375 7070 2c20 7375 7070 6f72  dim_supp, suppor
+00015850: 745f 7368 6170 653d 7375 7070 6f72 745f  t_shape=support_
+00015860: 7368 6170 652c 2073 697a 653d 6e65 775f  shape, size=new_
+00015870: 7369 7a65 0a20 2020 2029 0a0a 0a40 5f6d  size.    )...@_m
+00015880: 6f6d 656e 742e 7265 6769 7374 6572 285a  oment.register(Z
+00015890: 6572 6f53 756d 4e6f 726d 616c 5256 290a  eroSumNormalRV).
+000158a0: 6465 6620 7a65 726f 7375 6d6e 6f72 6d61  def zerosumnorma
+000158b0: 6c5f 6d6f 6d65 6e74 286f 702c 2072 762c  l_moment(op, rv,
+000158c0: 202a 7276 5f69 6e70 7574 7329 3a0a 2020   *rv_inputs):.  
+000158d0: 2020 7265 7475 726e 2070 742e 7a65 726f    return pt.zero
+000158e0: 735f 6c69 6b65 2872 7629 0a0a 0a40 5f64  s_like(rv)...@_d
+000158f0: 6566 6175 6c74 5f74 7261 6e73 666f 726d  efault_transform
+00015900: 2e72 6567 6973 7465 7228 5a65 726f 5375  .register(ZeroSu
+00015910: 6d4e 6f72 6d61 6c52 5629 0a64 6566 207a  mNormalRV).def z
+00015920: 6572 6f73 756d 5f64 6566 6175 6c74 5f74  erosum_default_t
+00015930: 7261 6e73 666f 726d 286f 702c 2072 7629  ransform(op, rv)
+00015940: 3a0a 2020 2020 6e5f 7a65 726f 7375 6d5f  :.    n_zerosum_
+00015950: 6178 6573 203d 2074 7570 6c65 286e 702e  axes = tuple(np.
+00015960: 6172 616e 6765 282d 6f70 2e6e 6469 6d5f  arange(-op.ndim_
+00015970: 7375 7070 2c20 3029 290a 2020 2020 7265  supp, 0)).    re
+00015980: 7475 726e 205a 6572 6f53 756d 5472 616e  turn ZeroSumTran
+00015990: 7366 6f72 6d28 6e5f 7a65 726f 7375 6d5f  sform(n_zerosum_
+000159a0: 6178 6573 290a 0a0a 405f 6c6f 6770 726f  axes)...@_logpro
+000159b0: 622e 7265 6769 7374 6572 285a 6572 6f53  b.register(ZeroS
+000159c0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
+000159d0: 7a65 726f 7375 6d6e 6f72 6d61 6c5f 6c6f  zerosumnormal_lo
+000159e0: 6770 286f 702c 2076 616c 7565 732c 206e  gp(op, values, n
+000159f0: 6f72 6d61 6c5f 6469 7374 2c20 7369 676d  ormal_dist, sigm
+00015a00: 612c 2073 7570 706f 7274 5f73 6861 7065  a, support_shape
+00015a10: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00015a20: 2028 7661 6c75 652c 2920 3d20 7661 6c75   (value,) = valu
+00015a30: 6573 0a20 2020 2073 6861 7065 203d 2076  es.    shape = v
+00015a40: 616c 7565 2e73 6861 7065 0a20 2020 206e  alue.shape.    n
+00015a50: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
+00015a60: 6f70 2e6e 6469 6d5f 7375 7070 0a0a 2020  op.ndim_supp..  
+00015a70: 2020 5f64 6567 5f66 7265 655f 7375 7070    _deg_free_supp
+00015a80: 6f72 745f 7368 6170 6520 3d20 7074 2e69  ort_shape = pt.i
+00015a90: 6e63 5f73 7562 7465 6e73 6f72 2873 6861  nc_subtensor(sha
+00015aa0: 7065 5b2d 6e5f 7a65 726f 7375 6d5f 6178  pe[-n_zerosum_ax
+00015ab0: 6573 3a5d 2c20 2d31 290a 2020 2020 5f66  es:], -1).    _f
+00015ac0: 756c 6c5f 7369 7a65 203d 2070 742e 7072  ull_size = pt.pr
+00015ad0: 6f64 2873 6861 7065 290a 2020 2020 5f64  od(shape).    _d
+00015ae0: 6567 7265 6573 5f6f 665f 6672 6565 646f  egrees_of_freedo
+00015af0: 6d20 3d20 7074 2e70 726f 6428 5f64 6567  m = pt.prod(_deg
+00015b00: 5f66 7265 655f 7375 7070 6f72 745f 7368  _free_support_sh
+00015b10: 6170 6529 0a0a 2020 2020 7a65 726f 7375  ape)..    zerosu
+00015b20: 6d73 203d 205b 0a20 2020 2020 2020 2070  ms = [.        p
+00015b30: 742e 616c 6c28 7074 2e69 7363 6c6f 7365  t.all(pt.isclose
+00015b40: 2870 742e 6d65 616e 2876 616c 7565 2c20  (pt.mean(value, 
+00015b50: 6178 6973 3d2d 6178 6973 202d 2031 292c  axis=-axis - 1),
+00015b60: 2030 2c20 6174 6f6c 3d31 652d 3929 290a   0, atol=1e-9)).
+00015b70: 2020 2020 2020 2020 666f 7220 6178 6973          for axis
+00015b80: 2069 6e20 7261 6e67 6528 6e5f 7a65 726f   in range(n_zero
+00015b90: 7375 6d5f 6178 6573 290a 2020 2020 5d0a  sum_axes).    ].
+00015ba0: 0a20 2020 206f 7574 203d 2070 742e 7375  .    out = pt.su
+00015bb0: 6d28 0a20 2020 2020 2020 2070 6d2e 6c6f  m(.        pm.lo
+00015bc0: 6770 286e 6f72 6d61 6c5f 6469 7374 2c20  gp(normal_dist, 
+00015bd0: 7661 6c75 6529 202a 205f 6465 6772 6565  value) * _degree
+00015be0: 735f 6f66 5f66 7265 6564 6f6d 202f 205f  s_of_freedom / _
+00015bf0: 6675 6c6c 5f73 697a 652c 0a20 2020 2020  full_size,.     
+00015c00: 2020 2061 7869 733d 7475 706c 6528 6e70     axis=tuple(np
+00015c10: 2e61 7261 6e67 6528 2d6e 5f7a 6572 6f73  .arange(-n_zeros
+00015c20: 756d 5f61 7865 732c 2030 2929 2c0a 2020  um_axes, 0)),.  
+00015c30: 2020 290a 0a20 2020 2072 6574 7572 6e20    )..    return 
+00015c40: 6368 6563 6b5f 7061 7261 6d65 7465 7273  check_parameters
+00015c50: 286f 7574 2c20 2a7a 6572 6f73 756d 732c  (out, *zerosums,
+00015c60: 206d 7367 3d22 6d65 616e 2876 616c 7565   msg="mean(value
+00015c70: 2c20 6178 6973 3d6e 5f7a 6572 6f73 756d  , axis=n_zerosum
+00015c80: 5f61 7865 7329 203d 2030 2229 0a         _axes) = 0").
```

### Comparing `pymc-5.5.0/pymc/distributions/shape_utils.py` & `pymc-5.6.0/pymc/distributions/shape_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,15 @@
     A new distribution variable that is equivalent to the original distribution with
     the new size. The new distribution will not reuse the old RandomState/Generator
     input, so it will be independent from the original distribution.
 
     Examples
     --------
     .. code-block:: python
+
         x = Normal.dist(shape=(2, 3))
         new_x = change_dist_size(x, new_size=(5, 3), expand=False)
         assert new_x.eval().shape == (5, 3)
 
         new_x = change_dist_size(x, new_size=(5, 3), expand=True)
         assert new_x.eval().shape == (5, 3, 2, 3)
```

### Comparing `pymc-5.5.0/pymc/distributions/simulator.py` & `pymc-5.6.0/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/timeseries.py` & `pymc-5.6.0/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/transforms.py` & `pymc-5.6.0/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/distributions/truncated.py` & `pymc-5.6.0/pymc/distributions/truncated.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     SymbolicRandomVariable,
     _moment,
     moment,
 )
 from pymc.distributions.shape_utils import _change_dist_size, change_dist_size, to_tuple
 from pymc.distributions.transforms import _default_transform
 from pymc.exceptions import TruncationError
-from pymc.logprob.abstract import MeasurableVariable, _logcdf, _logprob
+from pymc.logprob.abstract import _logcdf, _logprob
 from pymc.logprob.basic import icdf, logcdf
 from pymc.math import logdiffexp
 from pymc.util import check_dist_not_registered
 
 
 class TruncatedRV(SymbolicRandomVariable):
     """
@@ -60,17 +60,14 @@
 
     def update(self, node: Node):
         """Return the update mapping for the noise RV."""
         # Since RNG is a shared variable it shows up as the last node input
         return {node.inputs[-1]: node.outputs[0]}
 
 
-MeasurableVariable.register(TruncatedRV)
-
-
 @singledispatch
 def _truncated(op: Op, lower, upper, size, *params):
     """Return the truncated equivalent of another `RandomVariable`."""
     raise NotImplementedError(f"{op} does not have an equivalent truncated version implemented")
 
 
 class TruncationCheck(CheckAndRaise):
```

### Comparing `pymc-5.5.0/pymc/exceptions.py` & `pymc-5.6.0/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/func_utils.py` & `pymc-5.6.0/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/__init__.py` & `pymc-5.6.0/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/cov.py` & `pymc-5.6.0/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/gp.py` & `pymc-5.6.0/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/hsgp_approx.py` & `pymc-5.6.0/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/mean.py` & `pymc-5.6.0/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/gp/util.py` & `pymc-5.6.0/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/initial_point.py` & `pymc-5.6.0/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/__init__.py` & `pymc-5.6.0/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/abstract.py` & `pymc-5.6.0/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/basic.py` & `pymc-5.6.0/pymc/logprob/basic.py`

 * *Files 23% similar despite different names*

```diff
@@ -92,84 +92,325 @@
     """
 
     rvs_in_graph = _find_unallowed_rvs_in_graph(graph)
     if rvs_in_graph:
         warnings.warn(
             f"RandomVariables {rvs_in_graph} were found in the derived graph. "
             "These variables are a clone and do not match the original ones on identity.\n"
-            "If you are deriving a quantity that depends on model RVs, use `model.replace_rvs_by_values` first. For example: "
-            "`logp(model.replace_rvs_by_values([rv])[0], value)`",
+            "If you are deriving a quantity that depends on model RVs, use `model.replace_rvs_by_values` first. "
+            "For example: `logp(model.replace_rvs_by_values([rv])[0], value)`",
             stacklevel=3,
         )
 
 
-def logp(
-    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
-) -> TensorVariable:
-    """Return the log-probability graph of a Random Variable"""
+def _deprecate_warn_missing_rvs(warn_rvs, kwargs):
+    if "warn_missing_rvs" in kwargs:
+        warnings.warn(
+            "Argument `warn_missing_rvs` was renamed to `warn_rvs` and will be removed in a future release",
+            FutureWarning,
+        )
+        if warn_rvs is None:
+            warn_rvs = kwargs.pop("warn_missing_rvs")
+        else:
+            raise ValueError("Can't set both warn_rvs and warn_missing_rvs")
+    else:
+        if warn_rvs is None:
+            warn_rvs = True
+    return warn_rvs, kwargs
+
+
+def logp(rv: TensorVariable, value: TensorLike, warn_rvs=None, **kwargs) -> TensorVariable:
+    """Create a graph for the log-probability of a random variable.
+
+    Parameters
+    ----------
+    rv : TensorVariable
+    value : tensor_like
+        Should be the same type (shape and dtype) as the rv.
+    warn_rvs : bool, default True
+        Warn if RVs were found in the logp graph.
+        This can happen when a variable has other other random variables as inputs.
+        In that case, those random variables should be replaced by their respective values.
+        `pymc.logprob.conditional_logp` can also be used as an alternative.
+
+    Returns
+    -------
+    logp : TensorVariable
+
+    Raises
+    ------
+    RuntimeError
+        If the logp cannot be derived.
+
+    Examples
+    --------
+    Create a compiled function that evaluates the logp of a variable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+
+        value = pt.scalar("value")
+        rv_logp = pm.logp(rv, value)
+
+        # Use .eval() for debugging
+        print(rv_logp.eval({value: 0.9, mu: 0.0}))  # -1.32393853
+
+        # Compile a function for repeated evaluations
+        rv_logp_fn = pm.compile_pymc([value, mu], rv_logp)
+        print(rv_logp_fn(value=0.9, mu=0.0))  # -1.32393853
+
+
+    Derive the graph for a transformation of a RandomVariable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+        exp_rv = pt.exp(rv)
+
+        value = pt.scalar("value")
+        exp_rv_logp = pm.logp(exp_rv, value)
+
+        # Use .eval() for debugging
+        print(exp_rv_logp.eval({value: 0.9, mu: 0.0}))  # -0.81912844
+
+        # Compile a function for repeated evaluations
+        exp_rv_logp_fn = pm.compile_pymc([value, mu], exp_rv_logp)
+        print(exp_rv_logp_fn(value=0.9, mu=0.0))  # -0.81912844
+
+
+    Define a CustomDist logp
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        def normal_logp(value, mu, sigma):
+            return pm.logp(pm.Normal.dist(mu, sigma), value)
+
+        with pm.Model() as model:
+            mu = pm.Normal("mu")
+            sigma = pm.HalfNormal("sigma")
+            pm.CustomDist("x", mu, sigma, logp=normal_logp)
+
+    """
+    warn_rvs, kwargs = _deprecate_warn_missing_rvs(warn_rvs, kwargs)
 
     value = pt.as_tensor_variable(value, dtype=rv.dtype)
     try:
         return _logprob_helper(rv, value, **kwargs)
     except NotImplementedError:
         fgraph, _, _ = construct_ir_fgraph({rv: value})
         [(ir_rv, ir_value)] = fgraph.preserve_rv_mappings.rv_values.items()
         expr = _logprob_helper(ir_rv, ir_value, **kwargs)
         cleanup_ir([expr])
-        if warn_missing_rvs:
+        if warn_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
-def logcdf(
-    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
-) -> TensorVariable:
-    """Create a graph for the log-CDF of a Random Variable."""
+def logcdf(rv: TensorVariable, value: TensorLike, warn_rvs=None, **kwargs) -> TensorVariable:
+    """Create a graph for the log-CDF of a random variable.
+
+    Parameters
+    ----------
+    rv : TensorVariable
+    value : tensor_like
+        Should be the same type (shape and dtype) as the rv.
+    warn_rvs : bool, default True
+        Warn if RVs were found in the logcdf graph.
+        This can happen when a variable has other random variables as inputs.
+        In that case, those random variables should be replaced by their respective values.
+
+    Returns
+    -------
+    logp : TensorVariable
+
+    Raises
+    ------
+    RuntimeError
+        If the logcdf cannot be derived.
+
+    Examples
+    --------
+    Create a compiled function that evaluates the logcdf of a variable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+
+        value = pt.scalar("value")
+        rv_logcdf = pm.logcdf(rv, value)
+
+        # Use .eval() for debugging
+        print(rv_logcdf.eval({value: 0.9, mu: 0.0}))  # -0.2034146
+
+        # Compile a function for repeated evaluations
+        rv_logcdf_fn = pm.compile_pymc([value, mu], rv_logcdf)
+        print(rv_logcdf_fn(value=0.9, mu=0.0))  # -0.2034146
+
+
+    Derive the graph for a transformation of a RandomVariable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+        exp_rv = pt.exp(rv)
+
+        value = pt.scalar("value")
+        exp_rv_logcdf = pm.logcdf(exp_rv, value)
+
+        # Use .eval() for debugging
+        print(exp_rv_logcdf.eval({value: 0.9, mu: 0.0}))  # -0.78078813
+
+        # Compile a function for repeated evaluations
+        exp_rv_logcdf_fn = pm.compile_pymc([value, mu], exp_rv_logcdf)
+        print(exp_rv_logcdf_fn(value=0.9, mu=0.0))  # -0.78078813
+
+
+    Define a CustomDist logcdf
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        def normal_logcdf(value, mu, sigma):
+            return pm.logp(pm.Normal.dist(mu, sigma), value)
+
+        with pm.Model() as model:
+            mu = pm.Normal("mu")
+            sigma = pm.HalfNormal("sigma")
+            pm.CustomDist("x", mu, sigma, logcdf=normal_logcdf)
+
+    """
+    warn_rvs, kwargs = _deprecate_warn_missing_rvs(warn_rvs, kwargs)
     value = pt.as_tensor_variable(value, dtype=rv.dtype)
     try:
         return _logcdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
         expr = _logcdf_helper(ir_rv, value, **kwargs)
         cleanup_ir([expr])
-        if warn_missing_rvs:
+        if warn_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
-def icdf(
-    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
-) -> TensorVariable:
-    """Create a graph for the inverse CDF of a  Random Variable."""
+def icdf(rv: TensorVariable, value: TensorLike, warn_rvs=None, **kwargs) -> TensorVariable:
+    """Create a graph for the inverse CDF of a random variable.
+
+    Parameters
+    ----------
+    rv : TensorVariable
+    value : tensor_like
+        Should be the same type (shape and dtype) as the rv.
+    warn_rvs : bool, default True
+        Warn if RVs were found in the icdf graph.
+        This can happen when a variable has other random variables as inputs.
+        In that case, those random variables should be replaced by their respective values.
+
+    Returns
+    -------
+    icdf : TensorVariable
+
+    Raises
+    ------
+    RuntimeError
+        If the icdf cannot be derived.
+
+    Examples
+    --------
+    Create a compiled function that evaluates the icdf of a variable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+
+        value = pt.scalar("value")
+        rv_icdf = pm.icdf(rv, value)
+
+        # Use .eval() for debugging
+        print(rv_icdf.eval({value: 0.9, mu: 0.0}))  # 1.28155157
+
+        # Compile a function for repeated evaluations
+        rv_icdf_fn = pm.compile_pymc([value, mu], rv_icdf)
+        print(rv_icdf_fn(value=0.9, mu=0.0))  # 1.28155157
+
+
+    Derive the graph for a transformation of a RandomVariable
+
+    .. code-block:: python
+
+        import pymc as pm
+        import pytensor.tensor as pt
+
+        mu = pt.scalar("mu")
+        rv = pm.Normal.dist(mu, 1.0)
+        exp_rv = pt.exp(rv)
+
+        value = pt.scalar("value")
+        exp_rv_icdf = pm.icdf(exp_rv, value)
+
+        # Use .eval() for debugging
+        print(exp_rv_icdf.eval({value: 0.9, mu: 0.0}))  # 3.60222448
+
+        # Compile a function for repeated evaluations
+        exp_rv_icdf_fn = pm.compile_pymc([value, mu], exp_rv_icdf)
+        print(exp_rv_icdf_fn(value=0.9, mu=0.0))  # 3.60222448
+
+    """
+    warn_rvs, kwargs = _deprecate_warn_missing_rvs(warn_rvs, kwargs)
     value = pt.as_tensor_variable(value, dtype="floatX")
     try:
         return _icdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
         expr = _icdf_helper(ir_rv, value, **kwargs)
         cleanup_ir([expr])
-        if warn_missing_rvs:
+        if warn_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
 RVS_IN_JOINT_LOGP_GRAPH_MSG = (
     "Random variables detected in the logp graph: %s.\n"
     "This can happen when DensityDist logp or Interval transform functions reference nonlocal variables,\n"
     "or when not all rvs have a corresponding value variable."
 )
 
 
 def conditional_logp(
     rv_values: Dict[TensorVariable, TensorVariable],
-    warn_missing_rvs: bool = True,
+    warn_rvs=None,
     ir_rewriter: Optional[GraphRewriter] = None,
     extra_rewrites: Optional[Union[GraphRewriter, NodeRewriter]] = None,
     **kwargs,
 ) -> Dict[TensorVariable, TensorVariable]:
     r"""Create a map between variables and conditional log-probabilities
     such that the sum is their joint log-probability.
 
@@ -191,47 +432,52 @@
 
         \Sigma^2 \sim& \operatorname{InvGamma}(0.5, 0.5) \\
         Y \sim& \operatorname{N}(0, \Sigma)
 
     If we create a value variable for ``Y_rv``, i.e. ``y_vv = pt.scalar("y")``,
     the graph of ``conditional_logp({Y_rv: y_vv})`` is equivalent to the
     conditional log-probability :math:`\log p(Y = y \mid \Sigma^2)`, with a stochastic
-    ``sigma2_rv``. If we specify a value variable for ``sigma2_rv``, i.e.
+    ``sigma2_rv``.
+
+    If we specify a value variable for ``sigma2_rv``, i.e.
     ``s_vv = pt.scalar("s2")``, then ``conditional_logp({Y_rv: y_vv, sigma2_rv: s_vv})``
     yields the conditional log-probabilities of the two variables.
     The sum of the two terms gives their joint log-probability.
 
     .. math::
 
         \log p(Y = y, \Sigma^2 = \sigma^2) =
             \log p(Y = y \mid \Sigma^2 = \sigma^2) + \log p(\Sigma^2 = \sigma^2)
 
 
     Parameters
     ----------
-    rv_values
+    rv_values: dict
         A ``dict`` of variables that maps stochastic elements
         (e.g. `RandomVariable`\s) to symbolic `Variable`\s representing their
         values in a log-probability.
-    warn_missing_rvs
+    warn_rvs : bool, default True
         When ``True``, issue a warning when a `RandomVariable` is found in
         the logp graph and doesn't have a corresponding value variable specified in
         `rv_values`.
     ir_rewriter
         Rewriter that produces the intermediate representation of Measurable Variables.
     extra_rewrites
         Extra rewrites to be applied (e.g. reparameterizations, transforms,
         etc.)
 
     Returns
     -------
-    A ``dict`` that maps each value variable to the conditional log-probability term derived
-    from the respective `RandomVariable`.
+    values_to_logps: dict
+        A ``dict`` that maps each value variable to the conditional log-probability term derived
+        from the respective `RandomVariable`.
 
     """
+    warn_rvs, kwargs = _deprecate_warn_missing_rvs(warn_rvs, kwargs)
+
     fgraph, rv_values, _ = construct_ir_fgraph(rv_values, ir_rewriter=ir_rewriter)
 
     if extra_rewrites is not None:
         extra_rewrites.rewrite(fgraph)
 
     rv_remapper = fgraph.preserve_rv_mappings
 
@@ -326,15 +572,15 @@
         raise RuntimeError(
             f"The logprob terms of the following value variables could not be derived: {missing_value_terms}"
         )
 
     logprob_expressions = list(logprob_vars.values())
     cleanup_ir(logprob_expressions)
 
-    if warn_missing_rvs:
+    if warn_rvs:
         rvs_in_logp_expressions = _find_unallowed_rvs_in_graph(logprob_expressions)
         if rvs_in_logp_expressions:
             warnings.warn(RVS_IN_JOINT_LOGP_GRAPH_MSG % rvs_in_logp_expressions, UserWarning)
 
     return logprob_vars
 
 
@@ -358,15 +604,15 @@
         for rv, transform in rvs_to_transforms.items()
         if transform is not None
     }
     if values_to_transforms:
         # There seems to be an incorrect type hint in TransformValuesRewrite
         transform_rewrite = TransformValuesRewrite(values_to_transforms)  # type: ignore
 
-    kwargs.setdefault("warn_missing_rvs", False)
+    kwargs.setdefault("warn_rvs", False)
     temp_logp_terms = conditional_logp(
         rvs_to_values,
         extra_rewrites=transform_rewrite,
         use_jacobian=jacobian,
         **kwargs,
     )
```

### Comparing `pymc-5.5.0/pymc/logprob/binary.py` & `pymc-5.6.0/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/censoring.py` & `pymc-5.6.0/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/checks.py` & `pymc-5.6.0/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/cumsum.py` & `pymc-5.6.0/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/mixture.py` & `pymc-5.6.0/pymc/logprob/mixture.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,34 +40,40 @@
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Apply, Constant, Variable
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op, compute_test_value
 from pytensor.graph.rewriting.basic import node_rewriter, pre_greedy_node_rewriter
 from pytensor.ifelse import IfElse, ifelse
+from pytensor.scalar import Switch
+from pytensor.scalar import switch as scalar_switch
 from pytensor.tensor.basic import Join, MakeVector, switch
 from pytensor.tensor.random.rewriting import (
     local_dimshuffle_rv_lift,
     local_rv_size_lift,
     local_subtensor_rv_lift,
 )
 from pytensor.tensor.shape import shape_tuple
 from pytensor.tensor.subtensor import (
     AdvancedSubtensor,
     AdvancedSubtensor1,
     as_index_literal,
-    as_nontensor_scalar,
     get_canonical_form_slice,
     is_basic_idx,
 )
 from pytensor.tensor.type import TensorType
 from pytensor.tensor.type_other import NoneConst, NoneTypeT, SliceConstant, SliceType
 from pytensor.tensor.var import TensorVariable
 
-from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
+from pymc.logprob.abstract import (
+    MeasurableElemwise,
+    MeasurableVariable,
+    _logprob,
+    _logprob_helper,
+)
 from pymc.logprob.rewriting import (
     PreserveRVMappings,
     assume_measured_ir_outputs,
     local_lift_DiracDelta,
     measurable_ir_rewrites_db,
     subtensor_ops,
 )
@@ -321,45 +327,14 @@
             compute_test_value(node)
 
         new_mixture_rv.tag.test_value = old_mixture_rv.tag.test_value
 
     return [new_mixture_rv]
 
 
-@node_rewriter([switch])
-def find_measurable_switch_mixture(fgraph, node):
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    old_mixture_rv = node.default_output()
-    idx, *components = node.inputs
-
-    if rv_map_feature.request_measurable(components) != components:
-        return None
-
-    mix_op = MixtureRV(
-        2,
-        old_mixture_rv.dtype,
-        old_mixture_rv.broadcastable,
-    )
-    new_mixture_rv = mix_op.make_node(
-        *([NoneConst, as_nontensor_scalar(node.inputs[0])] + components[::-1])
-    ).default_output()
-
-    if pytensor.config.compute_test_value != "off":
-        if not hasattr(old_mixture_rv.tag, "test_value"):
-            compute_test_value(node)
-
-        new_mixture_rv.tag.test_value = old_mixture_rv.tag.test_value
-
-    return [new_mixture_rv]
-
-
 @_logprob.register(MixtureRV)
 def logprob_MixtureRV(
     op, values, *inputs: Optional[Union[TensorVariable, slice]], name=None, **kwargs
 ):
     (value,) = values
 
     join_axis = cast(Variable, inputs[0])
@@ -429,14 +404,59 @@
                 comp_logp,
                 pt.zeros_like(comp_logp),
             )
 
     return logp_val
 
 
+class MeasurableSwitchMixture(MeasurableElemwise):
+    valid_scalar_types = (Switch,)
+
+
+measurable_switch_mixture = MeasurableSwitchMixture(scalar_switch)
+
+
+@node_rewriter([switch])
+def find_measurable_switch_mixture(fgraph, node):
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
+
+    if rv_map_feature is None:
+        return None  # pragma: no cover
+
+    switch_cond, *components = node.inputs
+
+    # We don't support broadcasting of components, as that yields dependent (identical) values.
+    # The current logp implementation assumes all component values are independent.
+    # Broadcasting of the switch condition is fine
+    out_bcast = node.outputs[0].type.broadcastable
+    if any(comp.type.broadcastable != out_bcast for comp in components):
+        return None
+
+    # Check that `switch_cond` is not potentially measurable
+    valued_rvs = rv_map_feature.rv_values.keys()
+    if check_potential_measurability([switch_cond], valued_rvs):
+        return None
+
+    if rv_map_feature.request_measurable(components) != components:
+        return None
+
+    return [measurable_switch_mixture(switch_cond, *components)]
+
+
+@_logprob.register(MeasurableSwitchMixture)
+def logprob_switch_mixture(op, values, switch_cond, component_true, component_false, **kwargs):
+    [value] = values
+
+    return switch(
+        switch_cond,
+        _logprob_helper(component_true, value),
+        _logprob_helper(component_false, value),
+    )
+
+
 measurable_ir_rewrites_db.register(
     "find_measurable_index_mixture",
     find_measurable_index_mixture,
     "basic",
     "mixture",
 )
```

### Comparing `pymc-5.5.0/pymc/logprob/rewriting.py` & `pymc-5.6.0/pymc/logprob/rewriting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/scan.py` & `pymc-5.6.0/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/tensor.py` & `pymc-5.6.0/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/logprob/transforms.py` & `pymc-5.6.0/pymc/logprob/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import GraphRewriter, in2out, node_rewriter
 from pytensor.scalar import (
     Abs,
     Add,
+    ArcCosh,
+    ArcSinh,
+    ArcTanh,
     Cosh,
     Erf,
     Erfc,
     Erfcx,
     Exp,
     Log,
     Mul,
@@ -67,14 +70,17 @@
     Tanh,
 )
 from pytensor.scan.op import Scan
 from pytensor.tensor.exceptions import NotScalarConstantError
 from pytensor.tensor.math import (
     abs,
     add,
+    arccosh,
+    arcsinh,
+    arctanh,
     cosh,
     erf,
     erfc,
     erfcx,
     exp,
     log,
     mul,
@@ -365,15 +371,31 @@
         self.transform_rewrite.rewrite(fgraph)
         self.scan_transform_rewrite.rewrite(fgraph)
 
 
 class MeasurableTransform(MeasurableElemwise):
     """A placeholder used to specify a log-likelihood for a transformed measurable variable"""
 
-    valid_scalar_types = (Exp, Log, Add, Mul, Pow, Abs, Sinh, Cosh, Tanh, Erf, Erfc, Erfcx)
+    valid_scalar_types = (
+        Exp,
+        Log,
+        Add,
+        Mul,
+        Pow,
+        Abs,
+        Sinh,
+        Cosh,
+        Tanh,
+        ArcSinh,
+        ArcCosh,
+        ArcTanh,
+        Erf,
+        Erfc,
+        Erfcx,
+    )
 
     # Cannot use `transform` as name because it would clash with the property added by
     # the `TransformValuesRewrite`
     transform_elemwise: RVTransform
     measurable_input_idx: int
 
     def __init__(self, *args, transform: RVTransform, measurable_input_idx: int, **kwargs):
@@ -422,15 +444,16 @@
 def measurable_transform_logcdf(op: MeasurableTransform, value, *inputs, **kwargs):
     """Compute the log-CDF graph for a `MeasurabeTransform`."""
     other_inputs = list(inputs)
     measurable_input = other_inputs.pop(op.measurable_input_idx)
 
     backward_value = op.transform_elemwise.backward(value, *other_inputs)
 
-    # Some transformations, like squaring may produce multiple backward values
+    # Fail if transformation is not injective
+    # A TensorVariable is returned in 1-to-1 inversions, and a tuple in 1-to-many
     if isinstance(backward_value, tuple):
         raise NotImplementedError
 
     input_logcdf = _logcdf_helper(measurable_input, backward_value)
 
     # The jacobian is used to ensure a value in the supported domain was provided
     jacobian = op.transform_elemwise.log_jac_det(value, *other_inputs)
@@ -443,14 +466,19 @@
     """Compute the inverse CDF graph for a `MeasurabeTransform`."""
     other_inputs = list(inputs)
     measurable_input = other_inputs.pop(op.measurable_input_idx)
 
     input_icdf = _icdf_helper(measurable_input, value)
     icdf = op.transform_elemwise.forward(input_icdf, *other_inputs)
 
+    # Fail if transformation is not injective
+    # A TensorVariable is returned in 1-to-1 inversions, and a tuple in 1-to-many
+    if isinstance(op.transform_elemwise.backward(icdf, *other_inputs), tuple):
+        raise NotImplementedError
+
     return icdf
 
 
 @node_rewriter([reciprocal])
 def measurable_reciprocal_to_power(fgraph, node):
     """Convert reciprocal of `MeasurableVariable`s to power."""
     [inp] = node.inputs
@@ -497,15 +525,17 @@
 @node_rewriter([sub])
 def measurable_sub_to_neg(fgraph, node):
     """Convert subtraction involving `MeasurableVariable`s to addition with neg"""
     minuend, subtrahend = node.inputs
     return [pt.add(minuend, pt.neg(subtrahend))]
 
 
-@node_rewriter([exp, log, add, mul, pow, abs, sinh, cosh, tanh, erf, erfc, erfcx])
+@node_rewriter(
+    [exp, log, add, mul, pow, abs, sinh, cosh, tanh, arcsinh, arccosh, arctanh, erf, erfc, erfcx]
+)
 def find_measurable_transforms(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
     """Find measurable transformations from Elemwise operators."""
 
     # Node was already converted
     if isinstance(node.op, MeasurableVariable):
         return None  # pragma: no cover
 
@@ -540,14 +570,17 @@
     transform_dict = {
         Exp: ExpTransform(),
         Log: LogTransform(),
         Abs: AbsTransform(),
         Sinh: SinhTransform(),
         Cosh: CoshTransform(),
         Tanh: TanhTransform(),
+        ArcSinh: ArcsinhTransform(),
+        ArcCosh: ArccoshTransform(),
+        ArcTanh: ArctanhTransform(),
         Erf: ErfTransform(),
         Erfc: ErfcTransform(),
         Erfcx: ErfcxTransform(),
     }
     transform = transform_dict.get(type(scalar_op), None)
     if isinstance(scalar_op, Pow):
         # We only allow for the base to be measurable
@@ -656,14 +689,47 @@
     def forward(self, value, *inputs):
         return pt.tanh(value)
 
     def backward(self, value, *inputs):
         return pt.arctanh(value)
 
 
+class ArcsinhTransform(RVTransform):
+    name = "arcsinh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.arcsinh(value)
+
+    def backward(self, value, *inputs):
+        return pt.sinh(value)
+
+
+class ArccoshTransform(RVTransform):
+    name = "arccosh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.arccosh(value)
+
+    def backward(self, value, *inputs):
+        return pt.cosh(value)
+
+
+class ArctanhTransform(RVTransform):
+    name = "arctanh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.arctanh(value)
+
+    def backward(self, value, *inputs):
+        return pt.tanh(value)
+
+
 class ErfTransform(RVTransform):
     name = "erf"
     ndim_supp = 0
 
     def forward(self, value, *inputs):
         return pt.erf(value)
 
@@ -894,25 +960,29 @@
         return pt.log(sigmoid_value) + pt.log1p(-sigmoid_value)
 
 
 class SimplexTransform(RVTransform):
     name = "simplex"
 
     def forward(self, value, *inputs):
+        value = pt.as_tensor(value)
         log_value = pt.log(value)
-        shift = pt.sum(log_value, -1, keepdims=True) / value.shape[-1]
+        N = value.shape[-1].astype(value.dtype)
+        shift = pt.sum(log_value, -1, keepdims=True) / N
         return log_value[..., :-1] - shift
 
     def backward(self, value, *inputs):
         value = pt.concatenate([value, -pt.sum(value, -1, keepdims=True)], axis=-1)
         exp_value_max = pt.exp(value - pt.max(value, -1, keepdims=True))
         return exp_value_max / pt.sum(exp_value_max, -1, keepdims=True)
 
     def log_jac_det(self, value, *inputs):
+        value = pt.as_tensor(value)
         N = value.shape[-1] + 1
+        N = N.astype(value.dtype)
         sum_value = pt.sum(value, -1, keepdims=True)
         value_sum_expanded = value + sum_value
         value_sum_expanded = pt.concatenate([value_sum_expanded, pt.zeros(sum_value.shape)], -1)
         logsumexp_value_expanded = pt.logsumexp(value_sum_expanded, -1, keepdims=True)
         res = pt.log(N) + (N * sum_value) - (N * logsumexp_value_expanded)
         return pt.sum(res, -1)
```

### Comparing `pymc-5.5.0/pymc/logprob/utils.py` & `pymc-5.6.0/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/math.py` & `pymc-5.6.0/pymc/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,19 +439,25 @@
         return packed[diag_idxs]
     elif diagonal_only and not lower:
         diag_idxs = np.arange(2, n + 2)[::-1].cumsum() - n - 1
         return packed[diag_idxs]
     elif lower:
         out = pt.zeros((n, n), dtype=pytensor.config.floatX)
         idxs = np.tril_indices(n)
-        return pt.set_subtensor(out[idxs], packed)
+        # tag as lower triangular to enable pytensor rewrites
+        out = pt.set_subtensor(out[idxs], packed)
+        out.tag.lower_triangular = True
+        return out
     elif not lower:
         out = pt.zeros((n, n), dtype=pytensor.config.floatX)
         idxs = np.triu_indices(n)
-        return pt.set_subtensor(out[idxs], packed)
+        # tag as upper triangular to enable pytensor rewrites
+        out = pt.set_subtensor(out[idxs], packed)
+        out.tag.upper_triangular = True
+        return out
 
 
 class BatchedDiag(Op):
     """
     Fast BatchedDiag allocation
     """
```

### Comparing `pymc-5.5.0/pymc/model.py` & `pymc-5.6.0/pymc/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,17 @@
 import pytensor.sparse as sparse
 import pytensor.tensor as pt
 import scipy.sparse as sps
 
 from pytensor.compile import DeepCopyOp, get_mode
 from pytensor.compile.sharedvalue import SharedVariable
 from pytensor.graph.basic import Constant, Variable, graph_inputs
-from pytensor.graph.fg import FunctionGraph
 from pytensor.scalar import Cast
 from pytensor.tensor.elemwise import Elemwise
 from pytensor.tensor.random.op import RandomVariable
-from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
 from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.sharedvar import ScalarSharedVariable
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 from pymc.blocking import DictToArrayBijection, RaveledVars
 from pymc.data import GenTensorVariable, is_minibatch
 from pymc.distributions.transforms import _default_transform
@@ -71,14 +69,15 @@
     SeedSequenceSeed,
     compile_pymc,
     convert_observed_data,
     gradient,
     hessian,
     inputvars,
     replace_rvs_by_values,
+    rewrite_pregrad,
 )
 from pymc.util import (
     UNSET,
     WithMemoization,
     _add_future_warning_tag,
     get_transformed_name,
     get_value_vars_from_user_vars,
@@ -95,64 +94,14 @@
     "Potential",
     "set_data",
     "Point",
     "compile_fn",
 ]
 
 
-class InstanceMethod:
-    """Class for hiding references to instance methods so they can be pickled.
-
-    >>> self.method = InstanceMethod(some_object, 'method_name')
-    """
-
-    def __init__(self, obj, method_name):
-        self.obj = obj
-        self.method_name = method_name
-
-    def __call__(self, *args, **kwargs):
-        return getattr(self.obj, self.method_name)(*args, **kwargs)
-
-
-def incorporate_methods(source, destination, methods, wrapper=None, override=False):
-    """
-    Add attributes to a destination object which point to
-    methods from from a source object.
-
-    Parameters
-    ----------
-    source: object
-        The source object containing the methods.
-    destination: object
-        The destination object for the methods.
-    methods: list of str
-        Names of methods to incorporate.
-    wrapper: function
-        An optional function to allow the source method to be
-        wrapped. Should take the form my_wrapper(source, method_name)
-        and return a single value.
-    override: bool
-        If the destination object already has a method/attribute
-        an AttributeError will be raised if override is False (the default).
-    """
-    for method in methods:
-        if hasattr(destination, method) and not override:
-            raise AttributeError(
-                f"Cannot add method {method!r}" + "to destination object as it already exists. "
-                "To prevent this error set 'override=True'."
-            )
-        if hasattr(source, method):
-            if wrapper is None:
-                setattr(destination, method, getattr(source, method))
-            else:
-                setattr(destination, method, wrapper(source, method))
-        else:
-            setattr(destination, method, None)
-
-
 T = TypeVar("T", bound="ContextMeta")
 
 
 class ContextMeta(type):
     """Functionality for objects that put themselves in a context using
     the `with` statement.
     """
@@ -377,14 +326,16 @@
         for var, value in extra_vars_and_values.items():
             shared = pytensor.shared(
                 value, var.name + "_shared__", shape=[1 if s == 1 else None for s in value.shape]
             )
             self._extra_vars_shared[var.name] = shared
             givens.append((var, shared))
 
+        cost = rewrite_pregrad(cost)
+
         if compute_grads:
             grads = pytensor.grad(cost, grad_vars, disconnected_inputs="ignore")
             for grad_wrt, var in zip(grads, grad_vars):
                 grad_wrt.name = f"{var.name}_grad"
             outputs = [cost] + grads
         else:
             outputs = [cost]
@@ -820,14 +771,15 @@
                     value_vars.append(value_var)
                 else:
                     raise ValueError(
                         f"Requested variable {var} not found among the model variables"
                     )
 
         cost = self.logp(jacobian=jacobian)
+        cost = rewrite_pregrad(cost)
         return gradient(cost, value_vars)
 
     def d2logp(
         self,
         vars: Optional[Union[Variable, Sequence[Variable]]] = None,
         jacobian: bool = True,
     ) -> Variable:
@@ -858,14 +810,15 @@
                     value_vars.append(value_var)
                 else:
                     raise ValueError(
                         f"Requested variable {var} not found among the model variables"
                     )
 
         cost = self.logp(jacobian=jacobian)
+        cost = rewrite_pregrad(cost)
         return hessian(cost, value_vars)
 
     @property
     def datalogp(self) -> Variable:
         """PyTensor scalar of log-probability of the observed variables and
         potential terms"""
         return self.observedlogp + self.potentiallogp
@@ -1228,15 +1181,15 @@
                     # The dimension was created from another variable:
                     length_tensor_origin = length_tensor.owner.inputs[0]
                     # Get a handle on the tensor from which this dimension length was
                     # obtained by doing subindexing on the shape as in `.shape[i]`.
                     if isinstance(length_tensor_origin, TensorConstant):
                         raise ShapeError(
                             f"Resizing dimension '{dname}' with values of length {new_length} would lead to incompatibilities, "
-                            f"because the dimension length is tied to a {length_tensor_origin}. "
+                            f"because the dimension length is tied to a TensorConstant. "
                             f"Check if the dimension was defined implicitly before the shared variable '{name}' was created, "
                             f"for example by another model variable.",
                             actual=new_length,
                             expected=old_length,
                         )
 
                     # The shape entry this dimension is tied to is not a TensorConstant.
@@ -1405,75 +1358,35 @@
                 " sampling distribution."
             )
             warnings.warn(impute_message, ImputationWarning)
 
             if total_size is not None:
                 raise ValueError("total_size is not compatible with imputed variables")
 
-            if not isinstance(rv_var.owner.op, RandomVariable):
-                raise NotImplementedError(
-                    "Automatic inputation is only supported for univariate RandomVariables."
-                    f" {rv_var} of type {type(rv_var.owner.op)} is not supported."
-                )
+            from pymc.distributions.distribution import create_partial_observed_rv
 
-            if rv_var.owner.op.ndim_supp > 0:
-                raise NotImplementedError(
-                    f"Automatic inputation is only supported for univariate "
-                    f"RandomVariables, but {rv_var} is multivariate"
-                )
-
-            # We can get a random variable comprised of only the unobserved
-            # entries by lifting the indices through the `RandomVariable` `Op`.
+            (
+                (observed_rv, observed_mask),
+                (unobserved_rv, _),
+                joined_rv,
+            ) = create_partial_observed_rv(rv_var, mask)
+            observed_data = pt.as_tensor(data.data[observed_mask])
+
+            # Register ObservedRV corresponding to observed component
+            observed_rv.name = f"{name}_observed"
+            self.create_value_var(observed_rv, transform=None, value_var=observed_data)
+            self.add_named_variable(observed_rv)
+            self.observed_RVs.append(observed_rv)
 
-            masked_rv_var = rv_var[mask.nonzero()]
+            # Register FreeRV corresponding to unobserved components
+            self.register_rv(unobserved_rv, f"{name}_unobserved", transform=transform)
 
-            fgraph = FunctionGraph(
-                [i for i in graph_inputs((masked_rv_var,)) if not isinstance(i, Constant)],
-                [masked_rv_var],
-                clone=False,
-            )
-
-            (missing_rv_var,) = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
-
-            self.register_rv(missing_rv_var, f"{name}_missing", transform=transform)
-
-            # Now, we lift the non-missing observed values and produce a new
-            # `rv_var` that contains only those.
-            #
-            # The end result is two disjoint distributions: one for the missing
-            # values, and another for the non-missing values.
-
-            antimask_idx = (~mask).nonzero()
-            nonmissing_data = pt.as_tensor_variable(data[antimask_idx].data)
-            unmasked_rv_var = rv_var[antimask_idx]
-            unmasked_rv_var = unmasked_rv_var.owner.clone().default_output()
-
-            fgraph = FunctionGraph(
-                [i for i in graph_inputs((unmasked_rv_var,)) if not isinstance(i, Constant)],
-                [unmasked_rv_var],
-                clone=False,
-            )
-            (observed_rv_var,) = local_subtensor_rv_lift.transform(fgraph, fgraph.outputs[0].owner)
-            # Make a clone of the RV, but let it create a new rng so that observed and
-            # missing are not treated as equivalent nodes by pytensor. This would happen
-            # if the size of the masked and unmasked array happened to coincide
-            _, size, _, *inps = observed_rv_var.owner.inputs
-            observed_rv_var = observed_rv_var.owner.op(*inps, size=size, name=f"{name}_observed")
-            observed_rv_var.tag.observations = nonmissing_data
-
-            self.create_value_var(observed_rv_var, transform=None, value_var=nonmissing_data)
-            self.add_named_variable(observed_rv_var)
-            self.observed_RVs.append(observed_rv_var)
-
-            # Create deterministic that combines observed and missing
+            # Register Deterministic that combines observed and missing
             # Note: This can widely increase memory consumption during sampling for large datasets
-            rv_var = pt.empty(data.shape, dtype=observed_rv_var.type.dtype)
-            rv_var = pt.set_subtensor(rv_var[mask.nonzero()], missing_rv_var)
-            rv_var = pt.set_subtensor(rv_var[antimask_idx], observed_rv_var)
-            rv_var = Deterministic(name, rv_var, self, dims)
+            rv_var = Deterministic(name, joined_rv, self, dims)
 
         else:
             if sps.issparse(data):
                 data = sparse.basic.as_sparse(data, name=name)
             else:
                 data = pt.as_tensor_variable(data, name=name)
 
@@ -2195,23 +2108,22 @@
         ),
         var,
     )
 
     return var
 
 
-def Potential(name, var, model=None, dims=None):
-    """
-    Add an arbitrary factor potential to the model likelihood
-
-    The Potential function is used to add arbitrary factors (such as constraints or other likelihood components) to adjust the probability density of the model.
+def Potential(name, var: TensorVariable, model=None, dims=None) -> TensorVariable:
+    """Add an arbitrary term to the model log-probability.
 
     Warnings
     --------
-    Potential functions only influence logp-based sampling. Therefore, they are applicable for sampling with ``pm.sample`` but not ``pm.sample_prior_predictive`` or ``pm.sample_posterior_predictive``.
+    Potential terms only influence probability-based sampling, such as ``pm.sample``, but not forward sampling like
+    ``pm.sample_prior_predictive`` or ``pm.sample_posterior_predictive``. A warning is raised when doing forward
+    sampling with models containing Potential terms.
 
     Parameters
     ----------
     name : str
         Name of the potential variable to be registered in the model.
     var : tensor_like
         Expression to be added to the model joint logp.
@@ -2224,70 +2136,88 @@
     Returns
     -------
     var : tensor_like
         The registered, named model variable.
 
     Examples
     --------
-    Have a look at the following example:
-
-    In this example, we define a constraint on ``x`` to be greater or equal to 0 via the ``pm.Potential`` function.
-    We pass ``pm.math.log(pm.math.switch(constraint, 1, 0))`` as second argument which will return an expression depending on if the constraint is met or not and which will be added to the likelihood of the model.
-    The probablity density that this model produces agrees strongly with the constraint that ``x`` should be greater than or equal to 0. All the cases who do not satisfy the constraint are strictly not considered.
+    In this example, we define a constraint on ``x`` to be greater or equal to 0.
+    The statement ``pm.math.log(pm.math.switch(constraint, 0, 1))`` adds either 0 or -inf to the model logp,
+    depending on whether the constraint is met. During sampling, any proposals where ``x`` is negative will be rejected.
 
     .. code:: python
 
+        import pymc as pm
+
         with pm.Model() as model:
             x = pm.Normal("x", mu=0, sigma=1)
-            y = pm.Normal("y", mu=x, sigma=1, observed=data)
+
             constraint = x >= 0
             potential = pm.Potential("x_constraint", pm.math.log(pm.math.switch(constraint, 1, 0)))
 
-    However, if we use ``pm.math.log(pm.math.switch(constraint, 1.0, 0.5))`` the potential again penalizes the likelihood when constraint is not met but with some deviations allowed.
-    Here, Potential function is used to pass a soft constraint.
-    A soft constraint is a constraint that is only partially satisfied.
-    The effect of this is that the posterior probability for the parameters decreases as they move away from the constraint, but does not become exactly zero.
-    This allows the sampler to generate values that violate the constraint, but with lower probability.
+
+    Instead, with a soft constraint like ``pm.math.log(pm.math.switch(constraint, 1, 0.5))``,
+    the sampler will be less likely, but not forbidden, from accepting negative values for `x`.
 
     .. code:: python
 
+        import pymc as pm
+
         with pm.Model() as model:
-            x = pm.Normal("x", mu=0.1, sigma=1)
-            y = pm.Normal("y", mu=x, sigma=1, observed=data)
+            x = pm.Normal("x", mu=0, sigma=1)
+
             constraint = x >= 0
             potential = pm.Potential("x_constraint", pm.math.log(pm.math.switch(constraint, 1.0, 0.5)))
 
-    In this example, Potential is used to obtain an arbitrary prior.
-    This prior distribution refers to the prior knowledge that the values of ``max_items`` are likely to be small rather than being large.
-    The prior probability of ``max_items`` is defined using a Potential object with the log of the inverse of ``max_items`` as its value.
-    This means that larger values of ``max_items`` have a lower prior probability density, while smaller values of ``max_items`` have a higher prior probability density.
-    When the model is sampled, the posterior distribution of ``max_items`` given the observed value of ``n_items`` will be influenced by the power-law prior defined in the Potential object
+    A Potential term can depend on multiple variables.
+    In the following example, the ``soft_sum_constraint`` potential encourages ``x`` and ``y`` to have a small sum.
+    The more the sum deviates from zero, the more negative the penalty value of ``(-((x + y)**2))``.
 
     .. code:: python
 
-        with pm.Model():
+        import pymc as pm
+
+        with pm.Model() as model:
+            x = pm.Normal("x", mu=0, sigma=10)
+            y = pm.Normal("y", mu=0, sigma=10)
+            soft_sum_constraint = pm.Potential("soft_sum_constraint", -((x + y)**2))
+
+    A Potential can be used to define a specific prior term.
+    The following example imposes a power law prior on `max_items`, under the form ``log(1/max_items)``,
+    which penalizes very large values of `max_items`.
+
+    .. code:: python
+
+        import pymc as pm
+
+        with pm.Model() as model:
             # p(max_items) = 1 / max_items
             max_items = pm.Uniform("max_items", lower=1, upper=100)
             pm.Potential("power_prior", pm.math.log(1/max_items))
 
             n_items = pm.Uniform("n_items", lower=1, upper=max_items, observed=60)
 
-    In the next example, the ``soft_sum_constraint`` potential encourages ``x`` and ``y`` to have a small sum, effectively adding a soft constraint on the relationship between the two variables.
-    This can be useful in cases where you want to ensure that the sum of multiple variables stays within a certain range, without enforcing an exact value.
-    In this case, the larger the deviation, larger will be the negative value (-((x + y)**2)) which the MCMC sampler will attempt to minimize.
-    However, the sampler might generate values for some small deviations but with lower probability hence this is a soft constraint.
+    A Potential can be used to define a specific likelihood term.
+    In the following example, a normal likelihood term is added to fixed data.
+    The same result would be obtained by using an observed `Normal` variable.
 
     .. code:: python
 
+        import pymc as pm
+
+        def normal_logp(value, mu, sigma):
+            return -0.5 * ((value - mu) / sigma) ** 2 - pm.math.log(sigma)
+
         with pm.Model() as model:
-            x = pm.Normal("x", mu=0.1, sigma=1)
-            y = pm.Normal("y", mu=x, sigma=1, observed=data)
-            soft_sum_constraint = pm.Potential("soft_sum_constraint", -((x + y)**2))
+            mu = pm.Normal("x")
+            sigma = pm.HalfNormal("sigma")
+
+            data = [0.1, 0.5, 0.9]
+            llike = pm.Potential("llike", normal_logp(data, mu, sigma))
 
-    The potential value is incorporated into the model log-probability, so it should be -inf (or very negative) when a constraint is violated, so that those draws are rejected. 0 won't have any effect and positive values will make the proposals more likely to be accepted.
 
     """
     model = modelcontext(model)
     var.name = model.name_for(name)
     model.potentials.append(var)
     model.add_named_variable(var, dims)
```

### Comparing `pymc-5.5.0/pymc/model_graph.py` & `pymc-5.6.0/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/ode/__init__.py` & `pymc-5.6.0/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/ode/ode.py` & `pymc-5.6.0/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/ode/utils.py` & `pymc-5.6.0/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/plots/__init__.py` & `pymc-5.6.0/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/printing.py` & `pymc-5.6.0/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/pytensorf.py` & `pymc-5.6.0/pymc/pytensorf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1224,7 +1224,14 @@
 
     if raise_not_constant and not all(isinstance(folded_x, Constant) for folded_x in folded_xs):
         raise NotConstantValueError
 
     return tuple(
         folded_x.data if isinstance(folded_x, Constant) else folded_x for folded_x in folded_xs
     )
+
+
+def rewrite_pregrad(graph):
+    """Apply simplifying or stabilizing rewrites to graph that are safe to use
+    pre-grad.
+    """
+    return rewrite_graph(graph, include=("canonicalize", "stabilize"))
```

### Comparing `pymc-5.5.0/pymc/sampling/__init__.py` & `pymc-5.6.0/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/sampling/forward.py` & `pymc-5.6.0/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/sampling/jax.py` & `pymc-5.6.0/pymc/sampling/jax.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,14 @@
     model: Optional[Model] = None,
     var_names: Optional[Sequence[str]] = None,
     keep_untransformed: bool = False,
     chain_method: str = "parallel",
     postprocessing_backend: Optional[str] = None,
     postprocessing_chunks: Optional[int] = None,
     idata_kwargs: Optional[Dict[str, Any]] = None,
-    **kwargs,
 ) -> az.InferenceData:
     """
     Draw samples from the posterior using the NUTS method from the ``blackjax`` library.
 
     Parameters
     ----------
     draws : int, default 1000
@@ -526,15 +525,14 @@
     progressbar: bool = True,
     keep_untransformed: bool = False,
     chain_method: str = "parallel",
     postprocessing_backend: Optional[str] = None,
     postprocessing_chunks: Optional[int] = None,
     idata_kwargs: Optional[Dict] = None,
     nuts_kwargs: Optional[Dict] = None,
-    **kwargs,
 ) -> az.InferenceData:
     """
     Draw samples from the posterior using the NUTS method from the ``numpyro`` library.
 
     Parameters
     ----------
     draws : int, default 1000
```

### Comparing `pymc-5.5.0/pymc/sampling/mcmc.py` & `pymc-5.6.0/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/sampling/parallel.py` & `pymc-5.6.0/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/sampling/population.py` & `pymc-5.6.0/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/sampling_jax.py` & `pymc-5.6.0/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/smc/__init__.py` & `pymc-5.6.0/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/smc/kernels.py` & `pymc-5.6.0/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/smc/sampling.py` & `pymc-5.6.0/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/stats/__init__.py` & `pymc-5.6.0/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/stats/convergence.py` & `pymc-5.6.0/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/stats/log_likelihood.py` & `pymc-5.6.0/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/__init__.py` & `pymc-5.6.0/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/arraystep.py` & `pymc-5.6.0/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/compound.py` & `pymc-5.6.0/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.6.0/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.6.0/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.6.0/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/integration.py` & `pymc-5.6.0/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.6.0/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.6.0/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/metropolis.py` & `pymc-5.6.0/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/slicer.py` & `pymc-5.6.0/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/step_methods/step_sizes.py` & `pymc-5.6.0/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/testing.py` & `pymc-5.6.0/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/tuning/__init__.py` & `pymc-5.6.0/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/tuning/scaling.py` & `pymc-5.6.0/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/tuning/starting.py` & `pymc-5.6.0/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/util.py` & `pymc-5.6.0/pymc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import xarray
 
 from cachetools import LRUCache, cachedmethod
 from pytensor import Variable
 from pytensor.compile import SharedVariable
 from pytensor.graph.utils import ValidatingScratchpad
 
+from pymc.exceptions import BlockModelAccessError
+
 
 class _UnsetType:
     """Type for the `UNSET` object to make it look nice in `help(...)` outputs."""
 
     def __str__(self):
         return "UNSET"
 
@@ -246,15 +248,15 @@
     stacked_dims = {dim_name: ds[dim_name] for dim_name in sample_dims}
     ds = ds.transpose(*sample_dims, ...)
     stacked_dict = {
         vn: da.values.reshape((-1, *da.shape[num_sample_dims:])) for vn, da in ds.items()
     }
     points = [
         {vn: stacked_dict[vn][i, ...] for vn in var_names}
-        for i in range(np.product([len(coords) for coords in stacked_dims.values()]))
+        for i in range(np.prod([len(coords) for coords in stacked_dims.values()]))
     ]
     # use the list of points
     return cast(List[Dict[str, np.ndarray]], points), stacked_dims
 
 
 def drop_warning_stat(idata: arviz.InferenceData) -> arviz.InferenceData:
     """Returns a new ``InferenceData`` object with the "warning" stat removed from sample stats groups.
@@ -363,15 +365,15 @@
 
 def check_dist_not_registered(dist, model=None):
     """Check that a dist is not registered in the model already"""
     from pymc.model import modelcontext
 
     try:
         model = modelcontext(None)
-    except TypeError:
+    except (TypeError, BlockModelAccessError):
         pass
     else:
         if dist in model.basic_RVs:
             raise ValueError(
                 f"The dist {dist} was already registered in the current model.\n"
                 f"You should use an unregistered (unnamed) distribution created via "
                 f"the `.dist()` API instead, such as:\n`dist=pm.Normal.dist(0, 1)`"
```

### Comparing `pymc-5.5.0/pymc/variational/__init__.py` & `pymc-5.6.0/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/approximations.py` & `pymc-5.6.0/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/callbacks.py` & `pymc-5.6.0/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/inference.py` & `pymc-5.6.0/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/minibatch_rv.py` & `pymc-5.6.0/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/operators.py` & `pymc-5.6.0/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/opvi.py` & `pymc-5.6.0/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/stein.py` & `pymc-5.6.0/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/test_functions.py` & `pymc-5.6.0/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/variational/updates.py` & `pymc-5.6.0/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc/vartypes.py` & `pymc-5.6.0/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/pymc.egg-info/PKG-INFO` & `pymc-5.6.0/pymc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.5.0
+Version: 5.6.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -157,14 +157,16 @@
         
         |NumFOCUS|
         
         |PyMCLabs|
         
         |Mistplay|
         
+        |ODSC|
+        
         .. |Binder| image:: https://mybinder.org/badge_logo.svg
            :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
         .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
            :target: https://github.com/pymc-devs/pymc/actions
         .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
            :target: https://codecov.io/gh/pymc-devs/pymc
         .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
@@ -173,14 +175,16 @@
            :target: http://www.numfocus.org/
         .. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
            :target: http://www.numfocus.org/
         .. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
            :target: https://pymc-labs.io
         .. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
            :target: https://www.mistplay.com/
+        .. |ODSC| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/odsc/sponsor_odsc.png?raw=true
+           :target: https://odsc.com/california/?utm_source=pymc&utm_medium=referral
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pymc-5.5.0/pymc.egg-info/SOURCES.txt` & `pymc-5.6.0/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/scripts/docker_container.sh` & `pymc-5.6.0/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/setup.py` & `pymc-5.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.5.0/versioneer.py` & `pymc-5.6.0/versioneer.py`

 * *Files identical despite different names*

