# Comparing `tmp/academic_tracker-1.0.4.tar.gz` & `tmp/academic_tracker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "academic_tracker-1.0.4.tar", last modified: Wed Jul  5 13:45:36 2023, max compression
+gzip compressed data, was "academic_tracker-1.0.5.tar", last modified: Mon Jul 10 13:06:23 2023, max compression
```

## Comparing `academic_tracker-1.0.4.tar` & `academic_tracker-1.0.5.tar`

### file list

```diff
@@ -1,179 +1,180 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.625418 academic_tracker-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.525989 academic_tracker-1.0.4/.github/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.558659 academic_tracker-1.0.4/.github/workflows/
--rw-rw-rw-   0        0        0     1480 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/build.yml
--rw-rw-rw-   0        0        0     1531 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/build_documentation.yml
--rw-rw-rw-   0        0        0     1241 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/codecov.yml
--rw-rw-rw-   0        0        0      165 2023-07-05 12:15:20.000000 academic_tracker-1.0.4/.gitignore
--rw-rw-rw-   0        0        0      105 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1037 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/CITATION.cff
--rw-rw-rw-   0        0        0     1948 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      197 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9823 2023-07-05 13:45:36.624390 academic_tracker-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8759 2023-07-05 12:14:25.000000 academic_tracker-1.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.345114 academic_tracker-1.0.4/docs/
--rw-rw-rw-   0        0        0      598 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.526986 academic_tracker-1.0.4/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.527993 academic_tracker-1.0.4/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.377817 academic_tracker-1.0.4/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0      801 2022-09-01 18:37:58.000000 academic_tracker-1.0.4/docs/_build/html/_sources/api.rst.txt
--rw-rw-rw-   0        0        0     8147 2022-09-14 11:26:26.000000 academic_tracker-1.0.4/docs/_build/html/_sources/guide.rst.txt
--rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0    35244 2022-03-15 15:11:47.000000 academic_tracker-1.0.4/docs/_build/html/_sources/jsonschema.rst.txt
--rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/license.rst.txt
--rw-rw-rw-   0        0        0    21003 2022-06-28 19:30:27.000000 academic_tracker-1.0.4/docs/_build/html/_sources/reporting.rst.txt
--rw-rw-rw-   0        0        0      517 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/todo.rst.txt
--rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/tokenization.rst.txt
--rw-rw-rw-   0        0        0    32448 2022-03-24 20:40:49.000000 academic_tracker-1.0.4/docs/_build/html/_sources/tutorial.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.390800 academic_tracker-1.0.4/docs/_build/html/_static/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.528981 academic_tracker-1.0.4/docs/_build/html/_static/css/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.402422 academic_tracker-1.0.4/docs/_build/html/_static/css/fonts/
--rw-rw-rw-   0        0        0   444379 2022-09-13 14:59:21.000000 academic_tracker-1.0.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0      286 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0      801 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/api.rst
--rw-rw-rw-   0        0        0     6835 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/conf.py
--rw-rw-rw-   0        0        0     8147 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/guide.rst
--rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/index.rst
--rw-rw-rw-   0        0        0    35244 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/jsonschema.rst
--rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/license.rst
--rwxrwxrwx   0        0        0      787 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/make.bat
--rw-rw-rw-   0        0        0    21003 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/reporting.rst
--rw-rw-rw-   0        0        0      295 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/requirements.txt
--rw-rw-rw-   0        0        0      570 2023-07-05 07:49:44.000000 academic_tracker-1.0.4/docs/todo.rst
--rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/tokenization.rst
--rw-rw-rw-   0        0        0    32446 2023-07-05 07:49:44.000000 academic_tracker-1.0.4/docs/tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.424016 academic_tracker-1.0.4/example_configs/
--rw-rw-rw-   0        0        0    21920 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_project_and_summary_reports_no_duplicates__full_example.json
--rw-rw-rw-   0        0        0    22499 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__full_example.json
--rw-rw-rw-   0        0        0     2512 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__template.json
--rw-rw-rw-   0        0        0     2457 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports_no_duplicates__template.json
--rw-rw-rw-   0        0        0      252 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 13:45:36.625418 academic_tracker-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2428 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.529978 academic_tracker-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.437295 academic_tracker-1.0.4/src/academic_tracker/
--rw-rw-rw-   0        0        0     1485 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/__init__.py
--rw-rw-rw-   0        0        0    23047 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/__main__.py
--rw-rw-rw-   0        0        0    39919 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0    10645 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_modularized.py
--rw-rw-rw-   0        0        0    23904 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_webio.py
--rw-rw-rw-   0        0        0    12932 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/citation_parsing.py
--rw-rw-rw-   0        0        0     7934 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/fileio.py
--rw-rw-rw-   0        0        0    21407 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/helper_functions.py
--rw-rw-rw-   0        0        0    19018 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0     9348 2023-07-05 11:57:11.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_modularized.py
--rw-rw-rw-   0        0        0    21154 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_webio.py
--rw-rw-rw-   0        0        0    19791 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/tracker_schema.py
--rw-rw-rw-   0        0        0    13114 2023-07-05 11:57:27.000000 academic_tracker-1.0.4/src/academic_tracker/user_input_checking.py
--rw-rw-rw-   0        0        0    13468 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/webio.py
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.454162 academic_tracker-1.0.4/src/academic_tracker.egg-info/
--rw-rw-rw-   0        0        0     9823 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6564 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      215 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.517208 academic_tracker-1.0.4/tests/
--rw-rw-rw-   0        0        0      264 2022-04-05 15:23:06.000000 academic_tracker-1.0.4/tests/conftest.py
--rw-rw-rw-   0        0        0    15727 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/fixtures.py
--rw-rw-rw-   0        0        0       78 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/pytest.ini
--rw-rw-rw-   0        0        0    26868 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_athr_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0    22066 2023-07-05 10:39:45.000000 academic_tracker-1.0.4/tests/test_athr_srch_modularized.py
--rw-rw-rw-   0        0        0    10030 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_athr_srch_webio_no_internet.py
--rw-rw-rw-   0        0        0     6832 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_citation_parsing.py
--rw-rw-rw-   0        0        0    14698 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_fileio.py
--rw-rw-rw-   0        0        0    18175 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_helper_functions.py
--rw-rw-rw-   0        0        0    21571 2023-07-05 10:45:07.000000 academic_tracker-1.0.4/tests/test_main.py
--rw-rw-rw-   0        0        0    13183 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_ref_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0    13615 2023-07-05 11:58:19.000000 academic_tracker-1.0.4/tests/test_ref_srch_modularized.py
--rw-rw-rw-   0        0        0    13519 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_ref_srch_webio_no_internet.py
--rw-rw-rw-   0        0        0    41141 2023-07-05 11:22:09.000000 academic_tracker-1.0.4/tests/test_user_input_checking.py
--rw-rw-rw-   0        0        0     7179 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_webio_no_internet.py
-drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.624390 academic_tracker-1.0.4/tests/testing_files/
--rw-rw-rw-   0        0        0   248560 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_DOI_query.json
--rw-rw-rw-   0        0        0   665536 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_grant_query.json
--rw-rw-rw-   0        0        0     4068 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_pub_dict.json
--rw-rw-rw-   0        0        0  3516898 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_query.json
--rw-rw-rw-   0        0        0   348524 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_author_search_query.json
--rw-rw-rw-   0        0        0     4463 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_pub_dict.json
--rw-rw-rw-   0        0        0    13196 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_query.json
--rw-rw-rw-   0        0        0    11995 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.docx
--rw-rw-rw-   0        0        0       50 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.json
--rw-rw-rw-   0        0        0       28 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.txt
--rw-rw-rw-   0        0        0      158 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors.csv
--rw-rw-rw-   0        0        0      137 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors_missing_column.csv
--rw-rw-rw-   0        0        0      148 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors_missing_value.csv
--rw-rw-rw-   0        0        0     9873 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_project_emails.json
--rw-rw-rw-   0        0        0     7675 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/athr_project_emails_tabular.json
--rw-rw-rw-   0        0        0    19935 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_build_author_loop.txt
--rw-rw-rw-   0        0        0      758 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_build_loop_template_string.txt
--rw-rw-rw-   0        0        0    10266 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report.txt
--rw-rw-rw-   0        0        0    53142 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report_custom_template.txt
--rw-rw-rw-   0        0        0    13762 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors.json
--rw-rw-rw-   0        0        0    79728 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_tabular.json
--rw-rw-rw-   0        0        0    79858 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_truncated.json
--rw-rw-rw-   0        0        0     2927 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/collaborator_emails.json
--rw-rw-rw-   0        0        0     2721 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/collaborator_emails_tabular.json
--rw-rw-rw-   0        0        0      520 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config.json
--rw-rw-rw-   0        0        0    16074 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_tabular.json
--rw-rw-rw-   0        0        0    16210 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated.json
--rw-rw-rw-   0        0        0    19318 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_authors_adjusted.json
--rw-rw-rw-   0        0        0    16141 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noCrossref.json
--rw-rw-rw-   0        0        0    16081 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noORCID.json
--rw-rw-rw-   0        0        0    16143 2023-07-05 11:34:38.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noPubMed.json
--rw-rw-rw-   0        0        0    16803 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_ref_srch_summary_report.json
--rw-rw-rw-   0        0        0   127221 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/emails.json
--rw-rw-rw-   0        0        0        0 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/empty_file.txt
--rw-rw-rw-   0        0        0     2854 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/gen_reports_ref_summary_report.txt
--rw-rw-rw-   0        0        0     8639 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/has_author.xml
--rw-rw-rw-   0        0        0     8305 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/has_pubmed_grants.xml
--rw-rw-rw-   0        0        0  1085702 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/medline.txt
--rw-rw-rw-   0        0        0   221143 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/myncbi_webpages.json
--rw-rw-rw-   0        0        0    22898 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/no_author.xml
--rw-rw-rw-   0        0        0    26743 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/nsf_award_page.txt
--rw-rw-rw-   0        0        0     1261 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/parse_citations_test.txt
--rw-rw-rw-   0        0        0      521 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/project_report.txt
--rw-rw-rw-   0        0        0    15412 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pub_with_PMCID.xml
--rw-rw-rw-   0        0        0   376657 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/publication_dict.json
--rw-rw-rw-   0        0        0    11488 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/publication_dict_truncated.json
--rw-rw-rw-   0        0        0    15743 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict.json
--rw-rw-rw-   0        0        0     1245 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict_truncated.json
--rw-rw-rw-   0        0        0  1111833 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pymed_pubs.pkl
--rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_keys_for_citations.json
--rw-rw-rw-   0        0        0     1916 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_pub_dict.json
--rw-rw-rw-   0        0        0   278548 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_queries.json
--rw-rw-rw-   0        0        0    32553 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_PubMed_pubs.json
--rw-rw-rw-   0        0        0     2993 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_gen_reports_test_pub_dict.json
--rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_keys_for_citations.json
--rw-rw-rw-   0        0        0     6851 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_publication_dict.json
--rw-rw-rw-   0        0        0     1198 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_default.txt
--rw-rw-rw-   0        0        0     4141 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular1.csv
--rw-rw-rw-   0        0        0     2996 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular2.csv
--rw-rw-rw-   0        0        0     4209 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular3.csv
--rw-rw-rw-   0        0        0     6522 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular4.xlsx
--rw-rw-rw-   0        0        0      739 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_template_string.txt
--rw-rw-rw-   0        0        0     2239 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test1.txt
--rw-rw-rw-   0        0        0     1781 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test2.txt
--rw-rw-rw-   0        0        0    12494 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/reference_test.docx
--rw-rw-rw-   0        0        0      751 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/reference_test.txt
--rw-rw-rw-   0        0        0     6272 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_DOIs.json
--rw-rw-rw-   0        0        0     8720 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_author_query.json
--rw-rw-rw-   0        0        0    37686 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_pub_dict.json
--rw-rw-rw-   0        0        0    17630 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_pubs.json
--rw-rw-rw-   0        0        0   244461 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_query.json
--rw-rw-rw-   0        0        0       27 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_csv.csv
--rw-rw-rw-   0        0        0    11952 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_docx.docx
--rw-rw-rw-   0        0        0       14 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_text.txt
--rw-rw-rw-   0        0        0     1118 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenization_report.txt
--rw-rw-rw-   0        0        0   182317 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_MEDLINE.json
--rw-rw-rw-   0        0        0   115779 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations.json
--rw-rw-rw-   0        0        0    86779 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_duplicates_removed.json
--rw-rw-rw-   0        0        0     1568 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test.json
--rw-rw-rw-   0        0        0     2225 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test2.json
--rw-rw-rw-   0        0        0     1170 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test_empty.json
--rw-rw-rw-   0        0        0    44981 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_myncbi_page1.json
--rw-rw-rw-   0        0        0    34674 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_nsf_award_page.json
--rw-rw-rw-   0        0        0     3970 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_parsing_test.json
--rw-rw-rw-   0        0        0     2659 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_ref_test.json
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.737710 academic_tracker-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.323610 academic_tracker-1.0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.363716 academic_tracker-1.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     1480 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/.github/workflows/build.yml
+-rw-rw-rw-   0        0        0     1531 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/.github/workflows/build_documentation.yml
+-rw-rw-rw-   0        0        0     1241 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/.github/workflows/codecov.yml
+-rw-rw-rw-   0        0        0      165 2023-07-05 12:15:20.000000 academic_tracker-1.0.5/.gitignore
+-rw-rw-rw-   0        0        0      105 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1037 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/CITATION.cff
+-rw-rw-rw-   0        0        0     1948 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      197 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9823 2023-07-10 13:06:23.736712 academic_tracker-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8759 2023-07-05 12:14:25.000000 academic_tracker-1.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.421656 academic_tracker-1.0.5/docs/
+-rw-rw-rw-   0        0        0      598 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.324609 academic_tracker-1.0.5/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.325579 academic_tracker-1.0.5/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.453579 academic_tracker-1.0.5/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0      801 2022-09-01 18:37:58.000000 academic_tracker-1.0.5/docs/_build/html/_sources/api.rst.txt
+-rw-rw-rw-   0        0        0     8147 2022-09-14 11:26:26.000000 academic_tracker-1.0.5/docs/_build/html/_sources/guide.rst.txt
+-rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0    35244 2022-03-15 15:11:47.000000 academic_tracker-1.0.5/docs/_build/html/_sources/jsonschema.rst.txt
+-rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/_build/html/_sources/license.rst.txt
+-rw-rw-rw-   0        0        0    21003 2022-06-28 19:30:27.000000 academic_tracker-1.0.5/docs/_build/html/_sources/reporting.rst.txt
+-rw-rw-rw-   0        0        0      517 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/_build/html/_sources/todo.rst.txt
+-rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/_build/html/_sources/tokenization.rst.txt
+-rw-rw-rw-   0        0        0    32448 2022-03-24 20:40:49.000000 academic_tracker-1.0.5/docs/_build/html/_sources/tutorial.rst.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.457541 academic_tracker-1.0.5/docs/_build/html/_static/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.325579 academic_tracker-1.0.5/docs/_build/html/_static/css/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.469264 academic_tracker-1.0.5/docs/_build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0   444379 2022-09-13 14:59:21.000000 academic_tracker-1.0.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0      286 2022-09-09 08:24:14.000000 academic_tracker-1.0.5/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.5/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.5/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0      801 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/api.rst
+-rw-rw-rw-   0        0        0     6835 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/conf.py
+-rw-rw-rw-   0        0        0     8147 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/guide.rst
+-rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/index.rst
+-rw-rw-rw-   0        0        0    35244 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/jsonschema.rst
+-rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/license.rst
+-rwxrwxrwx   0        0        0      787 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/make.bat
+-rw-rw-rw-   0        0        0    21003 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/reporting.rst
+-rw-rw-rw-   0        0        0      295 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/docs/requirements.txt
+-rw-rw-rw-   0        0        0      570 2023-07-05 07:49:44.000000 academic_tracker-1.0.5/docs/todo.rst
+-rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/docs/tokenization.rst
+-rw-rw-rw-   0        0        0    32446 2023-07-07 18:38:23.000000 academic_tracker-1.0.5/docs/tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.495176 academic_tracker-1.0.5/example_configs/
+-rw-rw-rw-   0        0        0    21920 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/example_configs/many_projects_and_authors_project_and_summary_reports_no_duplicates__full_example.json
+-rw-rw-rw-   0        0        0    22499 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports__full_example.json
+-rw-rw-rw-   0        0        0     2512 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports__template.json
+-rw-rw-rw-   0        0        0     2457 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports_no_duplicates__template.json
+-rw-rw-rw-   0        0        0      252 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:06:23.737710 academic_tracker-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2428 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.327577 academic_tracker-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.513125 academic_tracker-1.0.5/src/academic_tracker/
+-rw-rw-rw-   0        0        0     1485 2023-07-07 12:41:34.000000 academic_tracker-1.0.5/src/academic_tracker/__init__.py
+-rw-rw-rw-   0        0        0    26366 2023-07-07 15:50:55.000000 academic_tracker-1.0.5/src/academic_tracker/__main__.py
+-rw-rw-rw-   0        0        0    39919 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/athr_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    10645 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/athr_srch_modularized.py
+-rw-rw-rw-   0        0        0    23904 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/athr_srch_webio.py
+-rw-rw-rw-   0        0        0    12932 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/citation_parsing.py
+-rw-rw-rw-   0        0        0     7934 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/fileio.py
+-rw-rw-rw-   0        0        0    21407 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/helper_functions.py
+-rw-rw-rw-   0        0        0    19018 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/ref_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0     9348 2023-07-05 11:57:11.000000 academic_tracker-1.0.5/src/academic_tracker/ref_srch_modularized.py
+-rw-rw-rw-   0        0        0    21154 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/ref_srch_webio.py
+-rw-rw-rw-   0        0        0    19791 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/tracker_schema.py
+-rw-rw-rw-   0        0        0    13114 2023-07-05 11:57:27.000000 academic_tracker-1.0.5/src/academic_tracker/user_input_checking.py
+-rw-rw-rw-   0        0        0    13468 2023-06-30 15:48:36.000000 academic_tracker-1.0.5/src/academic_tracker/webio.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.527109 academic_tracker-1.0.5/src/academic_tracker.egg-info/
+-rw-rw-rw-   0        0        0     9823 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6582 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      215 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 13:06:23.000000 academic_tracker-1.0.5/src/academic_tracker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.633880 academic_tracker-1.0.5/tests/
+-rw-rw-rw-   0        0        0      264 2022-04-05 15:23:06.000000 academic_tracker-1.0.5/tests/conftest.py
+-rw-rw-rw-   0        0        0    15727 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/fixtures.py
+-rw-rw-rw-   0        0        0       78 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/pytest.ini
+-rw-rw-rw-   0        0        0    12861 2023-07-07 15:00:57.000000 academic_tracker-1.0.5/tests/test_CLI.py
+-rw-rw-rw-   0        0        0    26868 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_athr_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    22066 2023-07-05 10:39:45.000000 academic_tracker-1.0.5/tests/test_athr_srch_modularized.py
+-rw-rw-rw-   0        0        0    10030 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_athr_srch_webio_no_internet.py
+-rw-rw-rw-   0        0        0     6832 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_citation_parsing.py
+-rw-rw-rw-   0        0        0    14698 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_fileio.py
+-rw-rw-rw-   0        0        0    18175 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_helper_functions.py
+-rw-rw-rw-   0        0        0    21571 2023-07-05 10:45:07.000000 academic_tracker-1.0.5/tests/test_main.py
+-rw-rw-rw-   0        0        0    13183 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_ref_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    13615 2023-07-05 11:58:19.000000 academic_tracker-1.0.5/tests/test_ref_srch_modularized.py
+-rw-rw-rw-   0        0        0    13519 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_ref_srch_webio_no_internet.py
+-rw-rw-rw-   0        0        0    41141 2023-07-05 11:22:09.000000 academic_tracker-1.0.5/tests/test_user_input_checking.py
+-rw-rw-rw-   0        0        0     7179 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/test_webio_no_internet.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:06:23.735715 academic_tracker-1.0.5/tests/testing_files/
+-rw-rw-rw-   0        0        0   248560 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/Crossref_DOI_query.json
+-rw-rw-rw-   0        0        0   665536 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/Crossref_grant_query.json
+-rw-rw-rw-   0        0        0     4068 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/Crossref_pub_dict.json
+-rw-rw-rw-   0        0        0  3516898 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/Crossref_query.json
+-rw-rw-rw-   0        0        0   348524 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ORCID_author_search_query.json
+-rw-rw-rw-   0        0        0     4463 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ORCID_pub_dict.json
+-rw-rw-rw-   0        0        0    13196 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ORCID_query.json
+-rw-rw-rw-   0        0        0    11995 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/PMID_reference.docx
+-rw-rw-rw-   0        0        0       50 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/PMID_reference.json
+-rw-rw-rw-   0        0        0       28 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/PMID_reference.txt
+-rw-rw-rw-   0        0        0      158 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/add_authors.csv
+-rw-rw-rw-   0        0        0      137 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/add_authors_missing_column.csv
+-rw-rw-rw-   0        0        0      148 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/add_authors_missing_value.csv
+-rw-rw-rw-   0        0        0     9873 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/athr_project_emails.json
+-rw-rw-rw-   0        0        0     7675 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/testing_files/athr_project_emails_tabular.json
+-rw-rw-rw-   0        0        0    19935 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/athr_srch_build_author_loop.txt
+-rw-rw-rw-   0        0        0      758 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/athr_srch_build_loop_template_string.txt
+-rw-rw-rw-   0        0        0    10266 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/athr_srch_summary_report.txt
+-rw-rw-rw-   0        0        0    53142 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/athr_srch_summary_report_custom_template.txt
+-rw-rw-rw-   0        0        0    13762 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/authors.json
+-rw-rw-rw-   0        0        0    79728 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/authors_by_project_dict_tabular.json
+-rw-rw-rw-   0        0        0    79858 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/authors_by_project_dict_truncated.json
+-rw-rw-rw-   0        0        0     2927 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/testing_files/collaborator_emails.json
+-rw-rw-rw-   0        0        0     2721 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/testing_files/collaborator_emails_tabular.json
+-rw-rw-rw-   0        0        0      520 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/config.json
+-rw-rw-rw-   0        0        0    16074 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/config_tabular.json
+-rw-rw-rw-   0        0        0    16210 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated.json
+-rw-rw-rw-   0        0        0    19318 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated_authors_adjusted.json
+-rw-rw-rw-   0        0        0    16141 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated_noCrossref.json
+-rw-rw-rw-   0        0        0    16081 2023-07-05 08:12:50.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated_noORCID.json
+-rw-rw-rw-   0        0        0    16143 2023-07-05 11:34:38.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated_noPubMed.json
+-rw-rw-rw-   0        0        0    16803 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/config_truncated_ref_srch_summary_report.json
+-rw-rw-rw-   0        0        0   127221 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/emails.json
+-rw-rw-rw-   0        0        0        0 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/empty_file.txt
+-rw-rw-rw-   0        0        0     2854 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/gen_reports_ref_summary_report.txt
+-rw-rw-rw-   0        0        0     8639 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/has_author.xml
+-rw-rw-rw-   0        0        0     8305 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/has_pubmed_grants.xml
+-rw-rw-rw-   0        0        0  1085702 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/medline.txt
+-rw-rw-rw-   0        0        0   221143 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/myncbi_webpages.json
+-rw-rw-rw-   0        0        0    22898 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/no_author.xml
+-rw-rw-rw-   0        0        0    26743 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/nsf_award_page.txt
+-rw-rw-rw-   0        0        0     1261 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/parse_citations_test.txt
+-rw-rw-rw-   0        0        0      521 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/project_report.txt
+-rw-rw-rw-   0        0        0    15412 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/pub_with_PMCID.xml
+-rw-rw-rw-   0        0        0   376657 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/publication_dict.json
+-rw-rw-rw-   0        0        0    11488 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/publication_dict_truncated.json
+-rw-rw-rw-   0        0        0    15743 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/pubs_by_author_dict.json
+-rw-rw-rw-   0        0        0     1245 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/pubs_by_author_dict_truncated.json
+-rw-rw-rw-   0        0        0  1111833 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/pymed_pubs.pkl
+-rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_Crossref_keys_for_citations.json
+-rw-rw-rw-   0        0        0     1916 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_Crossref_pub_dict.json
+-rw-rw-rw-   0        0        0   278548 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_Crossref_queries.json
+-rw-rw-rw-   0        0        0    32553 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_PubMed_pubs.json
+-rw-rw-rw-   0        0        0     2993 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_gen_reports_test_pub_dict.json
+-rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_keys_for_citations.json
+-rw-rw-rw-   0        0        0     6851 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_publication_dict.json
+-rw-rw-rw-   0        0        0     1198 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_default.txt
+-rw-rw-rw-   0        0        0     4141 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular1.csv
+-rw-rw-rw-   0        0        0     2996 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular2.csv
+-rw-rw-rw-   0        0        0     4209 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular3.csv
+-rw-rw-rw-   0        0        0     6522 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular4.xlsx
+-rw-rw-rw-   0        0        0      739 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_template_string.txt
+-rw-rw-rw-   0        0        0     2239 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_test1.txt
+-rw-rw-rw-   0        0        0     1781 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/ref_srch_report_test2.txt
+-rw-rw-rw-   0        0        0    12494 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/reference_test.docx
+-rw-rw-rw-   0        0        0      751 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/reference_test.txt
+-rw-rw-rw-   0        0        0     6272 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/scholarly_DOIs.json
+-rw-rw-rw-   0        0        0     8720 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/scholarly_author_query.json
+-rw-rw-rw-   0        0        0    37686 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/scholarly_pub_dict.json
+-rw-rw-rw-   0        0        0    17630 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/scholarly_pubs.json
+-rw-rw-rw-   0        0        0   244461 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/scholarly_query.json
+-rw-rw-rw-   0        0        0       27 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/testing_csv.csv
+-rw-rw-rw-   0        0        0    11952 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/testing_docx.docx
+-rw-rw-rw-   0        0        0       14 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/testing_text.txt
+-rw-rw-rw-   0        0        0     1118 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenization_report.txt
+-rw-rw-rw-   0        0        0   182317 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_MEDLINE.json
+-rw-rw-rw-   0        0        0   115779 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_citations.json
+-rw-rw-rw-   0        0        0    86779 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_citations_duplicates_removed.json
+-rw-rw-rw-   0        0        0     1568 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test.json
+-rw-rw-rw-   0        0        0     2225 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test2.json
+-rw-rw-rw-   0        0        0     1170 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test_empty.json
+-rw-rw-rw-   0        0        0    44981 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_myncbi_page1.json
+-rw-rw-rw-   0        0        0    34674 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_nsf_award_page.json
+-rw-rw-rw-   0        0        0     3970 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_parsing_test.json
+-rw-rw-rw-   0        0        0     2659 2022-03-08 11:18:32.000000 academic_tracker-1.0.5/tests/testing_files/tokenized_ref_test.json
```

### Comparing `academic_tracker-1.0.4/.github/workflows/build.yml` & `academic_tracker-1.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/.github/workflows/build_documentation.yml` & `academic_tracker-1.0.5/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/.github/workflows/codecov.yml` & `academic_tracker-1.0.5/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/CITATION.cff` & `academic_tracker-1.0.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/LICENSE` & `academic_tracker-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/PKG-INFO` & `academic_tracker-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: academic_tracker
-Version: 1.0.4
+Version: 1.0.5
 Summary: Find publications on PubMed, Crossref, ORCID, and Google Scholar for given authors or references.
 Home-page: https://github.com/MoseleyBioinformaticsLab/academic_tracker
 Author: Travis Thompson
 Author-email: ptth222@gmail.com
 License: BSD
 Keywords: PubMed publications citations Crossref ORCID Google Scholar
 Platform: any
