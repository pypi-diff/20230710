# Comparing `tmp/deepsecrets-1.1.1.tar.gz` & `tmp/deepsecrets-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.1.1.tar", max compression
+gzip compressed data, was "deepsecrets-1.1.2.tar", max compression
```

## Comparing `deepsecrets-1.1.1.tar` & `deepsecrets-1.1.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.1.1/LICENSE
--rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.1.1/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.1.1/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-07-04 12:10:29.237681 deepsecrets-1.1.1/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.1.1/deepsecrets/__main__.py
--rw-r--r--   0        0        0     7633 2023-07-04 11:57:11.643286 deepsecrets-1.1.1/deepsecrets/cli.py
--rw-r--r--   0        0        0     2256 2023-07-03 10:00:00.045463 deepsecrets-1.1.1/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.1.1/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.1.1/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.1.1/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.1.1/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.1.1/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.1.1/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.1.1/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7355 2023-06-28 16:55:39.241507 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      797 2023-06-28 18:04:12.582631 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-07-04 13:26:48.391130 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     3886 2023-06-28 16:55:38.707373 deepsecrets-1.1.1/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.1.1/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.1.1/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.1.1/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.1.1/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.1.1/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.1.1/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      281 2023-06-28 18:04:11.970796 deepsecrets-1.1.1/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-07-04 13:26:47.808614 deepsecrets-1.1.1/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8594 2023-07-04 09:53:49.065871 deepsecrets-1.1.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5166 2023-07-04 09:53:48.500643 deepsecrets-1.1.1/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.1.1/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.1.1/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0    10945 2023-07-04 12:01:13.022231 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-06-28 17:29:54.564568 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1371 2023-06-28 18:14:23.816502 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      556 2023-06-28 18:14:23.216059 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7398 2023-06-28 18:18:53.090440 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     7425 2023-07-04 13:39:06.736554 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     3845 2023-06-28 18:18:52.403328 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     6529 2023-07-04 13:39:05.813218 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-06-28 17:29:53.978332 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6862 2023-07-04 12:01:12.367278 deepsecrets-1.1.1/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3491 2023-07-05 06:48:16.796963 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5474 2023-07-04 09:56:49.777143 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     2681 2023-06-30 18:34:33.195619 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5265 2023-07-03 12:07:13.918625 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc
--rw-r--r--   0        0        0     1763 2023-07-05 06:48:16.188353 deepsecrets-1.1.1/deepsecrets/core/utils/cpu.py
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.1.1/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3022 2023-07-04 09:56:48.933550 deepsecrets-1.1.1/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.1.1/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0     1538 2023-06-30 18:34:31.705561 deepsecrets-1.1.1/deepsecrets/core/utils/guess_filetype.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.1.1/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2810 2023-07-03 12:07:13.137522 deepsecrets-1.1.1/deepsecrets/core/utils/lexer_finder.py
--rw-r--r--   0        0        0     2669 2023-07-04 14:27:00.175183 deepsecrets-1.1.1/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.1.1/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5823 2023-07-04 11:57:19.417209 deepsecrets-1.1.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3333 2023-07-04 11:57:18.653455 deepsecrets-1.1.1/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1709 2023-07-05 06:48:55.892463 deepsecrets-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 deepsecrets-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.1.2/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.1.2/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-07-04 12:10:29.237681 deepsecrets-1.1.2/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.1.2/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     7633 2023-07-05 06:50:44.322329 deepsecrets-1.1.2/deepsecrets/cli.py
+-rw-r--r--   0        0        0     2256 2023-07-05 06:50:44.322607 deepsecrets-1.1.2/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.1.2/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6192 2023-07-10 07:10:15.525374 deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.1.2/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.1.2/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.1.2/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4341 2023-07-10 07:10:14.909631 deepsecrets-1.1.2/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.1.2/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.1.2/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.1.2/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7355 2023-07-05 06:50:45.025780 deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      797 2023-07-05 06:50:45.124212 deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-07-04 13:26:48.391130 deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     3886 2023-07-05 06:50:44.322904 deepsecrets-1.1.2/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.1.2/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.1.2/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.1.2/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.1.2/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.1.2/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.1.2/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.1.2/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.1.2/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.1.2/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      281 2023-07-05 06:50:44.323170 deepsecrets-1.1.2/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-07-04 13:26:47.808614 deepsecrets-1.1.2/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8594 2023-07-05 06:50:45.105258 deepsecrets-1.1.2/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5166 2023-07-05 06:50:44.323480 deepsecrets-1.1.2/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.1.2/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.1.2/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.1.2/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10945 2023-07-05 06:50:45.116788 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-06-28 17:29:54.564568 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1394 2023-07-07 11:39:23.581532 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      576 2023-07-07 11:39:22.838020 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7398 2023-07-05 06:50:45.132557 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     8095 2023-07-07 12:00:19.692752 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     3845 2023-07-05 06:50:44.323946 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     7101 2023-07-07 12:00:18.994741 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-06-28 17:29:53.978332 deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.1.2/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6862 2023-07-05 06:50:44.324458 deepsecrets-1.1.2/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.1.2/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.1.2/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.1.2/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3491 2023-07-05 06:51:02.323194 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5474 2023-07-05 06:50:45.113254 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     2681 2023-07-05 06:50:45.210097 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5265 2023-07-05 06:50:45.207350 deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc
+-rw-r--r--   0        0        0     1763 2023-07-05 06:51:01.714239 deepsecrets-1.1.2/deepsecrets/core/utils/cpu.py
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.1.2/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3022 2023-07-05 06:50:44.324873 deepsecrets-1.1.2/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.1.2/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0     1538 2023-07-05 06:50:44.325103 deepsecrets-1.1.2/deepsecrets/core/utils/guess_filetype.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.1.2/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2810 2023-07-05 06:50:44.325414 deepsecrets-1.1.2/deepsecrets/core/utils/lexer_finder.py
+-rw-r--r--   0        0        0     2669 2023-07-05 06:50:44.325543 deepsecrets-1.1.2/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.1.2/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.2/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5823 2023-07-05 06:50:45.099734 deepsecrets-1.1.2/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3333 2023-07-05 06:50:44.325785 deepsecrets-1.1.2/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1709 2023-07-10 07:12:01.747588 deepsecrets-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 deepsecrets-1.1.2/PKG-INFO
```

### Comparing `deepsecrets-1.1.1/LICENSE` & `deepsecrets-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/README.md` & `deepsecrets-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/__init__.py` & `deepsecrets-1.1.2/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/cli.py` & `deepsecrets-1.1.2/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/config.py` & `deepsecrets-1.1.2/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2bed9a64 (Tue Jun 27 14:07:39 2023 UTC)
+moddate:  0xd6aeab64 (Mon Jul 10 07:10:14 2023 UTC)
 files sz: 4341
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.1.2/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.1.2/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/regex.py` & `deepsecrets-1.1.2/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.1.2/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.1.2/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.1.2/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0a669c64 (Wed Jun 28 16:55:38 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 3886
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1b769c64 (Wed Jun 28 18:04:11 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 281
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/file.py` & `deepsecrets-1.1.2/deepsecrets/core/model/file.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/finding.py` & `deepsecrets-1.1.2/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.1.2/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/model/token.py` & `deepsecrets-1.1.2/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2ceca364 (Tue Jul  4 09:53:48 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 5166
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.1.2/deepsecrets/core/modes/iscan_mode.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.1.2/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x080aa464 (Tue Jul  4 12:01:12 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 6862
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7f789c64 (Wed Jun 28 18:14:23 2023 UTC)
-files sz: 556
+moddate:  0x6af9a764 (Fri Jul  7 11:39:22 2023 UTC)
+files sz: 576
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -36,17 +36,17 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
-            0d5a0f640e5a10640f5a1165126410651364116514660464128404a60000
-            00ab0000000000000000005a1565126413651364116514660464148404a6
-            000000ab0000000000000000005a1664155300
+            0d5a0f640e5a10640f5a1164105a12651364116514641265156604641384
+            04a6000000ab0000000000000000005a1665136414651464126515660464
+            158404a6000000ab0000000000000000005a1764165300
            4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Language')
                        8 STORE_NAME               2 (__qualname__)
          
            5          10 LOAD_CONST               1 ('py')
@@ -84,51 +84,54 @@
          
           16          54 LOAD_CONST              12 ('java')
                       56 STORE_NAME              14 (JAVA)
          
           17          58 LOAD_CONST              13 ('kt')
                       60 STORE_NAME              15 (KOTLIN)
          
-          19          62 LOAD_CONST              14 ('any')
-                      64 STORE_NAME              16 (ANY)
+          18          62 LOAD_CONST              14 ('swift')
+                      64 STORE_NAME              16 (SWIFT)
          
-          20          66 LOAD_CONST              15 ('unknown')
-                      68 STORE_NAME              17 (UNKNOWN)
+          20          66 LOAD_CONST              15 ('any')
+                      68 STORE_NAME              17 (ANY)
          
-          22          70 LOAD_NAME               18 (classmethod)
+          21          70 LOAD_CONST              16 ('unknown')
+                      72 STORE_NAME              18 (UNKNOWN)
          
-          23          72 LOAD_CONST              16 ('text')
-                      74 LOAD_NAME               19 (str)
-                      76 LOAD_CONST              17 ('return')
-                      78 LOAD_NAME               20 (object)
-                      80 BUILD_TUPLE              4
-                      82 LOAD_CONST              18 (<code object from_text, file "/app/deepsecrets/core/tokenizers/helpers/semantic/language.py", line 22>)
-                      84 MAKE_FUNCTION            4 (annotations)
-         
-          22          86 PRECALL                  0
-                      90 CALL                     0
-         
-          23         100 STORE_NAME              21 (from_text)
-         
-          27         102 LOAD_NAME               18 (classmethod)
-         
-          28         104 LOAD_CONST              19 ('value')
-                     106 LOAD_NAME               19 (str)
-                     108 LOAD_CONST              17 ('return')
-                     110 LOAD_NAME               20 (object)
-                     112 BUILD_TUPLE              4
-                     114 LOAD_CONST              20 (<code object _missing_, file "/app/deepsecrets/core/tokenizers/helpers/semantic/language.py", line 27>)
-                     116 MAKE_FUNCTION            4 (annotations)
-         
-          27         118 PRECALL                  0
-                     122 CALL                     0
-         
-          28         132 STORE_NAME              22 (_missing_)
-                     134 LOAD_CONST              21 (None)
-                     136 RETURN_VALUE
+          23          74 LOAD_NAME               19 (classmethod)
+         
+          24          76 LOAD_CONST              17 ('text')
+                      78 LOAD_NAME               20 (str)
+                      80 LOAD_CONST              18 ('return')
+                      82 LOAD_NAME               21 (object)
+                      84 BUILD_TUPLE              4
+                      86 LOAD_CONST              19 (<code object from_text, file "/app/deepsecrets/core/tokenizers/helpers/semantic/language.py", line 23>)
+                      88 MAKE_FUNCTION            4 (annotations)
+         
+          23          90 PRECALL                  0
+                      94 CALL                     0
+         
+          24         104 STORE_NAME              22 (from_text)
+         
+          28         106 LOAD_NAME               19 (classmethod)
+         
+          29         108 LOAD_CONST              20 ('value')
+                     110 LOAD_NAME               20 (str)
+                     112 LOAD_CONST              18 ('return')
+                     114 LOAD_NAME               21 (object)
+                     116 BUILD_TUPLE              4
+                     118 LOAD_CONST              21 (<code object _missing_, file "/app/deepsecrets/core/tokenizers/helpers/semantic/language.py", line 28>)
+                     120 MAKE_FUNCTION            4 (annotations)
+         
+          28         122 PRECALL                  0
+                     126 CALL                     0
+         
+          29         136 STORE_NAME              23 (_missing_)
+                     138 LOAD_CONST              22 (None)
+                     140 RETURN_VALUE
          consts
             'Language'
             'py'
             'go'
             'php'
             ('js', 'jsx')
             'toml'
@@ -136,39 +139,40 @@
             'yaml'
             'ini'
             'pp'
             'sh'
             'cs'
             'java'
             'kt'
+            'swift'
             'any'
             'unknown'
             'text'
             'return'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c01a00000000000000000000000000000000000000000006401a6
                   010000ab0100000000000000006402190000000000000000007d0202007c
                   007c02a6010000ab0100000000000000005300
-                22           0 RESUME                   0
+                23           0 RESUME                   0
                
-                24           2 LOAD_FAST                1 (text)
+                25           2 LOAD_FAST                1 (text)
                              4 LOAD_METHOD              0 (split)
                             26 LOAD_CONST               1 ('.')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 LOAD_CONST               2 (-1)
                             44 BINARY_SUBSCR
                             54 STORE_FAST               2 (ext)
                
-                25          56 PUSH_NULL
+                26          56 PUSH_NULL
                             58 LOAD_FAST                0 (cls)
                             60 LOAD_FAST                2 (ext)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 RETURN_VALUE
                consts
                   None
@@ -176,49 +180,49 @@
                   -1
                names      ('split',)
                varnames   ('cls', 'text', 'ext')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/language.py'
                name       'from_text'
-               firstlineno 22
+               firstlineno 23
                lnotab 0x02023601
             'value'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007400000000000000000000006a0100000000000000005300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                
-                29           2 LOAD_GLOBAL              0 (Language)
+                30           2 LOAD_GLOBAL              0 (Language)
                             14 LOAD_ATTR                1 (UNKNOWN)
                             24 RETURN_VALUE
                consts
                   None
                names      ('Language', 'UNKNOWN')
                varnames   ('cls', 'value')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/language.py'
                name       '_missing_'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x0202
             None
-         names      ('__name__', '__module__', '__qualname__', 'PYTHON', 'GOLANG', 'PHP', 'JS', 'TOML', 'JSON', 'YAML', 'INI', 'PUPPET', 'SHELL', 'CSHARP', 'JAVA', 'KOTLIN', 'ANY', 'UNKNOWN', 'classmethod', 'str', 'object', 'from_text', '_missing_')
+         names      ('__name__', '__module__', '__qualname__', 'PYTHON', 'GOLANG', 'PHP', 'JS', 'TOML', 'JSON', 'YAML', 'INI', 'PUPPET', 'SHELL', 'CSHARP', 'JAVA', 'KOTLIN', 'SWIFT', 'ANY', 'UNKNOWN', 'classmethod', 'str', 'object', 'from_text', '_missing_')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/language.py'
          name       'Language'
          firstlineno 4
          lnotab
-            0x0a01040104010401040104010401040104010401040104010401040204
-            01040202010eff0e01020402010eff0e01
+            0x0a01040104010401040104010401040104010401040104010401040104
+            020401040202010eff0e01020402010eff0e01
       'Language'
       None
    names      ('aenum', 'MultiValueEnum', 'Language')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/language.py'
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     YAML = 'yaml'
     INI = 'ini'
     PUPPET = 'pp'
     SHELL = 'sh'
     CSHARP = 'cs'
     JAVA = 'java'
     KOTLIN = 'kt'
+    SWIFT = 'swift'
 
     ANY = 'any'
     UNKNOWN = 'unknown'
 
     @classmethod
     def from_text(cls, text: str) -> object:
         ext = text.split('.')[-1]
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8c799c64 (Wed Jun 28 18:18:52 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 3845
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf920a464 (Tue Jul  4 13:39:05 2023 UTC)
-files sz: 6529
+moddate:  0x52fea764 (Fri Jul  7 12:00:18 2023 UTC)
+files sz: 7101
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
@@ -1109,25 +1109,37 @@
             0102f7100c04010c011e02340134fe040408f9100a04010c011e02340134
             0134fd040508f8100b04010c011e023401340134fd040508f8108000f604
             7f001802011aff0e01
       'VariableDetectionRules'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 11
+         stacksize : 13
          flags     : 0
          code
             0x970065005a0164005a020200650365046a050000000000000000020065
             066a0700000000000000006401a6010000ab010000000000000000020065
             08020065066a0700000000000000006402a6010000ab0100000000000000
             006701ac03a6010000ab0100000000000000000200650865096a0a000000
             00000000006a0b00000000000000006701ac04a6010000ab010000000000
             00000002006508020065066a0700000000000000006405a6010000ab0100
             000000000000006701ac03a6010000ab01000000000000000064069c0369
-            00ac07a6040000ab04000000000000000067015a0c64085300
+            00ac07a6040000ab0400000000000000000200650365046a0c0000000000
+            000000020065066a0700000000000000006408a6010000ab010000000000
+            00000002006508020065066a0700000000000000006409a6010000ab0100
+            00000000000000020065066a070000000000000000640aa6010000ab0100
+            00000000000000020065066a070000000000000000640ba6010000ab0100
+            000000000000006703ac03a6010000ab0100000000000000000200650802
+            0065066a070000000000000000640ca6010000ab01000000000000000067
+            01ac03a6010000ab01000000000000000002006508020065066a07000000
+            0000000000640da6010000ab0100000000000000006701ac03a6010000ab
+            01000000000000000002006508020065066a070000000000000000640ea6
+            010000ab0100000000000000006701ac03a6010000ab0100000000000000
+            00640f9c046900ac07a6040000ab04000000000000000067025a0d641053
+            00
          166           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('VariableSuppressionRules')
                        8 STORE_NAME               2 (__qualname__)
          
          168          10 PUSH_NULL
@@ -1190,38 +1202,137 @@
          
          182         208 BUILD_MAP                0
          
          168         210 KW_NAMES                 7
                      212 PRECALL                  4
                      216 CALL                     4
          
-         167         226 BUILD_LIST               1
-                     228 STORE_NAME              12 (rules)
-                     230 LOAD_CONST               8 (None)
-                     232 RETURN_VALUE
+         185         226 PUSH_NULL
+                     228 LOAD_NAME                3 (VaribleSuppressor)
+         
+         186         230 LOAD_NAME                4 (Language)
+                     232 LOAD_ATTR               12 (SWIFT)
+         
+         187         242 PUSH_NULL
+                     244 LOAD_NAME                6 (re)
+                     246 LOAD_ATTR                7 (compile)
+                     256 LOAD_CONST               8 ('(n)(p)(n)(p)L')
+                     258 PRECALL                  1
+                     262 CALL                     1
+         
+         189         272 PUSH_NULL
+                     274 LOAD_NAME                8 (Match)
+         
+         190         276 PUSH_NULL
+                     278 LOAD_NAME                6 (re)
+                     280 LOAD_ATTR                7 (compile)
+                     290 LOAD_CONST               9 ('^decode$')
+                     292 PRECALL                  1
+                     296 CALL                     1
+         
+         191         306 PUSH_NULL
+                     308 LOAD_NAME                6 (re)
+                     310 LOAD_ATTR                7 (compile)
+                     320 LOAD_CONST              10 ('^decodeIfPresent$')
+                     322 PRECALL                  1
+                     326 CALL                     1
+         
+         192         336 PUSH_NULL
+                     338 LOAD_NAME                6 (re)
+                     340 LOAD_ATTR                7 (compile)
+                     350 LOAD_CONST              11 ('^unbox$')
+                     352 PRECALL                  1
+                     356 CALL                     1
+         
+         189         366 BUILD_LIST               3
+                     368 KW_NAMES                 3
+                     370 PRECALL                  1
+                     374 CALL                     1
+         
+         194         384 PUSH_NULL
+                     386 LOAD_NAME                8 (Match)
+                     388 PUSH_NULL
+                     390 LOAD_NAME                6 (re)
+                     392 LOAD_ATTR                7 (compile)
+                     402 LOAD_CONST              12 ('^\\($')
+                     404 PRECALL                  1
+                     408 CALL                     1
+                     418 BUILD_LIST               1
+                     420 KW_NAMES                 3
+                     422 PRECALL                  1
+                     426 CALL                     1
+         
+         195         436 PUSH_NULL
+                     438 LOAD_NAME                8 (Match)
+                     440 PUSH_NULL
+                     442 LOAD_NAME                6 (re)
+                     444 LOAD_ATTR                7 (compile)
+                     454 LOAD_CONST              13 ('^(key|keyPath)$')
+                     456 PRECALL                  1
+                     460 CALL                     1
+                     470 BUILD_LIST               1
+                     472 KW_NAMES                 3
+                     474 PRECALL                  1
+                     478 CALL                     1
+         
+         196         488 PUSH_NULL
+                     490 LOAD_NAME                8 (Match)
+                     492 PUSH_NULL
+                     494 LOAD_NAME                6 (re)
+                     496 LOAD_ATTR                7 (compile)
+                     506 LOAD_CONST              14 ('^:$')
+                     508 PRECALL                  1
+                     512 CALL                     1
+                     522 BUILD_LIST               1
+                     524 KW_NAMES                 3
+                     526 PRECALL                  1
+                     530 CALL                     1
+         
+         188         540 LOAD_CONST              15 ((1, 2, 3, 4))
+                     542 BUILD_CONST_KEY_MAP      4
+         
+         198         544 BUILD_MAP                0
+         
+         185         546 KW_NAMES                 7
+                     548 PRECALL                  4
+                     552 CALL                     4
+         
+         167         562 BUILD_LIST               2
+                     564 STORE_NAME              13 (rules)
+                     566 LOAD_CONST              16 (None)
+                     568 RETURN_VALUE
          consts
             'VariableSuppressionRules'
             '(p)(n).*?p(p)'
             '^<$'
             ('values',)
             ('types',)
             '^>$'
             (1, 2, 3)
             ('language', 'stream_pattern', 'match_rules', 'match_semantics')
+            '(n)(p)(n)(p)L'
+            '^decode$'
+            '^decodeIfPresent$'
+            '^unbox$'
+            '^\\($'
+            '^(key|keyPath)$'
+            '^:$'
+            (1, 2, 3, 4)
             None
-         names      ('__name__', '__module__', '__qualname__', 'VaribleSuppressor', 'Language', 'JS', 're', 'compile', 'Match', 'PygmentsToken', 'Name', 'Tag', 'rules')
+         names      ('__name__', '__module__', '__qualname__', 'VaribleSuppressor', 'Language', 'JS', 're', 'compile', 'Match', 'PygmentsToken', 'Name', 'Tag', 'SWIFT', 'rules')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
          name       'VariableSuppressionRules'
          firstlineno 166
          lnotab
             0x0a0204010c011e0204011eff1203040118ff100304011eff12f9040b02
-            f210ff
+            f2101104010c011e0204011e011e011efd12053401340134f8040a02f310
+            ee
       'VariableSuppressionRules'
    names      ('regex', 're', 'typing', 'List', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector', 'Match', 'VaribleDetector', 'VaribleSuppressor', 'pygments.token', 'Token', 'PygmentsToken', 'VariableDetectionRules', 'VariableSuppressionRules')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
    name       '<module>'
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,9 +176,25 @@
                     types=[PygmentsToken.Name.Tag]
                 ),
                 3: Match(values=[
                     re.compile('^>$'),
                 ]),
             },
             match_semantics={}
+        ),
+
+        VaribleSuppressor(
+            language=Language.SWIFT,
+            stream_pattern=re.compile('(n)(p)(n)(p)L'),
+            match_rules={
+                1: Match(values=[
+                    re.compile('^decode$'),
+                    re.compile('^decodeIfPresent$'),
+                    re.compile('^unbox$')
+                ]),
+                2: Match(values=[re.compile('^\($')]),
+                3: Match(values=[re.compile('^(key|keyPath)$')]),
+                4: Match(values=[re.compile('^:$')]),
+            },
+            match_semantics={}
         )
     ]
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/lexer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.1.2/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3012a564 (Wed Jul  5 06:48:16 2023 UTC)
+moddate:  0xd512a564 (Wed Jul  5 06:51:01 2023 UTC)
 files sz: 1763
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe0eca364 (Tue Jul  4 09:56:48 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 3022
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x37209f64 (Fri Jun 30 18:34:31 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 1538
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xf1b9a264 (Mon Jul  3 12:07:13 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 2810
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/cpu.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/cpu.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/fs.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/guess_filetype.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/guess_filetype.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/core/utils/lexer_finder.py` & `deepsecrets-1.1.2/deepsecrets/core/utils/lexer_finder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.1.2/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/rules/regexes.json` & `deepsecrets-1.1.2/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.1.2/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.1.2/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e09a464 (Tue Jul  4 11:57:18 2023 UTC)
+moddate:  0xc412a564 (Wed Jul  5 06:50:44 2023 UTC)
 files sz: 3333
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.1.1/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.1.2/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.1/pyproject.toml` & `deepsecrets-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.1.1"
+version = "1.1.2"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
```

### Comparing `deepsecrets-1.1.1/PKG-INFO` & `deepsecrets-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.1.1
+Version: 1.1.2
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
```

