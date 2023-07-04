# Comparing `tmp/pontos-23.7.0.tar.gz` & `tmp/pontos-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.7.0.tar", max compression
+gzip compressed data, was "pontos-23.7.1.tar", max compression
```

## Comparing `pontos-23.7.0.tar` & `pontos-23.7.1.tar`

### file list

```diff
@@ -1,254 +1,254 @@
--rw-r--r--   0        0        0    35149 2023-07-03 08:55:56.699958 pontos-23.7.0/LICENSE
--rw-r--r--   0        0        0     3836 2023-07-03 08:55:56.699958 pontos-23.7.0/README.md
--rw-r--r--   0        0        0   110395 2023-07-03 08:55:56.703958 pontos-23.7.0/poetry.lock
--rw-r--r--   0        0        0       32 2023-07-03 08:55:56.703958 pontos-23.7.0/poetry.toml
--rw-r--r--   0        0        0      791 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9995 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4396 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/errors.py
--rw-r--r--   0        0        0     5403 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/parser.py
--rw-r--r--   0        0        0        0 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/__init__.py
--rw-r--r--   0        0        0     1872 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/artifacts.py
--rw-r--r--   0        0        0     1605 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/create-repository.py
--rw-r--r--   0        0        0     2212 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/members.py
--rw-r--r--   0        0        0     2179 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/repositories.py
--rw-r--r--   0        0        0     6717 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/teams.py
--rw-r--r--   0        0        0     2789 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/workflow-runs.py
--rw-r--r--   0        0        0    14685 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4732 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/api.py
--rw-r--r--   0        0        0     2177 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     7339 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2646 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    11470 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/release.py
--rw-r--r--   0        0        0    12463 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12149 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1596 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2871 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7901 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3816 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6591 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_java.py
--rw-r--r--   0        0        0     6512 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8414 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/version.py
--rw-r--r--   0        0        0     2865 2023-07-03 08:55:56.711959 pontos-23.7.0/pyproject.toml
--rw-r--r--   0        0        0     1518 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17925 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3863 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15848 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    11614 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_java.py
--rw-r--r--   0        0        0    17081 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16677 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25664 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_version.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-03 14:47:01.863595 pontos-23.7.1/LICENSE
+-rw-r--r--   0        0        0     3836 2023-07-03 14:47:01.863595 pontos-23.7.1/README.md
+-rw-r--r--   0        0        0   110385 2023-07-03 14:47:01.867595 pontos-23.7.1/poetry.lock
+-rw-r--r--   0        0        0       32 2023-07-03 14:47:01.867595 pontos-23.7.1/poetry.toml
+-rw-r--r--   0        0        0      791 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4396 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-07-03 14:47:01.867595 pontos-23.7.1/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     5403 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/script/parser.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/__init__.py
+-rw-r--r--   0        0        0     1872 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/members.py
+-rw-r--r--   0        0        0     2179 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/repositories.py
+-rw-r--r--   0        0        0     6717 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/teams.py
+-rw-r--r--   0        0        0     2789 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/github/scripts/workflow-runs.py
+-rw-r--r--   0        0        0    14685 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4732 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2177 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     7339 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2646 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    11470 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/parser.py
+-rw-r--r--   0        0        0    14739 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/release.py
+-rw-r--r--   0        0        0    12463 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-07-03 14:47:01.871595 pontos-23.7.1/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12149 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1596 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2871 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7901 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3816 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6591 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6512 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8414 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13835 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16450 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5604 2023-07-03 14:47:01.875595 pontos-23.7.1/pontos/version/version.py
+-rw-r--r--   0        0        0     2993 2023-07-03 14:47:01.875595 pontos-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1518 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.875595 pontos-23.7.1/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3863 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.879596 pontos-23.7.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15848 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    11614 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    17081 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16677 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    26655 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    28629 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-07-03 14:47:01.883596 pontos-23.7.1/tests/version/test_version.py
+-rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 pontos-23.7.1/PKG-INFO
```

### Comparing `pontos-23.7.0/LICENSE` & `pontos-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/README.md` & `pontos-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/poetry.lock` & `pontos-23.7.1/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -408,21 +408,21 @@
 ]
 
 [package.extras]
 graph = ["objgraph (>=1.7.2)"]
 
 [[package]]
 name = "docutils"
