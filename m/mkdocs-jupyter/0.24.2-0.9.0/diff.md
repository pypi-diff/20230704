# Comparing `tmp/mkdocs_jupyter-0.24.2.tar.gz` & `tmp/mkdocs-jupyter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dist/mkdocs-jupyter-0.9.0.tar", last modified: Wed Dec 18 02:23:16 2019, max compression
```

## Comparing `mkdocs_jupyter-0.24.2.tar` & `mkdocs-jupyter-0.9.0.tar`

### file list

```diff
@@ -1,123 +1,27 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/.prettierignore
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/.prettierrc
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/CHANGELOG.md
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/RELEASE.md
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/Taskfile.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/codecov.yml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements-dev.lock
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements.lock
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/setup.cfg
--rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/docs/download-button.png
--rw-r--r--   0        0        0    64122 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/docs/logo-square.png
--rw-r--r--   0        0        0    33066 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/docs/logo.png
--rw-r--r--   0        0        0   106373 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/docs/material-theme.png
--rw-r--r--   0        0        0   117706 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/docs/mkdocs-theme.png
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/.gitignore
--rw-r--r--   0        0        0   122658 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/package-lock.json
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/package.json
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/webpack.config.js
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/src/index.js
--rw-r--r--   0        0        0    13069 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/src/styles/index.scss
--rw-r--r--   0        0        0   556872 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/src/styles/jupyter-lab.scss
--rw-r--r--   0        0        0    29201 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/js/src/styles/theme.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/__about__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/config.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/convert.py
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/nbconvert2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/plugin.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/preprocessors.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/utils.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/conf.json
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/notebook.html.j2
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/assets/clipboard.umd.js
--rw-r--r--   0        0        0   544956 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/assets/mkdocs-jupyter.css
--rw-r--r--   0        0        0   687267 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/assets/mkdocs-jupyter.css.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_html/assets/mkdocs-jupyter.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_md/conf.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/templates/mkdocs_md/md-no-codecell.md.j2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/test_base_usage.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/test_pkg.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/base-with-nbs-failure.yml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/base-with-nbs-pys.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/base-with-nbs.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/base-with-pys.yml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/base-without-nbs.yml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/material-execute-ignore.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/material-with-nbs-pys.yml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/material-with-nbs.yml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/material-with-pys.yml
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/demo-script.py
--rw-r--r--   0        0        0  3714417 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/demo.ipynb
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/fail.ipynb
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/index.md
--rw-r--r--   0        0        0   488224 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/ruby.ipynb
--rw-r--r--   0        0        0    25658 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/variational-inference-script.py
--rw-r--r--   0        0        0   116450 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/variational-inference.ipynb
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/extras/README.md
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/extras/default.css
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/extras/material.css
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/extras/styles.css
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/extras/styles.py
--rw-r--r--   0        0        0    38960 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/docs/img/jupyter.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/overrides/main.html
--rw-r--r--   0        0        0     8722 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/404.html
--rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/index.html
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/sitemap.xml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/sitemap.xml.gz
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/images/favicon.png
--rw-r--r--   0        0        0   113155 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/bundle.fc8c2696.min.js
--rw-r--r--   0        0        0   950012 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/bundle.fc8c2696.min.js.map
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    38916 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0   113607 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/stylesheets/main.7bf56d0a.min.css
--rw-r--r--   0        0        0    39059 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/stylesheets/main.7bf56d0a.min.css.map
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
--rw-r--r--   0        0        0  4209433 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/demo/index.html
--rw-r--r--   0        0        0   652473 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/demo-script/index.html
--rw-r--r--   0        0        0   566185 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/fail/index.html
--rw-r--r--   0        0        0    38960 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/img/jupyter.png
--rw-r--r--   0        0        0  1030035 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/ruby/index.html
--rw-r--r--   0        0        0   673904 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/variational-inference/index.html
--rw-r--r--   0        0        0   688537 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/mkdocs_jupyter/tests/mkdocs/site/variational-inference-script/index.html
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements/all.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements/linting.in
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements/linting.txt
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/requirements/pyproject.txt
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/LICENSE.txt
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/README.md
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/pyproject.toml
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.2/PKG-INFO
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.977059 mkdocs-jupyter-0.9.0/
+-rw-r--r--   0 danielfrg   (501) staff       (20)    11346 2019-12-18 01:58:08.000000 mkdocs-jupyter-0.9.0/LICENSE.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)      153 2019-12-18 02:16:48.000000 mkdocs-jupyter-0.9.0/MANIFEST.in
+-rw-r--r--   0 danielfrg   (501) staff       (20)      816 2019-12-18 02:23:16.977221 mkdocs-jupyter-0.9.0/PKG-INFO
+-rw-r--r--   0 danielfrg   (501) staff       (20)      290 2019-12-18 02:21:51.000000 mkdocs-jupyter-0.9.0/README.md
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.978059 mkdocs-jupyter-0.9.0/mkdocs_jupyter/
+-rw-r--r--   0 danielfrg   (501) staff       (20)       93 2019-12-18 01:58:25.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/__init__.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)      497 2019-12-18 02:23:16.978141 mkdocs-jupyter-0.9.0/mkdocs_jupyter/_version.py
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.976797 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/
+-rw-r--r--   0 danielfrg   (501) staff       (20)     2150 2019-12-18 00:11:59.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/jupyter-fixes.css
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1169 2019-12-18 00:11:45.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/jupyter-fixes.min.css
+-rw-r--r--   0 danielfrg   (501) staff       (20)      232 2019-12-18 00:12:53.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/notebook.tpl
+-rw-r--r--   0 danielfrg   (501) staff       (20)     5990 2019-12-18 00:14:07.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/convert.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1249 2019-12-18 00:09:13.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/plugin.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1607 2019-12-18 00:33:20.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/templates.py
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.975762 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/
+-rw-r--r--   0 danielfrg   (501) staff       (20)      816 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 danielfrg   (501) staff       (20)      602 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)        1 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       64 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)        1 2019-12-18 02:04:07.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 danielfrg   (501) staff       (20)       25 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/requires.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       15 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       25 2019-12-18 01:50:35.000000 mkdocs-jupyter-0.9.0/requirements.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)      221 2019-12-18 02:23:16.977749 mkdocs-jupyter-0.9.0/setup.cfg
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1036 2019-12-18 02:05:34.000000 mkdocs-jupyter-0.9.0/setup.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)    68611 2019-12-18 01:58:25.000000 mkdocs-jupyter-0.9.0/versioneer.py
```

### Comparing `mkdocs_jupyter-0.24.2/LICENSE.txt` & `mkdocs-jupyter-0.9.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -183,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2019 Daniel Rodriguez
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

