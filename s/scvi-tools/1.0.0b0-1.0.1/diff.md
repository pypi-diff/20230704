# Comparing `tmp/scvi_tools-1.0.0b0.tar.gz` & `tmp/scvi_tools-1.0.1.tar.gz`

## Comparing `scvi_tools-1.0.0b0.tar` & `scvi_tools-1.0.1.tar`

### file list

```diff
@@ -1,345 +1,351 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.editorconfig
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitattributes
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitmodules
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/codecov.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/readthedocs.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/setup.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/build.yml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/test.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/Makefile
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/conf.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/index.md
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/installation.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/make.bat
--rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/references.bib
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/references.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/code-24px.svg
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/computer-24px.svg
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/library_books-24px.svg
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/logo.png
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/logo.svg
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/old_logo.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/play_circle_outline-24px.svg
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/scvi-tools-horizontal.svg
--rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/scvi_team.jpg
--rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks-01.png
--rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks.png
--rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/css/override.css
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/ldvae.svg
--rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/overview.svg
--rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/scanvi_alt.svg
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/totalvi_cell.svg
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/class_no_inherited.rst
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/layout.html
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/datasets.md
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/developer.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/index.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/user.md
--rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/contributing/index.md
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/extensions/edit_colab_url.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    76851 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/index.md
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/figures/anndata_manager_schematic.svg
--rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/figures/setup_anndata_before_after.svg
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_atac.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_dev.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_hub.md
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_multimodal.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_quick_start.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_scrna.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_spatial.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_tuning.md
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/codebase_overview.md
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/counterfactual_prediction.md
--rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/differential_expression.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/transfer_learning.md
--rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/variational_inference.md
--rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/codebase_overview.svg
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/fdr_control.png
--rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/vi_projection.svg
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/amortizedlda.md
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/autozi.md
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/cellassign.md
--rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/destvi.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/gimvi.md
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/linearscvi.md
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/multivi.md
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/peakvi.md
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scanvi.md
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scar.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scbasset.md
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scvi.md
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/solo.md
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/stereoscope.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/tangram.md
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/totalvi.md
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/fdr_control.png
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scLVM_graphical_model.svg
--rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scanvi_pgm.png
--rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stLVM_graphical_model.svg
--rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
--rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
--rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/totalvi_graphical_model.svg
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_compat.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_constants.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_decorators.py
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_settings.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_types.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_callbacks.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_defaults.py
--rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_manager.py
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_tuner.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_types.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_utils.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/__init__.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_anntorchdataset.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_constants.py
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_datasets.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_download.py
--rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_manager.py
--rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_preprocessing.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_read.py
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/__init__.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_brain_large.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cellxgene.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cite_seq.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cortex.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_csv.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_dataset_10x.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_heartcellatlas.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_loom.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_pbmc.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_smfish.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_synthetic.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/__init__.py
--rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_arraylike_field.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_base_field.py
--rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_dataframe_field.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_layer_field.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_mudata.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_protein.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_scanvi.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_uns_field.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_ann_dataloader.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_concat_dataloader.py
--rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_data_splitting.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_semi_dataloader.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/__init__.py
--rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/_negative_binomial.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/_utils.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/__init__.py
--rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/_model.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/_module.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/__init__.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_model.py
--rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_module.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_task.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_utils.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/__init__.py
--rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/_model.py
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/_module.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/__init__.py
--rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/_model.py
--rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/_module.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/solo/__init__.py
--rw-r--r--   0        0        0    15785 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/solo/_model.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/__init__.py
--rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/_model.py
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/_module.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/__init__.py
--rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/_model.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/_module.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/_constants.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/_url.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/hub_metadata.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/hub_model.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/model_card_template.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_amortizedlda.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_autozi.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_condscvi.py
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_destvi.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_jaxscvi.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_linear_scvi.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_metrics.py
--rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_multivi.py
--rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_peakvi.py
--rw-r--r--   0        0        0    21345 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_scanvi.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_scvi.py
--rw-r--r--   0        0        0    54416 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_totalvi.py
--rw-r--r--   0        0        0    13899 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_utils.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/__init__.py
--rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_archesmixin.py
--rw-r--r--   0        0        0    32259 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_base_model.py
--rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_differential.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_jaxmixin.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_log_likelihood.py
--rwxr-xr-x   0        0        0    20652 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_pyromixin.py
--rw-r--r--   0        0        0    28358 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_rnamixin.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_training_mixin.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_utils.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_vaemixin.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/_mde.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/_minification.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/__init__.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_amortizedlda.py
--rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_autozivae.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_classifier.py
--rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_jaxvae.py
--rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_mrdeconv.py
--rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_multivae.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_peakvae.py
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_scanvae.py
--rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_totalvae.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_utils.py
--rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_vae.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_vaec.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/__init__.py
--rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_base_module.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_decorators.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_pyro.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/__init__.py
--rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/_base_components.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/_utils.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/__init__.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_callbacks.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_logger.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_metrics.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_progress.py
--rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainer.py
--rw-r--r--   0        0        0    51487 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainingplans.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainrunner.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_attrdict.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_decorators.py
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_docstrings.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_exceptions.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_jax.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_track.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/conftest.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_defaults.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_manager.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_tuner.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_types.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_utils.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/core/test_differential.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/core/test_distributions.py
--rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Cortex.loom
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
--rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Layer2_BC_count_matrix-1.tsv
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Rep11_MOB_count_matrix-1.tsv
--rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/SeqFISH.xlsx
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/TM_droplet_mat.h5ad
--rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brain_large.h5
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brain_small_metadata.pickle
--rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brainlarge_dataset_test.h5ad
--rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/expression.bin
--rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/fc-dropseq.loom
--rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/immune_control_expression_matrix.txt
--rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/immune_stimulated_expression_matrix.txt
--rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/mpfc-starmap.loom
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/osmFISH_SScortex_mouse_all_cell.loom
--rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/pbmc_10k_protein_v3.h5ad
--rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/pbmc_5k_protein_v3.h5ad
--rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/random_metadata.pickle
--rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/retina.loom
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus.zip
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/gene_info_pbmc.csv
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc_metadata.pickle
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.spring_and_pba.csv
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/data.zip
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/ob_counts.csv
--rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_1.loom
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_2.loom
--rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_3.loom
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa.fai
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa.sizes
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.gaps.bed
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataloaders/test_datasplitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/conftest.py
--rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_anndata.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_built_in_data.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_dataset10X.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_mudata.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_preprocessing.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/utils.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_cellassign.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_gimvi.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_scar.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_scbasset.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_solo.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_stereoscope.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_tangram.py
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_hub_metadata.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_hub_model.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_lightning.py
--rw-r--r--   0        0        0    56424 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_models.py
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_models_with_minified_data.py
--rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_mudata_models.py
--rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_pyro.py
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_scarches.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/notebooks/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/train/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/train/test_trainingplans.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitignore
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/LICENSE
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/README.md
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.editorconfig
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitattributes
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitmodules
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/codecov.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/readthedocs.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/setup.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/index.md
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/installation.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/references.bib
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/references.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/code-24px.svg
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/computer-24px.svg
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/library_books-24px.svg
+-rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/logo.png
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/old_logo.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/scvi-tools-horizontal.svg
+-rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/scvi_team.jpg
+-rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks-01.png
+-rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks.png
+-rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/css/override.css
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/ldvae.svg
+-rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/overview.svg
+-rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/scanvi_alt.svg
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/totalvi_cell.svg
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/class_no_inherited.rst
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/layout.html
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/datasets.md
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/developer.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/index.md
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/user.md
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/contributing/index.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/extensions/edit_colab_url.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    78407 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/index.md
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/figures/anndata_manager_schematic.svg
+-rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/figures/setup_anndata_before_after.svg
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_atac.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_dev.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_hub.md
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_multimodal.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_quick_start.md
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_scrna.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_spatial.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_tuning.md
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/codebase_overview.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/counterfactual_prediction.md
+-rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/differential_expression.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/transfer_learning.md
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/variational_inference.md
+-rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/codebase_overview.svg
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/fdr_control.png
+-rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/vi_projection.svg
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/amortizedlda.md
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/autozi.md
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/cellassign.md
+-rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/destvi.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/gimvi.md
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/linearscvi.md
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/multivi.md
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/peakvi.md
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scanvi.md
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scar.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scbasset.md
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scvi.md
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/solo.md
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/stereoscope.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/tangram.md
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/totalvi.md
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/fdr_control.png
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scLVM_graphical_model.svg
+-rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scanvi_pgm.png
+-rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
+-rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
+-rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/totalvi_graphical_model.svg
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_compat.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_constants.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_decorators.py
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_settings.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_types.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_callbacks.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_defaults.py
+-rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_manager.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_tuner.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_types.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_utils.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/__init__.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/_constants.py
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/_ppc.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/__init__.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_anntorchdataset.py
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_compat.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_constants.py
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_datasets.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_download.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_manager.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_preprocessing.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_read.py
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/__init__.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_brain_large.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cellxgene.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cite_seq.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cortex.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_csv.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_dataset_10x.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_heartcellatlas.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_loom.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_pbmc.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_smfish.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_synthetic.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/__init__.py
+-rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_arraylike_field.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_base_field.py
+-rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_dataframe_field.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_layer_field.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_mudata.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_protein.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_scanvi.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_uns_field.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_ann_dataloader.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_concat_dataloader.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_data_splitting.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_semi_dataloader.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/__init__.py
+-rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/_negative_binomial.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/_utils.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/_model.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/_module.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/__init__.py
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_model.py
+-rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_module.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_task.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/__init__.py
+-rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/_model.py
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/_module.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/__init__.py
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/_model.py
+-rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/_module.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/solo/__init__.py
+-rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/solo/_model.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/__init__.py
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/_model.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/_module.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/__init__.py
+-rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/_model.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/_module.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/_constants.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/_url.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/hub_metadata.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/hub_model.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/model_card_template.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/__init__.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_amortizedlda.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_autozi.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_condscvi.py
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_destvi.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_jaxscvi.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_linear_scvi.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_metrics.py
+-rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_multivi.py
+-rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_peakvi.py
+-rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_scanvi.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_scvi.py
+-rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_totalvi.py
+-rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_utils.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/__init__.py
+-rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_archesmixin.py
+-rw-r--r--   0        0        0    33943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_base_model.py
+-rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_differential.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_jaxmixin.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_log_likelihood.py
+-rwxr-xr-x   0        0        0    20650 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_pyromixin.py
+-rw-r--r--   0        0        0    29147 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_rnamixin.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_training_mixin.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_utils.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_vaemixin.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/_mde.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/_minification.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/__init__.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_amortizedlda.py
+-rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_autozivae.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_classifier.py
+-rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_jaxvae.py
+-rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_mrdeconv.py
+-rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_multivae.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_peakvae.py
+-rw-r--r--   0        0        0    13210 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_scanvae.py
+-rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_totalvae.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_utils.py
+-rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_vae.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_vaec.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/__init__.py
+-rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_base_module.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_decorators.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_pyro.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/__init__.py
+-rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/_base_components.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/_utils.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/__init__.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_callbacks.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_logger.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_metrics.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_progress.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainer.py
+-rw-r--r--   0        0        0    51888 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainingplans.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainrunner.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_attrdict.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_decorators.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_docstrings.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_exceptions.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_jax.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_track.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_defaults.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_manager.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_tuner.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_types.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_utils.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/core/test_differential.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/core/test_distributions.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/criticism/test_criticism.py
+-rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Cortex.loom
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
+-rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Layer2_BC_count_matrix-1.tsv
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Rep11_MOB_count_matrix-1.tsv
+-rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/SeqFISH.xlsx
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/TM_droplet_mat.h5ad
+-rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brain_large.h5
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brain_small_metadata.pickle
+-rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brainlarge_dataset_test.h5ad
+-rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/expression.bin
+-rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/fc-dropseq.loom
+-rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/immune_control_expression_matrix.txt
+-rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/immune_stimulated_expression_matrix.txt
+-rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/mpfc-starmap.loom
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/osmFISH_SScortex_mouse_all_cell.loom
+-rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/pbmc_10k_protein_v3.h5ad
+-rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/pbmc_5k_protein_v3.h5ad
+-rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/random_metadata.pickle
+-rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/retina.loom
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus.zip
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/gene_info_pbmc.csv
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc_metadata.pickle
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.spring_and_pba.csv
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/data.zip
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/ob_counts.csv
+-rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_1.loom
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_2.loom
+-rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_3.loom
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa.fai
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa.sizes
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.gaps.bed
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataloaders/test_dataloaders.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataloaders/test_datasplitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/conftest.py
+-rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_anndata.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_built_in_data.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_dataset10X.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_mudata.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_preprocessing.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/utils.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_cellassign.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_gimvi.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_scar.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_scbasset.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_solo.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_stereoscope.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_tangram.py
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_hub_metadata.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_hub_model.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_url.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/model/base/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_lightning.py
+-rw-r--r--   0        0        0    57068 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_models.py
+-rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_models_with_minified_data.py
+-rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_mudata_models.py
+-rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_pyro.py
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_scarches.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/notebooks/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/train/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/train/test_trainingplans.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/README.md
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/PKG-INFO
```

