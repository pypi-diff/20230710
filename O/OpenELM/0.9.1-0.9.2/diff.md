# Comparing `tmp/OpenELM-0.9.1.tar.gz` & `tmp/OpenELM-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenELM-0.9.1.tar", last modified: Mon Jul 10 19:36:48 2023, max compression
+gzip compressed data, was "OpenELM-0.9.2.tar", last modified: Mon Jul 10 21:07:59 2023, max compression
```

## Comparing `OpenELM-0.9.1.tar` & `OpenELM-0.9.2.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      834 2023-01-20 14:24:40.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      595 2023-01-20 14:24:40.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/workflows/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.github/workflows/build.yml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1919 2023-03-08 01:31:49.000000 OpenELM-0.9.1/.gitignore
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1162 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      686 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.readthedocs.yml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      840 2023-02-17 21:08:09.000000 OpenELM-0.9.1/CITATION.cff
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5220 2023-01-20 14:24:40.000000 OpenELM-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3812 2023-01-20 14:24:40.000000 OpenELM-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1065 2023-01-20 14:24:40.000000 OpenELM-0.9.1/LICENSE
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1872346 2023-07-10 19:30:39.000000 OpenELM-0.9.1/OpenELM_Paper.pdf
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5792 2023-07-10 19:36:48.000000 OpenELM-0.9.1/PKG-INFO
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4723 2023-07-10 19:30:39.000000 OpenELM-0.9.1/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      638 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/Makefile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      804 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/make.bat
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/source/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2814 2023-02-17 21:08:09.000000 OpenELM-0.9.1/docs/source/conf.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/source/images/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1150 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/images/openelm_favicon.ico
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      448 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/index.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      267 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/openelm.environments.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      657 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/openelm.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2115 2023-07-10 19:34:59.000000 OpenELM-0.9.1/pyproject.toml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      203 2023-07-10 19:30:39.000000 OpenELM-0.9.1/requirements.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      994 2023-07-10 19:30:39.000000 OpenELM-0.9.1/run_elm.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6298 2023-07-10 19:30:39.000000 OpenELM-0.9.1/run_p3.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       38 2023-07-10 19:36:48.000000 OpenELM-0.9.1/setup.cfg
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/OpenELM.egg-info/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5792 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/PKG-INFO
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15032 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/SOURCES.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        1 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/dependency_links.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/requires.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        8 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/top_level.txt
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      152 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/algorithms/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6037 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/genetic.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33376 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/map_elites.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/benchmarks/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8971 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_bugs.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9429 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_crossover.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1538 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_lm_speed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1552 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12530 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_tinygp.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2590 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmarks_triton.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/codegen/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      147 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6269 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/codegen_triton.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4265 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/codegen/codegen_utilities.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2726 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/codegen/configuration_codegen.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28547 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/codegen/modelling_codegen.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3404 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3705 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/config_template.pbtxt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4127 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/convert_ft.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7460 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/readme.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      270 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/triton_start.sh
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6925 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/configs.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      166 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/constants.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3784 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/elm.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      118 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12516 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/base.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/p3/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6966 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/p3/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    24594 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/p3/p3.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6171 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/poetry.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      534 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      471 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/active_to_passive.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      528 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/antonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      698 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/cause_and_effect.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      458 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/common_concept.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      805 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/diff.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/first_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      348 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/informal_to_formal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      475 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/larger_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      696 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/letters_list.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/negation.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      565 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/num_to_verbal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      819 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/orthography_starts_with.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      470 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/rhymes.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      365 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/second_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      932 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentence_similarity.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      706 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentiment.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      437 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/singular_to_plural.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sum.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      487 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/synonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      421 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/taxonomy_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      283 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-de.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-es.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      207 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-fr.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1523 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/word_in_context.json
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   108445 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/addsub.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    51855 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/aqua.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   230302 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/coin_flip.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   385739 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/commonsensqa.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103317 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/date_understanding.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   296065 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/gsm8k.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    86001 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/last_letters.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   200307 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/multiarith.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   368446 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/shuffled_objects.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   154726 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/singleeq.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   456229 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/strategyqa.csv
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   275766 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/svamp.csv
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   124409 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/active_to_passive.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    65651 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/antonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   159273 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/cause_and_effect.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103263 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/common_concept.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/diff.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/first_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   113139 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/informal_to_formal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    72257 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/larger_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    69787 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/letters_list.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   136337 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/negation.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    90713 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/num_to_verbal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   102849 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/orthography_starts_with.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    59593 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/rhymes.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/second_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   168475 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentence_similarity.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    99119 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentiment.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63269 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/singular_to_plural.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sum.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    61715 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/synonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   116251 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/taxonomy_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    64271 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-de.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-es.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63877 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-fr.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158299 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/word_in_context.json
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16216 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/active_to_passive.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7440 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/antonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2867 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/cause_and_effect.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3553 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/common_concept.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9496 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/diff.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/first_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1777 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/informal_to_formal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13878 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/larger_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    20496 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/letters_list.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    19956 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/negation.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9973 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/num_to_verbal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28548 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/orthography_starts_with.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26905 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/rhymes.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/second_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16857 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentence_similarity.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11210 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentiment.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9832 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/singular_to_plural.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9450 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sum.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7007 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/synonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    48523 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/taxonomy_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18183 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-de.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17017 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-es.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16752 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-fr.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26219 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/word_in_context.json
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   145630 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/active_to_passive.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   196170 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/antonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3009 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/cause_and_effect.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3944 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/common_concept.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   477101 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/diff.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/first_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1891 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/informal_to_formal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   407339 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/larger_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   693976 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/letters_list.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   176741 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/negation.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1000548 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/num_to_verbal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   808766 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/orthography_starts_with.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1150469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/rhymes.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/second_word_letter.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   663715 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentence_similarity.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   127802 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentiment.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   194002 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/singular_to_plural.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   474622 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sum.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158942 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/synonyms.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1450171 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/taxonomy_animal.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   513349 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-de.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   459674 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-es.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   471938 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-fr.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1044414 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/word_in_context.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15671 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/prompt.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4494 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/utils.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1408 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/README.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6795 2023-07-06 23:17:33.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5450 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_draw.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11741 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_framework.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16357 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_framework.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3759 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_gui.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    22633 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyglet_framework.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33046 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_framework.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5189 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3094 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.ui
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6770 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/simple_framework.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18390 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/framework.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      103 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9332 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/app.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15634 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/area.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4327 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/basic.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9967 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/button.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      667 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/const.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/container.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2375 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/deprecated.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5042 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/dialog.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2620 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/document.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2630 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/form.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1127 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/group.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4684 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/input.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1840 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/keysym.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4901 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/layout.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3332 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/menus.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1049 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/misc.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      360 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/pguglobals.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       99 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/readme.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4602 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/select.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11132 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/slider.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      991 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/style.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4488 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/surface.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12923 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/table.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11458 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/textarea.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16553 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/theme.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11434 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/widget.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4196 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/settings.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      722 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/environment_sandbox.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3346 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/helpers.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    25878 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/simulator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10542 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/sodarace.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_fixed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1267 2023-02-03 22:41:04.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1099 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/README.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      214 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1322 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/galloper.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      923 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/radial.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      541 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/runner.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      957 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/square.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3401 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/walk_creator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      973 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/wheel.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      628 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/utils.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9163 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/mutation_model.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      406 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/Dockerfile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      162 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/Pipfile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9266 2023-02-04 21:59:34.000000 OpenELM-0.9.1/src/openelm/sandbox/Pipfile.lock
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      931 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/sandbox/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       85 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/bootstrap.sh
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       33 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/build.sh
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)      107 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/launch.sh
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/server/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      496 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_fixed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1230 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       71 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      881 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/radial.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      933 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/square.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2975 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/walk_creator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3625 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/sandbox/server/index.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10138 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/sandbox/server/sandbox_codex_execute.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/templates/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/server/templates/index.html
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/utils/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      338 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/utils/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6293 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/utils/code_eval.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13343 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/utils/diff_eval.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      907 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/utils/utils.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/tests/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1018 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/conftest.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1762 2023-03-08 01:31:49.000000 OpenELM-0.9.1/tests/test_code_execute.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/tests/test_data/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17990 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_data/cppn_fixed.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2532 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_data/square.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18081 2023-02-17 21:08:10.000000 OpenELM-0.9.1/tests/test_diff.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8668 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_mapelites.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4628 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_sodarace_env.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2602 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_sodarace_walkers.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      736 2023-02-17 21:08:10.000000 OpenELM-0.9.1/tests/test_truncate.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/configs/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2152 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/configs/ppo_softprompt_config.yml
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/model/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12827 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/model/accelerate_ppo_softprompt_model.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/orchestrator/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6254 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1743 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_long_completions.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1600 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_sentiment.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1769 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_short_completions.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/.github/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      834 2023-01-20 14:24:40.000000 OpenELM-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      595 2023-01-20 14:24:40.000000 OpenELM-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/.github/workflows/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-02-17 21:08:09.000000 OpenELM-0.9.2/.github/workflows/build.yml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1919 2023-03-08 01:31:49.000000 OpenELM-0.9.2/.gitignore
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1162 2023-02-17 21:08:09.000000 OpenELM-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      686 2023-02-17 21:08:09.000000 OpenELM-0.9.2/.readthedocs.yml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      840 2023-02-17 21:08:09.000000 OpenELM-0.9.2/CITATION.cff
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5220 2023-01-20 14:24:40.000000 OpenELM-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3812 2023-01-20 14:24:40.000000 OpenELM-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1065 2023-01-20 14:24:40.000000 OpenELM-0.9.2/LICENSE
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1872346 2023-07-10 19:30:39.000000 OpenELM-0.9.2/OpenELM_Paper.pdf
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5955 2023-07-10 21:07:59.000000 OpenELM-0.9.2/PKG-INFO
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4886 2023-07-10 21:05:59.000000 OpenELM-0.9.2/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/docs/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      638 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/Makefile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      804 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/make.bat
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/docs/source/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2814 2023-02-17 21:08:09.000000 OpenELM-0.9.2/docs/source/conf.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/docs/source/images/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1150 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/source/images/openelm_favicon.ico
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      448 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/source/index.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      267 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/source/openelm.environments.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      657 2023-01-20 14:24:40.000000 OpenELM-0.9.2/docs/source/openelm.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2163 2023-07-10 20:57:19.000000 OpenELM-0.9.2/pyproject.toml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      175 2023-07-10 20:57:23.000000 OpenELM-0.9.2/requirements.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      994 2023-07-10 19:30:39.000000 OpenELM-0.9.2/run_elm.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6298 2023-07-10 19:30:39.000000 OpenELM-0.9.2/run_p3.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       38 2023-07-10 21:07:59.000000 OpenELM-0.9.2/setup.cfg
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5955 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/PKG-INFO
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15032 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/SOURCES.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        1 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/dependency_links.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/requires.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        8 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/OpenELM.egg-info/top_level.txt
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      152 2023-03-08 01:31:49.000000 OpenELM-0.9.2/src/openelm/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/algorithms/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/algorithms/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6037 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/algorithms/genetic.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33376 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/algorithms/map_elites.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/benchmarks/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/benchmarks/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8971 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmark_bugs.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9429 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmark_crossover.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1538 2023-03-08 01:31:49.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmark_lm_speed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1552 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmark_sodarace_parallel.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12530 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmark_tinygp.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2590 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/benchmarks/benchmarks_triton.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/codegen/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      147 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6269 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/codegen_triton.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4265 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/codegen/codegen_utilities.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2726 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/codegen/configuration_codegen.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28547 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/codegen/modelling_codegen.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3404 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/codegen_gptj_converter.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3705 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/config_template.pbtxt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4127 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/convert_ft.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7460 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/gptj_ftconverter.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/readme.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      270 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/codegen/triton_utils/triton_start.sh
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6925 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/configs.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      166 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/constants.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3784 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/elm.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      118 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12516 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/base.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/p3/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6966 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/p3/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    24594 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/p3/p3.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6171 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/poetry.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      534 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      471 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      528 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      698 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      458 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      805 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      469 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      348 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      475 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      696 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      565 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      819 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      470 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      365 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      932 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      706 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      437 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      487 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      421 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      283 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      207 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1523 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   108445 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/addsub.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    51855 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/aqua.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   230302 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/coin_flip.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   385739 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/commonsensqa.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103317 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/date_understanding.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   296065 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/gsm8k.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    86001 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/last_letters.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   200307 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/multiarith.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   368446 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/shuffled_objects.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   154726 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/singleeq.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   456229 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/strategyqa.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   275766 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/svamp.csv
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   124409 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    65651 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   159273 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103263 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   113139 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    72257 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    69787 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   136337 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    90713 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   102849 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    59593 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   168475 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    99119 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63269 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    61715 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   116251 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    64271 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63469 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63877 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158299 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16216 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7440 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2867 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3553 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9496 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1777 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13878 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    20496 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    19956 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9973 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28548 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26905 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16857 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11210 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9832 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9450 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7007 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    48523 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18183 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17017 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16752 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26219 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   145630 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   196170 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3009 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3944 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   477101 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1891 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   407339 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   693976 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   176741 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1000548 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   808766 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1150469 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   663715 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   127802 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   194002 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   474622 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158942 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1450171 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   513349 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   459674 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   471938 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1044414 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/word_in_context.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15671 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/prompt.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4494 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/prompt/utils.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1408 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/README.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6795 2023-07-06 23:17:33.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5450 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_draw.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11741 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16357 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3759 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_gui.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    22633 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyglet_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33046 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5189 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3094 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.ui
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6770 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/simple_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18390 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/framework.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      103 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9332 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/app.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15634 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/area.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4327 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/basic.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9967 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/button.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      667 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/const.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13556 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/container.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2375 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/deprecated.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5042 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/dialog.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2620 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/document.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2630 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/form.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1127 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/group.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4684 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/input.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1840 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/keysym.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4901 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/layout.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3332 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/menus.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1049 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/misc.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      360 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/pguglobals.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       99 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/readme.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4602 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/select.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11132 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/slider.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      991 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/style.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4488 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/surface.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12923 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/table.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11458 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/textarea.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16553 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/theme.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11434 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/widget.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4196 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/settings.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      722 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/environment_sandbox.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3346 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/helpers.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    25878 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/simulator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10542 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/sodarace.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/CPPN_fixed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1267 2023-02-03 22:41:04.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/CPPN_mutable.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1099 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/README.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      214 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1322 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/galloper.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      923 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/radial.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      541 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/runner.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      957 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/square.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3401 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/walk_creator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      973 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/wheel.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      628 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/environments/utils.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9163 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/mutation_model.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/sandbox/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      406 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/Dockerfile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      162 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/Pipfile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9266 2023-02-04 21:59:34.000000 OpenELM-0.9.2/src/openelm/sandbox/Pipfile.lock
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      931 2023-02-17 21:08:09.000000 OpenELM-0.9.2/src/openelm/sandbox/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/sandbox/scripts/
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       85 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/scripts/bootstrap.sh
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       33 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/scripts/build.sh
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)      107 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/scripts/launch.sh
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/sandbox/server/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/server/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:58.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      496 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/CPPN_fixed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1230 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       71 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      881 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/radial.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      933 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/square.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2975 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/walk_creator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3625 2023-03-08 01:31:49.000000 OpenELM-0.9.2/src/openelm/sandbox/server/index.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10138 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/sandbox/server/sandbox_codex_execute.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/sandbox/server/templates/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-01-20 14:24:40.000000 OpenELM-0.9.2/src/openelm/sandbox/server/templates/index.html
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/src/openelm/utils/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      338 2023-03-08 01:31:49.000000 OpenELM-0.9.2/src/openelm/utils/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6293 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/utils/code_eval.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13343 2023-02-17 21:08:10.000000 OpenELM-0.9.2/src/openelm/utils/diff_eval.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      907 2023-07-10 19:30:39.000000 OpenELM-0.9.2/src/openelm/utils/utils.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/tests/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1018 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/conftest.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1762 2023-03-08 01:31:49.000000 OpenELM-0.9.2/tests/test_code_execute.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/tests/test_data/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17990 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/test_data/cppn_fixed.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2532 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/test_data/square.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18081 2023-02-17 21:08:10.000000 OpenELM-0.9.2/tests/test_diff.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8668 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/test_mapelites.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4628 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/test_sodarace_env.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2602 2023-07-10 19:30:39.000000 OpenELM-0.9.2/tests/test_sodarace_walkers.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      736 2023-02-17 21:08:10.000000 OpenELM-0.9.2/tests/test_truncate.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/trlx_example/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/trlx_example/configs/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2152 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/configs/ppo_softprompt_config.yml
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/trlx_example/model/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12827 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/model/accelerate_ppo_softprompt_model.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 21:07:59.000000 OpenELM-0.9.2/trlx_example/orchestrator/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6254 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/orchestrator/ppo_softprompt_orchestrator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1743 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/ppo_softprompt_long_completions.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1600 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/ppo_softprompt_sentiment.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1769 2023-01-20 14:24:40.000000 OpenELM-0.9.2/trlx_example/ppo_softprompt_short_completions.py
```

### Comparing `OpenELM-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `OpenELM-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `OpenELM-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/.github/workflows/build.yml` & `OpenELM-0.9.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/.gitignore` & `OpenELM-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/.pre-commit-config.yaml` & `OpenELM-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/.readthedocs.yml` & `OpenELM-0.9.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/CITATION.cff` & `OpenELM-0.9.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/CODE_OF_CONDUCT.md` & `OpenELM-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/CONTRIBUTING.md` & `OpenELM-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/LICENSE` & `OpenELM-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/OpenELM_Paper.pdf` & `OpenELM-0.9.2/OpenELM_Paper.pdf`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/PKG-INFO` & `OpenELM-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenELM
-Version: 0.9.1
+Version: 0.9.2
 Summary: Evolution Through Large Models
 Author: CarperAI
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -40,14 +40,22 @@
 We want to support users with many different compute profiles!
 3. Provide a simple interface to a range of example environments for evolutionary search, to let users adapt these easily for their domain.
 4. Demonstrate the potential of evolution with LLMs.
 
 # Install
 `pip install openelm`
 
+To use the sodarace environment, you must first `pip install swig`.
+
+Then:
+
+`pip install openelm[sodaracer]`
+
+See the pyproject.toml for further install options.
+
 # Features
 
 ### LLM integration with evolutionary algorithms
 OpenELM supports the quality-diversity algorithms MAP-Elites, CVT-MAP-Elites, and Deep Grid MAP-Elites, as well as a simple genetic algorithm baseline.
 
 ### Evolutionary operators
 OpenELM supports:
```

