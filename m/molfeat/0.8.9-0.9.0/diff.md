# Comparing `tmp/molfeat-0.8.9.tar.gz` & `tmp/molfeat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.9.tar", last modified: Mon May 22 03:06:09 2023, max compression
+gzip compressed data, was "molfeat-0.9.0.tar", last modified: Mon Jul 10 19:41:46 2023, max compression
```

## Comparing `molfeat-0.8.9.tar` & `molfeat-0.9.0.tar`

### file list

```diff
@@ -1,174 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-22 03:05:53.000000 molfeat-0.8.9/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 03:04:49.000000 molfeat-0.8.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 03:05:53.000000 molfeat-0.8.9/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-22 03:05:53.000000 molfeat-0.8.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 03:05:54.000000 molfeat-0.8.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-22 03:04:49.000000 molfeat-0.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-22 03:06:09.774696 molfeat-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-22 03:04:49.000000 molfeat-0.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.754696 molfeat-0.8.9/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/custom_model_store.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 03:04:49.000000 molfeat-0.8.9/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 03:04:49.000000 molfeat-0.8.9/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:06:02.000000 molfeat-0.8.9/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/nb/etl/
--rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/chemberta-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/chemgpt-fix-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/dgl-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/entropy-transforner-zinc-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/featurizer-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/molt5-etl.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 03:04:49.000000 molfeat-0.8.9/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 03:04:49.000000 molfeat-0.8.9/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-22 03:04:49.000000 molfeat-0.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 03:04:49.000000 molfeat-0.8.9/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:06:09.774696 molfeat-0.8.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.071054 molfeat-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/5_community_contribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-10 19:38:29.000000 molfeat-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-10 19:38:29.000000 molfeat-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-07-10 19:38:29.000000 molfeat-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-10 19:41:46.067054 molfeat-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-10 19:38:29.000000 molfeat-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.047053 molfeat-0.9.0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   110397 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/community/contributions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/community/get_involved.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/custom_model_store.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60168 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-10 19:38:29.000000 molfeat-0.9.0/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-10 19:38:29.000000 molfeat-0.9.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33609 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-10 19:41:46.000000 molfeat-0.9.0/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:41:40.000000 molfeat-0.9.0/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.047053 molfeat-0.9.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/nb/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/chemberta-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/chemgpt-fix-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/dgl-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/entropy-transforner-zinc-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/featurizer-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/molt5-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-10 19:38:29.000000 molfeat-0.9.0/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-10 19:38:29.000000 molfeat-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:41:46.071054 molfeat-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_viz.py
```

### Comparing `molfeat-0.8.9/.github/CODE_OF_CONDUCT.md` & `molfeat-0.9.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.9.0/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.9.0/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.9.0/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.9.0/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.9.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/.github/workflows/doc.yml` & `molfeat-0.9.0/.github/workflows/doc.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 name: doc
 
 on:
   push:
     branches: ["main"]
-    tags: ["*"]
 
 # Prevent doc action on `main` to conflict with each others.
 concurrency:
   group: doc-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   doc:
-    runs-on: ubuntu-latest
+    runs-on: "ubuntu-latest"
+    timeout-minutes: 30
+
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
       - name: Checkout the code
         uses: actions/checkout@v3
 
-      - name: Setup conda
-        uses: mamba-org/provision-with-micromamba@v15
+      - name: Setup mamba
+        uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: env.yml
-          environment-name: molfeat
+          environment-name: my_env
+          cache-environment: true
           cache-downloads: true
-          cache-env: true
 
       - name: Install library
         run: python -m pip install --no-deps .
 
-      - name: Deploy the doc
+      - name: Configure git
         run: |
-          echo "Configure git"
-          git config --global user.name 'maclandrol'
-          git config --global user.email 'maclandrol@users.noreply.github.com'
+          git config --global user.name "${GITHUB_ACTOR}"
+          git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
+      - name: Deploy the doc
+        run: |
           echo "Get the gh-pages branch"
           git fetch origin gh-pages
 
