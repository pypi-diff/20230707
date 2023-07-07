# Comparing `tmp/tungstenkit-0.1.1a2.tar.gz` & `tmp/tungstenkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.1a2.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.2.tar", max compression
```

## Comparing `tungstenkit-0.1.1a2.tar` & `tungstenkit-0.1.2.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.1a2/README.md
--rw-r--r--   0        0        0     2870 2023-07-06 11:31:13.357118 tungstenkit-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.1a2/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.1a2/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0     9630 2023-06-07 05:35:48.388092 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5460 2023-07-06 11:26:24.750220 tungstenkit-0.1.1a2/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.1a2/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    14492 2023-07-06 11:25:00.322496 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     8429 2023-07-06 11:23:40.274731 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1337 2023-07-06 06:51:45.833948 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1381 2023-07-06 07:14:54.727252 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     3804 2023-07-05 06:46:26.252964 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1593 2023-07-05 06:44:48.858561 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4369 2023-07-05 06:49:54.926011 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6551 2023-07-05 06:47:11.688272 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
--rw-r--r--   0        0        0     3573 2023-06-07 06:31:35.793599 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      723 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     7935 2023-07-05 06:49:26.654380 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      924 2023-05-05 07:02:23.660425 tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.1a2/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.1a2/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-06 10:35:33.693110 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0     6231 2023-07-06 10:35:33.677110 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/500.html
--rw-r--r--   0        0        0   707673 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/657-2e4c261bfa28c304.js
--rw-r--r--   0        0        0    78459 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
--rw-r--r--   0        0        0   458866 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
--rw-r--r--   0        0        0   141052 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    89842 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
--rw-r--r--   0        0        0     5020 2023-07-06 10:35:33.325117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
--rw-r--r--   0        0        0     5049 2023-07-06 10:35:33.325117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
--rw-r--r--   0        0        0   130456 2023-07-06 10:35:33.325117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
--rw-r--r--   0        0        0      245 2023-07-06 10:35:33.325117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0        0        0    28371 2023-07-06 10:35:33.325117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-8f3afe3801b5eb58.js
--rw-r--r--   0        0        0    91460 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-c7250373c9756530.js
--rw-r--r--   0        0        0      791 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
--rw-r--r--   0        0        0    43645 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
--rw-r--r--   0        0        0      525 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/fMfFQ47widM1tYI27opXD/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-07-06 10:35:33.321117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/fMfFQ47widM1tYI27opXD/_ssgManifest.js
--rw-r--r--   0        0        0   259838 2023-07-06 10:35:33.329117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0     6244 2023-07-06 10:35:33.689110 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0    61184 2023-07-06 10:35:33.329117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0    27505 2023-07-06 10:35:33.329117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-07-06 10:35:33.329117 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12095 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11504 2023-07-04 14:01:36.561839 tungstenkit-0.1.1a2/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     7252 2023-06-02 08:07:56.573968 tungstenkit-0.1.1a2/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    11261 2023-06-07 06:14:27.599650 tungstenkit-0.1.1a2/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.1a2/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.1a2/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      606 2023-06-01 15:06:58.874575 tungstenkit-0.1.1a2/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.1a2/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.1a2/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    14054 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0     9948 2023-07-06 10:41:00.583575 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      509 2023-06-05 12:56:44.197918 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     2054 2023-06-26 07:20:09.814702 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     6213 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      967 2023-05-25 12:26:56.640679 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6335 2023-05-25 09:44:14.934739 tungstenkit-0.1.1a2/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.1a2/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2379 2023-06-02 12:43:00.699193 tungstenkit-0.1.1a2/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.1a2/tungstenkit/models.py
--rw-r--r--   0        0        0    10561 1970-01-01 00:00:00.000000 tungstenkit-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2/README.md
+-rw-r--r--   0        0        0     2868 2023-07-07 09:00:14.627450 tungstenkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-05 05:24:44.708624 tungstenkit-0.1.2/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0     9630 2023-06-07 05:35:48.388092 tungstenkit-0.1.2/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5460 2023-07-06 11:26:24.750220 tungstenkit-0.1.2/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.2/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    14492 2023-07-06 11:25:00.322496 tungstenkit-0.1.2/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     8398 2023-07-07 09:00:11.183463 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1337 2023-07-06 06:51:45.833948 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1381 2023-07-06 07:14:54.727252 tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
+-rw-r--r--   0        0        0     3573 2023-06-07 06:31:35.793599 tungstenkit-0.1.2/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-06 20:22:25.417271 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0     6231 2023-07-06 20:22:25.381271 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/500.html
+-rw-r--r--   0        0        0      523 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js
+-rw-r--r--   0        0        0   707397 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js
+-rw-r--r--   0        0        0    78459 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
+-rw-r--r--   0        0        0   458866 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
+-rw-r--r--   0        0        0   141052 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    89842 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
+-rw-r--r--   0        0        0     5020 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
+-rw-r--r--   0        0        0     5049 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
+-rw-r--r--   0        0        0   130456 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
+-rw-r--r--   0        0        0      245 2023-07-06 20:22:25.037277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0        0        0    28246 2023-07-06 20:22:25.037277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js
+-rw-r--r--   0        0        0    91460 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3851 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js
+-rw-r--r--   0        0        0      791 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
+-rw-r--r--   0        0        0    43645 2023-07-06 20:22:25.033277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
+-rw-r--r--   0        0        0   259838 2023-07-06 20:22:25.041277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0     6242 2023-07-06 20:22:25.393271 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0    61184 2023-07-06 20:22:25.041277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0    27505 2023-07-06 20:22:25.041277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-07-06 20:22:25.041277 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12615 2023-07-06 20:23:59.011863 tungstenkit-0.1.2/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    11261 2023-06-07 06:14:27.599650 tungstenkit-0.1.2/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.2/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.2/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      606 2023-06-01 15:06:58.874575 tungstenkit-0.1.2/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    14054 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0     9948 2023-07-06 10:41:00.583575 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      509 2023-06-05 12:56:44.197918 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2054 2023-06-26 07:20:09.814702 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.2/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     6213 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2379 2023-06-02 12:43:00.699193 tungstenkit-0.1.2/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2/tungstenkit/models.py
+-rw-r--r--   0        0        0    10559 1970-01-01 00:00:00.000000 tungstenkit-0.1.2/PKG-INFO
```

### Comparing `tungstenkit-0.1.1a2/LICENSE` & `tungstenkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/README.md` & `tungstenkit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/pyproject.toml` & `tungstenkit-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.1a2"
+version = "0.1.2"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.2/tungstenkit/_internal/blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.2/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.2/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.2/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.2/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.2/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.2/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.2/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/build_context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from tungstenkit._internal.utils.version import NotRequired
 
 from ..base_images import BaseImage, CUDAImageCollection, CustomImage, PythonImageCollection
 from ..gpu_pkg_collections import supported_gpu_pkg_names
 from ..pkg_manager import PythonPackageManager, RequirementsTxt
 from .template_args import TemplateArgs
 
+LARGE_FILE_THRESHOLD = 100 * 1024**2
+
 
 class BaseDockerfile(metaclass=abc.ABCMeta):
     def __init__(
         self,
         config: BuildConfig,
     ):
         self.config = config
@@ -109,32 +111,31 @@
 
         gpu_pkg_requirements = py_pkg_manager.list_gpu_pkg_pip_requirements()
         for r in gpu_pkg_requirements:
             list_pip_install_args.append(r.to_str().split(" "))
 
         extra_pkg_requirements = py_pkg_manager.list_extra_pkg_pip_requirements()
         for r in extra_pkg_requirements:
-            if r.pip_index_url:
+            if r.index_url:
                 list_pip_install_args.append(r.to_str().split(" "))
             else:
                 requirements_txt.add_requirement(r)
 
         requirements_txt_content = requirements_txt.build()
         pip_requirements_txt_path.write_text(requirements_txt_content)
         log_debug("pip install args: " + str(list_pip_install_args), pretty=False)
         log_debug("python requirements.txt:\n" + requirements_txt_content, pretty=False)
 
         # Set base image
         if self.config.base_image:
             image: BaseImage = CustomImage(self.config.base_image)
-        elif not isinstance(cuda_ver, NotRequired):
+        elif not isinstance(cuda_ver, NotRequired) and py_pkg_manager.requires_system_cuda():
             log_info("Fetching the list of cuda base images")
             cuda_image_collection = CUDAImageCollection.from_docker_hub()
-            # Infered successfully but got None -> any version is ok
-            if cuda_ver is None or not py_pkg_manager.requires_system_cuda:
+            if cuda_ver is None:  # Requires CUDA but any version is okay
                 image = cuda_image_collection.get_latest_image()
             else:
                 image = cuda_image_collection.get_cuda_image_by_cuda_cudnn_ver(cuda_ver, cudnn_ver)
         else:
             log_info("Fetching the list of python base images")
             python_image_collection = PythonImageCollection.from_docker_hub()
             image = python_image_collection.get_py_image_by_ver(py_ver)
@@ -187,16 +188,15 @@
                 if path.is_dir():
                     ret = split(path)
                     large_files.extend(ret[0])
                     small_files.extend(ret[1])
 
                 else:
                     size = path.stat(follow_symlinks=False).st_size
-                    # if size > 100 * 1024**2:
-                    if size > 10 * 1024:
+                    if size > LARGE_FILE_THRESHOLD:
                         large_files.append(path)
                     else:
                         small_files.append(path)
 
             if len(large_files) == 0:
                 return [], [curr_dir]
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/template_args.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,89 @@
 import abc
 import typing as t
 
+from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 
 from tungstenkit._internal.utils.string import removesuffix
 from tungstenkit._internal.utils.version import (
     check_if_two_versions_compatible,
-    check_version_with_constraint,
+    check_version_matching_clause_loosely,
 )
 
 from .common import GPUPackageConstraint, GPUPackageRelease
 
 
 class GPUPackageCollection(abc.ABC):
-    requires_system_cuda: bool
-
     @classmethod
     def init(cls):
         # TODO call from_file or from_remote periodically
         # raise NotImplementedError
         return cls.from_remote()
 
     @classmethod
+    @abc.abstractmethod
     def from_remote(cls):
         raise NotImplementedError
 
     @property
+    @abc.abstractmethod
     def has_no_compatible_vers(self) -> bool:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def get_available_cuda_vers(self, pkg_names: t.List[str]) -> t.Set[t.Optional[Version]]:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def get_available_cudnn_vers(self, pkg_names: t.List[str]) -> t.Set[t.Optional[Version]]:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def get_available_py_vers(self, pkg_names: t.List[str]) -> t.Set[Version]:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def add_constraint(self, constraint: GPUPackageConstraint) -> None:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def get_latest_releases(self, pkg_names: t.Iterable[str]) -> t.List[GPUPackageRelease]:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def get_err_msg_for_constraint(self, constraint: GPUPackageConstraint) -> t.Optional[str]:
         raise NotImplementedError
 
     @classmethod
+    @abc.abstractmethod
+    def requires_system_cuda(cls):
+        raise NotImplementedError
+
+    @classmethod
     def get_pkg_names(cls) -> t.Set[str]:
         raise NotImplementedError
 
     @classmethod
     def name(cls):
         return removesuffix(cls.__name__, "Collection").lower()
 
     @staticmethod
     def filter_releases_by_constraint(
         releases: t.List[GPUPackageRelease], constraint: GPUPackageConstraint
     ) -> t.List[GPUPackageRelease]:
         filter_fns: t.List[t.Callable[[GPUPackageRelease], bool]] = list()
-        if constraint.pkg_ver is not None:
+        if isinstance(constraint.pkg_spec, SpecifierSet):
+            pkg_specifier_set = constraint.pkg_spec
+            filter_fns.append(lambda release: release.pkg_ver in pkg_specifier_set)
+        if isinstance(constraint.pkg_spec, Version):
+            pkg_version_spec = constraint.pkg_spec
             filter_fns.append(
-                lambda release: check_version_with_constraint(
-                    ver=release.pkg_ver, constraint=constraint.pkg_ver
+                lambda release: check_version_matching_clause_loosely(
+                    release.pkg_ver, pkg_version_spec
                 )
             )
         if constraint.no_cuda is not None:
             filter_fns.append(
                 lambda release: release.no_cuda == constraint.no_cuda,
             )
         if constraint.cuda_ver is not None:
@@ -99,10 +115,12 @@
                     )
                     for release_py_ver in release.py_vers
                 ),
             )
         filtered: t.Union[filter, t.List] = releases
         for filter_fn in filter_fns:
             filtered = filter(filter_fn, filtered)
+
         if len(filter_fns) > 0:
-            releases = list(filtered)
-        return releases
+            filtered_list = list(filtered)
+
+        return filtered_list
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 
 import attrs
+from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 
 from tungstenkit._internal.utils.version import MIN_VER, order_optional_version
 
 
 @attrs.frozen(order=True)
 class GPUPackageRelease:
@@ -21,15 +22,15 @@
     pip_extra_index_url: t.Optional[str] = attrs.field(default=None, order=False)
     env_vars: t.Optional[t.Dict[str, str]] = attrs.field(default=None, order=False)
 
 
 @attrs.define
 class GPUPackageConstraint:
     pkg_name: t.Optional[str] = attrs.field(default=None)
-    pkg_ver: t.Optional[Version] = attrs.field(default=None)
+    pkg_spec: t.Optional[SpecifierSet | Version] = attrs.field(default=None)
     no_cuda: t.Optional[bool] = attrs.field(default=None)
     cuda_ver: t.Optional[Version] = attrs.field(default=None)
     any_cuda_in: t.Optional[t.Iterable[Version]] = attrs.field(default=None)
     py_ver: t.Optional[Version] = attrs.field(default=None)
     any_py_in: t.Optional[t.Iterable[Version]] = attrs.field(default=None)
 
     def __attrs_post_init__(self):
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .common import GPUPackageConstraint, GPUPackageRelease
 
 TF_METADATA_URL = "https://www.tensorflow.org/install/source"
 
 
 @attrs.define
 class TFCollection(GPUPackageCollection):
-    requires_system_cuda = True
     releases: t.List[GPUPackageRelease]
 
     @classmethod
     def from_remote(cls):
         all_releases: t.List[GPUPackageRelease] = []
         # TODO add parse error type
 
@@ -119,7 +118,11 @@
 
     def get_latest_releases(self, pkg_names: t.Iterable[str]):
         return [max(self.releases)] if pkg_names else []
 
     def get_err_msg_for_constraint(self, pkg_spec: GPUPackageConstraint):
         # TODO
         return ""