### Comparing `OpenELM-0.9.1/README.md` & `OpenELM-0.9.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 We want to support users with many different compute profiles!
 3. Provide a simple interface to a range of example environments for evolutionary search, to let users adapt these easily for their domain.
 4. Demonstrate the potential of evolution with LLMs.
 
 # Install
 `pip install openelm`
 
+To use the sodarace environment, you must first `pip install swig`.
+
+Then:
+
+`pip install openelm[sodaracer]`
+
+See the pyproject.toml for further install options.
+
 # Features
 
 ### LLM integration with evolutionary algorithms
 OpenELM supports the quality-diversity algorithms MAP-Elites, CVT-MAP-Elites, and Deep Grid MAP-Elites, as well as a simple genetic algorithm baseline.
 
 ### Evolutionary operators
 OpenELM supports:
```

### Comparing `OpenELM-0.9.1/docs/Makefile` & `OpenELM-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/docs/make.bat` & `OpenELM-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/docs/source/conf.py` & `OpenELM-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/docs/source/images/openelm_favicon.ico` & `OpenELM-0.9.2/docs/source/images/openelm_favicon.ico`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/docs/source/openelm.rst` & `OpenELM-0.9.2/docs/source/openelm.rst`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/pyproject.toml` & `OpenELM-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,12 @@
     "sphinx_rtd_theme",
     "sphinx_autodoc_typehints",
 ]
 triton = [
     "tritonclient[all]",
 ]
 notebook = ["ipython"]
