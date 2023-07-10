# Comparing `tmp/tungstenkit-0.1.2.post1.tar.gz` & `tmp/tungstenkit-0.1.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.2.post1.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.2.post3.tar", max compression
```

## Comparing `tungstenkit-0.1.2.post1.tar` & `tungstenkit-0.1.2.post3.tar`

### file list

```diff
@@ -1,172 +1,173 @@
--rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2.post1/LICENSE
--rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2.post1/README.md
--rw-r--r--   0        0        0     2874 2023-07-07 10:42:20.094860 tungstenkit-0.1.2.post1/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2.post1/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post1/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0     9630 2023-06-07 05:35:48.388092 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5492 2023-07-07 10:41:56.643078 tungstenkit-0.1.2.post1/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.2.post1/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    14492 2023-07-06 11:25:00.322496 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     8398 2023-07-07 09:00:11.183463 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1337 2023-07-06 06:51:45.833948 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1381 2023-07-06 07:14:54.727252 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
--rw-r--r--   0        0        0     3573 2023-06-07 06:31:35.793599 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2.post1/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2.post1/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-06 20:22:25.417271 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0     6231 2023-07-06 20:22:25.381271 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/500.html
--rw-r--r--   0        0        0      523 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js
--rw-r--r--   0        0        0   707397 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js
--rw-r--r--   0        0        0    78459 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
--rw-r--r--   0        0        0   458866 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
--rw-r--r--   0        0        0   141052 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    89842 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
--rw-r--r--   0        0        0     5020 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
--rw-r--r--   0        0        0     5049 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
--rw-r--r--   0        0        0   130456 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
--rw-r--r--   0        0        0      245 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0        0        0    28246 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js
--rw-r--r--   0        0        0    91460 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3851 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js
--rw-r--r--   0        0        0      791 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
--rw-r--r--   0        0        0    43645 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
--rw-r--r--   0        0        0   259838 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0     6242 2023-07-06 20:22:25.393271 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0    61184 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0    27505 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12615 2023-07-06 20:23:59.011863 tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2.post1/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2.post1/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    11261 2023-06-07 06:14:27.599650 tungstenkit-0.1.2.post1/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      606 2023-06-01 15:06:58.874575 tungstenkit-0.1.2.post1/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2.post1/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    14054 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0     9948 2023-07-06 10:41:00.583575 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      509 2023-06-05 12:56:44.197918 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     2054 2023-06-26 07:20:09.814702 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     6213 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post1/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2379 2023-06-02 12:43:00.699193 tungstenkit-0.1.2.post1/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2.post1/tungstenkit/models.py
--rw-r--r--   0        0        0    10565 1970-01-01 00:00:00.000000 tungstenkit-0.1.2.post1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2.post3/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2.post3/README.md
+-rw-r--r--   0        0        0     2874 2023-07-10 02:22:19.778628 tungstenkit-0.1.2.post3/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2.post3/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post3/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    11227 2023-07-10 01:57:53.808984 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5656 2023-07-07 10:51:10.626393 tungstenkit-0.1.2.post3/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.2.post3/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    14393 2023-07-07 15:07:43.422886 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     9054 2023-07-07 15:54:15.126198 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1337 2023-07-06 06:51:45.833948 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1381 2023-07-06 07:14:54.727252 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
+-rw-r--r--   0        0        0     3637 2023-07-10 00:40:05.143492 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2.post3/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2.post3/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-06 20:22:25.417271 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0     6231 2023-07-06 20:22:25.381271 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/500.html
+-rw-r--r--   0        0        0      523 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js
+-rw-r--r--   0        0        0   707397 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js
+-rw-r--r--   0        0        0    78459 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
+-rw-r--r--   0        0        0   458866 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
+-rw-r--r--   0        0        0   141052 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    89842 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
+-rw-r--r--   0        0        0     5020 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
+-rw-r--r--   0        0        0     5049 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
+-rw-r--r--   0        0        0   130456 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
+-rw-r--r--   0        0        0      245 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0        0        0    28246 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js
+-rw-r--r--   0        0        0    91460 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3851 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js
+-rw-r--r--   0        0        0      791 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
+-rw-r--r--   0        0        0    43645 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
+-rw-r--r--   0        0        0   259838 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0     6242 2023-07-06 20:22:25.393271 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0    61184 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0    27505 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12615 2023-07-06 20:23:59.011863 tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2.post3/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2.post3/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    11809 2023-07-10 01:23:36.875478 tungstenkit-0.1.2.post3/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      692 2023-07-10 00:18:51.354537 tungstenkit-0.1.2.post3/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2.post3/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    15496 2023-07-10 01:42:23.372713 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2173 2023-07-10 01:38:24.239273 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/project.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     5354 2023-07-07 15:46:00.858767 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post3/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.2.post3/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2.post3/tungstenkit/models.py
+-rw-r--r--   0        0        0    10565 1970-01-01 00:00:00.000000 tungstenkit-0.1.2.post3/PKG-INFO
```

### Comparing `tungstenkit-0.1.2.post1/LICENSE` & `tungstenkit-0.1.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/README.md` & `tungstenkit-0.1.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/pyproject.toml` & `tungstenkit-0.1.2.post3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.2.post1"
+version = "0.1.2.post3"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/callbacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-import os
 import typing as t
-from pathlib import Path
 from typing import Optional
 
 from rich import print as rprint
 
 from tungstenkit import exceptions
 from tungstenkit._internal import model_store
-from tungstenkit._internal.constants import default_model_repo
 from tungstenkit._internal.utils import regex
 
 
-def project_name_callback(ctx, param, project_name: str) -> str:
+def push_target_callback(ctx, param, project_name: str) -> t.Optional[str]:
+    if not project_name:
+        return None
+
     slash_separated = project_name.split("/")
     if len(slash_separated) != 2:
         raise exceptions.InvalidName(
-            f"Invalid project name: {project_name}\nFormat: <namespace slug>/<project slug> "
-            "(e.g., exampleuser/exampleproject)"
+            f"Invalid push target: {project_name}. It should be a project name or a model name"
+            " in a project"
+            " (e.g., exampleuser/exampleproject or exampleuser/exampleproject:exampleversion)"
         )
     return project_name
 
 
 def remote_model_name_callback(ctx, param, model_name: str) -> str:
-    format_help_msg = (
-        "Format of remote model name: <namespace slug>/<project slug>:<model version>"
-    )
+    format_help_msg = "Format of remote model name: [<namespace>/]<project>[:<version>]"
     invalid_format_msg = f"Invalid remote model name: {model_name}\n" + format_help_msg
     colon_separated = model_name.split(":")
-    if len(colon_separated) != 2:
+    if len(colon_separated) > 2:
         raise exceptions.InvalidName(invalid_format_msg)
 
     full_slug = colon_separated[0]
     slash_separated = full_slug.split("/")
-    if len(slash_separated) != 2:
+    if len(slash_separated) > 2:
         raise exceptions.InvalidName(invalid_format_msg)
 
     return model_name
 
 
 def stored_model_name_callback(ctx, param, model_name: t.Optional[str]) -> str:
     """
@@ -48,32 +47,14 @@
     if model_name:
         try:
             m = model_store.get(model_name)
         except exceptions.NotFound:
             raise exceptions.NotFound(f"model '{model_name}'")
         return m.name
 
-    wd = Path(os.getcwd()).resolve().parts[-1]
-
-    try:
-        default_repo = default_model_repo()
-        rprint(
-            f"Finding the latest model image built in the directory '{wd}' "
-            f"(tag: '{default_repo}:latest')... ",
-            end="",
-        )
-
-        model_store.get(f"{default_repo}:latest")
-        rprint("[bold green]succeeded[/bold green]")
-        return f"{default_repo}:latest"
-
-    except exceptions.NotFound:
-        rprint("[bold red]failed[/bold red]")
-
-    # TODO prompt to request to ask whether to use the latest model or not
     rprint("Finding the latest model image... ", end="")
     models = sorted(model_store.list(), key=lambda m: m.created_at, reverse=True)
 
     if len(models) == 0:
         raise exceptions.NotFound("No available models. Please build or pull first.")
 
     m = models[0]
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/model_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     DEFAULT_MODEL_MODULE,
     TUNGSTEN_DIR_IN_CONTAINER,
     TUNGSTEN_LOGO,
 )
 from tungstenkit._internal.containerize import build_model
 from tungstenkit._internal.demo_server import start_demo_server
 from tungstenkit._internal.pred_interface.local_interface import LocalModel
+from tungstenkit._internal.storables import ModelData
 from tungstenkit._internal.tungsten_clients import TungstenClient
 from tungstenkit._internal.utils import docker
 from tungstenkit._internal.utils.console import print_pretty, print_success, yes_or_no_prompt
 from tungstenkit._internal.utils.string import removeprefix
 
 from .callbacks import (
     input_fields_callback,
     model_name_validator,
-    project_name_callback,
     remote_model_name_callback,
     stored_model_name_callback,
 )
 from .options import common_options
 
 
 @click.group(hidden=True)
@@ -175,14 +175,40 @@
             ]
         )
     # TODO sort table (repo_name -> latest tag first -> created)
     print(tabulate(table, headers=table_headers))
 
 
 @model.command()
+@click.argument("src", type=str, default="", callback=stored_model_name_callback)
+@click.argument("target", type=str, callback=model_name_validator)
+@common_options
+def tag(src: str, target: str, **kwargs):
+    """
+    Rename a model
+    """
+
+    m = model_store.get(src)
+    c = docker.get_docker_client()
+    img = c.images.get(m.name)
+    img.tag(target)
+    model_store.add(
+        ModelData(
+            name=target,
+            io_data=m.io,
+            avatar=m.avatar,
+            readme=m.readme,
+            source_files=m.source_files.files if m.source_files else None,
+        )
+    )
+
+    print_pretty(f"Tagged model '{src}' to '{target}'.")
+
+
+@model.command()
 @click.argument("model_name", type=str)
 @common_options
 def remove(model_name: str, **kwargs):
     """
     Remove a model
 
     'MODEL_NAME' should be in the '<repo name>[:<tag>]' format
@@ -305,41 +331,64 @@
     model_data = model_store.get(model_name)
     docker.copy_from_image(
         model_data.id, TUNGSTEN_DIR_IN_CONTAINER, Path(save_dir), image_desc=model_data.name
     )
 
 
 @model.command()
-@click.argument("project", callback=project_name_callback)
-@click.option(
-    "--model-name",
-    "-n",
-    help="Name of the model in '<repo name>[:<tag>]' format",
-    callback=stored_model_name_callback,
-)
+@click.argument("model_name", type=str, default="", callback=stored_model_name_callback)
 @common_options
-def push(project: str, model_name: str, **kwargs):
+def push(model_name: str, **kwargs):
     """
     Push a model
 
-    'PROJECT' should be in the '<namespace>/<project>' format
+    \b
+    'MODEL_NAME' should be in the '[<namespace>/]<project>:<version>' format.
+    The default value for <namespace> is the current user's username.
     """
-    # TODO validate project
-    # TODO print the pushed model in server
+    splitted_by_colon = model_name.split(":")
+    project_full_slug = splitted_by_colon[0]
+    version = splitted_by_colon[1]
+
+    splitted_by_dash = project_full_slug.split("/")
+    if len(splitted_by_dash) > 2:
+        raise click.BadArgumentUsage(f"Invalid format: {model_name}")
+
     tungsten_client = TungstenClient.from_env()
+
+    if len(splitted_by_dash) == 1:
+        project_full_slug = tungsten_client.username + "/" + project_full_slug
+
     print(TUNGSTEN_LOGO)
