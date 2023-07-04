# Comparing `tmp/mne-bids-pipeline-1.3.0.tar.gz` & `tmp/mne-bids-pipeline-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-bids-pipeline-1.3.0.tar", last modified: Thu Jun  1 14:51:09 2023, max compression
+gzip compressed data, was "mne-bids-pipeline-1.4.0.tar", last modified: Tue Jul  4 08:15:53 2023, max compression
```

## Comparing `mne-bids-pipeline-1.3.0.tar` & `mne-bids-pipeline-1.4.0.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.875825 mne-bids-pipeline-1.3.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.circleci/config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.circleci/setup_bash.sh
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.875825 mne-bids-pipeline-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/circleci-redirector.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/BUILDING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/build-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97580 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/assets/mne.svg
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/changes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/doc-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10313 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/examples/gen_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/features/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/features/gen_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/features/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/freesurfer.md
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/governance.md
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/general.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.887825 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/artifacts.md
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/autobads.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/breaks.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/epochs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/filter.md
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/maxfilter.md
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/resample.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/ssp_ica.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/stim_artifact.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.887825 mne-bids-pipeline-1.3.0/docs/source/settings/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/reports/report_generation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.891825 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/contrasts.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/group_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/mvpa.md
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/time_freq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.891825 mne-bids-pipeline-1.3.0/docs/source/settings/source/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/bem.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/forward.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/general.md
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/inverse.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/tags.md
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.0.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.1.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.2.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.3.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.895825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69107 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7776 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.903825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/README
--rwxr-xr-x   0 runner    (1001) docker     (123)    32882 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.903825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.907825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.907825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    24358 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_99_group_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.911825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_04_make_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_05_make_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_99_group_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.915825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000117.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000246.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000247.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_FLASH_BEM.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_T1_BEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_coreg_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds001810.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds001971.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003104.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003392.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003775.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004107.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004229.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_eeg_matchingpennies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/ds000247_scans.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/ds001971_participants.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/freesurfer-license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_documented.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.680959 mne-bids-pipeline-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.660959 mne-bids-pipeline-1.4.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    40224 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.circleci/config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.circleci/setup_bash.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.660959 mne-bids-pipeline-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.github/workflows/circleci-redirector.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/BUILDING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-04 08:15:53.680959 mne-bids-pipeline-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/build-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    97580 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/assets/mne.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/changes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/doc-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10313 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/examples/gen_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/features/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/features/gen_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/features/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/getting_started/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/getting_started/freesurfer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/getting_started/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/governance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.664959 mne-bids-pipeline-1.4.0/docs/source/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/general.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.668959 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/artifacts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/autobads.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/breaks.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/epochs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/filter.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/maxfilter.md
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/resample.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/ssp_ica.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/stim_artifact.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.668959 mne-bids-pipeline-1.4.0/docs/source/settings/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/reports/report_generation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.668959 mne-bids-pipeline-1.4.0/docs/source/settings/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/sensor/contrasts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/sensor/group_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/sensor/mvpa.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/sensor/time_freq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.668959 mne-bids-pipeline-1.4.0/docs/source/settings/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/source/bem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/source/forward.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/source/general.md
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/settings/source/inverse.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/tags.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/v1.0.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/v1.1.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/v1.2.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/v1.3.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/docs/source/v1.4.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.668959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71506 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7859 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40500 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32882 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_02_head_pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_03_maxfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_04_frequency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_05_make_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_06a_run_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_06b_run_ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_07a_apply_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_07b_apply_ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_08_ptp_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.676959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19872 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24202 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_99_group_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.676959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_04_make_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_05_make_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_99_group_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.676959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.680959 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000117.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000246.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000247.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_FLASH_BEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_T1_BEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_coreg_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds001810.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds001971.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds003104.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds003392.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds003775.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds004107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds004229.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_eeg_matchingpennies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/ds000247_scans.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/ds001971_participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/freesurfer-license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_documented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:15:53.672959 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 08:15:53.000000 mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-04 08:15:32.000000 mne-bids-pipeline-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:15:53.680959 mne-bids-pipeline-1.4.0/setup.cfg
```

### Comparing `mne-bids-pipeline-1.3.0/.circleci/config.yml` & `mne-bids-pipeline-1.4.0/.circleci/config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             fi
       - checkout
       - bash_env
       - run:
           name: Get Python running
           command: |
             pip install --upgrade --progress-bar off pip setuptools
-            pip install --upgrade --progress-bar off "autoreject @ https://api.github.com/repos/autoreject/autoreject/zipball/master" "mne[hdf5] @ git+https://github.com/mne-tools/mne-python" "mne-bids[full] @ https://api.github.com/repos/mne-tools/mne-bids/zipball/main"
+            pip install --upgrade --progress-bar off "autoreject @ https://api.github.com/repos/autoreject/autoreject/zipball/master" "mne[hdf5] @ git+https://github.com/mne-tools/mne-python" "mne-bids[full] @ https://api.github.com/repos/mne-tools/mne-bids/zipball/main" numba
             pip install -ve .[tests]
             pip install PyQt6
       - run:
           name: Check Qt
           command: |
             wget -q https://raw.githubusercontent.com/mne-tools/mne-python/main/tools/check_qt_import.sh
             bash check_qt_import.sh PyQt6
@@ -398,14 +398,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ds001971/*/*/*.html
 
   test_ds004107:
     <<: *imageconfig
+    resource_class: large  # memory
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ds004107-2
@@ -663,14 +664,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ds000248_no_mri/*/*/*.html
 
   test_ds001810:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ds001810-2
@@ -763,14 +765,15 @@
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ds003392/*/*/*.html
             - mne_data/derivatives/mne-bids-pipeline/ds003392/*/*/*.json
             - mne_data/derivatives/mne-bids-pipeline/ds003392/*/*/*.tsv
 
   test_ds004229:
     <<: *imageconfig
+    resource_class: large  # head position estimation
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ds004229-2
@@ -831,14 +834,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/eeg_matchingpennies/*/*/*.html
 
   test_ERP_CORE_N400:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -871,14 +875,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_ERN:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -906,14 +911,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_LRP:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -941,14 +947,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_MMN:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -976,14 +983,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_N2pc:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -1011,14 +1019,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_N170:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
