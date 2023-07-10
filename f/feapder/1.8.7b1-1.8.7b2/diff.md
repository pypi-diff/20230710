# Comparing `tmp/feapder-1.8.7b1.tar.gz` & `tmp/feapder-1.8.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feapder-1.8.7b1.tar", last modified: Wed Jun 28 13:19:58 2023, max compression
+gzip compressed data, was "feapder-1.8.7b2.tar", last modified: Mon Jul 10 08:01:51 2023, max compression
```

## Comparing `feapder-1.8.7b1.tar` & `feapder-1.8.7b2.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.188048 feapder-1.8.7b1/
--rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.8.7b1/LICENSE
--rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.8.7b1/MANIFEST.in
--rw-r--r--   0 liubo      (501) staff       (20)     4813 2023-06-28 13:19:58.187377 feapder-1.8.7b1/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     4366 2023-06-28 12:11:24.000000 feapder-1.8.7b1/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.961220 feapder-1.8.7b1/feapder/
--rw-r--r--   0 liubo      (501) staff       (20)       11 2023-06-28 13:19:39.000000 feapder-1.8.7b1/feapder/VERSION
--rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.966416 feapder-1.8.7b1/feapder/buffer/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/buffer/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    14141 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/buffer/item_buffer.py
--rw-r--r--   0 liubo      (501) staff       (20)     5356 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/buffer/request_buffer.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.971031 feapder-1.8.7b1/feapder/commands/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b1/feapder/commands/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/commands/cmdline.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.982079 feapder-1.8.7b1/feapder/commands/create/
--rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.8.7b1/feapder/commands/create/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/commands/create/create_cookies.py
--rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.8.7b1/feapder/commands/create/create_init.py
--rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.8.7b1/feapder/commands/create/create_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/commands/create/create_json.py
--rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.8.7b1/feapder/commands/create/create_params.py
--rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/commands/create/create_project.py
--rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/commands/create/create_setting.py
--rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.8.7b1/feapder/commands/create/create_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/commands/create/create_table.py
--rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.8.7b1/feapder/commands/create_builder.py
--rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/commands/retry.py
--rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.8.7b1/feapder/commands/shell.py
--rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/commands/zip.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.991056 feapder-1.8.7b1/feapder/core/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/core/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6240 2022-12-01 11:29:17.000000 feapder-1.8.7b1/feapder/core/base_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)     3256 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/core/collector.py
--rw-r--r--   0 liubo      (501) staff       (20)     2808 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/core/handle_failed_items.py
--rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/core/handle_failed_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)    32962 2023-06-28 13:10:40.000000 feapder-1.8.7b1/feapder/core/parser_control.py
--rw-r--r--   0 liubo      (501) staff       (20)    21656 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/core/scheduler.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.998620 feapder-1.8.7b1/feapder/core/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.8.7b1/feapder/core/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     4368 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/core/spiders/air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/core/spiders/batch_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/core/spiders/spider.py
--rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/core/spiders/task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.024833 feapder-1.8.7b1/feapder/db/
--rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.8.7b1/feapder/db/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/db/memorydb.py
--rw-r--r--   0 liubo      (501) staff       (20)    13606 2021-12-04 11:42:58.000000 feapder-1.8.7b1/feapder/db/mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)    10799 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/db/mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)    29545 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/db/redisdb.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.029853 feapder-1.8.7b1/feapder/dedup/
--rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.8.7b1/feapder/dedup/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.8.7b1/feapder/dedup/basefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     4133 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/dedup/bitarray.py
--rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.8.7b1/feapder/dedup/bloomfilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/dedup/expirefilter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/dedup/litefilter.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.034330 feapder-1.8.7b1/feapder/network/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b1/feapder/network/__init__.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.038284 feapder-1.8.7b1/feapder/network/downloader/
--rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/network/downloader/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/network/downloader/_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.8.7b1/feapder/network/downloader/_requests.py
--rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/network/downloader/_selenium.py
--rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.8.7b1/feapder/network/downloader/base.py
--rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/network/item.py
--rw-r--r--   0 liubo      (501) staff       (20)     2070 2023-06-28 13:00:38.000000 feapder-1.8.7b1/feapder/network/proxy_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/network/proxy_pool_old.py
--rw-r--r--   0 liubo      (501) staff       (20)    17719 2023-06-28 12:58:09.000000 feapder-1.8.7b1/feapder/network/request.py
--rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/network/response.py
--rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/network/selector.py
--rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.8.7b1/feapder/network/user_agent.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.041290 feapder-1.8.7b1/feapder/network/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/network/user_pool/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/network/user_pool/base_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/network/user_pool/gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     5372 2022-09-25 13:50:01.000000 feapder-1.8.7b1/feapder/network/user_pool/guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/network/user_pool/normal_user_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.043832 feapder-1.8.7b1/feapder/pipelines/
--rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.8.7b1/feapder/pipelines/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.8.7b1/feapder/pipelines/console_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.8.7b1/feapder/pipelines/mongo_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.8.7b1/feapder/pipelines/mysql_pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)      363 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)    10917 2023-06-28 13:08:22.000000 feapder-1.8.7b1/feapder/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.048873 feapder-1.8.7b1/feapder/templates/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b1/feapder/templates/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/templates/air_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.8.7b1/feapder/templates/batch_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.8.7b1/feapder/templates/item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.052121 feapder-1.8.7b1/feapder/templates/project_template/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b1/feapder/templates/project_template/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/templates/project_template/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.052641 feapder-1.8.7b1/feapder/templates/project_template/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b1/feapder/templates/project_template/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.8.7b1/feapder/templates/project_template/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     8918 2023-06-28 13:11:47.000000 feapder-1.8.7b1/feapder/templates/project_template/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.053004 feapder-1.8.7b1/feapder/templates/project_template/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b1/feapder/templates/project_template/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/templates/spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.7b1/feapder/templates/task_spider_template.tmpl
--rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.8.7b1/feapder/templates/update_item_template.tmpl
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.058891 feapder-1.8.7b1/feapder/utils/
--rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.8.7b1/feapder/utils/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.8.7b1/feapder/utils/custom_argparse.py
--rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/utils/email_sender.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.060935 feapder-1.8.7b1/feapder/utils/js/
--rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/utils/js/intercept.js
--rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/utils/js/stealth.min.js
--rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.8.7b1/feapder/utils/log.py
--rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.8.7b1/feapder/utils/metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.8.7b1/feapder/utils/perfect_dict.py
--rw-r--r--   0 liubo      (501) staff       (20)     3670 2022-06-10 02:51:23.000000 feapder-1.8.7b1/feapder/utils/redis_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)    73692 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/utils/tools.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.065902 feapder-1.8.7b1/feapder/utils/webdriver/
--rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/utils/webdriver/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     9330 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/utils/webdriver/playwright_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)    12628 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/utils/webdriver/selenium_driver.py
--rw-r--r--   0 liubo      (501) staff       (20)     2574 2023-06-28 09:14:30.000000 feapder-1.8.7b1/feapder/utils/webdriver/webdirver.py
--rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.8.7b1/feapder/utils/webdriver/webdriver_pool.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:57.964278 feapder-1.8.7b1/feapder.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     4813 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     6017 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)       61 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/entry_points.txt
--rw-r--r--   0 liubo      (501) staff       (20)      435 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)        8 2023-06-28 13:19:57.000000 feapder-1.8.7b1/feapder.egg-info/top_level.txt
--rw-r--r--   0 liubo      (501) staff       (20)       38 2023-06-28 13:19:58.188334 feapder-1.8.7b1/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-06-28 09:14:32.000000 feapder-1.8.7b1/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.081125 feapder-1.8.7b1/tests/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.105208 feapder-1.8.7b1/tests/air-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     1218 2022-11-29 03:10:00.000000 feapder-1.8.7b1/tests/air-spider/test_air_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.8.7b1/tests/air-spider/test_air_spider_filter.py
--rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/air-spider/test_air_spider_item.py
--rw-r--r--   0 liubo      (501) staff       (20)      638 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/air-spider/test_render_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.106921 feapder-1.8.7b1/tests/batch-spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.112504 feapder-1.8.7b1/tests/batch-spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.8.7b1/tests/batch-spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.8.7b1/tests/batch-spider/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.8.7b1/tests/batch-spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.8.7b1/tests/batch-spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.114090 feapder-1.8.7b1/tests/batch-spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.8.7b1/tests/batch-spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/batch-spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.8.7b1/tests/batch-spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.108780 feapder-1.8.7b1/tests/batch-spider-integration/
--rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.8.7b1/tests/batch-spider-integration/batch_spider_integration_task.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.109495 feapder-1.8.7b1/tests/batch-spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.7b1/tests/batch-spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.8.7b1/tests/batch-spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.7b1/tests/batch-spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.111170 feapder-1.8.7b1/tests/batch-spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.7b1/tests/batch-spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/batch-spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/batch-spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.114782 feapder-1.8.7b1/tests/db/
--rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.8.7b1/tests/db/test_redis.py
--rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/jd_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.8.7b1/tests/mongo_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.116477 feapder-1.8.7b1/tests/spider/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.121743 feapder-1.8.7b1/tests/spider/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.8.7b1/tests/spider/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.8.7b1/tests/spider/items/spider_data_item.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.122281 feapder-1.8.7b1/tests/spider/log/
--rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.8.7b1/tests/spider/log/haha.log
--rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.8.7b1/tests/spider/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2676 2023-06-28 09:14:30.000000 feapder-1.8.7b1/tests/spider/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.124183 feapder-1.8.7b1/tests/spider/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.8.7b1/tests/spider/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      985 2022-10-25 08:22:40.000000 feapder-1.8.7b1/tests/spider/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.8.7b1/tests/spider/spiders/test_spider2.py
--rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.8.7b1/tests/spider/table.sql
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.117885 feapder-1.8.7b1/tests/spider-integration/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.118370 feapder-1.8.7b1/tests/spider-integration/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.7b1/tests/spider-integration/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.8.7b1/tests/spider-integration/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.7b1/tests/spider-integration/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.120628 feapder-1.8.7b1/tests/spider-integration/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.7b1/tests/spider-integration/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.8.7b1/tests/spider-integration/spiders/sina_news_parser.py
--rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.8.7b1/tests/spider-integration/spiders/tencent_news_parser.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.124986 feapder-1.8.7b1/tests/task-spider/
--rw-r--r--   0 liubo      (501) staff       (20)     2133 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/task-spider/test_task_spider.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.127493 feapder-1.8.7b1/tests/test-debugger/
--rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b1/tests/test-debugger/.DS_Store
--rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.128189 feapder-1.8.7b1/tests/test-debugger/items/
--rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     8784 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.129330 feapder-1.8.7b1/tests/test-debugger/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test-debugger/spiders/test_debugger.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.132474 feapder-1.8.7b1/tests/test-pipeline/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.133868 feapder-1.8.7b1/tests/test-pipeline/items/
--rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/test-pipeline/items/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/test-pipeline/items/spider_data_item.py
--rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.8.7b1/tests/test-pipeline/main.py
--rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.8.7b1/tests/test-pipeline/pipeline.py
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.8.7b1/tests/test-pipeline/setting.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.136106 feapder-1.8.7b1/tests/test-pipeline/spiders/
--rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.8.7b1/tests/test-pipeline/spiders/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/test-pipeline/spiders/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.8.7b1/tests/test-pipeline/table.sql
--rw-r--r--   0 liubo      (501) staff       (20)      281 2022-11-22 03:30:44.000000 feapder-1.8.7b1/tests/test.py
--rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test_dedup.py
--rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.8.7b1/tests/test_lock.py
--rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.8.7b1/tests/test_log.py
--rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.8.7b1/tests/test_metrics.py
--rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.8.7b1/tests/test_mongodb.py
--rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.8.7b1/tests/test_mysqldb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.8.7b1/tests/test_playwright.py
--rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.8.7b1/tests/test_playwright2.py
--rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.8.7b1/tests/test_rander.py
--rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.8.7b1/tests/test_rander2.py
--rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.8.7b1/tests/test_rander3.py
--rw-r--r--   0 liubo      (501) staff       (20)     1983 2022-09-07 09:10:17.000000 feapder-1.8.7b1/tests/test_rander_xhr.py
--rw-r--r--   0 liubo      (501) staff       (20)      148 2021-08-12 03:51:27.000000 feapder-1.8.7b1/tests/test_redisdb.py
--rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.8.7b1/tests/test_request.py
--rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.8.7b1/tests/test_spider_params.py
--rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.8.7b1/tests/test_task.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.160685 feapder-1.8.7b1/tests/test_template/
--rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.7b1/tests/test_template/test_spider.py
--rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.8.7b1/tests/test_tools.py
--rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.8.7b1/tests/test_webdriver.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-06-28 13:19:58.185644 feapder-1.8.7b1/tests/user_pool/
--rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.8.7b1/tests/user_pool/test_gold_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.8.7b1/tests/user_pool/test_guest_user_pool.py
--rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.8.7b1/tests/user_pool/test_normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.863384 feapder-1.8.7b2/
+-rw-r--r--   0 liubo      (501) staff       (20)     1102 2021-08-04 13:29:34.000000 feapder-1.8.7b2/LICENSE
+-rw-r--r--   0 liubo      (501) staff       (20)      231 2021-08-12 03:51:27.000000 feapder-1.8.7b2/MANIFEST.in
+-rw-r--r--   0 liubo      (501) staff       (20)     4813 2023-07-10 08:01:51.862552 feapder-1.8.7b2/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     4366 2023-06-28 12:11:24.000000 feapder-1.8.7b2/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.663342 feapder-1.8.7b2/feapder/
+-rw-r--r--   0 liubo      (501) staff       (20)       11 2023-07-10 08:00:59.000000 feapder-1.8.7b2/feapder/VERSION
+-rw-r--r--   0 liubo      (501) staff       (20)      815 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.668924 feapder-1.8.7b2/feapder/buffer/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/buffer/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    14141 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/buffer/item_buffer.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5356 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/buffer/request_buffer.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.673463 feapder-1.8.7b2/feapder/commands/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b2/feapder/commands/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3824 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/commands/cmdline.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.685879 feapder-1.8.7b2/feapder/commands/create/
+-rw-r--r--   0 liubo      (501) staff       (20)      543 2021-09-02 10:23:23.000000 feapder-1.8.7b2/feapder/commands/create/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      975 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/commands/create/create_cookies.py
+-rw-r--r--   0 liubo      (501) staff       (20)      670 2021-02-08 06:31:07.000000 feapder-1.8.7b2/feapder/commands/create/create_init.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6004 2022-09-07 03:39:37.000000 feapder-1.8.7b2/feapder/commands/create/create_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1366 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/commands/create/create_json.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1106 2021-09-02 10:23:23.000000 feapder-1.8.7b2/feapder/commands/create/create_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1360 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/commands/create/create_project.py
+-rw-r--r--   0 liubo      (501) staff       (20)      693 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/commands/create/create_setting.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3648 2022-09-07 03:39:37.000000 feapder-1.8.7b2/feapder/commands/create/create_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4288 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/commands/create/create_table.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3984 2022-10-21 10:06:04.000000 feapder-1.8.7b2/feapder/commands/create_builder.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1354 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/commands/retry.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5514 2022-10-21 10:06:04.000000 feapder-1.8.7b2/feapder/commands/shell.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2572 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/commands/zip.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.707574 feapder-1.8.7b2/feapder/core/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/core/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6240 2022-12-01 11:29:17.000000 feapder-1.8.7b2/feapder/core/base_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3256 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/core/collector.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2808 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/core/handle_failed_items.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1733 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/core/handle_failed_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)    32962 2023-06-28 13:10:40.000000 feapder-1.8.7b2/feapder/core/parser_control.py
+-rw-r--r--   0 liubo      (501) staff       (20)    21725 2023-07-10 07:59:40.000000 feapder-1.8.7b2/feapder/core/scheduler.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.712738 feapder-1.8.7b2/feapder/core/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)      417 2022-07-25 12:58:57.000000 feapder-1.8.7b2/feapder/core/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4375 2023-07-10 08:00:07.000000 feapder-1.8.7b2/feapder/core/spiders/air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    49433 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/core/spiders/batch_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13420 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/core/spiders/spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)    27875 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/core/spiders/task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.717475 feapder-1.8.7b2/feapder/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      136 2021-12-21 10:30:46.000000 feapder-1.8.7b2/feapder/db/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1117 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/db/memorydb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    13606 2021-12-04 11:42:58.000000 feapder-1.8.7b2/feapder/db/mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10799 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/db/mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)    29545 2023-07-05 08:42:31.000000 feapder-1.8.7b2/feapder/db/redisdb.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.723512 feapder-1.8.7b2/feapder/dedup/
+-rw-r--r--   0 liubo      (501) staff       (20)     6616 2022-09-25 13:50:01.000000 feapder-1.8.7b2/feapder/dedup/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      901 2022-09-25 13:50:01.000000 feapder-1.8.7b2/feapder/dedup/basefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4133 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/dedup/bitarray.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12518 2022-09-25 13:50:01.000000 feapder-1.8.7b2/feapder/dedup/bloomfilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2309 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/dedup/expirefilter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1854 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/dedup/litefilter.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.731140 feapder-1.8.7b2/feapder/network/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b2/feapder/network/__init__.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.736802 feapder-1.8.7b2/feapder/network/downloader/
+-rw-r--r--   0 liubo      (501) staff       (20)      299 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/network/downloader/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3217 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/network/downloader/_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1440 2022-09-09 06:16:43.000000 feapder-1.8.7b2/feapder/network/downloader/_requests.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3093 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/network/downloader/_selenium.py
+-rw-r--r--   0 liubo      (501) staff       (20)      694 2022-09-07 03:39:37.000000 feapder-1.8.7b2/feapder/network/downloader/base.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4341 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/network/item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2070 2023-06-28 13:00:38.000000 feapder-1.8.7b2/feapder/network/proxy_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    23025 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/network/proxy_pool_old.py
+-rw-r--r--   0 liubo      (501) staff       (20)    17719 2023-06-28 12:58:09.000000 feapder-1.8.7b2/feapder/network/request.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12743 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/network/response.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5661 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/network/selector.py
+-rw-r--r--   0 liubo      (501) staff       (20)   130399 2023-06-28 08:50:40.000000 feapder-1.8.7b2/feapder/network/user_agent.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.740748 feapder-1.8.7b2/feapder/network/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/network/user_pool/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     6397 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/network/user_pool/base_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10762 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/network/user_pool/gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     5372 2022-09-25 13:50:01.000000 feapder-1.8.7b2/feapder/network/user_pool/guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8648 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/network/user_pool/normal_user_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.744784 feapder-1.8.7b2/feapder/pipelines/
+-rw-r--r--   0 liubo      (501) staff       (20)     1382 2021-09-23 09:22:51.000000 feapder-1.8.7b2/feapder/pipelines/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1392 2022-09-25 13:50:01.000000 feapder-1.8.7b2/feapder/pipelines/console_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2405 2021-09-23 09:22:51.000000 feapder-1.8.7b2/feapder/pipelines/mongo_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2088 2021-04-08 03:41:12.000000 feapder-1.8.7b2/feapder/pipelines/mysql_pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)      363 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)    10917 2023-06-28 13:08:22.000000 feapder-1.8.7b2/feapder/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.752975 feapder-1.8.7b2/feapder/templates/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b2/feapder/templates/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)      592 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/templates/air_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2083 2022-09-07 03:39:38.000000 feapder-1.8.7b2/feapder/templates/batch_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2021-12-22 05:53:07.000000 feapder-1.8.7b2/feapder/templates/item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.757561 feapder-1.8.7b2/feapder/templates/project_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b2/feapder/templates/project_template/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)     1574 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/templates/project_template/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.758399 feapder-1.8.7b2/feapder/templates/project_template/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b2/feapder/templates/project_template/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2089 2021-09-02 10:23:23.000000 feapder-1.8.7b2/feapder/templates/project_template/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8918 2023-06-28 13:11:47.000000 feapder-1.8.7b2/feapder/templates/project_template/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.758794 feapder-1.8.7b2/feapder/templates/project_template/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-02-07 13:26:42.000000 feapder-1.8.7b2/feapder/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      808 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/templates/spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.7b2/feapder/templates/task_spider_template.tmpl
+-rw-r--r--   0 liubo      (501) staff       (20)      365 2022-09-19 07:00:37.000000 feapder-1.8.7b2/feapder/templates/update_item_template.tmpl
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.764861 feapder-1.8.7b2/feapder/utils/
+-rw-r--r--   0 liubo      (501) staff       (20)      135 2021-08-04 13:29:34.000000 feapder-1.8.7b2/feapder/utils/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1959 2021-02-07 13:26:42.000000 feapder-1.8.7b2/feapder/utils/custom_argparse.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2537 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/utils/email_sender.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.767667 feapder-1.8.7b2/feapder/utils/js/
+-rw-r--r--   0 liubo      (501) staff       (20)     6344 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/utils/js/intercept.js
+-rw-r--r--   0 liubo      (501) staff       (20)   166307 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/utils/js/stealth.min.js
+-rw-r--r--   0 liubo      (501) staff       (20)     8468 2023-06-28 09:47:12.000000 feapder-1.8.7b2/feapder/utils/log.py
+-rw-r--r--   0 liubo      (501) staff       (20)    16820 2023-06-28 09:14:32.000000 feapder-1.8.7b2/feapder/utils/metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2123 2021-08-12 03:51:27.000000 feapder-1.8.7b2/feapder/utils/perfect_dict.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3670 2022-06-10 02:51:23.000000 feapder-1.8.7b2/feapder/utils/redis_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)    73692 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/utils/tools.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.772688 feapder-1.8.7b2/feapder/utils/webdriver/
+-rw-r--r--   0 liubo      (501) staff       (20)      380 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/utils/webdriver/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     9344 2023-06-29 04:33:39.000000 feapder-1.8.7b2/feapder/utils/webdriver/playwright_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)    12699 2023-06-29 04:32:52.000000 feapder-1.8.7b2/feapder/utils/webdriver/selenium_driver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2574 2023-06-28 09:14:30.000000 feapder-1.8.7b2/feapder/utils/webdriver/webdirver.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3282 2023-06-28 09:14:31.000000 feapder-1.8.7b2/feapder/utils/webdriver/webdriver_pool.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.666840 feapder-1.8.7b2/feapder.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     4813 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     6017 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       61 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/entry_points.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      435 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        8 2023-07-10 08:01:51.000000 feapder-1.8.7b2/feapder.egg-info/top_level.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       38 2023-07-10 08:01:51.863576 feapder-1.8.7b2/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)     2103 2023-06-28 09:14:32.000000 feapder-1.8.7b2/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.788064 feapder-1.8.7b2/tests/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.803058 feapder-1.8.7b2/tests/air-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     1218 2022-11-29 03:10:00.000000 feapder-1.8.7b2/tests/air-spider/test_air_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1075 2023-06-28 09:14:30.000000 feapder-1.8.7b2/tests/air-spider/test_air_spider_filter.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1094 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/air-spider/test_air_spider_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)      638 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/air-spider/test_render_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.805050 feapder-1.8.7b2/tests/batch-spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.811043 feapder-1.8.7b2/tests/batch-spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-09-03 07:47:43.000000 feapder-1.8.7b2/tests/batch-spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-09-12 14:22:50.000000 feapder-1.8.7b2/tests/batch-spider/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2020 2023-06-09 12:31:43.000000 feapder-1.8.7b2/tests/batch-spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2227 2021-09-02 10:23:23.000000 feapder-1.8.7b2/tests/batch-spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.812298 feapder-1.8.7b2/tests/batch-spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-02-08 08:09:47.000000 feapder-1.8.7b2/tests/batch-spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1575 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/batch-spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-02-08 08:29:51.000000 feapder-1.8.7b2/tests/batch-spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.807251 feapder-1.8.7b2/tests/batch-spider-integration/
+-rw-r--r--   0 liubo      (501) staff       (20)      746 2021-03-03 03:39:52.000000 feapder-1.8.7b2/tests/batch-spider-integration/batch_spider_integration_task.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.807915 feapder-1.8.7b2/tests/batch-spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.7b2/tests/batch-spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1686 2021-12-30 08:52:14.000000 feapder-1.8.7b2/tests/batch-spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.7b2/tests/batch-spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.809608 feapder-1.8.7b2/tests/batch-spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.7b2/tests/batch-spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      581 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/batch-spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      584 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/batch-spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.812935 feapder-1.8.7b2/tests/db/
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2021-03-06 15:13:19.000000 feapder-1.8.7b2/tests/db/test_redis.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2087 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/jd_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2021-12-01 05:56:45.000000 feapder-1.8.7b2/tests/mongo_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.814909 feapder-1.8.7b2/tests/spider/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.819428 feapder-1.8.7b2/tests/spider/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2022-01-27 08:13:00.000000 feapder-1.8.7b2/tests/spider/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      358 2021-12-22 05:05:06.000000 feapder-1.8.7b2/tests/spider/items/spider_data_item.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.820077 feapder-1.8.7b2/tests/spider/log/
+-rw-r--r--   0 liubo      (501) staff       (20)     1719 2021-08-11 01:59:56.000000 feapder-1.8.7b2/tests/spider/log/haha.log
+-rw-r--r--   0 liubo      (501) staff       (20)      296 2022-08-31 02:19:25.000000 feapder-1.8.7b2/tests/spider/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2676 2023-06-28 09:14:30.000000 feapder-1.8.7b2/tests/spider/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.822004 feapder-1.8.7b2/tests/spider/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       42 2021-02-21 15:44:20.000000 feapder-1.8.7b2/tests/spider/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      985 2022-10-25 08:22:40.000000 feapder-1.8.7b2/tests/spider/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      612 2021-08-04 13:29:34.000000 feapder-1.8.7b2/tests/spider/spiders/test_spider2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      320 2021-02-08 08:40:34.000000 feapder-1.8.7b2/tests/spider/table.sql
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.816135 feapder-1.8.7b2/tests/spider-integration/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.816667 feapder-1.8.7b2/tests/spider-integration/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2021-03-03 03:39:52.000000 feapder-1.8.7b2/tests/spider-integration/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      517 2021-12-30 08:51:43.000000 feapder-1.8.7b2/tests/spider-integration/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2226 2021-09-02 10:23:23.000000 feapder-1.8.7b2/tests/spider-integration/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.818257 feapder-1.8.7b2/tests/spider-integration/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       63 2021-03-03 03:39:52.000000 feapder-1.8.7b2/tests/spider-integration/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      470 2023-03-29 13:31:04.000000 feapder-1.8.7b2/tests/spider-integration/spiders/sina_news_parser.py
+-rw-r--r--   0 liubo      (501) staff       (20)      456 2021-09-24 05:52:08.000000 feapder-1.8.7b2/tests/spider-integration/spiders/tencent_news_parser.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.822625 feapder-1.8.7b2/tests/task-spider/
+-rw-r--r--   0 liubo      (501) staff       (20)     2133 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/task-spider/test_task_spider.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.825120 feapder-1.8.7b2/tests/test-debugger/
+-rw-r--r--   0 liubo      (501) staff       (20)     6148 2022-03-18 07:14:05.000000 feapder-1.8.7b2/tests/test-debugger/.DS_Store
+-rw-r--r--   0 liubo      (501) staff       (20)       81 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.825762 feapder-1.8.7b2/tests/test-debugger/items/
+-rw-r--r--   0 liubo      (501) staff       (20)        0 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      352 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     8784 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.826731 feapder-1.8.7b2/tests/test-debugger/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       33 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      724 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test-debugger/spiders/test_debugger.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.832188 feapder-1.8.7b2/tests/test-pipeline/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.835122 feapder-1.8.7b2/tests/test-pipeline/items/
+-rw-r--r--   0 liubo      (501) staff       (20)       36 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/test-pipeline/items/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)      586 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/test-pipeline/items/spider_data_item.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1250 2022-09-07 03:39:38.000000 feapder-1.8.7b2/tests/test-pipeline/main.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1416 2021-04-08 03:41:12.000000 feapder-1.8.7b2/tests/test-pipeline/pipeline.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2021-09-02 10:23:23.000000 feapder-1.8.7b2/tests/test-pipeline/setting.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.836671 feapder-1.8.7b2/tests/test-pipeline/spiders/
+-rw-r--r--   0 liubo      (501) staff       (20)       31 2021-03-30 02:34:20.000000 feapder-1.8.7b2/tests/test-pipeline/spiders/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1514 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/test-pipeline/spiders/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      851 2021-03-18 02:19:03.000000 feapder-1.8.7b2/tests/test-pipeline/table.sql
+-rw-r--r--   0 liubo      (501) staff       (20)      281 2022-11-22 03:30:44.000000 feapder-1.8.7b2/tests/test.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3140 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test_dedup.py
+-rw-r--r--   0 liubo      (501) staff       (20)      469 2021-09-02 10:22:59.000000 feapder-1.8.7b2/tests/test_lock.py
+-rw-r--r--   0 liubo      (501) staff       (20)      329 2023-06-28 09:47:12.000000 feapder-1.8.7b2/tests/test_log.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1229 2023-06-28 09:14:32.000000 feapder-1.8.7b2/tests/test_metrics.py
+-rw-r--r--   0 liubo      (501) staff       (20)     4678 2021-12-01 05:56:51.000000 feapder-1.8.7b2/tests/test_mongodb.py
+-rw-r--r--   0 liubo      (501) staff       (20)      232 2021-10-14 08:25:11.000000 feapder-1.8.7b2/tests/test_mysqldb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1086 2023-06-28 09:14:31.000000 feapder-1.8.7b2/tests/test_playwright.py
+-rw-r--r--   0 liubo      (501) staff       (20)     3477 2023-06-28 09:14:30.000000 feapder-1.8.7b2/tests/test_playwright2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      660 2022-10-28 07:20:27.000000 feapder-1.8.7b2/tests/test_rander.py
+-rw-r--r--   0 liubo      (501) staff       (20)      769 2021-07-08 11:51:50.000000 feapder-1.8.7b2/tests/test_rander2.py
+-rw-r--r--   0 liubo      (501) staff       (20)      519 2022-09-14 07:25:07.000000 feapder-1.8.7b2/tests/test_rander3.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1983 2022-09-07 09:10:17.000000 feapder-1.8.7b2/tests/test_rander_xhr.py
+-rw-r--r--   0 liubo      (501) staff       (20)      148 2021-08-12 03:51:27.000000 feapder-1.8.7b2/tests/test_redisdb.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1634 2022-09-25 13:50:01.000000 feapder-1.8.7b2/tests/test_request.py
+-rw-r--r--   0 liubo      (501) staff       (20)      637 2021-04-08 03:41:12.000000 feapder-1.8.7b2/tests/test_spider_params.py
+-rw-r--r--   0 liubo      (501) staff       (20)      593 2022-07-25 12:58:57.000000 feapder-1.8.7b2/tests/test_task.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.837456 feapder-1.8.7b2/tests/test_template/
+-rw-r--r--   0 liubo      (501) staff       (20)     2336 2022-09-07 03:39:38.000000 feapder-1.8.7b2/tests/test_template/test_spider.py
+-rw-r--r--   0 liubo      (501) staff       (20)      429 2022-05-17 07:19:13.000000 feapder-1.8.7b2/tests/test_tools.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1011 2022-09-07 09:10:23.000000 feapder-1.8.7b2/tests/test_webdriver.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2023-07-10 08:01:51.852904 feapder-1.8.7b2/tests/user_pool/
+-rw-r--r--   0 liubo      (501) staff       (20)     2423 2022-06-10 02:51:23.000000 feapder-1.8.7b2/tests/user_pool/test_gold_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2121 2022-06-10 02:51:23.000000 feapder-1.8.7b2/tests/user_pool/test_guest_user_pool.py
+-rw-r--r--   0 liubo      (501) staff       (20)     1427 2022-06-10 02:51:23.000000 feapder-1.8.7b2/tests/user_pool/test_normal_user_pool.py
```

### Comparing `feapder-1.8.7b1/LICENSE` & `feapder-1.8.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/PKG-INFO` & `feapder-1.8.7b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.8.7b1
+Version: 1.8.7b2
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.8.7b1/README.md` & `feapder-1.8.7b2/README.md`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/__init__.py` & `feapder-1.8.7b2/feapder/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/buffer/item_buffer.py` & `feapder-1.8.7b2/feapder/buffer/item_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/buffer/request_buffer.py` & `feapder-1.8.7b2/feapder/buffer/request_buffer.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/cmdline.py` & `feapder-1.8.7b2/feapder/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/__init__.py` & `feapder-1.8.7b2/feapder/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_cookies.py` & `feapder-1.8.7b2/feapder/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_init.py` & `feapder-1.8.7b2/feapder/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_item.py` & `feapder-1.8.7b2/feapder/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_json.py` & `feapder-1.8.7b2/feapder/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_params.py` & `feapder-1.8.7b2/feapder/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_project.py` & `feapder-1.8.7b2/feapder/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_setting.py` & `feapder-1.8.7b2/feapder/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_spider.py` & `feapder-1.8.7b2/feapder/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create/create_table.py` & `feapder-1.8.7b2/feapder/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/create_builder.py` & `feapder-1.8.7b2/feapder/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/retry.py` & `feapder-1.8.7b2/feapder/commands/retry.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/shell.py` & `feapder-1.8.7b2/feapder/commands/shell.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/commands/zip.py` & `feapder-1.8.7b2/feapder/commands/zip.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/base_parser.py` & `feapder-1.8.7b2/feapder/core/base_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/collector.py` & `feapder-1.8.7b2/feapder/core/collector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/handle_failed_items.py` & `feapder-1.8.7b2/feapder/core/handle_failed_items.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/handle_failed_requests.py` & `feapder-1.8.7b2/feapder/core/handle_failed_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/parser_control.py` & `feapder-1.8.7b2/feapder/core/parser_control.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/scheduler.py` & `feapder-1.8.7b2/feapder/core/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,16 @@
             self._tab_spider_status, SPIDER_START_TIME_KEY, is_pop=True
         )
         if data:
             begin_timestamp = int(data)
 
             spand_time = tools.get_current_timestamp() - begin_timestamp
 
-            msg = "《%s》爬虫结束，耗时 %s" % (
+            msg = "《%s》爬虫%s，采集耗时 %s" % (
+                "被终止" if not self._keep_alive else "结束",
                 self._spider_name,
                 tools.format_seconds(spand_time),
             )
             log.info(msg)
 
             self.send_msg(msg)
```