-    tungsten_client.push_model(model_name=model_name, project=project)
+    tungsten_client.push_model(
+        model_name=model_name, project_full_slug=project_full_slug, version=version
+    )
 
 
 @model.command()
 @click.argument("remote_model", callback=remote_model_name_callback)
 @common_options
 def pull(remote_model: str, **kwargs):
     """
     Pull a model
 
-    'REMOTE_MODEL' should be in the '<namespace>/<project>[:<version>]' format
-    """
-    project, version = remote_model.split(":", maxsplit=1)
+    \b
+    'REMOTE_MODEL' should be in the '[<namespace>/]<project>[:<version>]' format.
+    The default value for <namespace> is the current user's username.
+    If <version> is omitted, the latest version will be selected.
+    """
+    splitted_by_colon = remote_model.split(":", maxsplit=1)
+    if len(splitted_by_colon) == 2:
+        project_full_slug, version = splitted_by_colon
+    else:
+        project_full_slug = splitted_by_colon[0]
+        version = None
+
+    tungsten_client = TungstenClient.from_env()
+
+    splitted_by_dash = project_full_slug.split("/")
+    if len(splitted_by_dash) == 1:
+        project_full_slug = tungsten_client.username + "/" + project_full_slug
+
     tungsten_client = TungstenClient.from_env()
     print(TUNGSTEN_LOGO)
-    tungsten_client.pull_model(project=project, model_version=version)
+    tungsten_client.pull_model(project_full_slug=project_full_slug, model_version=version)
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,29 @@
 
 
 def _default_include_files():
     return ["*"]
 
 
 def _default_exclude_files():
-    return [".*/", "__pycache__", "*.pyc", "*.pyo", "*.pyd", ".venv", "venv", ".env", "env"]
+    return [
+        ".*/",
+        "__pycache__",
+        "*.pyc",
+        "*.pyo",
+        "*.pyd",
+        ".venv",
+        "venv",
+        ".env",
+        "env",
+        ".git*",
+        ".vscode",
+        ".*cache",
+        ".ipynb_checkpoints",
+    ]
 
 
 # TODO print warnings if there are ignored fields
 # TODO more validators (e.g., include_files)
 class BuildConfig(BaseModel):
     gpu: bool = False
     mem_gb: int = 8
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/build_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,44 +212,45 @@
     for link_path in list(abs_path_to_build_dir.rglob("*")):
         if not link_path.is_symlink():
             continue
 
         pattern = link_path.relative_to(abs_path_to_build_dir).as_posix()
         if include_spec.match_file(pattern) and not exclude_spec.match_file(pattern):
             orig_target = Path(os.readlink(str(link_path)))
+
+            if not orig_target.is_absolute():
+                continue
+
             if not orig_target.exists():
                 log_warning(f"Target of symbolic link '{link_path}' does not exist")
                 continue
 
-            if orig_target.is_absolute():
-                try:
-                    orig_target.relative_to(abs_path_to_build_dir)
-                except ValueError:
-                    raise exceptions.BuildError(
-                        f"Target '{orig_target}' of link '{link_path}' is outside build dir at "
-                        f"'{abs_path_to_build_dir}'"
-                    )
-                tmp_link_path = (
-                    abs_path_to_build_dir
-                    / rel_path_to_tmp_dir
-                    / "symlinks"
-                    / link_path.relative_to(abs_path_to_build_dir)
-                )
-                new_target = os.path.relpath(orig_target, start=tmp_link_path)
-                tmp_link_path.parent.mkdir(parents=True, exist_ok=True)
-                os.symlink(new_target, tmp_link_path)
-                log_debug(
-                    f"Change target of link '{link_path}': '{orig_target}' -> '{new_target}'"
+            try:
+                orig_target.relative_to(abs_path_to_build_dir)
+            except ValueError:
+                raise exceptions.BuildError(
+                    f"Target '{orig_target}' of link '{link_path}' is outside build dir at "
+                    f"'{abs_path_to_build_dir}'"
                 )
-                link_and_target_pairs.append(
-                    (
-                        str(tmp_link_path),
-                        link_path.relative_to(abs_path_to_build_dir).as_posix(),
-                    )
+            tmp_link_path = (
+                abs_path_to_build_dir
+                / rel_path_to_tmp_dir
+                / "symlinks"
+                / link_path.relative_to(abs_path_to_build_dir)
+            )
+            new_target = os.path.relpath(orig_target, start=tmp_link_path)
+            tmp_link_path.parent.mkdir(parents=True, exist_ok=True)
+            os.symlink(new_target, tmp_link_path)
+            log_debug(f"Change target of link '{link_path}': '{orig_target}' -> '{new_target}'")
+            link_and_target_pairs.append(
+                (
+                    str(tmp_link_path),
+                    link_path.relative_to(abs_path_to_build_dir).as_posix(),
                 )
+            )
 
     return link_and_target_pairs
 
 
 def _copy_files(
     abs_path_to_build_dir: Path,
     rel_path_to_tmp_dir: Path,
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         If there is no large files, returns ``None``.
         """
         include_spec = PathSpec.from_lines("gitwildmatch", self.config.include_files)
         exclude_spec = PathSpec.from_lines(
             "gitwildmatch", self.config.exclude_files + [tmp_dir_in_build_ctx.as_posix()]
         )
 
-        def split(curr_dir: Path):
+        def split(curr_dir: Path) -> t.Tuple[t.List[Path], t.List[Path]]:
             large_files, small_files = [], []
             for path in curr_dir.iterdir():
                 if not include_spec.match_file(path.as_posix()) or exclude_spec.match_file(
                     path.as_posix()
                 ):
                     continue
 
@@ -198,13 +198,32 @@
                         small_files.append(path)
 
             if len(large_files) == 0:
                 return [], [curr_dir]
 
             return large_files, small_files
 
-        return split(curr_dir)
+        large_files, small_files = split(curr_dir)
+        large_files = sorted(
+            large_files,
+            key=lambda path: (_get_size_of_copy_target(path), path.name),
+            reverse=True,
+        )
+        small_files = sorted(
+            small_files,
+            key=lambda path: (_get_size_of_copy_target(path), path.name),
+            reverse=True,
+        )
+        return large_files, small_files
 
     @classmethod
     @abc.abstractmethod
     def python_entrypoint(cls) -> str:
         pass
