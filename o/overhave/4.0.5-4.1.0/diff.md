# Comparing `tmp/overhave-4.0.5.tar.gz` & `tmp/overhave-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-4.0.5.tar", max compression
+gzip compressed data, was "overhave-4.1.0.tar", max compression
```

## Comparing `overhave-4.0.5.tar` & `overhave-4.1.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0    23136 2023-07-06 06:26:56.936672 overhave-4.0.5/README.rst
--rw-r--r--   0        0        0     3193 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/__init__.py
--rw-r--r--   0        0        0       63 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5172 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      287 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0     2134 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10071 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      465 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1535 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3407 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0    10257 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     4997 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      631 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1404 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1648 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1578 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     2645 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1329 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3665 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/api/__init__.py
--rw-r--r--   0        0        0     5970 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/api/app.py
--rw-r--r--   0        0        0      216 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1271 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      867 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/token.py
--rw-r--r--   0        0        0     2422 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/settings.py
--rw-r--r--   0        0        0      580 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1304 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      550 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0      461 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/feature_type_views.py
--rw-r--r--   0        0        0     1184 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      969 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     2041 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4486 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     4047 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/__init__.py
--rw-r--r--   0        0        0      557 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/api.py
--rw-r--r--   0        0        0      647 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1755 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/s3.py
--rw-r--r--   0        0        0     1573 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      455 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/base.py
--rw-r--r--   0        0        0     1349 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/statuses.py
--rw-r--r--   0        0        0     8141 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/tables.py
--rw-r--r--   0        0        0      795 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/users.py
--rw-r--r--   0        0        0     1249 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     4103 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      897 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      316 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      557 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     2891 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1394 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1258 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      425 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2748 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1098 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1198 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      415 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5825 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     6633 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7209 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4555 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0     1312 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3956 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2184 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1888 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     2045 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2950 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     4028 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      506 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2032 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1288 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2519 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/getters.py
--rw-r--r--   0        0        0      353 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/__init__.py
--rw-r--r--   0        0        0      193 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/client/__init__.py
--rw-r--r--   0        0        0     3140 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/client/container.py
--rw-r--r--   0        0        0      983 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/getters.py
--rw-r--r--   0        0        0      342 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/__init__.py
--rw-r--r--   0        0        0      399 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4015 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0      532 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/errors.py
--rw-r--r--   0        0        0     4928 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4208 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1408 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2157 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0     1015 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      178 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/objects.py
--rw-r--r--   0        0        0      877 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1672 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     4323 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3538 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      927 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1102 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1260 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2452 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1638 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      981 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2874 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     6192 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2223 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3945 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      517 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5173 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3495 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2820 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      854 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8442 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0       95 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/__init__.py
--rw-r--r--   0        0        0      229 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/abstract.py
--rw-r--r--   0        0        0     1441 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/duplicate_id_mixin.py
--rw-r--r--   0        0        0      510 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/errors.py
--rw-r--r--   0        0        0     2827 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/validator.py
--rw-r--r--   0        0        0     1226 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3271 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/converters.py
--rw-r--r--   0        0        0     6178 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     5323 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4947 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1566 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     2176 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     1902 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      593 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     2464 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     3054 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     4451 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3702 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     6973 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      307 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4256 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/executor.py
--rw-r--r--   0        0        0     1056 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1750 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     4106 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1617 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      983 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/__init__.py
--rw-r--r--   0        0        0      623 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      499 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      590 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2139 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      110 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0     1287 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      258 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     2003 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0      609 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      377 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      741 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2757 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      569 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      430 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     1661 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/deps.py
--rw-r--r--   0        0        0     2439 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1319 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1384 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0     1674 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/settings.py
--rw-r--r--   0        0        0      132 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2082 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      885 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/time.py
--rw-r--r--   0        0        0      148 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/url.py
--rw-r--r--   0        0        0     3522 2023-07-06 06:26:56.960672 overhave-4.0.5/pyproject.toml
--rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0    23136 2023-07-10 05:49:29.631843 overhave-4.1.0/README.rst
+-rw-r--r--   0        0        0     3193 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5172 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      287 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0     2112 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10071 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      465 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1535 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3407 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0    10257 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      631 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1404 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1648 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1578 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     2645 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1329 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3665 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/__init__.py
+-rw-r--r--   0        0        0     5970 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/app.py
+-rw-r--r--   0        0        0      216 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1395 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      867 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     2422 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/deps.py
+-rw-r--r--   0        0        0      848 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/settings.py
+-rw-r--r--   0        0        0      580 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1416 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      550 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      461 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1184 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      969 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     2041 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4486 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     4047 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/admin.py
+-rw-r--r--   0        0        0      534 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/api.py
+-rw-r--r--   0        0        0      647 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1755 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1573 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      455 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/base.py
+-rw-r--r--   0        0        0     1349 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/statuses.py
+-rw-r--r--   0        0        0     8141 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/tables.py
+-rw-r--r--   0        0        0      795 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/users.py
+-rw-r--r--   0        0        0     1249 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     4103 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      897 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      316 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      754 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1487 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1396 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2748 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1098 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5825 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     6633 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7209 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4555 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0     1312 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3956 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2184 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1888 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     2045 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2950 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     4028 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      506 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2032 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1288 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2519 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/getters.py
+-rw-r--r--   0        0        0      353 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/client/__init__.py
+-rw-r--r--   0        0        0     3162 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/client/container.py
+-rw-r--r--   0        0        0      983 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/getters.py
+-rw-r--r--   0        0        0      342 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      399 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4015 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0      532 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/errors.py
+-rw-r--r--   0        0        0     4928 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4208 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1408 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2157 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0     1015 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      178 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/objects.py
+-rw-r--r--   0        0        0      877 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1672 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     4323 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3538 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1102 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1260 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2452 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1638 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      981 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2874 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     6192 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2223 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3945 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      517 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5100 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3495 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2820 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8442 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0       95 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/abstract.py
+-rw-r--r--   0        0        0     1441 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/duplicate_id_mixin.py
+-rw-r--r--   0        0        0      510 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/errors.py
+-rw-r--r--   0        0        0     2827 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/validator.py
+-rw-r--r--   0        0        0     1226 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3271 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/converters.py
+-rw-r--r--   0        0        0     6178 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     5323 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4947 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1566 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2176 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     1902 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      589 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     1930 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     3054 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     4451 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3728 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     7025 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      307 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4256 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0     1056 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1750 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     4106 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1617 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      983 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      237 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      499 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2139 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      110 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0     1287 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      258 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     2003 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0      609 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      377 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      741 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2115 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2757 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      569 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      420 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      430 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     1661 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/deps.py
+-rw-r--r--   0        0        0     2439 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1319 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1384 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0     1674 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/settings.py
+-rw-r--r--   0        0        0      132 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8494 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2082 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0      885 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/time.py
+-rw-r--r--   0        0        0      148 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/url.py
+-rw-r--r--   0        0        0     3522 2023-07-10 05:49:29.659843 overhave-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.1.0/PKG-INFO
```

### Comparing `overhave-4.0.5/README.rst` & `overhave-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/__init__.py` & `overhave-4.1.0/overhave/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/app.py` & `overhave-4.1.0/overhave/admin/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/files/ace-src/ace.js` & `overhave-4.1.0/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-4.1.0/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/files/css/overhave.css` & `overhave-4.1.0/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/files/favicon.ico` & `overhave-4.1.0/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/flask/flask_admin.py` & `overhave-4.1.0/overhave/admin/flask/flask_admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/flask/login_manager.py` & `overhave-4.1.0/overhave/admin/flask/login_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
+from dataclasses import dataclass
 
 from flask import redirect
 from flask_login import LoginManager