### Comparing `feapder-1.8.7b1/feapder/core/spiders/air_spider.py` & `feapder-1.8.7b2/feapder/core/spiders/air_spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
 
                     # 关闭item_buffer
                     self._item_buffer.stop()
 
                     # 关闭webdirver
                     Request.render_downloader and Request.render_downloader.close_all()
 
-                    if self._stop:
-                        log.info("爬虫被停止")
+                    if self._stop_spider:
+                        log.info("爬虫被终止")
                     else:
                         log.info("无任务，爬虫结束")
                     break
 
             except Exception as e:
                 log.exception(e)
```

### Comparing `feapder-1.8.7b1/feapder/core/spiders/batch_spider.py` & `feapder-1.8.7b2/feapder/core/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/spiders/spider.py` & `feapder-1.8.7b2/feapder/core/spiders/spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/core/spiders/task_spider.py` & `feapder-1.8.7b2/feapder/core/spiders/task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/db/memorydb.py` & `feapder-1.8.7b2/feapder/db/memorydb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/db/mongodb.py` & `feapder-1.8.7b2/feapder/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/db/mysqldb.py` & `feapder-1.8.7b2/feapder/db/mysqldb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/db/redisdb.py` & `feapder-1.8.7b2/feapder/db/redisdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,19 +591,19 @@
     def lpush(self, table, values):
         if isinstance(values, list):
             pipe = self._redis.pipeline()
 
             if not self._is_redis_cluster:
                 pipe.multi()
             for value in values:
-                pipe.rpush(table, value)
+                pipe.lpush(table, value)
             pipe.execute()
 
         else:
-            return self._redis.rpush(table, values)
+            return self._redis.lpush(table, values)
 
     def lpop(self, table, count=1):
         """
         @summary:
         ---------
         @param table:
         @param count:
```

### Comparing `feapder-1.8.7b1/feapder/dedup/__init__.py` & `feapder-1.8.7b2/feapder/dedup/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/dedup/basefilter.py` & `feapder-1.8.7b2/feapder/dedup/basefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/dedup/bitarray.py` & `feapder-1.8.7b2/feapder/dedup/bitarray.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/dedup/bloomfilter.py` & `feapder-1.8.7b2/feapder/dedup/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/dedup/expirefilter.py` & `feapder-1.8.7b2/feapder/dedup/expirefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/dedup/litefilter.py` & `feapder-1.8.7b2/feapder/dedup/litefilter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/downloader/_playwright.py` & `feapder-1.8.7b2/feapder/network/downloader/_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/downloader/_requests.py` & `feapder-1.8.7b2/feapder/network/downloader/_requests.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/downloader/_selenium.py` & `feapder-1.8.7b2/feapder/network/downloader/_selenium.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/downloader/base.py` & `feapder-1.8.7b2/feapder/network/downloader/base.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/item.py` & `feapder-1.8.7b2/feapder/network/item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/proxy_pool.py` & `feapder-1.8.7b2/feapder/network/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/proxy_pool_old.py` & `feapder-1.8.7b2/feapder/network/proxy_pool_old.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/request.py` & `feapder-1.8.7b2/feapder/network/request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/response.py` & `feapder-1.8.7b2/feapder/network/response.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/selector.py` & `feapder-1.8.7b2/feapder/network/selector.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/user_agent.py` & `feapder-1.8.7b2/feapder/network/user_agent.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/user_pool/base_user_pool.py` & `feapder-1.8.7b2/feapder/network/user_pool/base_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/user_pool/gold_user_pool.py` & `feapder-1.8.7b2/feapder/network/user_pool/gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/user_pool/guest_user_pool.py` & `feapder-1.8.7b2/feapder/network/user_pool/guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/network/user_pool/normal_user_pool.py` & `feapder-1.8.7b2/feapder/network/user_pool/normal_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/pipelines/__init__.py` & `feapder-1.8.7b2/feapder/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/pipelines/console_pipeline.py` & `feapder-1.8.7b2/feapder/pipelines/console_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/pipelines/mongo_pipeline.py` & `feapder-1.8.7b2/feapder/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/pipelines/mysql_pipeline.py` & `feapder-1.8.7b2/feapder/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/setting.py` & `feapder-1.8.7b2/feapder/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/.DS_Store` & `feapder-1.8.7b2/feapder/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/air_spider_template.tmpl` & `feapder-1.8.7b2/feapder/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/batch_spider_template.tmpl` & `feapder-1.8.7b2/feapder/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/project_template/.DS_Store` & `feapder-1.8.7b2/feapder/templates/project_template/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/project_template/CHECK_DATA.md` & `feapder-1.8.7b2/feapder/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/project_template/main.py` & `feapder-1.8.7b2/feapder/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/project_template/setting.py` & `feapder-1.8.7b2/feapder/templates/project_template/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/spider_template.tmpl` & `feapder-1.8.7b2/feapder/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/templates/task_spider_template.tmpl` & `feapder-1.8.7b2/feapder/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/custom_argparse.py` & `feapder-1.8.7b2/feapder/utils/custom_argparse.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/email_sender.py` & `feapder-1.8.7b2/feapder/utils/email_sender.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/js/intercept.js` & `feapder-1.8.7b2/feapder/utils/js/intercept.js`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/js/stealth.min.js` & `feapder-1.8.7b2/feapder/utils/js/stealth.min.js`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/log.py` & `feapder-1.8.7b2/feapder/utils/log.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/metrics.py` & `feapder-1.8.7b2/feapder/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/perfect_dict.py` & `feapder-1.8.7b2/feapder/utils/perfect_dict.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/redis_lock.py` & `feapder-1.8.7b2/feapder/utils/redis_lock.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/tools.py` & `feapder-1.8.7b2/feapder/utils/tools.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/webdriver/playwright_driver.py` & `feapder-1.8.7b2/feapder/utils/webdriver/playwright_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.driver: Playwright = None
         self.browser: Browser = None
         self.context: BrowserContext = None
         self.page: Page = None
         self.url = None
         self.storage_state_path = storage_state_path
 
-        self._driver_type = driver_type
+        self._driver_type = driver_type or "chromium"
         self._page_on_event_callback = page_on_event_callback
         self._url_regexes = url_regexes
         self._save_all = save_all
 
         if self._save_all and self._url_regexes:
             log.warning(
                 "获取完拦截的数据后, 请主动调用PlaywrightDriver的clear_cache()方法清空拦截的数据，否则数据会一直累加，导致内存溢出"
```

### Comparing `feapder-1.8.7b1/feapder/utils/webdriver/selenium_driver.py` & `feapder-1.8.7b2/feapder/utils/webdriver/selenium_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
         Args:
             xhr_url_regexes: 拦截xhr接口，支持正则，数组类型
             **kwargs:
         """
         super(SeleniumDriver, self).__init__(**kwargs)
         self._xhr_url_regexes = xhr_url_regexes