-sodaracer = ["pygame"]
+sodaracer = [
+    "swig>=4.1.0",
+    "box2d-py==2.3.8",
+    "pygame"
+]
```

### Comparing `OpenELM-0.9.1/run_elm.py` & `OpenELM-0.9.2/run_elm.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/run_p3.py` & `OpenELM-0.9.2/run_p3.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/OpenELM.egg-info/PKG-INFO` & `OpenELM-0.9.2/src/OpenELM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenELM
-Version: 0.9.1
+Version: 0.9.2
 Summary: Evolution Through Large Models
 Author: CarperAI
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -40,14 +40,22 @@
 We want to support users with many different compute profiles!
 3. Provide a simple interface to a range of example environments for evolutionary search, to let users adapt these easily for their domain.
 4. Demonstrate the potential of evolution with LLMs.
 
 # Install
 `pip install openelm`
 
+To use the sodarace environment, you must first `pip install swig`.
+
+Then:
+
+`pip install openelm[sodaracer]`
+
+See the pyproject.toml for further install options.
+
 # Features
 
 ### LLM integration with evolutionary algorithms
 OpenELM supports the quality-diversity algorithms MAP-Elites, CVT-MAP-Elites, and Deep Grid MAP-Elites, as well as a simple genetic algorithm baseline.
 
 ### Evolutionary operators
 OpenELM supports:
```

### Comparing `OpenELM-0.9.1/src/OpenELM.egg-info/SOURCES.txt` & `OpenELM-0.9.2/src/OpenELM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/algorithms/genetic.py` & `OpenELM-0.9.2/src/openelm/algorithms/genetic.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/algorithms/map_elites.py` & `OpenELM-0.9.2/src/openelm/algorithms/map_elites.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_bugs.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmark_bugs.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_crossover.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmark_crossover.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_lm_speed.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmark_lm_speed.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmark_sodarace_parallel.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_tinygp.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmark_tinygp.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/benchmarks/benchmarks_triton.py` & `OpenELM-0.9.2/src/openelm/benchmarks/benchmarks_triton.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/codegen_triton.py` & `OpenELM-0.9.2/src/openelm/codegen/codegen_triton.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/codegen_utilities.py` & `OpenELM-0.9.2/src/openelm/codegen/codegen_utilities.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/configuration_codegen.py` & `OpenELM-0.9.2/src/openelm/codegen/configuration_codegen.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/modelling_codegen.py` & `OpenELM-0.9.2/src/openelm/codegen/modelling_codegen.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py` & `OpenELM-0.9.2/src/openelm/codegen/triton_utils/codegen_gptj_converter.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/triton_utils/config_template.pbtxt` & `OpenELM-0.9.2/src/openelm/codegen/triton_utils/config_template.pbtxt`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/triton_utils/convert_ft.py` & `OpenELM-0.9.2/src/openelm/codegen/triton_utils/convert_ft.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py` & `OpenELM-0.9.2/src/openelm/codegen/triton_utils/gptj_ftconverter.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/codegen/triton_utils/readme.md` & `OpenELM-0.9.2/src/openelm/codegen/triton_utils/readme.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/configs.py` & `OpenELM-0.9.2/src/openelm/configs.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/elm.py` & `OpenELM-0.9.2/src/openelm/elm.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/base.py` & `OpenELM-0.9.2/src/openelm/environments/base.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/p3/__init__.py` & `OpenELM-0.9.2/src/openelm/environments/p3/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/p3/p3.py` & `OpenELM-0.9.2/src/openelm/environments/p3/p3.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/poetry.py` & `OpenELM-0.9.2/src/openelm/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/README.md` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/antonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/antonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/cause_and_effect.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/cause_and_effect.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/diff.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/diff.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/letters_list.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/letters_list.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/num_to_verbal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/num_to_verbal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/orthography_starts_with.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/orthography_starts_with.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentence_similarity.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/sentence_similarity.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentiment.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/sentiment.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/word_in_context.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/annotations/word_in_context.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/addsub.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/addsub.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/aqua.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/aqua.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/coin_flip.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/coin_flip.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/commonsensqa.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/commonsensqa.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/date_understanding.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/date_understanding.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/gsm8k.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/gsm8k.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/last_letters.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/last_letters.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/multiarith.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/multiarith.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/shuffled_objects.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/shuffled_objects.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/singleeq.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/singleeq.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/strategyqa.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/strategyqa.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/svamp.csv` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/cot_dataset/svamp.csv`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/active_to_passive.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/active_to_passive.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/antonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/antonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/cause_and_effect.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/cause_and_effect.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/common_concept.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/common_concept.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/diff.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/diff.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/first_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/first_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/informal_to_formal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/informal_to_formal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/larger_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/larger_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/letters_list.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/letters_list.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/negation.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/negation.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/num_to_verbal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/num_to_verbal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/orthography_starts_with.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/orthography_starts_with.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/rhymes.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/rhymes.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/second_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/second_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentence_similarity.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sentence_similarity.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentiment.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sentiment.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/singular_to_plural.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/singular_to_plural.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sum.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/sum.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/synonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/synonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/taxonomy_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/taxonomy_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-de.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-de.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-es.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-es.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-fr.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/translation_en-fr.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/word_in_context.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/induction_input/word_in_context.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/active_to_passive.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/active_to_passive.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/antonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/antonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/cause_and_effect.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/cause_and_effect.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/common_concept.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/common_concept.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/diff.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/diff.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/first_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/first_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/informal_to_formal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/informal_to_formal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/larger_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/larger_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/letters_list.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/letters_list.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/negation.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/negation.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/num_to_verbal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/num_to_verbal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/orthography_starts_with.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/orthography_starts_with.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/rhymes.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/rhymes.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/second_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/second_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentence_similarity.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sentence_similarity.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentiment.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sentiment.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/singular_to_plural.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/singular_to_plural.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sum.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/sum.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/synonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/synonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/taxonomy_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/taxonomy_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-de.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-de.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-es.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-es.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-fr.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/translation_en-fr.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/word_in_context.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/execute/word_in_context.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/active_to_passive.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/active_to_passive.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/antonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/antonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/cause_and_effect.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/cause_and_effect.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/common_concept.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/common_concept.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/diff.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/diff.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/first_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/first_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/informal_to_formal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/informal_to_formal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/larger_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/larger_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/letters_list.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/letters_list.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/negation.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/negation.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/num_to_verbal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/num_to_verbal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/orthography_starts_with.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/orthography_starts_with.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/rhymes.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/rhymes.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/second_word_letter.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/second_word_letter.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentence_similarity.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sentence_similarity.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentiment.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sentiment.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/singular_to_plural.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/singular_to_plural.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sum.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/sum.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/synonyms.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/synonyms.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/taxonomy_animal.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/taxonomy_animal.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-de.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-de.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-es.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-es.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-fr.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/translation_en-fr.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/word_in_context.json` & `OpenELM-0.9.2/src/openelm/environments/prompt/datasets/raw/induce/word_in_context.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/prompt.py` & `OpenELM-0.9.2/src/openelm/environments/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/prompt/utils.py` & `OpenELM-0.9.2/src/openelm/environments/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/README.md` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/__init__.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_draw.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_draw.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_gui.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_gui.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyglet_framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyglet_framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.ui` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.ui`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/simple_framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/backends/simple_framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/framework.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/framework.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/__init__.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/app.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/app.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/area.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/area.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/basic.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/basic.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/button.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/button.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/const.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/const.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/container.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/container.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/deprecated.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/deprecated.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/dialog.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/dialog.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/document.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/document.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/form.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/form.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/group.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/group.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/input.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/input.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/keysym.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/keysym.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/layout.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/layout.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/menus.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/menus.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/misc.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/misc.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/select.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/select.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/slider.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/slider.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/style.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/style.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/surface.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/surface.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/table.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/table.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/textarea.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/textarea.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/theme.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/theme.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/widget.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/widget.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/settings.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/box2d_examples/settings.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/environment_sandbox.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/environment_sandbox.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/helpers.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/helpers.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/simulator.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/simulator.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/sodarace.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/sodarace.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/CPPN_mutable.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/README.md` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/galloper.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/galloper.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/radial.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/radial.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/runner.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/runner.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/square.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/square.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/walk_creator.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/walk_creator.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/wheel.py` & `OpenELM-0.9.2/src/openelm/environments/sodaracer/walker/wheel.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/environments/utils.py` & `OpenELM-0.9.2/src/openelm/environments/utils.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/mutation_model.py` & `OpenELM-0.9.2/src/openelm/mutation_model.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/Pipfile.lock` & `OpenELM-0.9.2/src/openelm/sandbox/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/README.md` & `OpenELM-0.9.2/src/openelm/sandbox/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/radial.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/radial.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/square.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/square.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/walk_creator.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/environments/walker/walk_creator.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/index.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/index.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/sandbox/server/sandbox_codex_execute.py` & `OpenELM-0.9.2/src/openelm/sandbox/server/sandbox_codex_execute.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/utils/code_eval.py` & `OpenELM-0.9.2/src/openelm/utils/code_eval.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/utils/diff_eval.py` & `OpenELM-0.9.2/src/openelm/utils/diff_eval.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/src/openelm/utils/utils.py` & `OpenELM-0.9.2/src/openelm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/conftest.py` & `OpenELM-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_code_execute.py` & `OpenELM-0.9.2/tests/test_code_execute.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_data/cppn_fixed.json` & `OpenELM-0.9.2/tests/test_data/cppn_fixed.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_data/square.json` & `OpenELM-0.9.2/tests/test_data/square.json`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_diff.py` & `OpenELM-0.9.2/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_mapelites.py` & `OpenELM-0.9.2/tests/test_mapelites.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_sodarace_env.py` & `OpenELM-0.9.2/tests/test_sodarace_env.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_sodarace_walkers.py` & `OpenELM-0.9.2/tests/test_sodarace_walkers.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/tests/test_truncate.py` & `OpenELM-0.9.2/tests/test_truncate.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/README.md` & `OpenELM-0.9.2/trlx_example/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/configs/ppo_softprompt_config.yml` & `OpenELM-0.9.2/trlx_example/configs/ppo_softprompt_config.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/model/accelerate_ppo_softprompt_model.py` & `OpenELM-0.9.2/trlx_example/model/accelerate_ppo_softprompt_model.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py` & `OpenELM-0.9.2/trlx_example/orchestrator/ppo_softprompt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/ppo_softprompt_long_completions.py` & `OpenELM-0.9.2/trlx_example/ppo_softprompt_long_completions.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/ppo_softprompt_sentiment.py` & `OpenELM-0.9.2/trlx_example/ppo_softprompt_sentiment.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.9.1/trlx_example/ppo_softprompt_short_completions.py` & `OpenELM-0.9.2/trlx_example/ppo_softprompt_short_completions.py`

 * *Files identical despite different names*

