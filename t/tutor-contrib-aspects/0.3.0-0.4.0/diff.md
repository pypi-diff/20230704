# Comparing `tmp/tutor-contrib-aspects-0.3.0.tar.gz` & `tmp/tutor-contrib-aspects-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.3.0.tar", last modified: Fri Jun 30 16:51:53 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.4.0.tar", last modified: Tue Jul  4 13:19:48 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.3.0.tar` & `tutor-contrib-aspects-0.4.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:51:53.941579 tutor-contrib-aspects-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 16:51:53.000000 tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.925579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.933579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.929579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:53.937579 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 16:51:43.000000 tutor-contrib-aspects-0.3.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.723647 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.727648 tutor-contrib-aspects-0.4.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.731648 tutor-contrib-aspects-0.4.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.3.0/PKG-INFO` & `tutor-contrib-aspects-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.3.0
+Version: 0.4.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.3.0/README.rst` & `tutor-contrib-aspects-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/setup.py` & `tutor-contrib-aspects-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.3.0
+Version: 0.4.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.3.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 - _file_name: Open_edX_Admin_Dashboard_2.yaml
+  _roles:
+  - {{ SUPERSET_OPENEDX_ROLE_NAME }}
   css: ''
   dashboard_title: Open edX Admin Dashboard
   description: null
   metadata:
     chart_configuration: {}
     color_scheme: ''
     default_filters: '{}'
@@ -793,14 +795,16 @@
   sql: ''
   table_name: transcript_usage
   template_params: null
   uuid: bfbc2c72-4745-40ff-a7db-786711b90321
   version: 1.0.0
 
 - _file_name: Instructor_dashboard_4.yaml
+  _roles:
+  - {{ SUPERSET_OPENEDX_ROLE_NAME }}
   css: ''
   dashboard_title: Instructor dashboard
   description: null
   metadata:
     chart_configuration: {}
     color_scheme: ''
     default_filters: '{}'
@@ -1002,10 +1006,8 @@
     - null
     y_axis_format: SMART_NUMBER
   slice_name: Transcript/closed captioning usage per video
   uuid: 5593cd9b-81d4-4b9f-b4a7-cd377c92c5e6
   version: 1.0.0
   viz_type: dist_bar
 
-
-
 {{ patch("superset-extra-assets") }}
```

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files 6% similar despite different names*

```diff
@@ -64,26 +64,24 @@
 superset fab import-roles -p /app/security/roles.json
 echo_step "3" "Complete" "Setting up roles and perms"
 
 echo_step "4" "Starting" "Importing assets"
 
 cd /app/assets/
 rm -rf /app/assets/superset
-python /app/pythonpath/create_assets.py
 
-date=$(date -u +"%Y-%m-%dT%H:%M:%S.%6N+00:00") 
+mkdir /app/assets/superset -p
 
+date=$(date -u +"%Y-%m-%dT%H:%M:%S.%6N+00:00") 
 echo "version: 1.0.0
-type: Dashboard
+type: assets
 timestamp: '$date'" > superset/metadata.yaml
 
-zip -r superset.zip superset
+python /app/pythonpath/create_assets.py
 
-echo "\n\nImporting zip file\n\n"
-superset import-dashboards -p superset.zip
 
 rm -rf /app/assets/superset
 rm -rf /app/assets/superset.zip
 echo_step "4" "Complete" "Importing assets"
 
 # Set up a Row-Level Security filter to enforce course-based access restrictions.
 # Note: there are no cli commands or REST API endpoints to help us with this,
```

### Comparing `tutor-contrib-aspects-0.3.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.4.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