+        self._driver_type = self._driver_type or SeleniumDriver.CHROME
 
         if self._xhr_url_regexes and self._driver_type != SeleniumDriver.CHROME:
             raise Exception(
                 "xhr_url_regexes only support by chrome now! eg: driver_type=SeleniumDriver.CHROME"
             )
 
         if self._driver_type == SeleniumDriver.CHROME:
```

### Comparing `feapder-1.8.7b1/feapder/utils/webdriver/webdirver.py` & `feapder-1.8.7b2/feapder/utils/webdriver/webdirver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder/utils/webdriver/webdriver_pool.py` & `feapder-1.8.7b2/feapder/utils/webdriver/webdriver_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/feapder.egg-info/PKG-INFO` & `feapder-1.8.7b2/feapder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feapder
-Version: 1.8.7b1
+Version: 1.8.7b2
 Summary: feapder是一款支持分布式、批次采集、数据防丢、报警丰富的python爬虫框架
 Home-page: https://github.com/Boris-code/feapder.git
 Author: Boris
 Author-email: feapder@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `feapder-1.8.7b1/feapder.egg-info/SOURCES.txt` & `feapder-1.8.7b2/feapder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/setup.py` & `feapder-1.8.7b2/setup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/air-spider/test_air_spider.py` & `feapder-1.8.7b2/tests/air-spider/test_air_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/air-spider/test_air_spider_filter.py` & `feapder-1.8.7b2/tests/air-spider/test_air_spider_filter.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/air-spider/test_air_spider_item.py` & `feapder-1.8.7b2/tests/air-spider/test_air_spider_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/air-spider/test_render_spider.py` & `feapder-1.8.7b2/tests/air-spider/test_render_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider/items/spider_data_item.py` & `feapder-1.8.7b2/tests/batch-spider/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider/main.py` & `feapder-1.8.7b2/tests/batch-spider/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider/setting.py` & `feapder-1.8.7b2/tests/batch-spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider/spiders/test_spider.py` & `feapder-1.8.7b2/tests/batch-spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider/table.sql` & `feapder-1.8.7b2/tests/batch-spider/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider-integration/batch_spider_integration_task.sql` & `feapder-1.8.7b2/tests/batch-spider-integration/batch_spider_integration_task.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider-integration/main.py` & `feapder-1.8.7b2/tests/batch-spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider-integration/setting.py` & `feapder-1.8.7b2/tests/batch-spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider-integration/spiders/sina_news_parser.py` & `feapder-1.8.7b2/tests/batch-spider-integration/spiders/sina_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/batch-spider-integration/spiders/tencent_news_parser.py` & `feapder-1.8.7b2/tests/batch-spider-integration/spiders/tencent_news_parser.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/jd_spider.py` & `feapder-1.8.7b2/tests/jd_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/mongo_spider.py` & `feapder-1.8.7b2/tests/mongo_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider/log/haha.log` & `feapder-1.8.7b2/tests/spider/log/haha.log`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider/setting.py` & `feapder-1.8.7b2/tests/spider/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider/spiders/test_spider.py` & `feapder-1.8.7b2/tests/spider/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider/spiders/test_spider2.py` & `feapder-1.8.7b2/tests/spider/spiders/test_spider2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider-integration/main.py` & `feapder-1.8.7b2/tests/spider-integration/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/spider-integration/setting.py` & `feapder-1.8.7b2/tests/spider-integration/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/task-spider/test_task_spider.py` & `feapder-1.8.7b2/tests/task-spider/test_task_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-debugger/.DS_Store` & `feapder-1.8.7b2/tests/test-debugger/.DS_Store`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-debugger/setting.py` & `feapder-1.8.7b2/tests/test-debugger/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-debugger/spiders/test_debugger.py` & `feapder-1.8.7b2/tests/test-debugger/spiders/test_debugger.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/items/spider_data_item.py` & `feapder-1.8.7b2/tests/test-pipeline/items/spider_data_item.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/main.py` & `feapder-1.8.7b2/tests/test-pipeline/main.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/pipeline.py` & `feapder-1.8.7b2/tests/test-pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/setting.py` & `feapder-1.8.7b2/tests/test-pipeline/setting.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/spiders/test_spider.py` & `feapder-1.8.7b2/tests/test-pipeline/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test-pipeline/table.sql` & `feapder-1.8.7b2/tests/test-pipeline/table.sql`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_dedup.py` & `feapder-1.8.7b2/tests/test_dedup.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_metrics.py` & `feapder-1.8.7b2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_mongodb.py` & `feapder-1.8.7b2/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_playwright.py` & `feapder-1.8.7b2/tests/test_playwright.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_playwright2.py` & `feapder-1.8.7b2/tests/test_playwright2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_rander.py` & `feapder-1.8.7b2/tests/test_rander.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_rander2.py` & `feapder-1.8.7b2/tests/test_rander2.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_rander3.py` & `feapder-1.8.7b2/tests/test_rander3.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_rander_xhr.py` & `feapder-1.8.7b2/tests/test_rander_xhr.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_request.py` & `feapder-1.8.7b2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_spider_params.py` & `feapder-1.8.7b2/tests/test_spider_params.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_task.py` & `feapder-1.8.7b2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_template/test_spider.py` & `feapder-1.8.7b2/tests/test_template/test_spider.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/test_webdriver.py` & `feapder-1.8.7b2/tests/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/user_pool/test_gold_user_pool.py` & `feapder-1.8.7b2/tests/user_pool/test_gold_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/user_pool/test_guest_user_pool.py` & `feapder-1.8.7b2/tests/user_pool/test_guest_user_pool.py`

 * *Files identical despite different names*

### Comparing `feapder-1.8.7b1/tests/user_pool/test_normal_user_pool.py` & `feapder-1.8.7b2/tests/user_pool/test_normal_user_pool.py`

 * *Files identical despite different names*