```

### Comparing `academic_tracker-1.0.4/README.rst` & `academic_tracker-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/Makefile` & `academic_tracker-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/api.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/guide.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/guide.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/index.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/jsonschema.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/jsonschema.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/reporting.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/reporting.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/todo.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/todo.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/tokenization.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/tokenization.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_sources/tutorial.rst.txt` & `academic_tracker-1.0.5/docs/_build/html/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `academic_tracker-1.0.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/api.rst` & `academic_tracker-1.0.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/conf.py` & `academic_tracker-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/guide.rst` & `academic_tracker-1.0.5/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/index.rst` & `academic_tracker-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/jsonschema.rst` & `academic_tracker-1.0.5/docs/jsonschema.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/make.bat` & `academic_tracker-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/reporting.rst` & `academic_tracker-1.0.5/docs/reporting.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/todo.rst` & `academic_tracker-1.0.5/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/tokenization.rst` & `academic_tracker-1.0.5/docs/tokenization.rst`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/docs/tutorial.rst` & `academic_tracker-1.0.5/docs/tutorial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Configuration JSON File
 ~~~~~~~~~~~~~~~~~~~~~~~
 Details about the configuration JSON file can be found in the :doc:`jsonschema` 
 section, but in general the sections of the configuration JSON file that aren't 
 needed for a particular command are not required. For instance, the ORCID_search 
 section is not required for reference_search since it does not search ORCID. The 
