# Comparing `tmp/dolma-0.6.1.tar.gz` & `tmp/dolma-0.6.2.tar.gz`

## Comparing `dolma-0.6.1.tar` & `dolma-0.6.2.tar`

### file list

```diff
@@ -1,78 +1,82 @@
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dolma-0.6.1/Cargo.toml
--rw-r--r--   0      502       20      475 2023-06-27 20:15:25.000000 dolma-0.6.1/.flake8
--rw-r--r--   0      502       20     2791 2023-07-09 05:40:50.000000 dolma-0.6.1/.github/workflows/CI.yml
--rw-r--r--   0      502       20      549 2023-06-22 18:02:39.000000 dolma-0.6.1/.gitignore
--rw-r--r--   0      502       20     1813 2023-07-09 05:40:50.000000 dolma-0.6.1/CITATION.cff
--rw-r--r--   0      502       20    11357 2023-06-20 21:37:30.000000 dolma-0.6.1/LICENSE
--rw-r--r--   0      502       20     2294 2023-07-09 05:51:44.000000 dolma-0.6.1/Makefile
--rw-r--r--   0      502       20     3093 2023-07-09 05:51:23.000000 dolma-0.6.1/README.md
--rw-r--r--   0      502       20     3217 2023-07-09 05:42:06.000000 dolma-0.6.1/pyproject.toml
--rw-r--r--   0      502       20      736 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/__init__.py
--rw-r--r--   0      502       20     4401 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/__init__.py
--rw-r--r--   0      502       20     1494 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/__main__.py
--rw-r--r--   0      502       20     4689 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/deduper.py
--rw-r--r--   0      502       20     4589 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/mixer.py
--rw-r--r--   0      502       20      473 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/shared.py
--rw-r--r--   0      502       20     1957 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/tagger.py
--rw-r--r--   0      502       20      219 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/__init__.py
--rw-r--r--   0      502       20     6111 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/data_types.py
--rw-r--r--   0      502       20      337 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/errors.py
--rw-r--r--   0      502       20     6482 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/ft_dataset.py
--rw-r--r--   0      502       20     5557 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/ft_tagger.py
--rw-r--r--   0      502       20    15587 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/parallel.py
--rw-r--r--   0      502       20     6326 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/paths.py
--rw-r--r--   0      502       20     1254 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/registry.py
--rw-r--r--   0      502       20    11812 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/runtime.py
--rw-r--r--   0      502       20     1032 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/taggers.py
--rw-r--r--   0      502       20       42 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/trainer.py
--rw-r--r--   0      502       20     2031 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/utils.py
--rw-r--r--   0      502       20     9484 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/vizualizer.py
--rw-r--r--   0      502       20     3777 2023-06-22 18:00:53.000000 dolma-0.6.1/python/dolma/data/naughty_words_en.txt
--rw-r--r--   0      502       20        0 2023-06-21 16:42:48.000000 dolma-0.6.1/python/dolma/py.typed
--rw-r--r--   0      502       20       72 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/__init__.py
--rw-r--r--   0      502       20     3277 2023-06-22 18:02:34.000000 dolma-0.6.1/python/dolma/taggers/c4.py
--rw-r--r--   0      502       20     6433 2023-07-09 05:39:12.000000 dolma-0.6.1/python/dolma/taggers/code.py
--rw-r--r--   0      502       20     6857 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/gopher.py
--rw-r--r--   0      502       20     1898 2023-06-22 18:02:47.000000 dolma-0.6.1/python/dolma/taggers/jigsaw.py
--rw-r--r--   0      502       20     6391 2023-06-23 22:30:50.000000 dolma-0.6.1/python/dolma/taggers/language.py
--rw-r--r--   0      502       20     4876 2023-06-22 18:02:44.000000 dolma-0.6.1/python/dolma/taggers/length.py
--rw-r--r--   0      502       20    10494 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/pii.py
--rw-r--r--   0      502       20      744 2023-06-22 18:02:42.000000 dolma-0.6.1/python/dolma/taggers/sampling.py
--rw-r--r--   0      502       20      232 2023-06-22 18:32:09.000000 dolma-0.6.1/res/logo.md
--rw-r--r--   0      502       20  1813803 2023-06-22 18:39:27.000000 dolma-0.6.1/res/logo.png
--rw-r--r--   0      502       20     9277 2023-06-21 23:41:09.000000 dolma-0.6.1/src/bloom_filter.rs
--rw-r--r--   0      502       20    14421 2023-07-09 05:40:50.000000 dolma-0.6.1/src/deduper.rs
--rw-r--r--   0      502       20     1124 2023-07-09 05:40:50.000000 dolma-0.6.1/src/lib.rs
--rw-r--r--   0      502       20     7176 2023-07-09 05:40:50.000000 dolma-0.6.1/src/mixer.rs
--rw-r--r--   0      502       20    11131 2023-07-09 05:40:50.000000 dolma-0.6.1/src/s3_util.rs
--rw-r--r--   0      502       20    23416 2023-07-09 05:40:50.000000 dolma-0.6.1/src/shard.rs
--rw-r--r--   0      502       20      863 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/c4-cleaned.json
--rw-r--r--   0      502       20      564 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/dedupe-by-url.json
--rw-r--r--   0      502       20      553 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/dedupe-paragraphs.json
--rw-r--r--   0      502       20      815 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/email-spans.json
--rw-r--r--   0      502       20      799 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/filter-by-spans.json
--rw-r--r--   0      502       20      792 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/mixer.json
--rw-r--r--   0      502       20      716 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/paragraph-spans.json
--rw-r--r--   0      502       20    25985 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/documents.json.gz
--rw-r--r--   0      502       20      702 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/duplicate-paragraphs.json.gz
--rw-r--r--   0      502       20      489 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/dedupe-by-url.json.gz
--rw-r--r--   0      502       20      746 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/dedupe-paragraphs.json.gz
--rw-r--r--   0      502       20    26447 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/email-spans.json.gz
--rw-r--r--   0      502       20    14879 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/filter-by-spans.json.gz
--rw-r--r--   0      502       20    15748 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/mixer.json.gz
--rw-r--r--   0      502       20    26524 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/remove-paragraphs.json.gz
--rw-r--r--   0      502       20      614 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/pii-attributes.json.gz
--rw-r--r--   0      502       20      570 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/sample-attributes.json.gz
--rw-r--r--   0      502       20      543 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/toxicity-attributes.json.gz
--rw-r--r--   0      502       20      352 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/__init__.py
--rw-r--r--   0      502       20     3342 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_data_types.py
--rw-r--r--   0      502       20      471 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_deduper.py
--rw-r--r--   0      502       20      820 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_mixer.py
--rw-r--r--   0      502       20     1395 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_omegaconf.py
--rw-r--r--   0      502       20     2459 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_parallel.py
--rw-r--r--   0      502       20     8972 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_paths.py
--rw-r--r--   0      502       20     1846 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_runtime.py
--rw-r--r--   0      502       20     9701 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_taggers.py
--rw-r--r--   0      502       20     4043 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_utils.py
--rw-r--r--   0      502       20    57199 2023-07-09 05:40:50.000000 dolma-0.6.1/Cargo.lock
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 dolma-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dolma-0.6.2/Cargo.toml
+-rw-r--r--   0     1001      123      475 2023-07-10 21:38:08.000000 dolma-0.6.2/.flake8
+-rw-r--r--   0     1001      123     3220 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     2194 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      123      691 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0     1001      123     1077 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      123      414 2023-07-10 21:38:08.000000 dolma-0.6.2/.github/workflows/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0     1001      123      549 2023-07-10 21:38:08.000000 dolma-0.6.2/.gitignore
+-rw-r--r--   0     1001      123     1813 2023-07-10 21:38:08.000000 dolma-0.6.2/CITATION.cff
+-rw-r--r--   0     1001      123    11357 2023-07-10 21:38:08.000000 dolma-0.6.2/LICENSE
+-rw-r--r--   0     1001      123     2295 2023-07-10 21:38:08.000000 dolma-0.6.2/Makefile
+-rw-r--r--   0     1001      123     3156 2023-07-10 21:38:08.000000 dolma-0.6.2/README.md
+-rw-r--r--   0     1001      123     3217 2023-07-10 21:38:08.000000 dolma-0.6.2/pyproject.toml
+-rw-r--r--   0     1001      123      736 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/__init__.py
+-rw-r--r--   0     1001      123     4401 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/__init__.py
+-rw-r--r--   0     1001      123     1494 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/__main__.py
+-rw-r--r--   0     1001      123     4689 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/deduper.py
+-rw-r--r--   0     1001      123     4589 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/mixer.py
+-rw-r--r--   0     1001      123      473 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/shared.py
+-rw-r--r--   0     1001      123     1957 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/cli/tagger.py
+-rw-r--r--   0     1001      123      219 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/__init__.py
+-rw-r--r--   0     1001      123     6111 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/data_types.py
+-rw-r--r--   0     1001      123      337 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/errors.py
+-rw-r--r--   0     1001      123     6482 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/ft_dataset.py
+-rw-r--r--   0     1001      123     5557 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/ft_tagger.py
+-rw-r--r--   0     1001      123    15587 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/parallel.py
+-rw-r--r--   0     1001      123     6326 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/paths.py
+-rw-r--r--   0     1001      123     1254 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/registry.py
+-rw-r--r--   0     1001      123    11812 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/runtime.py
+-rw-r--r--   0     1001      123     1032 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/taggers.py
+-rw-r--r--   0     1001      123       42 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/trainer.py
+-rw-r--r--   0     1001      123     2031 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/utils.py
+-rw-r--r--   0     1001      123     9484 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/core/vizualizer.py
+-rw-r--r--   0     1001      123     3777 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/data/naughty_words_en.txt
+-rw-r--r--   0     1001      123        0 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/py.typed
+-rw-r--r--   0     1001      123       72 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/__init__.py
+-rw-r--r--   0     1001      123     3277 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/c4.py
+-rw-r--r--   0     1001      123     6433 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/code.py
+-rw-r--r--   0     1001      123     6857 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/gopher.py
+-rw-r--r--   0     1001      123     1898 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/jigsaw.py
+-rw-r--r--   0     1001      123     6391 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/language.py
+-rw-r--r--   0     1001      123     4876 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/length.py
+-rw-r--r--   0     1001      123    10494 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/pii.py
+-rw-r--r--   0     1001      123      744 2023-07-10 21:38:08.000000 dolma-0.6.2/python/dolma/taggers/sampling.py
+-rw-r--r--   0     1001      123      232 2023-07-10 21:38:08.000000 dolma-0.6.2/res/logo.md
+-rw-r--r--   0     1001      123  1813803 2023-07-10 21:38:08.000000 dolma-0.6.2/res/logo.png
+-rw-r--r--   0     1001      123     9277 2023-07-10 21:38:08.000000 dolma-0.6.2/src/bloom_filter.rs
+-rw-r--r--   0     1001      123    14421 2023-07-10 21:38:08.000000 dolma-0.6.2/src/deduper.rs
+-rw-r--r--   0     1001      123     1124 2023-07-10 21:38:08.000000 dolma-0.6.2/src/lib.rs
+-rw-r--r--   0     1001      123     7176 2023-07-10 21:38:08.000000 dolma-0.6.2/src/mixer.rs
+-rw-r--r--   0     1001      123    11131 2023-07-10 21:38:08.000000 dolma-0.6.2/src/s3_util.rs
+-rw-r--r--   0     1001      123    23416 2023-07-10 21:38:08.000000 dolma-0.6.2/src/shard.rs
+-rw-r--r--   0     1001      123      863 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/c4-cleaned.json
+-rw-r--r--   0     1001      123      564 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/dedupe-by-url.json
+-rw-r--r--   0     1001      123      553 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/dedupe-paragraphs.json
+-rw-r--r--   0     1001      123      815 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/email-spans.json
+-rw-r--r--   0     1001      123      799 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/filter-by-spans.json
+-rw-r--r--   0     1001      123      792 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/mixer.json
+-rw-r--r--   0     1001      123      716 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/config/paragraph-spans.json
+-rw-r--r--   0     1001      123    25985 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/documents.json.gz
+-rw-r--r--   0     1001      123      702 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/duplicate-paragraphs.json.gz
+-rw-r--r--   0     1001      123      489 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/dedupe-by-url.json.gz
+-rw-r--r--   0     1001      123      746 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/dedupe-paragraphs.json.gz
+-rw-r--r--   0     1001      123    26447 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/email-spans.json.gz
+-rw-r--r--   0     1001      123    14879 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/filter-by-spans.json.gz
+-rw-r--r--   0     1001      123    15748 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/mixer.json.gz
+-rw-r--r--   0     1001      123    26524 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/expected/remove-paragraphs.json.gz
+-rw-r--r--   0     1001      123      614 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/pii-attributes.json.gz
+-rw-r--r--   0     1001      123      570 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/sample-attributes.json.gz
+-rw-r--r--   0     1001      123      543 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/data/toxicity-attributes.json.gz
+-rw-r--r--   0     1001      123      352 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/__init__.py
+-rw-r--r--   0     1001      123     3342 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_data_types.py
+-rw-r--r--   0     1001      123      471 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_deduper.py
+-rw-r--r--   0     1001      123      820 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_mixer.py
+-rw-r--r--   0     1001      123     1395 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_omegaconf.py
+-rw-r--r--   0     1001      123     2459 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_parallel.py
+-rw-r--r--   0     1001      123     8972 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_paths.py
+-rw-r--r--   0     1001      123     1846 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_runtime.py
+-rw-r--r--   0     1001      123     9701 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_taggers.py
+-rw-r--r--   0     1001      123     4043 2023-07-10 21:38:08.000000 dolma-0.6.2/tests/python/test_utils.py
+-rw-r--r--   0     1001      123    57199 2023-07-10 21:38:15.000000 dolma-0.6.2/Cargo.lock
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 dolma-0.6.2/PKG-INFO
```