-from pydantic import BaseModel
 from werkzeug import Response
 
 from overhave import db
 from overhave.storage import ISystemUserStorage, SystemUserModel
 
 logger = logging.getLogger(__name__)
 
 
 class UnauthorizedUserError(Exception):
     """Raises when user is not authorized and trying to get user fields such as role or login."""
 
 
-class AdminPanelUser(BaseModel):
+@dataclass(frozen=True)
+class AdminPanelUser:
     """SystemUserModel wrapper for flask_login."""
 
     user_data: SystemUserModel | None
 
     @property
     def is_authenticated(self) -> bool:
         return self.user_data is not None
@@ -28,29 +29,30 @@
     def is_active(self) -> bool:
         return True
 
     @property
     def is_anonymous(self) -> bool:
         return self.user_data is None
 
+    @property
+    def _authorized_user(self) -> SystemUserModel:
+        if self.user_data is None:
+            raise UnauthorizedUserError("User is not authorized!")
+        return self.user_data
+
     def get_id(self) -> int:
-        return self._get_authorized_user_or_raise().id
+        return self._authorized_user.id
 
     @property
     def login(self) -> str:
-        return self._get_authorized_user_or_raise().login
+        return self._authorized_user.login
 
     @property
     def role(self) -> db.Role:
-        return self._get_authorized_user_or_raise().role
-
-    def _get_authorized_user_or_raise(self) -> SystemUserModel:
-        if self.user_data is None:
-            raise UnauthorizedUserError("User is not authorized!")
-        return self.user_data
+        return self._authorized_user.role
 
     def __unicode__(self) -> str:
         if self.user_data is not None:
             return self.user_data.login
         return "anonymous"
 
 
@@ -63,11 +65,11 @@
         self.user_loader(self._get_user)
         self.unauthorized_handler(self._unathorized_response)
 
         self._system_user_storage = system_user_storage
 
     def _get_user(self, user_id: int) -> AdminPanelUser:
         logger.info("Get user by id=%s...", user_id)