+
+    @classmethod
+    def requires_system_cuda(cls):
+        return True
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
     r"[.]whl"
 )
 
 
 @attrs.define
 class TorchCollection(GPUPackageCollection):
     # TODO filter by available cuda images
-    requires_system_cuda = False
-
     torch: t.List[GPUPackageRelease]
     torchvision: t.List[GPUPackageRelease]
     torchaudio: t.List[GPUPackageRelease]
 
     @classmethod
     def from_remote(cls):
         pkg_names = cls.get_pkg_names()
@@ -169,10 +167,18 @@
     def get_latest_releases(self, pkg_names: t.Iterable[str]):
         return [
             max(getattr(self, pkg_name))
             for pkg_name in self.get_pkg_names()
             if pkg_name in pkg_names
         ]
 
+    def get_err_msg_for_constraint(self, pkg_spec: GPUPackageConstraint):
+        # TODO
+        return ""
+
     @classmethod
     def get_pkg_names(cls):
         return list(attrs.fields_dict(cls).keys())
+
+    @classmethod
+    def requires_system_cuda(cls):
+        return False
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import typing as t
 
 import attrs
+from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 
 
 @attrs.frozen
 class PipRequirement:
     name: str
-    version: t.Optional[Version] = attrs.field(default=None)
-    pip_index_url: t.Optional[str] = attrs.field(default=None)
-    pip_extra_index_url: t.Optional[str] = attrs.field(default=None)
+    spec: t.Optional[Version | SpecifierSet] = attrs.field(default=None)
+    index_url: t.Optional[str] = attrs.field(default=None)
+    extra_index_url: t.Optional[str] = attrs.field(default=None)
 
     def to_str(self, index: bool = True):
         requirement = f"{self.name}"
-        if self.version:
-            requirement += f"=={self.version}"
-        if index and self.pip_index_url:
-            requirement += f" --index-url {self.pip_index_url}"
-        if index and self.pip_extra_index_url:
-            requirement += f" --extra-index-url {self.pip_extra_index_url}"
+        if isinstance(self.spec, Version):
+            requirement += f"=={self.spec}"
+        if isinstance(self.spec, SpecifierSet):
+            requirement += str(self.spec)
+        if index and self.index_url:
+            requirement += f" --index-url {self.index_url}"
+        if index and self.extra_index_url:
+            requirement += f" --extra-index-url {self.extra_index_url}"
         return requirement
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 import typing as t
 
 import attrs
