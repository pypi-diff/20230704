# Comparing `tmp/tungstenkit-0.1.0.tar.gz` & `tmp/tungstenkit-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.0.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.1a1.tar", max compression
```

## Comparing `tungstenkit-0.1.0.tar` & `tungstenkit-0.1.1a1.tar`

### file list

```diff
@@ -1,172 +1,175 @@
--rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.0/LICENSE
--rw-r--r--   0        0        0     7704 2023-06-08 13:32:45.296808 tungstenkit-0.1.0/README.md
--rw-r--r--   0        0        0     2868 2023-06-07 05:33:58.888669 tungstenkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.0/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.0/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.0/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.0/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0     9630 2023-06-07 05:35:48.388092 tungstenkit-0.1.0/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5378 2023-06-07 06:19:25.945256 tungstenkit-0.1.0/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.0/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    15272 2023-06-07 06:31:05.193620 tungstenkit-0.1.0/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     6597 2023-06-07 06:20:37.816697 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      644 2023-05-29 05:33:04.832002 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1153 2023-06-07 06:16:43.922538 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      230 2023-05-29 05:55:41.909098 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      397 2023-05-29 05:59:32.635863 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      438 2023-06-07 06:17:19.642252 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1253 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     3867 2023-05-12 11:40:17.613744 tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1593 2023-05-11 12:11:50.917409 tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4421 2023-05-11 12:12:32.285256 tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6598 2023-05-11 12:12:32.245256 tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4624 2023-06-01 08:29:23.281737 tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
--rw-r--r--   0        0        0     3573 2023-06-07 06:31:35.793599 tungstenkit-0.1.0/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      723 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     7784 2023-06-01 06:03:05.538290 tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      924 2023-05-05 07:02:23.660425 tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.0/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.0/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-09 00:51:06.380603 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0    78390 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
--rw-r--r--   0        0        0  1555099 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/934-e0819d120eb89b62.js
--rw-r--r--   0        0        0   452205 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
--rw-r--r--   0        0        0   141074 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
--rw-r--r--   0        0        0    90428 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
--rw-r--r--   0        0        0   142832 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-055212ca45717427.js
--rw-r--r--   0        0        0      250 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
--rw-r--r--   0        0        0    26797 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-22c1b33e4104cf9a.js
--rw-r--r--   0        0        0    91460 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-3c54a28f0adb43ad.js
--rw-r--r--   0        0        0     1914 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/css/6c93262152699231.css
--rw-r--r--   0        0        0    39283 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
--rw-r--r--   0        0        0      401 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/qTYF6hz8zCCC7Oy_19hX7/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-06-09 00:51:05.592607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/qTYF6hz8zCCC7Oy_19hX7/_ssgManifest.js
--rw-r--r--   0        0        0   256670 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0    26724 2023-06-09 00:51:06.344603 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0     2956 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0     1375 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/next.svg
--rw-r--r--   0        0        0     1138 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/thirteen.svg
--rw-r--r--   0        0        0    27505 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0      629 2023-06-09 00:51:05.600607 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/vercel.svg
--rw-r--r--   0        0        0     2587 2023-06-05 05:24:44.708624 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5173 2023-06-05 05:24:44.712623 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12095 2023-06-05 05:24:44.712623 tungstenkit-0.1.0/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11331 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     7252 2023-06-02 08:07:56.573968 tungstenkit-0.1.0/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    11261 2023-06-07 06:14:27.599650 tungstenkit-0.1.0/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.0/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.0/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.0/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.0/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.0/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5084 2023-06-02 08:30:41.454068 tungstenkit-0.1.0/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.0/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.0/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.0/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10199 2023-06-02 12:48:10.308932 tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.0/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      606 2023-06-01 15:06:58.874575 tungstenkit-0.1.0/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.0/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.0/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.0/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.0/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.0/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.0/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.0/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    14054 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0     9837 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      509 2023-06-05 12:56:44.197918 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     1941 2023-06-05 12:03:00.167498 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.0/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.0/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.0/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     6213 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.0/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.0/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.0/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.0/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      967 2023-05-25 12:26:56.640679 tungstenkit-0.1.0/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.0/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6335 2023-05-25 09:44:14.934739 tungstenkit-0.1.0/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.0/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2379 2023-06-02 12:43:00.699193 tungstenkit-0.1.0/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.0/tungstenkit/models.py
--rw-r--r--   0        0        0    10827 1970-01-01 00:00:00.000000 tungstenkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.1a1/README.md
+-rw-r--r--   0        0        0     2870 2023-07-04 14:03:50.429114 tungstenkit-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.1a1/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.1a1/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0     9630 2023-06-07 05:35:48.388092 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5378 2023-06-07 06:19:25.945256 tungstenkit-0.1.1a1/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.1a1/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    15272 2023-06-07 06:31:05.193620 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     6597 2023-06-07 06:20:37.816697 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      644 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1153 2023-06-07 06:16:43.922538 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      230 2023-05-29 05:55:41.909098 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      397 2023-05-29 05:59:32.635863 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      438 2023-06-07 06:17:19.642252 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1253 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     3867 2023-05-12 11:40:17.613744 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1593 2023-05-11 12:11:50.917409 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4421 2023-05-11 12:12:32.285256 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6598 2023-05-11 12:12:32.245256 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4624 2023-06-01 08:29:23.281737 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
+-rw-r--r--   0        0        0     3573 2023-06-07 06:31:35.793599 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     7784 2023-06-01 06:03:05.538290 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      924 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.1a1/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.1a1/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-14 05:40:17.862200 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0      401 2023-06-14 05:40:17.862200 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/S40LwJxEK4Dfl_G1r0OjF/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-06-14 05:40:17.862200 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/S40LwJxEK4Dfl_G1r0OjF/_ssgManifest.js
+-rw-r--r--   0        0        0    78390 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
+-rw-r--r--   0        0        0  1555099 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/934-e0819d120eb89b62.js
+-rw-r--r--   0        0        0   452205 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
+-rw-r--r--   0        0        0   141074 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
+-rw-r--r--   0        0        0    90428 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
+-rw-r--r--   0        0        0   142832 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-055212ca45717427.js
+-rw-r--r--   0        0        0      250 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
+-rw-r--r--   0        0        0    26797 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-22c1b33e4104cf9a.js
+-rw-r--r--   0        0        0    26780 2023-06-14 05:40:17.862200 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-ec668a0a6e43b7f3.js
+-rw-r--r--   0        0        0    91460 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3853 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-3c54a28f0adb43ad.js
+-rw-r--r--   0        0        0     1914 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/css/6c93262152699231.css
+-rw-r--r--   0        0        0    39283 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
+-rw-r--r--   0        0        0      401 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/qTYF6hz8zCCC7Oy_19hX7/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-06-09 00:51:05.592607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/qTYF6hz8zCCC7Oy_19hX7/_ssgManifest.js
+-rw-r--r--   0        0        0   256670 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0    26724 2023-06-14 05:40:17.862200 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0     2956 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0     1375 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/next.svg
+-rw-r--r--   0        0        0     1138 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/thirteen.svg
+-rw-r--r--   0        0        0    27505 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0      629 2023-06-09 00:51:05.600607 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/vercel.svg
+-rw-r--r--   0        0        0     2587 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5173 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12095 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-04 14:01:36.561839 tungstenkit-0.1.1a1/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     7252 2023-06-02 08:07:56.573968 tungstenkit-0.1.1a1/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    11261 2023-06-07 06:14:27.599650 tungstenkit-0.1.1a1/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.1a1/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5084 2023-06-02 08:30:41.454068 tungstenkit-0.1.1a1/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      606 2023-06-01 15:06:58.874575 tungstenkit-0.1.1a1/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.1a1/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.1a1/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    14054 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0     9841 2023-07-04 14:01:36.561839 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      509 2023-06-05 12:56:44.197918 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2054 2023-06-26 07:20:09.814702 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     6213 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      967 2023-05-25 12:26:56.640679 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6335 2023-05-25 09:44:14.934739 tungstenkit-0.1.1a1/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a1/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2379 2023-06-02 12:43:00.699193 tungstenkit-0.1.1a1/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.1a1/tungstenkit/models.py
+-rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 tungstenkit-0.1.1a1/PKG-INFO
```

### Comparing `tungstenkit-0.1.0/LICENSE` & `tungstenkit-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/README.md` & `tungstenkit-0.1.1a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tungstenkit: ML container made simple
 [![Version](https://img.shields.io/pypi/v/tungstenkit?color=%2334D058&label=pypi%20package)](https://pypi.org/project/tungstenkit/)
 [![License](https://img.shields.io/github/license/tungsten-ai/tungstenkit)](https://raw.githubusercontent.com/tungsten-ai/tungstenkit/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/tungstenkit?style=flat-square)](https://pypi.org/project/tungstenkit/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/tungstenkit.svg?color=%2334D058)](https://pypi.org/project/tungstenkit/)
 
-[Features](#features) | [Installation](#prerequisites) | [Getting Started](https://tungsten-ai.github.io/docs/getting_started) | [Documentation](https://tungsten-ai.github.io/docs) 
+[Introduction](#tungstenkit-ml-container-made-simple) | [Installation](#prerequisites) | [Getting Started](https://tungsten-ai.github.io/docs/getting_started) | [Documentation](https://tungsten-ai.github.io/docs) 
 
 Tungstenkit is ML containerization tool with a focus on developer productivity and versatility.
 
 The key features are:
 
 - [Requires only a few lines of Python code](#requires-only-a-few-lines-of-python-code)
 - [Build once, use everywhere](#build-once-use-everywhere):
```

### Comparing `tungstenkit-0.1.0/pyproject.toml` & `tungstenkit-0.1.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.0"
+version = "0.1.1a1"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/build_context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/template_args.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/css/6c93262152699231.css" as="style"/><link rel="stylesheet" href="/_next/static/css/6c93262152699231.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-3c54a28f0adb43ad.js" defer=""></script><script src="/_next/static/chunks/framework-73b8966a3c579ab0.js" defer=""></script><script src="/_next/static/chunks/main-6260d066cf2cd7b1.js" defer=""></script><script src="/_next/static/chunks/pages/_app-055212ca45717427.js" defer=""></script><script src="/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js" defer=""></script><script src="/_next/static/qTYF6hz8zCCC7Oy_19hX7/_buildManifest.js" defer=""></script><script src="/_next/static/qTYF6hz8zCCC7Oy_19hX7/_ssgManifest.js" defer=""></script></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1kvm0ug">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:1rem;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"qTYF6hz8zCCC7Oy_19hX7","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/css/6c93262152699231.css" as="style"/><link rel="stylesheet" href="/_next/static/css/6c93262152699231.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-3c54a28f0adb43ad.js" defer=""></script><script src="/_next/static/chunks/framework-73b8966a3c579ab0.js" defer=""></script><script src="/_next/static/chunks/main-6260d066cf2cd7b1.js" defer=""></script><script src="/_next/static/chunks/pages/_app-055212ca45717427.js" defer=""></script><script src="/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js" defer=""></script><script src="/_next/static/S40LwJxEK4Dfl_G1r0OjF/_buildManifest.js" defer=""></script><script src="/_next/static/S40LwJxEK4Dfl_G1r0OjF/_ssgManifest.js" defer=""></script></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1kvm0ug">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:1rem;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"S40LwJxEK4Dfl_G1r0OjF","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/934-e0819d120eb89b62.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/934-e0819d120eb89b62.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-055212ca45717427.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-055212ca45717427.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-22c1b33e4104cf9a.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-22c1b33e4104cf9a.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-3c54a28f0adb43ad.js` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-3c54a28f0adb43ad.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/css/6c93262152699231.css` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/css/6c93262152699231.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/6c93262152699231.css" as="style"/><link rel="stylesheet" href="/_next/static/css/6c93262152699231.css" data-n-g=""/><link rel="preload" href="/_next/static/css/e19e5222d7a223c1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e19e5222d7a223c1.css" data-n-p=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-3c54a28f0adb43ad.js" defer=""></script><script src="/_next/static/chunks/framework-73b8966a3c579ab0.js" defer=""></script><script src="/_next/static/chunks/main-6260d066cf2cd7b1.js" defer=""></script><script src="/_next/static/chunks/pages/_app-055212ca45717427.js" defer=""></script><script src="/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js" defer=""></script><script src="/_next/static/chunks/934-e0819d120eb89b62.js" defer=""></script><script src="/_next/static/chunks/pages/index-22c1b33e4104cf9a.js" defer=""></script><script src="/_next/static/qTYF6hz8zCCC7Oy_19hX7/_buildManifest.js" defer=""></script><script src="/_next/static/qTYF6hz8zCCC7Oy_19hX7/_ssgManifest.js" defer=""></script></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1kvm0ug">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:1rem;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css 1t3x66l">.css-1t3x66l{background-color:white;min-height:100vh;}</style><div class="MuiBox-root css-1t3x66l" id="main header"><style data-emotion="css ylfuw0">.css-ylfuw0{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:white;border:1px solid #E1E2E6;min-width:900px;}</style><div class="MuiBox-root css-ylfuw0"><style data-emotion="css jsa4zg">.css-jsa4zg{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;margin-left:4%;margin-right:4%;min-width:800px;}</style><div class="MuiBox-root css-jsa4zg"><div class="MuiBox-root css-0" style="width:100%;margin-top:2%;display:inline"><style data-emotion="css k008qs">.css-k008qs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;}</style><div class="MuiBox-root css-k008qs"><div class="mantine-Avatar-root mantine-qnn0x"><div class="mantine-1tfrire mantine-Avatar-placeholder"><svg class="mantine-13sjtfj mantine-Avatar-placeholderIcon" width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.877014 7.49988C0.877014 3.84219 3.84216 0.877045 7.49985 0.877045C11.1575 0.877045 14.1227 3.84219 14.1227 7.49988C14.1227 11.1575 11.1575 14.1227 7.49985 14.1227C3.84216 14.1227 0.877014 11.1575 0.877014 7.49988ZM7.49985 1.82704C4.36683 1.82704 1.82701 4.36686 1.82701 7.49988C1.82701 8.97196 2.38774 10.3131 3.30727 11.3213C4.19074 9.94119 5.73818 9.02499 7.50023 9.02499C9.26206 9.02499 10.8093 9.94097 11.6929 11.3208C12.6121 10.3127 13.1727 8.97172 13.1727 7.49988C13.1727 4.36686 10.6328 1.82704 7.49985 1.82704ZM10.9818 11.9787C10.2839 10.7795 8.9857 9.97499 7.50023 9.97499C6.01458 9.97499 4.71624 10.7797 4.01845 11.9791C4.97952 12.7272 6.18765 13.1727 7.49985 13.1727C8.81227 13.1727 10.0206 12.727 10.9818 11.9787ZM5.14999 6.50487C5.14999 5.207 6.20212 4.15487 7.49999 4.15487C8.79786 4.15487 9.84999 5.207 9.84999 6.50487C9.84999 7.80274 8.79786 8.85487 7.49999 8.85487C6.20212 8.85487 5.14999 7.80274 5.14999 6.50487ZM7.49999 5.10487C6.72679 5.10487 6.09999 5.73167 6.09999 6.50487C6.09999 7.27807 6.72679 7.90487 7.49999 7.90487C8.27319 7.90487 8.89999 7.27807 8.89999 6.50487C8.89999 5.73167 8.27319 5.10487 7.49999 5.10487Z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg></div></div><div class="MuiBox-root css-0" style="margin-left:20px;height:75px;display:inline"><div class="MuiBox-root css-0" style="height:fit-content;width:100%;position:relative;float:left"><style data-emotion="css 1su0e22">.css-1su0e22{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5rem;line-height:1.334;letter-spacing:0em;float:left;}</style><h5 class="MuiTypography-root MuiTypography-h5 css-1su0e22"></h5></div><div class="MuiBox-root css-0" style="width:100%;height:fit-content;float:left;margin-top:0px"><style data-emotion="css 1ww87vj">.css-1ww87vj{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;color:#677285;float:left;font-size:18px;}</style><p class="MuiTypography-root MuiTypography-body1 css-1ww87vj"></p></div></div></div><style data-emotion="css 1ejdhgq">.css-1ejdhgq{width:40%;margin-top:15px;}</style><div class="MuiBox-root css-1ejdhgq"><div><style data-emotion="css 5gn4a3">.css-5gn4a3{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:static;background-color:transparent;color:inherit;border:0px solid;box-shadow:none;width:25%;min-width:100px;}</style><style data-emotion="css wme2cb">.css-wme2cb{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:static;background-color:transparent;color:inherit;border:0px solid;box-shadow:none;width:25%;min-width:100px;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionStatic css-wme2cb"><style data-emotion="css orq8zk">.css-orq8zk{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;}@media (max-width:599.95px){.css-orq8zk .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root css-orq8zk"><style data-emotion="css 1anid1y">.css-1anid1y{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;overflow-x:hidden;width:100%;}</style><div class="MuiTabs-scroller MuiTabs-fixed css-1anid1y" style="overflow:hidden;margin-bottom:0"><div aria-label="action tabs example" class="MuiTabs-flexContainer css-k008qs" role="tablist"><style data-emotion="css 120y4ww">.css-120y4ww{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:none;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:1;-ms-flex-negative:1;flex-shrink:1;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(0, 0, 0, 0.6);-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;}.css-120y4ww.Mui-selected{color:#0f1f37;}.css-120y4ww.Mui-disabled{color:rgba(0, 0, 0, 0.38);}</style><style data-emotion="css evzcd5">.css-evzcd5{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:none;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:1;-ms-flex-negative:1;flex-shrink:1;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(0, 0, 0, 0.6);-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;}.css-evzcd5::-moz-focus-inner{border-style:none;}.css-evzcd5.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-evzcd5{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-evzcd5.Mui-selected{color:#0f1f37;}.css-evzcd5.Mui-disabled{color:rgba(0, 0, 0, 0.38);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary MuiTab-fullWidth Mui-selected css-evzcd5" tabindex="0" type="button" role="tab" aria-selected="true" id="action-tab-0" aria-controls="action-tabpanel-0"><div class="MuiBox-root css-k008qs"><style data-emotion="css 2h34d7">.css-2h34d7{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;margin-top:-3px;font-size:20px;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-2h34d7" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="PlayArrowOutlinedIcon"><path d="M10 8.64 15.27 12 10 15.36V8.64M8 5v14l11-7L8 5z"></path></svg><style data-emotion="css 1uqqc8d">.css-1uqqc8d{margin:0;font-family:"Open Sans","Source Sans","Helvetica",sans-serif;font-size:12px;margin-left:5px;}</style><span class="MuiTypography-root MuiTypography-mainTextSmall css-1uqqc8d">demo</span></div><style data-emotion="css fss1su">.css-fss1su{position:absolute;height:2px;bottom:0;width:100%;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#0f1f37;}</style><span class="MuiTabs-indicator css-fss1su"></span></button></div></div></div></header></div></div></div></div></div><style data-emotion="css 1qni66b">.css-1qni66b{margin-top:20px;margin-left:4%;margin-right:4%;min-width:0px;}</style><div class="MuiBox-root css-1qni66b"><style data-emotion="css hboir5">.css-hboir5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;}</style><div class="MuiBox-root css-hboir5" id="modelbodydemo"><style data-emotion="css 1ttywp7">.css-1ttywp7{width:45%;}</style><div class="MuiBox-root css-1ttywp7"><style data-emotion="css eyeyap">.css-eyeyap{float:left;margin-top:0px;width:100%;}</style><div class="MuiBox-root css-eyeyap"><style data-emotion="css 8atqhb">.css-8atqhb{width:100%;}</style><div class="MuiBox-root css-8atqhb" id="demoinput body header"><style data-emotion="css 101bqg5">.css-101bqg5{width:60%;float:left;}</style><div class="MuiBox-root css-101bqg5"><div><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionStatic css-wme2cb"><div class="MuiTabs-root css-orq8zk"><div class="MuiTabs-scroller MuiTabs-fixed css-1anid1y" style="overflow:hidden;margin-bottom:0"><div aria-label="action tabs example" class="MuiTabs-flexContainer css-k008qs" role="tablist"><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary MuiTab-fullWidth Mui-selected css-evzcd5" tabindex="0" type="button" role="tab" aria-selected="true" id="action-tab-0" aria-controls="action-tabpanel-0"><div class="MuiBox-root css-k008qs"><span class="MuiTypography-root MuiTypography-mainTextSmall css-1uqqc8d">Input</span></div><span class="MuiTabs-indicator css-fss1su"></span></button></div></div></div></header></div></div><style data-emotion="css 12h0i53">.css-12h0i53{width:30%;height:40px;float:right;}</style><div class="MuiBox-root css-12h0i53"><div class="mantine-Checkbox-root mantine-1u9ddca"><div class="mantine-14n9mxy mantine-Checkbox-body"><div class="mantine-1vf457v mantine-Checkbox-inner"><input id="mantine-Rakplam" type="checkbox" class="mantine-qjqn4g mantine-Checkbox-input"/><svg viewBox="0 0 10 7" fill="none" xmlns="http://www.w3.org/2000/svg" class="___ref-icon mantine-q9qwbl mantine-Checkbox-icon"><path d="M4 4.586L1.707 2.293A1 1 0 1 0 .293 3.707l3 3a.997.997 0 0 0 1.414 0l5-5A1 1 0 1 0 8.293.293L4 4.586z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg></div><div class="mantine-1svz3tp mantine-Checkbox-labelWrapper"><label class="mantine-9gvgd1 mantine-Checkbox-label" for="mantine-Rakplam">Show optional fields</label></div></div></div></div></div></div><form style="margin-top:70px"><style data-emotion="css crx5el">.css-crx5el{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;gap:26.4px;}</style><div class="MuiBox-root css-crx5el"></div><style data-emotion="css j26rjx">.css-j26rjx{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:end;-ms-flex-pack:end;-webkit-justify-content:flex-end;justify-content:flex-end;margin-top:16px;margin-bottom:20px;}</style><div class="MuiBox-root css-j26rjx"><style data-emotion="css dejwfd">.css-dejwfd{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:5px 15px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;border:1px solid rgba(15, 31, 55, 0.5);color:#0f1f37;margin-left:4px;margin-right:4px;}.css-dejwfd:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(15, 31, 55, 0.04);border:1px solid #0f1f37;}@media (hover: none){.css-dejwfd:hover{background-color:transparent;}}.css-dejwfd.Mui-disabled{color:rgba(0, 0, 0, 0.26);border:1px solid rgba(0, 0, 0, 0.12);}</style><style data-emotion="css 1h38o75">.css-1h38o75{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:5px 15px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;border:1px solid rgba(15, 31, 55, 0.5);color:#0f1f37;margin-left:4px;margin-right:4px;}.css-1h38o75::-moz-focus-inner{border-style:none;}.css-1h38o75.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1h38o75{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1h38o75:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(15, 31, 55, 0.04);border:1px solid #0f1f37;}@media (hover: none){.css-1h38o75:hover{background-color:transparent;}}.css-1h38o75.Mui-disabled{color:rgba(0, 0, 0, 0.26);border:1px solid rgba(0, 0, 0, 0.12);}</style><button class="MuiButtonBase-root MuiButton-root MuiButton-outlined MuiButton-outlinedPrimary MuiButton-sizeMedium MuiButton-outlinedSizeMedium MuiButton-root MuiButton-outlined MuiButton-outlinedPrimary MuiButton-sizeMedium MuiButton-outlinedSizeMedium css-1h38o75" tabindex="0" type="button"><style data-emotion="css 6xugel">.css-6xugel{display:inherit;margin-right:8px;margin-left:-4px;}.css-6xugel>*:nth-of-type(1){font-size:20px;}</style><span class="MuiButton-startIcon MuiButton-iconSizeMedium css-6xugel"><style data-emotion="css 76vawj">.css-76vawj{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;margin-top:-3px;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-76vawj" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="RestartAltIcon"><path d="M12 5V2L8 6l4 4V7c3.31 0 6 2.69 6 6 0 2.97-2.17 5.43-5 5.91v2.02c3.95-.49 7-3.85 7-7.93 0-4.42-3.58-8-8-8zm-6 8c0-1.65.67-3.15 1.76-4.24L6.34 7.34C4.9 8.79 4 10.79 4 13c0 4.08 3.05 7.44 7 7.93v-2.02c-2.83-.48-5-2.94-5-5.91z"></path></svg></span>Reset</button><style data-emotion="css ahepi3">.css-ahepi3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 16px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#fff;background-color:#0f1f37;box-shadow:0px 3px 1px -2px rgba(0,0,0,0.2),0px 2px 2px 0px rgba(0,0,0,0.14),0px 1px 5px 0px rgba(0,0,0,0.12);margin-left:4px;}.css-ahepi3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgb(10, 21, 38);box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);}@media (hover: none){.css-ahepi3:hover{background-color:#0f1f37;}}.css-ahepi3:active{box-shadow:0px 5px 5px -3px rgba(0,0,0,0.2),0px 8px 10px 1px rgba(0,0,0,0.14),0px 3px 14px 2px rgba(0,0,0,0.12);}.css-ahepi3.Mui-focusVisible{box-shadow:0px 3px 5px -1px rgba(0,0,0,0.2),0px 6px 10px 0px rgba(0,0,0,0.14),0px 1px 18px 0px rgba(0,0,0,0.12);}.css-ahepi3.Mui-disabled{color:rgba(0, 0, 0, 0.26);box-shadow:none;background-color:rgba(0, 0, 0, 0.12);}</style><style data-emotion="css 1gatag6">.css-1gatag6{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 16px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#fff;background-color:#0f1f37;box-shadow:0px 3px 1px -2px rgba(0,0,0,0.2),0px 2px 2px 0px rgba(0,0,0,0.14),0px 1px 5px 0px rgba(0,0,0,0.12);margin-left:4px;}.css-1gatag6::-moz-focus-inner{border-style:none;}.css-1gatag6.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1gatag6{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1gatag6:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgb(10, 21, 38);box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);}@media (hover: none){.css-1gatag6:hover{background-color:#0f1f37;}}.css-1gatag6:active{box-shadow:0px 5px 5px -3px rgba(0,0,0,0.2),0px 8px 10px 1px rgba(0,0,0,0.14),0px 3px 14px 2px rgba(0,0,0,0.12);}.css-1gatag6.Mui-focusVisible{box-shadow:0px 3px 5px -1px rgba(0,0,0,0.2),0px 6px 10px 0px rgba(0,0,0,0.14),0px 1px 18px 0px rgba(0,0,0,0.12);}.css-1gatag6.Mui-disabled{color:rgba(0, 0, 0, 0.26);box-shadow:none;background-color:rgba(0, 0, 0, 0.12);}</style><button class="MuiButtonBase-root MuiButton-root MuiButton-contained MuiButton-containedPrimary MuiButton-sizeMedium MuiButton-containedSizeMedium MuiButton-root MuiButton-contained MuiButton-containedPrimary MuiButton-sizeMedium MuiButton-containedSizeMedium css-1gatag6" tabindex="0" type="submit"><span class="MuiButton-startIcon MuiButton-iconSizeMedium css-6xugel"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-76vawj" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="DoubleArrowIcon"><path d="M15.5 5H11l5 7-5 7h4.5l5-7z"></path><path d="M8.5 5H4l5 7-5 7h4.5l5-7z"></path></svg></span>Run</button></div></form></div><style data-emotion="css 1d09i41">.css-1d09i41{width:50%;margin-left:5%;margin-top:0%;}</style><div class="MuiBox-root css-1d09i41" id="modelbodydemooutput"><style data-emotion="css 2aqw9r">.css-2aqw9r{width:100%;display:column;text-align:center;}</style><div class="MuiBox-root css-2aqw9r" id="preloadscreen"><style data-emotion="css yfgiza">.css-yfgiza{height:20%;width:25%;-webkit-print-color-scheme:black;color-scheme:black;margin-top:100px;opacity:0.6;}</style><img class="MuiBox-root css-yfgiza" alt="tungsten_logo" src="/tungsten_greyed_out_logo.png"/><style data-emotion="css 195yhvd">.css-195yhvd{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;font-size:18px;width:100%;margin:auto;margin-top:50px;text-align:center;opacity:0.5;}</style><p class="MuiTypography-root MuiTypography-body1 css-195yhvd">Please fill in the input fields to see the results</p></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"qTYF6hz8zCCC7Oy_19hX7","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/6c93262152699231.css" as="style"/><link rel="stylesheet" href="/_next/static/css/6c93262152699231.css" data-n-g=""/><link rel="preload" href="/_next/static/css/e19e5222d7a223c1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e19e5222d7a223c1.css" data-n-p=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-3c54a28f0adb43ad.js" defer=""></script><script src="/_next/static/chunks/framework-73b8966a3c579ab0.js" defer=""></script><script src="/_next/static/chunks/main-6260d066cf2cd7b1.js" defer=""></script><script src="/_next/static/chunks/pages/_app-055212ca45717427.js" defer=""></script><script src="/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js" defer=""></script><script src="/_next/static/chunks/934-e0819d120eb89b62.js" defer=""></script><script src="/_next/static/chunks/pages/index-ec668a0a6e43b7f3.js" defer=""></script><script src="/_next/static/S40LwJxEK4Dfl_G1r0OjF/_buildManifest.js" defer=""></script><script src="/_next/static/S40LwJxEK4Dfl_G1r0OjF/_ssgManifest.js" defer=""></script></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1kvm0ug">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:1rem;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css 1t3x66l">.css-1t3x66l{background-color:white;min-height:100vh;}</style><div class="MuiBox-root css-1t3x66l" id="main header"><style data-emotion="css ylfuw0">.css-ylfuw0{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:white;border:1px solid #E1E2E6;min-width:900px;}</style><div class="MuiBox-root css-ylfuw0"><style data-emotion="css jsa4zg">.css-jsa4zg{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;margin-left:4%;margin-right:4%;min-width:800px;}</style><div class="MuiBox-root css-jsa4zg"><div class="MuiBox-root css-0" style="width:100%;margin-top:2%;display:inline"><style data-emotion="css k008qs">.css-k008qs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;}</style><div class="MuiBox-root css-k008qs"><div class="mantine-Avatar-root mantine-qnn0x"><div class="mantine-1tfrire mantine-Avatar-placeholder"><svg class="mantine-13sjtfj mantine-Avatar-placeholderIcon" width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.877014 7.49988C0.877014 3.84219 3.84216 0.877045 7.49985 0.877045C11.1575 0.877045 14.1227 3.84219 14.1227 7.49988C14.1227 11.1575 11.1575 14.1227 7.49985 14.1227C3.84216 14.1227 0.877014 11.1575 0.877014 7.49988ZM7.49985 1.82704C4.36683 1.82704 1.82701 4.36686 1.82701 7.49988C1.82701 8.97196 2.38774 10.3131 3.30727 11.3213C4.19074 9.94119 5.73818 9.02499 7.50023 9.02499C9.26206 9.02499 10.8093 9.94097 11.6929 11.3208C12.6121 10.3127 13.1727 8.97172 13.1727 7.49988C13.1727 4.36686 10.6328 1.82704 7.49985 1.82704ZM10.9818 11.9787C10.2839 10.7795 8.9857 9.97499 7.50023 9.97499C6.01458 9.97499 4.71624 10.7797 4.01845 11.9791C4.97952 12.7272 6.18765 13.1727 7.49985 13.1727C8.81227 13.1727 10.0206 12.727 10.9818 11.9787ZM5.14999 6.50487C5.14999 5.207 6.20212 4.15487 7.49999 4.15487C8.79786 4.15487 9.84999 5.207 9.84999 6.50487C9.84999 7.80274 8.79786 8.85487 7.49999 8.85487C6.20212 8.85487 5.14999 7.80274 5.14999 6.50487ZM7.49999 5.10487C6.72679 5.10487 6.09999 5.73167 6.09999 6.50487C6.09999 7.27807 6.72679 7.90487 7.49999 7.90487C8.27319 7.90487 8.89999 7.27807 8.89999 6.50487C8.89999 5.73167 8.27319 5.10487 7.49999 5.10487Z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg></div></div><div class="MuiBox-root css-0" style="margin-left:20px;height:75px;display:inline"><div class="MuiBox-root css-0" style="height:fit-content;width:100%;position:relative;float:left"><style data-emotion="css 1su0e22">.css-1su0e22{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5rem;line-height:1.334;letter-spacing:0em;float:left;}</style><h5 class="MuiTypography-root MuiTypography-h5 css-1su0e22"></h5></div><div class="MuiBox-root css-0" style="width:100%;height:fit-content;float:left;margin-top:0px"><style data-emotion="css 1ww87vj">.css-1ww87vj{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;color:#677285;float:left;font-size:18px;}</style><p class="MuiTypography-root MuiTypography-body1 css-1ww87vj"></p></div></div></div><style data-emotion="css 1ejdhgq">.css-1ejdhgq{width:40%;margin-top:15px;}</style><div class="MuiBox-root css-1ejdhgq"><div><style data-emotion="css 5gn4a3">.css-5gn4a3{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:static;background-color:transparent;color:inherit;border:0px solid;box-shadow:none;width:25%;min-width:100px;}</style><style data-emotion="css wme2cb">.css-wme2cb{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:static;background-color:transparent;color:inherit;border:0px solid;box-shadow:none;width:25%;min-width:100px;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionStatic css-wme2cb"><style data-emotion="css orq8zk">.css-orq8zk{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;}@media (max-width:599.95px){.css-orq8zk .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root css-orq8zk"><style data-emotion="css 1anid1y">.css-1anid1y{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;overflow-x:hidden;width:100%;}</style><div class="MuiTabs-scroller MuiTabs-fixed css-1anid1y" style="overflow:hidden;margin-bottom:0"><div aria-label="action tabs example" class="MuiTabs-flexContainer css-k008qs" role="tablist"><style data-emotion="css 120y4ww">.css-120y4ww{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:none;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:1;-ms-flex-negative:1;flex-shrink:1;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(0, 0, 0, 0.6);-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;}.css-120y4ww.Mui-selected{color:#0f1f37;}.css-120y4ww.Mui-disabled{color:rgba(0, 0, 0, 0.38);}</style><style data-emotion="css evzcd5">.css-evzcd5{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:none;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:1;-ms-flex-negative:1;flex-shrink:1;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(0, 0, 0, 0.6);-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;}.css-evzcd5::-moz-focus-inner{border-style:none;}.css-evzcd5.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-evzcd5{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-evzcd5.Mui-selected{color:#0f1f37;}.css-evzcd5.Mui-disabled{color:rgba(0, 0, 0, 0.38);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary MuiTab-fullWidth Mui-selected css-evzcd5" tabindex="0" type="button" role="tab" aria-selected="true" id="action-tab-0" aria-controls="action-tabpanel-0"><div class="MuiBox-root css-k008qs"><style data-emotion="css 2h34d7">.css-2h34d7{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;margin-top:-3px;font-size:20px;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-2h34d7" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="PlayArrowOutlinedIcon"><path d="M10 8.64 15.27 12 10 15.36V8.64M8 5v14l11-7L8 5z"></path></svg><style data-emotion="css 1uqqc8d">.css-1uqqc8d{margin:0;font-family:"Open Sans","Source Sans","Helvetica",sans-serif;font-size:12px;margin-left:5px;}</style><span class="MuiTypography-root MuiTypography-mainTextSmall css-1uqqc8d">demo</span></div><style data-emotion="css fss1su">.css-fss1su{position:absolute;height:2px;bottom:0;width:100%;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#0f1f37;}</style><span class="MuiTabs-indicator css-fss1su"></span></button></div></div></div></header></div></div></div></div></div><style data-emotion="css 1qni66b">.css-1qni66b{margin-top:20px;margin-left:4%;margin-right:4%;min-width:0px;}</style><div class="MuiBox-root css-1qni66b"><style data-emotion="css hboir5">.css-hboir5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;}</style><div class="MuiBox-root css-hboir5" id="modelbodydemo"><style data-emotion="css 1ttywp7">.css-1ttywp7{width:45%;}</style><div class="MuiBox-root css-1ttywp7"><style data-emotion="css eyeyap">.css-eyeyap{float:left;margin-top:0px;width:100%;}</style><div class="MuiBox-root css-eyeyap"><style data-emotion="css 8atqhb">.css-8atqhb{width:100%;}</style><div class="MuiBox-root css-8atqhb" id="demoinput body header"><style data-emotion="css 101bqg5">.css-101bqg5{width:60%;float:left;}</style><div class="MuiBox-root css-101bqg5"><div><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionStatic css-wme2cb"><div class="MuiTabs-root css-orq8zk"><div class="MuiTabs-scroller MuiTabs-fixed css-1anid1y" style="overflow:hidden;margin-bottom:0"><div aria-label="action tabs example" class="MuiTabs-flexContainer css-k008qs" role="tablist"><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary MuiTab-fullWidth Mui-selected css-evzcd5" tabindex="0" type="button" role="tab" aria-selected="true" id="action-tab-0" aria-controls="action-tabpanel-0"><div class="MuiBox-root css-k008qs"><span class="MuiTypography-root MuiTypography-mainTextSmall css-1uqqc8d">Input</span></div><span class="MuiTabs-indicator css-fss1su"></span></button></div></div></div></header></div></div><style data-emotion="css 12h0i53">.css-12h0i53{width:30%;height:40px;float:right;}</style><div class="MuiBox-root css-12h0i53"><div class="mantine-Checkbox-root mantine-1u9ddca"><div class="mantine-14n9mxy mantine-Checkbox-body"><div class="mantine-1vf457v mantine-Checkbox-inner"><input id="mantine-Rakplam" type="checkbox" class="mantine-qjqn4g mantine-Checkbox-input"/><svg viewBox="0 0 10 7" fill="none" xmlns="http://www.w3.org/2000/svg" class="___ref-icon mantine-q9qwbl mantine-Checkbox-icon"><path d="M4 4.586L1.707 2.293A1 1 0 1 0 .293 3.707l3 3a.997.997 0 0 0 1.414 0l5-5A1 1 0 1 0 8.293.293L4 4.586z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg></div><div class="mantine-1svz3tp mantine-Checkbox-labelWrapper"><label class="mantine-9gvgd1 mantine-Checkbox-label" for="mantine-Rakplam">Show optional fields</label></div></div></div></div></div></div><form style="margin-top:70px"><style data-emotion="css crx5el">.css-crx5el{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;gap:26.4px;}</style><div class="MuiBox-root css-crx5el"></div><style data-emotion="css j26rjx">.css-j26rjx{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:end;-ms-flex-pack:end;-webkit-justify-content:flex-end;justify-content:flex-end;margin-top:16px;margin-bottom:20px;}</style><div class="MuiBox-root css-j26rjx"><style data-emotion="css dejwfd">.css-dejwfd{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:5px 15px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;border:1px solid rgba(15, 31, 55, 0.5);color:#0f1f37;margin-left:4px;margin-right:4px;}.css-dejwfd:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(15, 31, 55, 0.04);border:1px solid #0f1f37;}@media (hover: none){.css-dejwfd:hover{background-color:transparent;}}.css-dejwfd.Mui-disabled{color:rgba(0, 0, 0, 0.26);border:1px solid rgba(0, 0, 0, 0.12);}</style><style data-emotion="css 1h38o75">.css-1h38o75{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:5px 15px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;border:1px solid rgba(15, 31, 55, 0.5);color:#0f1f37;margin-left:4px;margin-right:4px;}.css-1h38o75::-moz-focus-inner{border-style:none;}.css-1h38o75.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1h38o75{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1h38o75:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(15, 31, 55, 0.04);border:1px solid #0f1f37;}@media (hover: none){.css-1h38o75:hover{background-color:transparent;}}.css-1h38o75.Mui-disabled{color:rgba(0, 0, 0, 0.26);border:1px solid rgba(0, 0, 0, 0.12);}</style><button class="MuiButtonBase-root MuiButton-root MuiButton-outlined MuiButton-outlinedPrimary MuiButton-sizeMedium MuiButton-outlinedSizeMedium MuiButton-root MuiButton-outlined MuiButton-outlinedPrimary MuiButton-sizeMedium MuiButton-outlinedSizeMedium css-1h38o75" tabindex="0" type="button"><style data-emotion="css 6xugel">.css-6xugel{display:inherit;margin-right:8px;margin-left:-4px;}.css-6xugel>*:nth-of-type(1){font-size:20px;}</style><span class="MuiButton-startIcon MuiButton-iconSizeMedium css-6xugel"><style data-emotion="css 76vawj">.css-76vawj{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;margin-top:-3px;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-76vawj" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="RestartAltIcon"><path d="M12 5V2L8 6l4 4V7c3.31 0 6 2.69 6 6 0 2.97-2.17 5.43-5 5.91v2.02c3.95-.49 7-3.85 7-7.93 0-4.42-3.58-8-8-8zm-6 8c0-1.65.67-3.15 1.76-4.24L6.34 7.34C4.9 8.79 4 10.79 4 13c0 4.08 3.05 7.44 7 7.93v-2.02c-2.83-.48-5-2.94-5-5.91z"></path></svg></span>Reset</button><style data-emotion="css ahepi3">.css-ahepi3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 16px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#fff;background-color:#0f1f37;box-shadow:0px 3px 1px -2px rgba(0,0,0,0.2),0px 2px 2px 0px rgba(0,0,0,0.14),0px 1px 5px 0px rgba(0,0,0,0.12);margin-left:4px;}.css-ahepi3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgb(10, 21, 38);box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);}@media (hover: none){.css-ahepi3:hover{background-color:#0f1f37;}}.css-ahepi3:active{box-shadow:0px 5px 5px -3px rgba(0,0,0,0.2),0px 8px 10px 1px rgba(0,0,0,0.14),0px 3px 14px 2px rgba(0,0,0,0.12);}.css-ahepi3.Mui-focusVisible{box-shadow:0px 3px 5px -1px rgba(0,0,0,0.2),0px 6px 10px 0px rgba(0,0,0,0.14),0px 1px 18px 0px rgba(0,0,0,0.12);}.css-ahepi3.Mui-disabled{color:rgba(0, 0, 0, 0.26);box-shadow:none;background-color:rgba(0, 0, 0, 0.12);}</style><style data-emotion="css 1gatag6">.css-1gatag6{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 16px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#fff;background-color:#0f1f37;box-shadow:0px 3px 1px -2px rgba(0,0,0,0.2),0px 2px 2px 0px rgba(0,0,0,0.14),0px 1px 5px 0px rgba(0,0,0,0.12);margin-left:4px;}.css-1gatag6::-moz-focus-inner{border-style:none;}.css-1gatag6.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1gatag6{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1gatag6:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgb(10, 21, 38);box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);}@media (hover: none){.css-1gatag6:hover{background-color:#0f1f37;}}.css-1gatag6:active{box-shadow:0px 5px 5px -3px rgba(0,0,0,0.2),0px 8px 10px 1px rgba(0,0,0,0.14),0px 3px 14px 2px rgba(0,0,0,0.12);}.css-1gatag6.Mui-focusVisible{box-shadow:0px 3px 5px -1px rgba(0,0,0,0.2),0px 6px 10px 0px rgba(0,0,0,0.14),0px 1px 18px 0px rgba(0,0,0,0.12);}.css-1gatag6.Mui-disabled{color:rgba(0, 0, 0, 0.26);box-shadow:none;background-color:rgba(0, 0, 0, 0.12);}</style><button class="MuiButtonBase-root MuiButton-root MuiButton-contained MuiButton-containedPrimary MuiButton-sizeMedium MuiButton-containedSizeMedium MuiButton-root MuiButton-contained MuiButton-containedPrimary MuiButton-sizeMedium MuiButton-containedSizeMedium css-1gatag6" tabindex="0" type="submit"><span class="MuiButton-startIcon MuiButton-iconSizeMedium css-6xugel"><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-76vawj" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="DoubleArrowIcon"><path d="M15.5 5H11l5 7-5 7h4.5l5-7z"></path><path d="M8.5 5H4l5 7-5 7h4.5l5-7z"></path></svg></span>Run</button></div></form></div><style data-emotion="css 1d09i41">.css-1d09i41{width:50%;margin-left:5%;margin-top:0%;}</style><div class="MuiBox-root css-1d09i41" id="modelbodydemooutput"><style data-emotion="css 2aqw9r">.css-2aqw9r{width:100%;display:column;text-align:center;}</style><div class="MuiBox-root css-2aqw9r" id="preloadscreen"><style data-emotion="css yfgiza">.css-yfgiza{height:20%;width:25%;-webkit-print-color-scheme:black;color-scheme:black;margin-top:100px;opacity:0.6;}</style><img class="MuiBox-root css-yfgiza" alt="tungsten_logo" src="/tungsten_greyed_out_logo.png"/><style data-emotion="css 195yhvd">.css-195yhvd{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;font-size:18px;width:100%;margin:auto;margin-top:50px;text-align:center;opacity:0.5;}</style><p class="MuiTypography-root MuiTypography-body1 css-195yhvd">Please fill in the input fields to see the results</p></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"S40LwJxEK4Dfl_G1r0OjF","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/next.svg` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/next.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/thirteen.svg` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/thirteen.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/frontend/vercel.svg` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/frontend/vercel.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/io.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         scheme = self.get_scheme()
 
         if scheme == "data":
             path = save_data_url(self, ".")
             return URIForFile(Path(path).as_uri())
 
         if scheme == "http" or scheme == "https":
-            download_file(url=self, out_path=".")
+            return URIForFile(download_file(url=self, out_path=".").as_uri())
 
         return self
 
     def to_data_uri(self) -> "URIForFile":
         scheme = self.get_scheme()
 
         if scheme == "data":
@@ -177,14 +177,18 @@
     @classmethod
     def __modify_schema__(
         cls, field_schema: t.Dict[str, t.Any], field: t.Optional[ModelField]
     ) -> None:
         field_schema["type"] = "string"
         field_schema["format"] = "uri"
 
+        default = field.default if field else None
+        if isinstance(default, File):
+            field_schema["default"] = default.__root__
+
     @classmethod
     def _get_typeenum(cls) -> FileType:
         return FileType(camel_to_snake(cls.__name__))
 
 
 class Image(File):
     @staticmethod
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/json_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     for o in demo_outputs:
         try:
             if o is None:
                 validated_demo_outputs.append(o)
             elif isinstance(o, demo_output_cls):
                 validated_demo_outputs.append(jsonable_encoder(run_validation(o)))
             elif isinstance(o, dict):
-                validated_demo_outputs.append(jsonable_encoder(demo_output_cls.parse_obj(o)))
+                validated_demo_outputs.append(jsonable_encoder(demo_output_cls(**o)))
             else:
                 raise exceptions.InvalidDemoOutput(
                     f"Invalid demo output type: {type(o)}. "
                     f"Allowed types: 'dict' and '{BaseIO}'"
                 )
         except pydantic.error_wrappers.ValidationError as e:
             raise exceptions.InvalidDemoOutput(str(e))
@@ -232,15 +232,15 @@
 ) -> t.List[t.Dict]:
     validated_outputs: t.List[t.Dict] = []
     for o in outputs:
         try:
             if isinstance(o, output_cls):
                 validated_outputs.append(jsonable_encoder(run_validation(o)))
             elif isinstance(o, dict):
-                validated_outputs.append(jsonable_encoder(output_cls.parse_obj(o)))
+                validated_outputs.append(jsonable_encoder(output_cls(**o)))
             else:
                 raise exceptions.InvalidOutput(
                     f"Invalid output type: {type(o)}. Allowed types: 'dict' and "
                     f"'{get_qualname(output_cls)}'"
                 )
         except pydantic.error_wrappers.ValidationError as e:
             raise exceptions.InvalidOutput(str(e))
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/avatar_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/model_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/storables/source_file_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/task.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,16 @@
                 input_schema=model.io.input_schema,
                 output_schema=model.io.output_schema,
                 demo_output_schema=model.io.demo_output_schema,
                 input_filetypes=model.io.input_filetypes,
                 output_filetypes=model.io.output_filetypes,
                 demo_output_filetypes=model.io.demo_output_filetypes,
                 gpu_memory=model.gpu_mem_gb * 1024 * 1024 if model.gpu and model.gpu_mem_gb else 0,
-                source_files=source_files,
-                skipped_source_files=skipped_source_files,
+                # source_files=source_files,
+                # skipped_source_files=skipped_source_files,
             )
 
             model_in_server = self.api.create_model(project=project, req=req)
             log_debug("Response: " + str(model_in_server), pretty=False)
 
             if model.readme:
                 log_info("Updating the README")
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 
     source_files: List[SourceFileDecl] = Field(default_factory=list)
     skipped_source_files: List[SkippedSourceFileDecl] = Field(default_factory=list)
 
     gpu_memory: int
 
 
+class ModelCreator(BaseModel):
+    id: int
+    username: str
+    name: str
+    avatar_url: str
+
+
 class Model(BaseModel):
     id: int
     project_id: int
     project_full_slug: str
 
     version: str
 
@@ -56,15 +63,15 @@
     gpu_memory: int
 
     readme_url: Optional[str]
 
     source_files_count: int
     examples_count: int
 
-    creator: User
+    creator: ModelCreator
     created_at: datetime
 
 
 class ModelReadmeUpdate(BaseModel):
     content: str
 
 
@@ -79,15 +86,15 @@
 class ModelPredictionExample(BaseModel):
     id: int
 
     input: dict
     output: dict
     demo_output: dict
 
-    creator: User
+    creator: ModelCreator
     created_at: datetime
 
 
 class ListModelPredictionExamples(BaseModel):
     __root__: List[ModelPredictionExample]
```

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/types.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.1a1/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/tungstenkit/exceptions.py` & `tungstenkit-0.1.1a1/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.0/PKG-INFO` & `tungstenkit-0.1.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -73,15 +73,15 @@
 
 # Tungstenkit: ML container made simple
 [![Version](https://img.shields.io/pypi/v/tungstenkit?color=%2334D058&label=pypi%20package)](https://pypi.org/project/tungstenkit/)
 [![License](https://img.shields.io/github/license/tungsten-ai/tungstenkit)](https://raw.githubusercontent.com/tungsten-ai/tungstenkit/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/tungstenkit?style=flat-square)](https://pypi.org/project/tungstenkit/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/tungstenkit.svg?color=%2334D058)](https://pypi.org/project/tungstenkit/)
 
-[Features](#features) | [Installation](#prerequisites) | [Getting Started](https://tungsten-ai.github.io/docs/getting_started) | [Documentation](https://tungsten-ai.github.io/docs) 
+[Introduction](#tungstenkit-ml-container-made-simple) | [Installation](#prerequisites) | [Getting Started](https://tungsten-ai.github.io/docs/getting_started) | [Documentation](https://tungsten-ai.github.io/docs) 
 
 Tungstenkit is ML containerization tool with a focus on developer productivity and versatility.
 
 The key features are:
 
 - [Requires only a few lines of Python code](#requires-only-a-few-lines-of-python-code)
 - [Build once, use everywhere](#build-once-use-everywhere):
```