-        return AdminPanelUser(user_data=self._system_user_storage.get_user(user_id=user_id))
+        return AdminPanelUser(user_data=self._system_user_storage.get_user_model(user_id=user_id))
 
     def _unathorized_response(self) -> Response:
         return redirect(f"/{self.login_view}")
```

### Comparing `overhave-4.0.5/overhave/admin/templates/emulation_run_detail.html` & `overhave-4.1.0/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/templates/feature.html` & `overhave-4.1.0/overhave/admin/templates/feature.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/templates/login.html` & `overhave-4.1.0/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/templates/test_run.html` & `overhave-4.1.0/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/templates/test_run_detail.html` & `overhave-4.1.0/overhave/admin/templates/test_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/templates/test_user.html` & `overhave-4.1.0/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/access.py` & `overhave-4.1.0/overhave/admin/views/access.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/base.py` & `overhave-4.1.0/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/draft.py` & `overhave-4.1.0/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/emulation.py` & `overhave-4.1.0/overhave/admin/views/emulation.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/emulation_run.py` & `overhave-4.1.0/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/feature.py` & `overhave-4.1.0/overhave/admin/views/feature.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/formatters/formatters.py` & `overhave-4.1.0/overhave/admin/views/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/formatters/helpers.py` & `overhave-4.1.0/overhave/admin/views/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/formatters/safe_formatter.py` & `overhave-4.1.0/overhave/admin/views/formatters/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/index/custom_page.py` & `overhave-4.1.0/overhave/admin/views/index/custom_page.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/index/login_form.py` & `overhave-4.1.0/overhave/admin/views/index/login_form.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/index/view.py` & `overhave-4.1.0/overhave/admin/views/index/view.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/scenario_test_run.py` & `overhave-4.1.0/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/tag.py` & `overhave-4.1.0/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/admin/views/testing_users.py` & `overhave-4.1.0/overhave/admin/views/testing_users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/app.py` & `overhave-4.1.0/overhave/api/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/auth/regular.py` & `overhave-4.1.0/overhave/api/auth/regular.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from http import HTTPStatus
 
 import fastapi
 from fastapi import security as fastapi_security
 from jose import JWTError
 
+from overhave import db
 from overhave.api.auth.models import AUTH_HEADERS
 from overhave.api.auth.token import get_token_data
 from overhave.api.deps import get_api_auth_settings, get_system_user_storage
 from overhave.api.settings import OverhaveApiAuthSettings
 from overhave.storage import ISystemUserStorage, SystemUserModel
 
 oauth2_scheme = fastapi_security.OAuth2PasswordBearer(tokenUrl="token")
@@ -25,11 +26,12 @@
     )
     try:
         token_data = get_token_data(auth_settings=auth_settings, token=token)
         if token_data is None:
             raise creds_exception
     except JWTError:
         raise creds_exception
-    user = storage.get_user_by_credits(login=token_data.username)
-    if user is None:
-        raise creds_exception
-    return user
+    with db.create_session() as session:
+        user = storage.get_user_by_credits(session=session, login=token_data.username)
+        if user is None:
+            raise creds_exception
+        return SystemUserModel.from_orm(user)
```

### Comparing `overhave-4.0.5/overhave/api/auth/token.py` & `overhave-4.1.0/overhave/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/deps.py` & `overhave-4.1.0/overhave/api/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/settings.py` & `overhave-4.1.0/overhave/api/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/__init__.py` & `overhave-4.1.0/overhave/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/auth_views.py` & `overhave-4.1.0/overhave/api/views/auth_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from http import HTTPStatus
 
 import fastapi
 from fastapi import security as fastapi_security
 from pydantic.types import SecretStr
 
+from overhave import db
 from overhave.api.auth import AUTH_HEADERS, create_access_token
 from overhave.api.deps import get_api_auth_settings, get_system_user_storage
 from overhave.api.settings import OverhaveApiAuthSettings
 from overhave.storage import AuthToken, ISystemUserStorage
 from overhave.utils import get_current_time
 
 
 def login_for_access_token(
     form_data: fastapi_security.OAuth2PasswordRequestForm = fastapi.Depends(),
     auth_settings: OverhaveApiAuthSettings = fastapi.Depends(get_api_auth_settings),
     storage: ISystemUserStorage = fastapi.Depends(get_system_user_storage),
 ) -> AuthToken:
-    user = storage.get_user_by_credits(login=form_data.username, password=SecretStr(form_data.password))
-    if not user:
-        raise fastapi.HTTPException(
-            status_code=HTTPStatus.UNAUTHORIZED,
-            detail="Incorrect username or password",
-            headers=AUTH_HEADERS.dict(),
-        )
+    with db.create_session() as session:
+        if not storage.get_user_by_credits(
+            session=session, login=form_data.username, password=SecretStr(form_data.password)
+        ):
+            raise fastapi.HTTPException(
+                status_code=HTTPStatus.UNAUTHORIZED,
+                detail="Incorrect username or password",
+                headers=AUTH_HEADERS.dict(),
+            )
     expires_at = get_current_time() + auth_settings.access_token_expire_timedelta
     access_token = create_access_token(auth_settings=auth_settings, username=form_data.username, expires_at=expires_at)
     return AuthToken(access_token=access_token, expires_at=expires_at)