### Comparing `scvi_tools-1.0.0b0/.pre-commit-config.yaml` & `scvi_tools-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/CODE_OF_CONDUCT.md` & `scvi_tools-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/.devcontainer/devcontainer.json` & `scvi_tools-1.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/.github/workflows/build.yml` & `scvi_tools-1.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/.github/workflows/release.yml` & `scvi_tools-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/.github/workflows/test.yml` & `scvi_tools-1.0.1/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,16 @@
                     - os: ubuntu-latest
                       python: "3.9"
                     - os: ubuntu-latest
                       python: "3.10"
                     - os: ubuntu-latest
                       python: "3.10"
                       pip-flags: "--pre"
+                    - os: ubuntu-latest
+                      python: "3.11"
 
         env:
             OS: ${{ matrix.os }}
             PYTHON: ${{ matrix.python }}
 
         steps:
             - uses: actions/checkout@v3
```

### Comparing `scvi_tools-1.0.0b0/docs/Makefile` & `scvi_tools-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/conf.py` & `scvi_tools-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/index.md` & `scvi_tools-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/installation.md` & `scvi_tools-1.0.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/make.bat` & `scvi_tools-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/references.bib` & `scvi_tools-1.0.1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/logo.png` & `scvi_tools-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/logo.svg` & `scvi_tools-1.0.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/old_logo.png` & `scvi_tools-1.0.1/docs/_static/old_logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/scvi-tools-horizontal.svg` & `scvi_tools-1.0.1/docs/_static/scvi-tools-horizontal.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/scvi_team.jpg` & `scvi_tools-1.0.1/docs/_static/scvi_team.jpg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tasks-01.png` & `scvi_tools-1.0.1/docs/_static/tasks-01.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tasks.png` & `scvi_tools-1.0.1/docs/_static/tasks.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tasks.svg` & `scvi_tools-1.0.1/docs/_static/tasks.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tutorials/ldvae.svg` & `scvi_tools-1.0.1/docs/_static/tutorials/ldvae.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tutorials/overview.svg` & `scvi_tools-1.0.1/docs/_static/tutorials/overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tutorials/scanvi_alt.svg` & `scvi_tools-1.0.1/docs/_static/tutorials/scanvi_alt.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_static/tutorials/totalvi_cell.svg` & `scvi_tools-1.0.1/docs/_static/tutorials/totalvi_cell.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_templates/class_no_inherited.rst` & `scvi_tools-1.0.1/docs/_templates/class_no_inherited.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_templates/layout.html` & `scvi_tools-1.0.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/_templates/autosummary/class.rst` & `scvi_tools-1.0.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/api/datasets.md` & `scvi_tools-1.0.1/docs/api/datasets.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/api/developer.md` & `scvi_tools-1.0.1/docs/api/developer.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/api/user.md` & `scvi_tools-1.0.1/docs/api/user.md`

 * *Files 7% similar despite different names*

```diff
@@ -122,25 +122,31 @@
 ## Model hub
 
 We have a hub for pre-trained `scvi-tools` models that is hosted on [huggingface](https://huggingface.co/models).
 Using the functionality that `scvi-tools` provides, users can download pre-trained `scvi-tools` models (and datasets)
 from this platform, and model generators can upload their own pre-trained `scvi-tools` models to this platform.
 
 ```{eval-rst}
-.. currentmodule:: scvi
+.. autosummary::
+   :toctree: reference/
+   :nosignatures:
+
+   hub.HubMetadata
+   hub.HubModelCardHelper
+   hub.HubModel
 ```
 
+## Model criticism
+
 ```{eval-rst}
 .. autosummary::
    :toctree: reference/
    :nosignatures:
 
-   scvi.hub.HubMetadata
-   scvi.hub.HubModelCardHelper
-   scvi.hub.HubModel
+   criticism.PosteriorPredictiveCheck
 ```
 
 ## Utilities
 
 Here we maintain miscellaneous general methods.
 
 ```{eval-rst}
```

### Comparing `scvi_tools-1.0.0b0/docs/contributing/index.md` & `scvi_tools-1.0.1/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/extensions/edit_colab_url.py` & `scvi_tools-1.0.1/docs/extensions/edit_colab_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/extensions/typed_returns.py` & `scvi_tools-1.0.1/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/release_notes/index.md` & `scvi_tools-1.0.1/docs/release_notes/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,31 +13,53 @@
 
 #### Removed
 
 -   Remove deprecated `use_gpu` in favor of PyTorch Lightning arguments `accelerator` and `devices` {pr}`xxxx`.
 
 ## Version 1.0
 
-### 1.0.0 (2023-MM-DD)
+### 1.0.1 (2023-07-04)
 
 #### Added
 
+-   Add support for Python 3.11 {pr}`1977`.
+
+#### Changed
+
+-   Upper bound Chex dependency to 0.1.8 due to NumPy installation conflicts {pr}`2132`.
+
+### 1.0.0 (2023-06-02)
+
+#### Added
+
+-   Add {class}`scvi.criticism.PosteriorPredictiveCheck` for model evaluation {pr}`2058`.
 -   Add {func}`scvi.data.reads_to_fragments` for scATAC data {pr}`1946`
 -   Add default `stacklevel` for `warnings` in `scvi.settings` {pr}`1971`.
 -   Add scBasset motif injection procedure {pr}`2010`.
 -   Add importance sampling based differential expression procedure {pr}`1872`.
+-   Raise clearer error when initializing {class}`scvi.external.SOLO` from {class}`scvi.model.SCVI` with extra categorical or continuous covariates {pr}`2027`.
 -   Add option to generate {class}`mudata.MuData` in {meth}`scvi.data.synthetic_iid` {pr}`2028`.
 -   Add option for disabling shuffling prior to splitting data in {class}`scvi.dataloaders.DataSplitter` {pr}`2037`.
 -   Add {meth}`scvi.data.AnnDataManager.create_torch_dataset` and expose custom sampler ability {pr}`2036`.
+-   Log training loss through Lightning's progress bar {pr}`2043`.
+-   Filter Jax undetected GPU warnings {pr}`2044`.
+-   Raise warning if MPS backend is selected for PyTorch, see https://github.com/pytorch/pytorch/issues/77764 {pr}`2045`.
+-   Add `deregister_manager` function to {class}`scvi.model.base.BaseModelClass`, allowing to clear
+    {class}`scvi.data.AnnDataManager` instances from memory {pr}`2060`.
+-   Add option to use a linear classifier in {class}`scvi.model.SCANVI` {pr}`2063`.
+-   Add lower bound 0.12.1 for Numpyro dependency {pr}`2078`.
+-   Add new section in scBasset tutorial for motif scoring {pr}`2079`.
 
 #### Fixed
 
 -   Fix creation of minified adata by copying original uns dict {pr}`2000`. This issue arises with anndata>=0.9.0.
 -   Fix {class}`scvi.model.TOTALVI` {class}`scvi.model.MULTIVI` handling of missing protein values {pr}`2009`.
 -   Fix bug in {meth}`scvi.distributions.NegativeBinomialMixture.sample` where `theta` and `mu` arguments were switched around {pr}`2024`.
+-   Fix bug in {meth}`scvi.dataloaders.SemiSupervisedDataLoader.resample_labels` where the labeled dataloader was not being reinitialized on subsample {pr}`2032`.
+-   Fix typo in {class}`scvi.model.JaxSCVI` example snippet {pr}`2075`.
 
 #### Changed
 
 -   Use sphinx book theme for documentation {pr}`1673`.
 -   {meth}`scvi.model.base.RNASeqMixin.posterior_predictive_sample` now outputs 3-d {class}`sparse.GCXS` matrices {pr}`1902`.
 -   Add an option to specify `dropout_ratio` in {meth}`scvi.data.synthetic_iid` {pr}`1920`.
 -   Update to lightning 2.0 {pr}`1961`
@@ -50,14 +72,16 @@
 -   Validate training data and code URLs for {class}`scvi.hub.HubMetadata` and {class}`scvi.hub.HubModelCardHelper` {pr}`1985`.
 -   Keyword arguments for encoders and decoders can now be passed in from the model level {pr}`1986`.
 -   Expose `local_dir` as a public property in {class}`scvi.hub.HubModel` {pr}`1994`.
 -   Use {func}`anndata.concat` internally inside {meth}`scvi.external.SOLO.from_scvi_model` {pr}`2013`.
 -   {class}`scvi.train.SemiSupervisedTrainingPlan` and {class}`scvi.train.ClassifierTrainingPlan` now log accuracy,
     F1 score, and AUROC metrics {pr}`2023`.
 -   Switch to cellxgene census for backend for cellxgene data function {pr}`2030`.
+-   Change default `max_cells` and `truncation` in {meth}`scvi.model.base.RNASeqMixin._get_importance_weights` {pr}`2064`.
+-   Refactor heuristic for default `max_epochs` as a separate function {meth}`scvi.model._utils.get_max_epochs_heuristic` {pr}`2083`.
 
 #### Removed
 
 -   Remove ability to set up ST data in {class}`~scvi.external.SpatialStereoscope.from_rna_model`, which was deprecated. ST data should be set up using {class}`~scvi.external.SpatialStereoscope.setup_anndata` {pr}`1949`.
 -   Remove custom reusable doc decorator which was used for de docs {pr}`1970`.
 -   Remove `drop_last` as an integer from {class}`~scvi.dataloaders.AnnDataLoader`, add typing and code cleanup {pr}`1975`.
 -   Remove seqfish and seqfish plus datasets {pr}`2017`.
```

### Comparing `scvi_tools-1.0.0b0/docs/release_notes/figures/anndata_manager_schematic.svg` & `scvi_tools-1.0.1/docs/release_notes/figures/anndata_manager_schematic.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/release_notes/figures/setup_anndata_before_after.svg` & `scvi_tools-1.0.1/docs/release_notes/figures/setup_anndata_before_after.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/tutorials/index.md` & `scvi_tools-1.0.1/docs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/tutorials/index_dev.md` & `scvi_tools-1.0.1/docs/tutorials/index_dev.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/index.md` & `scvi_tools-1.0.1/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/differential_expression.md` & `scvi_tools-1.0.1/docs/user_guide/background/differential_expression.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/transfer_learning.md` & `scvi_tools-1.0.1/docs/user_guide/background/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/variational_inference.md` & `scvi_tools-1.0.1/docs/user_guide/background/variational_inference.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/figures/codebase_overview.svg` & `scvi_tools-1.0.1/docs/user_guide/background/figures/codebase_overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/figures/fdr_control.png` & `scvi_tools-1.0.1/docs/user_guide/background/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/background/figures/vi_projection.svg` & `scvi_tools-1.0.1/docs/user_guide/background/figures/vi_projection.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/amortizedlda.md` & `scvi_tools-1.0.1/docs/user_guide/models/amortizedlda.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/autozi.md` & `scvi_tools-1.0.1/docs/user_guide/models/autozi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/cellassign.md` & `scvi_tools-1.0.1/docs/user_guide/models/cellassign.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/destvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/destvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/linearscvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/linearscvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/multivi.md` & `scvi_tools-1.0.1/docs/user_guide/models/multivi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/peakvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/peakvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/scanvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/scanvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/scar.md` & `scvi_tools-1.0.1/docs/user_guide/models/scar.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/scbasset.md` & `scvi_tools-1.0.1/docs/user_guide/models/scbasset.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/scvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/scvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/solo.md` & `scvi_tools-1.0.1/docs/user_guide/models/solo.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/stereoscope.md` & `scvi_tools-1.0.1/docs/user_guide/models/stereoscope.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/tangram.md` & `scvi_tools-1.0.1/docs/user_guide/models/tangram.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/totalvi.md` & `scvi_tools-1.0.1/docs/user_guide/models/totalvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/fdr_control.png` & `scvi_tools-1.0.1/docs/user_guide/models/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scLVM_graphical_model.svg` & `scvi_tools-1.0.1/docs/user_guide/models/figures/scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scanvi_pgm.png` & `scvi_tools-1.0.1/docs/user_guide/models/figures/scanvi_pgm.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png` & `scvi_tools-1.0.1/docs/user_guide/models/figures/scvi_annotated_graphical_model.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stLVM_graphical_model.svg` & `scvi_tools-1.0.1/docs/user_guide/models/figures/stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg` & `scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg` & `scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/docs/user_guide/models/figures/totalvi_graphical_model.svg` & `scvi_tools-1.0.1/docs/user_guide/models/figures/totalvi_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/__init__.py` & `scvi_tools-1.0.1/scvi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 """scvi-tools."""
 
 # Set default logging handler to avoid logging with logging.lastResort logger.
 import logging
+import warnings
 
 from ._constants import METRIC_KEYS, REGISTRY_KEYS
 from ._settings import settings
 
 # this import needs to come after prior imports to prevent circular import
-from . import autotune, data, model, external, utils
+from . import autotune, data, model, external, utils, criticism
 
 from importlib.metadata import version
 
 package_name = "scvi-tools"
 __version__ = version(package_name)
 
 settings.verbosity = logging.INFO
 test_var = "test"
 
 # Jax sets the root logger, this prevents double output.
 scvi_logger = logging.getLogger("scvi")
 scvi_logger.propagate = False
 
+# ignore Jax GPU warnings
+warnings.filterwarnings("ignore", message="No GPU/TPU found, falling back to CPU.")
+
 __all__ = [
     "settings",
     "REGISTRY_KEYS",
     "METRIC_KEYS",
     "autotune",
     "data",
     "model",
     "external",
     "utils",
+    "criticism",
 ]
```

### Comparing `scvi_tools-1.0.0b0/scvi/_constants.py` & `scvi_tools-1.0.1/scvi/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/_decorators.py` & `scvi_tools-1.0.1/scvi/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/_settings.py` & `scvi_tools-1.0.1/scvi/_settings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_callbacks.py` & `scvi_tools-1.0.1/scvi/autotune/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_defaults.py` & `scvi_tools-1.0.1/scvi/autotune/_defaults.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_manager.py` & `scvi_tools-1.0.1/scvi/autotune/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_tuner.py` & `scvi_tools-1.0.1/scvi/autotune/_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_types.py` & `scvi_tools-1.0.1/scvi/autotune/_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/autotune/_utils.py` & `scvi_tools-1.0.1/scvi/autotune/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/__init__.py` & `scvi_tools-1.0.1/scvi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_anntorchdataset.py` & `scvi_tools-1.0.1/scvi/data/_anntorchdataset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_compat.py` & `scvi_tools-1.0.1/scvi/data/_compat.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_constants.py` & `scvi_tools-1.0.1/scvi/data/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_datasets.py` & `scvi_tools-1.0.1/scvi/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_download.py` & `scvi_tools-1.0.1/scvi/data/_download.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_manager.py` & `scvi_tools-1.0.1/scvi/data/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_preprocessing.py` & `scvi_tools-1.0.1/scvi/data/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_read.py` & `scvi_tools-1.0.1/scvi/data/_read.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_utils.py` & `scvi_tools-1.0.1/scvi/data/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_brain_large.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_brain_large.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cellxgene.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_cellxgene.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cite_seq.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_cite_seq.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cortex.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_cortex.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_csv.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_csv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_dataset_10x.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_dataset_10x.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_heartcellatlas.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_heartcellatlas.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_loom.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_loom.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_pbmc.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_pbmc.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_smfish.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_smfish.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_synthetic.py` & `scvi_tools-1.0.1/scvi/data/_built_in_data/_synthetic.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/__init__.py` & `scvi_tools-1.0.1/scvi/data/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_arraylike_field.py` & `scvi_tools-1.0.1/scvi/data/fields/_arraylike_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_base_field.py` & `scvi_tools-1.0.1/scvi/data/fields/_base_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_dataframe_field.py` & `scvi_tools-1.0.1/scvi/data/fields/_dataframe_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_layer_field.py` & `scvi_tools-1.0.1/scvi/data/fields/_layer_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_mudata.py` & `scvi_tools-1.0.1/scvi/data/fields/_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_protein.py` & `scvi_tools-1.0.1/scvi/data/fields/_protein.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_scanvi.py` & `scvi_tools-1.0.1/scvi/data/fields/_scanvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/data/fields/_uns_field.py` & `scvi_tools-1.0.1/scvi/data/fields/_uns_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/dataloaders/__init__.py` & `scvi_tools-1.0.1/scvi/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/dataloaders/_ann_dataloader.py` & `scvi_tools-1.0.1/scvi/dataloaders/_ann_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/dataloaders/_concat_dataloader.py` & `scvi_tools-1.0.1/scvi/dataloaders/_concat_dataloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,25 +36,32 @@
         indices_list: List[List[int]],
         shuffle: bool = False,
         batch_size: int = 128,
         data_and_attributes: Optional[dict] = None,
         drop_last: Union[bool, int] = False,
         **data_loader_kwargs,
     ):