+
+
+def _get_size_of_copy_target(path: Path):
+    if path.is_dir():
+        size = sum(f.stat().st_size for f in path.glob("**/*") if f.is_file())
+    else:
+        size = path.stat(follow_symlinks=False).st_size
+    return size
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/template_args.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
                 id = None
                 if tag is None:
                     tag = storables.ModelData.generate_id()
                     id = tag
                 model_name = f"{repo_name}:{tag}"
 
                 # Build
-                tags = [model_name] if tag == "latest" else [model_name, f"{repo_name}:latest"]
-                build_ctx.build(tags=tags)
+                names = [model_name] if tag == "latest" else [model_name, f"{repo_name}:latest"]
+                build_ctx.build(tags=names)
 
                 # Add to the local store
                 io_schema = storables.ModelIOData(
                     input_schema=input_schema,
                     output_schema=output_schema,
                     demo_output_schema=demo_output_schema,
                     input_filetypes=model_config.input_filetypes,
@@ -66,17 +66,19 @@
                     demo_output_filetypes=model_config.demo_output_filetypes,
                 )
                 avatar = storables.AvatarData.fetch_default(hash_key=model_name)
                 if model_config.readme_md:
                     readme = storables.MarkdownData.from_path(model_config.readme_md)
                 else:
                     readme = None
