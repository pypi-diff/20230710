# Comparing `tmp/maud-metabolic-models-0.5.0.1.tar.gz` & `tmp/maud-metabolic-models-0.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maud-metabolic-models-0.5.0.1.tar", last modified: Tue Jun  6 14:30:42 2023, max compression
+gzip compressed data, was "maud-metabolic-models-0.5.1.1.tar", last modified: Mon Jul 10 11:37:44 2023, max compression
```

## Comparing `maud-metabolic-models-0.5.0.1.tar` & `maud-metabolic-models-0.5.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 14:30:42.478769 maud-metabolic-models-0.5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/experimental_setup.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/inits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/input_data_train.json
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/expected_stan_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/inits.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/hardcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/id_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/kinetic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/prior_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_idatas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_stan_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/loading_maud_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/parsing_kinetic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/running_stan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/debug.stan
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/model.stan
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/out_of_sample_model.stan
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/experimental_setup.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/inits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/input_data_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/expected_stan_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/inits.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/hardcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/id_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/kinetic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/prior_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_idatas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_stan_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/loading_maud_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/parsing_kinetic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/running_stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/debug.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/out_of_sample_model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/zip-safe
```

### Comparing `maud-metabolic-models-0.5.0.1/LICENSE` & `maud-metabolic-models-0.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/PKG-INFO` & `maud-metabolic-models-0.5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.5.0.1
+Version: 0.5.1.1
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.5.0.1/README.rst` & `maud-metabolic-models-0.5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/setup.cfg` & `maud-metabolic-models-0.5.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = maud-metabolic-models
 url = https://github.com/biosustain/Maud
 download_url = https://pypi.org/project/maud-metabolic-models/
 author = Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 author_email = tedgro@dtu.dk
-version = 0.5.0.1
+version = 0.5.1.1
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `maud-metabolic-models-0.5.0.1/setup.py` & `maud-metabolic-models-0.5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/analysis.py` & `maud-metabolic-models-0.5.1.1/src/maud/analysis.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/cli.py` & `maud-metabolic-models-0.5.1.1/src/maud/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import arviz as az
 import click
 import importlib_resources
 
 from maud.data.example_inputs import linear
 from maud.getting_idatas import get_idata
 from maud.loading_maud_inputs import load_maud_input
-from maud.running_stan import predict, sample, simulate, variational
+from maud.running_stan import optimize, predict, sample, simulate, variational
 
 
 EXAMPLE_INPUT_PATH = importlib_resources.files(linear)._paths[0]
 
 
 @click.group()
 @click.help_option("--help", "-h")
@@ -147,14 +147,26 @@
     default=EXAMPLE_INPUT_PATH,
 )
 def simulate_command(data_path, output_dir, n):
     """Generate draws from the initial values."""
     click.echo(do_simulate(data_path, output_dir, n))
 
 
+@cli.command("optimize")
+@click.option("--output_dir", default=".", help="Where to save the output")
+@click.argument(
+    "data_path",
+    type=click.Path(exists=True, dir_okay=True, file_okay=False),
+    default=EXAMPLE_INPUT_PATH,
+)
+def optimize_command(data_path, output_dir):
+    """Optimize the model parameters."""
+    click.echo(do_optimize(data_path, output_dir))
+
+
 def do_simulate(data_path, output_dir, n):
     """Generate draws from the initial values."""
 
     mi = load_maud_input(data_path=data_path)
     now = datetime.now().strftime("%Y%m%d%H%M%S")
     output_name = f"maud_output_sim-{mi.config.name}-{now}"
     output_path = os.path.join(output_dir, output_name)
@@ -187,14 +199,121 @@
     print("\n\nSimulated enzyme concentrations:")
     print(
         idata.posterior["conc_enzyme_train"]
         .mean(dim=["chain", "draw"])
         .to_series()
         .unstack()
         .T
+    )
+    print("\n\nSimulated reaction delta Gs:")
+    print(idata.posterior["dgr_train"].mean(dim=["chain", "draw"]).to_series())
+    print("\n\nSimulated measurements:")
+    print(
+        idata.posterior_predictive["yrep_conc_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+    )
+    print(
+        idata.posterior_predictive["yrep_flux_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+    )
+    print("\n\nSimulated log likelihoods:")
+    print(
+        idata.log_likelihood["llik_conc_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+    )
+    print(
+        idata.log_likelihood["llik_flux_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+    )
+    print("\n\nSimulated allostery terms:")
+    print(
+        idata.posterior["allostery_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
+    )
+    print("\n\nSimulated reversibility terms:")
+    print(
+        idata.posterior["reversibility_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
+    )
+    print("\n\nSimulated saturation terms:")
+    print(
+        idata.posterior["saturation_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
+    )
+    if mi.kinetic_model.phosphorylations is not None:
+        print("\n\nSimulated phosphorylation terms:")
+        print(
+            idata.posterior["phosphorylation_train"]
+            .mean(dim=["chain", "draw"])
+            .to_series()
+            .unstack()
+            .T
+        )
+    print("\n\nSimulated membrane potential:")
+    print(
+        idata.posterior["psi_train"].mean(dim=["chain", "draw"]).to_series().T
+    )
+    return output_path
+
+
+def do_optimize(data_path, output_dir):
+    """Optimize the model parameters."""
+
+    mi = load_maud_input(data_path=data_path)
+    now = datetime.now().strftime("%Y%m%d%H%M%S")
+    output_name = f"maud_output_opt-{mi.config.name}-{now}"
+    output_path = os.path.join(output_dir, output_name)
+    samples_path = os.path.join(output_path, "samples")
+    ui_dir = os.path.join(output_path, "user_input")
+    print("Creating output directory: " + output_path)
+    os.mkdir(output_path)
+    os.mkdir(samples_path)
+    print(f"Copying user input from {data_path} to {ui_dir}")
+    shutil.copytree(data_path, ui_dir)
+    stanfit = optimize(mi, samples_path)
+    idata = get_idata(stanfit.runset.csv_files, mi, "train")
+    idata.to_json(os.path.join(output_path, "idata.json"))
+    print("\n\nSimulated concentrations:")
+    print(
+        idata.posterior["conc_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
+    )
+    print("\n\nSimulated fluxes:")
+    print(
+        idata.posterior["flux_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
+    )
+    print("\n\nSimulated kms:")
+    print(idata.posterior["km"].mean(dim=["chain", "draw"]).to_series())
+    print("\n\nSimulated enzyme concentrations:")
+    print(
+        idata.posterior["conc_enzyme_train"]
+        .mean(dim=["chain", "draw"])
+        .to_series()
+        .unstack()
+        .T
     )
     print("\n\nSimulated reaction delta Gs:")
     print(idata.posterior["dgr_train"].mean(dim=["chain", "draw"]).to_series())
     print("\n\nSimulated measurements:")
     print(
         idata.posterior_predictive["yrep_conc_train"]
         .mean(dim=["chain", "draw"])
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/inits.json` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/inits.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/input_data_train.json` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/input_data_train.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/priors.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/expected_stan_input.json` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/expected_stan_input.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920212765957447%*

 * *Differences: {"'N_conc_measurement_train'": '7',*

 * * "'experiment_yconc_train'": '{delete: [0]}',*

 * * "'mic_ix_yconc_train'": '{delete: [1]}',*

 * * "'sigma_yconc_train'": '{delete: [0]}',*

 * * "'yconc_train'": '{delete: [1]}'}*