-same is true if the --no_ORCID option is used.
+same is true if the --no-ORCID option is used.
 
 Outputs
 ~~~~~~~
 The specific files output by Academic Tracker vary by the command used and some 
 options, but each command always creates a new timestamped directory in the working 
 directory. If the --test option is not used then the directory will be named 
 tracker-YYMMDDHHMM. If the --test option is used then the directory will be named 
@@ -23,30 +23,30 @@
 
 Search For Publications By Author
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --no_PubMed --verbose --silent]
+    academic_tracker author_search <config_json_file> [--test --prev-pub=<file-path> --no-GoogleScholar --no-ORCID --no-Crossref --no-PubMed --verbose --silent]
 
 
 Description
 -----------
 For each author in the Authors section of the configuration JSON file search 
 PubMed, ORCID, Crossref, and Google Scholar for publications they are an author 
 on. The cutoff_year attribute for either the projects or the authors can be used 
 to filter the publications to only those in that year or after. 
 
 Similarly, a previous publications JSON file can be used to filter out publications 
-that are already in the file. This file can be specified manually with the --prev_pub 
+that are already in the file. This file can be specified manually with the --prev-pub 
 option. If not specified manually author_search will automatically look for a 
 publications.json file in the most recent tracker directories and if it finds 
 one it will be used as the previous publications. To stop this automatic lookup 
