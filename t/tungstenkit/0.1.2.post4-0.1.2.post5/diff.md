# Comparing `tmp/tungstenkit-0.1.2.post4.tar.gz` & `tmp/tungstenkit-0.1.2.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.2.post4.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.2.post5.tar", max compression
```

## Comparing `tungstenkit-0.1.2.post4.tar` & `tungstenkit-0.1.2.post5.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2.post4/LICENSE
--rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2.post4/README.md
--rw-r--r--   0        0        0     2874 2023-07-10 02:28:05.117525 tungstenkit-0.1.2.post4/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2.post4/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post4/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0    11227 2023-07-10 01:57:53.808984 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5656 2023-07-07 10:51:10.626393 tungstenkit-0.1.2.post4/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2471 2023-06-05 07:47:33.325628 tungstenkit-0.1.2.post4/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    14393 2023-07-07 15:07:43.422886 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     9054 2023-07-07 15:54:15.126198 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1337 2023-07-06 06:51:45.833948 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1381 2023-07-06 07:14:54.727252 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
--rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2.post4/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2.post4/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-06 20:22:25.417271 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0     6231 2023-07-06 20:22:25.381271 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/500.html
--rw-r--r--   0        0        0      523 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js
--rw-r--r--   0        0        0   707397 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js
--rw-r--r--   0        0        0    78459 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
--rw-r--r--   0        0        0   458866 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
--rw-r--r--   0        0        0   141052 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    89842 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
--rw-r--r--   0        0        0     5020 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
--rw-r--r--   0        0        0     5049 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
--rw-r--r--   0        0        0   130456 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
--rw-r--r--   0        0        0      245 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0        0        0    28246 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js
--rw-r--r--   0        0        0    91460 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3851 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js
--rw-r--r--   0        0        0      791 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
--rw-r--r--   0        0        0    43645 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
--rw-r--r--   0        0        0   259838 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0     6242 2023-07-06 20:22:25.393271 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0    61184 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0    27505 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12615 2023-07-06 20:23:59.011863 tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2.post4/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2.post4/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    11809 2023-07-10 01:23:36.875478 tungstenkit-0.1.2.post4/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      692 2023-07-10 00:18:51.354537 tungstenkit-0.1.2.post4/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2.post4/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    15496 2023-07-10 01:42:23.372713 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     2173 2023-07-10 01:38:24.239273 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/project.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     5354 2023-07-07 15:46:00.858767 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post4/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.2.post4/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2.post4/tungstenkit/models.py
--rw-r--r--   0        0        0    10565 1970-01-01 00:00:00.000000 tungstenkit-0.1.2.post4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2.post5/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2.post5/README.md
+-rw-r--r--   0        0        0     2869 2023-07-10 07:05:13.701460 tungstenkit-0.1.2.post5/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2.post5/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post5/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    11183 2023-07-10 07:03:19.249951 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5656 2023-07-07 10:51:10.626393 tungstenkit-0.1.2.post5/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2471 2023-07-10 07:04:01.709772 tungstenkit-0.1.2.post5/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    13013 2023-07-10 07:02:50.614069 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     8942 2023-07-10 07:00:49.982540 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1174 2023-07-10 07:01:04.282487 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1149 2023-07-10 06:59:55.446738 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0      149 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     3757 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt
+-rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2.post5/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2.post5/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-06 20:22:25.417271 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0     6231 2023-07-06 20:22:25.381271 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/500.html
+-rw-r--r--   0        0        0      523 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_ssgManifest.js
+-rw-r--r--   0        0        0   707397 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js
+-rw-r--r--   0        0        0    78459 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
+-rw-r--r--   0        0        0   458866 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
+-rw-r--r--   0        0        0   141052 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    89842 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
+-rw-r--r--   0        0        0     5020 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
+-rw-r--r--   0        0        0     5049 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
+-rw-r--r--   0        0        0   130456 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
+-rw-r--r--   0        0        0      245 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0        0        0    28246 2023-07-06 20:22:25.037277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js
+-rw-r--r--   0        0        0    91460 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3851 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js
+-rw-r--r--   0        0        0      791 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
+-rw-r--r--   0        0        0    43645 2023-07-06 20:22:25.033277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
+-rw-r--r--   0        0        0   259838 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0     6242 2023-07-06 20:22:25.393271 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0    61184 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0    27505 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-07-06 20:22:25.041277 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0     2521 2023-07-06 10:20:26.771091 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12615 2023-07-06 20:23:59.011863 tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2.post5/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2.post5/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    11809 2023-07-10 01:23:36.875478 tungstenkit-0.1.2.post5/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3961 2023-05-29 11:48:58.538763 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      558 2023-05-26 09:51:05.829376 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1819 2023-06-07 07:58:21.892954 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9883 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      692 2023-07-10 00:18:51.354537 tungstenkit-0.1.2.post5/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5211 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2.post5/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    15496 2023-07-10 01:42:23.372713 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2149 2023-07-10 07:01:26.786401 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/project.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18703 2023-06-05 06:47:01.765782 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     5354 2023-07-10 06:15:33.654911 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post5/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.2.post5/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2.post5/tungstenkit/models.py
+-rw-r--r--   0        0        0    10565 1970-01-01 00:00:00.000000 tungstenkit-0.1.2.post5/PKG-INFO
```

### Comparing `tungstenkit-0.1.2.post4/LICENSE` & `tungstenkit-0.1.2.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/README.md` & `tungstenkit-0.1.2.post5/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/pyproject.toml` & `tungstenkit-0.1.2.post5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.2.post4"
+version = "0.1.2.post5"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -40,15 +40,15 @@
 [tool.poetry.scripts]
 tungsten = "tungstenkit._internal.cli.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 attrs = "^22.1.0"
 cattrs = "^22.1.0"