+        self.adata_manager = adata_manager
+        self.dataloader_kwargs = data_loader_kwargs
+        self.data_and_attributes = data_and_attributes
+        self._shuffle = shuffle
+        self._batch_size = batch_size
+        self._drop_last = drop_last
+
         self.dataloaders = []
         for indices in indices_list:
             self.dataloaders.append(
                 AnnDataLoader(
                     adata_manager,
                     indices=indices,
                     shuffle=shuffle,
                     batch_size=batch_size,
                     data_and_attributes=data_and_attributes,
                     drop_last=drop_last,
-                    **data_loader_kwargs,
+                    **self.dataloader_kwargs,
                 )
             )
         lens = [len(dl) for dl in self.dataloaders]
         self.largest_dl = self.dataloaders[np.argmax(lens)]
         super().__init__(self.largest_dl, **data_loader_kwargs)
 
     def __len__(self):
```

### Comparing `scvi_tools-1.0.0b0/scvi/dataloaders/_data_splitting.py` & `scvi_tools-1.0.1/scvi/dataloaders/_data_splitting.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/dataloaders/_semi_dataloader.py` & `scvi_tools-1.0.1/scvi/dataloaders/_semi_dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 
 from scvi import REGISTRY_KEYS
 from scvi.data import AnnDataManager
 from scvi.data._utils import get_anndata_attribute
 