-enter "ignore" for the --prev_pub option. The output publications.json file will 
+enter "ignore" for the --prev-pub option. The output publications.json file will 
 be a combination of the previous publications and any new publications found. To 
 be clear the new publications.json file will be the previous publications.json 
 file with any new entries added in. 
 
 The description of everything author_search does with the previous publications 
 may seem arbitrary and confusing. The idea is that users will make an initial 
 list of authors to keep track of and then run author_search every so often to 
@@ -68,33 +68,33 @@
 Options
 -------
 --test: 
 
 The test option changes the name of the output directory from tracker-YYMMDDHHMM 
 to tracker-test-YYMMDDHHMM and prevents any emails from being sent.
 
---prev_pub: 
+--prev-pub: 
 
 Specifies a publications.json file to use as a list of publications to ignore 
 when searching for new publications. Set to "ignore" to prevent author_search 
 from automatically looking for a publications.json file in tracker directories.
             
---no_GoogleScholar: 
+--no-GoogleScholar: 
 
 If used author_search will not search Google Scholar for publications.
 
---no_ORCID: 
+--no-ORCID: 
 
 If used author_search will not search ORCID for publications.
 
---no_Crossref: 
+--no-Crossref: 
 
 If used author_search will not search Crossref for publications.
 
---no_PubMed: 
+--no-PubMed: 
 
 If used author_search will not search PubMed for publications. This option is 
 assumed if the PubMed_search section of the configuration JSON file is missing.
 
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
@@ -278,15 +278,15 @@
     Success. Publications and reports saved in tracker-test-2202020140
 
 
 Designating a previous publications filepath instead of letting Academic Tracker find the most recent.
 
 .. code-block:: console
     