-pyyaml = "^6.0"
+pyyaml = "^5.4"
 pathspec = "^0.10.2"
 loguru = ">=0.6.0, <1.0.0"
 requests = "^2.28.1"
 beautifulsoup4 = "^4.11.1"
 jinja2 = "^3.1.2"
 pydantic = "^1.10.2"
 typing-extensions = "^4.4.0"
@@ -76,15 +76,15 @@
 mypy = "^1.1"
 black = "^22.3.0"
 isort = "^4.3.21"
 autoflake = "^1.3.1"
 flake8 = "^3.7.9"
 pytest = "^7.1.3"
 pytest-cov = "^2.8.1"
-types-pyyaml = "^6.0.12.2"
+types-pyyaml = "^5.4"
 types-requests = "^2.28.11.5"
 types-setuptools = "^65.6.0.2"
 twine = "^4.0.2"
 locust = "^2.14.2"
 types-tabulate = "^0.9.0.0"
 types-markdown = "^3.4.2.5"
 pytest-timeout = "^2.1.0"
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/model_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 from pathlib import Path
 
 import click
 from fastapi.encoders import jsonable_encoder
 from tabulate import tabulate
 
 from tungstenkit._internal import model_store
-from tungstenkit._internal.constants import (
-    DEFAULT_MODEL_MODULE,
-    TUNGSTEN_DIR_IN_CONTAINER,
-    TUNGSTEN_LOGO,
-)
+from tungstenkit._internal.constants import DEFAULT_MODEL_MODULE, TUNGSTEN_LOGO
 from tungstenkit._internal.containerize import build_model
 from tungstenkit._internal.demo_server import start_demo_server
 from tungstenkit._internal.pred_interface.local_interface import LocalModel
 from tungstenkit._internal.storables import ModelData
 from tungstenkit._internal.tungsten_clients import TungstenClient
 from tungstenkit._internal.utils import docker
 from tungstenkit._internal.utils.console import print_pretty, print_success, yes_or_no_prompt
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/constants.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 CONFIG_DIR = Path(os.getenv("TUNGSTEN_CONFIG_DIR", Path(appdirs.user_config_dir)))
 CONFIG_DIR = CONFIG_DIR.resolve()
 CONFIG_DIR.mkdir(parents=True, exist_ok=True)
 
 LOCK_DIR = Path(tempfile.gettempdir()) / "tungsten" / "locks"
 LOCK_DIR.mkdir(parents=True, exist_ok=True)
 
-WORKING_DIR_IN_CONTAINER = PurePosixPath("/tungsten")
 TUNGSTEN_DIR_IN_CONTAINER = PurePosixPath("/etc/tungsten")
+WORKING_DIR_IN_CONTAINER = PurePosixPath("/tungsten")
 
 MIN_SUPPORTED_PYTHON_VER = Version("3.7")
 MAX_SUPPORTED_PYTHON_VER = Version("3.11")
 MAX_SOURCE_FILE_SIZE = 10 * 1024 * 1024
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/build_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,20 +145,14 @@
         with FileLock(lock_path):
             with ThreadPoolExecutor(max_workers=8) as executor:
                 rel_path_to_dockerfile = rel_path_to_tmp_dir / "Dockerfile"
                 rel_path_to_tungstenkit = rel_path_to_tmp_dir / "tungstenkit"
                 rel_path_to_tungstenkit.mkdir()
                 future_list: t.List[Future] = []
 