-                model_data = storables.ModelData(
-                    name=model_name,
-                    io_data=io_schema,
-                    avatar=avatar,
-                    readme=readme,
-                    id=id,
-                    source_files=build_ctx.walk_fs(),
-                )
+
+                for name in names:
+                    model_data = storables.ModelData(
+                        name=name,
+                        io_data=io_schema,
+                        avatar=avatar,
+                        readme=readme,
+                        id=id,
+                        source_files=build_ctx.walk_fs(),
+                    )
                 model_data.save()
                 return storables.ModelData.load(model_name)
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/500.html` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/500.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/io.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/json_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import typing as t
+from datetime import datetime
 from pathlib import Path
 from uuid import uuid4
 
 import attrs
 import cattrs
 from filelock import FileLock
 
@@ -26,15 +27,14 @@
 
     def save(self, file_blob_create_policy: FileBlobCreatePolicy = "copy") -> ItemType:
         blob_store = BlobStore()
         with blob_store.prevent_deletion():
             data = self.save_blobs(blob_store, file_blob_create_policy)
             store = self._get_store()
             store.add(data)
-            store.tag(data.name, data.repo_name + ":latest")
         return data
 
     @classmethod
     def load(cls: t.Type[StorableType], name: str) -> StorableType:
         data = cls._get_store().get(name)
         return cls.load_blobs(data)
 
@@ -79,14 +79,19 @@
     def blobs(self) -> t.Set[Blob]:
         pass
 
     @property
     def name(self) -> str:
         return self.repo_name + ":" + self.tag
 
+    @property
+    @abc.abstractmethod
+    def created_at(self) -> datetime:
+        pass
+
     @abc.abstractmethod
     def cleanup(self):
         pass
 
     @staticmethod
     @abc.abstractmethod
     def parse_name(name: str) -> t.Tuple[str, str]:
@@ -125,14 +130,16 @@
         """Add to the colleciton and prune dangling items"""
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
             col.add(item)
             self._gc(col)
             col.save(self.collection_path)
 
+    # def get_latest_tag(self, repo: str):
+
     def tag(self, src_name: str, dest_name: str):
         src_repo, src_tag = self._item_type.parse_name(src_name)
         dest_repo, dest_tag = self._item_type.parse_name(dest_name)
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
             src = col.get_by_tag(src_repo, src_tag)
             if src is None:
@@ -261,20 +268,27 @@
 
     def get_by_id(self, id: str) -> t.Optional[ItemType]:
         if id not in self.items:
             return None
         return self.items[id]
 
     def list(self) -> t.List[t.Tuple[str, str, ItemType]]:
-        ret = []
+        ret: t.List[t.Tuple[str, str, ItemType]] = []
         for repo_name in self.repositories.keys():
             for tag, id in self.repositories[repo_name].items():
                 item = self.items[id]
                 ret.append((repo_name, tag, item))
-        return ret
+        return sorted(ret, key=lambda val: (val[0], datetime.utcnow() - val[2].created_at))
+
+    def list_in_repo(self, repo_name: str) -> t.List[t.Tuple[str, ItemType]]:
+        ret: t.List[t.Tuple[str, ItemType]] = []
+        for tag, id in self.repositories[repo_name].items():
+            item = self.items[id]
+            ret.append((tag, item))
+        return sorted(ret, key=lambda val: val[1].created_at, reverse=True)
 
     def prune(
         self, candidate_ids: t.Optional[t.Iterable[str]] = None
     ) -> t.List[t.Tuple[str, ItemType]]:
         if candidate_ids is None:
             candidate_ids = [id for id in self.items.keys()]
         else:
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/model_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 from tungstenkit._internal.json_store import JSONCollection
 from tungstenkit._internal.storables.model_data import ModelData, StoredModelData
 
 _store = JSONCollection[StoredModelData](StoredModelData)
 
 
+def add(model: ModelData) -> None:
+    stored = model.save()
+    _store.add(stored)
+
+
 def get(name: str) -> ModelData:
     stored = _store.get(name)
     return ModelData.load_blobs(stored)
 
 
 def list() -> t.List[ModelData]:
     stored = _store.list()
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/avatar_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/model_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/storables/source_file_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/task.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,84 +63,113 @@
         f = furl(self.base_url)
         f.path = f.path / API_BASE_STR / "user"
         log_request(url=f.url, method="GET")
         resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
         _check_resp(resp, f.url, "Failed to fetch user info")
         return schemas.User.parse_raw(resp.text)
 
-    def check_if_project_exists(self, project: str) -> bool:
+    def get_project(self, project_full_slug: str) -> t.Optional[schemas.Project]:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug
         log_request(url=f.url, method="GET")
         resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
         if resp.status_code == 404:
-            return False
+            return None
 
-        _check_resp(resp, f.url, f"Failed to check existence of project '{project}'")
-        return True
+        _check_resp(resp, f.url, f"Project not found: '{project_full_slug}'")
+        return schemas.Project.parse_raw(resp.text)
 
-    def get_project_avatar(self, project: str) -> storables.AvatarData:
-        f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "avatar"
-        log_request(url=f.url, method="GET")
-        resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
+    def fetch_project_avatar(
+        self, project_full_slug: str, avatar_url: str
+    ) -> storables.AvatarData:
+        log_request(url=avatar_url, method="GET")
+        resp = self.sess.get(avatar_url, timeout=CONNECTION_TINEOUT)
         if resp.status_code == 404:
-            return storables.AvatarData.fetch_default(project + " avatar", avatar_domain=f.host)
+            return storables.AvatarData.fetch_default(
+                project_full_slug + " avatar", avatar_domain=self.base_url
+            )
 
-        _check_resp(resp, f.url, f"Failed to fetch the avatar of project '{project}'")
+        _check_resp(
+            resp, avatar_url, f"Failed to fetch the avatar of project '{project_full_slug}'"
+        )
         return storables.AvatarData(bytes_=resp.content, extension=".png")
 
-    def get_model(self, project: str, version: str) -> schemas.Model:
+    def get_model(self, project_full_slug: str, version: str) -> schemas.Model:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models" / version
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug / "models" / version
         log_request(url=f.url, method="GET")
         resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
-        _check_resp(resp, f.url, f"Failed to fetch info of model '{project}:{version}'")
+        _check_resp(resp, f.url, f"Failed to fetch info of model '{project_full_slug}:{version}'")
         return schemas.Model.parse_raw(resp.text)
 
-    def create_model(self, project: str, req: schemas.ModelCreate) -> schemas.Model:
+    def get_latest_model(self, project_full_slug: str) -> t.Optional[schemas.Model]:
+        f = furl(self.base_url)
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug / "models"
+        f.args["per_page"] = str(1)
+        f.args["page"] = str(1)
+        f.args["order_by"] = "created_at"
+        f.args["sort"] = "desc"
+        log_request(url=f.url, method="GET")
+        resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
+        _check_resp(resp, f.url, f"Failed to fetch model list in project '{project_full_slug}'")
+        model_list = schemas.ModelList.parse_raw(resp.text)
+        if len(model_list.__root__) == 0:
+            return None
+        return model_list.__root__[0]
+
+    def create_model(self, project_full_slug: str, req: schemas.ModelCreate) -> schemas.Model:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models"
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug / "models"
         data = req.json()
         log_request(url=f.url, method="POST", data=data)
         resp = self.sess.post(f.url, data=data, timeout=CONNECTION_TINEOUT)
-        _check_resp(resp, f.url, f"Failed to create a model in project '{project}'")
+        _check_resp(resp, f.url, f"Failed to create a model in project '{project_full_slug}'")
         return schemas.Model.parse_raw(resp.text)
 
     def update_model_readme(
-        self, project: str, version: str, readme: storables.MarkdownData
+        self, project_full_slug: str, version: str, readme: storables.MarkdownData
     ) -> None:
         if len(readme.image_files) > 0:
             resps = self.upload_multiple_files_by_paths(
-                project=project, paths=readme.image_files, desc="Uploading image files in README"
+                project_full_slug=project_full_slug,
+                paths=readme.image_files,
+                desc="Uploading image files in README",
             )
             image_file_serving_urls = [r.serving_url for r in resps]
             readme_content = change_local_image_links_in_markdown(
                 md=readme.content,
                 local_img_paths=readme.image_files,
                 updates=image_file_serving_urls,
             )
 
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models" / version / "readme"
+        f.path = (
+            f.path / API_BASE_STR / "projects" / project_full_slug / "models" / version / "readme"
+        )
         log_request(url=f.url, method="PUT")
         data = schemas.ModelReadmeUpdate(content=readme_content).json()
         resp = self.sess.put(f.url, data=data, timeout=CONNECTION_TINEOUT)
         _check_resp(
-            resp, url=f.url, err_msg_prefix=f"Failed to upload README of model {project}:{version}"
+            resp,
+            url=f.url,
+            err_msg_prefix=f"Failed to upload README of model {project_full_slug}:{version}",
         )
 
     def get_model_readme(
-        self, project: str, version: str, image_download_dir: Path
+        self, project_full_slug: str, version: str, image_download_dir: Path
     ) -> storables.MarkdownData:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models" / version / "readme"
+        f.path = (
+            f.path / API_BASE_STR / "projects" / project_full_slug / "models" / version / "readme"
+        )
         log_request(url=f.url, method="GET")
         resp = self.sess.get(url=f.url, timeout=CONNECTION_TINEOUT)
-        _check_resp(resp, f.url, f"Failed to get the README of model {project}:{version}")
+        _check_resp(
+            resp, f.url, f"Failed to get the README of model {project_full_slug}:{version}"
+        )
 
         md = resp.text
         image_http_links = get_image_links(md, schemes=["http", "https"])
         if len(image_http_links) > 0:
             downloaded = self.download_multiple_files(
                 image_http_links,
                 out=image_download_dir,
@@ -148,43 +177,49 @@
             )
             md = change_img_links_in_markdown(
                 md, images=image_http_links, updates=[p.as_uri() for p in downloaded]
             )
             return storables.MarkdownData(content=md, image_files=downloaded)
         return storables.MarkdownData(content=md)
 
-    def get_model_source_tree(self, project: str, version: str) -> schemas.SourceTreeFolder:
+    def get_model_source_tree(
+        self, project_full_slug: str, version: str
+    ) -> schemas.SourceTreeFolder:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models" / version / "tree"
+        f.path = (
+            f.path / API_BASE_STR / "projects" / project_full_slug / "models" / version / "tree"
+        )
         log_request(url=f.url, method="GET")
         resp = self.sess.get(f.url, timeout=CONNECTION_TINEOUT)
         _check_resp(
             resp,
             url=f.url,
-            err_msg_prefix=f"Failed to get the source tree of model {project}:{version}",
+            err_msg_prefix=f"Failed to get the source tree of model {project_full_slug}:{version}",
         )
         parsed = schemas.SourceTreeFolder.parse_raw(resp.text)
         return parsed
 
     def download_model_source_file(
-        self, project: str, version: str, path: str, root_dir: Path
+        self, project_full_slug: str, version: str, path: str, root_dir: Path
     ) -> Path:
         download_dir = (root_dir / path).parent
         download_dir.mkdir(exist_ok=True, parents=True)
 
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "models" / version / "files"
+        f.path = (
+            f.path / API_BASE_STR / "projects" / project_full_slug / "models" / version / "files"
+        )
         f.path.segments += [path]  # For url encoding
         log_request(url=f.url, method="GET")
         return download_file(url=f.url, out_path=download_dir, sess=self.sess)
 
     def download_model_source_tree(
-        self, project: str, version: str, root_dir: Path
+        self, project_full_slug: str, version: str, root_dir: Path
     ) -> t.List[storables.SourceFile]:
-        root = self.get_model_source_tree(project=project, version=version)
+        root = self.get_model_source_tree(project_full_slug=project_full_slug, version=version)
         urls: t.List[str] = []
         download_paths: t.List[Path] = []
         ret: t.List[storables.SourceFile] = []
 
         def _add(path: t.Optional[PurePosixPath], folder: schemas.SourceTreeFolder):
             contents = folder.contents
             for c in contents:
@@ -194,15 +229,17 @@
                         downloaded = None
                     else:
                         if path is None:
                             downloaded = root_dir / c.name
                         else:
                             downloaded = root_dir / path / c.name
 
-                        urls.append(self._build_source_file_url(project, version, str(p)))
+                        urls.append(
+                            self._build_source_file_url(project_full_slug, version, str(p))
+                        )
                         download_paths.append(downloaded)
 
                     ret.append(
                         storables.SourceFile(
                             rel_path_in_model_fs=p,
                             abs_path_in_host_fs=downloaded,
                             size=c.size,
@@ -212,20 +249,22 @@
                     _add(p, c)
 
         _add(None, root)
         self.download_multiple_files(urls, download_paths)
         return ret
 
     def upload_model_source_files(
-        self, project: str, files: t.Iterable[storables.SourceFile]
+        self, project_full_slug: str, files: t.Iterable[storables.SourceFile]
     ) -> t.Tuple[t.List[schemas.SourceFileDecl], t.List[schemas.SkippedSourceFileDecl]]:
         source_files, skipped_source_files = [], []
         upload_path_dict = {f: f.abs_path_in_host_fs for f in files if f.abs_path_in_host_fs}
         upload_resps = self.upload_multiple_files_by_paths(
-            project=project, paths=list(upload_path_dict.values()), desc="Uploading source files"
+            project_full_slug=project_full_slug,
+            paths=list(upload_path_dict.values()),
+            desc="Uploading source files",
         )
         upload_resp_dict = {f: url for f, url in zip(upload_path_dict.keys(), upload_resps)}
         for f in files:
             p = str(f.rel_path_in_model_fs)
             if f in upload_resp_dict:
                 source_files.append(
                     schemas.SourceFileDecl(path=p, upload_id=upload_resp_dict[f].id)
@@ -243,16 +282,18 @@
         _check_resp(
             resp,
             f.url,
             err_msg_prefix="Failed to get metadata of the tungsten instance",
         )
         return schemas.ServerMetadata.parse_raw(resp.text)
 
-    def upload_file_by_path(self, project: str, path: Path, desc: t.Optional[str] = None) -> str:
-        url = self.build_upload_url(project=project)
+    def upload_file_by_path(
+        self, project_full_slug: str, path: Path, desc: t.Optional[str] = None
+    ) -> str:
+        url = self.build_upload_url(project_full_slug=project_full_slug)
         log_request(url=url, method="POST")
         resp = upload_form_data_by_path(
             method="post",
             url=url,
             file_path=path,
             field="file",
             sess=self.sess,
@@ -261,21 +302,21 @@
         )
         _check_resp(resp, url, f"Failed to upload file '{path}'")
         parsed = schemas.FileUploadResponse.parse_raw(resp.text)
         return parsed.serving_url
 
     def upload_file_by_buffer(
         self,
-        project: str,
+        project_full_slug: str,
         buffer: io.BufferedIOBase,
         file_name: str,
         content_type: str,
         desc: t.Optional[str] = None,
     ) -> str:
-        url = self.build_upload_url(project=project)
+        url = self.build_upload_url(project_full_slug=project_full_slug)
         log_request(url=url, method="POST")
         resp = upload_form_data_by_buffer(
             method="post",
             url=url,
             buffer=buffer,
             file_name=file_name,
             content_type=content_type,
@@ -285,21 +326,21 @@
             desc=desc,
         )
         _check_resp(resp, url, f"Failed to upload file '{file_name}'")
         parsed = schemas.FileUploadResponse.parse_raw(resp.text)
         return parsed.serving_url
 
     def upload_multiple_files_by_paths(
-        self, project: str, paths: t.List[Path], desc: t.Optional[str] = None
+        self, project_full_slug: str, paths: t.List[Path], desc: t.Optional[str] = None
     ) -> t.List[schemas.FileUploadResponse]:
         if len(paths) == 0:
             return []
 
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "uploads"
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug / "uploads"
         log_request(url=f.url, method="POST")
         responses = upload_multiple_form_data_by_paths(
             method="post",
             url=f.url,
             file_paths=paths,
             field="file",
             sess=self.sess,
@@ -333,17 +374,17 @@
         progress_bar: bool = True,
         desc: t.Optional[str] = None,
     ) -> t.List[Path]:
         return download_files_in_threadpool(
             *urls, out=out, sess=self.sess, progress_bar=progress_bar, desc=desc
         )
 
-    def build_upload_url(self, project: str) -> str:
+    def build_upload_url(self, project_full_slug: str) -> str:
         f = furl(self.base_url)
-        f.path = f.path / API_BASE_STR / "projects" / project / "uploads"
+        f.path = f.path / API_BASE_STR / "projects" / project_full_slug / "uploads"
         return f.url
 
     def _set_auth_header(self, access_token: str):
         self.sess.headers.update(Authorization="Bearer " + access_token)
 
     def _build_source_file_url(self, project: str, version: str, path: str) -> str:
         f = furl(self.base_url)
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,31 @@
         if self._server_metadata is None:
             self._server_metadata = self.api.get_server_metadata()
         return strip_scheme_in_http_url(self._server_metadata.registry_url)
 
     def push_model(
         self,
         model_name: str,
-        project: str,
+        project_full_slug: str,
+        version: t.Optional[str] = None,
     ) -> schemas.Model:
-        if not self.api.check_if_project_exists(project):
-            raise exceptions.NotFound(f"No project '{project}' in {self.api.base_url}")
+        project_in_server = self.api.get_project(project_full_slug)
+        if project_in_server is None:
+            raise exceptions.NotFound(f"No project '{project_full_slug}' in {self.api.base_url}")
+
+        if version:
+            try:
+                self.api.get_model(project_full_slug, version)
+                raise exceptions.Conflict(
+                    f"Version '{version}' already exists in project '{project_full_slug}'. "
+                    "Please retry after removing the model."
+                )
+            except exceptions.TungstenClientError as e:
+                if e.status_code != 404:
+                    raise e
 
         model = storables.ModelData.load(model_name)
         docker_image_id = model.docker_image_id
 
         docker_client = get_docker_client(timeout=DOCKER_CLIENT_TIMEOUT)
         docker_image: DockerImage = docker_client.images.get(docker_image_id)
 
@@ -105,19 +118,20 @@
                 input_schema=model.io.input_schema,
                 output_schema=model.io.output_schema,
                 demo_output_schema=model.io.demo_output_schema,
                 input_filetypes=model.io.input_filetypes,
                 output_filetypes=model.io.output_filetypes,
                 demo_output_filetypes=model.io.demo_output_filetypes,
                 gpu_memory=model.gpu_mem_gb * 1024 * 1024 if model.gpu and model.gpu_mem_gb else 0,
+                version=version,
                 # source_files=source_files,
                 # skipped_source_files=skipped_source_files,
             )
 
-            model_in_server = self.api.create_model(project=project, req=req)
+            model_in_server = self.api.create_model(project_full_slug=project_full_slug, req=req)
             log_debug("Response: " + str(model_in_server), pretty=False)
 
             # if model.readme:
             #     log_info("Updating the README")
             #     self.api.update_model_readme(
             #         project=project, version=model_in_server.version, readme=model.readme
             #     )
@@ -125,31 +139,49 @@
 
         finally:
             docker_client.images.remove(image=f"{remote_docker_repo}:{remote_docker_tag}")
 
         log_info("")
         print_success(
             f"Successfully pushed '{model.name}' to '{self.api.base_url}'\n"
-            f" - project: [green]{project}[/green]\n"
+            f" - project: [green]{project_full_slug}[/green]\n"
             f" - version: [green]{model_in_server.version}[/green]"
         )
         return model_in_server
 
-    def pull_model(self, project: str, model_version: str) -> storables.ModelData:
-        if not self.api.check_if_project_exists(project):
-            raise exceptions.NotFound(f"No project '{project}' in {self.api.base_url}")
+    def pull_model(
+        self, project_full_slug: str, model_version: t.Optional[str] = None
+    ) -> storables.ModelData:
+        project_in_server = self.api.get_project(project_full_slug)
+        if project_in_server is None:
+            raise exceptions.NotFound(f"No project '{project_full_slug}' in {self.api.base_url}")
+
+        if model_version:
+            model_in_server = self.api.get_model(
+                project_full_slug=project_full_slug, version=model_version
+            )
+        else:
+            latest_model = self.api.get_latest_model(project_full_slug=project_full_slug)
+            if latest_model is None:
+                raise exceptions.NotFound(f"No model in project '{project_full_slug}'")
+            model_in_server = latest_model
+            model_version = model_in_server.version
 
-        model_in_server = self.api.get_model(project=project, version=model_version)
         repo_name, tag = model_in_server.docker_image.split(":", maxsplit=1)
         remote_docker_repo = f"{self.docker_registry}/{repo_name}"
-        local_model_name = f"{remote_docker_repo}:{tag}"
+        local_model_name = f"{project_full_slug}:{model_version}"
 
         docker_client = get_docker_client(timeout=DOCKER_CLIENT_TIMEOUT)
         log_info("Pulling the model image")
         self._pull_from_docker_registry(remote_docker_repo, tag, docker_client=docker_client)
+
+        image = docker_client.images.get(remote_docker_repo + ":" + tag)
+        image.tag(project_full_slug, model_version)
+        docker_client.images.remove(remote_docker_repo + ":" + tag)
+
         with tempfile.TemporaryDirectory() as tmp_dir_str:
             tmp_dir = Path(tmp_dir_str)
 
             # if model_in_server.readme_url:
             #     readme_image_dir = tmp_dir / "readme_images"
             #     readme_image_dir.mkdir()
             #     log_info("Fetching the README")
@@ -168,15 +200,15 @@
             #         project=project, version=model_version, root_dir=source_files_dir
             #     )
             # else:
             #     source_files = []
 
             readme, source_files = None, []
 
-            avatar = self.api.get_project_avatar(project=project)
+            avatar = self.api.fetch_project_avatar(project_full_slug, project_in_server.avatar_url)
             io_data = storables.ModelIOData(
                 input_schema=model_in_server.input_schema,
                 output_schema=model_in_server.output_schema,
                 demo_output_schema=model_in_server.demo_output_schema,
                 input_filetypes=model_in_server.input_filetypes,
                 output_filetypes=model_in_server.output_filetypes,
                 demo_output_filetypes=model_in_server.demo_output_filetypes,
@@ -187,15 +219,15 @@
                 avatar=avatar,
                 readme=readme,
                 source_files=source_files,
             )
             m.save(file_blob_create_policy="rename")
 
             log_info("")
-            print_success(f"Successfully pulled '{remote_docker_repo}:{tag}'")
+            print_success(f"Successfully pulled '{project_full_slug}:{model_version}'")
             return storables.ModelData.load(local_model_name)
 
     def _push_to_docker_registry(self, repo: str, tag: str, docker_client: DockerClient):
         result = push_to_docker_registry(repo=repo, tag=tag, docker_client=docker_client)
 
         if not result.is_success and result.failure_reason == PullPushFailureReason.UNAUTHORIZED:
             auth_config = _input_auth(
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     output_filetypes: dict
     demo_output_filetypes: dict
 
     source_files: List[SourceFileDecl] = Field(default_factory=list)
     skipped_source_files: List[SkippedSourceFileDecl] = Field(default_factory=list)
 
     gpu_memory: int
+    vm: Optional[str] = None
+    version: Optional[str] = None
 
 
 class ModelCreator(BaseModel):
     id: int
     username: str
     name: str
     avatar_url: str
@@ -67,14 +69,18 @@
     source_files_count: int
     examples_count: int
 
     creator: ModelCreator
     created_at: datetime
 
 
+class ModelList(BaseModel):
+    __root__: List[Model]
+
+
 class ModelReadmeUpdate(BaseModel):
     content: str
 
 
 class ModelPredictionExampleCreate(BaseModel):
     input: dict
     output: dict
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/imports.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,42 +82,26 @@
 
 
 class UnknownModuleFinder(importlib.abc.MetaPathFinder):
     def __init__(self, loader: "UnknownModuleLazyLoader"):
         self._loader = loader
 
     def find_spec(self, fullname, path, target=None):
-        if self._loader.is_registered(fullname):
-            return self._gen_spec(fullname)
-
-    def _gen_spec(self, fullname):
         spec = importlib.machinery.ModuleSpec(fullname, self._loader)
         return spec
 
 
 class UnknownModuleLazyLoader(importlib.abc.Loader):
     def __init__(self, help_msg_on_err: Optional[str] = None):
         self._help_msg_on_err = help_msg_on_err
         self._registered: Dict[str, UnknownModule] = dict()
 
-    def register(self, fullname: str, module_attr: Optional[str] = None):
-        dot_separated = fullname.split(".")
-        for i in range(len(dot_separated)):
-            name = ".".join(dot_separated[: i + 1])
-            if importlib.util.find_spec(name) is None:
-                self._registered[name] = UnknownModule(name, self._help_msg_on_err)
-        if fullname in self._registered and module_attr:
-            self._registered[fullname]._add(module_attr)
-
-    def is_registered(self, fullname: str):
-        return fullname in self._registered
-
     def create_module(self, spec):
-        if spec.name in self._registered:
-            return self._registered[spec.name]
+        self._registered[spec.name] = UnknownModule(spec.name, self._help_msg_on_err)
+        return self._registered[spec.name]
 
     def exec_module(self, module):
         pass
 
 
 def get_imports(path):
     """
@@ -156,25 +140,19 @@
             continue
 
         for n in node.names:
             yield Import(module, n.name.split("."), n.asname)
 
 
 @contextmanager
-def lazy_import_ctx(imports: List[Import], help_msg_on_err: Optional[str] = None):
+def lazy_import_ctx(help_msg_on_err: Optional[str] = None):
     loader = UnknownModuleLazyLoader(help_msg_on_err)
     finder = UnknownModuleFinder(loader)
     try:
         sys.meta_path.append(finder)
-        for imp in imports:
-            if imp.module:
-                attr_name = ".".join(imp.name)
-                loader.register(".".join(imp.module), attr_name if attr_name else None)
-            else:
-                loader.register(".".join(imp.name))
         yield
     finally:
         for module_name in loader._registered.keys():
             if module_name in sys.modules:
                 del sys.modules[module_name]
         sys.meta_path.remove(finder)
 
@@ -187,18 +165,21 @@
     spec = importlib.util.find_spec(module)
     if spec is None:
         raise ModuleNotFoundError(module)
     if spec.origin is None:
         raise ModuleNotFoundError(
             f"Failed to initialize module '{module}'. Is it a Python module?"
         )
-    imports = get_imports(spec.origin)
-    with lazy_import_ctx(imports, help_msg_on_unknown_module_exec):
+    try:
         mod = importlib.import_module(module)
         return mod
+    except ModuleNotFoundError:
+        with lazy_import_ctx(help_msg_on_unknown_module_exec):
+            mod = importlib.import_module(module)
+            return mod
 
 
 def check_module(module: str) -> bool:
     try:
         spec = importlib.util.find_spec(module)
         return spec is not None and spec.origin is not None
     except ModuleNotFoundError:
```

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/types.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.2.post3/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post1/tungstenkit/exceptions.py` & `tungstenkit-0.1.2.post3/tungstenkit/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     pass
 
 
 class UploadError(TungstenException):
     pass
 
 
+class Conflict(TungstenException):
+    pass
+
+
 class BuildError(TungstenException):
     pass
 
 
 class InvalidOutput(TungstenException):
     pass
```

### Comparing `tungstenkit-0.1.2.post1/PKG-INFO` & `tungstenkit-0.1.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.2.post1
+Version: 0.1.2.post3
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