-    >academic_tracker author_search config_file.json --prev_pub prev_pub_file_path.json
+    >academic_tracker author_search config_file.json --prev-pub prev_pub_file_path.json
     Finding author's publications. This could take a while.
     Searching PubMed.
     Searching ORCID.
     Searching Google Scholar.
     Searching Crossref.
     Success. Publications and reports saved in tracker-2202020140
     
@@ -341,15 +341,15 @@
 
     A minimal example is shown, but the config can have other sections and run without error.
 
 Console:
 
 .. code-block:: console
     
-    >academic_tracker author_search config_file.json --no_ORCID
+    >academic_tracker author_search config_file.json --no-ORCID
     Finding author's publications. This could take a while.
     Searching PubMed.
     Searching Google Scholar.
     Searching Crossref.
     Success. Publications and reports saved in tracker-2202020140
 
 
@@ -357,15 +357,15 @@
 
 Search For Publications By Reference
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --no_PubMed --verbose --silent]
+    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev-pub=<file-path> --PMID-reference --MEDLINE-reference --no-Crossref --no-PubMed --verbose --silent]
 
 
 Description
 -----------
 Parse and tokenize the reference file or URL and then search PubMed and Crossref 
 for the publications found. ORCID is not searched because it is a database of 
 authors and does not support searching for publications directly. Google Scholar 
@@ -376,29 +376,29 @@
 it can be a JSON file of already tokenized data, a docx file, or a txt file. If 
 not a JSON file then each reference is expected to be on a single line. If it is 
 a URL then it can be either a MyNCBI URL or not. If it is a MyNCBI URL then it 
 is expected to be the first page of a bibliography and will be tokenized in a 
 specific way. All other URLs are simply read as a text file and tokenized like 
 one.
 