### Comparing `dolma-0.6.1/Cargo.toml` & `dolma-0.6.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dolma"
-version = "0.6.0"
+version = "0.6.2"
 edition = "2021"
 license = "Apache-2.0"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dolma"
```

### Comparing `dolma-0.6.1/.github/workflows/CI.yml` & `dolma-0.6.2/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-# This file is autogenerated by maturin v1.1.0
-# To update, run
-#
-#    maturin generate-ci github
-#
 name: CI
 
 on:
-  push:
-    branches:
-      - main
-      - master
-    tags:
-      - '*'
-  pull_request:
-  workflow_dispatch:
+   push:
+     branches:
+       - main
+       - master
+     tags:
+       - '*'
+   pull_request:
+   workflow_dispatch:
+
 
 permissions:
   contents: read
 
 jobs:
-  linux:
+  build-linux:
     runs-on: ubuntu-latest
+    env:
+      CC:   gcc-11
+      CXX:  g++-11
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
+      - name: Setup environment
+        run:  |
+          sudo apt-get update
+          sudo apt-get install --yes --upgrade build-essential cmake protobuf-compiler libssl-dev glibc-source
+      - name: Install 32bit version of libc
+        if: ${{ matrix.target == 'x86' }}
+        run: |
+          sudo apt-get install --yes --upgrade libc6-dev-i386
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
-          manylinux: auto
+          sccache: ${{ matrix.target == 'x86' && 'false' || 'true' }}
+          manylinux: ${{ matrix.target == 'x86' && 'auto' || '2_28' }}
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
-  windows:
+  build-windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
@@ -54,37 +61,37 @@
           python-version: '3.10'
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
+          sccache: true
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
-  macos:
+  build-macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
+          sccache: true
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   sdist:
@@ -102,15 +109,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
+    needs: [build-linux, build-windows, build-macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `dolma-0.6.1/.gitignore` & `dolma-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/CITATION.cff` & `dolma-0.6.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/LICENSE` & `dolma-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/Makefile` & `dolma-0.6.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 endif
 
 setup:
 	@echo "${OS_MESSAGE}: installing..."
 	$(shell "${CMAKE_SETUP}")
 	$(shell "${PROTOBUF_SETUP}")
 	$(shell "${OPENSSL_SETUP}")
-	which cargo || curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+	which cargo || curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
 	which maturin || pip install maturin
 
 publish:
 	maturin publish
 
 test: setup develop setup-test test-python test-rust clean-test
 
@@ -49,9 +49,13 @@
 	aws s3 sync tests/data/expected s3://ai2-llm/pretraining-data/tests/mixer/expected  --exclude ".*" --exclude "*/.*"
 
 develop:
 	maturin develop --extras=dev
 
 style:
 	rustfmt --edition 2021 src/*.rs
-	autopep8 --in-place --recursive python/ && isort python/ && black python/
-	autopep8 --in-place --recursive tests/python/ && isort tests/python/ && black tests/python/
+	autopep8 --in-place --recursive python/
+	isort python/
+	black python/
+	autopep8 --in-place --recursive tests/python/
+	isort tests/python/
+	black tests/python/
```

### Comparing `dolma-0.6.1/README.md` & `dolma-0.6.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 *Data to feed OLMo's Appetite*
 
 
 <img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256"></img>
 
 Data and tools for generating and inspecting OLMo pre-training data.
 
-To get started, install dolma using pip.
+To get started, install dolma using [pip](https://pypi.org/project/dolma/).
 
 ```shell
 pip install dolma
 ```
 
 ## Usage
 
@@ -44,26 +44,26 @@
 ```
 
 This command will run the `random_number_v1` tagger on all documents in the specified S3 paths. The results will be written to the `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v0/attributes/sample` and `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v1/attributes/sample` paths.
 
 ### `dolma dedupe`
 
 The dedupe command is used to deduplicate a set of documents at the attribute level using a bloom filter.
-For example configurations, see directory `test/config`. For example:
+For example configurations, see directory `tests/config`. For example:
 
 ```shell
-dolma dedupe -c test/config/dedupe-paragraphs.json
+dolma dedupe -c tests/config/dedupe-paragraphs.json
 ```
 
 ### `dolma mix`
 
-The mix command is used to mix documents from multiple sources, optionally filtering by attributes and/or performing string replacement. For example configurations, see directory `test/config`. For example:
+The mix command is used to mix documents from multiple sources, optionally filtering by attributes and/or performing string replacement. For example configurations, see directory `tests/config`. For example:
 
 ```shell
-dolma mix -c test/config/mixer.json
+dolma mix -c tests/config/mixer.json
 ```
 
 
 ## Development
 
 Create a conda environment with Python >= 3.8. In this case, we use Python 3.10 and use Anaconda to create the environment.
 
@@ -74,15 +74,15 @@
 After creating the environment, activate it and install necessary tools using the included makefile.
 
 ```shell
 conda activate dolma
 make setup
 ```
 
-Finally, to begin development, install the repository in editable mode using maturin.
+and restart your shell. Finally, to begin development, install the repository in editable mode using maturin.
 
 ```shell
 make develop
 ```
 
 To run tests, use the following command.
```

### Comparing `dolma-0.6.1/pyproject.toml` & `dolma-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dolma"
-version = "0.6.1"
+version = "0.6.2"
 description = "Data filters"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "requests",
     "tqdm",
```

### Comparing `dolma-0.6.1/python/dolma/__init__.py` & `dolma-0.6.2/python/dolma/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/cli/__init__.py` & `dolma-0.6.2/python/dolma/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/cli/__main__.py` & `dolma-0.6.2/python/dolma/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/cli/deduper.py` & `dolma-0.6.2/python/dolma/cli/deduper.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/cli/mixer.py` & `dolma-0.6.2/python/dolma/cli/mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/cli/tagger.py` & `dolma-0.6.2/python/dolma/cli/tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/data_types.py` & `dolma-0.6.2/python/dolma/core/data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/ft_dataset.py` & `dolma-0.6.2/python/dolma/core/ft_dataset.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/ft_tagger.py` & `dolma-0.6.2/python/dolma/core/ft_tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/parallel.py` & `dolma-0.6.2/python/dolma/core/parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/paths.py` & `dolma-0.6.2/python/dolma/core/paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/registry.py` & `dolma-0.6.2/python/dolma/core/registry.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/runtime.py` & `dolma-0.6.2/python/dolma/core/runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/taggers.py` & `dolma-0.6.2/python/dolma/core/taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/utils.py` & `dolma-0.6.2/python/dolma/core/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/core/vizualizer.py` & `dolma-0.6.2/python/dolma/core/vizualizer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/data/naughty_words_en.txt` & `dolma-0.6.2/python/dolma/data/naughty_words_en.txt`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/c4.py` & `dolma-0.6.2/python/dolma/taggers/c4.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/code.py` & `dolma-0.6.2/python/dolma/taggers/code.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/gopher.py` & `dolma-0.6.2/python/dolma/taggers/gopher.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/jigsaw.py` & `dolma-0.6.2/python/dolma/taggers/jigsaw.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/language.py` & `dolma-0.6.2/python/dolma/taggers/language.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/length.py` & `dolma-0.6.2/python/dolma/taggers/length.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/pii.py` & `dolma-0.6.2/python/dolma/taggers/pii.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/python/dolma/taggers/sampling.py` & `dolma-0.6.2/python/dolma/taggers/sampling.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/res/logo.png` & `dolma-0.6.2/res/logo.png`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/bloom_filter.rs` & `dolma-0.6.2/src/bloom_filter.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/deduper.rs` & `dolma-0.6.2/src/deduper.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/lib.rs` & `dolma-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/mixer.rs` & `dolma-0.6.2/src/mixer.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/s3_util.rs` & `dolma-0.6.2/src/s3_util.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/src/shard.rs` & `dolma-0.6.2/src/shard.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/c4-cleaned.json` & `dolma-0.6.2/tests/config/c4-cleaned.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/dedupe-by-url.json` & `dolma-0.6.2/tests/config/dedupe-by-url.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/dedupe-paragraphs.json` & `dolma-0.6.2/tests/config/dedupe-paragraphs.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/email-spans.json` & `dolma-0.6.2/tests/config/email-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/filter-by-spans.json` & `dolma-0.6.2/tests/config/filter-by-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/mixer.json` & `dolma-0.6.2/tests/config/mixer.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/config/paragraph-spans.json` & `dolma-0.6.2/tests/config/paragraph-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/documents.json.gz` & `dolma-0.6.2/tests/data/documents.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/duplicate-paragraphs.json.gz` & `dolma-0.6.2/tests/data/duplicate-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/expected/dedupe-paragraphs.json.gz` & `dolma-0.6.2/tests/data/expected/dedupe-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/expected/email-spans.json.gz` & `dolma-0.6.2/tests/data/expected/email-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/expected/filter-by-spans.json.gz` & `dolma-0.6.2/tests/data/expected/filter-by-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/expected/mixer.json.gz` & `dolma-0.6.2/tests/data/expected/mixer.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/expected/remove-paragraphs.json.gz` & `dolma-0.6.2/tests/data/expected/remove-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/pii-attributes.json.gz` & `dolma-0.6.2/tests/data/pii-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/sample-attributes.json.gz` & `dolma-0.6.2/tests/data/sample-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/data/toxicity-attributes.json.gz` & `dolma-0.6.2/tests/data/toxicity-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_data_types.py` & `dolma-0.6.2/tests/python/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_mixer.py` & `dolma-0.6.2/tests/python/test_mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_omegaconf.py` & `dolma-0.6.2/tests/python/test_omegaconf.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_parallel.py` & `dolma-0.6.2/tests/python/test_parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_paths.py` & `dolma-0.6.2/tests/python/test_paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_runtime.py` & `dolma-0.6.2/tests/python/test_runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/tests/python/test_taggers.py` & `dolma-0.6.2/tests/python/test_taggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,67 +214,67 @@
                 "end": 79,
                 "type": "fraction_of_characters_in_duplicate_10grams",
                 "score": 0.0,
                 "mention": text,
             },
         )
         self.assertEqual(
-            d["spans"][9], {"start": 0, "end": 15, "type": "character_count", "score": 79.0, "mention": text}
+            d["spans"][9], {"start": 0, "end": 79, "type": "character_count", "score": 79.0, "mention": text}
         )
         self.assertEqual(
-            d["spans"][10], {"start": 0, "end": 15, "type": "word_count", "score": 13.0, "mention": text}
+            d["spans"][10], {"start": 0, "end": 79, "type": "word_count", "score": 13.0, "mention": text}
         )
         self.assertEqual(
-            d["spans"][11], {"start": 0, "end": 15, "type": "median_word_length", "score": 4.0, "mention": text}
+            d["spans"][11], {"start": 0, "end": 79, "type": "median_word_length", "score": 4.0, "mention": text}
         )
         self.assertEqual(
-            d["spans"][12], {"start": 0, "end": 15, "type": "symbol_to_word_ratio", "score": 0.0, "mention": text}
+            d["spans"][12], {"start": 0, "end": 79, "type": "symbol_to_word_ratio", "score": 0.0, "mention": text}
         )
         self.assertEqual(
             d["spans"][13],
             {
                 "start": 0,
-                "end": 15,
+                "end": 79,
                 "type": "fraction_of_words_with_alpha_character",
                 "score": 1.0,
                 "mention": text,
             },
         )
         self.assertEqual(
-            d["spans"][14], {"start": 0, "end": 15, "type": "required_word_count", "score": 0.0, "mention": text}
+            d["spans"][14], {"start": 0, "end": 79, "type": "required_word_count", "score": 0.0, "mention": text}
         )
         self.assertEqual(
             d["spans"][15],
             {
                 "start": 0,
-                "end": 15,
+                "end": 79,
                 "type": "fraction_of_lines_starting_with_bullet_point",
                 "score": 0.0,
                 "mention": text,
             },
         )
         self.assertEqual(
             d["spans"][16],
             {
                 "start": 0,
-                "end": 15,
+                "end": 79,
                 "type": "fraction_of_lines_ending_with_ellipsis",
                 "score": 0.0,
                 "mention": text,
             },
         )
         self.assertEqual(
             d["spans"][17],
-            {"start": 0, "end": 15, "type": "fraction_of_duplicate_lines", "score": 0.0, "mention": text},
+            {"start": 0, "end": 79, "type": "fraction_of_duplicate_lines", "score": 0.0, "mention": text},
         )
         self.assertEqual(
             d["spans"][18],
             {
                 "start": 0,
-                "end": 15,
+                "end": 79,
                 "type": "fraction_of_characters_in_duplicate_lines",
                 "score": 0.0,
                 "mention": text,
             },
         )
 
     def test_word_count_is_whitespace_sep(self):