```

### Comparing `overhave-4.0.5/overhave/api/views/emulation_views.py` & `overhave-4.1.0/overhave/api/views/emulation_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/extra_views.py` & `overhave-4.1.0/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/feature_views.py` & `overhave-4.1.0/overhave/api/views/feature_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/tags_views.py` & `overhave-4.1.0/overhave/api/views/tags_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/testrun_views.py` & `overhave-4.1.0/overhave/api/views/testrun_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/api/views/testuser_views.py` & `overhave-4.1.0/overhave/api/views/testuser_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/base_settings.py` & `overhave-4.1.0/overhave/base_settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/admin.py` & `overhave-4.1.0/overhave/cli/admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/api.py` & `overhave-4.1.0/overhave/cli/api.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/consumers.py` & `overhave-4.1.0/overhave/cli/consumers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/db_cmds/group.py` & `overhave-4.1.0/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/db_cmds/regular.py` & `overhave-4.1.0/overhave/cli/db_cmds/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/s3.py` & `overhave-4.1.0/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/cli/synchronizer.py` & `overhave-4.1.0/overhave/cli/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/db/base.py` & `overhave-4.1.0/overhave/db/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/db/statuses.py` & `overhave-4.1.0/overhave/db/statuses.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/db/tables.py` & `overhave-4.1.0/overhave/db/tables.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/db/users.py` & `overhave-4.1.0/overhave/db/users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/db/utils.py` & `overhave-4.1.0/overhave/db/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/emulation/emulator.py` & `overhave-4.1.0/overhave/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/__init__.py` & `overhave-4.1.0/overhave/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/archiver.py` & `overhave-4.1.0/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/auth_managers/secret_mixin.py` & `overhave-4.1.0/overhave/entities/auth_managers/secret_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         self._make_secret()
 
     @staticmethod
     def _get_secret() -> SecretStr:
         return SecretStr(uuid4().hex)
 
     def _make_secret(self) -> None:
-        user = self._system_user_storage.get_user_by_credits(login=_ADMIN_USERNAME)
-        if user is not None:
-            logger.info("Admin user already exists")
-            return
         secret = self._get_secret()
+        with db.create_session() as session:
+            if self._system_user_storage.get_user_by_credits(session=session, login=_ADMIN_USERNAME):
+                logger.info("Admin user already exists")
+                return
+            self._system_user_storage.create_user(
+                session=session, login=_ADMIN_USERNAME, password=secret, role=db.Role.admin
+            )
         logger.info("Generated admin secret: %s", secret.get_secret_value())
-        self._system_user_storage.create_user(login=_ADMIN_USERNAME, password=secret, role=db.Role.admin)
```

### Comparing `overhave-4.0.5/overhave/entities/auth_managers/simple.py` & `overhave-4.1.0/overhave/entities/auth_managers/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from pydantic import SecretStr
 
+from overhave import db
 from overhave.entities.auth_managers.secret_mixin import AdminSecretMixin
 from overhave.storage import SystemUserModel
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSimpleAdminAuthorizationManagerException(Exception):
@@ -20,15 +21,16 @@
     """Class for user registration.
 
     Manager does not provide real auth_managers. Each user could use preferred name.
     This name will be used for user authority. Each user is unique. Passwords not required.
     """
 
     def authorize_user(self, username: str, password: SecretStr) -> SystemUserModel | None:
-        user = self._system_user_storage.get_user_by_credits(login=username)
-        if user is None:
-            user = self._system_user_storage.create_user(login=username, password=password)
-        if user.password is None:
-            raise NullablePasswordError(f"User with id={user.id} has not got password!")
-        if user.password.get_secret_value() == password.get_secret_value():
-            return user
+        with db.create_session() as session:
+            user = self._system_user_storage.get_user_by_credits(session=session, login=username)
+            if user is None:
+                user = self._system_user_storage.create_user(session=session, login=username, password=password)
+            if user.password is None:
+                raise NullablePasswordError(f"User with id={user.id} has not got password!")
+            if user.password == password.get_secret_value():
+                return SystemUserModel.from_orm(user)
         return None