+from ._ann_dataloader import AnnDataLoader
 from ._concat_dataloader import ConcatDataLoader
 
 
 class SemiSupervisedDataLoader(ConcatDataLoader):
     """DataLoader that supports semisupervised training.
 
     Parameters
@@ -85,15 +86,22 @@
 
     def resample_labels(self):
         """Resamples the labeled data."""
         labelled_idx = self.subsample_labels()
         # self.dataloaders[0] iterates over full_indices
         # self.dataloaders[1] iterates over the labelled_indices
         # change the indices of the labelled set
-        self.dataloaders[1].indices = labelled_idx
+        self.dataloaders[1] = AnnDataLoader(
+            self.adata_manager,
+            indices=labelled_idx,
+            shuffle=self._shuffle,
+            batch_size=self._batch_size,
+            data_and_attributes=self.data_and_attributes,
+            drop_last=self._drop_last,
+        )
 
     def subsample_labels(self):
         """Subsamples each label class by taking up to n_samples_per_label samples per class."""
         if self.n_samples_per_label is None:
             return np.concatenate(self.labeled_locs)
 
         sample_idx = []
```

### Comparing `scvi_tools-1.0.0b0/scvi/distributions/_negative_binomial.py` & `scvi_tools-1.0.1/scvi/distributions/_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/distributions/_utils.py` & `scvi_tools-1.0.1/scvi/distributions/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/cellassign/_model.py` & `scvi_tools-1.0.1/scvi/external/cellassign/_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     CategoricalObsField,
     LayerField,
     NumericalJointObsField,
     NumericalObsField,
 )
 from scvi.dataloaders import DataSplitter
 from scvi.external.cellassign._module import CellAssignModule
+from scvi.model._utils import get_max_epochs_heuristic
 from scvi.model.base import BaseModelClass, UnsupervisedTrainingMixin
 from scvi.train import LoudEarlyStopping, TrainingPlan, TrainRunner
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
@@ -201,16 +202,15 @@
             if "callbacks" in kwargs:
                 kwargs["callbacks"] += early_stopping_callback
             else:
                 kwargs["callbacks"] = early_stopping_callback
             kwargs["check_val_every_n_epoch"] = 1
 
         if max_epochs is None:
-            n_cells = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = DataSplitter(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0b0/scvi/external/cellassign/_module.py` & `scvi_tools-1.0.1/scvi/external/cellassign/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/gimvi/_model.py` & `scvi_tools-1.0.1/scvi/external/gimvi/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/gimvi/_module.py` & `scvi_tools-1.0.1/scvi/external/gimvi/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/gimvi/_task.py` & `scvi_tools-1.0.1/scvi/external/gimvi/_task.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/gimvi/_utils.py` & `scvi_tools-1.0.1/scvi/external/gimvi/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/scar/_model.py` & `scvi_tools-1.0.1/scvi/external/scar/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/scar/_module.py` & `scvi_tools-1.0.1/scvi/external/scar/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/scbasset/_model.py` & `scvi_tools-1.0.1/scvi/external/scbasset/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/scbasset/_module.py` & `scvi_tools-1.0.1/scvi/external/scbasset/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/solo/_model.py` & `scvi_tools-1.0.1/scvi/external/solo/_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from anndata import AnnData
 
 from scvi import REGISTRY_KEYS, settings
 from scvi.data import AnnDataManager
 from scvi.data.fields import CategoricalObsField, LayerField
 from scvi.dataloaders import DataSplitter
 from scvi.model import SCVI
+from scvi.model._utils import get_max_epochs_heuristic
 from scvi.model.base import BaseModelClass
 from scvi.module import Classifier
 from scvi.module.base import auto_move_data
 from scvi.train import ClassifierTrainingPlan, LoudEarlyStopping, TrainRunner
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
@@ -103,42 +104,69 @@
         **classifier_kwargs,
     ):
         """Instantiate a SOLO model from an scvi model.
 
         Parameters
         ----------
         scvi_model
-            Pre-trained model of :class:`~scvi.model.SCVI`. The
-            adata object used to initialize this model should have only
-            been setup with count data, and optionally a `batch_key`;
-            i.e., no extra covariates or labels, etc.
+            Pre-trained :class:`~scvi.model.SCVI` model. The AnnData object used to
+            initialize this model should have only been setup with count data, and
+            optionally a `batch_key`. Extra categorical and continuous covariates are
+            currenty unsupported.
         adata
-            Optional anndata to use that is compatible with scvi_model.
+            Optional AnnData to use that is compatible with `scvi_model`.
         restrict_to_batch
-            Batch category in `batch_key` used to setup adata for scvi_model
-            to restrict Solo model to. This allows to train a Solo model on
-            one batch of a scvi_model that was trained on multiple batches.
+            Batch category to restrict the SOLO model to if `scvi_model` was set up with
+            a `batch_key`. This allows the model to be trained on the subset of cells
+            belonging to `restrict_to_batch` when `scvi_model` was trained on multiple
+            batches. If `None`, all cells are used.
         doublet_ratio
             Ratio of generated doublets to produce relative to number of
             cells in adata or length of indices, if not `None`.
         **classifier_kwargs
             Keyword args for :class:`~scvi.module.Classifier`
 
         Returns
         -------
         SOLO model
         """
         _validate_scvi_model(scvi_model, restrict_to_batch=restrict_to_batch)
         orig_adata_manager = scvi_model.adata_manager
-        orig_batch_key = orig_adata_manager.get_state_registry(
+        orig_batch_key_registry = orig_adata_manager.get_state_registry(
             REGISTRY_KEYS.BATCH_KEY
-        ).original_key
-        orig_labels_key = orig_adata_manager.get_state_registry(
+        )
+        orig_labels_key_registry = orig_adata_manager.get_state_registry(
             REGISTRY_KEYS.LABELS_KEY
-        ).original_key
+        )
+        orig_batch_key = orig_batch_key_registry.original_key
+        orig_labels_key = orig_labels_key_registry.original_key
+
+        if len(orig_adata_manager.get_state_registry(REGISTRY_KEYS.CONT_COVS_KEY)) > 0:
+            raise ValueError(
+                "Initializing a SOLO model from SCVI with registered continuous "
+                "covariates is currently unsupported."
+            )
+        if len(orig_adata_manager.get_state_registry(REGISTRY_KEYS.CAT_COVS_KEY)) > 0:
+            raise ValueError(
+                "Initializing a SOLO model from SCVI with registered categorical "
+                "covariates is currently unsupported."
+            )
+        scvi_trained_with_batch = len(orig_batch_key_registry.categorical_mapping) > 1
+        if not scvi_trained_with_batch and restrict_to_batch is not None:
+            raise ValueError(
+                "Cannot specify `restrict_to_batch` when initializing a SOLO model from SCVI "
+                "not trained with multiple batches."
+            )
+        if scvi_trained_with_batch > 1 and restrict_to_batch is None:
+            warnings.warn(
+                "`restrict_to_batch` not specified but `scvi_model` was trained with "
+                "multiple batches. Doublets will be simulated using the first batch.",
+                UserWarning,
+                stacklevel=settings.warnings_stacklevel,
+            )
 
         if adata is not None:
             adata_manager = orig_adata_manager.transfer_fields(adata)
             cls.register_manager(adata_manager)
         else:
             adata_manager = orig_adata_manager
         adata = adata_manager.adata
@@ -161,21 +189,23 @@
         # anndata with only generated doublets
         doublet_adata = cls.create_doublets(
             adata_manager, indices=batch_indices, doublet_ratio=doublet_ratio
         )
         # if scvi wasn't trained with batch correction having the
         # zeros here does nothing.
         doublet_adata.obs[orig_batch_key] = (
-            restrict_to_batch if restrict_to_batch is not None else 0
+            restrict_to_batch
+            if restrict_to_batch is not None
+            else orig_adata_manager.get_state_registry(
+                REGISTRY_KEYS.BATCH_KEY
+            ).categorical_mapping[0]
         )
 
         # Create dummy labels column set to first label in adata (does not affect inference).
-        dummy_label = orig_adata_manager.get_state_registry(
-            REGISTRY_KEYS.LABELS_KEY
-        ).categorical_mapping[0]
+        dummy_label = orig_labels_key_registry.categorical_mapping[0]
         doublet_adata.obs[orig_labels_key] = dummy_label
 
         # if model is using observed lib size, needs to get lib sample
         # which is just observed lib size on log scale
         give_mean_lib = not scvi_model.module.use_observed_lib_size
 
         # get latent representations and make input anndata
@@ -325,16 +355,15 @@
             if "callbacks" in kwargs:
                 kwargs["callbacks"] += early_stopping_callback
             else:
                 kwargs["callbacks"] = early_stopping_callback
             kwargs["check_val_every_n_epoch"] = 1
 
         if max_epochs is None:
-            n_cells = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = DataSplitter(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0b0/scvi/external/stereoscope/_model.py` & `scvi_tools-1.0.1/scvi/external/stereoscope/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/stereoscope/_module.py` & `scvi_tools-1.0.1/scvi/external/stereoscope/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/tangram/_model.py` & `scvi_tools-1.0.1/scvi/external/tangram/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/external/tangram/_module.py` & `scvi_tools-1.0.1/scvi/external/tangram/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/hub/_constants.py` & `scvi_tools-1.0.1/scvi/hub/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/hub/_url.py` & `scvi_tools-1.0.1/scvi/hub/_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/hub/hub_metadata.py` & `scvi_tools-1.0.1/scvi/hub/hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/hub/hub_model.py` & `scvi_tools-1.0.1/scvi/hub/hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/hub/model_card_template.py` & `scvi_tools-1.0.1/scvi/hub/model_card_template.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/__init__.py` & `scvi_tools-1.0.1/scvi/model/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_amortizedlda.py` & `scvi_tools-1.0.1/scvi/model/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_autozi.py` & `scvi_tools-1.0.1/scvi/model/_autozi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_condscvi.py` & `scvi_tools-1.0.1/scvi/model/_condscvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_destvi.py` & `scvi_tools-1.0.1/scvi/model/_destvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_jaxscvi.py` & `scvi_tools-1.0.1/scvi/model/_jaxscvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     **model_kwargs
         Keyword args for :class:`~scvi.module.JaxVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.model.JaxSCVI.setup_anndata(adata, batch_key="batch")
-    >>> vae = scvi.model.SCVI(adata)
+    >>> vae = scvi.model.JaxSCVI(adata)
     >>> vae.train()
     >>> adata.obsm["X_scVI"] = vae.get_latent_representation()
     """
 
     _module_cls = JaxVAE
 
     def __init__(
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/_linear_scvi.py` & `scvi_tools-1.0.1/scvi/model/_linear_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_metrics.py` & `scvi_tools-1.0.1/scvi/model/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_multivi.py` & `scvi_tools-1.0.1/scvi/model/_multivi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_peakvi.py` & `scvi_tools-1.0.1/scvi/model/_peakvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_scanvi.py` & `scvi_tools-1.0.1/scvi/model/_scanvi.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     LayerField,
     NumericalJointObsField,
     NumericalObsField,
     ObsmField,
     StringUnsField,
 )
 from scvi.dataloaders import SemiSupervisedDataSplitter