+from packaging.requirements import Requirement
+from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 
 from tungstenkit import exceptions
 from tungstenkit._internal.constants import MAX_SUPPORTED_PYTHON_VER, MIN_SUPPORTED_PYTHON_VER
 from tungstenkit._internal.logging import log_info
 from tungstenkit._internal.utils.version import (
     NotRequired,
@@ -44,46 +46,55 @@
 @attrs.frozen
 class PythonPackageManager:
     _gpu_pkg_collections: t.Dict[str, GPUPackageCollection] = attrs.field(factory=dict, init=False)
     _required_gpu_pkg_names: t.Dict[str, t.Set[str]] = attrs.field(factory=dict, init=False)
     _update_history: t.List[UpdateHistory] = attrs.field(factory=list, init=False)
     _extra_pkgs: t.List[PipRequirement] = attrs.field(factory=list, init=False)
 
-    @property
-    def requires_system_cuda(self):
-        return any(col.requires_system_cuda for col in self._gpu_pkg_collections.values())
+    def requires_system_cuda(self) -> bool:
+        return any(col.requires_system_cuda() for col in self._gpu_pkg_collections.values())
 
     def add_requirement_str(self, requirement_str: str):
         # Parse requirement string
         # TODO support --extra-index-url and --index-url
-        pkg_ver: t.Optional[Version]
-        if "==" in requirement_str:
-            pkg_name, pkg_ver_str = requirement_str.split("==")
-            pkg_ver = Version(pkg_ver_str)
-            if not isinstance(pkg_ver, Version):
-                raise exceptions.PipPackageParseError(f'"{pkg_ver_str}" in python_packages')
+
+        try:
+            parsed = Requirement(requirement_str)
+        except IndexError:
+            raise exceptions.PipPackageParseError(
+                f"No package name in requirement string: {requirement_str}"
+            )
+        except Exception as e:
+            raise exceptions.PipPackageParseError(str(e))
+
+        pkg_name = parsed.name
+        specifier_set = parsed.specifier
+        specifier_list = list(specifier_set)
+
+        if len(specifier_set) == 1 and specifier_list[0].operator == "==":
+            spec: Version | SpecifierSet = Version(specifier_list[0].version)
         else:
-            pkg_name, pkg_ver = requirement_str, None
+            spec = specifier_set
 
         # Check if a GPU package
         collection_name = get_gpu_pkg_collection_name_by_pkg_name(pkg_name)
         if collection_name is None:
-            self._extra_pkgs.append(PipRequirement(name=pkg_name, version=pkg_ver))
+            self._extra_pkgs.append(PipRequirement(name=pkg_name, spec=spec))
             return
 
         # Lazy initialization of a GPU package collection
         if collection_name not in self._gpu_pkg_collections:
             log_info(f"Fetching the list of {collection_name} packages")
             collection_cls = gpu_pkg_collection_class_dict[collection_name]
             self._gpu_pkg_collections[collection_name] = collection_cls.init()
             self._required_gpu_pkg_names[collection_name] = set()
 
         self._required_gpu_pkg_names[collection_name].add(pkg_name)
-        if pkg_ver:
-            self._set_gpu_pkg_constraint(GPUPackageConstraint(pkg_name=pkg_name, pkg_ver=pkg_ver))
+        if spec and (isinstance(spec, Version) or len(spec) > 0):
+            self._set_gpu_pkg_constraint(GPUPackageConstraint(pkg_name=pkg_name, pkg_spec=spec))
 
     def set_gpu(self, gpu: bool):
         self._set_gpu_pkg_constraint(GPUPackageConstraint(no_cuda=not gpu))
 
     def set_cuda_equal_to(self, cuda_ver: Version):
         self._set_gpu_pkg_constraint(GPUPackageConstraint(cuda_ver=cuda_ver))
 
@@ -170,17 +181,17 @@
             gpu_pkgs_in_collection = gpu_pkg_collection.get_latest_releases(
                 self._required_gpu_pkg_names[gpu_pkg_collection_name]
             )
             pkgs.extend(
                 [
                     PipRequirement(
                         name=gpu_pkg.pkg_name,
-                        version=gpu_pkg.pkg_ver,
-                        pip_index_url=gpu_pkg.pip_index_url,
-                        pip_extra_index_url=gpu_pkg.pip_extra_index_url,
+                        spec=gpu_pkg.pkg_ver,
+                        index_url=gpu_pkg.pip_index_url,
+                        extra_index_url=gpu_pkg.pip_extra_index_url,
                     )
                     for gpu_pkg in gpu_pkgs_in_collection
                 ]
             )
         pkgs = sorted(pkgs, key=lambda pkg: pkg.name)
         return pkgs
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
     @property
     def is_empty(self):
         return len(self._pkg_requirements) == 0
 
     def add_requirement(self, requirement: PipRequirement):
         self._pkg_requirements.append(requirement.to_str(index=False))
-        if requirement.pip_extra_index_url:
-            self._extra_index_urls.add(requirement.pip_extra_index_url)
+        if requirement.extra_index_url:
+            self._extra_index_urls.add(requirement.extra_index_url)
 
     def build(self):
         requirements_txt = ""
         for extra_index_url in self._extra_index_urls:
             requirements_txt += f"--extra-index-url {extra_index_url}\n"
         for pkg_requirements in self._pkg_requirements:
             requirements_txt += f"{pkg_requirements}\n"
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.2/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c7250373c9756530.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/pages/404-1e77c517c165fca8.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_buildManifest.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_ssgManifest.js" defer=""></script><style data-emotion="mantine ki47pp 1kzx756 n8pl39 f9w8pv ojrz4j 1uuuflr">.mantine-ki47pp{font-size:9.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-1kzx756{font-size:2.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-n8pl39{font-size:1.375rem;font-weight:500;}.mantine-f9w8pv{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}.mantine-ojrz4j{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-1uuuflr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:0rem;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-f9w8pv"><div class="mantine-Center-root mantine-ojrz4j" style="height:100%"><div class="mantine-Stack-root mantine-1uuuflr"><div class="mantine-ki47pp">404</div><div class="mantine-1kzx756">Page Not Found</div><div class="mantine-n8pl39">The page you are looking for doesn’t exist.</div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"fMfFQ47widM1tYI27opXD","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-fb2189cefdf627af.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/pages/404-1e77c517c165fca8.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js" defer=""></script><style data-emotion="mantine ki47pp 1kzx756 n8pl39 f9w8pv ojrz4j 1uuuflr">.mantine-ki47pp{font-size:9.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-1kzx756{font-size:2.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-n8pl39{font-size:1.375rem;font-weight:500;}.mantine-f9w8pv{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}.mantine-ojrz4j{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-1uuuflr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:0rem;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-f9w8pv"><div class="mantine-Center-root mantine-ojrz4j" style="height:100%"><div class="mantine-Stack-root mantine-1uuuflr"><div class="mantine-ki47pp">404</div><div class="mantine-1kzx756">Page Not Found</div><div class="mantine-n8pl39">The page you are looking for doesn’t exist.</div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"afTF15k0tNJ2rEveq5WZR","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/500.html` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/500.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c7250373c9756530.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/pages/500-8c3654eb5b977ca1.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_buildManifest.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_ssgManifest.js" defer=""></script><style data-emotion="mantine ki47pp 1kzx756 n8pl39 f9w8pv ojrz4j 1uuuflr">.mantine-ki47pp{font-size:9.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-1kzx756{font-size:2.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-n8pl39{font-size:1.375rem;font-weight:500;}.mantine-f9w8pv{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}.mantine-ojrz4j{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-1uuuflr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:0rem;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-f9w8pv"><div class="mantine-Center-root mantine-ojrz4j" style="height:100%"><div class="mantine-Stack-root mantine-1uuuflr"><div class="mantine-ki47pp">500</div><div class="mantine-1kzx756">Internal Server Error</div><div class="mantine-n8pl39">The server encountered an error and counld not complete your request.</div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/500","query":{},"buildId":"fMfFQ47widM1tYI27opXD","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-fb2189cefdf627af.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/pages/500-8c3654eb5b977ca1.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js" defer=""></script><style data-emotion="mantine ki47pp 1kzx756 n8pl39 f9w8pv ojrz4j 1uuuflr">.mantine-ki47pp{font-size:9.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-1kzx756{font-size:2.375rem;font-weight:600;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;color:#0e2037;}.mantine-n8pl39{font-size:1.375rem;font-weight:500;}.mantine-f9w8pv{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}.mantine-ojrz4j{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-1uuuflr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:0rem;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-f9w8pv"><div class="mantine-Center-root mantine-ojrz4j" style="height:100%"><div class="mantine-Stack-root mantine-1uuuflr"><div class="mantine-ki47pp">500</div><div class="mantine-1kzx756">Internal Server Error</div><div class="mantine-n8pl39">The server encountered an error and counld not complete your request.</div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/500","query":{},"buildId":"afTF15k0tNJ2rEveq5WZR","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/657-2e4c261bfa28c304.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [657], {
+    [8], {
         8463: function(e, t, r) {
             "use strict";
             r.d(t, {
                 YF: function() {
                     return p
                 },
                 x7: function() {
@@ -26903,40 +26903,14 @@
             }
             r.d(t, {
                 Z: function() {
                     return n
                 }
             })
         },
-        9204: function(e, t, r) {
-            "use strict";
-            r.d(t, {
-                IZ: function() {
-                    return d
-                }
-            });
-            var n = r(6154);
-            let {
-                Axios: o,
-                AxiosError: a,
-                CanceledError: i,
-                isCancel: s,
-                CancelToken: c,
-                VERSION: l,
-                all: u,
-                Cancel: p,
-                isAxiosError: d,
-                spread: f,
-                toFormData: m,
-                AxiosHeaders: h,
-                HttpStatusCode: b,
-                formToJSON: v,
-                mergeConfig: g
-            } = n.Z
-        },
         6154: function(e, t, r) {
             "use strict";
             let n;
 
             function o(e, t) {
                 return function() {
                     return e.apply(t, arguments)
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-8f3afe3801b5eb58.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,59 +1,59 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [405], {
         8312: function(e, n, t) {
             (window.__NEXT_P = window.__NEXT_P || []).push(["/", function() {
-                return t(9890)
+                return t(3812)
             }])
         },
-        9890: function(e, n, t) {
+        3812: function(e, n, t) {
             "use strict";
             t.r(n), t.d(n, {
                 default: function() {
-                    return nC
+                    return nO
                 }
             });
-            var r, i, s, l, o, a, c, u, d = t(5893),
+            var r, i, l, s, o, a, c, u, d = t(5893),
                 p = t(4523),
                 m = t(9737),
-                h = t(9008),
-                x = t.n(h),
+                x = t(9008),
+                h = t.n(x),
                 f = t(3356),
                 g = t(5117),
                 j = t(9985),
                 v = t(2445),
                 y = t(7294),
                 b = t(741),
                 O = t(7789),
                 w = t(1232),
                 C = t(7564),
                 T = t(8818),
                 E = t(2185),
-                I = t(1163);
+                S = t(1163);
 
-            function S(e) {
-                let n = (0, I.useRouter)(),
+            function I(e) {
+                let n = (0, S.useRouter)(),
                     {
                         ref: t
                     } = (0, E.h)(),
                     {
                         avatar: r,
                         buttons: i,
-                        tabs: s,
-                        activeTab: l,
+                        tabs: l,
+                        activeTab: s,
                         align: o,
                         children: a
                     } = e,
                     c = e => {
-                        let t = s.find(n => n.value === e);
+                        let t = l.find(n => n.value === e);
                         t && n.push(t.link)
                     },
-                    u = null != s ? (0, d.jsx)(b.m, {
-                        value: l,
-                        defaultValue: l,
+                    u = null != l ? (0, d.jsx)(b.m, {
+                        value: s,
+                        defaultValue: s,
                         onTabChange: c,
                         color: "violet-manual.3",
                         styles: e => ({
                             tab: {
                                 "&:hover": {
                                     backgroundColor: e.colors.gray[0],
                                     borderColor: e.colors.gray[5]
@@ -76,15 +76,15 @@
                             },
                             tabRightSection: {
                                 paddingLeft: "5px",
                                 marginBottom: "3px"
                             }
                         }),
                         children: (0, d.jsx)(b.m.List, {
-                            children: s.map(e => (0, d.jsx)(b.m.Tab, {
+                            children: l.map(e => (0, d.jsx)(b.m.Tab, {
                                 value: e.value,
                                 rightSection: void 0 !== e.badgeLabel && null !== e.badgeLabel ? (0, d.jsx)(O.C, {
                                     size: "sm",
                                     children: e.badgeLabel
                                 }) : null,
                                 children: e.label
                             }, e.value))
@@ -167,15 +167,15 @@
                     model: n,
                     children: t
                 } = e, r = (0, d.jsx)(g.x, {
                     size: "xxl",
                     fw: 500,
                     inline: !0,
                     children: n.name
-                }), i = (0, d.jsx)(S, {
+                }), i = (0, d.jsx)(I, {
                     avatar: (0, d.jsx)(j.q, {
                         src: n.avatar_url,
                         size: "70px",
                         radius: "0"
                     }),
                     align: "center",
                     children: r
@@ -188,26 +188,24 @@
                         children: (0, d.jsx)(v.W, {
                             className: "layout-container-inner",
                             children: t
                         })
                     })
                 })
             }
-            var F = t(6154),
-                R = t(4155);
-            let z = () => {
-                console.log(R.env);
+            var F = t(6154);
+            let R = () => {
                 let e = F.Z.create({
                     timeout: 3e3
                 });
                 return e
             };
-            var Z = t(2819),
-                P = t(8767),
-                B = function(e) {
+            var z = t(2819),
+                Z = t(8767),
+                P = function(e) {
                     return Object.freeze({
                         axiosInstance: e,
                         create: function(n) {
                             return e.post("/predictions", n, {
                                 headers: {
                                     accept: "application/json",
                                     "Content-Type": "application/json"
@@ -219,15 +217,15 @@
                         },
                         cancel: function(n) {
                             return e.post("/predictions/".concat(n, "/cancel"))
                         }
                     })
                 };
 
-            function A(e) {
+            function B(e) {
                 let {
                     failureReason: n,
                     logsArea: t
                 } = e;
                 return (0, d.jsxs)(C.K, {
                     children: [(0, d.jsx)(g.x, {
                         color: "red.6",
@@ -243,50 +241,50 @@
                                 default:
                                     return "ERROR".concat(e ? ": ".concat(e) : "")
                             }
                         }(n)
                     }), t]
                 })
             }
-            var H = t(966);
+            var A = t(966);
 
-            function M(e) {
+            function H(e) {
                 let {
                     status: n,
                     logsArea: t
                 } = e;
                 return (0, d.jsxs)(C.K, {
                     children: [(0, d.jsxs)(w.Z, {
                         children: [(0, d.jsx)(g.x, {
                             fw: 500,
                             children: n.charAt(0).toUpperCase() + n.slice(1)
-                        }), (0, d.jsx)(H.a, {
+                        }), (0, d.jsx)(A.a, {
                             color: "gray",
                             variant: "dots",
                             size: "sm"
                         })]
                     }), t]
                 })
             }
-            var W = t(825);
+            var M = t(825);
 
-            function K(e) {
+            function W(e) {
                 let {
                     title: n,
                     rightIcon: t,
                     children: r,
                     ...i
                 } = e;
-                return (0, d.jsxs)(W.Z, {
+                return (0, d.jsxs)(M.Z, {
                     withBorder: !0,
                     padding: "lg",
                     radius: "lg",
                     h: "fit-content",
                     ...i,
-                    children: [(0, d.jsx)(W.Z.Section, {
+                    children: [(0, d.jsx)(M.Z.Section, {
                         withBorder: !0,
                         inheritPadding: !0,
                         py: "sm",
                         children: (0, d.jsxs)(w.Z, {
                             position: "apart",
                             children: ["string" == typeof n ? (0, d.jsx)(g.x, {
                                 fz: "xl",
@@ -296,158 +294,158 @@
                         })
                     }), (0, d.jsx)(p.x, {
                         pt: "md",
                         children: r
                     })]
                 })
             }
-            var U = t(3523),
-                q = t(2870);
+            var K = t(3523),
+                U = t(2870);
 
-            function D() {
+            function q() {
                 return (0, d.jsxs)(C.K, {
                     align: "center",
                     justify: "center",
                     spacing: "lg",
                     py: "xl",
-                    children: [(0, d.jsx)(U.M, {
-                        children: (0, d.jsx)(q.E, {
+                    children: [(0, d.jsx)(K.M, {
+                        children: (0, d.jsx)(U.E, {
                             mx: "auto",
                             maw: "40%",
                             opacity: .3,
                             alt: "tungsten_logo",
                             src: "/tungsten_greyed_out_logo.png"
                         })
                     }), (0, d.jsx)(g.x, {
                         color: "gray.6",
                         fz: "md",
                         children: 'Click "Run" to see amazing results.'
                     })]
                 })
             }
-            var J = t(8104);
+            var D = t(8104);
 
-            function V(e) {
+            function J(e) {
                 let {
                     name: n,
                     description: t,
                     required: r
-                } = e, i = (0, J.rZ)(), s = i.fn.variant({
+                } = e, i = (0, D.rZ)(), l = i.fn.variant({
                     variant: "filled",
                     color: "red"
                 }).background;
                 return (0, d.jsxs)(C.K, {
                     spacing: "xxs",
                     mb: "xs",
                     children: [(0, d.jsxs)(p.x, {
                         children: [(0, d.jsxs)(g.x, {
                             fw: 500,
                             fz: "md",
                             span: !0,
                             children: [n, " "]
                         }), r && (0, d.jsx)(g.x, {
                             span: !0,
-                            color: s,
+                            color: l,
                             children: "*"
                         })]
                     }), t ? (0, d.jsx)(g.x, {
                         color: "gray.7",
                         fz: "sm",
                         children: t
                     }) : void 0]
                 })
             }
-            var Y = t(983),
-                G = t(2679),
-                X = t(7297),
-                Q = t(7841),
-                $ = t(2276),
-                ee = t(7311),
-                en = t(2015);
+            var V = t(983),
+                Y = t(2679),
+                G = t(7297),
+                X = t(7841),
+                Q = t(2276),
+                $ = t(7311),
+                ee = t(2015);
+
+            function en() {
+                let e = (0, G.Z)(["\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: center;\n  height: 100px;\n  width: 100%;\n  background: transparent;\n  gap: 2rem;\n"]);
+                return en = function() {
+                    return e
+                }, e
+            }
 
             function et() {
-                let e = (0, X.Z)(["\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: center;\n  height: 100px;\n  width: 100%;\n  background: transparent;\n  gap: 2rem;\n"]);
+                let e = (0, G.Z)(["\n  width: 100%;\n  height: 90px;\n"]);
                 return et = function() {
                     return e
                 }, e
             }
 
             function er() {
-                let e = (0, X.Z)(["\n  width: 100%;\n  height: 90px;\n"]);
+                let e = (0, G.Z)(["\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 60px;\n  height: 60px;\n  background: #e9e9e9;\n  border: 1px black;\n  outline: none;\n  cursor: pointer;\n  padding-bottom: 3px;\n  &:hover {\n    background: #ddd;\n  }\n"]);
                 return er = function() {
                     return e
                 }, e
             }
-
-            function ei() {
-                let e = (0, X.Z)(["\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 60px;\n  height: 60px;\n  background: #e9e9e9;\n  border: 1px black;\n  outline: none;\n  cursor: pointer;\n  padding-bottom: 3px;\n  &:hover {\n    background: #ddd;\n  }\n"]);
-                return ei = function() {
-                    return e
-                }, e
-            }
-            let es = en.ZP.div(et()),
-                el = en.ZP.div(er());
-            en.ZP.button(ei());
-            var eo = function(e) {
+            let ei = ee.ZP.div(en()),
+                el = ee.ZP.div(et());
+            ee.ZP.button(er());
+            var es = function(e) {
                     let {
                         src: n
-                    } = e, r = (0, y.useId)(), [i, s] = (0, y.useState)(!1), [l, o] = (0, y.useState)(), a = !0;
+                    } = e, r = (0, y.useId)(), [i, l] = (0, y.useState)(!1), [s, o] = (0, y.useState)(), a = !0;
                     (0, y.useEffect)(() => {
                         if (a) {
                             let e = async () => {
                                 let e = (await t.e(33).then(t.t.bind(t, 1796, 23))).default,
                                     i = document.getElementById("waveform".concat(r)),
-                                    l = e.create({
+                                    s = e.create({
                                         barWidth: 3,
                                         barRadius: 3,
                                         barGap: 2,
                                         barMinHeight: 1,
                                         cursorWidth: 1,
                                         container: i,
                                         backend: "WebAudio",
                                         height: 80,
                                         progressColor: "#black",
                                         responsive: !0,
                                         waveColor: "#C4C4C4",
                                         cursorColor: "transparent"
                                     });
-                                o(l), l.load(n), l.on("finish", () => {
-                                    s(!1)
+                                o(s), s.load(n), s.on("finish", () => {
+                                    l(!1)
                                 })
                             };
                             e(), a = !1
                         }
                     }, []);
                     let c = e => {
-                        s(!i), e && e.playPause()
+                        l(!i), e && e.playPause()
                     };
                     return (0, d.jsx)(p.x, {
                         sx: {
                             maxWidth: "90%"
                         },
                         children: (0, d.jsx)(p.x, {
                             style: {
                                 padding: "0px",
                                 margin: "0px"
                             },
-                            children: (0, d.jsxs)(es, {
+                            children: (0, d.jsxs)(ei, {
                                 style: {
                                     padding: "0px",
                                     margin: "0px",
                                     height: "90px"
                                 },
-                                children: [(0, d.jsx)(Q.z, {
+                                children: [(0, d.jsx)(X.z, {
                                     sx: e => ({
                                         border: "none",
                                         borderRadius: e.radius.sm,
                                         width: "120px"
                                     }),
                                     variant: "contained",
-                                    leftIcon: i ? (0, d.jsx)($.Z, {}) : (0, d.jsx)(ee.Z, {}),
-                                    onClick: e => c(l),
+                                    leftIcon: i ? (0, d.jsx)(Q.Z, {}) : (0, d.jsx)($.Z, {}),
+                                    onClick: e => c(s),
                                     children: i ? "Pause" : "Play"
                                 }), (0, d.jsx)(el, {
                                     id: "waveform".concat(r),
                                     style: {
                                         padding: "0px",
                                         margin: "0px",
                                         height: "80px"
@@ -460,67 +458,67 @@
                                         margin: "0px"
                                     }
                                 })]
                             })
                         })
                     })
                 },
-                ea = t(335);
+                eo = t(335);
 
-            function ec(e) {
+            function ea(e) {
                 let {
                     src: n
                 } = e;
-                return (0, d.jsx)(Q.z, {
+                return (0, d.jsx)(X.z, {
                     component: "a",
                     href: n,
                     target: "_blank",
                     variant: "default",
-                    leftIcon: (0, d.jsx)(ea.Z, {
+                    leftIcon: (0, d.jsx)(eo.Z, {
                         size: "1rem"
                     }),
                     children: "Download file"
                 })
             }
-            var eu = t(5215);
+            var ec = t(5215);
             t(1717);
-            var ed = function(e) {
+            var eu = function(e) {
                 let {
                     src: n,
                     mimeType: t,
                     autoplay: r = !1,
                     controls: i = !0,
-                    responsive: s = !0,
-                    fluid: l = !0
+                    responsive: l = !0,
+                    fluid: s = !0
                 } = e, o = (0, y.useRef)(null), a = (0, y.useRef)(null), c = (e, n) => {
                     n.current = e
                 };
                 return (0, y.useEffect)(() => {
                     let e = {
                         autoplay: r,
                         controls: i,
-                        responsive: s,
-                        fluid: l,
+                        responsive: l,
+                        fluid: s,
                         sources: [{
                             src: n,
                             type: t
                         }]
                     };
                     if (a.current) {
                         let n = a.current;
                         n.autoplay(e.autoplay), n.src(e.sources)
                     } else {
                         var u;
                         let n = document.createElement("video-js");
                         n.classList.add("vjs-big-play-centered"), null === (u = o.current) || void 0 === u || u.appendChild(n);
-                        let t = a.current = (0, eu.Z)(n, e, () => {
+                        let t = a.current = (0, ec.Z)(n, e, () => {
                             c && c(t, a)
                         })
                     }
-                }, [n, t, r, i, s, l, o]), (0, y.useEffect)(() => {
+                }, [n, t, r, i, l, s, o]), (0, y.useEffect)(() => {
                     let e = a.current;
                     return () => {
                         e && !e.isDisposed() && (e.dispose(), a.current = null)
                     }
                 }, [a]), (0, d.jsx)(N.k, {
                     direction: "column",
                     sx: {
@@ -532,825 +530,825 @@
                         children: (0, d.jsx)("div", {
                             ref: o,
                             style: {}
                         })
                     })
                 })
             };
-            let ep = e => {
+            let ed = e => {
                     if ("string" != typeof e) return e.type;
-                    let n = (0, Y.lookup)(e);
+                    let n = (0, V.lookup)(e);
                     return n || "application/octet-stream"
                 },
-                em = (0, y.forwardRef)((e, n) => {
+                ep = (0, y.forwardRef)((e, n) => {
                     let t;
                     let {
                         file: r,
                         filetype: i
-                    } = e, [s, l] = (0, y.useState)("string" == typeof r ? r : URL.createObjectURL(r)), o = ep(r), a = (0, d.jsx)(p.x, {});
+                    } = e, [l, s] = (0, y.useState)("string" == typeof r ? r : URL.createObjectURL(r)), o = ed(r), a = (0, d.jsx)(p.x, {});
                     switch ((0, y.useEffect)(() => {
-                            l("string" == typeof r ? r : URL.createObjectURL(r))
+                            s("string" == typeof r ? r : URL.createObjectURL(r))
                         }, [r]), i) {
                         case "image":
-                            t = s ? (0, d.jsx)(G.LazyLoadImage, {
-                                src: s,
+                            t = l ? (0, d.jsx)(Y.LazyLoadImage, {
+                                src: l,
                                 style: {
                                     maxWidth: "100%",
                                     maxHeight: "100%"
                                 },
                                 alt: i
                             }) : a;
                             break;
                         case "video":
-                            t = s ? (0, d.jsx)(ed, {
-                                src: s,
+                            t = l ? (0, d.jsx)(eu, {
+                                src: l,
                                 mimeType: o
                             }) : a;
                             break;
                         case "audio":
-                            t = s ? (0, d.jsx)(eo, {
-                                src: s
+                            t = l ? (0, d.jsx)(es, {
+                                src: l
                             }) : a;
                             break;
                         default:
-                            t = s ? (0, d.jsx)(ec, {
-                                src: s
+                            t = l ? (0, d.jsx)(ea, {
+                                src: l
                             }) : a
                     }
                     return (0, d.jsx)(p.x, {
                         maw: "100%",
                         mah: "100%",
                         ref: n,
                         children: t
                     })
                 });
 
-            function eh(e, n) {
-                if (n) return s.FILE;
+            function em(e, n) {
+                if (n) return l.FILE;
                 if (e.choices && e.type && ["string", "number", "integer"].includes(e.type)) {
-                    if ("string" === e.type) return s.STR_CHOICE;
-                    if ("integer" === e.type) return s.INT_CHOICE;
-                    if ("number" === e.type) return s.FLOAT_CHOICE
+                    if ("string" === e.type) return l.STR_CHOICE;
+                    if ("integer" === e.type) return l.INT_CHOICE;
+                    if ("number" === e.type) return l.FLOAT_CHOICE
                 }
-                return "integer" === e.type ? void 0 !== e.minimum || void 0 !== e.maximum ? s.CONINT : s.INT : "number" === e.type ? void 0 !== e.minimum || void 0 !== e.maximum ? s.CONFLOAT : s.FLOAT : "boolean" === e.type ? s.BOOL : void 0 !== e.min_length || void 0 !== e.max_length ? s.CONSTR : s.STR
+                return "integer" === e.type ? void 0 !== e.minimum || void 0 !== e.maximum ? l.CONINT : l.INT : "number" === e.type ? void 0 !== e.minimum || void 0 !== e.maximum ? l.CONFLOAT : l.FLOAT : "boolean" === e.type ? l.BOOL : void 0 !== e.min_length || void 0 !== e.max_length ? l.CONSTR : l.STR
             }
-            em.defaultProps = {
+            ep.defaultProps = {
                 filetype: "binary"
-            }, em.displayName = "FileView", (r = s || (s = {}))[r.FILE = 0] = "FILE", r[r.STR = 1] = "STR", r[r.CONSTR = 2] = "CONSTR", r[r.INT = 3] = "INT", r[r.CONINT = 4] = "CONINT", r[r.FLOAT = 5] = "FLOAT", r[r.CONFLOAT = 6] = "CONFLOAT", r[r.BOOL = 7] = "BOOL", r[r.STR_CHOICE = 8] = "STR_CHOICE", r[r.INT_CHOICE = 9] = "INT_CHOICE", r[r.FLOAT_CHOICE = 10] = "FLOAT_CHOICE", (i = l || (l = {}))[i.FILE = 0] = "FILE", i[i.FILE_LIST = 1] = "FILE_LIST", i[i.FILE_DICT = 2] = "FILE_DICT", i[i.STR = 3] = "STR", i[i.NUMBER = 4] = "NUMBER", i[i.BOOL = 5] = "BOOL", i[i.JSON = 6] = "JSON";
+            }, ep.displayName = "FileView", (r = l || (l = {}))[r.FILE = 0] = "FILE", r[r.STR = 1] = "STR", r[r.CONSTR = 2] = "CONSTR", r[r.INT = 3] = "INT", r[r.CONINT = 4] = "CONINT", r[r.FLOAT = 5] = "FLOAT", r[r.CONFLOAT = 6] = "CONFLOAT", r[r.BOOL = 7] = "BOOL", r[r.STR_CHOICE = 8] = "STR_CHOICE", r[r.INT_CHOICE = 9] = "INT_CHOICE", r[r.FLOAT_CHOICE = 10] = "FLOAT_CHOICE", (i = s || (s = {}))[i.FILE = 0] = "FILE", i[i.FILE_LIST = 1] = "FILE_LIST", i[i.FILE_DICT = 2] = "FILE_DICT", i[i.STR = 3] = "STR", i[i.NUMBER = 4] = "NUMBER", i[i.BOOL = 5] = "BOOL", i[i.JSON = 6] = "JSON";
             var ex = t(2328),
-                ef = t(665),
-                eg = t(7577),
-                ej = t(5887),
-                ev = t(8393),
-                ey = t(9834),
-                eb = t(8198),
-                eO = t(3625);
+                eh = t(665),
+                ef = t(7577),
+                eg = t(5887),
+                ej = t(8393),
+                ev = t(9834),
+                ey = t(8198),
+                eb = t(3625);
 
-            function ew(e) {
+            function eO(e) {
                 let {
                     value: n,
                     iconSize: t,
                     ...r
                 } = e;
-                return (0, d.jsx)(eg.a, {
+                return (0, d.jsx)(ef.a, {
                     opacity: 0,
                     sx: {
                         pointerEvents: "none"
                     },
                     ...r,
                     children: (0, d.jsx)(w.Z, {
                         position: "right",
                         align: "center",
-                        children: (0, d.jsx)(ej.q, {
+                        children: (0, d.jsx)(eg.q, {
                             value: "string" == typeof n ? n : n.toString(),
                             timeout: 2e3,
                             children: e => {
                                 let {
                                     copied: n,
                                     copy: r
                                 } = e;
-                                return (0, d.jsx)(ev.u, {
+                                return (0, d.jsx)(ej.u, {
                                     label: n ? "Copied" : "Copy",
                                     withArrow: !0,
                                     position: "bottom",
-                                    children: (0, d.jsx)(ey.A, {
+                                    children: (0, d.jsx)(ev.A, {
                                         variant: "light",
                                         color: n ? "button-blue" : "gray",
                                         onClick: r,
                                         sx: {
                                             pointerEvents: "all"
                                         },
-                                        children: n ? (0, d.jsx)(eb.Z, {
+                                        children: n ? (0, d.jsx)(ey.Z, {
                                             size: t
-                                        }) : (0, d.jsx)(eO.Z, {
+                                        }) : (0, d.jsx)(eb.Z, {
                                             size: t
                                         })
                                     })
                                 })
                             }
                         })
                     })
                 })
             }
-            ew.defaultProps = {
+            eO.defaultProps = {
                 iconSize: "1rem"
             };
-            var eC = t(6817),
-                eT = t(6768),
-                eE = (0, eC.k)((e, n) => {
+            var ew = t(6817),
+                eC = t(6768),
+                eT = (0, ew.k)((e, n) => {
                     let {
                         color: t
                     } = n, r = t || ("dark" === e.colorScheme ? "dark" : "gray"), i = e.fn.variant({
                         color: r,
                         variant: "light"
                     });
                     return {
                         root: {
                             ...e.fn.fontStyles(),
                             lineHeight: e.lineHeight,
-                            padding: "".concat((0, eT.h)(2), " calc(").concat(e.spacing.xs, " / 2)"),
+                            padding: "".concat((0, eC.h)(2), " calc(").concat(e.spacing.xs, " / 2)"),
                             borderRadius: e.radius.sm,
                             color: "dark" === e.colorScheme ? "dark" === r ? e.colors.dark[0] : e.white : e.colors.dark[7],
                             backgroundColor: "dark" === e.colorScheme && "dark" === r ? e.colors.dark[5] : i.background,
                             fontFamily: e.fontFamilyMonospace,
                             fontSize: e.fontSizes.xs
                         },
                         block: {
                             padding: e.spacing.xs,
                             margin: 0,
                             whiteSpace: "pre-wrap",
                             wordBreak: "break-all"
                         }
                     }
                 });
-            let eI = {
+            let eE = {
                     fz: "sm"
                 },
                 eS = (0, y.forwardRef)((e, n) => {
                     let {
                         className: t,
                         children: r,
                         color: i,
-                        unstyled: s,
-                        variant: l,
+                        unstyled: l,
+                        variant: s,
                         mono: o,
                         ff: a,
                         noCopy: c,
                         ...u
-                    } = (0, J.N4)("Code", eI, e), {
+                    } = (0, D.N4)("Code", eE, e), {
                         classes: m,
-                        cx: h
-                    } = eE({
+                        cx: x
+                    } = eT({
                         color: i
                     }, {
                         name: "Code",
-                        unstyled: s,
-                        variant: l
-                    }), x = (0, J.rZ)(), {
+                        unstyled: l,
+                        variant: s
+                    }), h = (0, D.rZ)(), {
                         ref: f,
                         x: g,
                         y: j
                     } = (0, ex.i)({
                         resetOnExit: !0
-                    }), v = (0, ef.Y)(f, n);
+                    }), v = (0, eh.Y)(f, n);
                     return (0, d.jsx)(p.x, {
-                        ff: null != a ? a : o ? x.fontFamilyMonospace : x.fontFamily,
-                        className: h(m.root, m.block, t),
+                        ff: null != a ? a : o ? h.fontFamilyMonospace : h.fontFamily,
+                        className: x(m.root, m.block, t),
                         ref: v,
                         ...u,
                         children: (0, d.jsxs)(p.x, {
                             pos: "relative",
                             children: [null != r && "" !== r ? r : (0, d.jsx)(p.x, {
                                 children: "\xa0"
-                            }), !0 !== c && (0 !== g || 0 !== j) && null != r && "" !== r && (0, d.jsx)(ew, {
+                            }), !0 !== c && (0 !== g || 0 !== j) && null != r && "" !== r && (0, d.jsx)(eO, {
                                 value: "string" == typeof r ? r : r.toString(),
                                 iconSize: "1rem"
                             })]
                         })
                     })
                 });
 
-            function eN(e) {
+            function eI(e) {
                 let {
                     fieldName: n,
                     propObj: t,
                     filetype: r,
                     itemFiletype: i,
-                    value: s
+                    value: l
                 } = e, o = function(e, n, t) {
                     let r = Object.keys(e),
                         i = "array" === e.type,
-                        s = "object" === e.type && r.includes("additionalProperties");
-                    return n ? l.FILE : i && t ? l.FILE_LIST : s && t ? l.FILE_DICT : "integer" === e.type || "number" === e.type ? l.NUMBER : "boolean" === e.type ? l.BOOL : "string" === e.type ? l.STR : l.JSON
+                        l = "object" === e.type && r.includes("additionalProperties");
+                    return n ? s.FILE : i && t ? s.FILE_LIST : l && t ? s.FILE_DICT : "integer" === e.type || "number" === e.type ? s.NUMBER : "boolean" === e.type ? s.BOOL : "string" === e.type ? s.STR : s.JSON
                 }(t, r, i);
                 switch (o) {
-                    case l.FILE:
-                        return (0, d.jsx)(em, {
-                            file: s,
+                    case s.FILE:
+                        return (0, d.jsx)(ep, {
+                            file: l,
                             filetype: r
                         });
-                    case l.FILE_LIST:
+                    case s.FILE_LIST:
                         return (0, d.jsx)(C.K, {
                             spacing: "xxs",
-                            children: s.map((e, r) => (0, d.jsx)(eN, {
+                            children: l.map((e, r) => (0, d.jsx)(eI, {
                                 fieldName: "".concat(n, "-").concat(r.toString()),
                                 propObj: t.items,
                                 filetype: i,
                                 value: e
                             }, "".concat(n, "-").concat(r.toString())))
                         });
-                    case l.FILE_DICT:
+                    case s.FILE_DICT:
                         return (0, d.jsx)(C.K, {
                             spacing: "xxs",
-                            children: Object.keys(s).map(e => (0, d.jsxs)("div", {
-                                children: [(0, d.jsx)(V, {
+                            children: Object.keys(l).map(e => (0, d.jsxs)("div", {
+                                children: [(0, d.jsx)(J, {
                                     description: e
-                                }, e), (0, d.jsx)(eN, {
+                                }, e), (0, d.jsx)(eI, {
                                     fieldName: "".concat(n, "-").concat(e),
                                     propObj: t.additionalProperties,
                                     filetype: i,
-                                    value: s[e]
+                                    value: l[e]
                                 })]
                             }, "".concat(n, "-").concat(e)))
                         });
-                    case l.STR:
+                    case s.STR:
                         return (0, d.jsx)(eS, {
-                            children: s
+                            children: l
                         });
-                    case l.BOOL:
-                    case l.NUMBER:
+                    case s.BOOL:
+                    case s.NUMBER:
                         return (0, d.jsx)(eS, {
-                            children: s.toString()
+                            children: l.toString()
                         });
-                    case l.JSON:
+                    case s.JSON:
                         return (0, d.jsx)(eS, {
-                            children: JSON.stringify(s, void 0, 2)
+                            children: JSON.stringify(l, void 0, 2)
                         });
                     default:
                         throw TypeError("Unkown output field type ".concat(o, " "))
                 }
             }
 
-            function ek(e) {
+            function eN(e) {
                 let {
                     schema: n,
                     filetypes: t,
                     values: r,
                     spacing: i
-                } = e, s = [];
+                } = e, l = [];
                 return Object.keys(n.properties).forEach(e => {
-                    s.push({
+                    l.push({
                         name: e,
                         component: function(e) {
                             let i = n.properties[e],
-                                s = t[e];
-                            return (0, d.jsx)(eN, {
+                                l = t[e];
+                            return (0, d.jsx)(eI, {
                                 fieldName: e,
                                 propObj: i,
-                                filetype: s,
+                                filetype: l,
                                 itemFiletype: t["".concat(e, ".$item")],
                                 value: r[e]
                             })
                         }(e)
                     })
                 }), (0, d.jsx)(C.K, {
                     fz: "md",
                     spacing: i,
-                    children: s.map(e => (0, d.jsxs)("div", {
-                        children: [(0, d.jsx)(V, {
+                    children: l.map(e => (0, d.jsxs)("div", {
+                        children: [(0, d.jsx)(J, {
                             name: e.name
                         }), e.component]
                     }, "output-field-".concat(e.name)))
                 })
             }
-            eS.displayName = "CodeBlockWithLinebreak", ek.defaultProps = {
+            eS.displayName = "CodeBlockWithLinebreak", eN.defaultProps = {
                 spacing: "md"
             };
-            var eL = t(3723);
+            var ek = t(3723);
 
-            function e_(e) {
+            function eL(e) {
                 let {
                     children: n,
                     autoScroll: t,
                     fz: r,
                     h: i
-                } = e, s = (0, y.useRef)(null), {
-                    ref: l,
+                } = e, l = (0, y.useRef)(null), {
+                    ref: s,
                     width: o,
                     height: a
                 } = (0, E.h)(), {
                     ref: c,
                     x: u,
                     y: m
                 } = (0, ex.i)({
                     resetOnExit: !0
-                }), h = (0, ef.Y)(l, c), x = !!t && (0 === u || 0 === m), f = e => {
+                }), x = (0, eh.Y)(s, c), h = !!t && (0 === u || 0 === m), f = e => {
                     var n;
-                    null == s || null === (n = s.current) || void 0 === n || n.scrollTo({
-                        top: s.current.scrollHeight,
+                    null == l || null === (n = l.current) || void 0 === n || n.scrollTo({
+                        top: l.current.scrollHeight,
                         behavior: e
                     })
                 };
                 return (0, y.useEffect)(() => {
-                    t && x && f(t)
-                }, [x, t, n]), (0, d.jsxs)(p.x, {
+                    t && h && f(t)
+                }, [h, t, n]), (0, d.jsxs)(p.x, {
                     pos: "relative",
-                    ref: h,
-                    children: [(0, d.jsx)(eL.x, {
-                        viewportRef: s,
+                    ref: x,
+                    children: [(0, d.jsx)(ek.x, {
+                        viewportRef: l,
                         h: i,
                         children: (0, d.jsx)(eS, {
                             fz: r,
                             miw: o,
                             mih: a,
                             mono: !0,
                             noCopy: !0,
                             children: n
                         })
-                    }), (0 !== u || 0 !== m) && (0, d.jsx)(ew, {
+                    }), (0 !== u || 0 !== m) && (0, d.jsx)(eO, {
                         p: ".3rem",
                         value: null != n ? n : ""
                     })]
                 })
             }
 
-            function eF(e) {
+            function e_(e) {
                 let {
                     mode: n,
                     output: t,
                     demoOutput: r,
                     demoOutputSchema: i,
-                    demoOutputFiletypes: s,
-                    logs: l
-                } = e, o = (0, d.jsx)(ek, {
+                    demoOutputFiletypes: l,
+                    logs: s
+                } = e, o = (0, d.jsx)(eN, {
                     schema: i,
-                    filetypes: s,
+                    filetypes: l,
                     values: r
                 }), a = (0, d.jsx)(eS, {
                     fz: "xs",
                     mono: !0,
                     children: JSON.stringify(t, null, 2)
-                }), c = (0, d.jsx)(e_, {
-                    children: null != l ? l : ""
+                }), c = (0, d.jsx)(eL, {
+                    children: null != s ? s : ""
                 });
                 return (0, d.jsxs)(d.Fragment, {
                     children: ["preview" === n && o, "raw" === n && a, "logs" === n && c]
                 })
             }
-            e_.defaultProps = {
+            eL.defaultProps = {
                 fz: "xs",
                 h: "30vh",
                 children: ""
             };
-            var eR = t(3819),
-                ez = t(5158),
-                eZ = t(2972),
-                eP = t(7080);
+            var eF = t(3819),
+                eR = t(5158),
+                ez = t(2972),
+                eZ = t(7080);
 
-            function eB(e) {
+            function eP(e) {
                 let {
                     icon: n,
                     label: t
                 } = e;
-                return (0, d.jsxs)(U.M, {
+                return (0, d.jsxs)(K.M, {
                     children: [n, (0, d.jsx)(p.x, {
                         ml: 10,
                         children: t
                     })]
                 })
             }
 
-            function eA(e) {
+            function eB(e) {
                 let {
                     mode: n,
                     onChange: t,
                     w: r,
                     iconSize: i,
-                    ...s
-                } = e, l = {
+                    ...l
+                } = e, s = {
                     size: void 0 === i ? "1rem" : i
                 };
-                return (0, d.jsx)(eR.s, {
+                return (0, d.jsx)(eF.s, {
                     value: n,
                     onChange: t,
                     w: null != r ? r : "100%",
                     data: [{
-                        label: (0, d.jsx)(eB, {
-                            icon: (0, d.jsx)(ez.Z, {
-                                ...l
+                        label: (0, d.jsx)(eP, {
+                            icon: (0, d.jsx)(eR.Z, {
+                                ...s
                             }),
                             label: "Preview"
                         }),
                         value: "preview"
                     }, {
-                        label: (0, d.jsx)(eB, {
-                            icon: (0, d.jsx)(eZ.Z, {
-                                ...l
+                        label: (0, d.jsx)(eP, {
+                            icon: (0, d.jsx)(ez.Z, {
+                                ...s
                             }),
                             label: "Raw"
                         }),
                         value: "raw"
                     }, {
-                        label: (0, d.jsx)(eB, {
-                            icon: (0, d.jsx)(eP.Z, {
-                                ...l
+                        label: (0, d.jsx)(eP, {
+                            icon: (0, d.jsx)(eZ.Z, {
+                                ...s
                             }),
                             label: "Logs"
                         }),
                         value: "logs"
                     }],
-                    ...s
+                    ...l
                 })
             }
-            var eH = t(930),
-                eM = t(2615),
-                eW = t(4796),
-                eK = t(2675),
-                eU = t(8431),
-                eq = t(1885),
-                eD = t(1500),
-                eJ = t(6261),
-                eV = t(971),
-                eY = t(4151),
-                eG = t(3540),
-                eX = t(5851),
-                eQ = t(7339),
-                e$ = t(8044),
-                e0 = t(5204),
-                e1 = t(6862),
-                e5 = t(904),
-                e7 = t(7283);
+            var eA = t(930),
+                eH = t(2615),
+                eM = t(4796),
+                eW = t(2675),
+                eK = t(8431),
+                eU = t(1885),
+                eq = t(1500),
+                eD = t(6261),
+                eJ = t(971),
+                eV = t(4151),
+                eY = t(3540),
+                eG = t(5851),
+                eX = t(7339),
+                eQ = t(8044),
+                e$ = t(5204),
+                e0 = t(6862),
+                e1 = t(904),
+                e5 = t(7283);
             let e3 = {
                 iconSize: "1.1rem",
                 textProps: {
                     fz: "md"
                 }
             };
 
-            function e8(e) {
+            function e7(e) {
                 let n;
                 let {
                     wrapperProps: t,
                     value: r,
                     defaultValue: i,
-                    filetype: s,
-                    onChange: l,
+                    filetype: l,
+                    onChange: s,
                     textProps: o,
                     maxsize: a,
                     iconSize: c
-                } = (0, eJ.k)("DropzoneInput", e3, e), [u, m] = (0, eX.C)({
+                } = (0, eD.k)("DropzoneInput", e3, e), [u, m] = (0, eG.C)({
                     value: r,
-                    onChange: l,
+                    onChange: s,
                     finalValue: null
-                }), h = (0, J.rZ)();
-                return i && m(i), (0, d.jsx)(eY.I.Wrapper, {
+                }), x = (0, D.rZ)();
+                return i && m(i), (0, d.jsx)(eV.I.Wrapper, {
                     ...t,
                     children: (0, d.jsxs)(C.K, {
                         spacing: "xs",
                         children: [u ? function(e) {
-                            let n = (0, d.jsx)(em, {
+                            let n = (0, d.jsx)(ep, {
                                     file: e,
-                                    filetype: s
+                                    filetype: l
                                 }),
                                 t = typeof e !== i ? (0, d.jsxs)(w.Z, {
                                     maw: "100%",
                                     spacing: "xs",
                                     children: [(0, d.jsx)(g.x, {
                                         fz: "xs",
                                         color: "gray.7",
                                         children: "string" == typeof e ? decodeURI(e.split("/").pop()) : "".concat(e.name, " (").concat(function(e) {
                                             let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 2;
                                             if (!+e) return "0 Bytes";
                                             let t = Math.floor(Math.log(e) / Math.log(1024));
                                             return "".concat(parseFloat((e / Math.pow(1024, t)).toFixed(n < 0 ? 0 : n)), " ").concat(["Bytes", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB"][t])
                                         }(e.size), ")")
-                                    }), (0, d.jsx)(eV.P, {
+                                    }), (0, d.jsx)(eJ.P, {
                                         title: "Delete file",
                                         color: "gray.7",
                                         onClick: () => m(null)
                                     })]
                                 }) : void 0;
                             return (0, d.jsxs)(C.K, {
                                 spacing: "xs",
                                 maw: "100%",
-                                children: ["image" === s ? (0, d.jsx)(p.x, {
+                                children: ["image" === l ? (0, d.jsx)(p.x, {
                                     maw: "50%",
                                     children: n
                                 }) : n, t]
                             })
-                        }(u) : void 0, (0, d.jsx)(eG.fh, {
+                        }(u) : void 0, (0, d.jsx)(eY.fh, {
                             onDrop: e => {
-                                e.length > 0 && void 0 !== l && (m(e[0]), l(e[0]))
+                                e.length > 0 && void 0 !== s && (m(e[0]), s(e[0]))
                             },
                             maxSize: a,
                             accept: function() {
-                                if (["audio", "video", "image"].includes(s)) {
+                                if (["audio", "video", "image"].includes(l)) {
                                     let e = {};
-                                    for (let [n, t] of Object.entries(Y.extensions)) n.startsWith(s) && (e[n] = t.map(e => ".".concat(e)));
+                                    for (let [n, t] of Object.entries(V.extensions)) n.startsWith(l) && (e[n] = t.map(e => ".".concat(e)));
                                     return e
                                 }
                             }(),
                             maxFiles: 1,
                             children: (0, d.jsxs)(w.Z, {
                                 position: "center",
                                 spacing: "md",
                                 style: {
                                     pointerEvents: "none"
                                 },
-                                children: [(0, d.jsx)(eG.fh.Accept, {
-                                    children: (0, d.jsx)(e5.Z, {
-                                        color: h.colors[h.primaryColor][5],
+                                children: [(0, d.jsx)(eY.fh.Accept, {
+                                    children: (0, d.jsx)(e1.Z, {
+                                        color: x.colors[x.primaryColor][5],
                                         size: c
                                     })
-                                }), (0, d.jsx)(eG.fh.Reject, {
-                                    children: (0, d.jsx)(e7.Z, {
-                                        color: h.colors.red[6],
+                                }), (0, d.jsx)(eY.fh.Reject, {
+                                    children: (0, d.jsx)(e5.Z, {
+                                        color: x.colors.red[6],
                                         size: c
                                     })
-                                }), (0, d.jsx)(eG.fh.Idle, {
-                                    children: (n = "image" === s ? eQ.Z : "video" === s ? e$.Z : "audio" === s ? e0.Z : e1.Z, (0, d.jsx)(n, {
+                                }), (0, d.jsx)(eY.fh.Idle, {
+                                    children: (n = "image" === l ? eX.Z : "video" === l ? eQ.Z : "audio" === l ? e$.Z : e0.Z, (0, d.jsx)(n, {
                                         size: c
                                     }))
                                 }), (0, d.jsxs)(g.x, {
                                     inline: !0,
                                     ...o,
-                                    children: ["Drag ", s, " file here or click to select"]
+                                    children: ["Drag ", l, " file here or click to select"]
                                 })]
                             })
                         })]
                     })
                 })
             }
-            var e2 = t(6801),
-                e4 = t(806),
-                e9 = t(4419);
-            e9.ZP.registerCustom({
+            var e8 = t(6801),
+                e2 = t(806),
+                e4 = t(4419);
+            e4.ZP.registerCustom({
                 isApplicable: e => e instanceof File,
                 serialize: e => "null",
                 deserialize: e => null
             }, "decimal.js");
             let {
                 stringify: e6
-            } = e9.ZP, {
-                parse: ne
-            } = e9.ZP, nn = "This field is required.", [nt, nr, ni] = (0, e2.W)(), ns = e => {
+            } = e4.ZP, {
+                parse: e9
+            } = e4.ZP, ne = "This field is required.", [nn, nt, nr] = (0, e8.W)(), ni = e => {
                 let {
                     schema: n,
                     filetypes: t,
                     initialValues: r
-                } = e, i = Object.keys(n.properties), l = Object.fromEntries(i.map(e => [e, r && r[e] ? r[e] : function(e) {
+                } = e, i = Object.keys(n.properties), s = Object.fromEntries(i.map(e => [e, r && r[e] ? r[e] : function(e) {
                     let r = n.properties[e],
-                        i = eh(r, t[e]),
-                        l = r.default;
-                    if (null == l) switch (i) {
-                        case s.STR:
-                        case s.CONSTR:
-                        case s.INT:
-                        case s.FLOAT:
-                        case s.CONINT:
-                        case s.CONFLOAT:
-                            l = "";
+                        i = em(r, t[e]),
+                        s = r.default;
+                    if (null == s) switch (i) {
+                        case l.STR:
+                        case l.CONSTR:
+                        case l.INT:
+                        case l.FLOAT:
+                        case l.CONINT:
+                        case l.CONFLOAT:
+                            s = "";
                             break;
-                        case s.BOOL:
-                            l = !1;
+                        case l.BOOL:
+                            s = !1;
                             break;
                         default:
-                            l = null
+                            s = null
                     }
-                    return l
+                    return s
                 }(e)])), {
                     onSubmit: o,
                     values: a,
                     setFieldValue: c,
                     isTouched: u,
                     setTouched: d,
                     ...p
-                } = ni({
-                    initialValues: l,
+                } = nr({
+                    initialValues: s,
                     validate: Object.fromEntries(i.map(e => [e, function(e) {
                         let r = n.properties[e],
                             i = null != n.required && n.required.includes(e),
-                            l = eh(r, t[e]),
-                            o = e => null == e ? i ? nn : void 0 : "string" != typeof e && "string" == typeof e && ! function(e) {
+                            s = em(r, t[e]),
+                            o = e => null == e ? i ? ne : void 0 : "string" != typeof e && "string" == typeof e && ! function(e) {
                                 let n;
                                 try {
                                     n = new URL(e)
                                 } catch (e) {
                                     return !1
                                 }
                                 return "http:" === n.protocol || "https:" === n.protocol
                             }(e) ? "Not an HTTP(s) URL." : void 0,
                             a = e => {
-                                if (null == e) return i ? nn : void 0;
+                                if (null == e) return i ? ne : void 0;
                                 if ("string" != typeof e) throw TypeError("Invalid type for string form");
-                                return 0 === e.length ? i ? nn : void 0 : void 0 !== r.max_length && e.length > r.max_length ? "Maximum length is ".concat(r.max_length, " characters.") : void 0 !== r.min_length && e.length < r.min_length ? "Minimum length is ".concat(r.min_length, " characters.") : void 0
+                                return 0 === e.length ? i ? ne : void 0 : void 0 !== r.max_length && e.length > r.max_length ? "Maximum length is ".concat(r.max_length, " characters.") : void 0 !== r.min_length && e.length < r.min_length ? "Minimum length is ".concat(r.min_length, " characters.") : void 0
                             },
                             c = e => {
-                                if (null == e || "string" == typeof e && 0 === e.length) return i ? nn : void 0;
+                                if (null == e || "string" == typeof e && 0 === e.length) return i ? ne : void 0;
                                 if ("number" != typeof e) throw TypeError("Invalid type for number form");
                                 return void 0 !== r.maximum && e > r.maximum ? "Maximum value is ".concat(r.maximum) : void 0 !== r.minimum && e < r.minimum ? "Minimum value is ".concat(r.minimum, ".") : void 0
                             };
-                        switch (l) {
-                            case s.FILE:
+                        switch (s) {
+                            case l.FILE:
                                 return o;
-                            case s.STR:
-                            case s.CONSTR:
-                            case s.STR_CHOICE:
+                            case l.STR:
+                            case l.CONSTR:
+                            case l.STR_CHOICE:
                                 return a;
-                            case s.CONFLOAT:
-                            case s.FLOAT:
-                            case s.CONINT:
-                            case s.INT:
-                            case s.INT_CHOICE:
-                            case s.FLOAT_CHOICE:
+                            case l.CONFLOAT:
+                            case l.FLOAT:
+                            case l.CONINT:
+                            case l.INT:
+                            case l.INT_CHOICE:
+                            case l.FLOAT_CHOICE:
                                 return c;
                             default:
                                 return
                         }
                     }(e)]))
                 }), m = (e, t) => {
                     let r = (t, r) => e(Object.fromEntries(i.map(e => [e, function(e, t) {
                         let r = n.properties[e];
                         return null == t ? r.default : t
                     }(e, t[e])])), r);
                     return o(r, t)
-                }, h = (0, I.useRouter)(), [x, f] = (0, e4.X)({
+                }, x = (0, S.useRouter)(), [h, f] = (0, e2.X)({
                     key: "prediction-input-form",
                     defaultValue: null,
                     serialize: e6,
-                    deserialize: e => void 0 === e ? null : ne(e)
+                    deserialize: e => void 0 === e ? null : e9(e)
                 });
                 return (0, y.useEffect)(() => {
                     var e;
                     let r = () => {
                         f({
-                            path: h.asPath,
+                            path: x.asPath,
                             schema: n,
                             filetypes: t,
                             values: a
                         })
                     };
-                    return null === (e = h.events) || void 0 === e || e.on("routeChangeStart", r), document.documentElement.addEventListener("mouseleave", r), null == window || window.addEventListener("beforeunload", r), () => {
+                    return null === (e = x.events) || void 0 === e || e.on("routeChangeStart", r), document.documentElement.addEventListener("mouseleave", r), null == window || window.addEventListener("beforeunload", r), () => {
                         document.documentElement.removeEventListener("mouseleave", r), null == window || window.removeEventListener("beforeunload", r)
                     }
-                }, [n, t, h, f, a]), (0, y.useEffect)(() => {
-                    null != x && (null == x ? void 0 : x.values) && (null == x ? void 0 : x.path) === h.asPath && (null == x ? void 0 : x.schema) != null && JSON.stringify(null == x ? void 0 : x.schema) === JSON.stringify(n) && (null == x ? void 0 : x.filetypes) != null && JSON.stringify(null == x ? void 0 : x.filetypes) === JSON.stringify(t) && Object.keys(x.values).forEach(e => {
-                        (null == t[e] || null != x.values[e]) && (c(e, x.values[e]), d({
+                }, [n, t, x, f, a]), (0, y.useEffect)(() => {
+                    null != h && (null == h ? void 0 : h.values) && (null == h ? void 0 : h.path) === x.asPath && (null == h ? void 0 : h.schema) != null && JSON.stringify(null == h ? void 0 : h.schema) === JSON.stringify(n) && (null == h ? void 0 : h.filetypes) != null && JSON.stringify(null == h ? void 0 : h.filetypes) === JSON.stringify(t) && Object.keys(h.values).forEach(e => {
+                        (null == t[e] || null != h.values[e]) && (c(e, h.values[e]), d({
                             [e]: !0
                         }))
                     })
-                }, [x, c, n, t, h.asPath, d]), {
+                }, [h, c, n, t, x.asPath, d]), {
                     onSubmit: m,
                     values: a,
                     setFieldValue: c,
                     isTouched: u,
                     setTouched: d,
                     ...p
                 }
             }, nl = () => ({
                 placeholder: "Select one",
-                rightSection: (0, d.jsx)(eD.Z, {
+                rightSection: (0, d.jsx)(eq.Z, {
                     size: "1rem"
                 })
-            }), no = e => ({
+            }), ns = e => ({
                 min: null !== (o = e.minimum) && void 0 !== o ? o : void 0,
                 max: null !== (a = e.maximum) && void 0 !== a ? a : void 0,
                 styles: {
                     markLabel: {
                         display: "none"
                     },
                     label: {
                         display: "none"
                     }
                 }
-            }), na = e => ({
+            }), no = e => ({
                 min: null !== (c = e.minimum) && void 0 !== c ? c : void 0,
                 max: null !== (u = e.maximum) && void 0 !== u ? u : void 0,
                 stepHoldDelay: 500,
                 stepHoldInterval: 100,
                 removeTrailingZeros: !0
             });
 
-            function nc(e) {
+            function na(e) {
                 let {
                     fieldName: n,
                     fieldProp: t,
                     filetype: r
-                } = e, i = nr(), l = i.getInputProps(n), o = eh(t, r);
+                } = e, i = nt(), s = i.getInputProps(n), o = em(t, r);
                 switch (o) {
-                    case s.FILE:
-                        return (0, d.jsx)(e8, {
+                    case l.FILE:
+                        return (0, d.jsx)(e7, {
                             filetype: r,
                             maxsize: 1073741824,
                             iconSize: "1.1rem",
                             textProps: {
                                 size: "sm"
                             },
-                            ...l
+                            ...s
                         });
-                    case s.STR:
-                    case s.CONSTR:
-                        return (0, d.jsx)(eM.g, {
+                    case l.STR:
+                    case l.CONSTR:
+                        return (0, d.jsx)(eH.g, {
                             autosize: !0,
                             minRows: 1,
-                            ...l
+                            ...s
                         });
-                    case s.INT:
-                    case s.FLOAT:
-                        return (0, d.jsx)(eW.Y, {
+                    case l.INT:
+                    case l.FLOAT:
+                        return (0, d.jsx)(eM.Y, {
                             w: "100%",
-                            precision: o === s.INT ? 1 : 10,
-                            step: o === s.INT ? 1 : .01,
-                            ...na(t),
-                            ...l
+                            precision: o === l.INT ? 1 : 10,
+                            step: o === l.INT ? 1 : .01,
+                            ...no(t),
+                            ...s
                         });
-                    case s.CONINT:
-                    case s.CONFLOAT:
+                    case l.CONINT:
+                    case l.CONFLOAT:
                         return (0, d.jsxs)(w.Z, {
                             spacing: "1rem",
-                            children: [(0, d.jsx)(eW.Y, {
+                            children: [(0, d.jsx)(eM.Y, {
                                 w: "calc(30% - 1rem)",
-                                precision: o === s.CONINT ? 0 : 10,
-                                step: o === s.CONINT ? 1 : .01,
-                                ...na(t),
-                                ...l
-                            }), (0, d.jsx)(eK.i, {
+                                precision: o === l.CONINT ? 0 : 10,
+                                step: o === l.CONINT ? 1 : .01,
+                                ...no(t),
+                                ...s
+                            }), (0, d.jsx)(eW.i, {
                                 w: "70%",
-                                value: l.value,
-                                onChange: l.onChange,
-                                step: o === s.CONINT ? 1 : .01,
-                                ...no(t)
+                                value: s.value,
+                                onChange: s.onChange,
+                                step: o === l.CONINT ? 1 : .01,
+                                ...ns(t)
                             })]
                         });
-                    case s.STR_CHOICE:
+                    case l.STR_CHOICE:
                         if (null == t.choices) throw TypeError("No choices");
-                        return (0, d.jsx)(eU.Ph, {
+                        return (0, d.jsx)(eK.Ph, {
                             data: t.choices,
-                            ...l,
+                            ...s,
                             ...nl()
                         });
-                    case s.BOOL:
-                        return (0, d.jsx)(eq.r, {
-                            ...l
+                    case l.BOOL:
+                        return (0, d.jsx)(eU.r, {
+                            ...s
                         });
-                    case s.INT_CHOICE:
-                    case s.FLOAT_CHOICE:
+                    case l.INT_CHOICE:
+                    case l.FLOAT_CHOICE:
                         if (null == t.choices) throw TypeError("No choices");
-                        return (0, d.jsx)(eU.Ph, {
-                            value: null != l.value ? l.value.toString() : null,
+                        return (0, d.jsx)(eK.Ph, {
+                            value: null != s.value ? s.value.toString() : null,
                             data: t.choices.map(e => e.toString()),
                             onChange: e => {
                                 let n = null;
-                                "string" == typeof e && (n = Number(e)), l.onChange(n)
+                                "string" == typeof e && (n = Number(e)), s.onChange(n)
                             },
-                            ...Object.fromEntries(Object.entries(l).filter(e => !["onChange", "value"].includes(e[0])))
+                            ...Object.fromEntries(Object.entries(s).filter(e => !["onChange", "value"].includes(e[0])))
                         });
                     default:
                         throw TypeError("Unknown field type ".concat(o))
                 }
             }
 
-            function nu(e) {
+            function nc(e) {
                 let {
                     filetype: n,
                     value: t
                 } = e;
-                if (n) return (0, d.jsx)(em, {
+                if (n) return (0, d.jsx)(ep, {
                     file: t,
                     filetype: n
                 });
                 if (void 0 !== t) return (0, d.jsx)(eS, {
                     children: "string" != typeof t ? t.toString() : t
                 });
                 throw Error("`value` is undefined")
             }
 
-            function nd(e) {
+            function nu(e) {
                 let {
                     withForm: n,
                     schema: t,
                     filetypes: r,
                     values: i,
-                    showOptions: s,
-                    spacing: l
+                    showOptions: l,
+                    spacing: s
                 } = e, o = [], a = [];
 
                 function c(e) {
                     return (null == t ? void 0 : t.required) != null && (null == t ? void 0 : t.required.includes(e))
                 }
 
                 function u(e) {
-                    let s = t.properties[e],
-                        l = r[e];
-                    return n ? (0, d.jsx)(nc, {
+                    let l = t.properties[e],
+                        s = r[e];
+                    return n ? (0, d.jsx)(na, {
                         fieldName: e,
-                        fieldProp: s,
-                        filetype: l
-                    }) : (0, d.jsx)(nu, {
-                        filetype: l,
+                        fieldProp: l,
+                        filetype: s
+                    }) : (0, d.jsx)(nc, {
+                        filetype: s,
                         value: void 0 === i ? void 0 : i[e]
                     })
                 }
                 return Object.keys(t.properties).forEach(e => {
                     c(e) && o.push({
                         name: e,
                         component: u(e)
@@ -1359,341 +1357,337 @@
                     c(e) || a.push({
                         name: e,
                         component: u(e)
                     })
                 }), (0, d.jsxs)(p.x, {
                     fz: "md",
                     children: [(0, d.jsx)(C.K, {
-                        spacing: l,
+                        spacing: s,
                         children: o.map(e => (0, d.jsxs)("div", {
-                            children: [(0, d.jsx)(V, {
+                            children: [(0, d.jsx)(J, {
                                 name: e.name,
                                 required: !!n,
                                 description: n ? t.properties[e.name].description : void 0
                             }), e.component]
                         }, "input-field-".concat(e.name)))
-                    }), s && a.length > 0 ? (0, d.jsx)(T.T, {
-                        h: l
-                    }) : void 0, (0, d.jsx)(eH.U, {
-                        in: null != s && s,
+                    }), l && a.length > 0 ? (0, d.jsx)(T.T, {
+                        h: s
+                    }) : void 0, (0, d.jsx)(eA.U, {
+                        in: null != l && l,
                         children: (0, d.jsx)(C.K, {
-                            spacing: l,
+                            spacing: s,
                             children: a.map(e => (0, d.jsxs)("div", {
-                                children: [(0, d.jsx)(V, {
+                                children: [(0, d.jsx)(J, {
                                     name: e.name,
                                     required: !1,
                                     description: n ? t.properties[e.name].description : void 0
                                 }), e.component]
                             }, "input-field-".concat(e.name)))
                         })
                     })]
                 })
             }
-            nd.defaultProps = {
+            nu.defaultProps = {
                 spacing: "md",
                 values: void 0,
                 showOptions: !1
             };
-            var np = t(8078);
+            var nd = t(8078);
 
-            function nm(e) {
+            function np(e) {
                 let {
                     checked: n,
                     onChange: t,
                     ...r
                 } = e;
-                return (0, d.jsx)(np.X, {
+                return (0, d.jsx)(nd.X, {
                     label: "Show options",
                     checked: n,
                     onChange: e => t(e.currentTarget.checked),
                     ...r
                 })
             }
-            var nh = t(3575);
+            var nm = t(3575);
             let nx = {
                     height: "3rem"
                 },
-                nf = e => nh.N9.show({
+                nh = e => nm.N9.show({
                     message: "".concat(e),
                     color: "red",
                     sx: nx
                 });
-            var ng = t(4075);
-            let nj = (0, y.forwardRef)((e, n) => {
+            var nf = t(4075);
+            let ng = (0, y.forwardRef)((e, n) => {
                 var t, r;
                 let i;
                 let {
-                    prediction: s,
-                    model: l,
+                    prediction: l,
+                    model: s,
                     setPrediction: o
                 } = e, {
                     demo_output_schema: a,
                     demo_output_filetypes: c
-                } = l, u = new f.Z, m = z(), h = B(m), [x, g] = (0, y.useState)("preview"), j = (0, P.useMutation)({
+                } = s, u = new f.Z, m = R(), x = P(m), [h, g] = (0, y.useState)("preview"), j = (0, Z.useMutation)({
                     mutationFn: () => (u.remove("current_prediction", {
                         path: "/"
-                    }), o(null), h.cancel(s.id))
-                }), v = (null == s ? void 0 : s.status) && ["pending", "running"].includes(s.status) ? "auto" : "smooth", b = (0, d.jsx)(e_, {
+                    }), o(null), x.cancel(l.id))
+                }), v = (null == l ? void 0 : l.status) && ["pending", "running"].includes(l.status) ? "auto" : "smooth", b = (0, d.jsx)(eL, {
                     autoScroll: v,
-                    children: null !== (t = null == s ? void 0 : s.logs) && void 0 !== t ? t : ""
+                    children: null !== (t = null == l ? void 0 : l.logs) && void 0 !== t ? t : ""
                 }), O = (0, d.jsx)(T.T, {
                     h: "md"
                 }), C = (0, d.jsx)(T.T, {
                     h: "xl"
                 });
-                switch (null == s ? void 0 : s.status) {
+                switch (null == l ? void 0 : l.status) {
                     case "pending":
                     case "running":
                         i = (0, d.jsxs)(d.Fragment, {
-                            children: [(0, d.jsx)(M, {
-                                status: s.status,
-                                logsArea: "running" === s.status ? b : void 0
-                            }), O, (0, d.jsx)(Q.z, {
+                            children: [(0, d.jsx)(H, {
+                                status: l.status,
+                                logsArea: "running" === l.status ? b : void 0
+                            }), O, (0, d.jsx)(X.z, {
                                 onClick: () => j.mutate(),
                                 variant: "default",
                                 fullWidth: !0,
                                 children: "Cancel"
                             })]
                         });
                         break;
                     case "failed":
                         i = (0, d.jsxs)(d.Fragment, {
-                            children: [(0, d.jsx)(A, {
-                                failureReason: s.failure_reason,
+                            children: [(0, d.jsx)(B, {
+                                failureReason: l.failure_reason,
                                 logsArea: b
                             }), C]
                         });
                         break;
                     case "success":
                         i = (0, d.jsxs)(d.Fragment, {
-                            children: [(0, d.jsx)(eA, {
-                                mode: x,
+                            children: [(0, d.jsx)(eB, {
+                                mode: h,
                                 onChange: g
-                            }), O, (0, d.jsx)(eF, {
-                                mode: x,
-                                output: s.output,
-                                demoOutput: s.demo_output,
+                            }), O, (0, d.jsx)(e_, {
+                                mode: h,
+                                output: l.output,
+                                demoOutput: l.demo_output,
                                 demoOutputSchema: a,
                                 demoOutputFiletypes: c,
-                                logs: null !== (r = null == s ? void 0 : s.logs) && void 0 !== r ? r : ""
+                                logs: null !== (r = null == l ? void 0 : l.logs) && void 0 !== r ? r : ""
                             }), C, (0, d.jsx)(w.Z, {
                                 position: "right",
-                                children: (0, d.jsx)(Q.z, {
+                                children: (0, d.jsx)(X.z, {
                                     variant: "default",
                                     onClick: () => {
                                         window.scrollTo({
                                             top: 0,
                                             behavior: "auto"
                                         }), u.remove("current_prediction", {
                                             path: "/"
                                         }), o(null)
                                     },
-                                    leftIcon: (0, d.jsx)(ng.Z, {
+                                    leftIcon: (0, d.jsx)(nf.Z, {
                                         size: "1rem"
                                     }),
                                     children: "Clear"
                                 })
                             })]
                         });
                         break;
                     default:
-                        i = (0, d.jsx)(D, {})
+                        i = (0, d.jsx)(q, {})
                 }
                 return (0, d.jsx)(p.x, {
                     ref: n,
                     children: i
                 })
             });
-            nj.displayName = "ModelRunProgress";
-            var nv = t(9204),
-                ny = t(8697);
+            ng.displayName = "ModelRunProgress";
+            var nj = t(8697);
 
-            function nb(e) {
+            function nv(e) {
                 var n, t, r;
                 let {
                     model: i,
-                    currentPrediction: s,
-                    onFormSubmit: l,
+                    currentPrediction: l,
+                    onFormSubmit: s,
                     onError: o
                 } = e, {
                     input_schema: a,
                     input_filetypes: c
-                } = i, u = (0, I.useRouter)(), p = z(), m = Object.freeze({
+                } = i, u = (0, S.useRouter)(), p = R(), m = Object.freeze({
                     axiosInstance: p,
                     upload: function(e) {
                         let n = new FormData;
                         return n.append("file", e), p.post("/files", n, {
                             timeout: 3e5,
                             headers: {
                                 "Content-Type": "multipart/form-data"
                             }
                         })
                     }
-                }), [h, x] = (0, y.useState)(!1), [f, g] = (0, y.useState)(!1), [j, v] = (0, y.useState)(!1), {
+                }), [x, h] = (0, y.useState)(!1), [f, g] = (0, y.useState)(!1), [j, v] = (0, y.useState)(!1), {
                     start: b
-                } = (0, ny.K)(() => v(!1), 2e3), O = () => {
+                } = (0, nj.K)(() => v(!1), 2e3), O = () => {
                     v(!0), b()
-                }, E = ns({
+                }, E = ni({
                     schema: a,
                     filetypes: c
                 });
                 null === (n = u.events) || void 0 === n || n.on("routeChangeComplete", () => {
                     g(!1), v(!1)
                 }), null === (t = u.events) || void 0 === t || t.on("routeChangeError", () => {
                     g(!1), v(!1)
                 });
-                let S = async e => {
-                    let n;
-                    return n = e instanceof File ? await m.upload(e).then(e => e.data.serving_url).catch(e => (n = null, (0, nv.IZ)(e) && e.response && 401 === e.response.status && u.push("/sign_in"), n)) : e
-                }, N = async e => {
+                let I = async e => e instanceof File ? await m.upload(e).then(e => e.data.serving_url).catch(() => "") : e, N = async e => {
                     g(!0), O();
                     let n = Object.keys(i.input_schema.properties),
                         t = n.filter(e => !!i.input_filetypes[e]),
-                        r = t.map(n => S(e[n])),
-                        s = await Promise.all(r);
-                    if (s.some(e => null == e)) {
-                        o(), g(!1);
+                        r = t.map(n => I(e[n])),
+                        l = await Promise.all(r);
+                    if (l.some(e => "" === e)) {
+                        console.log(l), o(), g(!1);
                         return
                     }
                     let a = Object.fromEntries(n.map(n => {
                         let r = t.indexOf(n);
-                        return r >= 0 ? [n, s[r]] : [n, e[n]]
+                        return r >= 0 ? [n, l[r]] : [n, e[n]]
                     }));
-                    l(a), g(!1)
+                    s(a), g(!1)
                 }, {
                     setValues: k
                 } = E;
                 return (0, y.useLayoutEffect)(() => {
-                    null != s && k(s.input)
-                }, [s, k]), (0, d.jsxs)(C.K, {
+                    null != l && k(l.input)
+                }, [l, k]), (0, d.jsxs)(C.K, {
                     w: "100%",
                     spacing: "0",
                     children: [null != (r = i.input_schema).required && Object.keys(r.properties).some(e => {
                         var n;
                         return !(null === (n = r.required) || void 0 === n ? void 0 : n.includes(e))
                     }) ? (0, d.jsx)(w.Z, {
                         position: "right",
-                        children: (0, d.jsx)(nm, {
-                            checked: h,
-                            onChange: x
+                        children: (0, d.jsx)(np, {
+                            checked: x,
+                            onChange: h
                         })
-                    }) : void 0, (0, d.jsx)(nt, {
+                    }) : void 0, (0, d.jsx)(nn, {
                         form: E,
                         children: (0, d.jsxs)("form", {
                             onSubmit: E.onSubmit(N),
-                            children: [(0, d.jsx)(nd, {
+                            children: [(0, d.jsx)(nu, {
                                 withForm: !0,
                                 schema: a,
                                 filetypes: c,
-                                showOptions: h
+                                showOptions: x
                             }), (0, d.jsx)(T.T, {
                                 h: "xxl"
                             }), (0, d.jsxs)(w.Z, {
                                 position: "right",
                                 grow: !0,
-                                children: [(0, d.jsx)(Q.z, {
+                                children: [(0, d.jsx)(X.z, {
                                     onClick: E.reset,
-                                    leftIcon: (0, d.jsx)(ng.Z, {
+                                    leftIcon: (0, d.jsx)(nf.Z, {
                                         size: "1rem"
                                     }),
                                     variant: "default",
                                     children: "Reset"
-                                }), (0, d.jsx)(Q.z, {
-                                    leftIcon: (0, d.jsx)(ee.Z, {
+                                }), (0, d.jsx)(X.z, {
+                                    leftIcon: (0, d.jsx)($.Z, {
                                         size: "1rem"
                                     }),
                                     color: "run-green.4",
                                     loading: f || j,
                                     type: f || j ? void 0 : "submit",
                                     children: "Run"
                                 })]
                             })]
                         })
                     })]
                 })
             }
-            let nO = "Failed to run by unexpected server error";
+            let ny = "Failed to run by unexpected server error";
 
-            function nw(e) {
+            function nb(e) {
                 let {
                     model: n,
                     currentPrediction: t
-                } = e, r = z(), i = B(r), s = new f.Z, [l, o] = (0, y.useState)(t), {
+                } = e, r = R(), i = P(r), l = new f.Z, [s, o] = (0, y.useState)(t), {
                     scrollIntoView: a,
                     targetRef: c
-                } = (0, Z.g)({
+                } = (0, z.g)({
                     axis: "y"
-                }), u = (0, P.useMutation)({
+                }), u = (0, Z.useMutation)({
                     mutationFn: e => {
                         let n = i.create(e);
-                        return null != l && ["pending", "running"].includes(l.status) ? i.cancel(l.id).then(() => n) : n
+                        return null != s && ["pending", "running"].includes(s.status) ? i.cancel(s.id).then(() => n) : n
                     },
                     onSuccess: e => {
                         let {
                             data: n
                         } = e;
-                        s.set("current_prediction", n.id, {
+                        l.set("current_prediction", n.id, {
                             path: "/"
                         }), console.log(n), o(n), a({
                             alignment: "start"
                         })
                     },
                     onError: () => {
-                        nf(nO)
+                        nh(ny)
                     }
                 });
-                return (0, P.useQuery)({
-                    enabled: null != l && ("running" === l.status || "pending" === l.status),
+                return (0, Z.useQuery)({
+                    enabled: null != s && ("running" === s.status || "pending" === s.status),
                     retry: 5,
                     refetchInterval: 500,
                     queryKey: "",
-                    queryFn: () => i.get(l.id),
+                    queryFn: () => i.get(s.id),
                     onSuccess: e => o(e.data),
-                    onError: () => nf("Failed to update the status from server")
+                    onError: () => nh("Failed to update the status from server")
                 }), (0, d.jsxs)(w.Z, {
                     w: "100%",
                     spacing: "2rem",
                     align: "top",
                     grow: !0,
-                    children: [(0, d.jsx)(K, {
+                    children: [(0, d.jsx)(W, {
                         title: "Input",
-                        children: (0, d.jsx)(nb, {
+                        children: (0, d.jsx)(nv, {
                             model: n,
                             currentPrediction: t,
                             onFormSubmit: u.mutate,
-                            onError: () => nf(nO)
+                            onError: () => nh(ny)
                         })
-                    }), (0, d.jsx)(K, {
+                    }), (0, d.jsx)(W, {
                         title: "Output",
-                        children: (0, d.jsx)(nj, {
+                        children: (0, d.jsx)(ng, {
                             ref: c,
-                            prediction: l,
+                            prediction: s,
                             model: n,
                             setPrediction: o
                         })
                     })]
                 })
             }
 
-            function nC() {
-                let e = z(),
+            function nO() {
+                let e = R(),
                     n = Object.freeze({
                         axiosInstance: e,
                         get: function() {
                             return e.get("/metadata")
                         }
                     }),
-                    t = B(e),
+                    t = P(e),
                     r = new f.Z,
-                    [i, s] = (0, y.useState)(null),
-                    [l, o] = (0, y.useState)(null);
+                    [i, l] = (0, y.useState)(null),
+                    [s, o] = (0, y.useState)(null);
                 return (0, y.useLayoutEffect)(() => {
                     (async function() {
-                        await n.get().then(e => s(e.data)).catch(() => {
-                            nf("Failed to load model metadata by unexpected server error")
+                        await n.get().then(e => l(e.data)).catch(() => {
+                            nh("Failed to load model metadata by unexpected server error")
                         })
                     })()
                 }, []), (0, y.useEffect)(() => {
                     var e;
                     let n = null !== (e = r.get("current_prediction")) && void 0 !== e ? e : null;
                     (async function() {
                         n && await t.get(n).then(e => {
@@ -1701,35 +1695,35 @@
                                 data: n
                             } = e;
                             o(n)
                         }).catch(() => null)
                     })()
                 }, [i]), (0, d.jsxs)(p.x, {
                     children: [i ? (0, d.jsxs)(d.Fragment, {
-                        children: [(0, d.jsxs)(x(), {
+                        children: [(0, d.jsxs)(h(), {
                             children: [(0, d.jsx)("title", {
                                 children: "".concat(i.name, " - Run | Tungsten")
                             }), (0, d.jsx)("meta", {
                                 name: "viewport",
                                 content: "initial-scale=1.0, width=device-width"
                             })]
                         }), (0, d.jsx)(_, {
                             model: i,
-                            children: (0, d.jsx)(nw, {
+                            children: (0, d.jsx)(nb, {
                                 model: i,
-                                currentPrediction: l
+                                currentPrediction: s
                             })
                         })]
                     }) : void 0, (0, d.jsx)(m.f, {
                         visible: null == i
                     })]
                 })
             }
         },
         7579: function() {}
     },
     function(e) {
-        e.O(0, [544, 657, 774, 888, 179], function() {
+        e.O(0, [544, 8, 774, 888, 179], function() {
             return e(e.s = 8312)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-c7250373c9756530.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -72,15 +72,15 @@
         return Promise.all(Object.keys(s.f).reduce(function(t, n) {
             return s.f[n](e, t), t
         }, []))
     }, s.u = function(e) {
         return "static/chunks/925e0f50.b1049bda686b7dd5.js"
     }, s.miniCssF = function(e) {
         return "static/css/" + ({
-            657: "ba142f674ff207f4",
+            8: "ba142f674ff207f4",
             888: "9e15ad138d9a3a18"
         })[e] + ".css"
     }, s.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || Function("return this")()
         } catch (e) {
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/_next/static/fMfFQ47widM1tYI27opXD/_buildManifest.js` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 self.__BUILD_MANIFEST = {
     __rewrites: {
         beforeFiles: [],
         afterFiles: [],
         fallback: []
     },
-    "/": ["static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js", "static/css/ba142f674ff207f4.css", "static/chunks/657-2e4c261bfa28c304.js", "static/chunks/pages/index-8f3afe3801b5eb58.js"],
+    "/": ["static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js", "static/css/ba142f674ff207f4.css", "static/chunks/8-936f7a161aaf624f.js", "static/chunks/pages/index-27c7bca72f8b0e82.js"],
     "/404": ["static/chunks/pages/404-1e77c517c165fca8.js"],
     "/500": ["static/chunks/pages/500-8c3654eb5b977ca1.js"],
     "/_error": ["static/chunks/pages/_error-8353112a01355ec2.js"],
     sortedPages: ["/", "/404", "/500", "/_app", "/_error"]
 }, self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><link rel="preload" href="/_next/static/css/ba142f674ff207f4.css" as="style"/><link rel="stylesheet" href="/_next/static/css/ba142f674ff207f4.css" data-n-p=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c7250373c9756530.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js" defer=""></script><script src="/_next/static/chunks/657-2e4c261bfa28c304.js" defer=""></script><script src="/_next/static/chunks/pages/index-8f3afe3801b5eb58.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_buildManifest.js" defer=""></script><script src="/_next/static/fMfFQ47widM1tYI27opXD/_ssgManifest.js" defer=""></script><style data-emotion="mantine 1avyp1d 1nisyfe n34huv">.mantine-1nisyfe{position:absolute;top:0rem;right:0rem;left:0rem;bottom:0rem;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;overflow:hidden;}.mantine-n34huv{position:absolute;top:0rem;right:0rem;left:0rem;bottom:0rem;background-color:rgba(255, 255, 255, 0.75);border-radius:0rem;z-index:400;}.mantine-n34huv[data-center]{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-1avyp1d"><div class="mantine-LoadingOverlay-root mantine-1nisyfe" style="z-index:400"><svg width="2.25rem" height="2.25rem" viewBox="0 0 38 38" xmlns="http://www.w3.org/2000/svg" stroke="#228be6" class="mantine-1avyp1d" style="z-index:calc(400 + 1)" role="presentation"><g fill="none" fill-rule="evenodd"><g transform="translate(2.5 2.5)" stroke-width="5"><circle stroke-opacity=".5" cx="16" cy="16" r="16"></circle><path d="M32 16c0-9.94-8.06-16-16-16"><animateTransform attributeName="transform" type="rotate" from="0 16 16" to="360 16 16" dur="1s" repeatCount="indefinite"></animateTransform></path></g></g></svg><div class="mantine-Overlay-root mantine-n34huv"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"fMfFQ47widM1tYI27opXD","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/css/9e15ad138d9a3a18.css" as="style"/><link rel="stylesheet" href="/_next/static/css/9e15ad138d9a3a18.css" data-n-g=""/><link rel="preload" href="/_next/static/css/ba142f674ff207f4.css" as="style"/><link rel="stylesheet" href="/_next/static/css/ba142f674ff207f4.css" data-n-p=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-fb2189cefdf627af.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-74c4d6b2b5c362f3.js" defer=""></script><script src="/_next/static/chunks/pages/_app-0e0952e6981dcf87.js" defer=""></script><script src="/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js" defer=""></script><script src="/_next/static/chunks/8-936f7a161aaf624f.js" defer=""></script><script src="/_next/static/chunks/pages/index-27c7bca72f8b0e82.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js" defer=""></script><script src="/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js" defer=""></script><style data-emotion="mantine 1avyp1d 1nisyfe n34huv">.mantine-1nisyfe{position:absolute;top:0rem;right:0rem;left:0rem;bottom:0rem;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;overflow:hidden;}.mantine-n34huv{position:absolute;top:0rem;right:0rem;left:0rem;bottom:0rem;background-color:rgba(255, 255, 255, 0.75);border-radius:0rem;z-index:400;}.mantine-n34huv[data-center]{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}</style></head><body><div id="__next"><style data-emotion="css-global 1w883ez">html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:0.0625rem dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}</style><style data-emotion="css-global 1plzheg">*,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:Inter,sans-serif;background-color:#fff;color:#000;line-height:1.55;font-size:15px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}</style><style data-emotion="css-global 19s4s3x">input[type=text]{font-size:15px;}.mantine-Textarea-input{font-size:15px;}.mantine-Alert-message{font-size:15px;}.layout-container{min-width:max(74rem, 100%);}.layout-container-inner{min-width:64rem;padding-left:0;padding-right:0;}</style><div class="mantine-1avyp1d"><div class="mantine-LoadingOverlay-root mantine-1nisyfe" style="z-index:400"><svg width="2.25rem" height="2.25rem" viewBox="0 0 38 38" xmlns="http://www.w3.org/2000/svg" stroke="#228be6" class="mantine-1avyp1d" style="z-index:calc(400 + 1)" role="presentation"><g fill="none" fill-rule="evenodd"><g transform="translate(2.5 2.5)" stroke-width="5"><circle stroke-opacity=".5" cx="16" cy="16" r="16"></circle><path d="M32 16c0-9.94-8.06-16-16-16"><animateTransform attributeName="transform" type="rotate" from="0 16 16" to="360 16 16" dur="1s" repeatCount="indefinite"></animateTransform></path></g></g></svg><div class="mantine-Overlay-root mantine-n34huv"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"afTF15k0tNJ2rEveq5WZR","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.2/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,17 +64,18 @@
 
             file_serving_url = file_service.build_serving_url(filename, request=request)
             file_serving_urls.append(file_serving_url)
             return file_serving_url
 
         input = self.input.copy()
         for field_name in input_filetypes:
-            input[field_name] = convert_file_url_to_http(
-                input[field_name], allow_unknown_file_url=False
-            )
+            if input[field_name] is not None:
+                input[field_name] = convert_file_url_to_http(
+                    input[field_name], allow_unknown_file_url=False
+                )
         output = (
             None
             if self.output is None
             else apply_to_jsonable(
                 self.output,
                 cond=check_if_file_uri,
                 fn=lambda s: convert_file_url_to_http(s, allow_unknown_file_url=True),
@@ -116,17 +117,20 @@
 
     def create_prediction(self, input: t.Dict) -> str:
         _fill_omitted_input_fields_as_defaults(input, self.input_schema)
         input_filenames: t.Set[str] = set()
 
         try:
             for field_name in self.input_filetypes:
-                fileurl, filename = self._convert_file_serving_url_to_file_url(input[field_name])
-                input[field_name] = fileurl
-                input_filenames.add(filename)
+                if field_name in input.keys() and input[field_name] is not None:
+                    fileurl, filename = self._convert_file_serving_url_to_file_url(
+                        input[field_name]
+                    )
+                    input[field_name] = fileurl
+                    input_filenames.add(filename)
             try:
                 prediction_id, file_paths = self.model_client.create_demo(inputs=[input])
             except ModelClientError as e:
                 _raise_http_exc_by_model_client_err(e)
             pred = SavedPrediction(
                 id=prediction_id,
                 status="pending",
@@ -302,13 +306,20 @@
 
 def _raise_not_found(prediction_id: str):
     raise HTTPException(status_code=404, detail="No such prediction: " + prediction_id)
 
 
 def _fill_omitted_input_fields_as_defaults(input: t.Dict, input_schema: t.Dict):
     if "required" not in input_schema:
-        return
+        required_field_names = []
+    else:
+        required_field_names = input_schema["required"]
 
-    existing_field_names_in_input = list(input.keys())
+    required_field_names = list(filter(lambda key: key in required_field_names, input.keys()))
     for field_name, field_property in input_schema["properties"].items():
-        if field_name not in existing_field_names_in_input and "default" in field_property:
-            input[field_name] = field_property["default"]
+        if field_name not in input:
+            if "default" in field_property:
+                input[field_name] = field_property["default"]
+            elif field_name not in required_field_names:
+                input[field_name] = None
+            else:
+                HTTPException(status_code=422, detail=f"Field {field_name} is required.")
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/io.py` & `tungstenkit-0.1.2/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.2/tungstenkit/_internal/io_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import inspect
 import typing as t
 
 from pydantic import create_model as create_pydantic_model
 from pydantic.fields import FieldInfo
+from pydantic.typing import is_none_type, is_union
 
 from tungstenkit._internal import io
 from tungstenkit._internal.utils.string import camel_to_snake
 from tungstenkit._internal.utils.types import get_type_args, get_type_origin
 
 SUPPORTED_INPUT_TYPES: t.List[t.Type] = [
     int,
@@ -34,20 +36,36 @@
     if not issubclass(input_cls, io.BaseIO):
         raise TypeError(f"Input type {input_cls} is not a subclass of {io.BaseIO}")
 
     invalid_types: t.Dict[str, t.Type] = dict()
     type_hints = t.get_type_hints(input_cls)
     fields = input_cls.__fields__
     for name, type_ in type_hints.items():
+        field = fields[name]
         origin = get_type_origin(type_)
+        type_args = get_type_args(type_)
         valid = False
-        for supported_input_type in SUPPORTED_INPUT_TYPES:
-            if issubclass(origin, supported_input_type):
-                valid = True
-                break
+
+        if (
+            not field.required
+            and is_union(origin)
+            and sum(is_none_type(arg) for arg in type_args) == 1
+            and len(type_args) == 2
+        ):
+            type_idx = [is_none_type(arg) for arg in type_args].index(False)
+
+            valid = inspect.isclass(type_args[type_idx]) and any(
+                issubclass(type_args[type_idx], supported_input_type)
+                for supported_input_type in SUPPORTED_INPUT_TYPES
+            )
+        elif inspect.isclass(origin):
+            valid = any(
+                issubclass(origin, supported_input_type)
+                for supported_input_type in SUPPORTED_INPUT_TYPES
+            )
 
         if not valid:
             invalid_types[input_cls.__name__ + "." + name] = type_
 
     if len(invalid_types) > 0:
         err_msg = "Invalid input types:\n"
         for name, type_ in invalid_types.items():
@@ -61,14 +79,15 @@
             ]
         )
         raise TypeError(err_msg)
 
     # Set the default description on input fields if not set
     updated_fields: t.Dict[str, t.Tuple[t.Type, FieldInfo]] = dict()
     for name, type_ in type_hints.items():
+        field = fields[name]
         field_info = fields[name].field_info
         if not field_info.description:
             field_info.description = _build_default_description(field_name=name)
             updated_fields[name] = (type_, field_info)
 
     if len(updated_fields) > 0:
         input_cls = create_pydantic_model(  # type: ignore
@@ -77,27 +96,33 @@
             **updated_fields,
         )
 
     return input_cls
 
 
 def validate_output_class(output_cls: t.Type):
-    if not issubclass(output_cls, io.BaseIO):
+    if not inspect.isclass(output_cls) or not issubclass(output_cls, io.BaseIO):
         raise TypeError(f"Output type '{output_cls}' is not a subclass of '{io.BaseIO}'")
 
     invalid_types_and_reasons: t.Dict[str, t.Tuple[t.Type, str]] = dict()
 
     unsupported_field = False
     unsupported_dict_key = False
 
     def validate_type(type_: t.Type, field_name: str):
         nonlocal unsupported_field, unsupported_dict_key
+
         origin = get_type_origin(type_)
         type_args = get_type_args(type_)
 
+        if not inspect.isclass(origin):
+            unsupported_field = True
+            invalid_types_and_reasons[field_name] = (type_, "unsupported output type")
+            return
+
         for supported_output_type in SUPPORTED_OUTPUT_TERMINAL_TYPES:
             if issubclass(origin, supported_output_type):
                 return
 
         def set_no_type_args_err():
             invalid_types_and_reasons[field_name] = (
                 type_,
@@ -122,16 +147,19 @@
                         type_args[0],
                         "unsupported type for dictionary keys.",
                     )
                     unsupported_dict_key = True
                 validate_type(type_args[1], field_name + ".<'value'>")
 
         elif issubclass(origin, io.BaseIO):
-            for name, type_ in t.get_type_hints(origin).items():
-                validate_type(type_, field_name + "." + name)
+            if any(not field.required for field in origin.__fields__.values()):
+                invalid_types_and_reasons[field_name] = (type_, "output cannot have an option")
+            else:
+                for name, type_ in t.get_type_hints(origin).items():
+                    validate_type(type_, field_name + "." + name)
 
         else:
             unsupported_field = True
             invalid_types_and_reasons[field_name] = (type_, "unsupported output type")
 
     validate_type(output_cls, output_cls.__name__)
 
@@ -176,14 +204,27 @@
 
     ret: t.Dict[str, io.FileType] = dict()
 
     def _get_filetypes(type_: type, json_index: str):
         origin = get_type_origin(type_)
         type_args = get_type_args(type_)
 
+        if is_union(origin):
+            is_type_arg_none = [is_none_type(arg) for arg in type_args]
+            if sum(is_type_arg_none) != 1 or len(type_args) != 2:
+                return
+
+            type_idx = is_type_arg_none.index(False)
+            type_ = type_args[type_idx]
+            origin = get_type_origin(type_)
+            type_args = get_type_args(type_)
+
+        if not inspect.isclass(origin):
+            return
+
         if issubclass(origin, io.File):
             ret[json_index] = origin._get_typeenum()
 
         elif issubclass(origin, list):
             _get_filetypes(type_args[0], json_index=json_index + ".$item")
 
         elif issubclass(origin, dict):
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.2/tungstenkit/_internal/json_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.2/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.2/tungstenkit/_internal/model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.2/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/avatar_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/model_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.2/tungstenkit/_internal/storables/source_file_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/task.py` & `tungstenkit-0.1.2/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.2/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import typing
 
 from packaging.version import Version
+from pydantic.typing import get_args
 
 from tungstenkit._versions import py_version
 
 
 def get_type_args(t):
-    if py_version >= Version("3.8"):
-        return typing.get_args(t)
     try:
-        return t.__args__
-    except AttributeError:
+        return get_args(t)
+    except (AttributeError, TypeError):
         return tuple()
 
 
 def get_type_origin(t):
     if py_version >= Version("3.8"):
         origin = typing.get_origin(t)
         if origin is None:
             return t
+        return origin
     try:
         if py_version >= Version("3.7"):
             return t.__origin__
         return t.__extra__
     except AttributeError:
         return t
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.2/tungstenkit/_internal/utils/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
 def order_optional_version(optional_version: t.Optional[Version]):
     if optional_version is None:
         return MIN_VER
     return optional_version
 
 
-def check_version_with_constraint(ver: t.Optional[Version], constraint: t.Optional[Version]):
+def check_version_matching_clause_loosely(
+    ver: t.Optional[Version], constraint: t.Optional[Version]
+):
     """
     Check a version satisfies a constraint.
     For example, if constraint is ``1.1``, version ``1.2``, ``1`` is not passed.
     """
     if constraint is None:
         return True
```

### Comparing `tungstenkit-0.1.1a2/tungstenkit/exceptions.py` & `tungstenkit-0.1.2/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.1a2/PKG-INFO` & `tungstenkit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.1a2
+Version: 0.1.2
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