```

### Comparing `overhave-4.0.5/overhave/entities/feature/extractor.py` & `overhave-4.1.0/overhave/entities/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/file_extractor.py` & `overhave-4.1.0/overhave/entities/file_extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/git_initializer.py` & `overhave-4.1.0/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/language/prefixes.py` & `overhave-4.1.0/overhave/entities/language/prefixes.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/report_manager/report_manager.py` & `overhave-4.1.0/overhave/entities/report_manager/report_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/entities/settings.py` & `overhave-4.1.0/overhave/entities/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/__init__.py` & `overhave-4.1.0/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/base_factory.py` & `overhave-4.1.0/overhave/factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/components/admin_factory.py` & `overhave-4.1.0/overhave/factory/components/admin_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/components/emulation_factory.py` & `overhave-4.1.0/overhave/factory/components/emulation_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/components/publication_factory.py` & `overhave-4.1.0/overhave/factory/components/publication_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/components/synchronizer_factory.py` & `overhave-4.1.0/overhave/factory/components/synchronizer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/components/test_execution_factory.py` & `overhave-4.1.0/overhave/factory/components/test_execution_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/consumer_factory.py` & `overhave-4.1.0/overhave/factory/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/__init__.py` & `overhave-4.1.0/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/admin_context.py` & `overhave-4.1.0/overhave/factory/context/admin_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/base_context.py` & `overhave-4.1.0/overhave/factory/context/base_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/publication_context.py` & `overhave-4.1.0/overhave/factory/context/publication_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/synchronizer_context.py` & `overhave-4.1.0/overhave/factory/context/synchronizer_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/context/test_execution_context.py` & `overhave-4.1.0/overhave/factory/context/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/factory/getters.py` & `overhave-4.1.0/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/metrics/client/container.py` & `overhave-4.1.0/overhave/metrics/client/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     def consume_redis_task(self, task_type: str) -> None:
         self.consumed_redis_tasks.labels(task_type=task_type).inc()
 
 
 class TestRunOverhaveMetricContainer(BaseOverhaveMetricContainer):
     """Overhave prometheus metric container for test runs."""
 
