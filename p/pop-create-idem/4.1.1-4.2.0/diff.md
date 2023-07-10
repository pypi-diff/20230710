# Comparing `tmp/pop-create-idem-4.1.1.tar.gz` & `tmp/pop-create-idem-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-4.1.1.tar", last modified: Sun Jul  2 15:15:09 2023, max compression
+gzip compressed data, was "pop-create-idem-4.2.0.tar", last modified: Mon Jul 10 10:49:05 2023, max compression
```

## Comparing `pop-create-idem-4.1.1.tar` & `pop-create-idem-4.2.0.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8798 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8621 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/customize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/customize/contracts/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/customize/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2167 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     6216 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3477 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/test.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     4724 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)     1348 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1408 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1902 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
--rw-r--r--   0 root         (0) root         (0)     1152 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      819 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2805 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.767649 pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:09.771649 pop-create-idem-4.1.1/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8798 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8163 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-02 15:15:09.000000 pop-create-idem-4.1.1/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-02 15:15:09.775649 pop-create-idem-4.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-02 15:14:54.000000 pop-create-idem-4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8621 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/customize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/customize/contracts/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/customize/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     6216 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/test.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.209715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      819 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 10:49:04.000000 pop-create-idem-4.2.0/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:49:05.205715 pop-create-idem-4.2.0/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8163 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 10:49:05.000000 pop-create-idem-4.2.0/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 10:49:05.213715 pop-create-idem-4.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-10 10:48:49.000000 pop-create-idem-4.2.0/setup.py
```

### Comparing `pop-create-idem-4.1.1/LICENSE` & `pop-create-idem-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/PKG-INFO` & `pop-create-idem-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.1.1
+Version: 4.2.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-4.1.1/README.rst` & `pop-create-idem-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/cloudspec/__init__.py` & `pop-create-idem-4.2.0/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/cloudspec/conf.py` & `pop-create-idem-4.2.0/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/init.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/init.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,26 +40,46 @@
     hub,
     ctx,
     root_directory: pathlib.Path,
     create_plugins: List[str],
 ):
     start_time = timeit.default_timer()
 
-    # Run through all external customization before running create plugin
-    for customize_plugin in hub.cloudspec.customize._loaded:
-        try:
-            print(f"Running customization with plugin: {customize_plugin}")
-            hub.cloudspec.customize[customize_plugin].run(ctx)
-        except Exception as customization_err:
-            hub.log.error(
-                f"Failed to customize using {customize_plugin}: {customization_err}"
-            )
+    cloud_spec_customize_plugin = ctx.get("cloud_spec_customize_plugin")
+    if cloud_spec_customize_plugin:
+        for customize_plugin in cloud_spec_customize_plugin:
+            if customize_plugin not in hub.cloudspec.customize._loaded:
+                print(
+                    f"The cloud spec customize plugin '{customize_plugin}' is not loaded."
+                )
+                continue
+            hub.cloudspec.init.run_customize_cloud_spec(ctx, customize_plugin)
+    else:
+        # Run through all loaded customization. This can support multiple abstracted customization plugins (e.g.
+        # state, exec, test etc.) in a generated idem plugin
+        for customize_plugin in hub.cloudspec.customize._loaded:
+            hub.cloudspec.init.run_customize_cloud_spec(ctx, customize_plugin)
 
     for create_plugin in create_plugins:
         try:
             hub.log.info(f"Running create plugin: {create_plugin}")
             hub.cloudspec.create[create_plugin].run(ctx, root_directory)
         except Exception as e:
             hub.log.error(f"Failed to run create plugin: {create_plugin}")
             hub.log.error(e)
             raise
     print(f"Total Duration: {timeit.default_timer() - start_time} seconds")
+
+
+def run_customize_cloud_spec(hub, ctx, cloud_spec_customize_plugin):
+    try:
+        hub.log.debug(
+            f"Running customization with plugin: {cloud_spec_customize_plugin}"
+        )
+        hub.cloudspec.customize[cloud_spec_customize_plugin].run(ctx)
+        hub.log.debug(
+            f"Updated cloud spec after customization with plugin '{cloud_spec_customize_plugin}': {json.dumps(ctx.cloud_spec, indent=4)}"
+        )
+    except Exception as customization_err:
+        hub.log.error(
+            f"Failed to customize using {cloud_spec_customize_plugin}: {customization_err}"
+        )
```

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-4.2.0/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/conf.py` & `pop-create-idem-4.2.0/pop_create_idem/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,20 @@
         "dyne": "pop_create",
     },
     "templates_dir": {
         "options": ["--td"],
         "subcommands": ["_global_"],
         "dyne": "pop_create",
     },
+    "cloud_spec_customize_plugin": {
+        "options": ["--customize-plugin"],
+        "nargs": "+",
+        "subcommands": ["openapi3", "swagger", "idem-cloud"],
+        "dyne": "pop_create",
+    },
 }
 CONFIG = {
     "create_plugin": {
         "default": "state_modules",
         "dyne": "pop_create",
         "help": "The `create` plugin to use for resource modules. The other options are 'auto_states', 'exec_modules'.",
     },
@@ -43,14 +49,20 @@
         "dyne": "pop_create",
     },
     "templates_dir": {
         "default": None,
         "help": "The full absolute path of directory where jinja templates are saved",
         "dyne": "pop_create",
     },
+    "cloud_spec_customize_plugin": {
+        "default": None,
+        "help": "The name of the plugins for customizing cloud spec before resource modules are created. The default "
+        "customize plugin can be found under 'root_dir > project_name > cloudspec > customize`",
+        "dyne": "pop_create",
+    },
 }
 SUBCOMMANDS = {
     # https://openapi.tools/#converters
     "idem-cloud": {"help": "Boostrap an idem cloud project", "dyne": "pop_create"},
     "openapi3": {
         "help": "Create idem_cloud modules based off of an openapi3 spec",
         "dyne": "pop_create",
```

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,19 @@
     hub.pop.sub.add(dyne_name="cloudspec")
 
 
 def context(hub, ctx, directory: pathlib.Path):
     # all template files are copied without render
     ctx["_copy_without_render"] = ["*.jinja2"]
 
+    if hub.OPT.pop_create.cloud_spec_customize_plugin:
+        ctx[
+            "cloud_spec_customize_plugin"
+        ] = hub.OPT.pop_create.cloud_spec_customize_plugin
+
     # non openapi/swagger based would not have cloud_spec here
     if "cloud_spec" not in ctx or not ctx.cloud_spec:
         # If an acct plugin was passed in then we don't need to create auth plugins
         if ctx.get("simple_service_name"):
             ctx.service_name = ctx.simple_service_name
         elif not ctx.get("service_name"):
             ctx.service_name = (
```

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/params.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-4.2.0/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/tool/format/case.py` & `pop-create-idem-4.2.0/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-4.2.0/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem/tool/gradle.py` & `pop-create-idem-4.2.0/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-4.2.0/pop_create_idem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.1.1
+Version: 4.2.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-4.1.1/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-4.2.0/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.1.1/setup.py` & `pop-create-idem-4.2.0/setup.py`

 * *Files identical despite different names*