-from scvi.model._utils import _init_library_size
+from scvi.model._utils import _init_library_size, get_max_epochs_heuristic
 from scvi.model.utils import get_minified_adata_scrna
 from scvi.module import SCANVAE
 from scvi.train import SemiSupervisedTrainingPlan, TrainRunner
 from scvi.train._callbacks import SubSampleLabels
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
@@ -73,14 +73,17 @@
         * ``'gene-cell'`` - dispersion can differ for every gene in every cell
     gene_likelihood
         One of:
 
         * ``'nb'`` - Negative binomial distribution
         * ``'zinb'`` - Zero-inflated negative binomial distribution
         * ``'poisson'`` - Poisson distribution
+    linear_classifier
+        If `True`, uses a single linear layer for classification instead of a
+        multi-layer perceptron.
     **model_kwargs
         Keyword args for :class:`~scvi.module.SCANVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.model.SCANVI.setup_anndata(adata, batch_key="batch", labels_key="labels")
@@ -95,24 +98,26 @@
 
     1. :doc:`/tutorials/notebooks/harmonization`
     2. :doc:`/tutorials/notebooks/scarches_scvi_tools`
     3. :doc:`/tutorials/notebooks/seed_labeling`
     """
 
     _module_cls = SCANVAE
+    _training_plan_cls = SemiSupervisedTrainingPlan
 
     def __init__(
         self,
         adata: AnnData,
         n_hidden: int = 128,
         n_latent: int = 10,
         n_layers: int = 1,
         dropout_rate: float = 0.1,
         dispersion: Literal["gene", "gene-batch", "gene-label", "gene-cell"] = "gene",
         gene_likelihood: Literal["zinb", "nb", "poisson"] = "zinb",
+        linear_classifier: bool = False,
         **model_kwargs,
     ):
         super().__init__(adata)
         scanvae_model_kwargs = dict(model_kwargs)
 
         self._set_indices_and_labels()
 
@@ -147,14 +152,15 @@
             n_layers=n_layers,
             dropout_rate=dropout_rate,
             dispersion=dispersion,
             gene_likelihood=gene_likelihood,
             use_size_factor_key=use_size_factor_key,
             library_log_means=library_log_means,
             library_log_vars=library_log_vars,
+            linear_classifier=linear_classifier,
             **scanvae_model_kwargs,
         )
         self.module.minified_data_type = self.minified_data_type
 
         self.unsupervised_history_ = None
         self.semisupervised_history_ = None
 
@@ -385,16 +391,15 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.SemiSupervisedTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            n_cells = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
             if self.was_pretrained:
                 max_epochs = int(np.min([10, np.max([2, round(max_epochs / 3.0)])]))
 
         logger.info(f"Training for {max_epochs} epochs.")
 
         plan_kwargs = {} if plan_kwargs is None else plan_kwargs
@@ -408,15 +413,15 @@
             adata_manager=self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
             shuffle_set_split=shuffle_set_split,
             n_samples_per_label=n_samples_per_label,
             batch_size=batch_size,
         )
-        training_plan = SemiSupervisedTrainingPlan(
+        training_plan = self._training_plan_cls(
             self.module, self.n_labels, **plan_kwargs
         )
         if "callbacks" in trainer_kwargs.keys():
             trainer_kwargs["callbacks"].concatenate(sampler_callback)
         else:
             trainer_kwargs["callbacks"] = sampler_callback
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/_scvi.py` & `scvi_tools-1.0.1/scvi/model/_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/_totalvi.py` & `scvi_tools-1.0.1/scvi/model/_totalvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from scvi.data._utils import _check_nonnegative_integers
 from scvi.dataloaders import DataSplitter
 from scvi.model._utils import (
     _get_batch_code_from_category,
     _get_var_names_from_manager,
     _init_library_size,
     cite_seq_raw_counts_properties,
+    get_max_epochs_heuristic,
 )
 from scvi.model.base._utils import _de_core
 from scvi.module import TOTALVAE
 from scvi.train import AdversarialTrainingPlan, TrainRunner
 from scvi.utils._docstrings import de_dsp, devices_dsp, setup_anndata_dsp
 
 from .base import ArchesMixin, BaseModelClass, RNASeqMixin, VAEMixin
@@ -277,16 +278,15 @@
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
             plan_kwargs = update_dict
 
         if max_epochs is None:
-            n_cells = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = self._data_splitter_cls(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/_utils.py` & `scvi_tools-1.0.1/scvi/model/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,52 @@
 from scvi.data import AnnDataManager
 from scvi.utils._docstrings import devices_dsp
 from scvi.utils._exceptions import InvalidParameterError
 
 logger = logging.getLogger(__name__)
 
 
+def get_max_epochs_heuristic(
+    n_obs: int, epochs_cap: int = 400, decay_at_n_obs: int = 20000
+) -> int:
+    """Compute a heuristic for the default number of maximum epochs.
+
+    If `n_obs <= decay_at_n_obs`, the number of maximum epochs is set to
+    `epochs_cap`. Otherwise, the number of maximum epochs decays according to
+    `(decay_at_n_obs / n_obs) * epochs_cap`, with a minimum of 1.
+
+    Parameters
+    ----------
+    n_obs
+        The number of observations in the dataset.
+    epochs_cap
+        The maximum number of epochs for the heuristic.
+    decay_at_n_obs
+        The number of observations at which the heuristic starts decaying.
+
+    Returns
+    -------
+    `int`
+        A heuristic for the default number of maximum epochs.
+    """
+    max_epochs = min(round((decay_at_n_obs / n_obs) * epochs_cap), epochs_cap)
+    max_epochs = max(max_epochs, 1)
+
+    if max_epochs == 1:
+        warnings.warn(
+            "The default number of maximum epochs has been set to 1 due to the large"
+            "number of observations. Pass in `max_epochs` to the `train` function in "
+            "order to override this behavior.",
+            UserWarning,
+            stacklevel=settings.warnings_stacklevel,
+        )
+
+    return max_epochs
+
+
 @devices_dsp.dedent
 def parse_device_args(
     use_gpu: Optional[Union[str, int, bool]] = None,
     accelerator: str = "auto",
     devices: Union[int, List[int], str] = "auto",
     return_device: Optional[Literal["torch", "jax"]] = None,
     validate_single_device: bool = False,
@@ -64,20 +102,29 @@
 
     connector = _AcceleratorConnector(accelerator=accelerator, devices=devices)
     _accelerator = connector._accelerator_flag
     _devices = connector._devices_flag
 
     if _accelerator in ["tpu", "ipu", "hpu"]:
         warnings.warn(
-            f"The selected accelerator `{_accelerator}` has not been extensively ",
+            f"The selected accelerator `{_accelerator}` has not been extensively "
             "tested in scvi-tools. Please report any issues in the GitHub repo.",
             UserWarning,
             stacklevel=settings.warnings_stacklevel,
         )
 
+    if _accelerator == "mps":
+        warnings.warn(
+            "The accelerator has been set to `mps`. Please note that not all PyTorch "
+            "operations are supported with this backend. Refer to "
+            "https://github.com/pytorch/pytorch/issues/77764 for more details.",
+            UserWarning,
+            stacklevel=settings.warnings_stacklevel,
+        )
+
     # get the first device index
     if isinstance(_devices, list):
         device_idx = _devices[0]
     elif isinstance(_devices, str) and "," in _devices:
         device_idx = _devices.split(",")[0]
     else:
         device_idx = _devices
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/__init__.py` & `scvi_tools-1.0.1/scvi/model/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_archesmixin.py` & `scvi_tools-1.0.1/scvi/model/base/_archesmixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_base_model.py` & `scvi_tools-1.0.1/scvi/model/base/_base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,14 +220,50 @@
         if self.id not in self._per_instance_manager_store:
             self._per_instance_manager_store[self.id] = {}
 
         adata_id = adata_manager.adata_uuid
         instance_manager_store = self._per_instance_manager_store[self.id]
         instance_manager_store[adata_id] = adata_manager
 
+    def deregister_manager(self, adata: Optional[AnnData] = None):
+        """Deregisters the :class:`~scvi.data.AnnDataManager` instance associated with `adata`.
+
+        If `adata` is `None`, deregisters all :class:`~scvi.data.AnnDataManager` instances
+        in both the class and instance-specific manager stores, except for the one associated
+        with this model instance.
+        """
+        cls_manager_store = self._setup_adata_manager_store
+        instance_manager_store = self._per_instance_manager_store[self.id]
+
+        if adata is None:
+            instance_managers_to_clear = list(instance_manager_store.keys())
+            cls_managers_to_clear = list(cls_manager_store.keys())
+        else:
+            adata_manager = self._get_most_recent_anndata_manager(adata, required=True)
+            cls_managers_to_clear = [adata_manager.adata_uuid]
+            instance_managers_to_clear = [adata_manager.adata_uuid]
+
+        for adata_id in cls_managers_to_clear:
+            # don't clear the current manager by default
+            is_current_adata = (
+                adata is None and adata_id == self.adata_manager.adata_uuid
+            )
+            if is_current_adata or adata_id not in cls_manager_store:
+                continue
+            del cls_manager_store[adata_id]
+
+        for adata_id in instance_managers_to_clear:
+            # don't clear the current manager by default
+            is_current_adata = (
+                adata is None and adata_id == self.adata_manager.adata_uuid
+            )
+            if is_current_adata or adata_id not in instance_manager_store:
+                continue
+            del instance_manager_store[adata_id]
+
     @classmethod
     def _get_most_recent_anndata_manager(
         cls, adata: AnnOrMuData, required: bool = False
     ) -> Optional[AnnDataManager]:
         """Retrieves the :class:`~scvi.data.AnnDataManager` for a given AnnData object specific to this model class.
 
         Checks for the most recent :class:`~scvi.data.AnnDataManager` created for the given AnnData object via
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_differential.py` & `scvi_tools-1.0.1/scvi/model/base/_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_jaxmixin.py` & `scvi_tools-1.0.1/scvi/model/base/_jaxmixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import warnings
 from typing import List, Optional, Union
 
 import jax
-import numpy as np
 
 from scvi.dataloaders import DataSplitter
+from scvi.model._utils import get_max_epochs_heuristic
 from scvi.train import JaxModuleInit, JaxTrainingPlan, TrainRunner
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
 
 class JaxTrainingMixin:
@@ -58,16 +58,15 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.JaxTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            n_cells = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
         if use_gpu is None or use_gpu is True:
             try:
                 self.module.to(jax.devices("gpu")[0])
                 logger.info(
                     "Jax module moved to GPU. "
                     "Note: Pytorch lightning will show GPU is not being used for the Trainer."
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_log_likelihood.py` & `scvi_tools-1.0.1/scvi/model/base/_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_pyromixin.py` & `scvi_tools-1.0.1/scvi/model/base/_pyromixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import torch
 from lightning.pytorch.callbacks import Callback
 from pyro import poutine
 
 from scvi import settings
 from scvi.dataloaders import AnnDataLoader, DataSplitter, DeviceBackedDataSplitter
-from scvi.model._utils import parse_device_args
+from scvi.model._utils import get_max_epochs_heuristic, parse_device_args
 from scvi.train import PyroTrainingPlan, TrainRunner
 from scvi.utils import track
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
 
@@ -130,16 +130,15 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.PyroTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            n_obs = self.adata.n_obs
-            max_epochs = int(np.min([round((20000 / n_obs) * 1000), 1000]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs, epochs_cap=1000)
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
         if lr is not None and "optim" not in plan_kwargs.keys():
             plan_kwargs.update({"optim_kwargs": {"lr": lr}})
 
         if batch_size is None:
             # use data splitter which moves data to GPU once
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_rnamixin.py` & `scvi_tools-1.0.1/scvi/model/base/_rnamixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     def _get_importance_weights(
         self,
         adata: Optional[AnnData],
         indices: Optional[Sequence[int]],
         qz: db.Distribution,
         px: db.Distribution,
         zs: torch.Tensor,
-        max_cells: int = 128,
-        truncation: bool = True,
+        max_cells: int = 1024,
+        truncation: bool = False,
         n_mc_samples: int = 500,
         n_mc_samples_per_pass: int = 250,
     ) -> np.ndarray:
         """Computes importance weights for the given samples.
 
         This method computes importance weights for every latent code in `zs` as a way to
         encourage latent codes providing high likelihoods across many cells in the considered
@@ -153,14 +153,15 @@
         library_size: Union[float, Literal["latent"]] = 1,
         n_samples: int = 1,
         n_samples_overall: int = None,
         weights: Optional[Literal["uniform", "importance"]] = None,
         batch_size: Optional[int] = None,
         return_mean: bool = True,
         return_numpy: Optional[bool] = None,
+        **importance_weighting_kwargs,
     ) -> Union[np.ndarray, pd.DataFrame]:
         r"""Returns the normalized (decoded) gene expression.
 
         This is denoted as :math:`\rho_n` in the scVI paper.
 
         Parameters
         ----------
@@ -193,14 +194,16 @@
             Minibatch size for data loading into model. Defaults to `scvi.settings.batch_size`.
         return_mean
             Whether to return the mean of the samples.
         return_numpy
             Return a :class:`~numpy.ndarray` instead of a :class:`~pandas.DataFrame`. DataFrame includes
             gene names as columns. If either `n_samples=1` or `return_mean=True`, defaults to `False`.
             Otherwise, it defaults to `True`.
+        importance_weighting_kwargs
+            Keyword arguments passed into :meth:`~scvi.model.base.RNASeqMixin._get_importance_weights`.
 
         Returns
         -------
         If `n_samples` is provided and `return_mean` is False,
         this method returns a 3d tensor of shape (n_samples, n_cells, n_genes).
         If `n_samples` is provided and `return_mean` is True, it returns a 2d tensor
         of shape (n_cells, n_genes).
@@ -292,14 +295,15 @@
                 px = px_store.get_concatenated_distributions(axis=x_axis)
                 p = self._get_importance_weights(
                     adata,
                     indices,
                     qz=qz,
                     px=px,
                     zs=zs,
+                    **importance_weighting_kwargs,
                 )
             ind_ = np.random.choice(n_samples_, n_samples_overall, p=p, replace=True)
             exprs = exprs[ind_]
         elif n_samples > 1 and return_mean:
             exprs = exprs.mean(0)
 
         if return_numpy is None or return_numpy is False:
@@ -327,14 +331,15 @@
         batch_correction: bool = False,
         batchid1: Optional[Iterable[str]] = None,
         batchid2: Optional[Iterable[str]] = None,
         fdr_target: float = 0.05,
         silent: bool = False,
         weights: Optional[Literal["uniform", "importance"]] = "uniform",
         filter_outlier_cells: bool = False,
+        importance_weighting_kwargs: Optional[dict] = None,
         **kwargs,
     ) -> pd.DataFrame:
         r"""A unified method for differential expression analysis.
 
         Implements ``'vanilla'`` DE :cite:p:`Lopez18` and ``'change'`` mode DE :cite:p:`Boyeau19`.
 
         Parameters
@@ -350,29 +355,37 @@
         %(de_batch_size)s
         %(de_all_stats)s
         %(de_batch_correction)s
         %(de_batchid1)s
         %(de_batchid2)s
         %(de_fdr_target)s
         %(de_silent)s
+        weights
+            Weights to use for sampling. If `None`, defaults to `"uniform"`.
+        filter_outlier_cells
+            Whether to filter outlier cells with :meth:`~scvi.model.base.DifferentialComputation.filter_outlier_cells`.
+        importance_weighting_kwargs
+            Keyword arguments passed into :meth:`~scvi.model.base.RNASeqMixin._get_importance_weights`.
         **kwargs
             Keyword args for :meth:`scvi.model.base.DifferentialComputation.get_bayes_factors`
 
         Returns
         -------
         Differential expression DataFrame.
         """
         adata = self._validate_anndata(adata)
         col_names = adata.var_names
+        importance_weighting_kwargs = importance_weighting_kwargs or {}
         model_fn = partial(
             self.get_normalized_expression,
             return_numpy=True,
             n_samples=1,
             batch_size=batch_size,
             weights=weights,
+            **importance_weighting_kwargs,
         )
         representation_fn = (
             self.get_latent_representation if filter_outlier_cells else None
         )
 
         result = _de_core(
             self.get_anndata_manager(adata, required=True),
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_training_mixin.py` & `scvi_tools-1.0.1/scvi/model/base/_training_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Optional, Union
 
-import numpy as np
-
 from scvi.dataloaders import DataSplitter
+from scvi.model._utils import get_max_epochs_heuristic
 from scvi.train import TrainingPlan, TrainRunner
 from scvi.utils._docstrings import devices_dsp
 
 
 class UnsupervisedTrainingMixin:
     """General purpose unsupervised train method."""
 
@@ -54,17 +53,16 @@
             See :class:`~scvi.train.Trainer` for further options.
         plan_kwargs
             Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
-        n_cells = self.adata.n_obs
         if max_epochs is None:
-            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = self._data_splitter_cls(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_utils.py` & `scvi_tools-1.0.1/scvi/model/base/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/base/_vaemixin.py` & `scvi_tools-1.0.1/scvi/model/base/_vaemixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/utils/_mde.py` & `scvi_tools-1.0.1/scvi/model/utils/_mde.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/model/utils/_minification.py` & `scvi_tools-1.0.1/scvi/model/utils/_minification.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/__init__.py` & `scvi_tools-1.0.1/scvi/module/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_amortizedlda.py` & `scvi_tools-1.0.1/scvi/module/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_autozivae.py` & `scvi_tools-1.0.1/scvi/module/_autozivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_classifier.py` & `scvi_tools-1.0.1/scvi/module/_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,21 @@
     """Basic fully-connected NN classifier.
 
     Parameters
     ----------
     n_input
         Number of input dimensions
     n_hidden
-        Number of hidden nodes in hidden layer
+        Number of nodes in hidden layer(s). If `0`, the classifier only consists of a
+        single linear layer.
     n_labels
         Numput of outputs dimensions
     n_layers
-        Number of hidden layers
+        Number of hidden layers. If `0`, the classifier only consists of a single
+        linear layer.
     dropout_rate
         dropout_rate for nodes
     logits
         Return logits or not
     use_batch_norm
         Whether to use batch norm in layers
     use_layer_norm
@@ -41,28 +43,35 @@
         use_batch_norm: bool = True,
         use_layer_norm: bool = False,
         activation_fn: nn.Module = nn.ReLU,
         **kwargs,
     ):
         super().__init__()
         self.logits = logits
-        layers = [
-            FCLayers(
-                n_in=n_input,
-                n_out=n_hidden,
-                n_layers=n_layers,
-                n_hidden=n_hidden,
-                dropout_rate=dropout_rate,
-                use_batch_norm=use_batch_norm,
-                use_layer_norm=use_layer_norm,
-                activation_fn=activation_fn,
-                **kwargs,
-            ),
-            nn.Linear(n_hidden, n_labels),
-        ]
+        layers = []
+
+        if n_hidden > 0 and n_layers > 0:
+            layers.append(
+                FCLayers(
+                    n_in=n_input,
+                    n_out=n_hidden,
+                    n_layers=n_layers,
+                    n_hidden=n_hidden,
+                    dropout_rate=dropout_rate,
+                    use_batch_norm=use_batch_norm,
+                    use_layer_norm=use_layer_norm,
+                    activation_fn=activation_fn,
+                    **kwargs,
+                )
+            )
+        else:
+            n_hidden = n_input
+
+        layers.append(nn.Linear(n_hidden, n_labels))
+
         if not logits:
             layers.append(nn.Softmax(dim=-1))
 
         self.classifier = nn.Sequential(*layers)
 
     def forward(self, x):
         """Forward computation."""
```

