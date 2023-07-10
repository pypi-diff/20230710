# Comparing `tmp/NREL-jade-0.9.8.tar.gz` & `tmp/NREL-jade-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-jade-0.9.8.tar", last modified: Fri Mar 31 21:54:58 2023, max compression
+gzip compressed data, was "NREL-jade-0.9.9.tar", last modified: Mon Jul 10 15:04:38 2023, max compression
```

## Comparing `NREL-jade-0.9.8.tar` & `NREL-jade-0.9.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.930719 NREL-jade-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.882716 NREL-jade-0.9.8/NREL_jade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-31 21:54:58.000000 NREL-jade-0.9.8/NREL_jade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 21:54:58.930719 NREL-jade-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.886716 NREL-jade-0.9.8/jade/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.898717 NREL-jade-0.9.8/jade/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/auto_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/cancel_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/collect_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/hpc_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/jade.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/jade_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/prune_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/resubmit_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/run_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/run_multi_node_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/run_spark_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/show_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/show_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/show_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/submit_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/try_submit_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/cli/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.902717 NREL-jade-0.9.8/jade/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.902717 NREL-jade-0.9.8/jade/extensions/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/autoregression_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/autoregression_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/autoregression_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/autoregression_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      921 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/create_merge_pred_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/demo/merge_pred_gdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.906717 NREL-jade-0.9.8/jade/extensions/generic_command/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/extensions/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.910718 NREL-jade-0.9.8/jade/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/fake_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/hpc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/hpc_manager_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/hpc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/local_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/pbs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/hpc/slurm_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.918718 NREL-jade-0.9.8/jade/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/analysis_execution_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/async_cli_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/async_job_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_configuration_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_container_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_container_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_container_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_execution_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_inputs_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_parameters_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/job_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/jobs/results_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.922719 NREL-jade-0.9.8/jade/models/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/submission_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/models/submitter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/resource_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.922719 NREL-jade-0.9.8/jade/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.926719 NREL-jade-0.9.8/jade/spark/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/bin/run_spark_script.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/bin/run_spark_script_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/bin/run_user_script_wrapper.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.930719 NREL-jade-0.9.8/jade/spark/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/fairscheduler.xml.template
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/log4j.properties.template
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/metrics.properties.template
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/resourcesFile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/spark-defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/spark-defaults.conf.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     4428 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/spark-env.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4428 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/spark-env.sh.template
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/conf/workers.template
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:58.930719 NREL-jade-0.9.8/jade/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/custom_click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/repository_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/subprocess_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/timing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/jade/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 21:54:58.930719 NREL-jade-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-31 21:54:49.000000 NREL-jade-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.855487 NREL-jade-0.9.9/NREL_jade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 15:04:38.000000 NREL-jade-0.9.9/NREL_jade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.855487 NREL-jade-0.9.9/jade/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.859487 NREL-jade-0.9.9/jade/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/auto_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/cancel_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/collect_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/hpc_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/jade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/jade_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/prune_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/resubmit_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/run_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/run_multi_node_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/run_spark_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/show_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/show_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/show_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/submit_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/try_submit_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/cli/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.859487 NREL-jade-0.9.9/jade/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.859487 NREL-jade-0.9.9/jade/extensions/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/autoregression_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/autoregression_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/autoregression_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/autoregression_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      921 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/create_merge_pred_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/demo/merge_pred_gdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.859487 NREL-jade-0.9.9/jade/extensions/generic_command/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/extensions/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.863487 NREL-jade-0.9.9/jade/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/fake_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/hpc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/hpc_manager_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/hpc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/local_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/pbs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/hpc/slurm_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.863487 NREL-jade-0.9.9/jade/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/analysis_execution_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/async_cli_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/async_job_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_configuration_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_container_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_container_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_container_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_execution_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_inputs_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_parameters_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/job_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/jobs/results_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.863487 NREL-jade-0.9.9/jade/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/submission_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/models/submitter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/resource_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.863487 NREL-jade-0.9.9/jade/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/jade/spark/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/bin/run_spark_script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/bin/run_spark_script_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/bin/run_user_script_wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/jade/spark/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/fairscheduler.xml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/log4j.properties.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/metrics.properties.template
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/resourcesFile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/spark-defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/spark-defaults.conf.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4428 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/spark-env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4428 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/spark-env.sh.template
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/conf/workers.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/jade/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/custom_click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/repository_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/subprocess_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/timing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/jade/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:04:38.867487 NREL-jade-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-10 15:04:27.000000 NREL-jade-0.9.9/setup.py
```

### Comparing `NREL-jade-0.9.8/LICENSE` & `NREL-jade-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/NREL_jade.egg-info/PKG-INFO` & `NREL-jade-0.9.9/NREL_jade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-jade
-Version: 0.9.8
+Version: 0.9.9
 Summary: Provides HPC workflow automation services
 Home-page: https://github.com./NREL/jade
 Maintainer: Daniel Thom
 Maintainer-email: daniel.thom@nrel.gov
 License: BSD license
 Keywords: jade,hpc,workflow
 Platform: UNKNOWN