-The --PMID_reference and --MEDLINE_reference options change how the reference file 
-is interpreted. If the --PMID_reference option is used then it indicates that the 
+The --PMID-reference and --MEDLINE-reference options change how the reference file 
+is interpreted. If the --PMID-reference option is used then it indicates that the 
 given reference file is a list of PMIDs (PubMed's unique IDs). Instead of tokenizing 
 this file it is assumed that each line is a PMID so PubMed will be queried for 
 each PMID and Crossref will not be queried. The idea for this option was to be 
 able to quickly grab information from PubMed. 
 
-The --MEDLINE_reference option indicates that given reference file is a MEDLINE_ 
+The --MEDLINE-reference option indicates that given reference file is a MEDLINE_ 
 formatted file. This will be tokenized in a unique way since the publication 
 information is spread out over multiple lines in this format. This format is 
 supported because it is a dounload option on MyNCBI bibliography pages.
 
 Details about tokenization are in the :doc:`tokenization` section.
 
-The --prev_pub option is different for reference_search than it is for author_search. 
+The --prev-pub option is different for reference_search than it is for author_search. 
 First, reference_search does not automatically look for a publicaitons.json file 
 to use since the same assumptions as described for author_search do not hold here. 
 Second, publications in the prev_pub file are not used to ignore publications. 
 Publications in the prev_pub file will still be in the newly created publications.json 
 file. What this option does do is set the <is_in_comparison_file> keyword to True 
 for matching publications in the summary report.
 
@@ -406,33 +406,33 @@
 Options
 -------
 --test: 
 
 The test option changes the name of the output directory from tracker-YYMMDDHHMM 
 to tracker-test-YYMMDDHHMM and prevents any emails from being sent.
 
---prev_pub: 
+--prev-pub: 
 
 Specifies a publications.json file to use as a list of publications to compare 
 with when generating the summary report.
             
---PMID_reference: 
+--PMID-reference: 
 
 Specifies that the reference file is a list of PMIDs and to only return 
 information from PubMed.
                   
---MEDLINE_reference: 
+--MEDLINE-reference: 
 
 Specifies that the reference file is a MEDLINE_ formatted file.
             
---no_Crossref: 
+--no-Crossref: 
 
 If used reference_search will not search Crossref for publications.
 
---no_PubMed: 
+--no-PubMed: 
 
 If used reference_search will not search Crossref for publications. This option 
 is assumed if the PubMed_search section of the configuration JSON file is missing.
 
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
@@ -452,15 +452,15 @@
 
 An emails.json file is only created if the from_email attribute is given in 
 the summary_report section of the configuration JSON file. 
 
 A summary_report.txt file is only created if the summary_report attribute is in 
 the configuration JSON file. 
 
-If --PMID_reference is used no reports or emails are generated.
+If --PMID-reference is used no reports or emails are generated.
 
 Details about reports can be found in the :doc:`reporting` section.
 
 publications.json
 tokenized_reference.json
 emails.json
 summary_report.txt
@@ -510,15 +510,15 @@
     Success. Publications and reports saved in tracker-test-2202020140
 
 
 Designating a previous publications filepath.
 
 .. code-block:: console
     
-    >academic_tracker reference_search config_file.json reference_file.txt --prev_pub prev_pub_file_path.json
+    >academic_tracker reference_search config_file.json reference_file.txt --prev-pub prev_pub_file_path.json
     Finding publications. This could take a while. 
     Searching PubMed.
     Searching Crossref.
     Success. Publications and reports saved in tracker-2202020140
     
     
 Specifying that Academic Tracker shouldn't use Crossref.
@@ -538,15 +538,15 @@
 
     A minimal example is shown, but the config can have other sections and run without error.
 
 Console:
 
 .. code-block:: console
     
-    >academic_tracker reference_search config_file.json reference_file.txt --no_Crossref
+    >academic_tracker reference_search config_file.json reference_file.txt --no-Crossref
     Finding publications. This could take a while. 
     Searching PubMed.
     Success. Publications and reports saved in tracker-2202020140
 
 
 
 
@@ -813,25 +813,25 @@
 
 Tokenize A Reference
 ~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker tokenize_reference <references_file_or_URL> [--MEDLINE_reference --verbose --silent]
+    academic_tracker tokenize_reference <references_file_or_URL> [--MEDLINE-reference --verbose --silent]
 
 
 Description
 -----------
 Tokenize the input reference and output a tokenization report and JSON file.
 
 
 Options
 -------
---MEDLINE_reference: 
+--MEDLINE-reference: 
 
 Specifies that the reference file is a MEDLINE_ formatted file.
 
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
 
@@ -989,15 +989,15 @@
 
 Generate Reports And Emails Like Reference Search
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker gen_reports_and_emails_ref <config_json_file> <references_file_or_URL> <publication_json_file> [--test --prev_pub=<file-path> --MEDLINE_reference --verbose --silent]
+    academic_tracker gen_reports_and_emails_ref <config_json_file> <references_file_or_URL> <publication_json_file> [--test --prev-pub=<file-path> --MEDLINE-reference --verbose --silent]
 
 
 Description
 -----------
 Create reports and emails and send emails just like reference_search would if it 
 had found the publications in the given publications JSON file. The idea behind 
 this command is to give the user the ability to play with the reporting system 
@@ -1026,20 +1026,20 @@
 Options
 -------
 --test: 
 
 The test option changes the name of the output directory from tracker-YYMMDDHHMM 
 to tracker-test-YYMMDDHHMM and prevents any emails from being sent.
         
---prev_pub: 
+--prev-pub: 
 
 Specifies a publications.json file to use as a list of publications to compare 
 with when generating the summary report.
             
---MEDLINE_reference: 
+--MEDLINE-reference: 
 
 Specifies that the reference file is a MEDLINE_ formatted file.
         
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
```

### Comparing `academic_tracker-1.0.4/example_configs/many_projects_and_authors_project_and_summary_reports_no_duplicates__full_example.json` & `academic_tracker-1.0.5/example_configs/many_projects_and_authors_project_and_summary_reports_no_duplicates__full_example.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__full_example.json` & `academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports__full_example.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__template.json` & `academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports__template.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports_no_duplicates__template.json` & `academic_tracker-1.0.5/example_configs/many_projects_and_authors_with_summary_reports_no_duplicates__template.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/setup.py` & `academic_tracker-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/__init__.py` & `academic_tracker-1.0.5/src/academic_tracker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 ``helper_functions``
     This module contains functions that help the other modules function. The functions do things such as fuzzy matching, regex searching, and printing.
         
 ``webio``
     This module contains general functions for interfacing with the internet.
 
 """
-__version__ = "1.0.4"
+__version__ = "1.0.5"
```

### Comparing `academic_tracker-1.0.4/src/academic_tracker/__main__.py` & `academic_tracker-1.0.5/src/academic_tracker/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,59 @@
 """
 Usage:
-    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --no_PubMed --verbose --silent]
-    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --no_PubMed --verbose --silent]
+    academic_tracker author_search <config_json_file> [--test] 
+                                                      [--prev_pub=<file-path> --prev-pub=<file-path>] 
+                                                      [--no-GoogleScholar --no_GoogleScholar] 
+                                                      [--no-ORCID --no_ORCID] 
+                                                      [--no-Crossref --no_Crossref] 
+                                                      [--no-PubMed --no_PubMed]
+                                                      [--verbose --silent]
+    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test] 
+                                                                                  [--prev-pub=<file-path> --prev_pub=<file-path>]
+                                                                                  [--PMID-reference --PMID_reference]
+                                                                                  [--MEDLINE-reference --MEDLINE_reference]
+                                                                                  [--no-Crossref --no_Crossref]
+                                                                                  [--no-PubMed --no_PubMed]
+                                                                                  [--verbose --silent]
     academic_tracker find_ORCID <config_json_file> [--verbose --silent]
     academic_tracker find_Google_Scholar <config_json_file> [--verbose --silent]
     academic_tracker add_authors <config_json_file> <authors_file> [--verbose --silent]
-    academic_tracker tokenize_reference <references_file_or_URL> [--MEDLINE_reference --verbose --silent]
+    academic_tracker tokenize_reference <references_file_or_URL> [--MEDLINE-reference --MEDLINE_reference]
+                                                                 [--verbose --silent]
     academic_tracker gen_reports_and_emails_auth <config_json_file> <publication_json_file> [--test --verbose --silent]
-    academic_tracker gen_reports_and_emails_ref <config_json_file> <references_file_or_URL> <publication_json_file> [--test --prev_pub=<file-path> --MEDLINE_reference --verbose --silent]
+    academic_tracker gen_reports_and_emails_ref <config_json_file> <references_file_or_URL> <publication_json_file> [--test]
+                                                                                                                    [--prev-pub=<file-path> --prev_pub=<file-path>]
+                                                                                                                    [--MEDLINE-reference --MEDLINE_reference]
+                                                                                                                    [--verbose --silent]
     
 Options:
     -h --help                         Show this screen.
     -v --version                      Show version.
     --verbose                         Print hidden error messages.
     --silent                          Do not print anything to the screen.
     --test                            Generate pubs and email texts, but do not send emails.
-    --prev_pub=<file-path>            Filepath to json or csv with publication ids to ignore. Enter "ignore" for the <file_path> to not look for previous publications.json files in tracker directories.
+    --prev-pub=<file-path>            Filepath to json or csv with publication ids to ignore. 
+                                      Enter "ignore" for the <file_path> to not look for previous publications.json files in tracker directories.
+    --prev_pub=<file-path>            Deprecated. Use --prev-pub instead.
     
 Reference Type Options:    
-    --PMID_reference                  Indicates that the reference_file is a PMID file and only PubMed info will be returned.
-    --MEDLINE_reference               Indicates that the reference_file is a MEDLINE file.
+    --PMID-reference                  Indicates that the reference_file is a PMID file and only PubMed info will be returned.
+    --PMID_reference                  Deprecated. Use --PMID-reference instead.
+    --MEDLINE-reference               Indicates that the reference_file is a MEDLINE file.
+    --MEDLINE_reference               Deprecated. Use --MEDLINE-reference instead.
 
 Search Options:
-    --no_GoogleScholar                Don't search Google Scholar.
-    --no_ORCID                        Don't search ORCID.
-    --no_Crossref                     Don't search Crossref.
-    --no_PubMed                       Don't search PubMed.
+    --no-GoogleScholar                Don't search Google Scholar.
+    --no_GoogleScholar                Deprecated. Use --no-GoogleScholar instead.
+    --no-ORCID                        Don't search ORCID.
+    --no_ORCID                        Deprecated. Use --no-ORCID instead.
+    --no-Crossref                     Don't search Crossref.
+    --no_Crossref                     Deprecated. Use --no-Crossref instead.
+    --no-PubMed                       Don't search PubMed.
+    --no_PubMed                       Deprecated. Use --no-PubMed instead.
 """
 
 
 import re
 import os
 import datetime
 import sys
@@ -53,50 +77,68 @@
 
 
 VERBOSE = True
 SILENT = False
 
 def main():
     
+    ## Have to modify the doc string so docopt can recognize more options than what is written.
+    # options_to_alias = ["--no-PubMed", "--no-ORCID", "--no-Crossref", "--no-GoogleScholar", "--PMID-reference", "--MEDLINE-reference", "--prev-pub"]
+    # for option in options_to_alias:
+    #     alias = f"--{option[2:].replace('-', '_')}"
+    #     doc = __doc__.replace("option", f"{option} {alias}")
+        
+    # args = docopt.docopt(doc, version=str("Academic Tracker ") + __version__)
+    
     args = docopt.docopt(__doc__, version=str("Academic Tracker ") + __version__)
     
     user_input_checking.cli_inputs_check(args)
     
     global VERBOSE
     VERBOSE = args["--verbose"]
     global SILENT
     SILENT = args["--silent"]
     
     if len(sys.argv) > 1 and sys.argv[1] == "author_search":
-        author_search(args["<config_json_file>"], args["--no_ORCID"], 
-                      args["--no_GoogleScholar"], args["--no_Crossref"],
-                      args["--no_PubMed"],
-                      args["--test"], args["--prev_pub"])
+        author_search(args["<config_json_file>"], 
+                      args["--no_ORCID"] or args["--no-ORCID"], 
+                      args["--no_GoogleScholar"] or args["--no-GoogleScholar"], 
+                      args["--no_Crossref"] or args["--no-Crossref"],
+                      args["--no_PubMed"] or args["--no-PubMed"],
+                      args["--test"], 
+                      args["--prev-pub"] if args["--prev-pub"] else args["--prev_pub"])
     elif len(sys.argv) > 1 and sys.argv[1] == "reference_search":
-        if args["--PMID_reference"]:
+        if args["--PMID_reference"] or args["--PMID-reference"]:
             PMID_reference(args["<config_json_file>"], args["<references_file_or_URL>"], args["--test"])
         else:
-            reference_search(args["<config_json_file>"], args["<references_file_or_URL>"], 
-                             args["--MEDLINE_reference"], args["--no_Crossref"], 
-                             args["--no_PubMed"],
-                             args["--test"], args["--prev_pub"])
+            reference_search(args["<config_json_file>"], 
+                             args["<references_file_or_URL>"], 
+                             args["--MEDLINE_reference"] or args["--MEDLINE-reference"], 
+                             args["--no_Crossref"] or args["--no-Crossref"], 
+                             args["--no_PubMed"] or args["--no-PubMed"],
+                             args["--test"], 
+                             args["--prev-pub"] if args["--prev-pub"] else args["--prev_pub"])
     elif len(sys.argv) > 1 and sys.argv[1] == "find_ORCID":
         find_ORCID(args["<config_json_file>"])
     elif len(sys.argv) > 1 and sys.argv[1] == "find_Google_Scholar":
         find_Google_Scholar(args["<config_json_file>"])
     elif len(sys.argv) > 1 and sys.argv[1] == "add_authors":
         add_authors(args["<config_json_file>"], args["<authors_file>"])
     elif len(sys.argv) > 1 and sys.argv[1] == "tokenize_reference":
-        tokenize_reference(args["<references_file_or_URL>"], args["--MEDLINE_reference"])
+        tokenize_reference(args["<references_file_or_URL>"], 
+                           args["--MEDLINE_reference"] or args["--MEDLINE-reference"])
     elif len(sys.argv) > 1 and sys.argv[1] == "gen_reports_and_emails_auth":
         gen_reports_and_emails_auth(args["<config_json_file>"], args["<publication_json_file>"], args["--test"])
     elif len(sys.argv) > 1 and sys.argv[1] == "gen_reports_and_emails_ref":
-        gen_reports_and_emails_ref(args["<config_json_file>"], args["<references_file_or_URL>"], 
-                                   args["<publication_json_file>"], args["--MEDLINE_reference"], 
-                                   args["--test"], args["--prev_pub"])
+        gen_reports_and_emails_ref(args["<config_json_file>"], 
+                                   args["<references_file_or_URL>"], 
+                                   args["<publication_json_file>"], 
+                                   args["--MEDLINE_reference"] or args["--MEDLINE-reference"], 
+                                   args["--test"], 
+                                   args["--prev-pub"] if args["--prev-pub"] else args["--prev_pub"])
     else:
         print("Unrecognized command")  
         
 
 
 def author_search(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed, test, prev_pub_filepath):
     """Query sources for publications by author.
```

### Comparing `academic_tracker-1.0.4/src/academic_tracker/athr_srch_emails_and_reports.py` & `academic_tracker-1.0.5/src/academic_tracker/athr_srch_emails_and_reports.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/athr_srch_modularized.py` & `academic_tracker-1.0.5/src/academic_tracker/athr_srch_modularized.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/athr_srch_webio.py` & `academic_tracker-1.0.5/src/academic_tracker/athr_srch_webio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/citation_parsing.py` & `academic_tracker-1.0.5/src/academic_tracker/citation_parsing.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/fileio.py` & `academic_tracker-1.0.5/src/academic_tracker/fileio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/helper_functions.py` & `academic_tracker-1.0.5/src/academic_tracker/helper_functions.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/ref_srch_emails_and_reports.py` & `academic_tracker-1.0.5/src/academic_tracker/ref_srch_emails_and_reports.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/ref_srch_modularized.py` & `academic_tracker-1.0.5/src/academic_tracker/ref_srch_modularized.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/ref_srch_webio.py` & `academic_tracker-1.0.5/src/academic_tracker/ref_srch_webio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/tracker_schema.py` & `academic_tracker-1.0.5/src/academic_tracker/tracker_schema.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/user_input_checking.py` & `academic_tracker-1.0.5/src/academic_tracker/user_input_checking.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker/webio.py` & `academic_tracker-1.0.5/src/academic_tracker/webio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/src/academic_tracker.egg-info/PKG-INFO` & `academic_tracker-1.0.5/src/academic_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: academic-tracker
-Version: 1.0.4
+Version: 1.0.5
 Summary: Find publications on PubMed, Crossref, ORCID, and Google Scholar for given authors or references.
 Home-page: https://github.com/MoseleyBioinformaticsLab/academic_tracker
 Author: Travis Thompson
 Author-email: ptth222@gmail.com
 License: BSD
 Keywords: PubMed publications citations Crossref ORCID Google Scholar
 Platform: any
```

### Comparing `academic_tracker-1.0.4/src/academic_tracker.egg-info/SOURCES.txt` & `academic_tracker-1.0.5/src/academic_tracker.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 src/academic_tracker.egg-info/dependency_links.txt
 src/academic_tracker.egg-info/entry_points.txt
 src/academic_tracker.egg-info/requires.txt
 src/academic_tracker.egg-info/top_level.txt
 tests/conftest.py
 tests/fixtures.py
 tests/pytest.ini
+tests/test_CLI.py
 tests/test_athr_srch_emails_and_reports.py
 tests/test_athr_srch_modularized.py
 tests/test_athr_srch_webio_no_internet.py
 tests/test_citation_parsing.py
 tests/test_fileio.py
 tests/test_helper_functions.py
 tests/test_main.py