```diff
@@ -1,12 +1,12 @@
 {
     "N_allosteric_enzyme": 2,
     "N_allostery": 2,
     "N_competitive_inhibition": 1,
-    "N_conc_measurement_train": 8,
+    "N_conc_measurement_train": 7,
     "N_drain": 0,
     "N_edge": 3,
     "N_edge_prod": 3,
     "N_edge_sub": 3,
     "N_enzyme": 3,
     "N_enzyme_knockout_train": 0,
     "N_enzyme_measurement_train": 6,
@@ -150,15 +150,14 @@
         2,
         3
     ],
     "experiment_yconc_train": [
         1,
         1,
         1,
-        1,
         2,
         2,
         2,
         2
     ],
     "experiment_yenz_train": [
         1,
@@ -172,15 +171,14 @@
         1,
         2
     ],
     "likelihood": 1,
     "max_num_steps": 1000000,
     "mic_ix_yconc_train": [
         2,
-        3,
         1,
         4,
         2,
         3,
         1,
         4
     ],
@@ -407,15 +405,14 @@
         3,
         3
     ],
     "reject_non_steady": 1,
     "rel_tol": 1e-05,
     "sigma_yconc_train": [
         0.1,
-        0.1,
         0.05,
         0.05,
         0.1,
         0.1,
         0.05,
         0.05
     ],
@@ -493,15 +490,14 @@
     "water_stoichiometry": [
         0.0,
         0.0,
         0.0
     ],
     "yconc_train": [
         0.59,
-        0.38,
         1.09,
         1.05,
         0.54,
         0.38,
         1.12,
         1.14
     ],
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/experiments.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/kinetic_model.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/parameters.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/priors.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/experiments.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/inits.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/inits.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/parameters.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/priors.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/experiments.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/experiments.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [[experiment]]
 id = "condition1"
 is_train = true
 is_test = true
 temperature = 299.0
 measurements = [
   {target_type = "mic", metabolite = "M1", compartment = "c", value = 0.59, error_scale = 0.1},
-  {target_type = "mic", metabolite = "M2", compartment = "c", value = 0.38, error_scale = 0.1},
   {target_type = "mic", metabolite = "M1", compartment = "e", value = 1.09, error_scale = 0.05},
   {target_type = "mic", metabolite = "M2", compartment = "e", value = 1.05, error_scale = 0.05},
   {target_type = "flux", reaction = "r3", value = 0.19, error_scale = 0.1},
   {target_type = "enzyme", enzyme = "r1", value = 1.5, error_scale = 0.1},
   {target_type = "enzyme", enzyme = "r2", value = 1.5, error_scale = 0.1},
   {target_type = "enzyme", enzyme = "r3", value = 1.5, error_scale = 0.1},
 ]
+initial_state = [
+  {metabolite = "M2", compartment = "c", value = 0.38},
+]
 
 [[experiment]]
 id = "condition2"
 is_train = true
 is_test = true
 measurements = [
   {target_type = "mic", metabolite = "M1", compartment = "c", value = 0.54, error_scale = 0.1},
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/parameters.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/priors.toml` & `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/experiment.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/experiment.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,27 +72,42 @@
 
     def __post_init__(self):
         """Add id field."""
         self.id = ID_SEPARATOR.join(["pko", self.experiment, self.enzyme])
 
 
 @dataclass
+class InitConcentration:
+    """Indication of the initial value of a concentration in the ODE."""
+
+    metabolite: str
+    compartment: str
+    value: float
+    target_id: str = Field(default=None, init=False, exclude=True)
+
+    def __post_init__(self):
+        """Add target_id field."""
+        self.target_id = ID_SEPARATOR.join([self.metabolite, self.compartment])
+
+
+@dataclass
 class Experiment:
     """Maud representation of an experiment.
 
     This means a case where the boundary conditions and all measured quantities
     can be assumed to be the same - often the term "condition" is used for this.
 
     """
 
     id: str
     is_train: bool
     is_test: bool
     temperature: float = 298.15
     measurements: List[Measurement] = Field(default_factory=lambda: [])
+    initial_state: List[InitConcentration] = Field(default_factory=lambda: [])
     enzyme_knockouts: List[EnzymeKnockout] = Field(default_factory=lambda: [])
     pme_knockouts: List[PhosphorylationModifyingEnzymeKnockout] = Field(
         default_factory=lambda: []
     )
 
     @validator("temperature")
     def temp_must_be_non_negative(cls, v):
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/kinetic_model.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/kinetic_model.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_config.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     :param likelihood: Whether or not to take measurements into account.
     :param cmdstanpy_config: Arguments to cmdstanpy.CmdStanModel.sample.
     :param reject_non_steady: Reject draws if a non-steady state is encountered.
     :param ode_config: Configuration for Stan's ode solver.
     :param stanc_options: Valid choices for CmdStanModel argument `stanc_options`.
     :param cpp_options: Valid choices for CmdStanModel `cpp_options`.
     :param variational_options: Arguments for CmdStanModel.variational.
+    :param optimize_options: Arguments for CmdStanModel.optimize.
     :param user_inits_file: path to a csv file of initial values.
     :param steady_state_threshold_abs: absolute threshold for Sv=0 be at steady state
     :param steady_state_threshold_rel: relative threshold for Sv=0 be at steady state
     :param default_initial_concentration: in molecule_unit per volume_unit
     :param drain_small_conc_corrector: number for correcting small conc drains
     :param molecule_unit: A unit for counting molecules, like 'mol' or 'mmol'
     :param volume_unit: A unit for measuring volume, like 'L'
@@ -45,14 +46,15 @@
     experiments_file: str
     likelihood: bool
     cmdstanpy_config: Optional[dict] = None
     cmdstanpy_config_predict: Optional[dict] = None
     stanc_options: Optional[dict] = None
     cpp_options: Optional[dict] = None
     variational_options: Optional[dict] = None
+    optimize_options: Optional[dict] = None
     user_inits_file: Optional[str] = None
     ode_config: ODEConfig = Field(default_factory=ODEConfig)
     reject_non_steady: bool = True
     steady_state_threshold_abs: float = 1e-8
     steady_state_threshold_rel: float = 1e-3
     default_initial_concentration: float = 0.01
     drain_small_conc_corrector: float = 1e-6
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_init.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_init.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_input.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_parameter.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_parameter.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/prior.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/prior.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/data_model/prior_input.py` & `maud-metabolic-models-0.5.1.1/src/maud/data_model/prior_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/getting_idatas.py` & `maud-metabolic-models-0.5.1.1/src/maud/getting_idatas.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/getting_parameters.py` & `maud-metabolic-models-0.5.1.1/src/maud/getting_parameters.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/getting_priors.py` & `maud-metabolic-models-0.5.1.1/src/maud/getting_priors.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/getting_stan_inputs.py` & `maud-metabolic-models-0.5.1.1/src/maud/getting_stan_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,15 +505,15 @@
     balanced_mics = [m for m in kinetic_model.mics if m.balanced]
     inits = [[default for _ in balanced_mics] for e in experiments]
     for i, experiment in enumerate(experiments):
         msmts = [
             m
             for m in experiment.measurements
             if m.target_type == MeasurementType.MIC
-        ]
+        ] + experiment.initial_state
         for j, mic in enumerate(balanced_mics):
             if any(mic.id == m.target_id for m in msmts):
                 inits[i][j] = gmean(
                     [m.value for m in msmts if mic.id == m.target_id]
                 )
     inits_train = [
         inits[i] for i, exp in enumerate(experiments) if exp.is_train
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/loading_maud_inputs.py` & `maud-metabolic-models-0.5.1.1/src/maud/loading_maud_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/parsing_kinetic_models.py` & `maud-metabolic-models-0.5.1.1/src/maud/parsing_kinetic_models.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/running_stan.py` & `maud-metabolic-models-0.5.1.1/src/maud/running_stan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code for sampling from a posterior distribution."""
 
 import os
 
 import arviz as az
 import cmdstanpy
+from cmdstanpy import CmdStanMLE
 from cmdstanpy.stanfit.mcmc import CmdStanMCMC
 from cmdstanpy.stanfit.vb import CmdStanVB
 
 from maud.data_model.maud_input import MaudInput
 
 
 HERE = os.path.dirname(os.path.abspath(__file__))
@@ -38,14 +39,25 @@
 SIM_CONFIG = {
     "chains": 1,
     "fixed_param": True,
     "iter_warmup": 0,
     "show_progress": False,
     "threads_per_chain": 1,
 }
+DEFAULT_OPTIMIZE_CONFIG = {
+    "algorithm": "LBFGS",
+    "iter": 3000,
+    "init_alpha": 1e-4,
+    "tol_param": 1e-12,
+    "history_size": 10,
+    "show_console": True,
+    "refresh": 1,
+    "save_profile": True,
+    "save_iterations": True,
+}
 
 
 def sample(mi: MaudInput, output_dir: str) -> CmdStanMCMC:
     """Sample from the posterior defined by mi.
 
     :param mi: a MaudInput object
     :param output_dir: a string specifying where to save the output.
@@ -112,14 +124,40 @@
         iter_sampling=n,
         data=os.path.join(output_dir, "input_data_train.json"),
         inits=os.path.join(output_dir, "inits.json"),
         **SIM_CONFIG,
     )
 
 
+def optimize(mi: MaudInput, output_dir: str) -> CmdStanMLE:
+    """Generate MLE from the input maud model.
+
+    :param mi: a MaudInput object
+    :param output_dir: a string specifying where to save the output.
+    """
+    mi_options = (
+        {} if mi.config.optimize_options is None else mi.config.optimize_options
+    )
+    model = cmdstanpy.CmdStanModel(
+        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH),
+        cpp_options=mi.config.cpp_options,
+        stanc_options=mi.config.stanc_options,
+    )
+    set_up_output_dir(output_dir, mi)
+    return model.optimize(
+        data=os.path.join(output_dir, "input_data_train.json"),
+        inits=os.path.join(output_dir, "inits.json"),
+        output_dir=output_dir,
+        **{
+            **DEFAULT_OPTIMIZE_CONFIG,
+            **mi_options,
+        },
+    )
+
+
 def set_up_output_dir(output_dir: str, mi: MaudInput):
     """Write input data and inits to the output directory."""
     input_path_train = os.path.join(output_dir, "input_data_train.json")
     input_path_test = os.path.join(output_dir, "input_data_test.json")
     inits_path = os.path.join(output_dir, "inits.json")
     cmdstanpy.utils.write_stan_json(input_path_train, mi.stan_input_train)
     if mi.stan_input_test is not None:
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/stan/functions.stan` & `maud-metabolic-models-0.5.1.1/src/maud/stan/functions.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/stan/model.stan` & `maud-metabolic-models-0.5.1.1/src/maud/stan/model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/stan/out_of_sample_model.stan` & `maud-metabolic-models-0.5.1.1/src/maud/stan/out_of_sample_model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud/utils.py` & `maud-metabolic-models-0.5.1.1/src/maud/utils.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/PKG-INFO` & `maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.5.0.1
+Version: 0.5.1.1
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/SOURCES.txt` & `maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