+    __test__ = False
+
     def __init__(self, registry: CollectorRegistry):
         super().__init__(registry=registry)
         self._init_test_run_metrics()
 
     def _init_test_run_metrics(self) -> None:
         self.test_run_tasks_statuses = Counter(
             "test_run_tasks_statuses",
```

### Comparing `overhave-4.0.5/overhave/metrics/getters.py` & `overhave-4.1.0/overhave/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/base_publisher.py` & `overhave-4.1.0/overhave/publication/base_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/errors.py` & `overhave-4.1.0/overhave/publication/errors.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/git_publisher.py` & `overhave-4.1.0/overhave/publication/git_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-4.1.0/overhave/publication/gitlab/gitlab_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/gitlab/settings.py` & `overhave-4.1.0/overhave/publication/gitlab/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/gitlab/tokenizer/client.py` & `overhave-4.1.0/overhave/publication/gitlab/tokenizer/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/gitlab/tokenizer/settings.py` & `overhave-4.1.0/overhave/publication/gitlab/tokenizer/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/settings.py` & `overhave-4.1.0/overhave/publication/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/stash/settings.py` & `overhave-4.1.0/overhave/publication/stash/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/publication/stash/stash_publisher.py` & `overhave-4.1.0/overhave/publication/stash/stash_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/config_injector.py` & `overhave-4.1.0/overhave/pytest_plugin/config_injector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/deps.py` & `overhave-4.1.0/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/__init__.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-4.1.0/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/plugin.py` & `overhave-4.1.0/overhave/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/plugin_resolver.py` & `overhave-4.1.0/overhave/pytest_plugin/plugin_resolver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/pytest_plugin/proxy_manager.py` & `overhave-4.1.0/overhave/pytest_plugin/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/__init__.py` & `overhave-4.1.0/overhave/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/compiler/compiler.py` & `overhave-4.1.0/overhave/scenario/compiler/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from typing import Sequence
+
 import allure
 from pytest_bdd import types as default_types
 
 from overhave.entities import OverhaveLanguageSettings
 from overhave.scenario.compiler.settings import OverhaveScenarioCompilerSettings
 from overhave.scenario.prefix_mixin import PrefixMixin
-from overhave.storage import TestExecutorContext
+from overhave.storage import TagModel, TestExecutorContext
 
 
 def generate_task_info(tasks: list[str], header: str | None) -> str:
     if tasks and header is not None:
         return f"{header}: {', '.join(tasks)}"
     return ""
 
 
-def generate_tags_list(context: TestExecutorContext) -> list[str] | None:
-    if feature_tags := [i.value for i in context.feature.feature_tags]:
-        return feature_tags
-    return None
+def _join_all_tags(lines: Sequence[str]) -> str:
+    return " ".join(lines).replace("  ", " ")
 
 
 class ScenarioCompilerError(Exception):
     """Base exception for :class:`ScenarioCompiler` errors."""
 
 
 class IncorrectScenarioTextError(ScenarioCompilerError):
@@ -41,21 +41,17 @@
         self._tasks_keyword = tasks_keyword
 
     def _get_feature_type_tag(self, scenario_text: str, tag: str) -> str:
         if f"{self._compilation_settings.tag_prefix}{tag}" in scenario_text:
             return ""
         return f"{self._compilation_settings.tag_prefix}{tag}"
 
-    def _get_additional_tags(self, scenario_text: str, tags: list[str] | None) -> str:
-        if f"{self._compilation_settings.tag_prefix}{tags}" in scenario_text:
-            return ""
-        if tags is not None:
-            tags_with_prefix = (f"{self._compilation_settings.tag_prefix}{tag}" for tag in tags)
-            return f"{' '.join(tags_with_prefix)}"
-        return ""
+    def _get_additional_tags(self, scenario_text: str, tags: list[TagModel]) -> str:
+        tags_with_prefix = (f"{self._compilation_settings.tag_prefix}{tag.value}" for tag in tags)
+        return f"{' '.join(tag for tag in tags_with_prefix if tag not in scenario_text)}"
 
     def _get_severity_tag(self, severity: allure.severity_level) -> str:
         return f"{self._compilation_settings.severity_prefix}{severity.value}"
 
     def _get_feature_prefix_if_specified(self, scenario_text: str) -> str | None:
         keywords: list[str] = [default_types.FEATURE]
         if self._language_settings.step_prefixes is not None:
@@ -87,19 +83,24 @@
         text = context.scenario.text
         feature_prefix = self._get_feature_prefix_if_specified(scenario_text=text)
         if not feature_prefix:
             feature_prefix = self._detect_feature_prefix_by_scenario_format(scenario_text=text)
         blocks_delimiter = f" {self._compilation_settings.blocks_delimiter} "
         if context.test_run.start is None:
             raise RuntimeError
+        joined_tags = _join_all_tags(
+            (
+                self._get_feature_type_tag(scenario_text=text, tag=context.feature.feature_type.name),
+                self._get_additional_tags(scenario_text=text, tags=context.feature.feature_tags),
+                self._get_severity_tag(severity=context.feature.severity),
+            )
+        )
         return "\n".join(
             (
-                f"{self._get_feature_type_tag(scenario_text=text, tag=context.feature.feature_type.name)} "
-                f"{self._get_additional_tags(scenario_text=text, tags=generate_tags_list(context))} "
-                f"{self._get_severity_tag(severity=context.feature.severity)}",
+                joined_tags,
                 f"{self._as_prefix(feature_prefix)} {context.feature.name}",
                 f"{self._compilation_settings.id_prefix} {context.feature.id}",
                 (
                     f"{self._compilation_settings.created_by_prefix} {context.feature.author}"
                     f"{blocks_delimiter}"
                     f"{self._compilation_settings.last_edited_by_prefix} {context.feature.last_edited_by}"
                     f"{self._compilation_settings.time_delimiter} "
```

### Comparing `overhave-4.0.5/overhave/scenario/compiler/settings.py` & `overhave-4.1.0/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/file_manager/file_manager.py` & `overhave-4.1.0/overhave/scenario/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/file_manager/settings.py` & `overhave-4.1.0/overhave/scenario/file_manager/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/parser/models.py` & `overhave-4.1.0/overhave/scenario/parser/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/parser/parser.py` & `overhave-4.1.0/overhave/scenario/parser/parser.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/validator/duplicate_id_mixin.py` & `overhave-4.1.0/overhave/scenario/validator/duplicate_id_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/scenario/validator/validator.py` & `overhave-4.1.0/overhave/scenario/validator/validator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/__init__.py` & `overhave-4.1.0/overhave/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/api_auth_storage.py` & `overhave-4.1.0/overhave/storage/api_auth_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/converters.py` & `overhave-4.1.0/overhave/storage/converters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/draft_storage.py` & `overhave-4.1.0/overhave/storage/draft_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/emulation_storage.py` & `overhave-4.1.0/overhave/storage/emulation_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/feature_storage.py` & `overhave-4.1.0/overhave/storage/feature_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/feature_tag_storage.py` & `overhave-4.1.0/overhave/storage/feature_tag_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/feature_type_storage.py` & `overhave-4.1.0/overhave/storage/feature_type_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/scenario_storage.py` & `overhave-4.1.0/overhave/storage/scenario_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/system_user_group_storage.py` & `overhave-4.1.0/overhave/storage/system_user_group_storage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
 
+import sqlalchemy.orm as so
+
 from overhave import db
 
 
 class ISystemUserGroupStorage(abc.ABC):
     """Abstract class for system user storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def has_any_group(user_groups: list[str]) -> bool:
+    def has_any_group(session: so.Session, user_groups: list[str]) -> bool:
         pass
 
 
 class SystemUserGroupStorage(ISystemUserGroupStorage):
     """Class for system user storage."""
 
     @staticmethod
-    def has_any_group(user_groups: list[str]) -> bool:
-        with db.create_session() as session:
-            group = session.query(db.GroupRole).filter(db.GroupRole.group.in_(user_groups)).first()
-            return group is not None
+    def has_any_group(session: so.Session, user_groups: list[str]) -> bool:
+        return session.query(db.GroupRole).filter(db.GroupRole.group.in_(user_groups)).first() is not None
```

### Comparing `overhave-4.0.5/overhave/storage/system_user_storage.py` & `overhave-4.1.0/overhave/storage/system_user_storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 import abc
 
-import sqlalchemy as sa
+import sqlalchemy.orm as so
 from pydantic import SecretStr
 
 from overhave import db
 from overhave.storage.converters import SystemUserModel
 
 
 class ISystemUserStorage(abc.ABC):
     """Abstract class for system user storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def get_user(user_id: int) -> SystemUserModel | None:
+    def get_user_model(user_id: int) -> SystemUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def create_user(login: str, password: SecretStr | None = None, role: db.Role = db.Role.user) -> SystemUserModel:
+    def create_user(
+        session: so.Session, login: str, password: SecretStr | None = None, role: db.Role = db.Role.user
+    ) -> db.UserRole:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_user_by_credits(login: str, password: SecretStr | None = None) -> SystemUserModel | None:
-        pass
-
-    @staticmethod
-    @abc.abstractmethod
-    def update_user_role(user_model: SystemUserModel) -> None:
+    def get_user_by_credits(session: so.Session, login: str, password: SecretStr | None = None) -> db.UserRole | None:
         pass
 
 
 class SystemUserStorage(ISystemUserStorage):
     """Class for system user storage."""
 
     @staticmethod
-    def get_user(user_id: int) -> SystemUserModel | None:
+    def get_user_model(user_id: int) -> SystemUserModel | None:
         with db.create_session() as session:
             db_user = session.get(db.UserRole, user_id)
             if db_user is not None:
                 return SystemUserModel.from_orm(db_user)
             return None
 
     @staticmethod
-    def create_user(login: str, password: SecretStr | None = None, role: db.Role = db.Role.user) -> SystemUserModel:
-        with db.create_session() as session:
-            db_password = None
-            if password is not None:
-                db_password = password.get_secret_value()
-            db_user = db.UserRole(login=login, password=db_password, role=role)
-            session.add(db_user)
-            session.flush()
-            return SystemUserModel.from_orm(db_user)
-
-    @staticmethod
-    def get_user_by_credits(login: str, password: SecretStr | None = None) -> SystemUserModel | None:
-        with db.create_session() as session:
-            query = session.query(db.UserRole).filter(db.UserRole.login == login)
-            if password is not None:
-                query = query.filter(db.UserRole.password == password.get_secret_value())
-            db_user = query.one_or_none()
-            if db_user is not None:
-                return SystemUserModel.from_orm(db_user)
-            return None
-
-    @staticmethod
-    def update_user_role(user_model: SystemUserModel) -> None:
-        with db.create_session() as session:
-            session.execute(sa.update(db.UserRole).where(db.UserRole.id == user_model.id).values(role=user_model.role))
+    def create_user(
+        session: so.Session, login: str, password: SecretStr | None = None, role: db.Role = db.Role.user
+    ) -> db.UserRole:
+        db_password = None
+        if password is not None:
+            db_password = password.get_secret_value()
+        db_user = db.UserRole(login=login, password=db_password, role=role)
+        session.add(db_user)
+        session.flush()
+        return db_user
+
+    @staticmethod
+    def get_user_by_credits(session: so.Session, login: str, password: SecretStr | None = None) -> db.UserRole | None:
+        query = session.query(db.UserRole).filter(db.UserRole.login == login)
+        if password is not None:
+            query = query.filter(db.UserRole.password == password.get_secret_value())
+        return query.one_or_none()
```

### Comparing `overhave-4.0.5/overhave/storage/test_run_storage.py` & `overhave-4.1.0/overhave/storage/test_run_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/storage/test_user_storage.py` & `overhave-4.1.0/overhave/storage/test_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/synchronization/storage_manager.py` & `overhave-4.1.0/overhave/synchronization/storage_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         session.flush()
         return parse_obj_as(list[TagModel], db_tags)
 
     def feature_type_by_name(self, session: so.Session, feature_type: FeatureTypeName) -> FeatureTypeModel:
         db_feature_type = self._feature_type_storage.feature_type_by_name(session=session, name=feature_type)
         return FeatureTypeModel.from_orm(db_feature_type)
 
-    def ensure_users_exist(self, info: StrictFeatureInfo) -> None:
+    def ensure_users_exist(self, session: so.Session, info: StrictFeatureInfo) -> None:
         for user in {info.author, info.last_edited_by}:
-            if self._system_user_storage.get_user_by_credits(login=user) is not None:
+            if self._system_user_storage.get_user_by_credits(session=session, login=user):
                 continue
             raise FeatureInfoUserNotFoundError(f"Could not find user with login={user}!")
 
     def update_db_feature(self, model: FeatureModel, scenario: str) -> None:
         scenario_model = self._scenario_storage.get_scenario_by_feature_id(model.id)
         self._feature_storage.update_feature(model)
         scenario_model.text = scenario
```

### Comparing `overhave-4.0.5/overhave/synchronization/synchronizer.py` & `overhave-4.1.0/overhave/synchronization/synchronizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         self._scenario_parser = scenario_parser
         self._feature_extractor = feature_extractor
         self._git_initializer = git_initializer
         self._storage_manager = storage_manager
 
     def _update_feature(self, model: FeatureModel, info: StrictFeatureInfo, file_ts: datetime) -> None:
         logger.info("Feature is gonna be updated...")
-        self._storage_manager.ensure_users_exist(info)
-        model.name = info.name
         with db.create_session() as session:
+            self._storage_manager.ensure_users_exist(session=session, info=info)
             model.feature_tags = self._storage_manager.get_feature_tags(session=session, info=info)
+        model.name = info.name
         model.severity = info.severity
         model.last_edited_by = info.last_edited_by
         model.last_edited_at = file_ts
         model.task = info.tasks
         self._storage_manager.update_db_feature(model=model, scenario=info.scenarios)
         logger.info("Feature has been updated successfully.")
 
@@ -73,17 +73,17 @@
         if info.author is None:
             raise NullableInfoAuthorError("Could not create feature without author!")
         if info.last_edited_by is None:
             info.last_edited_by = info.author
 
         info.id = ANY_INT
         strict_info = StrictFeatureInfo(**info.dict())
-        self._storage_manager.ensure_users_exist(strict_info)
 
         with db.create_session() as session:
+            self._storage_manager.ensure_users_exist(session=session, info=strict_info)
             feature_tags = self._storage_manager.get_feature_tags(session=session, info=strict_info)
             feature_type = self._storage_manager.feature_type_by_name(session=session, feature_type=strict_info.type)
 
         feature_model = FeatureModel(
             id=strict_info.id,
             created_at=get_current_time(),
             name=strict_info.name,
```

### Comparing `overhave-4.0.5/overhave/test_execution/executor.py` & `overhave-4.1.0/overhave/test_execution/executor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/test_execution/objects.py` & `overhave-4.1.0/overhave/test_execution/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/test_execution/settings.py` & `overhave-4.1.0/overhave/test_execution/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/test_execution/step_collector.py` & `overhave-4.1.0/overhave/test_execution/step_collector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/test_execution/test_runner.py` & `overhave-4.1.0/overhave/test_execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/__init__.py` & `overhave-4.1.0/overhave/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/__init__.py` & `overhave-4.1.0/overhave/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/api_client/authenticator.py` & `overhave-4.1.0/overhave/transport/http/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/base_client/auth.py` & `overhave-4.1.0/overhave/transport/http/base_client/auth.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/base_client/client.py` & `overhave-4.1.0/overhave/transport/http/base_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/base_client/settings.py` & `overhave-4.1.0/overhave/transport/http/base_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/gitlab_client/client.py` & `overhave-4.1.0/overhave/transport/http/gitlab_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/gitlab_client/models.py` & `overhave-4.1.0/overhave/transport/http/gitlab_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/gitlab_client/utils.py` & `overhave-4.1.0/overhave/transport/http/gitlab_client/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/stash_client/client.py` & `overhave-4.1.0/overhave/transport/http/stash_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/stash_client/models.py` & `overhave-4.1.0/overhave/transport/http/stash_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/http/stash_client/settings.py` & `overhave-4.1.0/overhave/transport/http/stash_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/ldap/authenticator.py` & `overhave-4.1.0/overhave/transport/ldap/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/consumer.py` & `overhave-4.1.0/overhave/transport/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/deps.py` & `overhave-4.1.0/overhave/transport/redis/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/objects.py` & `overhave-4.1.0/overhave/transport/redis/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/producer.py` & `overhave-4.1.0/overhave/transport/redis/producer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/runner.py` & `overhave-4.1.0/overhave/transport/redis/runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/redis/settings.py` & `overhave-4.1.0/overhave/transport/redis/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/s3/manager.py` & `overhave-4.1.0/overhave/transport/s3/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/s3/models.py` & `overhave-4.1.0/overhave/transport/s3/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/overhave/transport/s3/settings.py` & `overhave-4.1.0/overhave/transport/s3/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.5/pyproject.toml` & `overhave-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overhave"
-version = "4.0.5"
+version = "4.1.0"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
```

### Comparing `overhave-4.0.5/PKG-INFO` & `overhave-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overhave
-Version: 4.0.5
+Version: 4.1.0
 Summary: Overhave - web-framework for BDD
 Author: Vladislav Mukhamatnurov
 Author-email: livestreamepidemz@yandex.ru
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