-                _copy_tungstenkit(
-                    build_dir=build_dir,
-                    rel_path_to_tungstenkit=rel_path_to_tungstenkit,
-                    executor=executor,
-                    future_list=future_list,
-                )
                 build_config.copy_files.extend(
                     _convert_abs_symlinks_to_rel(
                         build_dir,
                         include_patterns=build_config.include_files,
                         exclude_patterns=build_config.exclude_files,
                         rel_path_to_tmp_dir=rel_path_to_tmp_dir,
                     )
@@ -175,15 +169,14 @@
                         copy_dir=rel_path_to_tmp_dir,
                         future_list=future_list,
                         ignore_patterns=["tungstenkit"],
                     )
 
                 dockerfile = dockerfile_generator.generate(
                     tmp_dir_in_build_ctx=rel_path_to_tmp_dir,
-                    tungstenkit_dir_in_build_ctx=rel_path_to_tungstenkit,
                 )
                 dockerfile_path = build_dir / rel_path_to_dockerfile
                 dockerfile_path.write_text(dockerfile)
                 log_debug(
                     "Dockerfile:\n"
                     + "\n".join(["  " + line for line in dockerfile.strip().split("\n") if line]),
                     pretty=False,
@@ -310,39 +303,14 @@
             (src_in_build_ctx.relative_to(abs_path_to_build_dir).as_posix(), dest_str)
         )
 
     log_info("")
     return files_with_dest
 
 
-def _copy_tungstenkit(
-    build_dir: Path,
-    rel_path_to_tungstenkit: Path,
-    executor: ThreadPoolExecutor,
-    future_list: t.List[Future],
-):
-    requirements_txt_path = Path(__file__).parent / "metadata" / "tungstenkit" / "requirements.txt"
-    pyproject_toml_path = requirements_txt_path.with_name("pyproject.toml")
-    tungstenkit_dir_in_build_ctx = build_dir / rel_path_to_tungstenkit
-    requirements_txt_path_in_build_ctx = tungstenkit_dir_in_build_ctx / requirements_txt_path.name
-    pyproject_toml_path_in_build_ctx = tungstenkit_dir_in_build_ctx / pyproject_toml_path.name
-
-    src_dir = Path(tungstenkit.__file__).parent
-    shutil.copy(str(requirements_txt_path), str(requirements_txt_path_in_build_ctx))
-    shutil.copy(str(pyproject_toml_path), str(pyproject_toml_path_in_build_ctx))
-    future_list.append(
-        executor.submit(
-            shutil.copytree,
-            str(src_dir),
-            str(tungstenkit_dir_in_build_ctx / "tungstenkit"),
-            ignore=shutil.ignore_patterns("*.pyc"),  # TODO add more
-        )
-    )
-
-
 def _show_progress_while_copying_files(
     copy_dir: Path, future_list: t.List[Future], ignore_patterns: t.Optional[t.List[str]] = None
 ):
     progress = Progress(TextColumn("{task.description}"))
     desc_prefix = "Copied: "
     task = progress.add_task(desc_prefix + "0B")
     with progress:
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 
 import attrs
 import jinja2
 from packaging.version import Version
 from pathspec import PathSpec
 
+import tungstenkit
 from tungstenkit._internal.configs import BuildConfig
 from tungstenkit._internal.logging import log_debug, log_info, log_warning
 from tungstenkit._internal.utils.version import NotRequired
 
 from ..base_images import BaseImage, CUDAImageCollection, CustomImage, PythonImageCollection
 from ..gpu_pkg_collections import supported_gpu_pkg_names
 from ..pkg_manager import PythonPackageManager, RequirementsTxt
