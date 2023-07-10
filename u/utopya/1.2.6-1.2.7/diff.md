# Comparing `tmp/utopya-1.2.6.tar.gz` & `tmp/utopya-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utopya-1.2.6.tar", last modified: Fri Jul  7 10:06:02 2023, max compression
+gzip compressed data, was "utopya-1.2.7.tar", last modified: Mon Jul 10 08:52:54 2023, max compression
```

## Comparing `utopya-1.2.6.tar` & `utopya-1.2.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.711444 utopya-1.2.6/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-07 10:05:51.000000 utopya-1.2.6/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7633 2023-07-07 10:05:51.000000 utopya-1.2.6/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)     3148 2023-07-07 10:06:02.710444 utopya-1.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-07-07 10:05:51.000000 utopya-1.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-07 10:05:51.000000 utopya-1.2.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 10:06:02.711444 utopya-1.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5691 2023-07-07 10:05:51.000000 utopya-1.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.693444 utopya-1.2.6/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.695444 utopya-1.2.6/tests/_gen_figures/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/_gen_figures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/_gen_figures/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/_gen_figures/test_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.695444 utopya-1.2.6/tests/backend/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 10:05:52.000000 utopya-1.2.6/tests/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8239 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/backend/test_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)    10242 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/backend/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/backend/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.697444 utopya-1.2.6/tests/cli/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test__shell_complete.py
--rw-rw-rw-   0 root         (0) root         (0)     2810 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test__to_migrate.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_batch.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15337 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6940 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_run_and_eval.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/cli/test_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.698444 utopya-1.2.6/tests/eval/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 10:05:52.000000 utopya-1.2.6/tests/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9145 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/eval/test_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/eval/test_datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/eval/test_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/eval/test_plot_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    45409 2023-07-07 10:05:51.000000 utopya-1.2.6/tests/eval/test_plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.701444 utopya-1.2.6/utopya/
--rw-rw-rw-   0 root         (0) root         (0)     3255 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3340 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_import_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_signal.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.702444 utopya-1.2.6/utopya/_yaml_registry/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_yaml_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9532 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_yaml_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    10253 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/_yaml_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    18565 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.703444 utopya-1.2.6/utopya/cfg/
--rw-rw-rw-   0 root         (0) root         (0)    20229 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/cfg/base_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)    13771 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/cfg/base_plots.yml
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/cfg/btm_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/cfg/user_cfg_header.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/cfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.704444 utopya-1.2.6/utopya/eval/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6936 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/_plot_func_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/containers.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/data_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plotcreators.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plothelper.py
--rw-rw-rw-   0 root         (0) root         (0)     9048 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plotmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.706444 utopya-1.2.6/utopya/eval/plots/
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7502 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/_attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    72572 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/_mpl.py
--rw-rw-rw-   0 root         (0) root         (0)    12091 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    58799 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/abm.py
--rw-rw-rw-   0 root         (0) root         (0)    25571 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    62459 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/ca.py
--rw-rw-rw-   0 root         (0) root         (0)     6924 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/distributions.py
--rw-rw-rw-   0 root         (0) root         (0)    24529 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     9451 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/snsplot.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/plots/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/eval/transform.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23144 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.707444 utopya-1.2.6/utopya/model_registry/
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/_registration.py
--rw-rw-rw-   0 root         (0) root         (0)    16777 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    15927 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/info_bundle.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/model_registry/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    70544 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/multiverse.py
--rw-rw-rw-   0 root         (0) root         (0)    19695 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    12297 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/project_registry.py
--rw-rw-rw-   0 root         (0) root         (0)    54018 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)    13652 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/stop_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)    52862 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/testtools.py
--rw-rw-rw-   0 root         (0) root         (0)     9031 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/tools.py
--rw-rw-rw-   0 root         (0) root         (0)    41450 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/workermanager.py
--rw-rw-rw-   0 root         (0) root         (0)     5421 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.702444 utopya-1.2.6/utopya.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3148 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-07 10:06:02.000000 utopya-1.2.6/utopya.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.708444 utopya-1.2.6/utopya_backend/
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17418 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.708444 utopya-1.2.6/utopya_backend/io/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.708444 utopya-1.2.6/utopya_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18987 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/model/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8082 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/model/step.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_backend/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:06:02.710444 utopya-1.2.6/utopya_cli/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18051 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/_copy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     9861 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/_shared.py
--rw-rw-rw-   0 root         (0) root         (0)    15347 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    17744 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/eval.py
--rw-rw-rw-   0 root         (0) root         (0)    24141 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7872 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/projects.py
--rw-rw-rw-   0 root         (0) root         (0)     6753 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-07-07 10:05:51.000000 utopya-1.2.6/utopya_cli/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.576851 utopya-1.2.7/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-10 08:52:43.000000 utopya-1.2.7/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2023-07-10 08:52:43.000000 utopya-1.2.7/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-07-10 08:52:54.576851 utopya-1.2.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5594 2023-07-10 08:52:43.000000 utopya-1.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-10 08:52:43.000000 utopya-1.2.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 08:52:54.577850 utopya-1.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-07-10 08:52:43.000000 utopya-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.558850 utopya-1.2.7/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.560850 utopya-1.2.7/tests/_gen_figures/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/_gen_figures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/_gen_figures/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/_gen_figures/test_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.561850 utopya-1.2.7/tests/backend/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8239 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/backend/test_benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)    10242 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/backend/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/backend/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.562850 utopya-1.2.7/tests/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test__shell_complete.py
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test__to_migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15337 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6940 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_run_and_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/cli/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.563850 utopya-1.2.7/tests/eval/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9145 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/test_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/test_datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/test_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/test_plot_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    45377 2023-07-10 08:52:43.000000 utopya-1.2.7/tests/eval/test_plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.567850 utopya-1.2.7/utopya/
+-rw-rw-rw-   0 root         (0) root         (0)     3255 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_import_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_signal.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.568850 utopya-1.2.7/utopya/_yaml_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_yaml_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9532 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_yaml_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    10253 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/_yaml_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    18565 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.569850 utopya-1.2.7/utopya/cfg/
+-rw-rw-rw-   0 root         (0) root         (0)    20229 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/cfg/base_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13771 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/cfg/base_plots.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/cfg/btm_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/cfg/user_cfg_header.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.570850 utopya-1.2.7/utopya/eval/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6936 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/_plot_func_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/data_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plotcreators.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plothelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9048 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plotmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.572850 utopya-1.2.7/utopya/eval/plots/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7502 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/_attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    72723 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/_mpl.py
+-rw-rw-rw-   0 root         (0) root         (0)    12091 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    58799 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/abm.py
+-rw-rw-rw-   0 root         (0) root         (0)    25571 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    62459 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/ca.py
+-rw-rw-rw-   0 root         (0) root         (0)     6924 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24529 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     9451 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/snsplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/plots/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/eval/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23144 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.573850 utopya-1.2.7/utopya/model_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)    16777 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    15927 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/info_bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/model_registry/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    70544 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/multiverse.py
+-rw-rw-rw-   0 root         (0) root         (0)    19695 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/project_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    54018 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    13652 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/stop_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    52862 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/testtools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9031 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    41450 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/workermanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5421 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.568850 utopya-1.2.7/utopya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-10 08:52:54.000000 utopya-1.2.7/utopya.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.574850 utopya-1.2.7/utopya_backend/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17418 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.574850 utopya-1.2.7/utopya_backend/io/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.574850 utopya-1.2.7/utopya_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18987 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/model/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8082 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/model/step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_backend/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:52:54.576851 utopya-1.2.7/utopya_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18051 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/_copy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     9861 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/_shared.py
+-rw-rw-rw-   0 root         (0) root         (0)    15347 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/eval.py
+-rw-rw-rw-   0 root         (0) root         (0)    24141 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7872 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     6753 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-07-10 08:52:43.000000 utopya-1.2.7/utopya_cli/test.py
```

### Comparing `utopya-1.2.6/COPYING` & `utopya-1.2.7/COPYING`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/COPYING.LESSER` & `utopya-1.2.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/PKG-INFO` & `utopya-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.2.6
+Version: 1.2.7
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Benjamin Herdeanu <Benjamin.Herdeanu@iup.uni-heidelberg.de>, Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: opt
 Provides-Extra: dev
 License-File: COPYING
 License-File: COPYING.LESSER
 
 
 ``utopya``: A simulation management and evaluation framework
 ============================================================
```