```

### Comparing `dolma-0.6.1/tests/python/test_utils.py` & `dolma-0.6.2/tests/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.1/Cargo.lock` & `dolma-0.6.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dolma"
-version = "0.6.0"
+version = "0.6.2"
 dependencies = [
  "ahash",
  "aws-config",
  "aws-sdk-s3",
  "byteorder",
  "clap",
  "env_logger",
```

### Comparing `dolma-0.6.1/PKG-INFO` & `dolma-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolma
-Version: 0.6.1
+Version: 0.6.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests
 Requires-Dist: tqdm
@@ -52,15 +52,15 @@
 *Data to feed OLMo's Appetite*
 
 
 <img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256"></img>
 
 Data and tools for generating and inspecting OLMo pre-training data.
 
-To get started, install dolma using pip.
+To get started, install dolma using [pip](https://pypi.org/project/dolma/).
 
 ```shell
 pip install dolma
 ```
 
 ## Usage
 
@@ -93,26 +93,26 @@
 ```
 
 This command will run the `random_number_v1` tagger on all documents in the specified S3 paths. The results will be written to the `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v0/attributes/sample` and `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v1/attributes/sample` paths.
 
 ### `dolma dedupe`
 
 The dedupe command is used to deduplicate a set of documents at the attribute level using a bloom filter.
-For example configurations, see directory `test/config`. For example:
+For example configurations, see directory `tests/config`. For example:
 
 ```shell
-dolma dedupe -c test/config/dedupe-paragraphs.json
+dolma dedupe -c tests/config/dedupe-paragraphs.json
 ```
 
 ### `dolma mix`
 
-The mix command is used to mix documents from multiple sources, optionally filtering by attributes and/or performing string replacement. For example configurations, see directory `test/config`. For example:
+The mix command is used to mix documents from multiple sources, optionally filtering by attributes and/or performing string replacement. For example configurations, see directory `tests/config`. For example:
 
 ```shell
-dolma mix -c test/config/mixer.json
+dolma mix -c tests/config/mixer.json
 ```
 
 
 ## Development
 
 Create a conda environment with Python >= 3.8. In this case, we use Python 3.10 and use Anaconda to create the environment.
 
@@ -123,15 +123,15 @@
 After creating the environment, activate it and install necessary tools using the included makefile.
 
 ```shell
 conda activate dolma
 make setup
 ```
 
-Finally, to begin development, install the repository in editable mode using maturin.
+and restart your shell. Finally, to begin development, install the repository in editable mode using maturin.
 
 ```shell
 make develop
 ```
 
 To run tests, use the following command.
```