@@ -25,19 +26,17 @@
         config: BuildConfig,
     ):
         self.config = config
 
     def generate(
         self,
         tmp_dir_in_build_ctx: Path,
-        tungstenkit_dir_in_build_ctx: Path,
     ):
         template_args = self.build_template_args(
             tmp_dir_in_build_ctx=tmp_dir_in_build_ctx,
-            tungstenkit_dir_in_build_ctx=tungstenkit_dir_in_build_ctx,
         )
         log_debug("Dockerfile template args:\n" + str(template_args))
         log_info("\n")
         log_info(f"[bold]Use GPU: {template_args.device == 'gpu'}[/bold]")
         log_info(f"[bold]Base image: [green]{template_args.image.name}[/green][/bold]")
         log_info(
             f"[bold]Python version: [green]{str(template_args.python_version)}[/green][/bold]"
@@ -54,15 +53,14 @@
         dockerfile = template.render(**attrs.asdict(template_args, recurse=False))
 
         return dockerfile
 
     def build_template_args(
         self,
         tmp_dir_in_build_ctx: Path,
-        tungstenkit_dir_in_build_ctx: Path,
     ):
         # TODO perfer cuda version available in docker hub
         # TODO check py vers compatible with miniforge3
         # TODO don't use cuda base image if python package already includes cuda (e.g. torch)
 
         cuda_ver: t.Optional[t.Union[Version, NotRequired]] = (
             self.config.cuda_version if self.config.gpu else NotRequired()
@@ -74,14 +72,16 @@
 
         # Add pip requirements
         py_pkg_manager = PythonPackageManager()
         for requirement_str in self.config.python_packages:
             # TODO requirement_str -> requirement
             py_pkg_manager.add_requirement_str(requirement_str)
 
+        py_pkg_manager.add_requirement_str(tungstenkit.__name__ + "==" + tungstenkit.__version__)
+
         # Set user-defined CUDA & Python versions
         py_pkg_manager.set_gpu(self.config.gpu)
 
         # Infer CUDA, CuDNN and Python versions if requested
         if self.config.gpu:
             if cuda_ver is None:
                 cuda_ver = py_pkg_manager.infer_cuda_ver()
@@ -152,15 +152,14 @@
             list_pip_install_args=list_pip_install_args,
             system_packages=self.config.system_packages,
             pip_wheels_in_build_ctx=self.config.pip_wheels,
             env_vars=self.config.environment_variables,
             tungsten_env_vars=self.config.tungsten_environment_variables,
             copy_files=self.config.copy_files,
             device="gpu" if self.config.gpu else "cpu",
-            tungstenkit_dir_in_build_ctx=tungstenkit_dir_in_build_ctx,
             large_files=large_files,
             small_files=small_files,
         )
 
         return template_args
 
     def split_large_and_small_files(
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files 26% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 COPY {{ path.as_posix() }} /tmp/wheels
 {% endfor %}
 RUN rm -rf /tmp/wheels
 {% endif %}
 
 {% if pip_requirements_txt_in_build_ctx != None %}
 COPY --link {{ pip_requirements_txt_in_build_ctx.as_posix() }} /tmp/requirements.txt
-COPY --link {{ tungstenkit_dir_in_build_ctx.as_posix()}} {{ tungstenkit_dir_in_container.as_posix()}}
-RUN {{ cache.mount_pip_cache() }} echo "." >> /tmp/requirements.txt && \
-    cd {{ tungstenkit_dir_in_container.as_posix()}} && \
-    pip install -r /tmp/requirements.txt && \
+RUN pip install -r /tmp/requirements.txt && \
     rm -f /tmp/requirements.txt
 {% endif%}
 
 {% if dockerfile_commands|length > 0 %}
 {% for cmd in dockerfile_commands %}
 {{ cmd }}
 {% endfor %}
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/metadata/tungstenkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/500.html` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/500.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/afTF15k0tNJ2rEveq5WZR/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/8-936f7a161aaf624f.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-27c7bca72f8b0e82.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-fb2189cefdf627af.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/io.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/json_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/avatar_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/model_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/storables/source_file_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/task.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/__init__.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
-from .user import User
-
 
 class SourceFileDecl(BaseModel):
     path: str
     upload_id: int
 
 
 class SkippedSourceFileDecl(BaseModel):
```

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/tungsten_clients/schemas/project.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/tungsten_clients/schemas/project.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/types.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.2.post5/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/tungstenkit/exceptions.py` & `tungstenkit-0.1.2.post5/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post4/PKG-INFO` & `tungstenkit-0.1.2.post5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.2.post4
+Version: 0.1.2.post5
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -50,15 +50,15 @@
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: pathspec (>=0.10.2,<0.11.0)
 Requires-Dist: pillow (>=5.2.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pynvml (>=11.5.0,<12.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: pyyaml (>=5.4,<6.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Requires-Dist: uvicorn (>=0.17.6,<1.0.0)
```