-version = "0.19"
+version = "0.20.1"
 description = "Docutils -- Python Documentation Utilities"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "docutils-0.19-py3-none-any.whl", hash = "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"},
-    {file = "docutils-0.19.tar.gz", hash = "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6"},
+    {file = "docutils-0.20.1-py3-none-any.whl", hash = "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6"},
+    {file = "docutils-0.20.1.tar.gz", hash = "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"},
 ]
 
 [[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
 optional = false
@@ -565,30 +565,30 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.6.0"
+version = "6.7.0"
 description = "Read metadata from Python packages"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-6.6.0-py3-none-any.whl", hash = "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed"},
-    {file = "importlib_metadata-6.6.0.tar.gz", hash = "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"},
+    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
+    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
 ]
 
 [package.dependencies]
 zipp = ">=0.5"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 perf = ["ipython"]
-testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
 name = "isort"
 version = "5.12.0"
 description = "A Python utility / library to sort Python imports."
 optional = false
 python-versions = ">=3.8.0"
@@ -953,21 +953,21 @@
 files = [
     {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
     {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.5.3"
+version = "3.8.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.5.3-py3-none-any.whl", hash = "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed"},
-    {file = "platformdirs-3.5.3.tar.gz", hash = "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"},
+    {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
+    {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
@@ -1538,9 +1538,9 @@
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
-python-versions = "^3.9"
-content-hash = "d4878b00c9044f468f56232f9711780ccf479f6ca6f0e3f3749d07669fd97f48"
+python-versions = ">=3.9"
+content-hash = "932a855529a7013e65ff932897960282dfbcce758838c91916df27ff2c7b8806"
```

### Comparing `pontos-23.7.0/pontos/__init__.py` & `pontos-23.7.1/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/changelog/__init__.py` & `pontos-23.7.1/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/changelog/conventional_commits.py` & `pontos-23.7.1/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/changelog/errors.py` & `pontos-23.7.1/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/changelog/main.py` & `pontos-23.7.1/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/errors.py` & `pontos-23.7.1/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/git/__init__.py` & `pontos-23.7.1/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/git/git.py` & `pontos-23.7.1/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/git/status.py` & `pontos-23.7.1/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/__init__.py` & `pontos-23.7.1/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/__init__.py` & `pontos-23.7.1/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/argparser.py` & `pontos-23.7.1/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/cmds.py` & `pontos-23.7.1/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/core.py` & `pontos-23.7.1/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/env.py` & `pontos-23.7.1/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/errors.py` & `pontos-23.7.1/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/event.py` & `pontos-23.7.1/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/actions/main.py` & `pontos-23.7.1/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/__init__.py` & `pontos-23.7.1/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/api.py` & `pontos-23.7.1/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/artifacts.py` & `pontos-23.7.1/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/branch.py` & `pontos-23.7.1/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/client.py` & `pontos-23.7.1/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/contents.py` & `pontos-23.7.1/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/errors.py` & `pontos-23.7.1/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/helper.py` & `pontos-23.7.1/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/labels.py` & `pontos-23.7.1/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/organizations.py` & `pontos-23.7.1/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/pull_requests.py` & `pontos-23.7.1/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/release.py` & `pontos-23.7.1/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/repositories.py` & `pontos-23.7.1/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/search.py` & `pontos-23.7.1/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/tags.py` & `pontos-23.7.1/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/teams.py` & `pontos-23.7.1/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/api/workflows.py` & `pontos-23.7.1/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/argparser.py` & `pontos-23.7.1/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/cmds.py` & `pontos-23.7.1/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/main.py` & `pontos-23.7.1/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/__init__.py` & `pontos-23.7.1/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/artifact.py` & `pontos-23.7.1/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/base.py` & `pontos-23.7.1/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/branch.py` & `pontos-23.7.1/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/organization.py` & `pontos-23.7.1/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/pull_request.py` & `pontos-23.7.1/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/release.py` & `pontos-23.7.1/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/search.py` & `pontos-23.7.1/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/tag.py` & `pontos-23.7.1/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/models/workflow.py` & `pontos-23.7.1/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/pr_template.md` & `pontos-23.7.1/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/script/__init__.py` & `pontos-23.7.1/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/script/errors.py` & `pontos-23.7.1/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/script/load.py` & `pontos-23.7.1/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/script/parser.py` & `pontos-23.7.1/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/artifacts-download.py` & `pontos-23.7.1/pontos/github/scripts/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/artifacts.py` & `pontos-23.7.1/pontos/github/scripts/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/branchprotection.py` & `pontos-23.7.1/pontos/github/scripts/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/create-repository.py` & `pontos-23.7.1/pontos/github/scripts/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/enforce-admins.py` & `pontos-23.7.1/pontos/github/scripts/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/lock-branch.py` & `pontos-23.7.1/pontos/github/scripts/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/members.py` & `pontos-23.7.1/pontos/github/scripts/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/release-assets-download.py` & `pontos-23.7.1/pontos/github/scripts/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/repositories.py` & `pontos-23.7.1/pontos/github/scripts/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/search-repositories.py` & `pontos-23.7.1/pontos/github/scripts/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/team-repositories.py` & `pontos-23.7.1/pontos/github/scripts/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/teams.py` & `pontos-23.7.1/pontos/github/scripts/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/github/scripts/workflow-runs.py` & `pontos-23.7.1/pontos/github/scripts/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/helper.py` & `pontos-23.7.1/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/models/__init__.py` & `pontos-23.7.1/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/__init__.py` & `pontos-23.7.1/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/api.py` & `pontos-23.7.1/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/cpe/__init__.py` & `pontos-23.7.1/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/cpe/api.py` & `pontos-23.7.1/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/cve/__init__.py` & `pontos-23.7.1/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/cve/api.py` & `pontos-23.7.1/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/models/__init__.py` & `pontos-23.7.1/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/models/cpe.py` & `pontos-23.7.1/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/models/cve.py` & `pontos-23.7.1/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/models/cvss_v2.py` & `pontos-23.7.1/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/nvd/models/cvss_v3.py` & `pontos-23.7.1/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/pontos.py` & `pontos-23.7.1/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/release/__init__.py` & `pontos-23.7.1/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/release/helper.py` & `pontos-23.7.1/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/release/main.py` & `pontos-23.7.1/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/release/parser.py` & `pontos-23.7.1/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/release/release.py` & `pontos-23.7.1/pontos/release/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,24 @@
 from pontos.version.schemes import VersioningScheme
 
 from .helper import ReleaseType, find_signing_key, get_git_repository_name
 
 
 @dataclass
 class ReleaseInformation:
-    last_release_version: Version
+    last_release_version: Optional[Version]
     release_version: Version
     git_release_tag: str
     next_version: Version
 
     def write_github_output(self):
         with ActionIO.out() as output:
-            output.write("last-release-version", self.last_release_version)
+            output.write(
+                "last-release-version", self.last_release_version or ""
+            )
             output.write("release-version", self.release_version)
             output.write("git-release-tag", self.git_release_tag)
             output.write("next-version", self.next_version)
 
 
 class ReleaseReturnValue(IntEnum):
     """
@@ -121,25 +123,30 @@
         return release_version
 
     def _has_tag(self, git_version: str) -> bool:
         git_tags = self.git.list_tags()
         return git_version in git_tags
 
     def _create_changelog(
-        self, release_version: str, last_release_version: str, cc_config: Path
+        self,
+        release_version: Version,
+        last_release_version: Optional[Version],
+        cc_config: Path,
     ) -> str:
         changelog_builder = ChangelogBuilder(
             space=self.space,
             project=self.project,
             config=cc_config,
             git_tag_prefix=self.git_tag_prefix,
         )
 
         return changelog_builder.create_changelog(
-            last_version=last_release_version,
+            last_version=last_release_version.parsed_version
+            if last_release_version
+            else None,
             next_version=release_version,
         )
 
     async def _create_release(
         self, release_version: Version, token: str, release_text: str
     ) -> None:
         github = GitHubAsyncRESTApi(token=token)
@@ -222,18 +229,18 @@
                 parse_version=versioning_scheme.parse_version,
                 git_tag_prefix=self.git_tag_prefix,
                 tag_name=f"{self.git_tag_prefix}{release_series}.*"
                 if release_series
                 else None,
             )
         except PontosError as e:
-            self.terminal.error(
+            last_release_version = None
+            self.terminal.warning(
                 f"Could not determine last release version. {e}"
             )
-            return ReleaseReturnValue.NO_LAST_RELEASE_VERSION
 
         if not last_release_version:
             if not release_version:
                 self.terminal.error("Unable to determine last release version.")
                 return ReleaseReturnValue.NO_LAST_RELEASE_VERSION
             else:
                 self.terminal.info(
@@ -283,18 +290,23 @@
                     self.git.add(path)
             except VersionError as e:
                 self.terminal.error(
                     f"Unable to update version to {release_version}. {e}"
                 )
                 return ReleaseReturnValue.UPDATE_VERSION_ERROR
 
-        self.terminal.info(
-            f"Creating changelog for {release_version} since "
-            f"{last_release_version}"
-        )
+        if last_release_version:
+            self.terminal.info(
+                f"Creating changelog for {release_version} since "
+                f"{last_release_version}"
+            )
+        else:
+            self.terminal.info(
+                f"Creating changelog for {release_version} as initial release."
+            )
 
         release_text = self._create_changelog(
             release_version, last_release_version, cc_config
         )
 
         commit_msg = f"Automatic release to {release_version}"
```

### Comparing `pontos-23.7.0/pontos/release/sign.py` & `pontos-23.7.1/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/terminal/__init__.py` & `pontos-23.7.1/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/terminal/null.py` & `pontos-23.7.1/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/terminal/rich.py` & `pontos-23.7.1/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/terminal/terminal.py` & `pontos-23.7.1/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/testing/__init__.py` & `pontos-23.7.1/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/updateheader/__init__.py` & `pontos-23.7.1/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/updateheader/__main__.py` & `pontos-23.7.1/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/updateheader/updateheader.py` & `pontos-23.7.1/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/__init__.py` & `pontos-23.7.1/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/__main__.py` & `pontos-23.7.1/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/_calculator.py` & `pontos-23.7.1/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/__init__.py` & `pontos-23.7.1/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_cargo.py` & `pontos-23.7.1/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_cmake.py` & `pontos-23.7.1/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_command.py` & `pontos-23.7.1/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_go.py` & `pontos-23.7.1/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_java.py` & `pontos-23.7.1/pontos/version/commands/_java.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_javascript.py` & `pontos-23.7.1/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/commands/_python.py` & `pontos-23.7.1/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/errors.py` & `pontos-23.7.1/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/helper.py` & `pontos-23.7.1/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/main.py` & `pontos-23.7.1/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/parser.py` & `pontos-23.7.1/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/project.py` & `pontos-23.7.1/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/schemes/__init__.py` & `pontos-23.7.1/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/schemes/_pep440.py` & `pontos-23.7.1/pontos/version/schemes/_pep440.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 class PEP440Version(Version):
     """
     A class handling PEP 440 based version information
     """
 
     def __init__(self, version: str) -> None:
+        super().__init__(version)
         self._version = PackagingVersion(version)
         self._parse_local()
 
     def _parse_local(self):
         self._local = None
         if self._version.local:
             match = _LOCAL_RELEASE_REGEXP.match(self._version.local)
@@ -119,15 +120,15 @@
 
     @property
     def is_release_candidate(self) -> bool:
         """Whether this version is a release candidate."""
         return self.is_pre_release and self.pre and self.pre[0] == "rc"
 
     @classmethod
-    def from_string(cls, version: str) -> "Version":
+    def from_string(cls, version: str) -> "PEP440Version":
         """
         Create a version from a version string
 
         Args:
             version: Version string to parse
 
         Raises:
@@ -149,43 +150,53 @@
         This method can be used to convert version instances from different
         versioning schemes.
         """
 
         if isinstance(version, cls):
             return version
 
+        try:
+            # try to parse the original version string
+            return cls.from_string(version.parsed_version)
+        except VersionError:
+            pass
+
         version_local = (
             f"+{version.local[0]}{version.local[1]}" if version.local else ""
         )
         if version.is_dev_release:
             if not version.pre:
-                return cls.from_string(
+                new_version = cls.from_string(
                     f"{version.major}."
                     f"{version.minor}."
                     f"{version.patch}"
                     f".dev{version.dev}"
                     f"{version_local}"
                 )
-            return cls.from_string(
-                f"{version.major}."
-                f"{version.minor}."
-                f"{version.patch}"
-                f"-{version.pre[0]}{version.pre[1]}"
-                f".dev{version.dev}"
-            )
-        if version.is_pre_release:
-            return cls.from_string(
+            else:
+                new_version = cls.from_string(
+                    f"{version.major}."
+                    f"{version.minor}."
+                    f"{version.patch}"
+                    f"-{version.pre[0]}{version.pre[1]}"
+                    f".dev{version.dev}"
+                )
+        elif version.is_pre_release:
+            new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-{version.pre[0]}{version.pre[1]}"
                 f"{version_local}"
             )
+        else:
+            new_version = cls.from_string(str(version))
 
-        return cls.from_string(str(version))
+        new_version._parsed_version = version.parsed_version
+        return new_version
 
     def __eq__(self, other: Any) -> bool:
         if other is None:
             return False
         if isinstance(other, str):
             # allow to compare against "current" for now
             return False
```

### Comparing `pontos-23.7.0/pontos/version/schemes/_scheme.py` & `pontos-23.7.1/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/pontos/version/schemes/_semantic.py` & `pontos-23.7.1/pontos/version/schemes/_semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     `Semantic Versioning<https://semver.org/>`_
     """
 
     def __init__(
         self,
         version: str,
     ) -> None:
+        super().__init__(version)
         self._version_info = VersionInfo.parse(version)
         self._parse_build()
         self._parse_pre_release()
 
     def _parse_pre_release(self) -> None:
         self._dev = None
         self._pre_release = None
@@ -253,60 +254,69 @@
         This method can be used to convert version instances from different
         versioning schemes.
         """
 
         if isinstance(version, cls):
             return version
 
+        try:
+            # try to parse the original version string
+            return cls.from_string(version.parsed_version)
+        except VersionError:
+            pass
+
         version_local = (
             f"+{version.local[0]}{version.local[1]}" if version.local else ""
         )
         if version.is_dev_release:
             if not version.pre:
-                return cls.from_string(
+                new_version = cls.from_string(
                     f"{version.major}."
                     f"{version.minor}."
                     f"{version.patch}"
                     f"-dev{version.dev}"
                     f"{version_local}"
                 )
-
-            return cls.from_string(
-                f"{version.major}."
-                f"{version.minor}."
-                f"{version.patch}"
-                f"-{version.pre[0]}{version.pre[1]}"
-                f"-dev{version.dev}"
-            )
-        if version.is_alpha_release:
-            return cls.from_string(
+            else:
+                new_version = cls.from_string(
+                    f"{version.major}."
+                    f"{version.minor}."
+                    f"{version.patch}"
+                    f"-{version.pre[0]}{version.pre[1]}"
+                    f"-dev{version.dev}"
+                )
+        elif version.is_alpha_release:
+            new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-alpha{version.pre[1]}"
                 f"{version_local}"
             )
-        if version.is_beta_release:
-            return cls.from_string(
+        elif version.is_beta_release:
+            new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-beta{version.pre[1]}"
                 f"{version_local}"
             )
-        if version.is_pre_release:
-            return cls.from_string(
+        elif version.is_pre_release:
+            new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-{version.pre[0]}{version.pre[1]}"
                 f"{version_local}"
             )
+        else:
+            new_version = cls.from_string(str(version))
 
-        return cls.from_string(str(version))
+        new_version._parsed_version = version.parsed_version
+        return new_version
 
 
 # pylint: disable=protected-access
 class SemanticVersionCalculator(VersionCalculator):
     version_cls = SemanticVersion
 
     @classmethod
```

### Comparing `pontos-23.7.0/pontos/version/version.py` & `pontos-23.7.1/pontos/version/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,24 @@
       containing a pre release version like `1.2.3-alpha1-dev1`
     * A development version has no local part
     * Alpha, Beta, Release Candidate and Development versions are pre releases
     * Alpha, Beta and Release Candidate versions pre must return the following
       names for the first value in the tuple: `alpha`, `beta`, `rc` and `dev`
     """
 
+    def __init__(self, original_version: str) -> None:
+        self._parsed_version = original_version
+
+    @property
+    def parsed_version(self) -> str:
+        """
+        Original version string from which the version has been parsed
+        """
+        return self._parsed_version
+
     @property
     @abstractmethod
     def major(self) -> int:
         """The first item of the version or ``0`` if unavailable."""
 
     @property
     @abstractmethod
```

### Comparing `pontos-23.7.0/pyproject.toml` & `pontos-23.7.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.7.0"
+version = "23.7.1"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -30,36 +30,36 @@
 ]
 include = [
   "pontos/updateheader/templates/",
   "pontos/github/pr_template.md"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-colorful = "^0.5.4"
+python = ">=3.9"
+colorful = ">=0.5.4"
 tomlkit = ">=0.5.11"
 packaging = ">=20.3"
 httpx = {extras = ["http2"], version = ">=0.23,<0.25"}
 rich = ">=12.4.4"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
-python-dateutil = "^2.8.2"
-semver = ">=2.13,<4.0"
-lxml = "^4.9.0"
+python-dateutil = ">=2.8.2"
+semver = ">=2.13"
+lxml = ">=4.9.0"
 
 [tool.poetry.dev-dependencies]
-autohooks = ">=22.7.0"
-autohooks-plugin-pylint = ">=21.6.0"
-autohooks-plugin-black = ">=22.7.0"
-autohooks-plugin-isort = ">=22.3.0"
-rope = "^1.9.0"
-coverage = "^7.2"
+autohooks = { version = ">=22.7.0", python = "^3.9" }
+autohooks-plugin-pylint = { version = ">=21.6.0", python = "^3.9" }
+autohooks-plugin-black = { version = ">=22.7.0", python = "^3.9" }
+autohooks-plugin-isort = { version = ">=22.3.0", python = "^3.9" }
+rope = ">=1.9.0"
+coverage = ">=7.2"
 myst-parser = ">=0.19.1"
-Sphinx = "^7.0.1"
-furo = "^2023.5.20"
-sphinx-autobuild = "^2021.3.14"
+Sphinx = ">=7.0.1"
+furo = ">=2023.5.20"
+sphinx-autobuild = ">=2021.3.14"
 
 [tool.black]
 line-length = 80
 target-version = ['py39', 'py310', 'py311']
 exclude = '''
 /(
     \.git
```

### Comparing `pontos-23.7.0/tests/__init__.py` & `pontos-23.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/changelog/__init__.py` & `pontos-23.7.1/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/changelog/test_conventional_commits.py` & `pontos-23.7.1/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/changelog/test_parser.py` & `pontos-23.7.1/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/git/__init__.py` & `pontos-23.7.1/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/git/test_git.py` & `pontos-23.7.1/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/git/test_status.py` & `pontos-23.7.1/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/__init__.py` & `pontos-23.7.1/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/actions/__init__.py` & `pontos-23.7.1/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/actions/test-pull-request-event.json` & `pontos-23.7.1/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/actions/test_core.py` & `pontos-23.7.1/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/actions/test_env.py` & `pontos-23.7.1/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/actions/test_event.py` & `pontos-23.7.1/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/__init__.py` & `pontos-23.7.1/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/pr-files.json` & `pontos-23.7.1/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/release-response.json` & `pontos-23.7.1/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_artifacts.py` & `pontos-23.7.1/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_branch.py` & `pontos-23.7.1/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_client.py` & `pontos-23.7.1/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_contents.py` & `pontos-23.7.1/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_labels.py` & `pontos-23.7.1/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_organizations.py` & `pontos-23.7.1/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_pull_requests.py` & `pontos-23.7.1/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_release.py` & `pontos-23.7.1/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_repositories.py` & `pontos-23.7.1/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_search.py` & `pontos-23.7.1/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_tags.py` & `pontos-23.7.1/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_teams.py` & `pontos-23.7.1/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/api/test_workflows.py` & `pontos-23.7.1/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/__init__.py` & `pontos-23.7.1/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_artifact.py` & `pontos-23.7.1/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_base.py` & `pontos-23.7.1/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_branch.py` & `pontos-23.7.1/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_organization.py` & `pontos-23.7.1/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_pull_request.py` & `pontos-23.7.1/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_release.py` & `pontos-23.7.1/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_search.py` & `pontos-23.7.1/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_tag.py` & `pontos-23.7.1/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/models/test_workflow.py` & `pontos-23.7.1/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/script/__init__.py` & `pontos-23.7.1/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/script/test_load.py` & `pontos-23.7.1/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/script/test_parser.py` & `pontos-23.7.1/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/test_argparser.py` & `pontos-23.7.1/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/github/test_cmds.py` & `pontos-23.7.1/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/models/__init__.py` & `pontos-23.7.1/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/models/test_models.py` & `pontos-23.7.1/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/__init__.py` & `pontos-23.7.1/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/cpe/__init__.py` & `pontos-23.7.1/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/cpe/test_api.py` & `pontos-23.7.1/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/cve/__init__.py` & `pontos-23.7.1/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/cve/test_api.py` & `pontos-23.7.1/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/models/__init__.py` & `pontos-23.7.1/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/models/test_cpe.py` & `pontos-23.7.1/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/models/test_cve.py` & `pontos-23.7.1/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/nvd/test_api.py` & `pontos-23.7.1/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/release/__init__.py` & `pontos-23.7.1/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/release/test_helper.py` & `pontos-23.7.1/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/release/test_parser.py` & `pontos-23.7.1/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/release/test_release.py` & `pontos-23.7.1/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/release/test_sign.py` & `pontos-23.7.1/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/terminal/__init__.py` & `pontos-23.7.1/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/terminal/test_terminal.py` & `pontos-23.7.1/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/test_helper.py` & `pontos-23.7.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/test_pontos.py` & `pontos-23.7.1/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/testing/__init__.py` & `pontos-23.7.1/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/testing/test_testing.py` & `pontos-23.7.1/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/updateheader/__init__.py` & `pontos-23.7.1/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/updateheader/test_header.py` & `pontos-23.7.1/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/__init__.py` & `pontos-23.7.1/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/__init__.py` & `pontos-23.7.1/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_cargo.py` & `pontos-23.7.1/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_cmake.py` & `pontos-23.7.1/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_go.py` & `pontos-23.7.1/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_java.py` & `pontos-23.7.1/tests/version/commands/test_java.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_javascript.py` & `pontos-23.7.1/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/commands/test_python.py` & `pontos-23.7.1/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/schemes/__init__.py` & `pontos-23.7.1/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/schemes/test_pep440.py` & `pontos-23.7.1/tests/version/schemes/test_pep440.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,48 @@
             "1.4.1",
             "2.4.1-dev1",
             "2.4.1-dev3",
         ]
         for version in versions:
             self.assertEqual(Version.from_string(version), Version(version))
 
+    def test_parsed_version(self):
+        versions = [
+            "0.0.1",
+            "1.2.3",
+            "1.2.3-post1.dev1",
+            "1.2.3-a1",
+            "1.2.3-b1",
+            "1.2.3-rc1",
+            "1.2.3-a1+dev1",
+            "1.2.3-a1-dev1",
+            "1.4.1",
+            "2.4.1-dev1",
+            "2.4.1-dev3",
+            "1.2.3.post1",
+            "1.2.3a1",
+            "1.2.3b1",
+            "1.2.3rc1",
+            "1.2.3a1+dev1",
+            "1.2.3a1.dev1",
+            "22.4.1.dev1",
+            "22.4.1.dev3",
+            "2022.4.1.dev3",
+        ]
+        for version in versions:
+            self.assertEqual(
+                Version.from_string(version).parsed_version, version
+            )
+
+        semver_version = SemanticVersion.from_string("22.4.1-dev1")
+        pep440_version = Version.from_version(semver_version)
+
+        self.assertEqual(str(pep440_version), "22.4.1.dev1")
+        self.assertEqual(pep440_version.parsed_version, "22.4.1-dev1")
+
     def test_parse_error(self):
         versions = [
             "abc",
             "1.2.3d",
         ]
 
         for version in versions:
```

### Comparing `pontos-23.7.0/tests/version/schemes/test_semantic.py` & `pontos-23.7.1/tests/version/schemes/test_semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,44 @@
             "22.4.1",
             "22.4.1-dev1",
             "22.4.1-dev3",
         ]
         for version in versions:
             self.assertEqual(Version.from_string(version), Version(version))
 
+    def test_parsed_version(self):
+        versions = [
+            "0.0.1",
+            "1.2.3",
+            "1.2.3-foo1",
+            "1.2.3-a1",
+            "1.2.3-alpha1",
+            "1.2.3-alpha1-dev1",
+            "1.2.3-b1",
+            "1.2.3-beta1",
+            "1.2.3-beta1-dev1",
+            "1.2.3-rc1",
+            "1.2.3-rc1-dev1",
+            "1.2.3-dev1",
+            "1.2.3+foo1",
+            "22.4.1",
+            "22.4.1-dev1",
+            "22.4.1-dev3",
+        ]
+        for version in versions:
+            self.assertEqual(
+                Version.from_string(version).parsed_version, version
+            )
+
+        pep440_version = PEP440Version.from_string("22.4.1.dev1")
+        semver_version = Version.from_version(pep440_version)
+
+        self.assertEqual(str(semver_version), "22.4.1-dev1")
+        self.assertEqual(semver_version.parsed_version, "22.4.1.dev1")
+
     def test_parse_error(self):
         versions = [
             "abc",
             "1.2.3d",
             "1.2.3.post1",
             "1.2.3a1",
             "1.2.3b1",
```

### Comparing `pontos-23.7.0/tests/version/test_commands.py` & `pontos-23.7.1/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_errors.py` & `pontos-23.7.1/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_helper.py` & `pontos-23.7.1/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_main.py` & `pontos-23.7.1/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_parser.py` & `pontos-23.7.1/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_project.py` & `pontos-23.7.1/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/tests/version/test_version.py` & `pontos-23.7.1/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.0/PKG-INFO` & `pontos-23.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.7.0
+Version: 23.7.1
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: colorful (>=0.5.4,<0.6.0)
+Requires-Dist: colorful (>=0.5.4)
 Requires-Dist: httpx[http2] (>=0.23,<0.25)
-Requires-Dist: lxml (>=4.9.0,<5.0.0)
+Requires-Dist: lxml (>=4.9.0)
 Requires-Dist: packaging (>=20.3)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: rich (>=12.4.4)
-Requires-Dist: semver (>=2.13,<4.0)
+Requires-Dist: semver (>=2.13)
 Requires-Dist: tomlkit (>=0.5.11)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Documentation, https://greenbone.github.io/pontos/
 Project-URL: Repository, https://github.com/greenbone/pontos/
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
```

