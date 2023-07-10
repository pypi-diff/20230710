# Comparing `tmp/troubadix-23.6.3.tar.gz` & `tmp/troubadix-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.6.3.tar", max compression
+gzip compressed data, was "troubadix-23.7.0.tar", max compression
```

## Comparing `troubadix-23.6.3.tar` & `troubadix-23.7.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    35149 2023-06-29 07:15:50.444448 troubadix-23.6.3/LICENSE
--rw-r--r--   0        0        0     2730 2023-06-29 07:15:50.444448 troubadix-23.6.3/README.md
--rw-r--r--   0        0        0     2516 2023-06-29 07:15:50.448448 troubadix-23.6.3/pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2450 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     6010 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   125168 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     4507 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8566 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4043 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2172 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9557 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/troubadix.py
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 08:28:45.946539 troubadix-23.7.0/LICENSE
+-rw-r--r--   0        0        0     2730 2023-07-10 08:28:45.946539 troubadix-23.7.0/README.md
+-rw-r--r--   0        0        0     2516 2023-07-10 08:28:45.946539 troubadix-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2450 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   125216 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4507 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8566 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3790 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4081 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9557 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.7.0/PKG-INFO
```

### Comparing `troubadix-23.6.3/LICENSE` & `troubadix-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/README.md` & `troubadix-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/pyproject.toml` & `troubadix-23.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.6.3"
+version = "23.7.0"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.6.3/tests/__init__.py` & `troubadix-23.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/helper/__init__.py` & `troubadix-23.7.0/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.7.0/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/helper/test_patterns.py` & `troubadix-23.7.0/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/__init__.py` & `troubadix-23.7.0/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/fail.nasl` & `troubadix-23.7.0/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/fail2.nasl` & `troubadix-23.7.0/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test.nasl` & `troubadix-23.7.0/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_badwords.py` & `troubadix-23.7.0/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_copyright_text.py` & `troubadix-23.7.0/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_copyright_year.py` & `troubadix-23.7.0/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_creation_date.py` & `troubadix-23.7.0/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_cve_format.py` & `troubadix-23.7.0/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_cvss_format.py` & `troubadix-23.7.0/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_dependencies.py` & `troubadix-23.7.0/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_dependency_category_order.py` & `troubadix-23.7.0/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.7.0/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_deprecated_functions.py` & `troubadix-23.7.0/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_double_end_points.py` & `troubadix-23.7.0/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_duplicate_oid.py` & `troubadix-23.7.0/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.7.0/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_encoding.py` & `troubadix-23.7.0/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.7.0/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.7.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.7.0/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.7.0/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.7.0/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.7.0/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.7.0/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.7.0/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.7.0/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_grammar.py` & `troubadix-23.7.0/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.7.0/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_illegal_characters.py` & `troubadix-23.7.0/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_log_messages.py` & `troubadix-23.7.0/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.7.0/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.7.0/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.7.0/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.7.0/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_newlines.py` & `troubadix-23.7.0/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.7.0/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.7.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_qod.py` & `troubadix-23.7.0/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_reporting_consistency.py` & `troubadix-23.7.0/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.7.0/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.7.0/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.7.0/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_category.py` & `troubadix-23.7.0/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_copyright.py` & `troubadix-23.7.0/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_family.py` & `troubadix-23.7.0/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_tag_form.py` & `troubadix-23.7.0/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.7.0/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.7.0/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.7.0/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_xref_form.py` & `troubadix-23.7.0/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_script_xref_url.py` & `troubadix-23.7.0/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_security_messages.py` & `troubadix-23.7.0/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.7.0/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_solution_text.py` & `troubadix-23.7.0/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_solution_type.py` & `troubadix-23.7.0/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_spelling.py` & `troubadix-23.7.0/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_tabs.py` & `troubadix-23.7.0/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_todo_tbd.py` & `troubadix-23.7.0/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.7.0/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_using_display.py` & `troubadix-23.7.0/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_valid_oid.py` & `troubadix-23.7.0/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.7.0/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.7.0/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/plugins/test_vt_placement.py` & `troubadix-23.7.0/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/__init__.py` & `troubadix-23.7.0/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.7.0/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.7.0/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.7.0/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.7.0/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.7.0/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_argparser.py` & `troubadix-23.7.0/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_helper.py` & `troubadix-23.7.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_naslinter.py` & `troubadix-23.7.0/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_reporter.py` & `troubadix-23.7.0/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_results.py` & `troubadix-23.7.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/tests/test_runner.py` & `troubadix-23.7.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/__init__.py` & `troubadix-23.7.0/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/argparser.py` & `troubadix-23.7.0/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/codespell/codespell.exclude` & `troubadix-23.7.0/troubadix/codespell/codespell.exclude`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 Add more important informations
  * Add suppor... [Please see the references for more information on the vulnerabilities]");
   a denial of service. (CVE-2016-4429) Tim Ruehsen discovered that the
   - A division by zero in the CAF demuxer
 "admin:admin:huawei,3com,allied,alteon,amitech,billon,checkpoint,cisco,com3,davox,dlink,draytek,dynalink,everfocus,flowpoint,foundry networks,hp:all,ftp",
   Admin endpoints to a public WAN (Internet) / public LAN without authentication.
 "Administrator:admin:cisco,conexant,corecess,gvc:all",
+  # admin:<redacted>:0:0:Adminstrator:/:/bin/sh
 "Admin|shs",
 "Adminstrator|",
 "adminstrator|changeme",
 "ADMN|admn",
 # ADSL Router, VxWorks SNMPv1/v2c Agent, Conexant System, Inc.
 A flaw was found in Nettle in versions before 3.7.2, where several Nettle signature verification functions (GOST DSA, EDDSA & ECDSA) result in the Elliptic Curve Cryptography point (ECC) multiply function being called with out-of-range scalers, possibly resulting in incorrect results. This flaw allows an attacker to force an invalid signature, causing an assertion failure or possible validation. The highest threat to this vulnerability is to confidentiality, integrity, as well as system availability.(CVE-2021-20305)");
 Aftandilian, and Jordi Chancel as the original reporters.");
```