### Comparing `scvi_tools-1.0.0b0/scvi/module/_jaxvae.py` & `scvi_tools-1.0.1/scvi/module/_jaxvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_mrdeconv.py` & `scvi_tools-1.0.1/scvi/module/_mrdeconv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_multivae.py` & `scvi_tools-1.0.1/scvi/module/_multivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_peakvae.py` & `scvi_tools-1.0.1/scvi/module/_peakvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_scanvae.py` & `scvi_tools-1.0.1/scvi/module/_scanvae.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,18 +58,24 @@
         * ``'zinb'`` - Zero-inflated negative binomial distribution
     y_prior
         If None, initialized to uniform probability over cell types
     labels_groups
         Label group designations
     use_labels_groups
         Whether to use the label groups
+    linear_classifier
+        If `True`, uses a single linear layer for classification instead of a
+        multi-layer perceptron.
+    classifier_parameters
+        Keyword arguments passed into :class:`~scvi.module.Classifier`.
     use_batch_norm
         Whether to use batch norm in layers
     use_layer_norm
         Whether to use layer norm in layers
+    linear_classifier
     **vae_kwargs
         Keyword args for :class:`~scvi.module.VAE`
     """
 
     def __init__(
         self,
         n_input: int,
@@ -85,14 +91,15 @@
             Literal["gene", "gene-batch", "gene-label", "gene-cell"]
         ] = "gene",
         log_variational: Tunable[bool] = True,
         gene_likelihood: Tunable[Literal["zinb", "nb"]] = "zinb",
         y_prior=None,
         labels_groups: Sequence[int] = None,
         use_labels_groups: bool = False,
+        linear_classifier: bool = False,
         classifier_parameters: Optional[dict] = None,
         use_batch_norm: Tunable[Literal["encoder", "decoder", "none", "both"]] = "both",
         use_layer_norm: Tunable[Literal["encoder", "decoder", "none", "both"]] = "none",
         **vae_kwargs,
     ):
         super().__init__(
             n_input,
@@ -116,16 +123,16 @@
         use_batch_norm_decoder = use_batch_norm == "decoder" or use_batch_norm == "both"
         use_layer_norm_encoder = use_layer_norm == "encoder" or use_layer_norm == "both"
         use_layer_norm_decoder = use_layer_norm == "decoder" or use_layer_norm == "both"
 
         self.n_labels = n_labels
         # Classifier takes n_latent as input
         cls_parameters = {
-            "n_layers": n_layers,
-            "n_hidden": n_hidden,
+            "n_layers": 0 if linear_classifier else n_layers,
+            "n_hidden": 0 if linear_classifier else n_hidden,
             "dropout_rate": dropout_rate,
         }
         cls_parameters.update(classifier_parameters)
         self.classifier = Classifier(
             n_latent,
             n_labels=n_labels,
             use_batch_norm=use_batch_norm_encoder,
```

### Comparing `scvi_tools-1.0.0b0/scvi/module/_totalvae.py` & `scvi_tools-1.0.1/scvi/module/_totalvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_utils.py` & `scvi_tools-1.0.1/scvi/module/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_vae.py` & `scvi_tools-1.0.1/scvi/module/_vae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/_vaec.py` & `scvi_tools-1.0.1/scvi/module/_vaec.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/base/_base_module.py` & `scvi_tools-1.0.1/scvi/module/base/_base_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/module/base/_decorators.py` & `scvi_tools-1.0.1/scvi/module/base/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/nn/_base_components.py` & `scvi_tools-1.0.1/scvi/nn/_base_components.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/__init__.py` & `scvi_tools-1.0.1/scvi/train/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_callbacks.py` & `scvi_tools-1.0.1/scvi/train/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_logger.py` & `scvi_tools-1.0.1/scvi/train/_logger.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_metrics.py` & `scvi_tools-1.0.1/scvi/train/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_progress.py` & `scvi_tools-1.0.1/scvi/train/_progress.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_trainer.py` & `scvi_tools-1.0.1/scvi/train/_trainer.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/train/_trainingplans.py` & `scvi_tools-1.0.1/scvi/train/_trainingplans.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     def training_step(self, batch, batch_idx):
         """Training step for the model."""
         if "kl_weight" in self.loss_kwargs:
             kl_weight = self.kl_weight
             self.loss_kwargs.update({"kl_weight": kl_weight})
             self.log("kl_weight", kl_weight, on_step=True, on_epoch=False)
         _, _, scvi_loss = self.forward(batch, loss_kwargs=self.loss_kwargs)
-        self.log("train_loss", scvi_loss.loss, on_epoch=True)
+        self.log("train_loss", scvi_loss.loss, on_epoch=True, prog_bar=True)
         self.compute_and_log_metrics(scvi_loss, self.train_metrics, "train")
         return scvi_loss.loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for the model."""
         # loss kwargs here contains `n_obs` equal to n_training_obs
         # so when relevant, the actual loss value is rescaled to number