### Comparing `utopya-1.2.6/README.md` & `utopya-1.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,30 +33,35 @@
 To install utopya, first enter the virtual environment of your choice.
 The utopya package is available on [PyPI][utopya-pypi]:
 
 ```bash
 pip install utopya
 ```
 
-Alternatively, use the following command to install from a certain branch:
-
-```bash
-pip install git+https://gitlab.com/utopia-project/utopya.git@<branch-name>
-```
-
-The above commands will install `utopya`, the `utopya_backend` and the utopya CLI, pulling in all requirements.
+This will install `utopya`, the `utopya_backend` and the utopya CLI, pulling in all requirements.
 You should now be able to invoke the utopya CLI:
 
 ```bash
 utopya --help
 ```
 
 *Note:* utopya does not specify minimum versions for its requirements; but it is always tested using the latest versions of its dependencies (for Python 3.8 to 3.11).
 In case you run into problems, consider upgrading the involved packages using `pip install --upgrade`.
 
+## Optional Dependencies
+To include all optional dependencies in the installation (e.g. for plotting networks), use the following command:
+
+```bash
+pip install utopya[opt]
+```
+
+This may require that you install the following packages first:
+* [graphviz][graphviz]
+    * See [the PyGraphviz docs](https://pygraphviz.github.io/documentation/stable/install.html) for further instructions.
+
 <!-- end: installation -->
 
 
 # Getting started
 * For a simple example, see the [demo project](demo/).
 * For a larger example of how utopya can be used, have a look at [Utopia][Utopia].
 * For more information, refer to the [utopya documentation](https://utopya.readthedocs.io/).
@@ -119,7 +124,9 @@
 [LGPL]: https://www.gnu.org/licenses/lgpl-3.0.en.html
 [utopya-repo]: https://gitlab.com/utopia-project/utopya
 [utopya-pypi]: https://pypi.org/project/utopya/
 [Utopia]: https://gitlab.com/utopia-project/utopia
 [dantro]: https://gitlab.com/utopia-project/dantro
 [paramspace]: https://gitlab.com/blsqr/paramspace
 [Utopia-Project]: https://utopia-project.org/
+
+[graphviz]: https://graphviz.org
```

### Comparing `utopya-1.2.6/pyproject.toml` & `utopya-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/setup.py` & `utopya-1.2.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     "sphinx-togglebutton",
     "ipython>=7.0",
     "myst-parser[linkify]",
     "sphinx-click",
     "pytest",
 ]
 
+# Optional dependencies
+OPTIONAL_DEPS = [
+    "networkx",
+    "pygraphviz",
+]
+
 
 # .. Description ..............................................................
 
 DESCRIPTION = "A simulation management and evaluation framework"
 LONG_DESCRIPTION = """
 ``utopya``: A simulation management and evaluation framework
 ============================================================
@@ -157,15 +163,16 @@
     data_files=[("", ["COPYING", "COPYING.LESSER", "README.md"])],
     #
     # Dependencies
     install_requires=INSTALL_DEPS,
     extras_require=dict(
         test=TEST_DEPS,
         doc=DOC_DEPS,
-        dev=TEST_DEPS + DOC_DEPS,
+        opt=OPTIONAL_DEPS,
+        dev=TEST_DEPS + DOC_DEPS + OPTIONAL_DEPS,
     ),
     #
     # Command line scripts
     entry_points={
         "console_scripts": [
             "utopya = utopya_cli.cli:cli",
         ],
```

### Comparing `utopya-1.2.6/tests/_gen_figures/__init__.py` & `utopya-1.2.7/tests/_gen_figures/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/_gen_figures/test_plots.py` & `utopya-1.2.7/tests/_gen_figures/test_plots.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/backend/test_benchmark.py` & `utopya-1.2.7/tests/backend/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/backend/test_model.py` & `utopya-1.2.7/tests/backend/test_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/backend/test_tools.py` & `utopya-1.2.7/tests/backend/test_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test__shell_complete.py` & `utopya-1.2.7/tests/cli/test__shell_complete.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test__to_migrate.py` & `utopya-1.2.7/tests/cli/test__to_migrate.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_batch.py` & `utopya-1.2.7/tests/cli/test_batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_config.py` & `utopya-1.2.7/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_models.py` & `utopya-1.2.7/tests/cli/test_models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_projects.py` & `utopya-1.2.7/tests/cli/test_projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_run_and_eval.py` & `utopya-1.2.7/tests/cli/test_run_and_eval.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/cli/test_test.py` & `utopya-1.2.7/tests/cli/test_test.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/eval/test_containers.py` & `utopya-1.2.7/tests/eval/test_containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/eval/test_datamanager.py` & `utopya-1.2.7/tests/eval/test_datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/eval/test_groups.py` & `utopya-1.2.7/tests/eval/test_groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/eval/test_plot_utils.py` & `utopya-1.2.7/tests/eval/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/tests/eval/test_plotting.py` & `utopya-1.2.7/tests/eval/test_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1175,22 +1175,20 @@
     assert len(gp._edges_to_draw) == 3
     assert gp._nodes_to_shrink == [2]
 
     # Now go through configurations and test initialization and drawing
     for name, cfg in load_yml(GRAPH_PLOT_CLS).items():
         fig = plt.figure()
 
-        # Try using a graphviz node layout, which requires pydot
+        # Try using a graphviz node layout, which requires pygraphviz
         if name == "graphviz":
             try:
-                import pydot
+                import pygraphviz
             except ImportError:
-                with pytest.raises(
-                    ImportError, match="No module named 'pydot'"
-                ):
+                with pytest.raises(ImportError, match="requires pygraphviz"):
                     gp = GraphPlot(digraph, fig=fig, **cfg)
 
                 continue
 
         _raises = cfg.pop("_raises", None)
         _warns = cfg.pop("_warns", None)
         _match = cfg.pop("_match", None)
```

### Comparing `utopya-1.2.6/utopya/__init__.py` & `utopya-1.2.7/utopya/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 utopya as its frontend.
 For model implementations, the :py:mod:`utopya_backend` package can assist in
 building Python-based models that use :py:mod:`utopya` as a frontend.
 
 Also visit :ref:`the user manual front page <welcome>` for more information.
 """
 
-__version__ = "1.2.6"
+__version__ = "1.2.7"
 """The :py:mod:`utopya` package version"""
 
 # .. Logging ..................................................................
 # TODO Consider setting up logging elsewhere -- but needs to be done first!
 from dantro.logging import REMARK as _DEFAULT_LOG_LEVEL
 from dantro.logging import getLogger as _getLogger
```

### Comparing `utopya-1.2.6/utopya/_cluster.py` & `utopya-1.2.7/utopya/_cluster.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/_import_tools.py` & `utopya-1.2.7/utopya/_import_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/_yaml_registry/entry.py` & `utopya-1.2.7/utopya/_yaml_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/_yaml_registry/registry.py` & `utopya-1.2.7/utopya/_yaml_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/batch.py` & `utopya-1.2.7/utopya/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/cfg/base_cfg.yml` & `utopya-1.2.7/utopya/cfg/base_cfg.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/cfg/base_plots.yml` & `utopya-1.2.7/utopya/cfg/base_plots.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/cfg/btm_cfg.yml` & `utopya-1.2.7/utopya/cfg/btm_cfg.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/cfg.py` & `utopya-1.2.7/utopya/cfg.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/_plot_func_resolver.py` & `utopya-1.2.7/utopya/eval/_plot_func_resolver.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/containers.py` & `utopya-1.2.7/utopya/eval/containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/data_ops.py` & `utopya-1.2.7/utopya/eval/data_ops.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/datamanager.py` & `utopya-1.2.7/utopya/eval/datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/groups.py` & `utopya-1.2.7/utopya/eval/groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plotcreators.py` & `utopya-1.2.7/utopya/eval/plotcreators.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plothelper.py` & `utopya-1.2.7/utopya/eval/plothelper.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plotmanager.py` & `utopya-1.2.7/utopya/eval/plotmanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/_attractor.py` & `utopya-1.2.7/utopya/eval/plots/_attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/_graph.py` & `utopya-1.2.7/utopya/eval/plots/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "shell": nx.shell_layout,
     "bipartite": nx.bipartite_layout,
     "kamada_kawai": nx.kamada_kawai_layout,
     "planar": nx.planar_layout,
     "random": nx.random_layout,
     "spectral": nx.spectral_layout,
     "spiral": nx.spiral_layout,
+    "graphviz": nx.nx_agraph.graphviz_layout,
 }
 """Available networkx node layout options"""
 
 # -----------------------------------------------------------------------------
 
 
 class GraphPlot:
@@ -123,19 +124,21 @@
                     `networkx layout models <https://networkx.github.io/documentation/stable/reference/drawing.html#module-networkx.drawing.layout>`_
                     are: ``spring``, ``circular``, ``shell``, ``bipartite``,
                     ``kamada_kawai``, ``planar``, ``random``, ``spectral``,
                     ``spiral``.
                     See :py:data:`.POSITIONING_MODELS_NETWORKX`.
 
                     If installed, `GraphViz <https://pypi.org/project/graphviz/>`_
-                    models can be selected with a prepended ``graphviz_``.
+                    models can be selected using the
+                    ``agraph_graphviz`` :py:func:`~networkx.drawing.nx_agraph.graphviz_layout`)
+                    layout function, with the ``prog`` argument specifying the layout model.
                     Options depend on the ``GraphViz`` version but may include:
                     ``dot``, ``neato``, ``fdp``, ``sfdp``, ``twopi``,
-                    ``circo``. (Passed as ``prog`` argument to
-                    :py:func:`~networkx.drawing.nx_agraph.graphviz_layout`).
+                    ``circo``. Other arguments must be passed as a single string separated by a hyphen,
+                    e.g. ``'-len=1000-overlap_scaling=100-sep=100'``.
 
                     If the argument is a callable, it is invoked with the graph
                     as the first positional argument and is expected to return
                     networkx-compatible node positions, i.e. a mapping from
                     nodes to a 2-tuple denoting the position.
                 further kwargs:
                     Passed on to the chosen layout model.