```

### Comparing `academic_tracker-1.0.4/tests/fixtures.py` & `academic_tracker-1.0.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_athr_srch_emails_and_reports.py` & `academic_tracker-1.0.5/tests/test_athr_srch_emails_and_reports.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_athr_srch_modularized.py` & `academic_tracker-1.0.5/tests/test_athr_srch_modularized.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_athr_srch_webio_no_internet.py` & `academic_tracker-1.0.5/tests/test_athr_srch_webio_no_internet.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_citation_parsing.py` & `academic_tracker-1.0.5/tests/test_citation_parsing.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_fileio.py` & `academic_tracker-1.0.5/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_helper_functions.py` & `academic_tracker-1.0.5/tests/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_main.py` & `academic_tracker-1.0.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_ref_srch_emails_and_reports.py` & `academic_tracker-1.0.5/tests/test_ref_srch_emails_and_reports.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_ref_srch_modularized.py` & `academic_tracker-1.0.5/tests/test_ref_srch_modularized.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_ref_srch_webio_no_internet.py` & `academic_tracker-1.0.5/tests/test_ref_srch_webio_no_internet.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_user_input_checking.py` & `academic_tracker-1.0.5/tests/test_user_input_checking.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/test_webio_no_internet.py` & `academic_tracker-1.0.5/tests/test_webio_no_internet.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/Crossref_DOI_query.json` & `academic_tracker-1.0.5/tests/testing_files/Crossref_DOI_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/Crossref_grant_query.json` & `academic_tracker-1.0.5/tests/testing_files/Crossref_grant_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/Crossref_pub_dict.json` & `academic_tracker-1.0.5/tests/testing_files/Crossref_pub_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/Crossref_query.json` & `academic_tracker-1.0.5/tests/testing_files/Crossref_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ORCID_author_search_query.json` & `academic_tracker-1.0.5/tests/testing_files/ORCID_author_search_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ORCID_pub_dict.json` & `academic_tracker-1.0.5/tests/testing_files/ORCID_pub_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ORCID_query.json` & `academic_tracker-1.0.5/tests/testing_files/ORCID_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/PMID_reference.docx` & `academic_tracker-1.0.5/tests/testing_files/PMID_reference.docx`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_project_emails.json` & `academic_tracker-1.0.5/tests/testing_files/athr_project_emails.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_project_emails_tabular.json` & `academic_tracker-1.0.5/tests/testing_files/athr_project_emails_tabular.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_srch_build_author_loop.txt` & `academic_tracker-1.0.5/tests/testing_files/athr_srch_build_author_loop.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_srch_build_loop_template_string.txt` & `academic_tracker-1.0.5/tests/testing_files/athr_srch_build_loop_template_string.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report.txt` & `academic_tracker-1.0.5/tests/testing_files/athr_srch_summary_report.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report_custom_template.txt` & `academic_tracker-1.0.5/tests/testing_files/athr_srch_summary_report_custom_template.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/authors.json` & `academic_tracker-1.0.5/tests/testing_files/authors.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_tabular.json` & `academic_tracker-1.0.5/tests/testing_files/authors_by_project_dict_tabular.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_truncated.json` & `academic_tracker-1.0.5/tests/testing_files/authors_by_project_dict_truncated.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/collaborator_emails.json` & `academic_tracker-1.0.5/tests/testing_files/collaborator_emails.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/collaborator_emails_tabular.json` & `academic_tracker-1.0.5/tests/testing_files/collaborator_emails_tabular.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config.json` & `academic_tracker-1.0.5/tests/testing_files/config.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_tabular.json` & `academic_tracker-1.0.5/tests/testing_files/config_tabular.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated_authors_adjusted.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated_authors_adjusted.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated_noCrossref.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated_noCrossref.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated_noORCID.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated_noORCID.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated_noPubMed.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated_noPubMed.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/config_truncated_ref_srch_summary_report.json` & `academic_tracker-1.0.5/tests/testing_files/config_truncated_ref_srch_summary_report.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/emails.json` & `academic_tracker-1.0.5/tests/testing_files/emails.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/gen_reports_ref_summary_report.txt` & `academic_tracker-1.0.5/tests/testing_files/gen_reports_ref_summary_report.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/has_author.xml` & `academic_tracker-1.0.5/tests/testing_files/has_author.xml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/has_pubmed_grants.xml` & `academic_tracker-1.0.5/tests/testing_files/has_pubmed_grants.xml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/medline.txt` & `academic_tracker-1.0.5/tests/testing_files/medline.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/myncbi_webpages.json` & `academic_tracker-1.0.5/tests/testing_files/myncbi_webpages.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/no_author.xml` & `academic_tracker-1.0.5/tests/testing_files/no_author.xml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/nsf_award_page.txt` & `academic_tracker-1.0.5/tests/testing_files/nsf_award_page.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/parse_citations_test.txt` & `academic_tracker-1.0.5/tests/testing_files/parse_citations_test.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/project_report.txt` & `academic_tracker-1.0.5/tests/testing_files/project_report.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/pub_with_PMCID.xml` & `academic_tracker-1.0.5/tests/testing_files/pub_with_PMCID.xml`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/publication_dict.json` & `academic_tracker-1.0.5/tests/testing_files/publication_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/publication_dict_truncated.json` & `academic_tracker-1.0.5/tests/testing_files/publication_dict_truncated.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict.json` & `academic_tracker-1.0.5/tests/testing_files/pubs_by_author_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict_truncated.json` & `academic_tracker-1.0.5/tests/testing_files/pubs_by_author_dict_truncated.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/pymed_pubs.pkl` & `academic_tracker-1.0.5/tests/testing_files/pymed_pubs.pkl`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_pub_dict.json` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_Crossref_pub_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_queries.json` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_Crossref_queries.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_PubMed_pubs.json` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_PubMed_pubs.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_gen_reports_test_pub_dict.json` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_gen_reports_test_pub_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_publication_dict.json` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_publication_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_default.txt` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_default.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular1.csv` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular1.csv`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular2.csv` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular2.csv`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular3.csv` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular3.csv`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular4.xlsx` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_tabular4.xlsx`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_template_string.txt` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_template_string.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test1.txt` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_test1.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test2.txt` & `academic_tracker-1.0.5/tests/testing_files/ref_srch_report_test2.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/reference_test.docx` & `academic_tracker-1.0.5/tests/testing_files/reference_test.docx`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/reference_test.txt` & `academic_tracker-1.0.5/tests/testing_files/reference_test.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/scholarly_DOIs.json` & `academic_tracker-1.0.5/tests/testing_files/scholarly_DOIs.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/scholarly_author_query.json` & `academic_tracker-1.0.5/tests/testing_files/scholarly_author_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/scholarly_pub_dict.json` & `academic_tracker-1.0.5/tests/testing_files/scholarly_pub_dict.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/scholarly_pubs.json` & `academic_tracker-1.0.5/tests/testing_files/scholarly_pubs.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/scholarly_query.json` & `academic_tracker-1.0.5/tests/testing_files/scholarly_query.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/testing_docx.docx` & `academic_tracker-1.0.5/tests/testing_files/testing_docx.docx`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenization_report.txt` & `academic_tracker-1.0.5/tests/testing_files/tokenization_report.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_MEDLINE.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_MEDLINE.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_citations.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_citations.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_citations_duplicates_removed.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_citations_duplicates_removed.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test2.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test2.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test_empty.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_citations_for_report_test_empty.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_myncbi_page1.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_myncbi_page1.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_nsf_award_page.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_nsf_award_page.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_parsing_test.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_parsing_test.json`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.4/tests/testing_files/tokenized_ref_test.json` & `academic_tracker-1.0.5/tests/testing_files/tokenized_ref_test.json`

 * *Files identical despite different names*