@@ -1046,14 +1055,15 @@
       - persist_to_workspace:
           root: ~/
           paths:
             - mne_data/derivatives/mne-bids-pipeline/ERP_CORE/*/*/*/*.html
 
   test_ERP_CORE_P3:
     <<: *imageconfig
+    resource_class: large
     steps:
       - attach_workspace:
           at: ~/
       - bash_env
       - restore_cache:
           keys:
             - data-cache-ERP_CORE-1
```

### Comparing `mne-bids-pipeline-1.3.0/.circleci/setup_bash.sh` & `mne-bids-pipeline-1.4.0/.circleci/setup_bash.sh`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/.github/config.yml` & `mne-bids-pipeline-1.4.0/.github/config.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/.github/workflows/release.yml` & `mne-bids-pipeline-1.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/.github/workflows/run-tests.yml` & `mne-bids-pipeline-1.4.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/CONTRIBUTING.md` & `mne-bids-pipeline-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/LICENSE.txt` & `mne-bids-pipeline-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/Makefile` & `mne-bids-pipeline-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/PKG-INFO` & `mne-bids-pipeline-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-bids-pipeline
-Version: 1.3.0
+Version: 1.4.0
 Summary: A full-flegded processing pipeline for your MEG and EEG data
 Author: Eric Larson, Alexandre Gramfort, Mainak Jas
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License: Copyright © 2019-2022, authors of MNE-BIDS-Pipeline
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne-bids-pipeline-1.3.0/README.md` & `mne-bids-pipeline-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/codecov.yml` & `mne-bids-pipeline-1.4.0/codecov.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/hooks.py` & `mne-bids-pipeline-1.4.0/docs/hooks.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/mkdocs.yml` & `mne-bids-pipeline-1.4.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/assets/favicon.ico` & `mne-bids-pipeline-1.4.0/docs/source/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/assets/mne.svg` & `mne-bids-pipeline-1.4.0/docs/source/assets/mne.svg`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/css/extra.css` & `mne-bids-pipeline-1.4.0/docs/source/css/extra.css`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/examples/gen_examples.py` & `mne-bids-pipeline-1.4.0/docs/source/examples/gen_examples.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/features/gen_steps.py` & `mne-bids-pipeline-1.4.0/docs/source/features/gen_steps.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/features/overview.md` & `mne-bids-pipeline-1.4.0/docs/source/features/overview.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/getting_started/basic_usage.md` & `mne-bids-pipeline-1.4.0/docs/source/getting_started/basic_usage.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/getting_started/freesurfer.md` & `mne-bids-pipeline-1.4.0/docs/source/getting_started/freesurfer.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/getting_started/install.md` & `mne-bids-pipeline-1.4.0/docs/source/getting_started/install.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/index.md` & `mne-bids-pipeline-1.4.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/general.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/general.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         - data_type
         - eog_channels
         - eeg_bipolar_channels
         - eeg_reference
         - eeg_template_montage
         - drop_channels
         - reader_extra_params
+        - read_raw_bids_verbose
         - analyze_channels
         - plot_psd_for_runs
         - n_jobs
         - parallel_backend
         - dask_open_dashboard
         - dask_temp_dir
         - dask_worker_memory_limit
```

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/autobads.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/autobads.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/epochs.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/epochs.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/filter.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/filter.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/resample.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/resample.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/ssp_ica.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/preprocessing/ssp_ica.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         - n_proj_eog
         - n_proj_ecg
         - ssp_meg
         - ecg_proj_from_average
         - eog_proj_from_average
         - ssp_reject_eog
         - ssp_reject_ecg
+        - ssp_ecg_channel
         - ica_reject
         - ica_algorithm
         - ica_l_freq
         - ica_max_iterations
         - ica_n_components
         - ica_decim
         - ica_ctps_ecg_threshold
```

### Comparing `mne-bids-pipeline-1.3.0/docs/source/settings/sensor/mvpa.md` & `mne-bids-pipeline-1.4.0/docs/source/settings/sensor/mvpa.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/v1.0.md.inc` & `mne-bids-pipeline-1.4.0/docs/source/v1.0.md.inc`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/docs/source/v1.3.md.inc` & `mne-bids-pipeline-1.4.0/docs/source/v1.3.md.inc`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## v1.3.0 (unreleased)
+## v1.3.0 (released 2023/06/01)
 
 ### :new: New features & enhancements
 
 - Provide a more helpful log message if the CSP decoding step is being skipped (#734 by @hoechenberger)
 - Use `rich` for improved logging control and styling (#737 by @larsoner)
 
 [//]: # (- Whatever (#000 by @whoever))
@@ -11,12 +11,12 @@
 
 [//]: # (- Whatever (#000 by @whoever))
 
 ### :medical_symbol: Code health
 
 - Avoid using deprecated `openpyxl` API when working with Excel spreadsheets (#735 by @larsoner)
 
-### :bug: Bug fixes)
+### :bug: Bug fixes
 
 - Fix pandas 2.0 compatibility (#732 by @larsoner)
 - Fix bug with `mne.sys_info` insertion in reports (#732 by @larsoner)
 - Always generate CSP decdoing grand average analysis if CSP decoding was used on the single-subject level (#733 by @hoechenberger)
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,26 +200,23 @@
 covariance (via `noise_cov='rest'`).
 """
 
 ch_types: Iterable[Literal["meg", "mag", "grad", "eeg"]] = []
 """
 The channel types to consider.
 
-!!! info
-    Currently, MEG and EEG data cannot be processed together.
-
 ???+ example "Example"
     ```python
     # Use EEG channels:
     ch_types = ['eeg']
 
     # Use magnetometer and gradiometer MEG channels:
     ch_types = ['mag', 'grad']
 
-    # Currently does not work and will raise an error message:
+    # Use MEG and EEG channels:
     ch_types = ['meg', 'eeg']
     ```
 """
 
 data_type: Optional[Literal["meg", "eeg"]] = None
 """
 The BIDS data type.
@@ -231,15 +228,15 @@
 
 ???+ example "Example"
     The dataset contains simultaneous recordings of MEG and EEG, and we only
     wish to process the EEG data, which is stored inside the MEG files:
 
     ```python
     ch_types = ['eeg']
-    data_type = 'eeg'
+    data_type = 'meg'
     ```
 
     The dataset contains simultaneous recordings of MEG and EEG, and we only
     wish to process the gradiometer data:
 
     ```python
     ch_types = ['grad']
@@ -415,14 +412,22 @@
 ???+ example "Example"
     Enforce units for EDF files:
     ```python
     reader_extra_params = {"units": "uV"}
     ```
 """
 
+read_raw_bids_verbose: Optional[Literal["error"]] = None
+"""
+Verbosity level to pass to `read_raw_bids(..., verbose=read_raw_bids_verbose)`.
+If you know your dataset will contain files that are not perfectly BIDS
+compliant (e.g., "Did not find any meg.json..."), you can set this to
+`'error'` to suppress warnings emitted by read_raw_bids.
+"""
+
 ###############################################################################
 # BREAK DETECTION
 # ---------------
 
 find_breaks: bool = False
 """
 During an experimental run, the recording might be interrupted by breaks of
@@ -575,14 +580,24 @@
 ???+ example "Example"
     ```python
     mf_st_duration = None
     mf_st_duration = 10.  # to apply tSSS with 0.1Hz highpass filter.
     ```
 """
 
+mf_st_correlation: float = 0.98
+"""
+The correlation limit for spatio-temporal SSS (tSSS).
+
+???+ example "Example"
+    ```python
+    st_correlation = 0.98
+    ```
+"""
+
 mf_head_origin: Union[Literal["auto"], ArrayLike] = "auto"
 """
 `mf_head_origin` : array-like, shape (3,) | 'auto'
 Origin of internal and external multipolar moment space in meters.
 If 'auto', it will be estimated from headshape points.
 If automatic fitting fails (e.g., due to having too few digitization
 points), consider separately calling the fitting function with different
@@ -590,25 +605,50 @@
 
 ???+ example "Example"
     ```python
     mf_head_origin = 'auto'
     ```
 """
 
-mf_reference_run: Optional[str] = None
+mf_destination: Union[Literal["reference_run"], ArrayLike] = "reference_run"
 """
 Despite all possible care to avoid movements in the MEG, the participant
 will likely slowly drift down from the Dewar or slightly shift the head
 around in the course of the recording session. Hence, to take this into
-account, we are realigning all data to a single position. For this, you need
-to define a reference run (typically the one in the middle of
-the recording session).
+account, we are realigning all data to a single position. For this, you can:
+
+1. Choose a reference run. Often one from the middle of the recording session
+   is a good choice. Set `mf_destination = "reference_run" and then set
+   [`config.mf_reference_run`](mne_bids_pipeline._config.mf_reference_run).
+   This will result in a device-to-head transformation that differs between
+   subjects.
+2. Choose a standard position in the MEG coordinate frame. For this, pass
+   a 4x4 transformation matrix for the device-to-head
+   transform. This will result in a device-to-head transformation that is
+   the same across all subjects.
+
+   ???+ example "A Standardized Position"
+   ```python
+   from mne.transforms import translation
+   mf_destination = translation(z=0.04)
+   ```
+"""
+
+mf_int_order: int = 8
+"""
+Internal order for the Maxwell basis. Can be set to something lower (e.g., 6
+or higher for datasets where lower or higher spatial complexity, respectively,
+is expected.
+"""
 
+mf_reference_run: Optional[str] = None
+"""
 Which run to take as the reference for adjusting the head position of all
-runs. If `None`, pick the first run.
+runs when [`mf_destination="reference_run"`](mne_bids_pipeline._config.mf_destination).
+If `None`, pick the first run.
 
 ???+ example "Example"
     ```python
     mf_reference_run = '01'  # Use run "01"
     ```
 """
 
@@ -637,14 +677,47 @@
      [according to BIDS](https://bids-specification.readthedocs.io/en/stable/99-appendices/06-meg-file-formats.html#cross-talk-and-fine-calibration-files).
 ???+ example "Example"
     ```python
     mf_ctc_fname = '/path/to/your/file/crosstalk_ct.fif'
     ```
 """  # noqa : E501
 
+mf_mc: bool = False
+"""
+If True, perform movement compensation on the data.
+"""
+
+mf_mc_t_step_min: float = 0.01
+"""
+Minimum time step to use during cHPI coil amplitude estimation.
+"""
+
+mf_mc_t_window: Union[float, Literal["auto"]] = "auto"
+"""
+The window to use during cHPI coil amplitude estimation and in cHPI filtering.
+Can be "auto" to autodetect a reasonable value or a float (in seconds).
+"""
+
+mf_mc_gof_limit: float = 0.98
+"""
+Minimum goodness of fit to accept for each cHPI coil.
+"""
+
+mf_mc_dist_limit: float = 0.005
+"""
+Minimum distance (m) to accept for cHPI position fitting.
+"""
+
+mf_filter_chpi: Optional[bool] = None
+"""
+Use mne.chpi.filter_chpi after Maxwell filtering. Can be None to use
+the same value as [`mf_mc`][mne_bids_pipeline._config.mf_mc].
+Only used when [`use_maxwell_filter=True`][mne_bids_pipeline._config.use_maxwell_filter]
+"""  # noqa: E501
+
 ###############################################################################
 # STIMULATION ARTIFACT
 # --------------------
 # used in 01-import_and_maxfilter.py
 
 fix_stim_artifact: bool = False
 """
@@ -1124,14 +1197,20 @@
     ```python
     ssp_reject_eog = {'grad': 10e-10, 'mag': 20e-12, 'eeg': 400e-6}
     ssp_reject_eog = {'grad': 15e-10}
     ssp_reject_eog = None
     ```
 """
 
+ssp_ecg_channel: Optional[str] = None
+"""
+Channel to use for ECG SSP. Can be useful when the autodetected ECG channel
+is not reliable.
+"""
+
 # Rejection based on ICA
 # ~~~~~~~~~~~~~~~~~~~~~~
 ica_reject: Optional[Dict[str, float]] = None
 """
 Peak-to-peak amplitude limits to exclude epochs from ICA fitting.
 
 This allows you to remove strong transient artifacts, which could negatively
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_import.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib
 import os
 import pathlib
 from types import SimpleNamespace
 from typing import Optional, List
 
 import matplotlib
+import numpy as np
 import mne
 from mne.utils import _check_option, _validate_type
 
 from ._logging import logger, gen_log_kwargs
 from .typing import PathLike
 
 
@@ -339,14 +340,33 @@
 
     _check_option(
         "config.config_validation",
         config.config_validation,
         ("raise", "warn", "ignore"),
     )
 
+    _validate_type(
+        config.mf_destination,
+        (str, list, tuple, np.ndarray),
+        "config.mf_destination",
+    )
+    if isinstance(config.mf_destination, str):
+        _check_option(
+            "config.mf_destination",
+            config.mf_destination,
+            ("reference_run",),
+        )
+    else:
+        destination = np.array(config.mf_destination, float)
+        if destination.shape != (4, 4):
+            raise ValueError(
+                "config.mf_destination, if array-like, must have shape (4, 4) "
+                f"but got shape {destination.shape}"
+            )
+
 
 _REMOVED_NAMES = {
     "debug": dict(
         new_name="on_error",
         instead='use on_error="debug" instead',
     ),
     "decim": dict(
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_template.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_template.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_utils.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_config_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,36 +114,45 @@
 
     if not sessions:
         return [None]
     else:
         return sessions
 
 
-@functools.lru_cache(maxsize=None)
-def _get_runs_all_subjects_cached(
-    **config_dict: Dict[str, Any],
-) -> Dict[str, Union[List[None], List[str]]]:
-    config = SimpleNamespace(**config_dict)
-    # Sometimes we check list equivalence for ch_types, so convert it back
-    config.ch_types = list(config.ch_types)
-    return get_runs_all_subjects(config)
-
-
 def get_runs_all_subjects(
     config: SimpleNamespace,
 ) -> Dict[str, Union[List[None], List[str]]]:
     """Gives the mapping between subjects and their runs.
 
     Returns
     -------
     a dict of runs present in the bids_path
     for each subject asked in the configuration file
     (and not for each subject present in the bids_path).
     """
-    # We cannot use get_subjects() because if there is just one subject
+    # Use caching under the hood for speed
+    return copy.deepcopy(
+        _get_runs_all_subjects_cached(
+            bids_root=config.bids_root,
+            data_type=config.data_type,
+            ch_types=tuple(config.ch_types),
+            subjects=tuple(config.subjects) if config.subjects != "all" else "all",
+            exclude_subjects=tuple(config.exclude_subjects),
+            exclude_runs=tuple(config.exclude_runs) if config.exclude_runs else None,
+        )
+    )
+
+
+@functools.lru_cache(maxsize=None)
+def _get_runs_all_subjects_cached(
+    **config_dict: Dict[str, Any],
+) -> Dict[str, Union[List[None], List[str]]]:
+    config = SimpleNamespace(**config_dict)
+    # Sometimes we check list equivalence for ch_types, so convert it back
+    config.ch_types = list(config.ch_types)
     subj_runs = dict()
     for subject in get_subjects(config):
         # Only traverse through the current subject's directory
         valid_runs_subj = _get_entity_vals_cached(
             config.bids_root / f"sub-{subject}",
             entity_key="run",
             ignore_datatypes=_get_ignore_datatypes(config),
@@ -166,15 +175,18 @@
 def get_intersect_run(config: SimpleNamespace) -> List[str]:
     """Returns the intersection of all the runs of all subjects."""
     subj_runs = get_runs_all_subjects(config)
     return list(set.intersection(*map(set, subj_runs.values())))
 
 
 def get_runs(
-    *, config: SimpleNamespace, subject: str, verbose: bool = False
+    *,
+    config: SimpleNamespace,
+    subject: str,
+    verbose: bool = False,
 ) -> Union[List[str], List[None]]:
     """Returns a list of runs in the BIDS input data.
 
     Parameters
     ----------
     subject
         Returns a list of the runs of this subject.
@@ -186,23 +198,15 @@
     The list of runs of the subject. If no BIDS `run` entity could be found,
     returns `[None]`.
     """
     if subject == "average":  # Used when creating the report
         return [None]
 
     runs = copy.deepcopy(config.runs)
-
-    subj_runs = _get_runs_all_subjects_cached(
-        bids_root=config.bids_root,
-        data_type=config.data_type,
-        ch_types=tuple(config.ch_types),
-        subjects=tuple(config.subjects) if config.subjects != "all" else "all",
-        exclude_subjects=tuple(config.exclude_subjects),
-        exclude_runs=tuple(config.exclude_runs) if config.exclude_runs else None,
-    )
+    subj_runs = get_runs_all_subjects(config=config)
     valid_runs = subj_runs[subject]
 
     if len(get_subjects(config)) > 1:
         # Notify if different subjects do not share the same runs
 
         same_runs = True
         for runs_sub_i in subj_runs.values():
@@ -214,25 +218,55 @@
                 "Extracted all the runs. "
                 "Beware, not all subjects share the same "
                 "set of runs."
             )
             logger.info(**gen_log_kwargs(message=msg))
 
     if runs == "all":
-        runs = valid_runs
+        runs = list(valid_runs)
 
     if not runs:
-        return [None]
+        runs = [None]
     else:
         inclusion = set(runs).issubset(set(valid_runs))
         if not inclusion:
             raise ValueError(
                 f"Invalid run. It can be a subset of {valid_runs} but " f"got {runs}"
             )
-        return runs
+    return runs
+
+
+def get_runs_tasks(
+    *,
+    config: SimpleNamespace,
+    subject: str,
+    session: Optional[str],
+    include_noise: bool = True,
+) -> List[Tuple[str]]:
+    """Get (run, task) tuples for all runs plus (maybe) rest."""
+    from ._import_data import _get_noise_path, _get_rest_path
+
+    runs = get_runs(config=config, subject=subject)
+    tasks = [get_task(config=config)] * len(runs)
+    kwargs = dict(
+        cfg=config,
+        subject=subject,
+        session=session,
+        kind="orig",
+        add_bads=False,
+    )
+    if _get_rest_path(**kwargs):
+        runs.append(None)
+        tasks.append("rest")
+    if include_noise:
+        mf_reference_run = get_mf_reference_run(config=config)
+        if _get_noise_path(mf_reference_run=mf_reference_run, **kwargs):
+            runs.append(None)
+            tasks.append("noise")
+    return tuple(zip(runs, tasks))
 
 
 def get_mf_reference_run(config: SimpleNamespace) -> str:
     # Retrieve to run identifier (number, name) of the reference run
     if config.mf_reference_run is not None:
         return config.mf_reference_run
     # Use the first run
@@ -553,7 +587,25 @@
         STEP_MODULES["init"]
         + STEP_MODULES["preprocessing"]
         + STEP_MODULES["sensor"]
         + STEP_MODULES["source"]
     )
 
     return STEP_MODULES
+
+
+def _bids_kwargs(*, config: SimpleNamespace) -> dict:
+    """Get the standard BIDS config entries."""
+    return dict(
+        proc=config.proc,
+        task=get_task(config),
+        datatype=get_datatype(config),
+        acq=config.acq,
+        rec=config.rec,
+        space=config.space,
+        bids_root=config.bids_root,
+        deriv_root=config.deriv_root,
+    )
+
+
+def _do_mf_autobad(*, cfg: SimpleNamespace) -> bool:
+    return cfg.find_noisy_channels_meg or cfg.find_flat_channels_meg
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_decoding.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_decoding.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_download.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_download.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_import_data.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_import_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from types import SimpleNamespace
 from typing import Dict, Optional, Iterable, Union, List, Literal
 
 import mne
+from mne.utils import _pl
 from mne_bids import BIDSPath, read_raw_bids, get_bids_path_from_fname
 import numpy as np
 import pandas as pd
 
+from ._config_utils import (
+    get_mf_reference_run,
+    get_runs,
+    get_datatype,
+    get_task,
+    _bids_kwargs,
+    _do_mf_autobad,
+)
 from ._io import _read_json, _empty_room_match_path
 from ._logging import gen_log_kwargs, logger
 from ._run import _update_for_splits
 from .typing import PathLike
 
 
 def make_epochs(
@@ -210,15 +219,19 @@
 def _load_data(cfg: SimpleNamespace, bids_path: BIDSPath) -> mne.io.BaseRaw:
     # read_raw_bids automatically
     # - populates bad channels using the BIDS channels.tsv
     # - sets channels types according to BIDS channels.tsv `type` column
     # - sets raw.annotations using the BIDS events.tsv
 
     subject = bids_path.subject
-    raw = read_raw_bids(bids_path=bids_path, extra_params=cfg.reader_extra_params)
+    raw = read_raw_bids(
+        bids_path=bids_path,
+        extra_params=cfg.reader_extra_params,
+        verbose=cfg.read_raw_bids_verbose,
+    )
 
     _crop_data(cfg, raw=raw, subject=subject)
 
     raw.load_data()
     if hasattr(raw, "fix_mag_coil_types"):
         raw.fix_mag_coil_types()
 
@@ -364,30 +377,37 @@
     raw
         The imported data.
     """
     subject = bids_path_in.subject
     session = bids_path_in.session
     run = bids_path_in.run
 
+    # 1. _load_data (_crop_data)
     raw = _load_data(cfg=cfg, bids_path=bids_path_in)
+    # 2. _set_eeg_montage
     _set_eeg_montage(cfg=cfg, raw=raw, subject=subject, session=session, run=run)
+    # 3. _create_bipolar_channels
     _create_bipolar_channels(
         cfg=cfg, raw=raw, subject=subject, session=session, run=run
     )
+    # 4. _drop_channels_func
     _drop_channels_func(cfg=cfg, raw=raw, subject=subject, session=session)
+    # 5. _find_breaks_func
     _find_breaks_func(cfg=cfg, raw=raw, subject=subject, session=session, run=run)
     if data_is_rest is None:
         data_is_rest = (cfg.task == "rest") or cfg.task_is_rest
     if not data_is_rest:
+        # 6. _rename_events_func
         _rename_events_func(cfg=cfg, raw=raw, subject=subject, session=session, run=run)
+        # 7. _fix_stim_artifact_func
         _fix_stim_artifact_func(cfg=cfg, raw=raw)
 
     if bids_path_bads_in is not None:
         bads = _read_bads_tsv(cfg=cfg, bids_path_bads=bids_path_bads_in)
-        msg = f"Marking {len(bads)} channels as bad."
+        msg = f"Marking {len(bads)} channel{_pl(bads)} as bad."
         logger.info(**gen_log_kwargs(message=msg))
         raw.info["bads"] = bads
         raw.info._check_consistency()
 
     return raw
 
 
@@ -432,15 +452,19 @@
     raw_er.pick_types(meg=True, exclude=[])
 
     # Don't deal with ref for now (initial data quality / auto bad step)
     if bids_path_ref_in is None:
         return raw_er
 
     # Load reference run plus its auto-bads
-    raw_ref = read_raw_bids(bids_path_ref_in, extra_params=cfg.reader_extra_params)
+    raw_ref = read_raw_bids(
+        bids_path_ref_in,
+        extra_params=cfg.reader_extra_params,
+        verbose=cfg.read_raw_bids_verbose,
+    )
     if bids_path_ref_bads_in is not None:
         bads = _read_bads_tsv(
             cfg=cfg,
             bids_path_bads=bids_path_ref_bads_in,
         )
         raw_ref.info["bads"] = bads
         raw_ref.info._check_consistency()
@@ -492,127 +516,213 @@
         f'{len(break_annots) if break_annots else "no"} break periods.'
     )
     logger.info(**gen_log_kwargs(message=msg))
 
     raw.set_annotations(raw.annotations + break_annots)  # add to existing
 
 
-def _get_raw_paths(
+def _get_bids_path_in(
     *,
     cfg: SimpleNamespace,
     subject: str,
     session: Optional[str],
     run: Optional[str],
-    kind: Literal["raw", "sss"],
-    add_bads: bool = True,
-    include_mf_ref: bool = True,
-) -> dict:
-    # Construct the basenames of the files we wish to load, and of the empty-
-    # room recording we wish to save.
-    # The basenames of the empty-room recording output file does not contain
-    # the "run" entity.
+    task: Optional[str],
+    kind: Literal["orig", "sss"] = "orig",
+) -> BIDSPath:
+    # b/c can be used before this is updated
     path_kwargs = dict(
         subject=subject,
         run=run,
         session=session,
-        task=cfg.task,
+        task=task or cfg.task,
         acquisition=cfg.acq,
         recording=cfg.rec,
         space=cfg.space,
-        datatype=cfg.datatype,
+        datatype=get_datatype(config=cfg),
         check=False,
     )
     if kind == "sss":
         path_kwargs["root"] = cfg.deriv_root
         path_kwargs["suffix"] = "raw"
         path_kwargs["extension"] = ".fif"
         path_kwargs["processing"] = "sss"
     else:
         assert kind == "orig", kind
         path_kwargs["root"] = cfg.bids_root
         path_kwargs["suffix"] = None
         path_kwargs["extension"] = None
         path_kwargs["processing"] = cfg.proc
     bids_path_in = BIDSPath(**path_kwargs)
+    return bids_path_in
 
-    in_files = dict()
-    key = f"raw_run-{run}"
-    in_files[key] = bids_path_in
-    _update_for_splits(in_files, key, single=True)
-    if add_bads:
-        _add_bads_file(
+
+def _get_run_path(
+    *,
+    cfg: SimpleNamespace,
+    subject: str,
+    session: Optional[str],
+    run: Optional[str],
+    task: Optional[str],
+    kind: Literal["orig", "sss"],
+    add_bads: Optional[bool] = None,
+    allow_missing: bool = False,
+    key: Optional[str] = None,
+) -> dict:
+    bids_path_in = _get_bids_path_in(
+        cfg=cfg,
+        subject=subject,
+        session=session,
+        run=run,
+        task=task,
+        kind=kind,
+    )
+    return _path_dict(
+        cfg=cfg,
+        bids_path_in=bids_path_in,
+        key=key,
+        add_bads=add_bads,
+        kind=kind,
+        allow_missing=allow_missing,
+    )
+
+
+def _get_rest_path(
+    *,
+    cfg: SimpleNamespace,
+    subject: str,
+    session: Optional[str],
+    kind: Literal["orig", "sss"],
+    add_bads: Optional[bool] = None,
+) -> dict:
+    if not (cfg.process_rest and not cfg.task_is_rest):
+        return dict()
+    return _get_run_path(
+        cfg=cfg,
+        subject=subject,
+        session=session,
+        run=None,
+        task="rest",
+        kind=kind,
+        add_bads=add_bads,
+        allow_missing=True,
+    )
+
+
+def _get_noise_path(
+    *,
+    cfg: SimpleNamespace,
+    subject: str,
+    session: Optional[str],
+    kind: Literal["orig", "sss"],
+    mf_reference_run: Optional[str],
+    add_bads: Optional[bool] = None,
+) -> dict:
+    if not (cfg.process_empty_room and get_datatype(config=cfg) == "meg"):
+        return dict()
+    if kind == "sss":
+        raw_fname = _get_bids_path_in(
             cfg=cfg,
-            in_files=in_files,
-            key=key,
+            subject=subject,
+            session=session,
+            run=None,
+            task="noise",
+            kind=kind,
         )
-    orig_key = key
-
-    if run == cfg.runs[0]:
-        do = dict(
-            rest=cfg.process_rest and not cfg.task_is_rest,
-            noise=cfg.process_empty_room and cfg.datatype == "meg",
+    else:
+        # This must match the logic of _02_find_empty_room.py
+        raw_fname = _get_bids_path_in(
+            cfg=cfg,
+            subject=subject,
+            session=session,
+            run=mf_reference_run,
+            task=get_task(config=cfg),
+            kind=kind,
         )
-        for task in ("rest", "noise"):
-            if not do[task]:
-                continue
-            key = f"raw_{task}"
-            if kind == "sss":
-                raw_fname = bids_path_in.copy().update(run=None, task=task)
-            else:
-                if task == "rest":
-                    raw_fname = bids_path_in.copy().update(run=None, task=task)
-                else:
-                    raw_fname = _read_json(_empty_room_match_path(bids_path_in, cfg))[
-                        "fname"
-                    ]
-                    if raw_fname is not None:
-                        raw_fname = get_bids_path_from_fname(raw_fname)
-            if raw_fname is None:
-                continue
-            in_files[key] = raw_fname
-            _update_for_splits(in_files, key, single=True, allow_missing=True)
-            if not in_files[key].fpath.exists():
-                in_files.pop(key)
-            elif add_bads:
-                _add_bads_file(
-                    cfg=cfg,
-                    in_files=in_files,
-                    key=key,
-                )
-            if include_mf_ref and task == "noise":
-                key = "raw_ref_run"
-                in_files[key] = (
-                    in_files[orig_key].copy().update(run=cfg.mf_reference_run)
-                )
-                _update_for_splits(in_files, key, single=True, allow_missing=True)
-                if not in_files[key].fpath.exists():
-                    in_files.pop(key)
-                elif add_bads:
-                    _add_bads_file(
-                        cfg=cfg,
-                        in_files=in_files,
-                        key=key,
-                    )
-
-    return in_files
+        raw_fname = _read_json(_empty_room_match_path(raw_fname, cfg))["fname"]
+        if raw_fname is None:
+            return dict()
+        raw_fname = get_bids_path_from_fname(raw_fname)
+    return _path_dict(
+        cfg=cfg,
+        bids_path_in=raw_fname,
+        add_bads=add_bads,
+        kind=kind,
+        allow_missing=True,
+    )
 
 
-def _add_bads_file(
+def _get_run_rest_noise_path(
     *,
     cfg: SimpleNamespace,
-    in_files: dict,
-    key: str,
-) -> None:
-    bids_path_in = in_files[key]
-    bads_tsv_fname = _bads_path(
+    subject: str,
+    session: Optional[str],
+    run: Optional[str],
+    task: Optional[str],
+    kind: Literal["orig", "sss"],
+    mf_reference_run: Optional[str],
+    add_bads: Optional[bool] = None,
+) -> dict:
+    kwargs = dict(
         cfg=cfg,
-        bids_path_in=bids_path_in,
+        subject=subject,
+        session=session,
+        kind=kind,
+        add_bads=add_bads,
+    )
+    if run is None and task in ("noise", "rest"):
+        if task == "noise":
+            return _get_noise_path(mf_reference_run=mf_reference_run, **kwargs)
+        else:
+            assert task == "rest"
+            return _get_rest_path(**kwargs)
+    else:
+        return _get_run_path(run=run, task=task, **kwargs)
+
+
+def _get_mf_reference_run_path(
+    cfg: SimpleNamespace,
+    subject: str,
+    session: Optional[str],
+    add_bads: bool,
+) -> dict:
+    return _get_run_path(
+        cfg=cfg,
+        subject=subject,
+        session=session,
+        run=cfg.mf_reference_run,
+        task=None,
+        kind="orig",
+        add_bads=add_bads,
+        key="raw_ref_run",
     )
-    if bads_tsv_fname.fpath.is_file():
-        in_files[f"{key}-bads"] = bads_tsv_fname
+
+
+def _path_dict(
+    *,
+    cfg: SimpleNamespace,
+    bids_path_in: BIDSPath,
+    add_bads: Optional[bool] = None,
+    kind: Literal["orig", "sss"],
+    allow_missing: bool,
+    key: Optional[str] = None,
+) -> dict:
+    if add_bads is None:
+        add_bads = kind == "orig" and _do_mf_autobad(cfg=cfg)
+    in_files = dict()
+    key = key or f"raw_task-{bids_path_in.task}_run-{bids_path_in.run}"
+    in_files[key] = bids_path_in
+    _update_for_splits(in_files, key, single=True, allow_missing=True)
+    if allow_missing and not in_files[key].fpath.exists():
+        return dict()
+    if add_bads:
+        bads_tsv_fname = _bads_path(cfg=cfg, bids_path_in=bids_path_in)
+        if bads_tsv_fname.fpath.is_file() or not allow_missing:
+            in_files[f"{key}-bads"] = bads_tsv_fname
+    return in_files
 
 
 def _auto_scores_path(
     *,
     cfg: SimpleNamespace,
     bids_path_in: BIDSPath,
 ) -> BIDSPath:
@@ -642,7 +752,53 @@
 def _read_bads_tsv(
     *,
     cfg: SimpleNamespace,
     bids_path_bads: BIDSPath,
 ) -> List[str]:
     bads_tsv = pd.read_csv(bids_path_bads.fpath, sep="\t", header=0)
     return bads_tsv[bads_tsv.columns[0]].tolist()
+
+
+def _import_data_kwargs(*, config: SimpleNamespace, subject: str) -> dict:
+    """Get config params needed for any raw data loading."""
+    return dict(
+        # import_experimental_data / general
+        process_empty_room=config.process_empty_room,
+        process_rest=config.process_rest,
+        task_is_rest=config.task_is_rest,
+        # _get_raw_paths, _get_noise_path
+        use_maxwell_filter=config.use_maxwell_filter,
+        mf_reference_run=get_mf_reference_run(config=config),
+        data_type=config.data_type,
+        # automatic add_bads
+        find_noisy_channels_meg=config.find_noisy_channels_meg,
+        find_flat_channels_meg=config.find_flat_channels_meg,
+        # 1. _load_data
+        reader_extra_params=config.reader_extra_params,
+        crop_runs=config.crop_runs,
+        read_raw_bids_verbose=config.read_raw_bids_verbose,
+        # 2. _set_eeg_montage
+        eeg_template_montage=config.eeg_template_montage,
+        # 3. _create_bipolar_channels
+        eeg_bipolar_channels=config.eeg_bipolar_channels,
+        ch_types=config.ch_types,
+        eog_channels=config.eog_channels,
+        # 4. _drop_channels_func
+        drop_channels=config.drop_channels,
+        # 5. _find_breaks_func
+        find_breaks=config.find_breaks,
+        min_break_duration=config.min_break_duration,
+        t_break_annot_start_after_previous_event=config.t_break_annot_start_after_previous_event,  # noqa:E501
+        t_break_annot_stop_before_next_event=config.t_break_annot_stop_before_next_event,  # noqa:E501
+        # 6. _rename_events_func
+        rename_events=config.rename_events,
+        on_rename_missing_events=config.on_rename_missing_events,
+        # 7. _fix_stim_artifact_func
+        fix_stim_artifact=config.fix_stim_artifact,
+        stim_artifact_tmin=config.stim_artifact_tmin,
+        stim_artifact_tmax=config.stim_artifact_tmax,
+        # args used for all runs that process raw (reporting / writing)
+        plot_psd_for_runs=config.plot_psd_for_runs,
+        _raw_split_size=config._raw_split_size,
+        runs=get_runs(config=config, subject=subject),  # XXX needs to accept session!
+        **_bids_kwargs(config=config),
+    )
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_io.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_io.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_logging.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
                 warning="bold magenta",
                 error="bold red",
             )
         )
         self.__console = rich.console.Console(**kwargs)
         return self.__console
 
+    def rule(self, title="", *, align="center"):
+        self.__console.rule(title=title, characters="─", style="rule.line", align=align)
+
     @property
     def level(self):
         return self._level
 
     @level.setter
     def level(self, level):
         level = int(level)
@@ -103,14 +106,15 @@
 
 def gen_log_kwargs(
     message: str,
     *,
     subject: Optional[Union[str, int]] = None,
     session: Optional[Union[str, int]] = None,
     run: Optional[Union[str, int]] = None,
+    task: Optional[str] = None,
     step: Optional[str] = None,
     emoji: str = "⏳️",
     box: str = "│ ",
 ) -> LogKwargsT:
     from ._run import _get_step_path, _short_step_path
 
     # Try to figure these out
@@ -118,14 +122,18 @@
     up_locals = stack[1].frame.f_locals
     if subject is None:
         subject = up_locals.get("subject", None)
     if session is None:
         session = up_locals.get("session", None)
     if run is None:
         run = up_locals.get("run", None)
+        if run is None:
+            task = task or up_locals.get("task", None)
+            if task in ("noise", "rest"):
+                run = task
     if step is None:
         step_path = _get_step_path(stack)
         if step_path:
             step = _short_step_path(_get_step_path())
         else:
             step = ""
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_main.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,17 +198,19 @@
     msg = f"Using configuration: {config}"
     logger.info(**gen_log_kwargs(message=msg, emoji="🧾", box="╶╴", step=""))
 
     config_imported = _import_config(
         config_path=config_path,
         overrides=overrides,
     )
-    for step_module in step_modules:
+    for si, step_module in enumerate(step_modules):
         start = time.time()
         step = _short_step_path(pathlib.Path(step_module.__file__))
+        if si == 0:
+            logger.rule()
         msg = "Now running  👇"
         logger.info(**gen_log_kwargs(message=msg, box="┌╴", emoji="🚀", step=step))
         step_module.main(config=config_imported)
         elapsed = time.time() - start
         hours, remainder = divmod(elapsed, 3600)
         hours = int(hours)
         minutes, seconds = divmod(remainder, 60)
@@ -217,7 +219,8 @@
         elapsed = f"{seconds}s"
         if minutes:
             elapsed = f"{minutes}m {elapsed}"
         if hours:
             elapsed = f"{hours}h {elapsed}"
         msg = f"Done running  👆 [{elapsed}]"
         logger.info(**gen_log_kwargs(message=msg, box="└╴", emoji="🎉", step=step))
+        logger.rule()
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_parallel.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_parallel.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_reject.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_reject.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_report.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from filelock import FileLock
 import matplotlib.transforms
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
 import mne
+from mne.io import BaseRaw
 from mne.utils import _pl
 from mne_bids import BIDSPath
 from mne_bids.stats import count_events
 
 from ._config_utils import sanitize_cond_name, get_subjects, _restrict_analyze_channels
 from ._decoding import _handle_csp_args
 from ._logging import logger, gen_log_kwargs
@@ -26,20 +27,21 @@
 def _open_report(
     *,
     cfg: SimpleNamespace,
     exec_params: SimpleNamespace,
     subject: str,
     session: Optional[str],
     run: Optional[str] = None,
+    task: Optional[str] = None,
 ):
     fname_report = BIDSPath(
         subject=subject,
         session=session,
         # Report is across all runs, but for logging purposes it's helpful
-        # to pass the run for gen_log_kwargs
+        # to pass the run and task for gen_log_kwargs
         run=None,
         task=cfg.task,
         acquisition=cfg.acq,
         recording=cfg.rec,
         space=cfg.space,
         extension=".h5",
         datatype=cfg.datatype,
@@ -1190,27 +1192,29 @@
 
 def _add_raw(
     *,
     cfg: SimpleNamespace,
     report: mne.report.Report,
     bids_path_in: BIDSPath,
     title: str,
+    tags: tuple = (),
+    raw: Optional[BaseRaw] = None,
 ):
     if bids_path_in.run is not None:
-        title += f", run {bids_path_in.run}"
+        title += f", run {repr(bids_path_in.run)}"
     elif bids_path_in.task in ("noise", "rest"):
-        title += f", run {bids_path_in.task}"
+        title += f", {bids_path_in.task}"
     plot_raw_psd = (
         cfg.plot_psd_for_runs == "all"
         or bids_path_in.run in cfg.plot_psd_for_runs
         or bids_path_in.task in cfg.plot_psd_for_runs
     )
     with mne.use_log_level("error"):
         report.add_raw(
-            raw=bids_path_in,
+            raw=raw or bids_path_in,
             title=title,
             butterfly=5,
             psd=plot_raw_psd,
-            tags=("raw", "filtered", f"run-{bids_path_in.run}"),
+            tags=("raw", f"run-{bids_path_in.run}") + tags,
             # caption=bids_path_in.basename,  # TODO upstream
             replace=True,
         )
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_run.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 def failsafe_run(
     get_input_fnames: Optional[Callable] = None,
     get_output_fnames: Optional[Callable] = None,
 ) -> Callable:
     def failsafe_run_decorator(func):
         @functools.wraps(func)  # Preserve "identity" of original function
-        def wrapper(*args, **kwargs):
+        def __mne_bids_pipeline_failsafe_wrapper__(*args, **kwargs):
+            __mne_bids_pipeline_step__ = pathlib.Path(inspect.getfile(func))  # noqa
             exec_params = kwargs["exec_params"]
             on_error = exec_params.on_error
             memory = ConditionalStepMemory(
                 exec_params=exec_params,
                 get_input_fnames=get_input_fnames,
                 get_output_fnames=get_output_fnames,
             )
@@ -64,50 +65,54 @@
                 }
                 message = (
                     f"A critical error occurred. " f"The error message was: {str(e)}"
                 )
                 log_info["success"] = False
                 log_info["error_message"] = str(e)
 
+                # Find the limit / step where the error occurred
+                step_dir = pathlib.Path(__file__).parent / "steps"
+                tb = traceback.extract_tb(e.__traceback__)
+                for fi, frame in enumerate(inspect.stack()):
+                    is_step = pathlib.Path(frame.filename).parent.parent == step_dir
+                    del frame
+                    if is_step:
+                        # omit everything before the "step" dir, which will
+                        # generally be stuff from this file and joblib
+                        tb = tb[-fi:]
+                        break
+                tb = "".join(traceback.format_list(tb))
+
                 if on_error == "abort":
-                    message += (
-                        "\n\nAborting pipeline run. The full traceback " "is:\n\n"
-                    )
-                    if sys.version_info >= (3, 10):
-                        message += "\n".join(traceback.format_exception(e))
-                    else:
-                        message += "\n".join(
-                            traceback.format_exception(
-                                etype=type(e), value=e, tb=e.__traceback__
-                            )
-                        )
+                    message += f"\n\nAborting pipeline run. The traceback is:\n\n{tb}"
+
                     if os.getenv("_MNE_BIDS_STUDY_TESTING", "") == "true":
                         raise
                     logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="❌")
                     )
                     sys.exit(1)
                 elif on_error == "debug":
                     message += "\n\nStarting post-mortem debugger."
                     logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="🐛")
                     )
                     extype, value, tb = sys.exc_info()
-                    traceback.print_exc()
+                    print(tb)
                     pdb.post_mortem(tb)
                     sys.exit(1)
                 else:
                     message += "\n\nContinuing pipeline run."
                     logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="🔂")
                     )
             log_info["time"] = round(time.time() - t0, ndigits=1)
             return log_info
 
-        return wrapper
+        return __mne_bids_pipeline_failsafe_wrapper__
 
     return failsafe_run_decorator
 
 
 def hash_file_path(path: pathlib.Path) -> str:
     with open(path, "rb") as f:
         md5_hash = hashlib.md5(f.read())
@@ -357,17 +362,22 @@
 
 
 def _get_step_path(
     stack: Optional[List[inspect.FrameInfo]] = None,
 ) -> pathlib.Path:
     if stack is None:
         stack = inspect.stack()
+    paths = list()
     for frame in stack:
         fname = pathlib.Path(frame.filename)
         if "steps" in fname.parts:
             return fname
+        else:  # pragma: no cover
+            if frame.function == "__mne_bids_pipeline_failsafe_wrapper__":
+                return frame.frame.f_locals["__mne_bids_pipeline_step__"]
     else:  # pragma: no cover
-        raise RuntimeError("Could not find step path")
+        paths = "\n".join(paths)
+        raise RuntimeError(f"Could not find step path in call stack:\n{paths}")
 
 
 def _short_step_path(step_path: pathlib.Path) -> str:
     return f"{step_path.parent.name}/{step_path.stem}"
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_viz.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/_viz.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Optional
 from types import SimpleNamespace
 
 from mne_bids.config import BIDS_VERSION
 from mne_bids.utils import _write_json
 
-from ..._config_utils import get_datatype, get_subjects, get_sessions
+from ..._config_utils import get_subjects, get_sessions, _bids_kwargs
 from ..._logging import gen_log_kwargs, logger
 from ..._run import failsafe_run
 
 
 def init_dataset(cfg) -> None:
     """Prepare the pipeline directory in /derivatives."""
     fname_json = cfg.deriv_root / "dataset_description.json"
@@ -58,19 +58,18 @@
 
 
 def get_config(
     *,
     config,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        datatype=get_datatype(config),
-        deriv_root=config.deriv_root,
         PIPELINE_NAME=config.PIPELINE_NAME,
         VERSION=config.VERSION,
         CODE_URL=config.CODE_URL,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config):
     """Initialize the output directories."""
     init_dataset(cfg=get_config(config=config))
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from typing import Dict, Optional
 
 from mne.utils import _pl
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_datatype,
-    get_task,
     get_sessions,
     get_subjects,
-    get_runs,
+    get_mf_reference_run,
+    _bids_kwargs,
 )
 from ..._io import _empty_room_match_path, _write_json
 from ..._logging import gen_log_kwargs, logger
 from ..._run import _update_for_splits, failsafe_run, save_logs
 
 
 def get_input_fnames_find_empty_room(
     *, subject: str, session: Optional[str], run: Optional[str], cfg: SimpleNamespace
 ) -> Dict[str, BIDSPath]:
-    """Get paths of files required by filter_data function."""
+    """Get paths of files required by find_empty_room function."""
     bids_path_in = BIDSPath(
         subject=subject,
         run=run,
         session=session,
         task=cfg.task,
         acquisition=cfg.acq,
         recording=cfg.rec,
@@ -37,15 +37,15 @@
     )
     in_files: Dict[str, BIDSPath] = dict()
     in_files[f"raw_run-{run}"] = bids_path_in
     _update_for_splits(in_files, f"raw_run-{run}", single=True)
     if hasattr(bids_path_in, "find_matching_sidecar"):
         in_files["sidecar"] = (
             bids_path_in.copy()
-            .update(datatype=None)
+            .update(datatype=None, suffix="meg")
             .find_matching_sidecar(extension=".json")
         )
     try:
         fname = bids_path_in.find_empty_room(use_sidecar_only=True)
     except Exception:
         fname = None
     if fname is None and hasattr(bids_path_in, "get_empty_room_candidates"):
@@ -100,22 +100,15 @@
 
 
 def get_config(
     *,
     config,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        proc=config.proc,
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        bids_root=config.bids_root,
-        deriv_root=config.deriv_root,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config) -> None:
     """Run find_empty_room."""
     if not config.process_empty_room:
@@ -126,18 +119,15 @@
         msg = "Skipping, empty-room data only relevant for MEG …"
         logger.info(**gen_log_kwargs(message=msg, emoji="skip"))
         return
     # This will be I/O bound if the sidecar is not complete, so let's not run
     # in parallel.
     logs = list()
     for subject in get_subjects(config):
-        if config.use_maxwell_filter:
-            run = config.mf_reference_run
-        else:
-            run = get_runs(config=config, subject=subject)[0]
+        run = get_mf_reference_run(config=config)
         logs.append(
             find_empty_room(
                 cfg=get_config(
                     config=config,
                 ),
                 exec_params=config.exec_params,
                 subject=subject,
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,168 +10,174 @@
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_mf_cal_fname,
     get_mf_ctc_fname,
     get_subjects,
     get_sessions,
-    get_runs,
-    get_task,
-    get_datatype,
-    get_mf_reference_run,
+    get_runs_tasks,
+    _do_mf_autobad,
 )
 from ..._import_data import (
-    _get_raw_paths,
+    _get_run_rest_noise_path,
+    _get_mf_reference_run_path,
     import_experimental_data,
     import_er_data,
     _bads_path,
     _auto_scores_path,
+    _import_data_kwargs,
 )
 from ..._io import _write_json
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._report import _open_report, _add_raw
 from ..._run import failsafe_run, save_logs
 from ..._viz import plot_auto_scores
 
 
 def get_input_fnames_data_quality(
     *,
     cfg: SimpleNamespace,
     subject: str,
     session: Optional[str],
-    run: str,
+    run: Optional[str],
+    task: Optional[str],
 ) -> dict:
-    """Get paths of files required by maxwell_filter function."""
-    include_mf_ref = _do_mf_autobad(cfg=cfg)
-    in_files = _get_raw_paths(
+    """Get paths of files required by assess_data_quality function."""
+    kwargs = dict(
         cfg=cfg,
         subject=subject,
         session=session,
+        add_bads=False,
+    )
+    in_files = _get_run_rest_noise_path(
         run=run,
+        task=task,
         kind="orig",
-        add_bads=False,
-        include_mf_ref=include_mf_ref,
+        mf_reference_run=cfg.mf_reference_run,
+        **kwargs,
     )
+    # When doing autobad for the noise run, we also need the reference run
+    if _do_mf_autobad(cfg=cfg) and run is None and task == "noise":
+        in_files.update(_get_mf_reference_run_path(**kwargs))
     return in_files
 
 
 @failsafe_run(
     get_input_fnames=get_input_fnames_data_quality,
 )
 def assess_data_quality(
     *,
     cfg: SimpleNamespace,
     exec_params: SimpleNamespace,
     subject: str,
     session: Optional[str],
-    run: str,
+    run: Optional[str],
+    task: Optional[str],
     in_files: dict,
-) -> None:
+) -> dict:
     """Assess data quality and find and mark bad channels."""
     import matplotlib.pyplot as plt
 
     out_files = dict()
-    orig_run = run
-    # raw_ref_run will be .pop()ed inside this loop, do not include it
-    raw_keys = list(key for key in in_files.keys() if key != "raw_ref_run")
-    for key in raw_keys:
-        bids_path_in = in_files.pop(key)
-        if key == "raw_noise":
-            run = "noise"
-        elif key == "raw_rest":
-            run = "rest"
-        else:  # raw_run-{run}
-            run = orig_run
-        if _do_mf_autobad(cfg=cfg):
-            if key == "raw_noise":
-                bids_path_ref_in = in_files.pop("raw_ref_run")
-            else:
-                bids_path_ref_in = None
-            auto_scores = _find_bads_maxwell(
-                cfg=cfg,
-                exec_params=exec_params,
-                bids_path_in=bids_path_in,
-                bids_path_ref_in=bids_path_ref_in,
-                key=key,
-                subject=subject,
-                session=session,
-                run=run,
-                out_files=out_files,
-            )
+    key = f"raw_task-{task}_run-{run}"
+    bids_path_in = in_files.pop(key)
+    if _do_mf_autobad(cfg=cfg):
+        if key == "raw_task-noise_run-None":
+            bids_path_ref_in = in_files.pop("raw_ref_run")
         else:
-            auto_scores = None
+            bids_path_ref_in = None
+        auto_scores = _find_bads_maxwell(
+            cfg=cfg,
+            exec_params=exec_params,
+            bids_path_in=bids_path_in,
+            bids_path_ref_in=bids_path_ref_in,
+            subject=subject,
+            session=session,
+            run=run,
+            task=task,
+            out_files=out_files,
+        )
+    else:
+        auto_scores = None
+    del key
 
-        # Report
-        with _open_report(
-            cfg=cfg, exec_params=exec_params, subject=subject, session=session, run=run
-        ) as report:
-            # Original data
-            kind = "original" if not cfg.proc else cfg.proc
-            msg = f"Adding {kind} raw data to report"
+    # Report
+    with _open_report(
+        cfg=cfg,
+        exec_params=exec_params,
+        subject=subject,
+        session=session,
+        run=run,
+        task=task,
+    ) as report:
+        # Original data
+        kind = "original" if not cfg.proc else cfg.proc
+        msg = f"Adding {kind} raw data to report"
+        logger.info(**gen_log_kwargs(message=msg))
+        _add_raw(
+            cfg=cfg,
+            report=report,
+            bids_path_in=bids_path_in,
+            title=f"Raw ({kind})",
+            tags=("data-quality",),
+        )
+        if cfg.find_noisy_channels_meg:
+            assert auto_scores is not None
+            msg = "Adding noisy channel detection to report"
             logger.info(**gen_log_kwargs(message=msg))
-            _add_raw(
-                cfg=cfg,
-                report=report,
-                bids_path_in=bids_path_in,
-                title=f"Raw ({kind} run {run})",
+            figs = plot_auto_scores(auto_scores, ch_types=cfg.ch_types)
+            captions = [f"Run {run}"] * len(figs)
+            tags = ("raw", "data-quality", f"run-{run}")
+            report.add_figure(
+                fig=figs,
+                caption=captions,
+                section="Data quality",
+                title=f"Bad channel detection: {run}",
+                tags=tags,
+                replace=True,
             )
-            if cfg.find_noisy_channels_meg:
-                assert auto_scores is not None
-                msg = "Adding noisy channel detection to report"
-                logger.info(**gen_log_kwargs(message=msg))
-                figs = plot_auto_scores(auto_scores, ch_types=cfg.ch_types)
-                captions = [f"Run {run}"] * len(figs)
-                tags = ("raw", "data-quality", f"run-{run}")
-                report.add_figure(
-                    fig=figs,
-                    caption=captions,
-                    section="Data quality",
-                    title=f"Bad channel detection: {run}",
-                    tags=tags,
-                    replace=True,
-                )
-                for fig in figs:
-                    plt.close(fig)
+            for fig in figs:
+                plt.close(fig)
 
     assert len(in_files) == 0, in_files.keys()
     return out_files
 
 
 def _find_bads_maxwell(
     *,
     cfg: SimpleNamespace,
     exec_params: SimpleNamespace,
     bids_path_in: BIDSPath,
     bids_path_ref_in: Optional[BIDSPath],
     subject: str,
     session: Optional[str],
-    run: str,
-    key: str,
+    run: Optional[str],
+    task: Optional[str],
     out_files: dict,
 ):
     if cfg.find_flat_channels_meg and not cfg.find_noisy_channels_meg:
         msg = "Finding flat channels."
     elif cfg.find_noisy_channels_meg and not cfg.find_flat_channels_meg:
         msg = "Finding noisy channels using Maxwell filtering."
     else:
         msg = "Finding flat channels and noisy channels using " "Maxwell filtering."
     logger.info(**gen_log_kwargs(message=msg))
 
-    if key == "raw_noise":
+    if run is None and task == "noise":
         raw = import_er_data(
             cfg=cfg,
             bids_path_er_in=bids_path_in,
             bids_path_er_bads_in=None,
             bids_path_ref_in=bids_path_ref_in,
             bids_path_ref_bads_in=None,
             prepare_maxwell_filter=True,
         )
     else:
-        data_is_rest = key == "raw_rest"
+        data_is_rest = run is None and task == "rest"
         raw = import_experimental_data(
             bids_path_in=bids_path_in,
             bids_path_bads_in=None,
             cfg=cfg,
             data_is_rest=data_is_rest,
         )
 
@@ -217,15 +223,15 @@
         else:
             msg = "Found no noisy channels."
 
         logger.info(**gen_log_kwargs(message=msg))
         bads.extend(auto_noisy_chs)
 
     bads = sorted(set(bads))
-    msg = f"Found {len(bads)} channels as bad."
+    msg = f"Found {len(bads)} channel{_pl(bads)} as bad."
     raw.info["bads"] = bads
     del bads
     logger.info(**gen_log_kwargs(message=msg))
 
     if cfg.find_noisy_channels_meg:
         out_files["auto_scores"] = _auto_scores_path(
             cfg=cfg,
@@ -288,49 +294,21 @@
             session=session,
         )
         extra_kwargs["mf_ctc_fname"] = get_mf_ctc_fname(
             config=config,
             subject=subject,
             session=session,
         )
-        extra_kwargs["mf_reference_run"] = get_mf_reference_run(config=config)
         extra_kwargs["mf_head_origin"] = config.mf_head_origin
     cfg = SimpleNamespace(
-        process_empty_room=config.process_empty_room,
-        process_rest=config.process_rest,
-        task_is_rest=config.task_is_rest,
-        runs=get_runs(config=config, subject=subject),
-        proc=config.proc,
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        bids_root=config.bids_root,
-        deriv_root=config.deriv_root,
-        reader_extra_params=config.reader_extra_params,
-        crop_runs=config.crop_runs,
-        rename_events=config.rename_events,
-        eeg_bipolar_channels=config.eeg_bipolar_channels,
-        eeg_template_montage=config.eeg_template_montage,
-        fix_stim_artifact=config.fix_stim_artifact,
-        stim_artifact_tmin=config.stim_artifact_tmin,
-        stim_artifact_tmax=config.stim_artifact_tmax,
-        find_flat_channels_meg=config.find_flat_channels_meg,
-        find_noisy_channels_meg=config.find_noisy_channels_meg,
-        drop_channels=config.drop_channels,
-        find_breaks=config.find_breaks,
-        min_break_duration=config.min_break_duration,
-        t_break_annot_start_after_previous_event=config.t_break_annot_start_after_previous_event,  # noqa:E501
-        t_break_annot_stop_before_next_event=config.t_break_annot_stop_before_next_event,  # noqa:E501
-        data_type=config.data_type,
-        ch_types=config.ch_types,
-        eog_channels=config.eog_channels,
-        on_rename_missing_events=config.on_rename_missing_events,
-        plot_psd_for_runs=config.plot_psd_for_runs,
+        # These are included in _import_data_kwargs for automatic add_bads
+        # detection
+        # find_flat_channels_meg=config.find_flat_channels_meg,
+        # find_noisy_channels_meg=config.find_noisy_channels_meg,
+        **_import_data_kwargs(config=config, subject=subject),
         **extra_kwargs,
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run maxwell_filter."""
@@ -341,18 +319,19 @@
         logs = parallel(
             run_func(
                 cfg=get_config(config=config, subject=subject, session=session),
                 exec_params=config.exec_params,
                 subject=subject,
                 session=session,
                 run=run,
+                task=task,
             )
             for subject in get_subjects(config)
             for session in get_sessions(config)
-            for run in get_runs(config=config, subject=subject)
+            for run, task in get_runs_tasks(
+                config=config,
+                subject=subject,
+                session=session,
+            )
         )
 
     save_logs(config=config, logs=logs)
-
-
-def _do_mf_autobad(*, cfg: SimpleNamespace) -> bool:
-    return cfg.find_noisy_channels_meg or cfg.find_flat_channels_meg
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_03_maxfilter.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,349 +10,346 @@
 The head position of all runs is corrected to the run specified in
 config.mf_reference_run.
 It is critical to mark bad channels before Maxwell filtering.
 
 The function loads machine-specific calibration files.
 """
 
+import gc
 from typing import Optional
 from types import SimpleNamespace
 
 import numpy as np
 import mne
 from mne_bids import read_raw_bids
 
 from ..._config_utils import (
     get_mf_cal_fname,
     get_mf_ctc_fname,
     get_subjects,
     get_sessions,
-    get_runs,
-    get_task,
-    get_datatype,
-    get_mf_reference_run,
+    get_runs_tasks,
 )
 from ..._import_data import (
     import_experimental_data,
     import_er_data,
-    _get_raw_paths,
-    _add_bads_file,
+    _get_run_path,
+    _get_run_rest_noise_path,
+    _get_mf_reference_run_path,
+    _import_data_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._report import _open_report, _add_raw
 from ..._run import failsafe_run, save_logs, _update_for_splits
 
 
 def get_input_fnames_maxwell_filter(
     *,
     cfg: SimpleNamespace,
     subject: str,
     session: Optional[str],
-    run: str,
+    run: Optional[str],
+    task: Optional[str],
 ) -> dict:
     """Get paths of files required by maxwell_filter function."""
-    in_files = _get_raw_paths(
+    kwargs = dict(
         cfg=cfg,
         subject=subject,
         session=session,
+    )
+    in_files = _get_run_rest_noise_path(
         run=run,
+        task=task,
         kind="orig",
+        mf_reference_run=cfg.mf_reference_run,
+        **kwargs,
     )
-    ref_bids_path = (
-        list(in_files.values())[0]
-        .copy()
-        .update(
-            run=cfg.mf_reference_run,
-            check=True,
+    # head positions
+    if cfg.mf_mc:
+        if run is None and task == "noise":
+            pos_run, pos_task = cfg.mf_reference_run, cfg.task
+        else:
+            pos_run, pos_task = run, task
+        path = _get_run_path(
+            run=pos_run,
+            task=pos_task,
+            add_bads=False,
+            kind="orig",
+            **kwargs,
+        )[f"raw_task-{pos_task}_run-{pos_run}"]
+        in_files[f"raw_task-{task}_run-{run}-pos"] = path.update(
+            extension=".pos",
+            root=cfg.deriv_root,
+            check=False,
+            task=pos_task,
+            run=pos_run,
         )
-    )
-    key = "raw_ref_run"
-    in_files[key] = ref_bids_path
-    _add_bads_file(
-        cfg=cfg,
-        in_files=in_files,
-        key=key,
-    )
+
+    # reference run (used for `destination` and also bad channels for noise)
+    in_files.update(_get_mf_reference_run_path(add_bads=True, **kwargs))
+
+    # standard files
     in_files["mf_cal_fname"] = cfg.mf_cal_fname
     in_files["mf_ctc_fname"] = cfg.mf_ctc_fname
     return in_files
 
 
 @failsafe_run(
     get_input_fnames=get_input_fnames_maxwell_filter,
 )
 def run_maxwell_filter(
     *,
     cfg: SimpleNamespace,
     exec_params: SimpleNamespace,
     subject: str,
     session: Optional[str],
-    run: str,
+    run: Optional[str],
+    task: Optional[str],
     in_files: dict,
 ) -> dict:
     if cfg.proc and "sss" in cfg.proc and cfg.use_maxwell_filter:
         raise ValueError(
             f"You cannot set use_maxwell_filter to True "
             f"if data have already processed with Maxwell-filter."
             f" Got proc={cfg.proc}."
         )
-    in_key = f"raw_run-{run}"
+    if isinstance(cfg.mf_destination, str):
+        destination = cfg.mf_destination
+        assert destination == "reference_run"
+    else:
+        destination = np.array(cfg.mf_destination, float)
+        assert destination.shape == (4, 4)
+        destination = mne.transforms.Transform("meg", "head", destination)
+
+    filter_chpi = cfg.mf_mc if cfg.mf_filter_chpi is None else cfg.mf_filter_chpi
+    is_rest_noise = run is None and task in ("noise", "rest")
+    if is_rest_noise:
+        nice_names = dict(rest="resting-state", noise="empty-room")
+        recording_type = nice_names[task]
+    else:
+        recording_type = "experimental"
+    in_key = f"raw_task-{task}_run-{run}"
     bids_path_in = in_files.pop(in_key)
     bids_path_bads_in = in_files.pop(f"{in_key}-bads", None)
-    bids_path_out = bids_path_in.copy().update(
+    bids_path_out_kwargs = dict(
+        subject=subject,  # need these in the case of an empty room match
+        session=session,
         processing="sss",
         suffix="raw",
         extension=".fif",
         root=cfg.deriv_root,
         check=False,
     )
+    bids_path_out = bids_path_in.copy().update(**bids_path_out_kwargs)
+
     # Now take everything from the bids_path_in and overwrite the parameters
     subject = bids_path_in.subject  # noqa: F841
     session = bids_path_in.session  # noqa: F841
     run = bids_path_in.run
 
     out_files = dict()
     # Load dev_head_t and digitization points from MaxFilter reference run.
-    if cfg.mf_reference_run is not None:
-        # Only log if we have more than just a single run
-        msg = f"Loading reference run: {cfg.mf_reference_run}."
-        logger.info(**gen_log_kwargs(message=msg))
+    msg = f"Loading reference run: {cfg.mf_reference_run}."
+    logger.info(**gen_log_kwargs(message=msg))
 
     bids_path_ref_in = in_files.pop("raw_ref_run")
     raw = read_raw_bids(
-        bids_path=bids_path_ref_in, extra_params=cfg.reader_extra_params
+        bids_path=bids_path_ref_in,
+        extra_params=cfg.reader_extra_params,
+        verbose=cfg.read_raw_bids_verbose,
     )
     bids_path_ref_bads_in = in_files.pop("raw_ref_run-bads", None)
-    dev_head_t = raw.info["dev_head_t"]
+    if isinstance(destination, str):
+        assert destination == "reference_run"
+        destination = raw.info["dev_head_t"]
     del raw
-
-    raw = import_experimental_data(
-        cfg=cfg,
-        bids_path_in=bids_path_in,
-        bids_path_bads_in=bids_path_bads_in,
-        data_is_rest=False,
-    )
+    assert isinstance(destination, mne.transforms.Transform), destination
 
     # Maxwell-filter experimental data.
-    msg = "Applying Maxwell filter to experimental data: "
-
+    apply_msg = "Applying "
     if cfg.mf_st_duration:
-        msg += f"tSSS (st_duration: {cfg.mf_st_duration} sec)."
+        apply_msg += f"tSSS ({cfg.mf_st_duration} sec, corr={cfg.mf_st_correlation})"
     else:
-        msg += "SSS."
-    logger.info(**gen_log_kwargs(message=msg))
-
-    # Warn if no bad channels are set before Maxwell filter
-    if not raw.info["bads"]:
-        msg = (
-            "No channels were marked as bad. Please carefully check "
-            "your data to ensure this is correct; otherwise, Maxwell "
-            "filtering WILL cause problems."
-        )
-        logger.warning(**gen_log_kwargs(message=msg))
+        apply_msg += "SSS"
+    if cfg.mf_mc:
+        apply_msg += " with MC"
+        head_pos = mne.chpi.read_head_pos(in_files.pop(f"{in_key}-pos"))
+    else:
+        head_pos = None
+    apply_msg += " to"
 
-    # Keyword arguments shared between Maxwell filtering of the
-    # experimental and the empty-room data.
-    common_mf_kws = dict(
-        # TODO: Add head_pos, st_correlation, eSSS
+    mf_kws = dict(
         calibration=in_files.pop("mf_cal_fname"),
         cross_talk=in_files.pop("mf_ctc_fname"),
         st_duration=cfg.mf_st_duration,
+        st_correlation=cfg.mf_st_correlation,
         origin=cfg.mf_head_origin,
         coord_frame="head",
-        destination=dev_head_t,
+        destination=destination,
+        head_pos=head_pos,
     )
 
-    raw_sss = mne.preprocessing.maxwell_filter(raw, **common_mf_kws)
-    out_files["sss_raw"] = bids_path_out
-    msg = f"Writing {out_files['sss_raw'].fpath.relative_to(cfg.deriv_root)}"
-    logger.info(**gen_log_kwargs(message=msg))
-    raw_sss.save(
-        out_files["sss_raw"],
-        split_naming="bids",
-        overwrite=True,
-        split_size=cfg._raw_split_size,
-    )
-    del raw
-    # we need to be careful about split files
-    _update_for_splits(out_files, "sss_raw")
-
-    if exec_params.interactive:
-        raw_sss.plot(n_channels=50, butterfly=True, block=True)
-    del raw_sss
-
-    # Reporting
-    with _open_report(
-        cfg=cfg, exec_params=exec_params, subject=subject, session=session, run=run
-    ) as report:
-        msg = "Adding Maxwell filtered raw data to report."
-        _add_raw(
+    logger.info(**gen_log_kwargs(message=f"{apply_msg} {recording_type} data"))
+    if not (run is None and task == "noise"):
+        data_is_rest = run is None and task == "rest"
+        raw = import_experimental_data(
             cfg=cfg,
-            report=report,
-            bids_path_in=out_files["sss_raw"],
-            title="Raw (maxwell filtered)",
+            bids_path_in=bids_path_in,
+            bids_path_bads_in=bids_path_bads_in,
+            data_is_rest=data_is_rest,
+        )
+        fr = raw.info["dev_head_t"]["trans"]
+        where = "original head position"
+    else:
+        raw = import_er_data(
+            cfg=cfg,
+            bids_path_er_in=bids_path_in,
+            bids_path_ref_in=bids_path_ref_in,
+            # TODO: This can break processing, need to use union for all,
+            # otherwise can get for ds003392:
+            # "Reference run data rank does not match empty-room data rank"
+            # bids_path_er_bads_in=bids_path_noise_bads,
+            bids_path_er_bads_in=None,
+            bids_path_ref_bads_in=bids_path_ref_bads_in,
+            prepare_maxwell_filter=True,
         )
-    del bids_path_in
+        fr = np.eye(4)
+        where = "MEG device origin"
 
-    # Noise data processing.
-    nice_names = dict(rest="resting-state", noise="empty-room")
-    for task in ("rest", "noise"):
-        in_key = f"raw_{task}"
-        if in_key not in in_files:
-            continue
-        recording_type = nice_names[task]
-        msg = f"Processing {recording_type} recording …"
-        logger.info(**gen_log_kwargs(message=msg, run=task))
-        bids_path_noise = in_files.pop(in_key)
-        bids_path_noise_bads = in_files.pop(f"{in_key}-bads", None)
-        if task == "rest":
-            raw_noise = import_experimental_data(
-                cfg=cfg,
-                bids_path_in=bids_path_noise,
-                bids_path_bads_in=bids_path_noise_bads,
-                data_is_rest=True,
-            )
-        else:
-            raw_noise = import_er_data(
-                cfg=cfg,
-                bids_path_er_in=bids_path_noise,
-                bids_path_ref_in=bids_path_ref_in,
-                # TODO: This can break processing, need to use union for all,
-                # otherwise can get for ds003392:
-                # "Reference run data rank does not match empty-room data rank"
-                # bids_path_er_bads_in=bids_path_noise_bads,
-                bids_path_er_bads_in=None,
-                bids_path_ref_bads_in=bids_path_ref_bads_in,
-                prepare_maxwell_filter=True,
-            )
+    # Give some information about the transformation
+    to = destination["trans"]
+    dist = 1000 * np.linalg.norm(fr[:3, 3] - to[:3, 3])
+    angle = np.rad2deg(
+        mne.transforms._angle_between_quats(
+            *mne.transforms.rot_to_quat(np.array([to[:3, :3], fr[:3, :3]]))
+        )
+    )
+    msg = f"Destination is {dist:0.1f} mm and {angle:0.1f}° from the {where}"
+    logger.info(**gen_log_kwargs(message=msg))
 
-        # Maxwell-filter noise data.
-        msg = f"Applying Maxwell filter to {recording_type} recording"
-        logger.info(**gen_log_kwargs(message=msg, run=task))
-        raw_noise_sss = mne.preprocessing.maxwell_filter(raw_noise, **common_mf_kws)
+    # Warn if no bad channels are set before Maxwell filter
+    if not raw.info["bads"]:
+        msg = (
+            "No channels were marked as bad. Please carefully check "
+            "your data to ensure this is correct; otherwise, Maxwell "
+            "filtering WILL cause problems."
+        )
+        logger.warning(**gen_log_kwargs(message=msg))
 
+    raw_sss = mne.preprocessing.maxwell_filter(raw, **mf_kws)
+    del raw
+    gc.collect()
+
+    if is_rest_noise:
         # Perform a sanity check: empty-room rank should exactly match the
         # experimental data rank after Maxwell filtering; resting-state rank
         # should be equal or be greater than experimental data rank.
         #
         # We're treating the two cases differently, because we don't
         # copy the bad channel selection from the reference run over to
         # the resting-state recording.
 
-        raw_sss = mne.io.read_raw_fif(out_files["sss_raw"])
-        rank_exp = mne.compute_rank(raw_sss, rank="info")["meg"]
-        rank_noise = mne.compute_rank(raw_noise_sss, rank="info")["meg"]
+        bids_path_ref_sss = bids_path_ref_in.copy().update(**bids_path_out_kwargs)
+        raw_exp = mne.io.read_raw_fif(bids_path_ref_sss)
+        rank_exp = mne.compute_rank(raw_exp, rank="info")["meg"]
+        rank_noise = mne.compute_rank(raw_sss, rank="info")["meg"]
+        del raw_exp
 
         if task == "rest":
             if rank_exp > rank_noise:
                 msg = (
                     f"Resting-state rank ({rank_noise}) is lower than "
                     f"reference run data rank ({rank_exp}). We will try to "
                     f"take care of this during epoching of the experimental "
                     f"data."
                 )
-                logger.warning(**gen_log_kwargs(message=msg, run=task))
+                logger.warning(**gen_log_kwargs(message=msg))
             else:
                 pass  # Should cause no problems!
         elif not np.isclose(rank_exp, rank_noise):
             msg = (
                 f"Reference run data rank {rank_exp:.1f} does not "
                 f"match {recording_type} data rank {rank_noise:.1f} after "
                 f"Maxwell filtering. This indicates that the data "
                 f"were processed  differently."
             )
             raise RuntimeError(msg)
 
-        out_files[in_key] = bids_path_out.copy().update(
-            task=task, run=None, processing="sss"
+    if filter_chpi:
+        logger.info(**gen_log_kwargs(message="Filtering cHPI"))
+        mne.chpi.filter_chpi(
+            raw_sss,
+            t_window=cfg.mf_mc_t_window,
         )
 
-        # Save only the channel types we wish to analyze
-        # (same as for experimental data above).
-        msg = "Writing " f"{out_files[in_key].fpath.relative_to(cfg.deriv_root)}"
-        logger.info(**gen_log_kwargs(message=msg, run=task))
-        raw_noise_sss.save(
-            out_files[in_key],
-            overwrite=True,
-            split_naming="bids",
-            split_size=cfg._raw_split_size,
-        )
-        _update_for_splits(out_files, in_key)
-        del raw_noise_sss
+    out_files["sss_raw"] = bids_path_out
+    msg = f"Writing {out_files['sss_raw'].fpath.relative_to(cfg.deriv_root)}"
+    logger.info(**gen_log_kwargs(message=msg))
+    raw_sss.save(
+        out_files["sss_raw"],
+        split_naming="bids",
+        overwrite=True,
+        split_size=cfg._raw_split_size,
+    )
+    _update_for_splits(out_files, "sss_raw")
 
-        with _open_report(
-            cfg=cfg, exec_params=exec_params, subject=subject, session=session, run=task
-        ) as report:
-            msg = "Adding Maxwell filtered raw data to report"
-            logger.info(**gen_log_kwargs(message=msg, run=task))
-            _add_raw(
-                cfg=cfg,
-                report=report,
-                bids_path_in=out_files[in_key],
-                title="Raw (maxwell filtered)",
-            )
+    if exec_params.interactive:
+        raw_sss.plot(n_channels=50, butterfly=True, block=True)
+
+    # Reporting
+    with _open_report(
+        cfg=cfg,
+        exec_params=exec_params,
+        subject=subject,
+        session=session,
+        run=run,
+        task=task,
+    ) as report:
+        msg = "Adding Maxwell filtered raw data to report."
+        logger.info(**gen_log_kwargs(message=msg))
+        _add_raw(
+            cfg=cfg,
+            report=report,
+            bids_path_in=out_files["sss_raw"],
+            title="Raw (maxwell filtered)",
+            tags=("sss",),
+            raw=raw_sss,
+        )
 
     assert len(in_files) == 0, in_files.keys()
     return out_files
 
 
 def get_config(
     *,
     config: SimpleNamespace,
     subject: str,
     session: Optional[str],
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        reader_extra_params=config.reader_extra_params,
         mf_cal_fname=get_mf_cal_fname(
             config=config,
             subject=subject,
             session=session,
         ),
         mf_ctc_fname=get_mf_ctc_fname(
             config=config,
             subject=subject,
             session=session,
         ),
         mf_st_duration=config.mf_st_duration,
+        mf_st_correlation=config.mf_st_correlation,
         mf_head_origin=config.mf_head_origin,
-        process_empty_room=config.process_empty_room,
-        process_rest=config.process_rest,
-        task_is_rest=config.task_is_rest,
-        # XXX needs to accept session!
-        runs=get_runs(config=config, subject=subject),
-        use_maxwell_filter=config.use_maxwell_filter,
-        proc=config.proc,
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        bids_root=config.bids_root,
-        deriv_root=config.deriv_root,
-        crop_runs=config.crop_runs,
-        rename_events=config.rename_events,
-        eeg_template_montage=config.eeg_template_montage,
-        fix_stim_artifact=config.fix_stim_artifact,
-        stim_artifact_tmin=config.stim_artifact_tmin,
-        stim_artifact_tmax=config.stim_artifact_tmax,
-        find_flat_channels_meg=config.find_flat_channels_meg,
-        find_noisy_channels_meg=config.find_noisy_channels_meg,
-        mf_reference_run=get_mf_reference_run(config),
-        drop_channels=config.drop_channels,
-        find_breaks=config.find_breaks,
-        min_break_duration=config.min_break_duration,
-        t_break_annot_start_after_previous_event=config.t_break_annot_start_after_previous_event,  # noqa:E501
-        t_break_annot_stop_before_next_event=config.t_break_annot_stop_before_next_event,  # noqa:E501
-        ch_types=config.ch_types,
-        data_type=config.data_type,
-        on_rename_missing_events=config.on_rename_missing_events,
-        plot_psd_for_runs=config.plot_psd_for_runs,
-        _raw_split_size=config._raw_split_size,
+        mf_mc=config.mf_mc,
+        mf_filter_chpi=config.mf_filter_chpi,
+        mf_destination=config.mf_destination,
+        mf_int_order=config.mf_int_order,
+        mf_mc_t_window=config.mf_mc_t_window,
+        **_import_data_kwargs(config=config, subject=subject),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run maxwell_filter."""
     if not config.use_maxwell_filter:
@@ -367,14 +364,19 @@
         logs = parallel(
             run_func(
                 cfg=get_config(config=config, subject=subject, session=session),
                 exec_params=config.exec_params,
                 subject=subject,
                 session=session,
                 run=run,
+                task=task,
             )
             for subject in get_subjects(config)
             for session in get_sessions(config)
-            for run in get_runs(config=config, subject=subject)
+            for run, task in get_runs_tasks(
+                config=config,
+                subject=subject,
+                session=session,
+            )
         )
 
     save_logs(config=config, logs=logs)
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_04_frequency_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,65 +18,66 @@
 from types import SimpleNamespace
 from typing import Optional, Union, Literal, Iterable
 
 import mne
 
 from ..._config_utils import (
     get_sessions,
-    get_runs,
+    get_runs_tasks,
     get_subjects,
-    get_task,
-    get_datatype,
-    get_mf_reference_run,
 )
 from ..._import_data import (
     import_experimental_data,
     import_er_data,
-    _get_raw_paths,
+    _get_run_rest_noise_path,
+    _import_data_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._report import _open_report, _add_raw
 from ..._run import failsafe_run, save_logs, _update_for_splits
 
 
 def get_input_fnames_frequency_filter(
     *,
     cfg: SimpleNamespace,
     subject: str,
     session: Optional[str],
     run: str,
+    task: Optional[str],
 ) -> dict:
     """Get paths of files required by filter_data function."""
     kind = "sss" if cfg.use_maxwell_filter else "orig"
-    return _get_raw_paths(
+    return _get_run_rest_noise_path(
         cfg=cfg,
         subject=subject,
         session=session,
         run=run,
+        task=task,
         kind=kind,
-        include_mf_ref=False,
+        mf_reference_run=cfg.mf_reference_run,
     )
 
 
 def notch_filter(
     raw: mne.io.BaseRaw,
     subject: str,
     session: Optional[str],
     run: str,
+    task: Optional[str],
     freqs: Optional[Union[float, Iterable[float]]],
     trans_bandwidth: Union[float, Literal["auto"]],
     notch_widths: Optional[Union[float, Iterable[float]]],
-    data_type: Literal["experimental", "empty-room", "resting-state"],
+    run_type: Literal["experimental", "empty-room", "resting-state"],
 ) -> None:
     """Filter data channels (MEG and EEG)."""
     if freqs is None:
-        msg = f"Not applying notch filter to {data_type} data."
+        msg = f"Not applying notch filter to {run_type} data."
     else:
-        msg = f"Notch filtering {data_type} data at {freqs} Hz."
+        msg = f"Notch filtering {run_type} data at {freqs} Hz."
 
     logger.info(**gen_log_kwargs(message=msg))
 
     if freqs is None:
         return
 
     raw.notch_filter(
@@ -88,29 +89,30 @@
 
 
 def bandpass_filter(
     raw: mne.io.BaseRaw,
     subject: str,
     session: Optional[str],
     run: str,
+    task: Optional[str],
     l_freq: Optional[float],
     h_freq: Optional[float],
     l_trans_bandwidth: Union[float, Literal["auto"]],
     h_trans_bandwidth: Union[float, Literal["auto"]],
-    data_type: Literal["experimental", "empty-room", "resting-state"],
+    run_type: Literal["experimental", "empty-room", "resting-state"],
 ) -> None:
     """Filter data channels (MEG and EEG)."""
     if l_freq is not None and h_freq is None:
-        msg = f"High-pass filtering {data_type} data; lower bound: " f"{l_freq} Hz"
+        msg = f"High-pass filtering {run_type} data; lower bound: " f"{l_freq} Hz"
     elif l_freq is None and h_freq is not None:
-        msg = f"Low-pass filtering {data_type} data; upper bound: " f"{h_freq} Hz"
+        msg = f"Low-pass filtering {run_type} data; upper bound: " f"{h_freq} Hz"
     elif l_freq is not None and h_freq is not None:
-        msg = f"Band-pass filtering {data_type} data; range: " f"{l_freq} – {h_freq} Hz"
+        msg = f"Band-pass filtering {run_type} data; range: " f"{l_freq} – {h_freq} Hz"
     else:
-        msg = f"Not applying frequency filtering to {data_type} data."
+        msg = f"Not applying frequency filtering to {run_type} data."
 
     logger.info(**gen_log_kwargs(message=msg))
 
     if l_freq is None and h_freq is None:
         return
 
     raw.filter(
@@ -123,92 +125,115 @@
 
 
 def resample(
     raw: mne.io.BaseRaw,
     subject: str,
     session: Optional[str],
     run: str,
+    task: Optional[str],
     sfreq: float,
-    data_type: Literal["experimental", "empty-room", "resting-state"],
+    run_type: Literal["experimental", "empty-room", "resting-state"],
 ) -> None:
     if not sfreq:
         return
 
-    msg = f"Resampling {data_type} data to {sfreq:.1f} Hz"
+    msg = f"Resampling {run_type} data to {sfreq:.1f} Hz"
     logger.info(**gen_log_kwargs(message=msg))
     raw.resample(sfreq, npad="auto")
 
 
 @failsafe_run(
     get_input_fnames=get_input_fnames_frequency_filter,
 )
 def filter_data(
     *,
     cfg: SimpleNamespace,
     exec_params: SimpleNamespace,
     subject: str,
     session: Optional[str],
     run: str,
+    task: Optional[str],
     in_files: dict,
 ) -> dict:
     """Filter data from a single subject."""
     out_files = dict()
-    in_key = f"raw_run-{run}"
-    bids_path = in_files.pop(in_key)
+    in_key = f"raw_task-{task}_run-{run}"
+    bids_path_in = in_files.pop(in_key)
     bids_path_bads_in = in_files.pop(f"{in_key}-bads", None)
 
-    # Create paths for reading and writing the filtered data.
+    if run is None and task in ("noise", "rest"):
+        run_type = dict(rest="resting-state", noise="empty-room")[task]
+    else:
+        run_type = "experimental"
+
     if cfg.use_maxwell_filter:
-        msg = f"Reading: {bids_path.basename}"
+        msg = f"Reading {run_type} recording: " f"{bids_path_in.basename}"
         logger.info(**gen_log_kwargs(message=msg))
-        raw = mne.io.read_raw_fif(bids_path)
+        raw = mne.io.read_raw_fif(bids_path_in)
+    elif run is None and task == "noise":
+        raw = import_er_data(
+            cfg=cfg,
+            bids_path_er_in=bids_path_in,
+            bids_path_ref_in=in_files.pop("raw_ref_run"),
+            bids_path_er_bads_in=bids_path_bads_in,
+            # take bads from this run (0)
+            bids_path_ref_bads_in=in_files.pop("raw_ref_run-bads", None),
+            prepare_maxwell_filter=False,
+        )
     else:
+        data_is_rest = run is None and task == "rest"
         raw = import_experimental_data(
             cfg=cfg,
-            bids_path_in=bids_path,
+            bids_path_in=bids_path_in,
             bids_path_bads_in=bids_path_bads_in,
-            data_is_rest=False,
+            data_is_rest=data_is_rest,
         )
 
-    out_files[in_key] = bids_path.copy().update(
+    out_files[in_key] = bids_path_in.copy().update(
         root=cfg.deriv_root,
         processing="filt",
         extension=".fif",
         suffix="raw",
         split=None,
+        task=task,
+        run=run,
     )
+
     raw.load_data()
     notch_filter(
         raw=raw,
         subject=subject,
         session=session,
         run=run,
+        task=task,
         freqs=cfg.notch_freq,
         trans_bandwidth=cfg.notch_trans_bandwidth,
         notch_widths=cfg.notch_widths,
-        data_type="experimental",
+        run_type=run_type,
     )
     bandpass_filter(
         raw=raw,
         subject=subject,
         session=session,
         run=run,
+        task=task,
         h_freq=cfg.h_freq,
         l_freq=cfg.l_freq,
         h_trans_bandwidth=cfg.h_trans_bandwidth,
         l_trans_bandwidth=cfg.l_trans_bandwidth,
-        data_type="experimental",
+        run_type=run_type,
     )
     resample(
         raw=raw,
         subject=subject,
         session=session,
         run=run,
+        task=task,
         sfreq=cfg.raw_resample_sfreq,
-        data_type="experimental",
+        run_type=run_type,
     )
 
     raw.save(
         out_files[in_key],
         overwrite=True,
         split_naming="bids",
         split_size=cfg._raw_split_size,
@@ -216,165 +241,52 @@
     _update_for_splits(out_files, in_key)
     fmax = 1.5 * cfg.h_freq if cfg.h_freq is not None else np.inf
     if exec_params.interactive:
         # Plot raw data and power spectral density.
         raw.plot(n_channels=50, butterfly=True)
         raw.compute_psd(fmax=fmax).plot()
 
-    del raw
-
-    nice_names = dict(rest="resting-state", noise="empty-room")
-    for task in ("rest", "noise"):
-        in_key = f"raw_{task}"
-        if in_key not in in_files:
-            continue
-        data_type = nice_names[task]
-        bids_path_noise = in_files.pop(in_key)
-        bids_path_noise_bads = in_files.pop(f"{in_key}-bads", None)
-        if cfg.use_maxwell_filter:
-            msg = f"Reading {data_type} recording: " f"{bids_path_noise.basename}"
-            logger.info(**gen_log_kwargs(message=msg, run=task))
-            raw_noise = mne.io.read_raw_fif(bids_path_noise)
-        elif data_type == "empty-room":
-            raw_noise = import_er_data(
-                cfg=cfg,
-                bids_path_er_in=bids_path_noise,
-                bids_path_ref_in=bids_path,
-                bids_path_er_bads_in=bids_path_noise_bads,
-                # take bads from this run (0)
-                bids_path_ref_bads_in=bids_path_bads_in,
-                prepare_maxwell_filter=False,
-            )
-        else:
-            raw_noise = import_experimental_data(
-                cfg=cfg,
-                bids_path_in=bids_path_noise,
-                bids_path_bads_in=bids_path_noise_bads,
-                data_is_rest=True,
-            )
-        out_files[in_key] = bids_path.copy().update(
-            root=cfg.deriv_root,
-            processing="filt",
-            extension=".fif",
-            suffix="raw",
-            split=None,
-            task=task,
-            run=None,
-        )
-
-        raw_noise.load_data()
-        notch_filter(
-            raw=raw_noise,
-            subject=subject,
-            session=session,
-            run=task,
-            freqs=cfg.notch_freq,
-            trans_bandwidth=cfg.notch_trans_bandwidth,
-            notch_widths=cfg.notch_widths,
-            data_type=data_type,
-        )
-        bandpass_filter(
-            raw=raw_noise,
-            subject=subject,
-            session=session,
-            run=task,
-            h_freq=cfg.h_freq,
-            l_freq=cfg.l_freq,
-            h_trans_bandwidth=cfg.h_trans_bandwidth,
-            l_trans_bandwidth=cfg.l_trans_bandwidth,
-            data_type=data_type,
-        )
-        resample(
-            raw=raw_noise,
-            subject=subject,
-            session=session,
-            run=task,
-            sfreq=cfg.raw_resample_sfreq,
-            data_type=data_type,
-        )
-
-        raw_noise.save(
-            out_files[in_key],
-            overwrite=True,
-            split_naming="bids",
-            split_size=cfg._raw_split_size,
-        )
-        _update_for_splits(out_files, in_key)
-        if exec_params.interactive:
-            # Plot raw data and power spectral density.
-            raw_noise.plot(n_channels=50, butterfly=True)
-            raw_noise.compute_psd(fmax=fmax).plot()
-
-    assert len(in_files) == 0, in_files.keys()
-
     with _open_report(
-        cfg=cfg, exec_params=exec_params, subject=subject, session=session, run=run
+        cfg=cfg,
+        exec_params=exec_params,
+        subject=subject,
+        session=session,
+        run=run,
+        task=task,
     ) as report:
         msg = "Adding filtered raw data to report"
         logger.info(**gen_log_kwargs(message=msg))
-        for fname in out_files.values():
-            _add_raw(
-                cfg=cfg,
-                report=report,
-                bids_path_in=fname,
-                title="Raw (filtered)",
-            )
+        _add_raw(
+            cfg=cfg,
+            report=report,
+            bids_path_in=out_files[in_key],
+            title="Raw (filtered)",
+            tags=("filtered",),
+            raw=raw,
+        )
 
+    assert len(in_files) == 0, in_files.keys()
     return out_files
 
 
 def get_config(
     *,
     config: SimpleNamespace,
     subject: str,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        reader_extra_params=config.reader_extra_params,
-        process_empty_room=config.process_empty_room,
-        process_rest=config.process_rest,
-        task_is_rest=config.task_is_rest,
-        runs=get_runs(config=config, subject=subject),
-        use_maxwell_filter=config.use_maxwell_filter,
-        proc=config.proc,
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        bids_root=config.bids_root,
-        deriv_root=config.deriv_root,
         l_freq=config.l_freq,
         h_freq=config.h_freq,
         notch_freq=config.notch_freq,
         l_trans_bandwidth=config.l_trans_bandwidth,
         h_trans_bandwidth=config.h_trans_bandwidth,
         notch_trans_bandwidth=config.notch_trans_bandwidth,
         notch_widths=config.notch_widths,
         raw_resample_sfreq=config.raw_resample_sfreq,
-        crop_runs=config.crop_runs,
-        rename_events=config.rename_events,
-        eeg_bipolar_channels=config.eeg_bipolar_channels,
-        eeg_template_montage=config.eeg_template_montage,
-        fix_stim_artifact=config.fix_stim_artifact,
-        stim_artifact_tmin=config.stim_artifact_tmin,
-        stim_artifact_tmax=config.stim_artifact_tmax,
-        find_flat_channels_meg=config.find_flat_channels_meg,
-        find_noisy_channels_meg=config.find_noisy_channels_meg,
-        mf_reference_run=get_mf_reference_run(config),
-        drop_channels=config.drop_channels,
-        find_breaks=config.find_breaks,
-        min_break_duration=config.min_break_duration,
-        t_break_annot_start_after_previous_event=config.t_break_annot_start_after_previous_event,  # noqa:E501
-        t_break_annot_stop_before_next_event=config.t_break_annot_stop_before_next_event,  # noqa:E501
-        data_type=config.data_type,
-        ch_types=config.ch_types,
-        eog_channels=config.eog_channels,
-        on_rename_missing_events=config.on_rename_missing_events,
-        plot_psd_for_runs=config.plot_psd_for_runs,
-        _raw_split_size=config._raw_split_size,
+        **_import_data_kwargs(config=config, subject=subject),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run filter."""
     with get_parallel_backend(config.exec_params):
@@ -386,14 +298,19 @@
                     config=config,
                     subject=subject,
                 ),
                 exec_params=config.exec_params,
                 subject=subject,
                 session=session,
                 run=run,
+                task=task,
             )
             for subject in get_subjects(config)
             for session in get_sessions(config)
-            for run in get_runs(config=config, subject=subject)
+            for run, task in get_runs_tasks(
+                config=config,
+                subject=subject,
+                session=session,
+            )
         )
 
     save_logs(config=config, logs=logs)
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_05_make_epochs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from types import SimpleNamespace
 from typing import Optional
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
-    get_task,
     get_runs,
     get_subjects,
     get_eeg_reference,
     get_sessions,
-    get_datatype,
+    _bids_kwargs,
 )
 from ..._import_data import make_epochs, annotations_to_events
 from ..._logging import gen_log_kwargs, logger
 from ..._report import _open_report
 from ..._run import (
     failsafe_run,
     save_logs,
@@ -299,24 +298,15 @@
 
 def get_config(
     *,
     config,
     subject: str,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        runs=get_runs(config=config, subject=subject),
         use_maxwell_filter=config.use_maxwell_filter,
-        proc=config.proc,
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        bids_root=config.bids_root,
-        deriv_root=config.deriv_root,
         task_is_rest=config.task_is_rest,
         conditions=config.conditions,
         epochs_tmin=config.epochs_tmin,
         epochs_tmax=config.epochs_tmax,
         epochs_metadata_tmin=config.epochs_metadata_tmin,
         epochs_metadata_tmax=config.epochs_metadata_tmax,
         epochs_metadata_keep_first=config.epochs_metadata_keep_first,
@@ -326,14 +316,16 @@
         epochs_decim=config.epochs_decim,
         ch_types=config.ch_types,
         noise_cov=_sanitize_callable(config.noise_cov),
         eeg_reference=get_eeg_reference(config),
         rest_epochs_duration=config.rest_epochs_duration,
         rest_epochs_overlap=config.rest_epochs_overlap,
         _epochs_split_size=config._epochs_split_size,
+        runs=get_runs(config=config, subject=subject),
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config) -> None:
     """Run epochs."""
     with get_parallel_backend(config.exec_params):
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_06a_run_ica.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 
 import mne
 from mne.report import Report
 from mne.preprocessing import ICA, create_ecg_epochs, create_eog_epochs
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
-    get_sessions,
     get_runs,
+    get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_eeg_reference,
+    _bids_kwargs,
 )
 from ..._import_data import make_epochs, annotations_to_events
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._reject import _get_reject
 from ..._report import _agg_backend
 from ..._run import failsafe_run, _update_for_splits, save_logs
@@ -535,22 +534,16 @@
     *,
     config: SimpleNamespace,
     subject: Optional[str] = None,
     session: Optional[str] = None,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
         conditions=config.conditions,
-        task=get_task(config),
-        task_is_rest=config.task_is_rest,
-        datatype=get_datatype(config),
         runs=get_runs(config=config, subject=subject),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
+        task_is_rest=config.task_is_rest,
         ica_l_freq=config.ica_l_freq,
         ica_algorithm=config.ica_algorithm,
         ica_n_components=config.ica_n_components,
         ica_max_iterations=config.ica_max_iterations,
         ica_decim=config.ica_decim,
         ica_reject=config.ica_reject,
         ica_eog_threshold=config.ica_eog_threshold,
@@ -568,14 +561,15 @@
         epochs_metadata_keep_first=config.epochs_metadata_keep_first,
         epochs_metadata_keep_last=config.epochs_metadata_keep_last,
         epochs_metadata_query=config.epochs_metadata_query,
         eeg_reference=get_eeg_reference(config),
         eog_channels=config.eog_channels,
         rest_epochs_duration=config.rest_epochs_duration,
         rest_epochs_overlap=config.rest_epochs_overlap,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run ICA."""
     if config.spatial_filter != "ica":
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_06b_run_ssp.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import mne
 from mne.preprocessing import create_eog_epochs, create_ecg_epochs
 from mne import compute_proj_evoked, compute_proj_epochs
 from mne_bids import BIDSPath
 from mne.utils import _pl
 
 from ..._config_utils import (
-    get_sessions,
     get_runs,
+    get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
+    _bids_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._reject import _get_reject
 from ..._report import _open_report
 from ..._run import failsafe_run, _update_for_splits, save_logs
 
@@ -98,27 +97,33 @@
     minimums = dict(ecg=cfg.min_ecg_epochs, eog=cfg.min_eog_epochs)
     rejects = dict(ecg=cfg.ssp_reject_ecg, eog=cfg.ssp_reject_eog)
     avg = dict(ecg=cfg.ecg_proj_from_average, eog=cfg.eog_proj_from_average)
     n_projs = dict(ecg=cfg.n_proj_ecg, eog=cfg.n_proj_eog)
     ch_name = dict(ecg=None, eog=None)
     if cfg.eog_channels:
         ch_name["eog"] = cfg.eog_channels
-        assert all([ch_name in raw.ch_names for ch_name in ch_name["eog"]])
+        assert all(ch_name in raw.ch_names for ch_name in ch_name["eog"])
+    if cfg.ssp_ecg_channel:
+        ch_name["ecg"] = cfg.ssp_ecg_channel
+        assert ch_name["ecg"] in raw.ch_names, ch_name["ecg"]
     if cfg.ssp_meg == "auto":
         cfg.ssp_meg = "combined" if cfg.use_maxwell_filter else "separate"
     for kind in proj_kinds:
         projs[kind] = []
-        if not any(n_projs[kind]):
+        if not any(n_projs[kind].values()):
             continue
         proj_epochs = epochs_fun[kind](
-            raw, ch_name=ch_name[kind], decim=cfg.epochs_decim
+            raw,
+            ch_name=ch_name[kind],
+            decim=cfg.epochs_decim,
         )
-        n_orig = len(proj_epochs)
+        n_orig = len(proj_epochs.selection)
         rate = n_orig / raw.times[-1] * 60
-        msg = f"Detected {rate_names[kind]} rate: {rate:5.1f} bpm"
+        bpm_msg = f"{rate:5.1f} bpm"
+        msg = f"Detected {rate_names[kind]} rate: {bpm_msg}"
         logger.info(**gen_log_kwargs(message=msg))
         # Enough to start
         if len(proj_epochs) >= minimums[kind]:
             reject_ = _get_reject(
                 subject=subject,
                 session=session,
                 reject=rejects[kind],
@@ -136,49 +141,52 @@
                 f"{kind.upper()}-"
                 f"{proj_epochs.times[0]:0.3f}-"
                 f"{proj_epochs.times[-1]:0.3f})"
             )
             projs[kind] = fun(
                 use, meg=cfg.ssp_meg, **n_projs[kind], desc_prefix=desc_prefix
             )
-            out_files[f"{kind}_epochs"] = (
+            out_files[f"epochs_{kind}"] = (
                 out_files["proj"]
                 .copy()
                 .update(suffix=f"{kind}-epo", split=None, check=False)
             )
-            proj_epochs.save(out_files[f"{kind}_epochs"], overwrite=True)
+            proj_epochs.save(out_files[f"epochs_{kind}"], overwrite=True)
         else:
             msg = (
                 f"No {kind.upper()} projectors computed: got "
                 f"{len(proj_epochs)} good epochs < {minimums[kind]} "
-                f"(from {n_orig} original events)."
+                f"(from {n_orig} original events; {bpm_msg})."
             )
             logger.warning(**gen_log_kwargs(message=msg))
         del proj_epochs
 
     mne.write_proj(out_files["proj"], sum(projs.values(), []), overwrite=True)
     assert len(in_files) == 0, in_files.keys()
 
     # Report
     with _open_report(
         cfg=cfg, exec_params=exec_params, subject=subject, session=session
     ) as report:
         for kind in proj_kinds:
-            if f"epochs_{kind}" not in out_files:
+            key = f"epochs_{kind}"
+            if key not in out_files:
                 continue
 
             msg = f"Adding {kind.upper()} SSP to report."
             logger.info(**gen_log_kwargs(message=msg))
             proj_epochs = mne.read_epochs(out_files[f"epochs_{kind}"])
             projs = mne.read_proj(out_files["proj"])
             projs = [p for p in projs if kind.upper() in p["desc"]]
             assert len(projs), len(projs)  # should exist if the epochs do
             picks_trace = None
             if kind == "ecg":
-                if "ecg" in proj_epochs:
+                if cfg.ssp_ecg_channel:
+                    picks_trace = [cfg.ssp_ecg_channel]
+                elif "ecg" in proj_epochs:
                     picks_trace = "ecg"
             else:
                 assert kind == "eog"
                 if cfg.eog_channels:
                     picks_trace = cfg.eog_channels
                 elif "eog" in proj_epochs:
                     picks_trace = "eog"
@@ -202,34 +210,30 @@
 
 def get_config(
     *,
     config: SimpleNamespace,
     subject: str,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        runs=get_runs(config=config, subject=subject),
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
         eog_channels=config.eog_channels,
-        deriv_root=config.deriv_root,
+        ssp_ecg_channel=config.ssp_ecg_channel,
         ssp_reject_ecg=config.ssp_reject_ecg,
         ecg_proj_from_average=config.ecg_proj_from_average,
         ssp_reject_eog=config.ssp_reject_eog,
         eog_proj_from_average=config.eog_proj_from_average,
         min_ecg_epochs=config.min_ecg_epochs,
         min_eog_epochs=config.min_eog_epochs,
         n_proj_eog=config.n_proj_eog,
         n_proj_ecg=config.n_proj_ecg,
         ssp_meg=config.ssp_meg,
         ch_types=config.ch_types,
         epochs_decim=config.epochs_decim,
         use_maxwell_filter=config.use_maxwell_filter,
+        runs=get_runs(config=config, subject=subject),
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run SSP."""
     if config.spatial_filter != "ssp":
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_07a_apply_ica.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from mne.report import Report
 
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_subjects,
     get_sessions,
-    get_task,
-    get_datatype,
+    _bids_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._reject import _get_reject
 from ..._report import _open_report, _agg_backend
 from ..._run import failsafe_run, _update_for_splits, save_logs
 
@@ -177,24 +176,19 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         baseline=config.baseline,
         ica_reject=config.ica_reject,
         ch_types=config.ch_types,
         _epochs_split_size=config._epochs_split_size,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Apply ICA."""
     if not config.spatial_filter == "ica":
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_07b_apply_ssp.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
+    _bids_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._run import failsafe_run, _update_for_splits, save_logs
 from ..._parallel import parallel_func, get_parallel_backend
 
 
 def get_input_fnames_apply_ssp(
@@ -84,21 +83,16 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         _epochs_split_size=config._epochs_split_size,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Apply ssp."""
     if not config.spatial_filter == "ssp":
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/preprocessing/_08_ptp_reject.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
+    _bids_kwargs,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._reject import _get_reject
 from ..._report import _open_report
 from ..._run import failsafe_run, _update_for_splits, save_logs
 
@@ -159,28 +158,23 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
         baseline=config.baseline,
         reject_tmin=config.reject_tmin,
         reject_tmax=config.reject_tmax,
         spatial_filter=config.spatial_filter,
         ica_reject=config.ica_reject,
-        deriv_root=config.deriv_root,
         reject=config.reject,
         ch_types=config.ch_types,
         _epochs_split_size=config._epochs_split_size,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run epochs."""
     parallel, run_func = parallel_func(drop_ptp, exec_params=config.exec_params)
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_all_contrasts,
+    _bids_kwargs,
     _restrict_analyze_channels,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._report import _open_report, _sanitize_cond_tag
 from ..._run import failsafe_run, save_logs, _sanitize_callable
 
@@ -143,27 +142,21 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         conditions=config.conditions,
         contrasts=get_all_contrasts(config),
-        proc=config.proc,
         noise_cov=_sanitize_callable(config.noise_cov),
         analyze_channels=config.analyze_channels,
         ch_types=config.ch_types,
         report_evoked_n_time_points=config.report_evoked_n_time_points,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run evoked."""
     if config.task_is_rest:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 import mne
 from mne.decoding import Scaler, Vectorizer
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_eeg_reference,
-    _restrict_analyze_channels,
     get_decoding_contrasts,
+    _bids_kwargs,
+    _restrict_analyze_channels,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._decoding import LogReg
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._run import failsafe_run, save_logs
 from ..._report import (
     _open_report,
@@ -214,31 +213,26 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         conditions=config.conditions,
         contrasts=get_decoding_contrasts(config),
         decode=config.decode,
         decoding_metric=config.decoding_metric,
         decoding_epochs_tmin=config.decoding_epochs_tmin,
         decoding_epochs_tmax=config.decoding_epochs_tmax,
         decoding_n_splits=config.decoding_n_splits,
         random_state=config.random_state,
         analyze_channels=config.analyze_channels,
         ch_types=config.ch_types,
         eeg_reference=get_eeg_reference(config),
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run time-by-time decoding."""
     if not config.contrasts:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 from sklearn.preprocessing import StandardScaler
 from sklearn.pipeline import make_pipeline
 from sklearn.model_selection import StratifiedKFold
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_eeg_reference,
-    _restrict_analyze_channels,
     get_decoding_contrasts,
+    _bids_kwargs,
+    _restrict_analyze_channels,
 )
 from ..._decoding import LogReg
 from ..._logging import gen_log_kwargs, logger
 from ..._run import failsafe_run, save_logs
 from ..._parallel import get_parallel_backend, get_parallel_backend_name
 from ..._report import (
     _open_report,
@@ -291,31 +290,26 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         conditions=config.conditions,
         contrasts=get_decoding_contrasts(config),
         decode=config.decode,
         decoding_metric=config.decoding_metric,
         decoding_n_splits=config.decoding_n_splits,
         decoding_time_generalization=config.decoding_time_generalization,
         decoding_time_generalization_decim=config.decoding_time_generalization_decim,  # noqa: E501
         random_state=config.random_state,
         analyze_channels=config.analyze_channels,
         ch_types=config.ch_types,
         eeg_reference=get_eeg_reference(config),
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run time-by-time decoding."""
     if not config.contrasts:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 import mne
 
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
-    _restrict_analyze_channels,
     get_eeg_reference,
     sanitize_cond_name,
+    _bids_kwargs,
+    _restrict_analyze_channels,
 )
 from ..._logging import gen_log_kwargs, logger
 from ..._run import failsafe_run, save_logs
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._report import _open_report, _sanitize_cond_tag
 
 
@@ -158,32 +157,27 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        deriv_root=config.deriv_root,
         time_frequency_conditions=config.time_frequency_conditions,
         analyze_channels=config.analyze_channels,
         spatial_filter=config.spatial_filter,
         ch_types=config.ch_types,
         eeg_reference=get_eeg_reference(config),
         time_frequency_freq_min=config.time_frequency_freq_min,
         time_frequency_freq_max=config.time_frequency_freq_max,
         time_frequency_cycles=config.time_frequency_cycles,
         time_frequency_subtract_evoked=config.time_frequency_subtract_evoked,
         time_frequency_baseline=config.time_frequency_baseline,
         time_frequency_baseline_mode=config.time_frequency_baseline_mode,
         time_frequency_crop=config.time_frequency_crop,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run Time-frequency decomposition."""
     if not config.time_frequency_conditions:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 from sklearn.decomposition import PCA
 from sklearn.model_selection import StratifiedKFold, cross_val_score
 from sklearn.pipeline import make_pipeline
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_eeg_reference,
-    _restrict_analyze_channels,
     get_decoding_contrasts,
+    _bids_kwargs,
+    _restrict_analyze_channels,
 )
 from ..._decoding import LogReg, _handle_csp_args
 from ..._logging import logger, gen_log_kwargs
 from ..._parallel import parallel_func, get_parallel_backend
 from ..._run import failsafe_run, save_logs
 from ..._report import (
     _open_report,
@@ -509,33 +508,28 @@
 
 
 def get_config(
     *, config: SimpleNamespace, subject: str, session: Optional[str]
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
         # Data parameters
-        datatype=get_datatype(config),
-        deriv_root=config.deriv_root,
-        task=get_task(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
         use_maxwell_filter=config.use_maxwell_filter,
         analyze_channels=config.analyze_channels,
         ch_types=config.ch_types,
         eeg_reference=get_eeg_reference(config),
         # Processing parameters
         time_frequency_subtract_evoked=config.time_frequency_subtract_evoked,
         decoding_metric=config.decoding_metric,
         decoding_csp_freqs=config.decoding_csp_freqs,
         decoding_csp_times=config.decoding_csp_times,
         decoding_n_splits=config.decoding_n_splits,
         decoding_contrasts=get_decoding_contrasts(config),
         n_boot=config.n_boot,
         random_state=config.random_state,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run all subjects decoding in parallel."""
     if not config.contrasts or not config.decoding_csp:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_noise_cov_bids_path,
+    _bids_kwargs,
 )
 from ..._config_import import _import_config
 from ..._config_utils import _restrict_analyze_channels, get_all_contrasts
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._report import _open_report, _sanitize_cond_tag, _all_conditions
 from ..._run import failsafe_run, save_logs, _sanitize_callable
@@ -71,16 +70,16 @@
             processing="filt",
             suffix="raw",
             extension=".fif",
             datatype=cfg.datatype,
             root=cfg.deriv_root,
             check=False,
         )
-        data_type = "resting-state" if cfg.noise_cov == "rest" else "empty-room"
-        if data_type == "resting-state":
+        run_type = "resting-state" if cfg.noise_cov == "rest" else "empty-room"
+        if run_type == "resting-state":
             bids_path_raw_noise.task = "rest"
         else:
             bids_path_raw_noise.task = "noise"
         in_files["raw"] = bids_path_raw_noise
     else:
         assert cov_type == "epochs", cov_type
         in_files["epochs"] = fname_epochs
@@ -125,16 +124,16 @@
     exec_params: SimpleNamespace,
     subject: str,
     session: Optional[str],
     in_files: dict,
     out_files: dict,
 ) -> mne.Covariance:
     fname_raw = in_files.pop("raw")
-    data_type = "resting-state" if fname_raw.task == "rest" else "empty-room"
-    msg = f"Computing regularized covariance based on {data_type} recording."
+    run_type = "resting-state" if fname_raw.task == "rest" else "empty-room"
+    msg = f"Computing regularized covariance based on {run_type} recording."
     logger.info(**gen_log_kwargs(message=msg))
     msg = f"Input:  {fname_raw.basename}"
     logger.info(**gen_log_kwargs(message=msg))
     msg = f'Output: {out_files["cov"].basename}'
     logger.info(**gen_log_kwargs(message=msg))
 
     raw_noise = mne.io.read_raw_fif(fname_raw, preload=True)
@@ -279,28 +278,22 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        proc=config.proc,
         spatial_filter=config.spatial_filter,
         ch_types=config.ch_types,
-        deriv_root=config.deriv_root,
         run_source_estimation=config.run_source_estimation,
         noise_cov=_sanitize_callable(config.noise_cov),
         conditions=config.conditions,
         all_contrasts=get_all_contrasts(config),
         analyze_channels=config.analyze_channels,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run cov."""
     if not config.run_source_estimation:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_99_group_average.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/sensor/_99_group_average.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 
 import mne
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_sessions,
     get_subjects,
-    get_task,
-    get_datatype,
     get_eeg_reference,
     get_decoding_contrasts,
     get_all_contrasts,
+    _bids_kwargs,
 )
 from ..._decoding import _handle_csp_args
 from ..._logging import gen_log_kwargs, logger
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._run import failsafe_run, save_logs
 from ..._report import run_report_average_sensor
 
@@ -593,22 +592,15 @@
 def get_config(
     *,
     config,
 ) -> SimpleNamespace:
     dtg_decim = config.decoding_time_generalization_decim
     cfg = SimpleNamespace(
         subjects=get_subjects(config),
-        task=get_task(config),
         task_is_rest=config.task_is_rest,
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        proc=config.proc,
-        deriv_root=config.deriv_root,
         conditions=config.conditions,
         contrasts=get_all_contrasts(config),
         decode=config.decode,
         decoding_metric=config.decoding_metric,
         decoding_n_splits=config.decoding_n_splits,
         decoding_time_generalization=config.decoding_time_generalization,
         decoding_time_generalization_decim=dtg_decim,
@@ -621,20 +613,21 @@
         cluster_forming_t_threshold=config.cluster_forming_t_threshold,
         cluster_n_permutations=config.cluster_n_permutations,
         analyze_channels=config.analyze_channels,
         interpolate_bads_grand_average=config.interpolate_bads_grand_average,
         ch_types=config.ch_types,
         eeg_reference=get_eeg_reference(config),
         sessions=get_sessions(config),
-        bids_root=config.bids_root,
-        data_type=config.data_type,
         exclude_subjects=config.exclude_subjects,
         all_contrasts=get_all_contrasts(config),
         report_evoked_n_time_points=config.report_evoked_n_time_points,
         cluster_permutation_p_threshold=config.cluster_permutation_p_threshold,
+        # TODO: needed because get_datatype gets called again...
+        data_type=config.data_type,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 @failsafe_run()
 def run_group_average_sensor(
     *,
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_04_make_forward.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_04_make_forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 from mne_bids import BIDSPath, get_head_mri_trans
 
 from ..._config_utils import (
     get_fs_subject,
     get_subjects,
     _get_bem_conductivity,
     get_fs_subjects_dir,
-    get_task,
     get_runs,
-    get_datatype,
     _meg_in_ch_types,
     get_sessions,
+    _bids_kwargs,
 )
 from ..._config_import import _import_config
 from ..._logging import logger, gen_log_kwargs
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._report import _open_report
 from ..._run import failsafe_run, save_logs
 
@@ -239,30 +238,24 @@
 
 def get_config(
     *,
     config: SimpleNamespace,
     subject: str,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
         runs=get_runs(config=config, subject=subject),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
         mindist=config.mindist,
         spacing=config.spacing,
         use_template_mri=config.use_template_mri,
         adjust_coreg=config.adjust_coreg,
         source_info_path_update=config.source_info_path_update,
         ch_types=config.ch_types,
         fs_subject=get_fs_subject(config=config, subject=subject),
         fs_subjects_dir=get_fs_subjects_dir(config),
-        deriv_root=config.deriv_root,
-        bids_root=config.bids_root,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run forward."""
     if not config.run_source_estimation:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_05_make_inverse.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_05_make_inverse.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 )
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_noise_cov_bids_path,
     get_subjects,
     sanitize_cond_name,
-    get_task,
-    get_datatype,
     get_sessions,
     get_fs_subjects_dir,
     get_fs_subject,
+    _bids_kwargs,
 )
 from ..._logging import logger, gen_log_kwargs
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._report import _open_report, _sanitize_cond_tag
 from ..._run import failsafe_run, save_logs, _sanitize_callable
 
 
@@ -158,32 +157,26 @@
 
 def get_config(
     *,
     config: SimpleNamespace,
     subject: str,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        proc=config.proc,
-        space=config.space,
         source_info_path_update=config.source_info_path_update,
         inverse_targets=config.inverse_targets,
         ch_types=config.ch_types,
         conditions=config.conditions,
         loose=config.loose,
         depth=config.depth,
         inverse_method=config.inverse_method,
-        deriv_root=config.deriv_root,
         noise_cov=_sanitize_callable(config.noise_cov),
         report_stc_n_time_points=config.report_stc_n_time_points,
         fs_subject=get_fs_subject(config=config, subject=subject),
         fs_subjects_dir=get_fs_subjects_dir(config),
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 def main(*, config: SimpleNamespace) -> None:
     """Run inv."""
     if not config.run_source_estimation:
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_99_group_average.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/steps/source/_99_group_average.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 from mne_bids import BIDSPath
 
 from ..._config_utils import (
     get_fs_subjects_dir,
     get_subjects,
     sanitize_cond_name,
     get_fs_subject,
-    get_task,
-    get_datatype,
     get_sessions,
     get_all_contrasts,
+    _bids_kwargs,
 )
 from ..._logging import logger, gen_log_kwargs
 from ..._parallel import get_parallel_backend, parallel_func
 from ..._report import run_report_average_source
 from ..._run import failsafe_run, save_logs
 
 
@@ -122,35 +121,29 @@
 
 
 def get_config(
     *,
     config: SimpleNamespace,
 ) -> SimpleNamespace:
     cfg = SimpleNamespace(
-        task=get_task(config),
         task_is_rest=config.task_is_rest,
-        datatype=get_datatype(config),
-        acq=config.acq,
-        rec=config.rec,
-        space=config.space,
-        proc=config.proc,
         conditions=config.conditions,
         inverse_method=config.inverse_method,
         fs_subjects_dir=get_fs_subjects_dir(config),
-        deriv_root=config.deriv_root,
         subjects_dir=get_fs_subjects_dir(config),
-        bids_root=config.bids_root,
-        data_type=config.data_type,
         ch_types=config.ch_types,
         subjects=config.subjects,
         exclude_subjects=config.exclude_subjects,
         sessions=get_sessions(config),
         use_template_mri=config.use_template_mri,
         all_contrasts=get_all_contrasts(config),
         report_stc_n_time_points=config.report_stc_n_time_points,
+        # TODO: needed because get_datatype gets called again...
+        data_type=config.data_type,
+        **_bids_kwargs(config=config),
     )
     return cfg
 
 
 # pass 'average' subject for logging
 @failsafe_run()
 def run_group_average_source(
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 run_source_estimation = False
 
 on_rename_missing_events = "ignore"
 
 parallel_backend = "dask"
 dask_worker_memory_limit = "2G"
-n_jobs = 2
+n_jobs = 4
 
 if task == "N400":
     dask_open_dashboard = True
 
     rename_events = {
         "response/201": "response/correct",
         "response/202": "response/error",
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000117.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000117.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 bids_root = "~/mne_data/ds000117"
 deriv_root = "~/mne_data/derivatives/mne-bids-pipeline/ds000117"
 
 task = "facerecognition"
 ch_types = ["meg"]
 runs = ["01", "02"]
 sessions = ["meg"]
-interactive = False
-acq = None
 subjects = ["01"]
 
 raw_resample_sfreq = 125.0
 crop_runs = (0, 300)  # Reduce memory usage on CI system
 
-find_flat_channels_meg = False
-find_noisy_channels_meg = False
+find_flat_channels_meg = True
+find_noisy_channels_meg = True
 use_maxwell_filter = True
 
-mf_reference_run = "01"
+mf_reference_run = "02"
 mf_cal_fname = bids_root + "/derivatives/meg_derivatives/sss_cal.dat"
 mf_ctc_fname = bids_root + "/derivatives/meg_derivatives/ct_sparse.fif"
 
 reject = {"grad": 4000e-13, "mag": 4e-12}
 conditions = ["Famous", "Unfamiliar", "Scrambled"]
 contrasts = [
     ("Famous", "Scrambled"),
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000246.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000246.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000247.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000247.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003392.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds003392.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003775.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds003775.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004107.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/configs/config_ds004107.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 bids_root = f"~/mne_data/{study_name}"
 deriv_root = f"~/mne_data/derivatives/mne-bids-pipeline/{study_name}"
 subjects = ["mind002"]
 sessions = ["01"]
 conditions = ["left", "right"]  # there are also tone and noise
 task = "auditory"
 ch_types = ["meg"]
-crop_runs = (0, 100)  # to speed up computations
+crop_runs = (0, 120)  # to speed up computations
 spatial_filter = "ssp"
 l_freq = 1.0
 h_freq = 40.0
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/conftest.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,12 +27,15 @@
     ignore:`np.*` is a deprecated alias for .*:DeprecationWarning
     ignore:.*implicit namespace.*:DeprecationWarning
     ignore:Deprecated call to `pkg_resources.*:DeprecationWarning
     ignore:.*declare_namespace.*mpl_toolkits.*:DeprecationWarning
     ignore:_SixMetaPathImporter\.find_spec.*:ImportWarning
     ignore:pkg_resources is deprecated.*:DeprecationWarning
     ignore:`product` is deprecated as of NumPy.*:DeprecationWarning
+    # seaborn calling tight layout, etc.
+    ignore:The figure layout has changed to tight:UserWarning
+    ignore:The \S+_cmap function was deprecated.*:DeprecationWarning
     """
     for warning_line in warning_lines.split("\n"):
         warning_line = warning_line.strip()
         if warning_line and not warning_line.startswith("#"):
             config.addinivalue_line("filterwarnings", warning_line)
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/datasets.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/datasets.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_cli.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_documented.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_documented.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_run.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_validation.py` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/PKG-INFO` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-bids-pipeline
-Version: 1.3.0
+Version: 1.4.0
 Summary: A full-flegded processing pipeline for your MEG and EEG data
 Author: Eric Larson, Alexandre Gramfort, Mainak Jas
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License: Copyright © 2019-2022, authors of MNE-BIDS-Pipeline
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/SOURCES.txt` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 docs/source/governance.md
 docs/source/index.md
 docs/source/tags.md
 docs/source/v1.0.md.inc
 docs/source/v1.1.md.inc
 docs/source/v1.2.md.inc
 docs/source/v1.3.md.inc
+docs/source/v1.4.md.inc
 docs/source/assets/favicon.ico
 docs/source/assets/mne.svg
 docs/source/css/extra.css
 docs/source/examples/gen_examples.py
 docs/source/features/gen_steps.py
 docs/source/features/overview.md
 docs/source/getting_started/basic_usage.md
@@ -89,22 +90,23 @@
 mne_bids_pipeline/steps/freesurfer/contrib/README
 mne_bids_pipeline/steps/freesurfer/contrib/run.py
 mne_bids_pipeline/steps/freesurfer/contrib/version
 mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py
 mne_bids_pipeline/steps/init/_02_find_empty_room.py
 mne_bids_pipeline/steps/init/__init__.py
 mne_bids_pipeline/steps/preprocessing/_01_data_quality.py
-mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py
-mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py
-mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py
-mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py
-mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py
-mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py
-mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py
-mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py
+mne_bids_pipeline/steps/preprocessing/_02_head_pos.py
+mne_bids_pipeline/steps/preprocessing/_03_maxfilter.py
+mne_bids_pipeline/steps/preprocessing/_04_frequency_filter.py
+mne_bids_pipeline/steps/preprocessing/_05_make_epochs.py
+mne_bids_pipeline/steps/preprocessing/_06a_run_ica.py
+mne_bids_pipeline/steps/preprocessing/_06b_run_ssp.py
+mne_bids_pipeline/steps/preprocessing/_07a_apply_ica.py
+mne_bids_pipeline/steps/preprocessing/_07b_apply_ssp.py
+mne_bids_pipeline/steps/preprocessing/_08_ptp_reject.py
 mne_bids_pipeline/steps/preprocessing/__init__.py
 mne_bids_pipeline/steps/sensor/_01_make_evoked.py
 mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py
 mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py
 mne_bids_pipeline/steps/sensor/_04_time_frequency.py
 mne_bids_pipeline/steps/sensor/_05_decoding_csp.py
 mne_bids_pipeline/steps/sensor/_06_make_cov.py
```

### Comparing `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/requires.txt` & `mne-bids-pipeline-1.4.0/mne_bids_pipeline.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.3.0/pyproject.toml` & `mne-bids-pipeline-1.4.0/pyproject.toml`

 * *Files identical despite different names*