@@ -713,28 +716,14 @@
             log.remark(
                 "Calculating the node positions using a positioning model ..."
             )
 
             if callable(model):
                 self.positions = model(self._g, **kwargs)
 
-            elif model.startswith("graphviz_"):
-                try:
-                    # graphviz models
-                    model = model[9:]
-                    self.positions = nx.nx_pydot.graphviz_layout(
-                        self._g, prog=model, **kwargs
-                    )
-
-                except ModuleNotFoundError as err:
-                    raise ModuleNotFoundError(
-                        "When trying to use the graphviz node positioning "
-                        f"model '{model}': '{err}'"
-                    ) from err
-
             # else: is a networkx positioning model
             else:
                 self.positions = POSITIONING_MODELS_NETWORKX[model](
                     self._g, **kwargs
                 )
 
     def parse_nodes(
@@ -965,14 +954,15 @@
     def parse_edges(
         self,
         *,
         width=None,
         edge_color=None,
         edge_cmap=None,
         cmap_norm=None,
+        alpha=None,
         edge_vmin: float = None,
         edge_vmax: float = None,
         colorbar: dict = None,
         update_colormapping: bool = True,
         **kwargs,
     ):
         """Parses the edge layout configuration and updates the edge kwargs of
@@ -1052,15 +1042,15 @@
             self._edge_kwargs["width"] = self._scale_to_interval(
                 [self._g.edges[n][prop] for n in self._edges_to_draw], interval
             )
 
         elif width is not None:
             self._edge_kwargs["width"] = width
 
-        # Node colors
+        # Edge colors
         if isinstance(edge_color, dict) and "from_property" in edge_color:
             prop = edge_color["from_property"]
             interval = edge_color.get("scale_to_interval", None)
 
             # If provided a mapping, map the property values to scalar values
             if "map_to_scalar" in edge_color:
                 map_to_scalar = np.vectorize(edge_color["map_to_scalar"].get)
@@ -1074,14 +1064,26 @@
 
             self._edge_kwargs["edge_color"] = _edge_colors
             self._show_edge_cbar = True
 
         elif edge_color is not None:
             self._edge_kwargs["edge_color"] = edge_color
 
+        # Edge alpha
+        if isinstance(alpha, dict) and "from_property" in alpha:
+            prop = alpha["from_property"]
+            interval = alpha.get("scale_to_interval", None)
+
+            self._edge_kwargs["alpha"] = self._scale_to_interval(
+                [self._g.edges[n][prop] for n in self._edges_to_draw], interval
+            )
+
+        elif alpha is not None:
+            self._edge_kwargs["alpha"] = alpha
+
         # ... property mapping done.
 
         # Get colorbar configuration and update the existing kwargs
         colorbar = colorbar if colorbar is not None else {}
         cbar_labels = colorbar.pop("labels", None)
         self._show_edge_cbar = colorbar.pop("enabled", self._show_edge_cbar)
         self._edge_cbar_kwargs.update(colorbar)
```

### Comparing `utopya-1.2.6/utopya/eval/plots/_mpl.py` & `utopya-1.2.7/utopya/eval/plots/_mpl.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/_utils.py` & `utopya-1.2.7/utopya/eval/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/abm.py` & `utopya-1.2.7/utopya/eval/plots/abm.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/attractor.py` & `utopya-1.2.7/utopya/eval/plots/attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/ca.py` & `utopya-1.2.7/utopya/eval/plots/ca.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/distributions.py` & `utopya-1.2.7/utopya/eval/plots/distributions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/graph.py` & `utopya-1.2.7/utopya/eval/plots/graph.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/snsplot.py` & `utopya-1.2.7/utopya/eval/plots/snsplot.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/plots/time_series.py` & `utopya-1.2.7/utopya/eval/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/eval/transform.py` & `utopya-1.2.7/utopya/eval/transform.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/exceptions.py` & `utopya-1.2.7/utopya/exceptions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model.py` & `utopya-1.2.7/utopya/model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/__init__.py` & `utopya-1.2.7/utopya/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/_registration.py` & `utopya-1.2.7/utopya/model_registry/_registration.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/entry.py` & `utopya-1.2.7/utopya/model_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/info_bundle.py` & `utopya-1.2.7/utopya/model_registry/info_bundle.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/registry.py` & `utopya-1.2.7/utopya/model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/model_registry/utils.py` & `utopya-1.2.7/utopya/model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/multiverse.py` & `utopya-1.2.7/utopya/multiverse.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/parameter.py` & `utopya-1.2.7/utopya/parameter.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/plotting.py` & `utopya-1.2.7/utopya/plotting.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/project_registry.py` & `utopya-1.2.7/utopya/project_registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/reporter.py` & `utopya-1.2.7/utopya/reporter.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/stop_conditions.py` & `utopya-1.2.7/utopya/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/task.py` & `utopya-1.2.7/utopya/task.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/testtools.py` & `utopya-1.2.7/utopya/testtools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/tools.py` & `utopya-1.2.7/utopya/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/workermanager.py` & `utopya-1.2.7/utopya/workermanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya/yaml.py` & `utopya-1.2.7/utopya/yaml.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya.egg-info/PKG-INFO` & `utopya-1.2.7/utopya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.2.6
+Version: 1.2.7
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Benjamin Herdeanu <Benjamin.Herdeanu@iup.uni-heidelberg.de>, Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: opt
 Provides-Extra: dev
 License-File: COPYING
 License-File: COPYING.LESSER
 
 
 ``utopya``: A simulation management and evaluation framework
 ============================================================
```

### Comparing `utopya-1.2.6/utopya.egg-info/SOURCES.txt` & `utopya-1.2.7/utopya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/benchmark.py` & `utopya-1.2.7/utopya_backend/benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/logging.py` & `utopya-1.2.7/utopya_backend/logging.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/model/__init__.py` & `utopya-1.2.7/utopya_backend/model/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/model/base.py` & `utopya-1.2.7/utopya_backend/model/base.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/model/step.py` & `utopya-1.2.7/utopya_backend/model/step.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/signal.py` & `utopya-1.2.7/utopya_backend/signal.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_backend/tools.py` & `utopya-1.2.7/utopya_backend/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/_copy_model.py` & `utopya-1.2.7/utopya_cli/_copy_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/_shared.py` & `utopya-1.2.7/utopya_cli/_shared.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/_utils.py` & `utopya-1.2.7/utopya_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/batch.py` & `utopya-1.2.7/utopya_cli/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/cli.py` & `utopya-1.2.7/utopya_cli/cli.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/config.py` & `utopya-1.2.7/utopya_cli/config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/eval.py` & `utopya-1.2.7/utopya_cli/eval.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/models.py` & `utopya-1.2.7/utopya_cli/models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/projects.py` & `utopya-1.2.7/utopya_cli/projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/run.py` & `utopya-1.2.7/utopya_cli/run.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.6/utopya_cli/test.py` & `utopya-1.2.7/utopya_cli/test.py`

 * *Files identical despite different names*