```

### Comparing `NREL-jade-0.9.8/NREL_jade.egg-info/SOURCES.txt` & `NREL-jade-0.9.9/NREL_jade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/PKG-INFO` & `NREL-jade-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-jade
-Version: 0.9.8
+Version: 0.9.9
 Summary: Provides HPC workflow automation services
 Home-page: https://github.com./NREL/jade
 Maintainer: Daniel Thom
 Maintainer-email: daniel.thom@nrel.gov
 License: BSD license
 Keywords: jade,hpc,workflow
 Platform: UNKNOWN
```

### Comparing `NREL-jade-0.9.8/jade/cli/auto_config.py` & `NREL-jade-0.9.9/jade/cli/auto_config.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/cancel_jobs.py` & `NREL-jade-0.9.9/jade/cli/cancel_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/cluster.py` & `NREL-jade-0.9.9/jade/cli/cluster.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/collect_stats.py` & `NREL-jade-0.9.9/jade/cli/collect_stats.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/common.py` & `NREL-jade-0.9.9/jade/cli/common.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/config.py` & `NREL-jade-0.9.9/jade/cli/config.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/db.py` & `NREL-jade-0.9.9/jade/cli/db.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/extensions.py` & `NREL-jade-0.9.9/jade/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/hpc_jobs.py` & `NREL-jade-0.9.9/jade/cli/hpc_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/jade.py` & `NREL-jade-0.9.9/jade/cli/jade.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/jade_internal.py` & `NREL-jade-0.9.9/jade/cli/jade_internal.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/pipeline.py` & `NREL-jade-0.9.9/jade/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/prune_files.py` & `NREL-jade-0.9.9/jade/cli/prune_files.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/resubmit_jobs.py` & `NREL-jade-0.9.9/jade/cli/resubmit_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/run.py` & `NREL-jade-0.9.9/jade/cli/run.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/run_jobs.py` & `NREL-jade-0.9.9/jade/cli/run_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/run_multi_node_job.py` & `NREL-jade-0.9.9/jade/cli/run_multi_node_job.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/run_spark_cluster.py` & `NREL-jade-0.9.9/jade/cli/run_spark_cluster.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/show_events.py` & `NREL-jade-0.9.9/jade/cli/show_events.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/show_results.py` & `NREL-jade-0.9.9/jade/cli/show_results.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/show_status.py` & `NREL-jade-0.9.9/jade/cli/show_status.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/spark.py` & `NREL-jade-0.9.9/jade/cli/spark.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/stats.py` & `NREL-jade-0.9.9/jade/cli/stats.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/submit_jobs.py` & `NREL-jade-0.9.9/jade/cli/submit_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/try_submit_jobs.py` & `NREL-jade-0.9.9/jade/cli/try_submit_jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/cli/wait.py` & `NREL-jade-0.9.9/jade/cli/wait.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/enums.py` & `NREL-jade-0.9.9/jade/enums.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/events.py` & `NREL-jade-0.9.9/jade/events.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/exceptions.py` & `NREL-jade-0.9.9/jade/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/autoregression_execution.py` & `NREL-jade-0.9.9/jade/extensions/demo/autoregression_execution.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/autoregression_inputs.py` & `NREL-jade-0.9.9/jade/extensions/demo/autoregression_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/autoregression_parameters.py` & `NREL-jade-0.9.9/jade/extensions/demo/autoregression_parameters.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/cli.py` & `NREL-jade-0.9.9/jade/extensions/demo/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/create_merge_pred_gdp.py` & `NREL-jade-0.9.9/jade/extensions/demo/create_merge_pred_gdp.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/demo/merge_pred_gdp.py` & `NREL-jade-0.9.9/jade/extensions/demo/merge_pred_gdp.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/generic_command/cli.py` & `NREL-jade-0.9.9/jade/extensions/generic_command/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_configuration.py` & `NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_execution.py` & `NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_execution.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_inputs.py` & `NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/generic_command/generic_command_parameters.py` & `NREL-jade-0.9.9/jade/extensions/generic_command/generic_command_parameters.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/extensions/registry.py` & `NREL-jade-0.9.9/jade/extensions/registry.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/common.py` & `NREL-jade-0.9.9/jade/hpc/common.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/fake_manager.py` & `NREL-jade-0.9.9/jade/hpc/fake_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/hpc_manager.py` & `NREL-jade-0.9.9/jade/hpc/hpc_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/hpc_manager_interface.py` & `NREL-jade-0.9.9/jade/hpc/hpc_manager_interface.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/hpc_submitter.py` & `NREL-jade-0.9.9/jade/hpc/hpc_submitter.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/local_manager.py` & `NREL-jade-0.9.9/jade/hpc/local_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/pbs_manager.py` & `NREL-jade-0.9.9/jade/hpc/pbs_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/hpc/slurm_manager.py` & `NREL-jade-0.9.9/jade/hpc/slurm_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/analysis_execution_base.py` & `NREL-jade-0.9.9/jade/jobs/analysis_execution_base.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/async_cli_command.py` & `NREL-jade-0.9.9/jade/jobs/async_cli_command.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/async_job_interface.py` & `NREL-jade-0.9.9/jade/jobs/async_job_interface.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/cluster.py` & `NREL-jade-0.9.9/jade/jobs/cluster.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_analysis.py` & `NREL-jade-0.9.9/jade/jobs/job_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_configuration.py` & `NREL-jade-0.9.9/jade/jobs/job_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_configuration_factory.py` & `NREL-jade-0.9.9/jade/jobs/job_configuration_factory.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_container_by_key.py` & `NREL-jade-0.9.9/jade/jobs/job_container_by_key.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_container_by_name.py` & `NREL-jade-0.9.9/jade/jobs/job_container_by_name.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_container_interface.py` & `NREL-jade-0.9.9/jade/jobs/job_container_interface.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_execution_interface.py` & `NREL-jade-0.9.9/jade/jobs/job_execution_interface.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_manager_base.py` & `NREL-jade-0.9.9/jade/jobs/job_manager_base.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_parameters_interface.py` & `NREL-jade-0.9.9/jade/jobs/job_parameters_interface.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_post_process.py` & `NREL-jade-0.9.9/jade/jobs/job_post_process.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_queue.py` & `NREL-jade-0.9.9/jade/jobs/job_queue.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_runner.py` & `NREL-jade-0.9.9/jade/jobs/job_runner.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/job_submitter.py` & `NREL-jade-0.9.9/jade/jobs/job_submitter.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/pipeline_manager.py` & `NREL-jade-0.9.9/jade/jobs/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/jobs/results_aggregator.py` & `NREL-jade-0.9.9/jade/jobs/results_aggregator.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/loggers.py` & `NREL-jade-0.9.9/jade/loggers.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/__init__.py` & `NREL-jade-0.9.9/jade/models/__init__.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/base.py` & `NREL-jade-0.9.9/jade/models/base.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/cluster_config.py` & `NREL-jade-0.9.9/jade/models/cluster_config.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/hpc.py` & `NREL-jade-0.9.9/jade/models/hpc.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/jobs.py` & `NREL-jade-0.9.9/jade/models/jobs.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/pipeline.py` & `NREL-jade-0.9.9/jade/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/singularity.py` & `NREL-jade-0.9.9/jade/models/singularity.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/spark.py` & `NREL-jade-0.9.9/jade/models/spark.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/submission_group.py` & `NREL-jade-0.9.9/jade/models/submission_group.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/models/submitter_params.py` & `NREL-jade-0.9.9/jade/models/submitter_params.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/resource_monitor.py` & `NREL-jade-0.9.9/jade/resource_monitor.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/result.py` & `NREL-jade-0.9.9/jade/result.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/fairscheduler.xml.template` & `NREL-jade-0.9.9/jade/spark/conf/fairscheduler.xml.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/log4j.properties.template` & `NREL-jade-0.9.9/jade/spark/conf/log4j.properties.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/metrics.properties.template` & `NREL-jade-0.9.9/jade/spark/conf/metrics.properties.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/spark-defaults.conf` & `NREL-jade-0.9.9/jade/spark/conf/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/spark-defaults.conf.template` & `NREL-jade-0.9.9/jade/spark/conf/spark-defaults.conf.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/spark-env.sh` & `NREL-jade-0.9.9/jade/spark/conf/spark-env.sh`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/spark-env.sh.template` & `NREL-jade-0.9.9/jade/spark/conf/spark-env.sh.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/conf/workers.template` & `NREL-jade-0.9.9/jade/spark/conf/workers.template`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/spark/metrics.py` & `NREL-jade-0.9.9/jade/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/custom_click_options.py` & `NREL-jade-0.9.9/jade/utils/custom_click_options.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/dataframe_utils.py` & `NREL-jade-0.9.9/jade/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/repository_info.py` & `NREL-jade-0.9.9/jade/utils/repository_info.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/run_command.py` & `NREL-jade-0.9.9/jade/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/sql.py` & `NREL-jade-0.9.9/jade/utils/sql.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/subprocess_manager.py` & `NREL-jade-0.9.9/jade/utils/subprocess_manager.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/timing_utils.py` & `NREL-jade-0.9.9/jade/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/jade/utils/utils.py` & `NREL-jade-0.9.9/jade/utils/utils.py`

 * *Files identical despite different names*

### Comparing `NREL-jade-0.9.8/setup.py` & `NREL-jade-0.9.9/setup.py`

 * *Files identical despite different names*