@@ -559,15 +559,15 @@
         z = inference_outputs["z"]
         loss = scvi_loss.loss
         # fool classifier if doing adversarial training
         if kappa > 0 and self.adversarial_classifier is not False:
             fool_loss = self.loss_adversarial_classifier(z, batch_tensor, False)
             loss += fool_loss * kappa
 
-        self.log("train_loss", loss, on_epoch=True)
+        self.log("train_loss", loss, on_epoch=True, prog_bar=True)
         self.compute_and_log_metrics(scvi_loss, self.train_metrics, "train")
         opt1.zero_grad()
         self.manual_backward(loss)
         opt1.step()
 
         # train adversarial classifier
         # this condition will not be met unless self.adversarial_classifier is not False
@@ -712,17 +712,18 @@
         )
         self.loss_kwargs.update({"classification_ratio": classification_ratio})
         self.initialize_metrics(n_classes)
 
     def initialize_metrics(self, n_classes: int):
         """Initialize metrics."""
         kwargs = {"task": "multiclass", "num_classes": n_classes}
-        self.accuracy = Accuracy(**kwargs)
-        self.f1 = F1Score(**kwargs)
-        self.auroc = AUROC(**kwargs)
+        self.train_accuracy = Accuracy(**kwargs)
+        self.train_f1 = F1Score(**kwargs)
+        self.val_accuracy = Accuracy(**kwargs)
+        self.val_f1 = F1Score(**kwargs)
 
     def log_with_mode(self, key: str, value: Any, mode: str, **kwargs):
         """Log with mode."""
         # TODO: Include this with a base training plan
         self.log(f"{mode}_{key}", value, **kwargs)
 
     def compute_and_log_metrics(
@@ -736,38 +737,47 @@
             return
 
         classification_loss = loss_output.classification_loss
         true_labels = loss_output.true_labels
         logits = loss_output.logits
         predicted_labels = torch.argmax(logits, dim=-1, keepdim=True)
 
-        self.accuracy(predicted_labels, true_labels)
-        self.f1(predicted_labels, true_labels)
-        self.auroc(logits, true_labels.view(-1).long())
+        if mode == "train":
+            accuracy = self.train_accuracy
+            f1 = self.train_f1
+        else:
+            accuracy = self.val_accuracy
+            f1 = self.val_f1
+
+        accuracy(predicted_labels, true_labels)
+        f1(predicted_labels, true_labels)
 
         self.log_with_mode(
             METRIC_KEYS.CLASSIFICATION_LOSS_KEY,
             classification_loss,
             mode,
             on_step=False,
             on_epoch=True,
+            batch_size=loss_output.n_obs_minibatch,
         )
         self.log_with_mode(
             METRIC_KEYS.ACCURACY_KEY,
-            self.accuracy,
+            accuracy,
             mode,
             on_step=False,
             on_epoch=True,
+            batch_size=loss_output.n_obs_minibatch,
         )
         self.log_with_mode(
             METRIC_KEYS.F1_SCORE_KEY,
-            self.f1,
+            f1,
             mode,
             on_step=False,
             on_epoch=True,
+            batch_size=loss_output.n_obs_minibatch,
         )
         # currently not logging auroc due to accumulation error
 
     def training_step(self, batch, batch_idx):
         """Training step for semi-supervised training."""
         # Potentially dangerous if batch is from a single dataloader with two keys
         if len(batch) == 2:
@@ -787,14 +797,15 @@
         _, _, loss_output = self.forward(full_dataset, loss_kwargs=input_kwargs)
         loss = loss_output.loss
         self.log(
             "train_loss",
             loss,
             on_epoch=True,
             batch_size=loss_output.n_obs_minibatch,
+            prog_bar=True,
         )
         self.compute_and_log_metrics(loss_output, self.train_metrics, "train")
         return loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for semi-supervised training."""
         # Potentially dangerous if batch is from a single dataloader with two keys
@@ -1152,15 +1163,15 @@
         self.log_with_mode(METRIC_KEYS.F1_SCORE_KEY, self.f1, mode)
         self.log_with_mode(METRIC_KEYS.AUROC_KEY, self.auroc, mode)
 
     def training_step(self, batch, batch_idx):
         """Training step for classifier training."""
         soft_prediction = self.forward(batch[self.data_key])
         loss = self.loss_fn(soft_prediction, batch[self.labels_key].view(-1).long())
-        self.log("train_loss", loss, on_epoch=True)
+        self.log("train_loss", loss, on_epoch=True, prog_bar=True)
         return loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for classifier training."""
         soft_prediction = self.forward(batch[self.data_key])
         loss = self.loss_fn(soft_prediction, batch[self.labels_key].view(-1).long())
         self.log("validation_loss", loss)
```

### Comparing `scvi_tools-1.0.0b0/scvi/train/_trainrunner.py` & `scvi_tools-1.0.1/scvi/train/_trainrunner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/utils/_decorators.py` & `scvi_tools-1.0.1/scvi/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/utils/_docstrings.py` & `scvi_tools-1.0.1/scvi/utils/_docstrings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/utils/_exceptions.py` & `scvi_tools-1.0.1/scvi/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/scvi/utils/_track.py` & `scvi_tools-1.0.1/scvi/utils/_track.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/conftest.py` & `scvi_tools-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/autotune/test_manager.py` & `scvi_tools-1.0.1/tests/autotune/test_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/autotune/test_tuner.py` & `scvi_tools-1.0.1/tests/autotune/test_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/autotune/test_types.py` & `scvi_tools-1.0.1/tests/autotune/test_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/core/test_differential.py` & `scvi_tools-1.0.1/tests/core/test_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/core/test_distributions.py` & `scvi_tools-1.0.1/tests/core/test_distributions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/Cortex.loom` & `scvi_tools-1.0.1/tests/data/Cortex.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz` & `scvi_tools-1.0.1/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/Layer2_BC_count_matrix-1.tsv` & `scvi_tools-1.0.1/tests/data/Layer2_BC_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/Rep11_MOB_count_matrix-1.tsv` & `scvi_tools-1.0.1/tests/data/Rep11_MOB_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/SeqFISH.xlsx` & `scvi_tools-1.0.1/tests/data/SeqFISH.xlsx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/TM_droplet_mat.h5ad` & `scvi_tools-1.0.1/tests/data/TM_droplet_mat.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/brain_large.h5` & `scvi_tools-1.0.1/tests/data/brain_large.h5`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/brain_small_metadata.pickle` & `scvi_tools-1.0.1/tests/data/brain_small_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/brainlarge_dataset_test.h5ad` & `scvi_tools-1.0.1/tests/data/brainlarge_dataset_test.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/expression.bin` & `scvi_tools-1.0.1/tests/data/expression.bin`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/fc-dropseq.loom` & `scvi_tools-1.0.1/tests/data/fc-dropseq.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/immune_control_expression_matrix.txt` & `scvi_tools-1.0.1/tests/data/immune_control_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/immune_stimulated_expression_matrix.txt` & `scvi_tools-1.0.1/tests/data/immune_stimulated_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/mpfc-starmap.loom` & `scvi_tools-1.0.1/tests/data/mpfc-starmap.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/osmFISH_SScortex_mouse_all_cell.loom` & `scvi_tools-1.0.1/tests/data/osmFISH_SScortex_mouse_all_cell.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/pbmc_10k_protein_v3.h5ad` & `scvi_tools-1.0.1/tests/data/pbmc_10k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/pbmc_5k_protein_v3.h5ad` & `scvi_tools-1.0.1/tests/data/pbmc_5k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/random_metadata.pickle` & `scvi_tools-1.0.1/tests/data/random_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/retina.loom` & `scvi_tools-1.0.1/tests/data/retina.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/seqfishplus.zip` & `scvi_tools-1.0.1/tests/data/seqfishplus.zip`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/gene_info_pbmc.csv` & `scvi_tools-1.0.1/tests/data/10X/gene_info_pbmc.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/pbmc_metadata.pickle` & `scvi_tools-1.0.1/tests/data/10X/pbmc_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv` & `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx` & `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.1/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz` & `scvi_tools-1.0.1/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.spring_and_pba.csv` & `scvi_tools-1.0.1/tests/data/HEMATO/bBM.spring_and_pba.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz` & `scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz` & `scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv` & `scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx` & `scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/simulation/simulation_1.loom` & `scvi_tools-1.0.1/tests/data/simulation/simulation_1.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/simulation/simulation_2.loom` & `scvi_tools-1.0.1/tests/data/simulation/simulation_2.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/data/simulation/simulation_3.loom` & `scvi_tools-1.0.1/tests/data/simulation/simulation_3.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataloaders/test_datasplitter.py` & `scvi_tools-1.0.1/tests/dataloaders/test_datasplitter.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/conftest.py` & `scvi_tools-1.0.1/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/test_anndata.py` & `scvi_tools-1.0.1/tests/dataset/test_anndata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/test_built_in_data.py` & `scvi_tools-1.0.1/tests/dataset/test_built_in_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/test_dataset10X.py` & `scvi_tools-1.0.1/tests/dataset/test_dataset10X.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/test_mudata.py` & `scvi_tools-1.0.1/tests/dataset/test_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/test_preprocessing.py` & `scvi_tools-1.0.1/tests/dataset/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/dataset/utils.py` & `scvi_tools-1.0.1/tests/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_cellassign.py` & `scvi_tools-1.0.1/tests/external/test_cellassign.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_gimvi.py` & `scvi_tools-1.0.1/tests/external/test_gimvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_scar.py` & `scvi_tools-1.0.1/tests/external/test_scar.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_scbasset.py` & `scvi_tools-1.0.1/tests/external/test_scbasset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_stereoscope.py` & `scvi_tools-1.0.1/tests/external/test_stereoscope.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/external/test_tangram.py` & `scvi_tools-1.0.1/tests/external/test_tangram.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/hub/test_hub_metadata.py` & `scvi_tools-1.0.1/tests/hub/test_hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/hub/test_hub_model.py` & `scvi_tools-1.0.1/tests/hub/test_hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/models/test_lightning.py` & `scvi_tools-1.0.1/tests/models/test_lightning.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/models/test_models.py` & `scvi_tools-1.0.1/tests/models/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1108,14 +1108,32 @@
     m = SCVI(a, use_observed_lib_size=False)
     a2 = scvi.data.synthetic_iid()
     a2.obs["size_factor"] = np.random.randint(1, 5, size=(a2.shape[0],))
     scanvi_model = scvi.model.SCANVI.from_scvi_model(m, "label_0", adata=a2)
     scanvi_model.train(1)
 
 
+def test_linear_classifier_scanvi(n_latent: int = 10, n_labels: int = 5):
+    adata = synthetic_iid(n_labels=n_labels)
+    SCANVI.setup_anndata(
+        adata,
+        "labels",
+        "label_0",
+        batch_key="batch",
+    )
+    model = SCANVI(adata, linear_classifier=True, n_latent=n_latent)
+
+    assert len(model.module.classifier.classifier) == 2  # linear layer + softmax
+    assert isinstance(model.module.classifier.classifier[0], torch.nn.Linear)
+    assert model.module.classifier.classifier[0].in_features == n_latent
+    assert model.module.classifier.classifier[0].out_features == n_labels - 1
+
+    model.train(max_epochs=1)
+
+
 def test_linear_scvi(save_path):
     adata = synthetic_iid()
     adata = adata[:, :10].copy()
     LinearSCVI.setup_anndata(adata)
     model = LinearSCVI(adata, n_latent=10)
     model.train(1, check_val_every_n_epoch=1, train_size=0.5)
     assert len(model.history["elbo_train"]) == 1
```

### Comparing `scvi_tools-1.0.0b0/tests/models/test_models_with_minified_data.py` & `scvi_tools-1.0.1/tests/models/test_models_with_minified_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/models/test_mudata_models.py` & `scvi_tools-1.0.1/tests/models/test_mudata_models.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/models/test_pyro.py` & `scvi_tools-1.0.1/tests/models/test_pyro.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/models/test_scarches.py` & `scvi_tools-1.0.1/tests/models/test_scarches.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/tests/train/test_trainingplans.py` & `scvi_tools-1.0.1/tests/train/test_trainingplans.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/.gitignore` & `scvi_tools-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/LICENSE` & `scvi_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/README.md` & `scvi_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0b0/pyproject.toml` & `scvi_tools-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 
 [project]
 name = "scvi-tools"
-version = "1.0.0b0"
+version = "1.0.1"
 description = "Deep probabilistic analysis of single-cell omics data."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "The scvi-tools development team"},
 ]