### Comparing `troubadix-23.6.3/troubadix/codespell/codespell.ignore` & `troubadix-23.7.0/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/helper/__init__.py` & `troubadix-23.7.0/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/helper/helper.py` & `troubadix-23.7.0/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.7.0/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/helper/patterns.py` & `troubadix-23.7.0/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugin.py` & `troubadix-23.7.0/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/__init__.py` & `troubadix-23.7.0/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/badwords.py` & `troubadix-23.7.0/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/copyright_text.py` & `troubadix-23.7.0/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/copyright_year.py` & `troubadix-23.7.0/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/creation_date.py` & `troubadix-23.7.0/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/cve_format.py` & `troubadix-23.7.0/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/cvss_format.py` & `troubadix-23.7.0/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/dependencies.py` & `troubadix-23.7.0/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/dependency_category_order.py` & `troubadix-23.7.0/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.7.0/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/deprecated_functions.py` & `troubadix-23.7.0/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/double_end_points.py` & `troubadix-23.7.0/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/duplicate_oid.py` & `troubadix-23.7.0/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.7.0/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/encoding.py` & `troubadix-23.7.0/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.7.0/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.7.0/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/grammar.py` & `troubadix-23.7.0/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.7.0/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/illegal_characters.py` & `troubadix-23.7.0/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/log_messages.py` & `troubadix-23.7.0/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.7.0/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.7.0/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.7.0/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.7.0/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/newlines.py` & `troubadix-23.7.0/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.7.0/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.7.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/qod.py` & `troubadix-23.7.0/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/reporting_consistency.py` & `troubadix-23.7.0/troubadix/plugins/reporting_consistency.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "2015/gb_vnc_brute_force.nasl",
     "2012/gb_secpod_ssl_ciphers_weak_report.nasl",
     "GSHB/GSHB_Kompendium.nasl",
     "/policy_control_template.nasl",
     "/template.nasl",
     "test_ipv6_packet_forgery.nasl",
     "test_version_func_inc.nasl",
+    "pre2008/mssql_brute_force.nasl",
 ]
 
 
 class CheckReportingConsistency(FileContentPlugin):
     name = "check_reporting_consistency"
 
     def check_content(
```

### Comparing `troubadix-23.6.3/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.7.0/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.7.0/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.7.0/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_category.py` & `troubadix-23.7.0/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_copyright.py` & `troubadix-23.7.0/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_family.py` & `troubadix-23.7.0/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_tag_form.py` & `troubadix-23.7.0/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.7.0/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.7.0/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.7.0/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_xref_form.py` & `troubadix-23.7.0/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/script_xref_url.py` & `troubadix-23.7.0/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/security_messages.py` & `troubadix-23.7.0/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.7.0/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/solution_text.py` & `troubadix-23.7.0/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/solution_type.py` & `troubadix-23.7.0/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/spelling.py` & `troubadix-23.7.0/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/tabs.py` & `troubadix-23.7.0/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/todo_tbd.py` & `troubadix-23.7.0/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.7.0/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/using_display.py` & `troubadix-23.7.0/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/valid_oid.py` & `troubadix-23.7.0/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.7.0/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.7.0/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.7.0/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/plugins/vt_placement.py` & `troubadix-23.7.0/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/reporter.py` & `troubadix-23.7.0/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/results.py` & `troubadix-23.7.0/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/runner.py` & `troubadix-23.7.0/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-23.7.0/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/common.py` & `troubadix-23.7.0/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.7.0/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.7.0/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.7.0/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/troubadix/troubadix.py` & `troubadix-23.7.0/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.3/PKG-INFO` & `troubadix-23.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.6.3
+Version: 23.7.0
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