-          TAG_OR_BRANCH_NAME=${GITHUB_REF##*/}
-          if [ $TAG_OR_BRANCH_NAME = "main" ]; then
-            echo "Build and deploy the doc on main"
-            mike deploy --push --force main
-          else
-            echo "Build and deploy the doc on $TAG_OR_BRANCH_NAME"
-            mike deploy --push --force stable
-            mike deploy --push --force $TAG_OR_BRANCH_NAME
-          fi
+          echo "Build and deploy the doc on main"
+          mike deploy --push --force main
```

### Comparing `molfeat-0.8.9/.github/workflows/release.yml` & `molfeat-0.9.0/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     inputs:
       release-version:
         description: "A valid Semver version string"
         required: true
 
 permissions:
   contents: write
+  pull-requests: write
 
 jobs:
   release:
     # Do not release if not triggered from the default branch
     if: github.ref == format('refs/heads/{0}', github.event.repository.default_branch)
 
     runs-on: ubuntu-latest
@@ -22,25 +23,24 @@
       run:
         shell: bash -l {0}
 
     steps:
       - name: Checkout the code
         uses: actions/checkout@v3
 
-      - name: Setup Mamba
-        uses: mamba-org/provision-with-micromamba@v15
+      - name: Setup mamba
+        uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: env.yml
-          environment-name: release
+          environment-name: my_env
+          cache-environment: true
           cache-downloads: true
-          cache-env: true
-          extra-specs: |
+          create-args: >-
             pip
             semver
-            rever==0.5.1
             python-build
             setuptools_scm
 
       - name: Check the version is valid semver
         run: |
           RELEASE_VERSION="${{ inputs.release-version }}"
 
@@ -65,31 +65,38 @@
 
           if [ "$IS_HIGHER_VERSION" != "1" ]; then
             echo "The version '$RELEASE_VERSION' is not higher than the latest version '$LATEST_VERSION'."
             echo "The release process is aborted."
             exit 1
           fi
 
+      - name: Build Changelog
+        id: github_release
+        uses: mikepenz/release-changelog-builder-action@v4
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+          toTag: "main"
+
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
-      - name: Perform the release with rever
-        run: |
-          rever ${{ inputs.release-version }}
-
       - name: Create and push git tag
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           # Tag the release
           git tag -a "${{ inputs.release-version }}" -m "Release version ${{ inputs.release-version }}"
 
-          # Push the commit from rever to main
+          # Checkout the git tag
+          git checkout "${{ inputs.release-version }}"
+
+          # Push the modified changelogs
           git push origin main
 
           # Push the tags
           git push origin "${{ inputs.release-version }}"
 
       - name: Install library
         run: python -m pip install --no-deps .
@@ -103,8 +110,17 @@
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
-          body: "See [CHANGELOGS.rst](https://github.com/datamol-io/molfeat/blob/main/CHANGELOG.rst)."
+          body: ${{steps.github_release.outputs.changelog}}
+
+      - name: Deploy the doc
+        run: |
+          echo "Get the gh-pages branch"
+          git fetch origin gh-pages
+
+          echo "Build and deploy the doc on ${{ inputs.release-version }}"
+          mike deploy --push --force stable
+          mike deploy --push --force ${{ inputs.release-version }}
```

### Comparing `molfeat-0.8.9/.github/workflows/test.yml` & `molfeat-0.9.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,43 +14,42 @@
 jobs:
   build-test:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
         os: ["ubuntu-latest"] #, "macos-latest", "windows-latest"]
-        pytorch-lightning-version: ["1.8", "1.9"]
-        pytorch-version: ["1.11"]
+        pytorch-version: ["1.12"]
 
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
 
     defaults:
       run:
         shell: bash -l {0}
 
     name: |
       os=${{ matrix.os }}
       - python=${{ matrix.python-version }}
-      - pytorch-lightning=${{ matrix.pytorch-lightning-version }}
       - pytorch=${{ matrix.pytorch-version }}
 
     steps:
       - name: Checkout the code
         uses: actions/checkout@v3
 
-      - name: Setup conda
-        uses: mamba-org/provision-with-micromamba@v15
+      - name: Setup mamba
+        uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: env.yml
-          environment-name: molfeat
+          environment-name: my_env
+          cache-environment: true
           cache-downloads: true
-          cache-env: true
-          extra-specs: |
+          create-args: >-
             python=${{ matrix.python-version }}
+            pytorch=${{ matrix.pytorch-version }}
 
       - name: Install library
         run: python -m pip install --no-deps .
 
       - name: Run pytest
         run: pytest
```

### Comparing `molfeat-0.8.9/.gitignore` & `molfeat-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/CHANGELOG.rst` & `molfeat-0.9.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,171 @@
-==================
-molfeat Change Log
-==================
+# Molfeat Changelogs
 
-.. current developments
+_Only changelogs previous to 0.8.10. See the GitHub releases for new changelogs._
 
-v0.8.9
-====================
+## v0.8.9
 
 **Added:**
 
-* Support for new featurizers (GPT2-Zinc480M-87M and  Roberta-Zinc480M-102M)
-* ETL scripts/notebooks for transparency
+- Support for new featurizers (GPT2-Zinc480M-87M and
+  Roberta-Zinc480M-102M)
+- ETL scripts/notebooks for transparency
 
 **Fixed:**
 
-* Nav Bar with Tabs
-* Typos in docs
+- Nav Bar with Tabs
+- Typos in docs
 
 **Authors:**
 
-* Cas Wognum
-* Emmanuel Noutahi
+- Cas Wognum
+- Emmanuel Noutahi
 
-
-
-v0.8.8
-====================
+## v0.8.8
 
 **Added:**
 
-* A model named Molt5
-* Existing plugins to a the `plugin.yml` file
-* Documents missing featurizers
+- A model named Molt5
+- Existing plugins to a the `plugin.yml` file
+- Documents missing featurizers
 
 **Changed:**
 
-* Different docs style, with Tabs on the top for `Overview`, `Usage`, `Tutorials`, `API`, `Contribute`, `License`
-* Small updates in docs
+- Different docs style, with Tabs on the top for `Overview`, `Usage`,
+  `Tutorials`, `API`, `Contribute`, `License`
+- Small updates in docs
 
 **Fixed:**
 
-* Fix #43: Pretrained models should now work better with `batch_transform`,  allowing efficient parallelization, while retaining all cached features.
+- Fix #43: Pretrained models should now work better with
+  `batch_transform`, allowing efficient parallelization, while
+  retaining all cached features.
 
 **Authors:**
 
-* DomInvivo
-* dessygil
-* maclandrol
-
+- DomInvivo
+- dessygil
+- maclandrol
 
-
-v0.8.7
-====================
+## v0.8.7
 
 **Added:**
 
-* Support for `ignore_padding` in Graphormer
-* More flexibility overall for graphormer embeddings
+- Support for `ignore_padding` in Graphormer
+- More flexibility overall for graphormer embeddings
 
 **Changed:**
 
-* Phased out rdchem.Mol, rdchem.Atom and rdkit.Bond in favor of datamol versions
-* Fully automated release process.
+- Phased out rdchem.Mol, rdchem.Atom and rdkit.Bond in favor of
+  datamol versions
+- Fully automated release process.
 
 **Fixed:**
 
-* Random logging in cache coming from testing if an input is a molecule
-* Some small typos in doc strings
-* Naming of JTVAE models
-* Fix issue #37 by making WeaveFeaturizer faster
-* Usage card for rdkit and fingerprints/descriptors featurizers
+- Random logging in cache coming from testing if an input is a
+  molecule
+- Some small typos in doc strings
+- Naming of JTVAE models
+- Fix issue #37 by making WeaveFeaturizer faster
+- Usage card for rdkit and fingerprints/descriptors featurizers
 
 **Authors:**
 
-* Hadrien Mary
-* maclandrol
-* rbyrne-momatx
-
+- Hadrien Mary
+- maclandrol
+- rbyrne-momatx
 
-
-v0.8.6
-====================
+## v0.8.6
 
 **Added:**
 
-* Support for batch transformation in `MoleculeTransformer` for calculators that implements `batch_compute`
+- Support for batch transformation in `MoleculeTransformer` for
+  calculators that implements `batch_compute`
 
 **Changed:**
 
-* Pull request template for better directive.
+- Pull request template for better directive.
 
 **Authors:**
 
-* maclandrol
-
-
+- maclandrol
 
-v0.8.5
-====================
+## v0.8.5
 
 **Authors:**
 
-
-
-
-v0.8.4
-====================
+## v0.8.4
 
 **Added:**
 
-* Add Google Analytics support.
+- Add Google Analytics support.
 
 **Removed:**
 
-* Remove support for the `np.float128` dtype (issue #26)
+- Remove support for the `np.float128` dtype (issue #26)
 
 **Fixed:**
 
-* Color bug of the search input bar
+- Color bug of the search input bar
 
 **Authors:**
 
-* Cas Wognum
-* Honore Hounwanou
-* maclandrol
-
-
+- Cas Wognum
+- Honore Hounwanou
+- maclandrol
 
-v0.8.3
-====================
+## v0.8.3
 
 **Added:**
 
-* More documentation and tutorials
-* pip dependencies and optional dependencies in pyproject.toml
-* Github issue templates
+- More documentation and tutorials
+- pip dependencies and optional dependencies in pyproject.toml
+- Github issue templates
 
 **Changed:**
 
-* Updated all occurrences of old molfeat links with new ones.
-* Documentation and readme
+- Updated all occurrences of old molfeat links with new ones.
+- Documentation and readme
 
 **Removed:**
 
-* duplicated CODEOWNER file
+- duplicated CODEOWNER file
 
 **Fixed:**
 
-* Bug in serialization of transformers with a serializable calculator
-* Minor typos and function definition
-* Links in pyprojects
+- Bug in serialization of transformers with a serializable calculator
+- Minor typos and function definition
+- Links in pyprojects
 
 **Authors:**
 
-* Cas Wognum
-* Hadrien Mary
-* Honore Hounwanou
-* Saurav Maheshkar
-* Therence
-* maclandrol
-
-
+- Cas Wognum
+- Hadrien Mary
+- Honore Hounwanou
+- Saurav Maheshkar
+- Therence
+- maclandrol
 
-v0.8.1
-====================
+## v0.8.1
 
 **Added:**
 
-* Extended the simple benchmark in the docs to also include a search benchmark, based on the RDKit benchmarking platform
-* Added missing API documentation for `molfeat.plugins` and `molfeat.store`.
+- Extended the simple benchmark in the docs to also include a search
+  benchmark, based on the RDKit benchmarking platform
+- Added missing API documentation for `molfeat.plugins` and
+  `molfeat.store`.
 
 **Changed:**
 
-* Changed the styling of the docs to match the new datamol.io styling.
+- Changed the styling of the docs to match the new datamol.io styling.
 
 **Authors:**
 
-* Cas Wognum
-* Hadrien Mary
-* Therence
+- Cas Wognum
+- Hadrien Mary
+- Therence
 
-
-
-v0.8.0
-====================
+## v0.8.0
 
 **Authors:**
 
-* Hadrien Mary
-
-
+- Hadrien Mary
```

### Comparing `molfeat-0.8.9/LICENSE` & `molfeat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/PKG-INFO` & `molfeat-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.9
+Version: 0.9.0
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -143,19 +143,17 @@
 
 ## How to cite
 
 Please cite Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667).
 
 ## Contribute
 
-See [developers](docs/developers/) for a comprehensive guide on how to contribute to `Molfeat`
-
-## Changelogs
-
-See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
+See [developers](docs/developers/) for a comprehensive guide on how to contribute to `molfeat`. `molfeat` is a community-led
+initiative and whether you're a first-time contributor or an open-source veteran, this project greatly benefits from your contributions.
+To learn more about the community and [datamol.io](https://datamol.io/) ecosystem, please see [community](docs/community/).
 
 ## Maintainers
 
 - @cwognum
 - @maclandrol
 - @hadim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.9 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.0 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -92,10 +92,13 @@
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
-contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
-@hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
+contribute to `molfeat`. `molfeat` is a community-led initiative and whether
+you're a first-time contributor or an open-source veteran, this project greatly
+benefits from your contributions. To learn more about the community and
+[datamol.io](https://datamol.io/) ecosystem, please see [community](docs/
+community/). ## Maintainers - @cwognum - @maclandrol - @hadim ## License Under
+the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.9/README.md` & `molfeat-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,17 @@
 
 ## How to cite
 
 Please cite Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667).
 
 ## Contribute
 
-See [developers](docs/developers/) for a comprehensive guide on how to contribute to `Molfeat`
-
-## Changelogs
-
-See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
+See [developers](docs/developers/) for a comprehensive guide on how to contribute to `molfeat`. `molfeat` is a community-led
+initiative and whether you're a first-time contributor or an open-source veteran, this project greatly benefits from your contributions.
+To learn more about the community and [datamol.io](https://datamol.io/) ecosystem, please see [community](docs/community/).
 
 ## Maintainers
 
 - @cwognum
 - @maclandrol
 - @hadim
```

#### html2text {}

```diff
@@ -72,10 +72,13 @@
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
-contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
-@hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
+contribute to `molfeat`. `molfeat` is a community-led initiative and whether
+you're a first-time contributor or an open-source veteran, this project greatly
+benefits from your contributions. To learn more about the community and
+[datamol.io](https://datamol.io/) ecosystem, please see [community](docs/
+community/). ## Maintainers - @cwognum - @maclandrol - @hadim ## License Under
+the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.9/docs/api/molfeat.calc.md` & `molfeat-0.9.0/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/assets/css/custom-molfeat.css` & `molfeat-0.9.0/docs/assets/css/custom-molfeat.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/assets/css/custom.css` & `molfeat-0.9.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/developers/contribute.md` & `molfeat-0.9.0/docs/developers/contribute.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 # Contribute
 
-Welcome to the molfeat community! We appreciate everyone's contribution and welcome all. Apart from code contributions, there are various other ways to support the community such as answering questions, providing assistance to others, enhancing the documentation, giving a ⭐️ or sharing the project.
+Welcome to the molfeat community! We appreciate everyone's contribution and welcome all. Apart from code contributions, there are various other ways to support the community. If you would like to get involved, please see the [community documentation](../community/get_involved.md) for more details on how to contribute. However you choose to contribute, please be mindful and respect our [code of conduct](https://github.com/datamol-io/molfeat/blob/main/.github/CODE_OF_CONDUCT.md).
 
-However you choose to contribute, please be mindful and respect our [code of conduct](https://github.com/datamol-io/molfeat/blob/main/.github/CODE_OF_CONDUCT.md).
-
-
-## Ways to contribute
-
-You can contribute to molfeat in several ways:
-
-- Fix existing code issues.
-- Submit issues related to bugs or new features.
-- Suggest or implement new featurizers.
-- Improve existing documentation or add new tutorials. 
-
-For a more detailed description of the development lifecycle of molfeat, please refer to the rest of this document.
+!!! note annotate "Get inspired by community contributions"
+    As we love community contributions, we decided to create a dedicate space in our documentation to highlight and celebrate such contributions.
+    Visit [Community Contribitons](../community/contributions.md) to learn more!
 
+The rest of this page details the development lifecycle of molfeat.
 
 ## Setup a dev environment
 
-First you'll need to fork and clone the repository. Once you have a local copy, install the dependencies. 
+First you'll need to fork and clone the repository. Once you have a local copy, install the dependencies.
 It is strongly recommended that you do so in a new conda environment.
 
-
 ```bash
 mamba env create -n molfeat -f env.yml
-conda activate molfeat
+mamba activate molfeat
 pip install -e .
 ```
 
-
 ## Continuous Integration
 
 molfeat uses Github Actions to:
 
 - **Build and test** `molfeat`.
 - **Check code formating** the code: `black`.
 - **Documentation**: build and deploy the documentation on `main` and for every new git tag.
@@ -49,33 +38,27 @@
 You can build and serve the documentation locally with:
 
 ```bash
 # Build and serve the doc
 mkdocs serve
 ```
 
-
 ## Submitting Pull Requests
 
 If you're considering a large code contribution to molfeat, please open an issue first to get early feedback on the idea.
 
 Once you think the code is ready to be reviewed, push it to your fork and open a pull request. We will assign a reviewer to your PR.
 For a change to be accepted all existing tests will need to pass. We expect additional tests and documentation for any new features.
 
 If you are developing a plugin for molfeat, please refer to the corresponding section [Extending molfeat](./create-plugin.md)
 
-
-## Adding ETL notebooks
-
-Here's an improved version:
-
 ## Adding ETL Notebooks
 
 The ETL (extraction, transformation, and loading) scripts document the process of creating new featurizers, and we make our ETL notebooks open to the community for transparency purposes. As a developer adding new featurizers, please document your process in the [etl notebook folder](https://github.com/datamol-io/molfeat/tree/main/nb/etl).
 
 By documenting your process in the ETL notebook, you help ensure that the registration of new models can be reviewed by the community and provide greater visibility into the development process. This can help build trust with our users and contributors, and encourage collaboration and feedback.
 
 ## Releasing a New Version
 
 To release a new version, code maintainers can use the `release` GitHub action. However, before releasing a new version, it is important to coordinate with the code owners to ensure that the release roadmap is followed and any critical pull requests have been merged.
 
-The release roadmap should be followed to ensure that the new version is stable, functional, and meets the requirements of the release. This includes proper testing, documentation, and ensuring backward compatibility where necessary. By following these guidelines, we can ensure that new versions are released smoothly and efficiently, with clear communication to our users and contributors.
+The release roadmap should be followed to ensure that the new version is stable, functional, and meets the requirements of the release. This includes proper testing, documentation, and ensuring backward compatibility where necessary. By following these guidelines, we can ensure that new versions are released smoothly and efficiently, with clear communication to our users and contributors.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `molfeat-0.8.9/docs/developers/create-plugin.md` & `molfeat-0.9.0/docs/developers/create-plugin.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Molecular featurization is an active area of research leading to the steady emergence of new approaches to solve this complex set of problems. As new molecular featurizers emerge, you can easily add yours to molfeat and share it with the rest of the community.
 
 For developers that are planning to extend molfeat functionality, we recommend using the [plugin system](https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/). The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently of the core package, removing the bottleneck of a central party that reviews and approves new plugins.
 
 However, plugins are not always required and sometimes a simple pull request is the better option. 
 
 | :heavy_check_mark: **Do** use plugins if...                                          | :x: **Do not** use plugins if...                                                                                           |
-| ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
+|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
 | If a new featurizer can not be loaded by current classes.                            | If a new featurizer can already be loaded through existing classes.                                                        |
 | If a new featurizer requires additional, possibly difficult-to-install dependencies. | If a new featurizer requires no additional dependencies.                                                                   |
 | If you want to make a new class of featurizers available to the molfeat community.   | If you can show through benchmarks that a featurizer is so performant, it should be available as part of the core package. |
 | If you want to extend the functionality of molfeat for private / internal use.       |                                                                                                                            |
 
 
 !!! note annotate "Decided you don't need a plugin after all?"
```

### Comparing `molfeat-0.8.9/docs/developers/register-plugin.md` & `molfeat-0.9.0/docs/developers/register-plugin.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 The `molfeat` plugin registry aims to be the home for all publicly available `molfeat` plugins. It
 collects information on the type of plugins provided by your package and which `molfeat` versions it is compatible with.
 
 If you are starting to develop a new plugin or if you already have one, please register it here.
 We strongly encourage you to **register at early stages of development**, both to reserve the name of your plugin and to inform the community of your ongoing work.
 
+!!! note annotate "Curious what other plugins exist?"
+    Visit [Community contributions](../community/contributions.md) to learn more about the current plugins!
 
 ## How to register a plugin
 
 1. Fork this repository
 2. Add your plugin to the end of the `plugins.yaml` file, e.g.
     ```
     ...
```

### Comparing `molfeat-0.8.9/docs/images/logo-black.png` & `molfeat-0.9.0/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/images/logo-black.svg` & `molfeat-0.9.0/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/images/logo-title.svg` & `molfeat-0.9.0/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/images/logo.png` & `molfeat-0.9.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/images/logo.svg` & `molfeat-0.9.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/index.md` & `molfeat-0.9.0/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,48 +3,46 @@
 Molfeat is a hub of molecular featurizers. It supports a wide variety of out-of-the-box molecular featurizers and can be easily extended to include your own custom featurizers.
 
 - 🚀 Fast, with a simple and efficient API.
 - 🔄 Unify pre-trained molecular embeddings and hand-crafted featurizers in a single package.
 - ➕ Easily add your own featurizers through plugins.
 - 📈 Benefit from increased performance through a trouble-free caching system.
 
-
 Visit our website at https://molfeat.datamol.io.
 
-
 ## Installation
 
 ### Installing Molfeat
 
 Use mamba:
 
 ```bash
 mamba install -c conda-forge molfeat
 ```
 
 _**Tips:** You can replace `mamba` by `conda`._
 
 _**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._
 
-
 ### Installing Plugins
 
 The functionality of molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
 ### Optional dependencies
-Not all featurizers in Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them. 
+
+Not all featurizers in Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them.
 
 - To install `dgl`: run `mamba install -c dglteam dgl`
-- To install `dgllife`:  run `mamba install -c conda-forge dgllife`
+- To install `dgllife`: run `mamba install -c conda-forge dgllife`
 - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
 - To install `pyg`: run `mamba install -c conda-forge pytorch_geometric`
 - To install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-pretrained`
 - To install `map4`: see https://github.com/reymond-group/map4
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`.
 
-
 ## How to cite
-Please cite Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667).
+
+Please cite Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667).
```

### Comparing `molfeat-0.8.9/docs/tutorials/add_your_own.ipynb` & `molfeat-0.9.0/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/custom_model_store.ipynb` & `molfeat-0.9.0/docs/tutorials/custom_model_store.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/datacache.ipynb` & `molfeat-0.9.0/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/graphs.ipynb` & `molfeat-0.9.0/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/integrations.ipynb` & `molfeat-0.9.0/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.9.0/docs/tutorials/pyg_integration.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976229636591478%*

 * *Differences: {"'cells'": '{1: {\'source\': [\'## PyG integration\\n\', \'\\n\', \'<div class="admonition tip '*

 * *            'highlight">\\n\', \'    <p class="admonition-title">Community contribution</p>\\n\', '*

 * *            "'    <p>Curious how one would run this tutorial on <a "*

 * *            'href="https://www.graphcore.ai/products/ipu">Graphcore IPUs</a>? See this tutorial '*

 * *            'contributed by <a '*

 * *            'href="https://github.com/s-maddrellmander">@s-maddrellmander</a>:\\n\', \'    <a '*

 * *            'href= […]*

```diff
@@ -17,15 +17,21 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## PyG integration"
+                "## PyG integration\n",
+                "\n",
+                "<div class=\"admonition tip highlight\">\n",
+                "    <p class=\"admonition-title\">Community contribution</p>\n",
+                "    <p>Curious how one would run this tutorial on <a href=\"https://www.graphcore.ai/products/ipu\">Graphcore IPUs</a>? See this tutorial contributed by <a href=\"https://github.com/s-maddrellmander\">@s-maddrellmander</a>:\n",
+                "    <a href=\"https://ipu.dev/lDvDHL\"><img alt=\"Run on Gradient\" src=\"https://camo.githubusercontent.com/c9931a1689c37ab786edd3e1e5f59b9a6f7d097628c4689ce2432563ef884524/68747470733a2f2f6173736574732e706170657273706163652e696f2f696d672f6772616469656e742d62616467652e737667\"></a></p>\n",
+                "</div>\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -244,15 +250,17 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dataset = DTset(df.smiles.values, df.exp.values, featurizer)\n",
                 "generator = torch.Generator().manual_seed(42)\n",
-                "train_dt, test_dt = torch.utils.data.random_split(dataset, [0.8, 0.2], generator=generator)"
+                "train_size = int(0.8 * len(dataset))\n",
+                "test_size = len(dataset) - train_size\n",
+                "train_dt, test_dt = torch.utils.data.random_split(dataset, [train_size, test_size], generator=generator)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
@@ -419,14 +427,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `molfeat-0.8.9/docs/tutorials/save_and_load.ipynb` & `molfeat-0.9.0/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.9.0/docs/tutorials/transformer_finetuning.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977949134199134%*

 * *Differences: {"'cells'": "{1: {'source': ['## HuggingFace Transformer Finetuning\\n', '\\n', '<div "*

 * *            'class="admonition tip highlight">\\n\', \'    <p class="admonition-title">Community '*

 * *            "contribution</p>\\n', '    <p>Curious how one would run this tutorial on <a "*

 * *            'href="https://www.graphcore.ai/products/ipu">Graphcore IPUs</a>? See this tutorial '*

 * *            'contributed by <a '*

 * *            'href="https://github.com/s-maddrellmander">@s-maddrellmander</a>:\\n\', \'    <a '*

 * *        […]*

```diff
@@ -17,15 +17,21 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## HuggingFace Transformer Finetuning"
+                "## HuggingFace Transformer Finetuning\n",
+                "\n",
+                "<div class=\"admonition tip highlight\">\n",
+                "    <p class=\"admonition-title\">Community contribution</p>\n",
+                "    <p>Curious how one would run this tutorial on <a href=\"https://www.graphcore.ai/products/ipu\">Graphcore IPUs</a>? See this tutorial contributed by <a href=\"https://github.com/s-maddrellmander\">@s-maddrellmander</a>:\n",
+                "    <a href=\"https://ipu.dev/yoyy6N\"><img alt=\"Run on Gradient\" src=\"https://camo.githubusercontent.com/c9931a1689c37ab786edd3e1e5f59b9a6f7d097628c4689ce2432563ef884524/68747470733a2f2f6173736574732e706170657273706163652e696f2f696d672f6772616469656e742d62616467652e737667\"></a></p>\n",
+                "</div>"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -286,15 +292,17 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "dataset = DTset(df.smiles.values, df.p_np.values, featurizer)\n",
                 "generator = torch.Generator().manual_seed(42)\n",
-                "train_dt, test_dt = torch.utils.data.random_split(dataset, [0.8, 0.2], generator=generator)"
+                "train_size = int(0.8 * len(dataset))\n",
+                "test_size = len(dataset) - train_size\n",
+                "train_dt, test_dt = torch.utils.data.random_split(dataset, [train_size, test_size], generator=generator)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
@@ -526,14 +534,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `molfeat-0.8.9/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.9.0/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/env.yml` & `molfeat-0.9.0/env.yml`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,23 @@
   # Scientific
   - pandas
   - numpy
   - scipy
   - h5py
   - pyarrow
   - matplotlib
-  - pydantic
+  - pydantic >=2.0.0
 
   # Chemistry
   - datamol >=0.8.0
   - rdkit >=2021.09
   - pmapper
-  - mordred
 
   # ML
-  - pytorch >=1.10.2
+  - pytorch =1.12
   - scikit-learn
   - fcd_torch
 
   # Optional: featurizers
   - dgl
   - dgllife
   - graphormer-pretrained >=0.2.3
@@ -67,15 +66,11 @@
   - mkdocstrings
   - mkdocstrings-python
   - mkdocs-jupyter
   - markdown-include
   - mdx_truly_sane_lists
   - mike >=1.0.0
 
-  # Releasing tools
-  - rever >=0.4.5
-  - conda-smithy
-
   # EN: consider using poetry
   - twine
   - build
   - setuptools-scm
```

### Comparing `molfeat-0.8.9/mkdocs.yml` & `molfeat-0.9.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 remote_branch: "gh-pages"
 use_directory_urls: false
 copyright: Copyright 2020 - 2023 datamol.io
 
 nav:
   - Getting started:
-      - What is molfeat ?: index.md
-      - How to use ?: usage.md
+      - What is molfeat?: index.md
+      - How to use molfeat?: usage.md
       - Why should you care?: benchmark.ipynb
       - License: license.md
 
   - Tutorials:
       - Types of featurizers: tutorials/types_of_featurizers.ipynb
       - Add your own:
           - Create your own featurizers: tutorials/add_your_own.ipynb
@@ -26,17 +26,21 @@
           - Training a GNN with PyG: tutorials/pyg_integration.ipynb
           - Finetuning a pretrained transformer: tutorials/transformer_finetuning.ipynb
       - Save and Load: tutorials/save_and_load.ipynb
       - The Data Cache: tutorials/datacache.ipynb
 
   - Developers:
       - Contributing: developers/contribute.md
-      - Extending Molfeat: developers/create-plugin.md
+      - Extending molfeat: developers/create-plugin.md
       - Registering your Plugin: developers/register-plugin.md
 
+  - Community:
+      - Get involved: community/get_involved.md
+      - Community contributions: community/contributions.md
+
   - API:
       - molfeat.calc: api/molfeat.calc.md
       - molfeat.trans:
           - molfeat.trans.base: api/molfeat.trans.base.md
           - molfeat.trans.fp: api/molfeat.trans.fp.md
           - molfeat.trans.graph: api/molfeat.trans.graph.md
           - molfeat.trans.struct: api/molfeat.trans.struct.md
```

### Comparing `molfeat-0.8.9/molfeat/calc/__init__.py` & `molfeat-0.9.0/molfeat/calc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from .base import SerializableCalculator
-from .base import _CALCULATORS
+from .base import SerializableCalculator, _CALCULATORS
 from .cats import CATS
-from .descriptors import RDKitDescriptors2D
-from .descriptors import RDKitDescriptors3D
-from .descriptors import MordredDescriptors
+from .descriptors import RDKitDescriptors2D, RDKitDescriptors3D
 from .fingerprints import FPCalculator, FP_FUNCS
-from .pharmacophore import Pharmacophore2D
-from .pharmacophore import Pharmacophore3D
+from .pharmacophore import Pharmacophore2D, Pharmacophore3D
+from .shape import ElectroShapeDescriptors, USRDescriptors
 from .skeys import ScaffoldKeyCalculator
-from .shape import USRDescriptors, ElectroShapeDescriptors
 
 
 def get_calculator(name: str, **params):
     """Get molecular calculator based on name
 
     Args:
         name: Name of the featurizer
@@ -31,16 +27,14 @@
     name = name.lower()
     if name in FP_FUNCS.keys():
         featurizer = FPCalculator(name, **params)
     elif name == "desc3d":
         featurizer = RDKitDescriptors3D(**params)
     elif name == "desc2d":
         featurizer = RDKitDescriptors2D(**params)
-    elif name == "mordred":
-        featurizer = MordredDescriptors(**params)
     elif name == "cats":
         featurizer = CATS(**params)
     elif name == "cats2d":
         params["use_3d_distances"] = False
         featurizer = CATS(**params)
     elif name == "cats3d":
         params["use_3d_distances"] = True
```

### Comparing `molfeat-0.8.9/molfeat/calc/_atom_bond_features.py` & `molfeat-0.9.0/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/_map4.py` & `molfeat-0.9.0/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/_mhfp.py` & `molfeat-0.9.0/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/atom.py` & `molfeat-0.9.0/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/base.py` & `molfeat-0.9.0/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/bond.py` & `molfeat-0.9.0/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/cats.py` & `molfeat-0.9.0/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/descriptors.py` & `molfeat-0.9.0/molfeat/calc/descriptors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import copy
-from typing import Union, List, Optional
 from collections import OrderedDict
+from typing import List, Optional, Union
 
 import datamol as dm
 import numpy as np
-
 from loguru import logger
+from rdkit.Chem import (
+    Descriptors,
+    Descriptors3D,
+    FindMolChiralCenters,
+    rdMolDescriptors,
+    rdPartialCharges,
+)
 from rdkit.Chem.QED import properties
-from rdkit.Chem import Descriptors
-from rdkit.Chem import Descriptors3D
-from rdkit.Chem import FindMolChiralCenters
-from rdkit.Chem import rdPartialCharges
-from rdkit.Chem import rdMolDescriptors
 
-from molfeat.utils.commons import requires_conformer
-from molfeat.utils.commons import requires_standardization
-from molfeat.utils.datatype import to_numpy
-from molfeat.utils import requires
 from molfeat.calc.base import SerializableCalculator
-
-if requires.check("mordred"):
-    from mordred import Calculator as MordredCalculator
-    from mordred import descriptors as mordred_descriptors
-
-else:
-    MordredCalculator = requires.mock("mordred")
+from molfeat.utils.commons import requires_conformer, requires_standardization
+from molfeat.utils.datatype import to_numpy
 
 
 def _charge_descriptors_computation(mol: dm.Mol):
     """Recompute properly the RDKIT 2D Descriptors related to charge
 
     Args:
         mol: input molecule for which the charge descriptors should be recomputed
@@ -175,98 +167,14 @@
             vals.append(val)
         vals = to_numpy(vals)
         if self.replace_nan:
             vals = np.nan_to_num(vals)
         return vals
 
 
-class MordredDescriptors(SerializableCalculator):
-    r"""
-    Compute mordred descriptors.
-    The descriptor calculator does not mask errors in featurization and will propagate them.
-
-    !!! note
-        Mordred descriptors can results in undefined or nan behaviour depending on your input molecule.
-        It is recommended that the user handles those nan values himself by either removing the descriptor
-        or imputing the missing values.
-    """
-
-    def __init__(
-        self,
-        ignore_3D: bool = True,
-        replace_nan: bool = False,
-        do_not_standardize: bool = False,
-        **kwargs,
-    ):
-        """Mordred descriptor computation
-
-        Args:
-            ignore_3D (bool, optional): Whether to ignore 3D descriptors or include them
-            replace_nan (bool, optional): Whether to replace nan or infinite values. Defaults to False.
-            do_not_standardize: Whether to force standardize molecules or keep it the same
-
-        """
-        if not requires.check("mordred"):
-            logger.error(
-                "`mordred` is not available, please install it `pip install 'mordred[full]'`"
-            )
-            raise ImportError("Cannot import `mordred`")
-        self.replace_nan = replace_nan
-        self.ignore_3D = ignore_3D
-        self.do_not_standardize = do_not_standardize
-        self._calc = None
-        self._init_calc()
-
-    def _init_calc(self):
-        """Initialize mordred calculator"""
-        self._calc = MordredCalculator(mordred_descriptors, ignore_3D=self.ignore_3D)
-
-    @property
-    def columns(self):
-        """
-        Get the name of all the descriptors of this calculator
-        """
-        return [str(x) for x in self._calc.descriptors]
-
-    def __len__(self):
-        """Return the length of the calculator"""
-        return len(self._calc)
-
-    def __getstate__(self):
-        """Serialize the class for pickling."""
-        state = {}
-        state["ignore_3D"] = self.ignore_3D
-        state["replace_nan"] = self.replace_nan
-        state["do_not_standardize"] = getattr(self, "do_not_standardize", False)
-        return state
-
-    def __setstate__(self, state: dict):
-        """Reload the class from pickling."""
-        self.__dict__.update(state)
-        self._init_calc()
-
-    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
-        r"""
-        Get rdkit basic descriptors for a molecule
-
-        Args:
-            mol: the molecule of interest
-            conformer_id (int, optional): Optional
-
-        Returns:
-            props (np.ndarray): list of computed mordred molecular descriptors
-        """
-        mol = dm.to_mol(mol)
-        vals = self._calc(mol, conformer_id).fill_missing()
-        vals = to_numpy(vals)
-        if self.replace_nan:
-            vals = np.nan_to_num(vals)
-        return vals
-
-
 class RDKitDescriptors3D(SerializableCalculator):
     """
     Compute a list of 3D rdkit descriptors
     """
 
     def __init__(
         self,
@@ -326,24 +234,24 @@
 
     @property
     def columns(self):
         """Get the descriptors columns"""
         return self._columns
 
     @requires_conformer
-    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
+    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1) -> np.ndarray:
         r"""
         Get rdkit 3D descriptors for a molecule
 
         Args:
             mol: the molecule of interest
-            conformer_id (int, optional): Optional conformer id. Defaults to -1.
+            conformer_id: Optional conformer id. Defaults to -1.
 
         Returns:
-            props (np.ndarray): list of computed mordred molecular descriptors
+            props: list of computed molecular descriptors
         """
 
         mol = dm.to_mol(mol)
         desc_val = []
         for desc in self._descr:
             val = float("nan")
             if desc not in self.ignore_descrs:
```

### Comparing `molfeat-0.8.9/molfeat/calc/fingerprints.py` & `molfeat-0.9.0/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/pharmacophore.py` & `molfeat-0.9.0/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/shape.py` & `molfeat-0.9.0/molfeat/calc/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
 import datamol as dm
 import numpy as np
-
-from loguru import logger
 from numpy.linalg import norm
+from rdkit.Chem import rdForceFieldHelpers, rdMolDescriptors, rdPartialCharges
 from scipy.special import cbrt
-from rdkit.Chem import rdPartialCharges, rdForceFieldHelpers
-from rdkit.Chem import rdMolDescriptors
+
 from molfeat.calc.base import SerializableCalculator
 from molfeat.utils.commons import requires_conformer
 
 
 class USRDescriptors(SerializableCalculator):
     """Descriptors for the shape of a molecule.
 
@@ -54,24 +52,24 @@
         return self._columns
 
     def __len__(self):
         """Compute descriptors length"""
         return len(self.columns)
 
     @requires_conformer
-    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
+    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1) -> np.ndarray:
         r"""
         Get rdkit 3D descriptors for a molecule
 
         Args:
             mol: the molecule of interest
-            conformer_id (int, optional): Optional conformer id. Defaults to -1.
+            conformer_id: Optional conformer id. Defaults to -1.
 
         Returns:
-            shape_descriptors (np.ndarray): list of computed mordred molecular descriptors
+            shape_descriptors: list of computed molecular descriptors
         """
         if self.method == "USR":
             shape_descr = rdMolDescriptors.GetUSR(mol, confId=conformer_id)
         elif self.method == "USRCAT":
             shape_descr = rdMolDescriptors.GetUSRCAT(mol, confId=conformer_id)
         if self.replace_nan:
             shape_descr = np.nan_to_num(shape_descr, self.replace_nan)
```

### Comparing `molfeat-0.8.9/molfeat/calc/skeys.py` & `molfeat-0.9.0/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/calc/tree.py` & `molfeat-0.9.0/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/data/cats_features.fdef` & `molfeat-0.9.0/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/data/elements.xz` & `molfeat-0.9.0/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/data/elements_completed.xz` & `molfeat-0.9.0/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/data/origin.xz` & `molfeat-0.9.0/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/data/skey_parameters.csv` & `molfeat-0.9.0/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/plugins/entry_point.py` & `molfeat-0.9.0/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/plugins/factories.py` & `molfeat-0.9.0/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/store/loader.py` & `molfeat-0.9.0/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/store/modelcard.py` & `molfeat-0.9.0/molfeat/store/modelcard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from typing import Optional
-from typing import List
-from typing import Union
-
 from datetime import datetime
-from pydantic.typing import Literal
-from pydantic import BaseModel
-from pydantic import Field
+from typing import List, Literal, Optional, Union
+
 import datamol as dm
+from pydantic import BaseModel, ConfigDict, Field
 
 
 def get_model_init(card):
     """Get the model initialization code
 
     Args:
         card: model card to use
@@ -49,29 +45,35 @@
         )
     else:
         raise ValueError(f"Unknown model group {card.group}")
     return import_statement, loader_statement
 
 
 class ModelInfo(BaseModel):
+    model_config = ConfigDict(
+        protected_namespaces=(
+            "protected_",
+        )  # Prevents warning from usage of model_ prefix in fields
+    )
+
     name: str
     inputs: str = "smiles"
     type: Literal["pretrained", "hand-crafted", "hashed", "count"]
     version: int = 0
     group: Optional[str] = "all"
     submitter: str
     description: str
     representation: Literal["graph", "line-notation", "vector", "tensor", "other"]
     require_3D: Optional[bool] = False
-    tags: Optional[List[str]]
+    tags: Optional[List[str]] = []
     authors: Optional[List[str]]
-    reference: Optional[str]
+    reference: Optional[str] = None
     created_at: datetime = Field(default_factory=datetime.now)
-    sha256sum: Optional[str]
-    model_usage: Optional[str]
+    sha256sum: Optional[str] = None
+    model_usage: Optional[str] = None
 
     def path(self, root_path: str):
         """Generate the folder path where to save this model
 
         Args:
             root_path: path to the root folder
         """
@@ -82,17 +84,17 @@
         """Compare two model card information and returns True if they are the same
 
         Args:
             new_card: card to search for in the modelstore
             match_only: list of minimum attribute that should match between the two model information
         """
 
-        self_content = self.dict().copy()
+        self_content = self.model_dump().copy()
         if not isinstance(new_card, dict):
-            new_card = new_card.dict()
+            new_card = new_card.model_dump()
         new_content = new_card.copy()
         # we always remove the datetime field
         self_content.pop("created_at", None)
         new_content.pop("created_at", None)
         if match_only is not None:
             self_content = {k: self_content.get(k) for k in match_only}
             new_content = {k: new_content.get(k) for k in match_only}
```

### Comparing `molfeat-0.8.9/molfeat/store/modelstore.py` & `molfeat-0.9.0/molfeat/store/modelstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from typing import Optional
-from typing import Any
-from typing import Union
-from typing import Callable
-
-import yaml
-import joblib
-import pathlib
 import os
-import fsspec
+import pathlib
 import tempfile
-import platformdirs
-import filelock
+from typing import Any, Callable, Optional, Union
+
 import datamol as dm
+import filelock
+import fsspec
+import joblib
+import platformdirs
+import yaml
 from dotenv import load_dotenv
 from loguru import logger
 
 from molfeat.store.modelcard import ModelInfo
 from molfeat.utils import commons
 
-
 load_dotenv()
 
 
 class ModelStoreError(Exception):
     pass
```

### Comparing `molfeat-0.8.9/molfeat/trans/base.py` & `molfeat-0.9.0/molfeat/trans/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Mapping
 from typing import Union
 from typing import List
 from typing import Any
 from typing import Callable
 from typing import Optional
 from typing import Dict
@@ -571,19 +572,19 @@
 
     def to_state_json(self) -> str:
         return json.dumps(self.to_state_dict())
 
     def to_state_yaml(self) -> str:
         return yaml.dump(self.to_state_dict(), Dumper=yaml.SafeDumper)
 
-    def to_state_json_file(self, filepath: str):
+    def to_state_json_file(self, filepath: Union[str, Path]):
         with fsspec.open(filepath, "w") as f:
             f.write(self.to_state_json())  # type: ignore
 
-    def to_state_yaml_file(self, filepath: str):
+    def to_state_yaml_file(self, filepath: Union[str, Path]):
         with fsspec.open(filepath, "w") as f:
             f.write(self.to_state_yaml())  # type: ignore
 
     # State to featurizer methods
 
     @staticmethod
     def from_state_dict(state: dict, override_args: Optional[dict] = None) -> "MoleculeTransformer":
@@ -670,24 +671,24 @@
         override_args: Optional[dict] = None,
     ) -> "MoleculeTransformer":
         state_dict = yaml.load(state_yaml, Loader=yaml.SafeLoader)
         return MoleculeTransformer.from_state_dict(state_dict, override_args=override_args)
 
     @staticmethod
     def from_state_json_file(
-        filepath: str,
+        filepath: Union[str, Path],
         override_args: Optional[dict] = None,
     ) -> "MoleculeTransformer":
         with fsspec.open(filepath, "r") as f:
             featurizer = MoleculeTransformer.from_state_json(f.read(), override_args=override_args)  # type: ignore
         return featurizer
 
     @staticmethod
     def from_state_yaml_file(
-        filepath: str,
+        filepath: Union[str, Path],
         override_args: Optional[dict] = None,
     ) -> "MoleculeTransformer":
         with fsspec.open(filepath, "r") as f:
             featurizer = MoleculeTransformer.from_state_yaml(f.read(), override_args=override_args)  # type: ignore
         return featurizer
```

### Comparing `molfeat-0.8.9/molfeat/trans/concat.py` & `molfeat-0.9.0/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/fp.py` & `molfeat-0.9.0/molfeat/trans/fp.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         For counting fingerprints, you just need to add the '-count' suffix to the name of the fingerprint. For example:
         "morgan-count:2"
     """
 
     AVAILABLE_FPS = list(FP_FUNCS.keys()) + [
         "desc3D",
         "desc2D",
-        "mordred",
         "cats2D",
         "cats3D",
         "pharm2D",
         "pharm3D",
         "scaffoldkeys",
         "skeys",
         "electroshape",
```

### Comparing `molfeat-0.8.9/molfeat/trans/graph/adj.py` & `molfeat-0.9.0/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/graph/tree.py` & `molfeat-0.9.0/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/pretrained/base.py` & `molfeat-0.9.0/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.9.0/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/pretrained/fcd.py` & `molfeat-0.9.0/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.9.0/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.9.0/molfeat/trans/pretrained/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/struct/esm.py` & `molfeat-0.9.0/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/trans/struct/prot1D.py` & `molfeat-0.9.0/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/cache.py` & `molfeat-0.9.0/molfeat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/commons.py` & `molfeat-0.9.0/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/const.py` & `molfeat-0.9.0/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/converters.py` & `molfeat-0.9.0/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/datatype.py` & `molfeat-0.9.0/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/log.py` & `molfeat-0.9.0/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/parsing.py` & `molfeat-0.9.0/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/pooler.py` & `molfeat-0.9.0/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/requires.py` & `molfeat-0.9.0/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/utils/state.py` & `molfeat-0.9.0/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat/viz.py` & `molfeat-0.9.0/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/molfeat.egg-info/PKG-INFO` & `molfeat-0.9.0/molfeat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.9
+Version: 0.9.0
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -143,19 +143,17 @@
 
 ## How to cite
 
 Please cite Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/latestdoi/613548667).
 
 ## Contribute
 
-See [developers](docs/developers/) for a comprehensive guide on how to contribute to `Molfeat`
-
-## Changelogs
-
-See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
+See [developers](docs/developers/) for a comprehensive guide on how to contribute to `molfeat`. `molfeat` is a community-led
+initiative and whether you're a first-time contributor or an open-source veteran, this project greatly benefits from your contributions.
+To learn more about the community and [datamol.io](https://datamol.io/) ecosystem, please see [community](docs/community/).
 
 ## Maintainers
 
 - @cwognum
 - @maclandrol
 - @hadim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.9 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.0 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -92,10 +92,13 @@
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
-contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
-@hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
+contribute to `molfeat`. `molfeat` is a community-led initiative and whether
+you're a first-time contributor or an open-source veteran, this project greatly
+benefits from your contributions. To learn more about the community and
+[datamol.io](https://datamol.io/) ecosystem, please see [community](docs/
+community/). ## Maintainers - @cwognum - @maclandrol - @hadim ## License Under
+the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.9/molfeat.egg-info/SOURCES.txt` & `molfeat-0.9.0/molfeat.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-.authors.yml
 .gitignore
-.mailmap
-AUTHORS.rst
-CHANGELOG.rst
+CHANGELOG.md
 LICENSE
 README.md
 env.yml
 mkdocs.yml
 plugin.yml
 pyproject.toml
-rever.xsh
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/SECURITY.md
 .github/ISSUE_TEMPLATE/1_bug_report.yaml
 .github/ISSUE_TEMPLATE/2_refactor.yaml
 .github/ISSUE_TEMPLATE/3_documentation.yaml
 .github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+.github/ISSUE_TEMPLATE/5_community_contribution.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/workflows/code-check.yml
 .github/workflows/doc.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 docs/benchmark.ipynb
 docs/index.md
@@ -41,14 +38,16 @@
 docs/api/molfeat.trans.struct.md
 docs/api/molfeat.utils.md
 docs/api/molfeat.viz.md
 docs/assets/css/custom-molfeat.css
 docs/assets/css/custom.css
 docs/assets/css/tweak-width.css
 docs/assets/js/google-analytics.js
+docs/community/contributions.md
+docs/community/get_involved.md
 docs/developers/contribute.md
 docs/developers/create-plugin.md
 docs/developers/register-plugin.md
 docs/images/logo-black.png
 docs/images/logo-black.svg
 docs/images/logo-title.svg
 docs/images/logo.png
@@ -128,15 +127,14 @@
 molfeat/utils/state.py
 nb/etl/chemberta-etl.ipynb
 nb/etl/chemgpt-fix-etl.ipynb
 nb/etl/dgl-etl.ipynb
 nb/etl/entropy-transforner-zinc-etl.ipynb
 nb/etl/featurizer-etl.ipynb
 nb/etl/molt5-etl.ipynb
-news/TEMPLATE.rst
 tests/test_atom_bond_calculator.py
 tests/test_descriptors.py
 tests/test_fp.py
 tests/test_graphs.py
 tests/test_pharmacophore.py
 tests/test_pretrained.py
 tests/test_prot_embed.py
```

### Comparing `molfeat-0.8.9/nb/etl/chemberta-etl.ipynb` & `molfeat-0.9.0/nb/etl/chemberta-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/nb/etl/chemgpt-fix-etl.ipynb` & `molfeat-0.9.0/nb/etl/chemgpt-fix-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/nb/etl/dgl-etl.ipynb` & `molfeat-0.9.0/nb/etl/dgl-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/nb/etl/entropy-transforner-zinc-etl.ipynb` & `molfeat-0.9.0/nb/etl/entropy-transforner-zinc-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/nb/etl/featurizer-etl.ipynb` & `molfeat-0.9.0/nb/etl/featurizer-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/nb/etl/molt5-etl.ipynb` & `molfeat-0.9.0/nb/etl/molt5-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/pyproject.toml` & `molfeat-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     "h5py",
     "pyarrow",
     "pydantic",
     "platformdirs",
     "scikit-learn",
     "packaging",
     "pmapper",
-    "mordred",
 
 ]
 
 [project.optional-dependencies]
 dgl = [
     "dgl",
     "dgllife",
@@ -122,14 +121,13 @@
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose --cov-report xml --cov-report term --color yes"
 testpaths = ["tests"]
 norecursedirs = "tests/helpers"
-filterwarnings = ["ignore::DeprecationWarning:mordred.*:"]
 
 [tool.coverage.run]
 omit = ["setup.py", "tests/*"]
 
 [tool.coverage.xml]
 output = "cov.xml"
```

### Comparing `molfeat-0.8.9/tests/test_atom_bond_calculator.py` & `molfeat-0.9.0/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/tests/test_descriptors.py` & `molfeat-0.9.0/tests/test_descriptors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-import unittest as ut
-import pytest
-
 import tempfile
-
-import joblib
+import unittest as ut
 
 import datamol as dm
+import joblib
 import numpy as np
+import pytest
 
-from molfeat.calc import CATS
-from molfeat.calc import ScaffoldKeyCalculator
-from molfeat.calc import RDKitDescriptors2D
-from molfeat.calc import RDKitDescriptors3D
-from molfeat.calc import MordredDescriptors
-from molfeat.calc import USRDescriptors
-from molfeat.calc import ElectroShapeDescriptors
+from molfeat.calc import (
+    CATS,
+    ElectroShapeDescriptors,
+    RDKitDescriptors2D,
+    RDKitDescriptors3D,
+    ScaffoldKeyCalculator,
+    USRDescriptors,
+)
 from molfeat.calc.skeys import skdistance
-from molfeat.utils import requires
 
 
 class TestDescPharm(ut.TestCase):
     r"""Test cases for descriptors and pharmacophore generation"""
     smiles = [
         "CCOc1c(OC)cc(CCN)cc1OC",
         "COc1cc(CCN)cc(OC)c1OC",
@@ -58,20 +56,14 @@
 
     def test_rdkit3d(self):
         calc = RDKitDescriptors3D()
         mol = dm.conformers.generate(dm.to_mol(self.smiles[0]))
         fps = calc(mol)
         self.assertEqual(len(fps), len(calc))
 
-    @pytest.mark.xfail(not requires.check("mordred"), reason="3rd party module mordred is missing")
-    def test_mordred(self):
-        calc = MordredDescriptors()
-        fps = calc(self.smiles[0])
-        self.assertEqual(len(fps), len(calc))
-
     def test_cats_2d(self):
         smiles = "Nc1cnn(-c2ccccc2)c(=O)c1Cl"
         mol = dm.to_mol(smiles)
 
         calc = CATS(max_dist=5, scale="raw", use_3d_distances=False)
         assert calc(mol).shape == (126,)
```

### Comparing `molfeat-0.8.9/tests/test_fp.py` & `molfeat-0.9.0/tests/test_fp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import time
 import os
 import shutil
+import tempfile
+import time
 import unittest as ut
-import torch
+
 import datamol as dm
-import pandas as pd
-import numpy as np
-import tempfile
 import joblib
-
+import numpy as np
+import pandas as pd
+import torch
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect
-from molfeat.calc import SerializableCalculator
-from molfeat.calc.descriptors import MordredDescriptors
+
+from molfeat.calc import RDKitDescriptors2D, SerializableCalculator
 from molfeat.calc.fingerprints import FPCalculator
 from molfeat.calc.pharmacophore import Pharmacophore2D
 from molfeat.trans import MoleculeTransformer
 from molfeat.trans.base import PrecomputedMolTransformer
-from molfeat.trans.fp import FPVecTransformer
-from molfeat.trans.fp import FPVecFilteredTransformer
 from molfeat.trans.concat import FeatConcat
+from molfeat.trans.fp import FPVecFilteredTransformer, FPVecTransformer
 from molfeat.utils.cache import DataCache, FileCache, MPDataCache
 
 
 class CustomBatchCalculator(SerializableCalculator):
     def __init__(self, random_seed: int = 42, length: int = 10):
         self.random_seed = random_seed
         self.length = length
@@ -227,21 +226,20 @@
         concat_transf2 = FeatConcat(transf, dtype=np.float32, params=dict(rdkit=dict(length=2000)))
         concat_transf1.fit(self.smiles)
         concat_transf2.fit(self.smiles)
         out1, ids = concat_transf1(self.smiles, enforce_dtype=True, ignore_errors=True)
         out2, ids = concat_transf1(self.smiles, enforce_dtype=True, ignore_errors=True)
         np.testing.assert_allclose(out1, out2)
 
-    # @pytest.mark.xfail
     def test_caching(self):
-        ## check performance when cache is added from existing cache
+        # check performance when cache is added from existing cache
         smiles = dm.data.freesolv().smiles.values[:50]
-        desc = MordredDescriptors(replace_nan=False, ignore_3D=True)
+        desc = RDKitDescriptors2D(replace_nan=False, ignore_3D=True)
         transff = MoleculeTransformer(desc, verbose=True)
-        cache = DataCache(name="mordred")
+        cache = DataCache(name="rdkit2d")
 
         t1 = time.time()
         out1 = transff(smiles)
         elapsed1 = time.time() - t1
         # let's cache only a part of the dataset
         cache(smiles[: len(smiles) // 2], transff)
 
@@ -260,15 +258,15 @@
         # should be even faster now that the full dataset is cached
         t3 = time.time()
         out3 = precomp(smiles)
         elapsed3 = time.time() - t3
         self.assertTrue(elapsed3 <= elapsed1 or elapsed1 < 1.5)
         np.testing.assert_array_equal(out1, out3)
 
-        ## check when cache is build on the fly from a
+        # check when cache is build on the fly from a
         transff = MoleculeTransformer("desc2d")
         cache = DataCache(name="desc2d_transformer1")
         t1 = time.time()
         out1 = cache(smiles, transff)
         precomp = PrecomputedMolTransformer(cache=cache, featurizer=transff)
         elapsed1 = time.time() - t1
         out2 = precomp.transform(smiles)
@@ -276,15 +274,15 @@
         out3 = precomp.transform(smiles)
         elapsed3 = time.time() - t1 - elapsed1 - elapsed2
         self.assertTrue(elapsed3 <= elapsed2 or elapsed2 < 1.5)
         self.assertTrue(elapsed3 <= elapsed1 or elapsed2 < 1.5)
         np.testing.assert_array_equal(out1, out2)
         np.testing.assert_array_equal(out1, out3)
 
-        ## check when cache is build on the fly while the transformer name is not defined
+        # check when cache is build on the fly while the transformer name is not defined
         cache = DataCache(name="desc2d_transformer2")
         t1 = time.time()
         out1 = cache(smiles, transff)
         precomp = PrecomputedMolTransformer(cache=cache, featurizer="desc2d")
         elapsed1 = time.time() - t1
         out2 = precomp.transform(smiles)
         elapsed2 = time.time() - t1 - elapsed1
```

### Comparing `molfeat-0.8.9/tests/test_graphs.py` & `molfeat-0.9.0/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/tests/test_pharmacophore.py` & `molfeat-0.9.0/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/tests/test_pretrained.py` & `molfeat-0.9.0/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/tests/test_prot_embed.py` & `molfeat-0.9.0/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.9/tests/test_state.py` & `molfeat-0.9.0/tests/test_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-import pytest
-
-import numpy as np
 import datamol as dm
+import numpy as np
+import pytest
 
 from molfeat._version import __version__ as MOLFEAT_VERSION
-from molfeat.trans.fp import FPVecTransformer
-from molfeat.trans.fp import FPVecFilteredTransformer
-from molfeat.trans.base import MoleculeTransformer
-from molfeat.trans.base import PrecomputedMolTransformer
-from molfeat.trans.graph import AdjGraphTransformer
-from molfeat.trans.graph import DGLGraphTransformer
-from molfeat.trans.graph import TopoDistGraphTransformer
-from molfeat.trans.graph import PYGGraphTransformer
-from molfeat.trans.pretrained import PretrainedDGLTransformer
-from molfeat.trans.pretrained import GraphormerTransformer
-from molfeat.trans.pretrained import PretrainedHFTransformer
-
-from molfeat.calc.atom import AtomCalculator
+from molfeat.calc import (
+    CATS,
+    FPCalculator,
+    Pharmacophore2D,
+    RDKitDescriptors2D,
+    ScaffoldKeyCalculator,
+)
+from molfeat.calc._atom_bond_features import atom_chiral_tag_one_hot, atom_one_hot
+from molfeat.calc.atom import AtomCalculator, AtomMaterialCalculator
 from molfeat.calc.bond import BondCalculator
-from molfeat.calc.atom import AtomMaterialCalculator
-from molfeat.calc import FPCalculator
-from molfeat.calc import ScaffoldKeyCalculator
-from molfeat.calc import RDKitDescriptors2D
-from molfeat.calc import CATS
-from molfeat.calc import Pharmacophore2D
-from molfeat.calc._atom_bond_features import atom_chiral_tag_one_hot
-from molfeat.calc._atom_bond_features import atom_one_hot
-from molfeat.trans.graph import MolTreeDecompositionTransformer
-
-from molfeat.utils.cache import MolToKey
-from molfeat.utils.cache import FileCache
+from molfeat.trans.base import MoleculeTransformer, PrecomputedMolTransformer
+from molfeat.trans.fp import FPVecFilteredTransformer, FPVecTransformer
+from molfeat.trans.graph import (
+    AdjGraphTransformer,
+    DGLGraphTransformer,
+    MolTreeDecompositionTransformer,
+    PYGGraphTransformer,
+    TopoDistGraphTransformer,
+)
+from molfeat.trans.pretrained import (
+    GraphormerTransformer,
+    PretrainedDGLTransformer,
+    PretrainedHFTransformer,
+)
+from molfeat.utils.cache import FileCache, MolToKey
 from molfeat.utils.state import compare_state
 
 
 def _dummy_featurizer_fn(x):
     return np.random.random(1024)
```

### Comparing `molfeat-0.8.9/tests/test_utils.py` & `molfeat-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