@@ -21,43 +21,45 @@
 urls.Home-page = "https://scvi-tools.org"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Science/Research",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
     "anndata>=0.7.5",
-    "chex",
+    "chex<=0.1.8",
     "docrep>=0.3.2",
     "flax",
     "jax>=0.4.4",
     "jaxlib>=0.4.3",
     "optax",
-    "numpy>=1.17.0",
+    "numpy>=1.21.0",
     "pandas>=1.0",
     "scipy",
     "scikit-learn>=0.21.2",
     "rich>=12.0.0",
     "h5py>=2.9.0",
     "torch>=1.8.0",
     "lightning>=2.0,<2.1",
     "torchmetrics>=0.11.0",
     "pyro-ppl>=1.6.0",
     "tqdm>=4.56.0",
     "scikit-learn>=0.21.2",
-    "numpyro",
+    "numpyro>=0.12.1",
     "ml-collections>=0.1.1",
     "mudata>=0.1.2",
     "sparse>=0.14.0",
+    "xarray>=2023.2.0",
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "black",
     "pytest",
@@ -85,15 +87,15 @@
   "sphinxcontrib-bibtex>=1.0.0",
   "myst-parser",
   "myst-nb",
   "sphinx-autodoc-typehints",
 ]
 autotune = [
   "hyperopt>=0.2",
-  "ray[tune]>=2.2.0",
+  "ray[tune]>=2.5.0",
   "ipython",
   "scib-metrics>=0.3",
 ]
 pymde = ["pymde"]
 tutorials = ["scanpy", "leidenalg", "python-igraph", "loompy", "scikit-misc", "pynndescent", "pymde", "huggingface_hub", "genomepy"]
 hub = ["huggingface_hub"]
 regseq = [
```

### Comparing `scvi_tools-1.0.0b0/PKG-INFO` & `scvi_tools-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scvi-tools
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: Deep probabilistic analysis of single-cell omics data.
 Project-URL: Documentation, https://scvi-tools.org
 Project-URL: Source, https://github.com/scverse/scvi-tools
 Project-URL: Home-page, https://scvi-tools.org
 Author: The scvi-tools development team
 Maintainer-email: The scvi-tools development team <adamgayoso@berkeley.edu>
 License: BSD 3-Clause License
@@ -40,42 +40,44 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Requires-Dist: anndata>=0.7.5
-Requires-Dist: chex
+Requires-Dist: chex<=0.1.8
 Requires-Dist: docrep>=0.3.2
 Requires-Dist: flax
 Requires-Dist: h5py>=2.9.0
 Requires-Dist: jax>=0.4.4
 Requires-Dist: jaxlib>=0.4.3
 Requires-Dist: lightning<2.1,>=2.0
 Requires-Dist: ml-collections>=0.1.1
 Requires-Dist: mudata>=0.1.2
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: numpyro
+Requires-Dist: numpy>=1.21.0
+Requires-Dist: numpyro>=0.12.1
 Requires-Dist: optax
 Requires-Dist: pandas>=1.0
 Requires-Dist: pyro-ppl>=1.6.0
 Requires-Dist: rich>=12.0.0
 Requires-Dist: scikit-learn>=0.21.2
 Requires-Dist: scipy
 Requires-Dist: sparse>=0.14.0
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchmetrics>=0.11.0
 Requires-Dist: tqdm>=4.56.0
+Requires-Dist: xarray>=2023.2.0
 Provides-Extra: autotune
 Requires-Dist: hyperopt>=0.2; extra == 'autotune'
 Requires-Dist: ipython; extra == 'autotune'
-Requires-Dist: ray[tune]>=2.2.0; extra == 'autotune'
+Requires-Dist: ray[tune]>=2.5.0; extra == 'autotune'
 Requires-Dist: scib-metrics>=0.3; extra == 'autotune'
 Provides-Extra: census
 Requires-Dist: cellxgene-census; extra == 'census'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: cellxgene-census; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
```

