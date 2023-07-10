# Comparing `tmp/patent_client-3.2.4.tar.gz` & `tmp/patent_client-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-3.2.4.tar", max compression
+gzip compressed data, was "patent_client-3.2.6.tar", max compression
```

## Comparing `patent_client-3.2.4.tar` & `patent_client-3.2.6.tar`

### file list

```diff
@@ -1,165 +1,167 @@
--rw-r--r--   0        0        0      593 2023-04-30 00:25:43.167737 patent_client-3.2.4/LICENSE
--rw-r--r--   0        0        0     4414 2023-04-30 00:25:43.167737 patent_client-3.2.4/README.md
--rw-r--r--   0        0        0     3485 2023-04-30 00:25:43.207737 patent_client-3.2.4/pyproject.toml
--rw-r--r--   0        0        0     2590 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/__init__.py
--rw-r--r--   0        0        0      215 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/default_settings.yml
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/__init__.py
--rw-r--r--   0        0        0      271 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      350 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/api.py
--rw-r--r--   0        0        0      406 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     8854 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/examples/example.xml
--rw-r--r--   0        0        0     7248 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.json
--rw-r--r--   0        0        0     8853 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.xml
--rw-r--r--   0        0        0      304 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1180 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/model.py
--rw-r--r--   0        0        0     1603 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/schema.py
--rw-r--r--   0        0        0      594 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0       77 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      355 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/api.py
--rw-r--r--   0        0        0      380 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0   285423 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
--rw-r--r--   0        0        0      323 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2117 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/model.py
--rw-r--r--   0        0        0     4163 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      283 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4041 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/schema.py
--rw-r--r--   0        0        0      904 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0    76105 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/example.xml
--rw-r--r--   0        0        0    44095 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.json
--rw-r--r--   0        0        0    76104 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.xml
--rw-r--r--   0        0        0    11924 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/us_example.json
--rw-r--r--   0        0        0    22970 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/us_example.xml
--rw-r--r--   0        0        0      114 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1269 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1102 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      600 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      972 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5024 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/api.py
--rw-r--r--   0        0        0     1884 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/cql.py
--rw-r--r--   0        0        0     3127 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2043 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      399 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2633 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1095 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     1610 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      776 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      306 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3943 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      891 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1652 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      668 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3099 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     3973 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0     5916 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     9015 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34663 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     2318 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/session.py
--rw-r--r--   0        0        0     1613 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/util.py
--rw-r--r--   0        0        0     5991 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/parser.py
--rw-r--r--   0        0        0     1129 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/session.py
--rw-r--r--   0        0        0     1300 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/test_parser.py
--rw-r--r--   0        0        0      278 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/uspto/__init__.py
--rw-r--r--   0        0        0      105 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     3822 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4269 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     3404 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/model.py
--rw-r--r--   0        0        0     3473 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/schema.py
--rw-r--r--   0        0        0     2234 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/schema_test.py
--rw-r--r--   0        0        0    13274 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_1.xml
--rw-r--r--   0        0        0    11638 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_2.xml
--rw-r--r--   0        0        0   277704 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_3.xml
--rw-r--r--   0        0        0       76 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     2983 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1979 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     5405 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3705 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     5062 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5146 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     2094 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema.py
--rw-r--r--   0        0        0      983 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema_test.py
--rw-r--r--   0        0        0      271 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/session.py
--rw-r--r--   0        0        0     4134 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      117 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/peds/__init__.py
--rw-r--r--   0        0        0     7525 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/manager.py
--rw-r--r--   0        0        0     9017 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    19255 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/model.py
--rw-r--r--   0        0        0     8585 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/schema.py
--rw-r--r--   0        0        0      529 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/schema_test.py
--rw-r--r--   0        0        0    94546 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/test/app_12721698.json
--rw-r--r--   0        0        0    15274 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/test/expected.json
--rw-r--r--   0        0        0      331 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/ptab/__init__.py
--rw-r--r--   0        0        0     5774 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/developer.uspto.gov.crt
--rw-r--r--   0        0        0     3207 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2135 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     7387 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/model.py
--rw-r--r--   0        0        0    69917 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/ptabApiV2.json
--rw-r--r--   0        0        0     3597 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/schema.py
--rw-r--r--   0        0        0      282 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/session.py
--rw-r--r--   0        0        0      159 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/util.py
--rw-r--r--   0        0        0       72 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     4943 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/public_search/api.py
--rw-r--r--   0        0        0     3891 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/manager.py
--rw-r--r--   0        0        0    12219 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/model.py
--rw-r--r--   0        0        0     7277 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4331 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     3689 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query_test.py
--rw-r--r--   0        0        0    10290 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/schema.py
--rw-r--r--   0        0        0     1254 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/schema_test.py
--rw-r--r--   0        0        0   387227 2023-04-30 00:25:43.339738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio.json
--rw-r--r--   0        0        0   213101 2023-04-30 00:25:43.339738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio_expected.json
--rw-r--r--   0        0        0  2431829 2023-04-30 00:25:43.343738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs.json
--rw-r--r--   0        0        0  1880230 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs_expected.json
--rw-r--r--   0        0        0      565 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/__init__.py
--rw-r--r--   0        0        0     5030 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/manager.py
--rw-r--r--   0        0        0     1696 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/model.py
--rw-r--r--   0        0        0      775 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/model_test.py
--rw-r--r--   0        0        0     3148 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/related.py
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/test_manager.py
--rw-r--r--   0        0        0     1913 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/util.py
--rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4263 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6204 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      834 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3565 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      931 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      204 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/__init__.py
--rw-r--r--   0        0        0     5774 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/date_parse.py
--rw-r--r--   0        0        0     9054 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/date_parse_test.py
--rw-r--r--   0        0        0    15027 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/functional.py
--rw-r--r--   0        0        0    12808 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/regex_helper.py
--rw-r--r--   0        0        0      611 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/format.py
--rw-r--r--   0        0        0     2699 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/version.py
--rw-r--r--   0        0        0     6965 1970-01-01 00:00:00.000000 patent_client-3.2.4/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-07-10 16:32:51.595110 patent_client-3.2.6/LICENSE
+-rw-r--r--   0        0        0     4414 2023-07-10 16:32:51.595110 patent_client-3.2.6/README.md
+-rw-r--r--   0        0        0     3478 2023-07-10 16:32:51.639111 patent_client-3.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2590 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/default_settings.yml
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/api.py
+-rw-r--r--   0        0        0      406 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     8854 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/examples/example.xml
+-rw-r--r--   0        0        0     7248 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/expected/example.json
+-rw-r--r--   0        0        0     8853 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/expected/example.xml
+-rw-r--r--   0        0        0      304 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1180 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/model.py
+-rw-r--r--   0        0        0     1603 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      594 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0       77 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      380 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0   285423 2023-07-10 16:32:51.639111 patent_client-3.2.6/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
+-rw-r--r--   0        0        0   285493 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/legal_code_descriptions_202307.xlsx
+-rw-r--r--   0        0        0      323 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2117 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     4162 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      283 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4041 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0      904 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0    76105 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/test/example.xml
+-rw-r--r--   0        0        0    44095 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/example.json
+-rw-r--r--   0        0        0    78351 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/example.xml
+-rw-r--r--   0        0        0    11924 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/us_example.json
+-rw-r--r--   0        0        0    22970 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/test/us_example.xml
+-rw-r--r--   0        0        0      114 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1269 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1102 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      600 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      972 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5024 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/published/api.py
+-rw-r--r--   0        0        0     1884 2023-07-10 16:32:51.643111 patent_client-3.2.6/src/patent_client/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     3127 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2043 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      399 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2633 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1095 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     1610 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      776 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      306 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3943 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      891 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1652 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      668 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3099 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     3973 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0     5916 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     9015 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34663 2023-07-10 16:32:51.647111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     2318 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/epo/ops/session.py
+-rw-r--r--   0        0        0     1613 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/epo/ops/util.py
+-rw-r--r--   0        0        0     5991 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/parser.py
+-rw-r--r--   0        0        0     1163 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/session.py
+-rw-r--r--   0        0        0     1300 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/test_parser.py
+-rw-r--r--   0        0        0      278 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/uspto/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-10 16:32:51.651111 patent_client-3.2.6/src/patent_client/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4269 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     4326 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/model.py
+-rw-r--r--   0        0        0     3473 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/schema.py
+-rw-r--r--   0        0        0     2234 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/schema_test.py
+-rw-r--r--   0        0        0    13274 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_1.xml
+-rw-r--r--   0        0        0    11638 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_2.xml
+-rw-r--r--   0        0        0   277704 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_3.xml
+-rw-r--r--   0        0        0       76 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     2983 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1979 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     5405 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3705 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     5062 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5146 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     2094 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/schema.py
+-rw-r--r--   0        0        0      983 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/schema_test.py
+-rw-r--r--   0        0        0      271 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/session.py
+-rw-r--r--   0        0        0     4134 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2023-07-10 16:32:51.663111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2023-07-10 16:32:51.667111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2023-07-10 16:32:51.667111 patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      117 2023-07-10 16:32:51.667111 patent_client-3.2.6/src/patent_client/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     7716 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9017 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    19255 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/model.py
+-rw-r--r--   0        0        0      175 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/model_test.py
+-rw-r--r--   0        0        0     8585 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/schema.py
+-rw-r--r--   0        0        0      529 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/schema_test.py
+-rw-r--r--   0        0        0    94546 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/test/app_12721698.json
+-rw-r--r--   0        0        0    15274 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/peds/test/expected.json
+-rw-r--r--   0        0        0      331 2023-07-10 16:32:51.691111 patent_client-3.2.6/src/patent_client/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0     5774 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/developer.uspto.gov.crt
+-rw-r--r--   0        0        0     3243 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2135 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     7558 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/model.py
+-rw-r--r--   0        0        0    69917 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/ptabApiV2.json
+-rw-r--r--   0        0        0     3597 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/schema.py
+-rw-r--r--   0        0        0      282 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/session.py
+-rw-r--r--   0        0        0      159 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/ptab/util.py
+-rw-r--r--   0        0        0       72 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     4943 2023-07-10 16:32:51.695111 patent_client-3.2.6/src/patent_client/uspto/public_search/api.py
+-rw-r--r--   0        0        0     3891 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/manager.py
+-rw-r--r--   0        0        0    12219 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/model.py
+-rw-r--r--   0        0        0     7277 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4331 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     3689 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0    10290 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/schema.py
+-rw-r--r--   0        0        0     1254 2023-07-10 16:32:51.779112 patent_client-3.2.6/src/patent_client/uspto/public_search/schema_test.py
+-rw-r--r--   0        0        0   387227 2023-07-10 16:32:51.791112 patent_client-3.2.6/src/patent_client/uspto/public_search/test/biblio.json
+-rw-r--r--   0        0        0   213101 2023-07-10 16:32:51.791112 patent_client-3.2.6/src/patent_client/uspto/public_search/test/biblio_expected.json
+-rw-r--r--   0        0        0  2431829 2023-07-10 16:32:51.791112 patent_client-3.2.6/src/patent_client/uspto/public_search/test/docs.json
+-rw-r--r--   0        0        0  1880230 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/uspto/public_search/test/docs_expected.json
+-rw-r--r--   0        0        0      565 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/manager.py
+-rw-r--r--   0        0        0     1711 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/model.py
+-rw-r--r--   0        0        0      775 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/model_test.py
+-rw-r--r--   0        0        0     3148 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/related.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/test_manager.py
+-rw-r--r--   0        0        0     1913 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/base/util.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4263 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6204 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      834 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3565 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      931 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      204 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/datetime/__init__.py
+-rw-r--r--   0        0        0     5774 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/datetime/date_parse.py
+-rw-r--r--   0        0        0     9054 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/datetime/date_parse_test.py
+-rw-r--r--   0        0        0    15027 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/datetime/functional.py
+-rw-r--r--   0        0        0    12808 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/datetime/regex_helper.py
+-rw-r--r--   0        0        0      611 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/format.py
+-rw-r--r--   0        0        0     2699 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2023-07-10 16:32:51.795112 patent_client-3.2.6/src/patent_client/version.py
+-rw-r--r--   0        0        0     6978 1970-01-01 00:00:00.000000 patent_client-3.2.6/PKG-INFO
```

### Comparing `patent_client-3.2.4/LICENSE` & `patent_client-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/README.md` & `patent_client-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/pyproject.toml` & `patent_client-3.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "patent_client"
-version = "3.2.4"
+version = "3.2.6"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
 
 keywords = ["patent", "intellectual property", "usitc", "epo", "ops", "trademark", "inpadoc", "337"]
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Legal Industry",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering",
 ]
 
@@ -59,15 +59,14 @@
 
 
 [tool.poetry.dev-dependencies]
 
 # PyTest and Plugins
 pytest = "^7.1.2"
 vcrpy = "^4.2.0"
-codecov = "^2.1.12"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.19.0"
 pytest-xdist = "^2.5.0"
 mypy = "^0.961"
 black = {version = "^22.12.0", allow-prereleases = true}
 pandas = "1.3.5"
```

### Comparing `patent_client-3.2.4/src/patent_client/__init__.py` & `patent_client-3.2.6/src/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/examples/example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/examples/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.json` & `patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/family/fixtures/expected/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/model.py` & `patent_client-3.2.6/src/patent_client/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/schema.py` & `patent_client-3.2.6/src/patent_client/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/family/schema_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/model.py` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes.py` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/national_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if out_path.exists():
             return out_path
         response = session.get(excel_url, stream=True)
         with out_path.open("wb") as f:
             for chunk in response.iter_content(chunk_size=8192):
                 f.write(chunk)
         return out_path
-    except IndexError:
+    except Exception:
         logger.debug("Could not find live code file - falling back to default dated 2022-11-12")
         return Path(__file__).parent / "legal_code_descriptions_20221112.xlsx"
 
 
 def create_code_database(excel_path):
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
```

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/schema.py` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/schema_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.json` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/example.xml`

 * *Files 1% similar despite different names*

#### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/example.xml`

```diff
@@ -893,10 +893,35 @@
         <ops:L008EP desc="Legal Event Code 1">PLBE</ops:L008EP>
         <ops:L018EP desc="DATE last exchanged">2022-02-09</ops:L018EP>
         <ops:L019EP desc="DATE first created">2022-02-02</ops:L019EP>
         <ops:L500EP>
           <ops:L510EP desc="Free Format Text">ORIGINAL CODE: 0009261</ops:L510EP>
         </ops:L500EP>
       </ops:legal>
+      <ops:legal code="REG " desc="REFERENCE TO A NATIONAL CODE" infl=" " dateMigr="00010101">
+        <ops:pre line="00001">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE Ref Country Code BE</ops:pre>
+        <ops:pre line="00002">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE Ref Legal Event Code SPCF</ops:pre>
+        <ops:pre line="00003">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE Free Format Text PRODUCT NAME: DELAMANIDE; AUTHORISATION NUMBER AND DATE:</ops:pre>
+        <ops:pre line="00004">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE SPC Suppl Protection Certif 2014C/053</ops:pre>
+        <ops:pre line="00005">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE Filing DATE 20140909</ops:pre>
+        <ops:pre line="00006">EP    99203729A 2022-09-27REG  REFERENCE TO A NATIONAL CODE Expiry DATE 20231010</ops:pre>
+        <ops:L001EP desc="Country Code">EP</ops:L001EP>
+        <ops:L002EP desc="Filing / Published Document">F</ops:L002EP>
+        <ops:L003EP desc="Document Number">99203729</ops:L003EP>
+        <ops:L004EP desc="Kind Code">A</ops:L004EP>
+        <ops:L005EP desc="IPR Type">PI</ops:L005EP>
+        <ops:L007EP desc="Gazette DATE">2022-09-27</ops:L007EP>
+        <ops:L008EP desc="Legal Event Code 1">REG</ops:L008EP>
+        <ops:L018EP desc="DATE last exchanged">2022-10-22</ops:L018EP>
+        <ops:L019EP desc="DATE first created">2022-10-17</ops:L019EP>
+        <ops:L500EP>
+          <ops:L501EP desc="Ref Country Code">BE</ops:L501EP>
+          <ops:L502EP desc="Ref Legal Event Code" descData="SUPPLEMENTARY PROTECTION CERTIFICATE FILED" infl=" ">SPCF</ops:L502EP>
+          <ops:L510EP desc="Free Format Text">PRODUCT NAME: DELAMANIDE; AUTHORISATION NUMBER AND DATE:</ops:L510EP>
+          <ops:L511EP desc="SPC Suppl Protection Certif">2014C/053</ops:L511EP>
+          <ops:L512EP desc="Filing DATE">20140909</ops:L512EP>
+          <ops:L513EP desc="Expiry DATE">20231010</ops:L513EP>
+        </ops:L500EP>
+      </ops:legal>
     </ops:family-member>
   </ops:patent-family>
 </ops:world-patent-data>
```

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/us_example.json` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/expected/us_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/us_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/legal/test/us_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/api.py` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/api_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.py` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.txt` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/messages.txt` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/model.py` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/number_service/schema.py` & `patent_client-3.2.6/src/patent_client/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/api.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/api_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/cql.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/manager.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/manager_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/model/biblio.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/model/fulltext.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/model/images.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/model/search.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/biblio.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/fulltext.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/images.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/search.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/schema_test.py` & `patent_client-3.2.6/src/patent_client/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_2.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_3.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_4.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example_2.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/description_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/claims_example.json` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/image_example.json` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/search_result.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/full_cycle_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/image_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/published/test/search_example.xml` & `patent_client-3.2.6/src/patent_client/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/session.py` & `patent_client-3.2.6/src/patent_client/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/epo/ops/util.py` & `patent_client-3.2.6/src/patent_client/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/parser.py` & `patent_client-3.2.6/src/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/session.py` & `patent_client-3.2.6/src/patent_client/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,14 @@
             expire_after=datetime.timedelta(days=max_age),
             backend="sqlite",
             allowable_methods=("GET", "POST"),
             ignored_parameters=[
                 "Authorization",
             ],
         )
-        self.headers["User-Agent"] = f"Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
+        self.headers[
+            "User-Agent"
+        ] = f"Mozilla/5.0 Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
         # Install a default retry on the session using urrlib3
         retry = Retry(total=5, backoff_factor=0.2)
         self.mount("https://", HTTPAdapter(max_retries=retry))
         self.mount("http://", HTTPAdapter(max_retries=retry))
```

### Comparing `patent_client-3.2.4/src/patent_client/settings.py` & `patent_client-3.2.6/src/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/test_parser.py` & `patent_client-3.2.6/src/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/manager.py` & `patent_client-3.2.6/src/patent_client/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/manager_test.py` & `patent_client-3.2.6/src/patent_client/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/model.py` & `patent_client-3.2.6/src/patent_client/uspto/assignment/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import datetime
+import warnings
 from dataclasses import dataclass
 from dataclasses import field
 from typing import *
 
 from patent_client import session
 from patent_client.util import Model
 from patent_client.util.base.related import get_model
@@ -47,15 +48,15 @@
         response = session.get(self.image_url, stream=True)
         with open(f"{self.id}.pdf", "wb") as f:
             f.write(response.raw.read())
 
 
 @dataclass
 class Property(Model):
-    appl_id: str
+    appl_id: "Optional[str]" = None
     invention_title: "Optional[str]" = None
     inventors: "Optional[str]" = None
     # Numbers
     pct_num: "Optional[str]" = None
     intl_reg_num: "Optional[str]" = None
     publ_num: "Optional[str]" = None
     pat_num: "Optional[str]" = None
@@ -67,15 +68,33 @@
 
     def __repr__(self):
         return f"Property(appl_id={self.appl_id}, invention_title={self.invention_title})"
 
     @property
     def application(self) -> "patent_client.uspto.peds.model.USApplication":
         """The related US Application"""
-        return get_model("patent_client.uspto.peds.model.USApplication").objects.get(appl_id=self.appl_id)
+        try:
+            appl_id = getattr(self, "appl_id", None)
+            if appl_id is not None:
+                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(appl_id=appl_id)
+            appl_id = getattr(self, "pct_num", None)
+            if appl_id is not None:
+                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(appl_id=appl_id)
+            pub_num = getattr(self, "publ_num", None)
+            if pub_num is not None:
+                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    app_early_pub_number=pub_num
+                )
+            pat_num = getattr(self, "pat_num", None)
+            if pat_num is not None:
+                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(patent_number=pat_num)
+        except Exception:
+            pass
+        warnings.warn(f"Unable to find application for {self}")
+        return None
 
     @property
     def patent(self) -> "patent_client.uspto.fulltext.patent.model.Patent":
         """The related US Patent, if any"""
         return get_model("patent_client.uspto.peds.fulltext.patent.model.Patent").objects.get(
             publication_number=self.pat_num
         )
```

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/schema.py` & `patent_client-3.2.6/src/patent_client/uspto/assignment/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/schema_test.py` & `patent_client-3.2.6/src/patent_client/uspto/assignment/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_1.xml` & `patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_2.xml` & `patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_3.xml` & `patent_client-3.2.6/src/patent_client/uspto/assignment/test/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/api.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/gd_input.csv` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/manager.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/model.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/model_test.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/query.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/query_test.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema_test.py` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app.json` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app_expected.json` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list.json` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-3.2.6/src/patent_client/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/manager.py` & `patent_client-3.2.6/src/patent_client/uspto/peds/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,19 @@
                         f"{response.status_code}\n{response.text}\n{response.headers}\n{json.dumps(query_params)}"
                     )
             data = response.json()
             self.pages[page_number] = data["queryResults"]["searchResponse"]["response"]
         return self.pages[page_number]
 
     def query_params(self, page_no):
+        if "query" in self.config.filter:
+            query = self.config.filter["query"]
+            query["start"] = page_no * self.page_size + self.config.offset
+            return query
+
         sort_query = ""
         for s in self.config.order_by:
             if s[0] == "-":
                 sort_query += f"{inflection.camelize(s[1:], uppercase_first_letter=False)} desc ".strip()
             else:
                 sort_query += (f"{inflection.camelize(s, uppercase_first_letter=False)} asc").strip()
         if not sort_query:
```

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/manager_test.py` & `patent_client-3.2.6/src/patent_client/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/model.py` & `patent_client-3.2.6/src/patent_client/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/schema.py` & `patent_client-3.2.6/src/patent_client/uspto/peds/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/schema_test.py` & `patent_client-3.2.6/src/patent_client/uspto/peds/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/test/app_12721698.json` & `patent_client-3.2.6/src/patent_client/uspto/peds/test/app_12721698.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/peds/test/expected.json` & `patent_client-3.2.6/src/patent_client/uspto/peds/test/expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/developer.uspto.gov.crt` & `patent_client-3.2.6/src/patent_client/uspto/ptab/developer.uspto.gov.crt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/manager.py` & `patent_client-3.2.6/src/patent_client/uspto/ptab/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         if self.config.limit:
             return length if length < self.config.limit else self.config.limit
         else:
             return length
 
     def _len(self):
         response = session.get(self.url + self.path, params=self.query())
+        response.raise_for_status()
         return response.json()["recordTotalQuantity"]
 
     def query(self):
         query = dict()
         for k, v in self.config.filter.items():
             key = k if k not in peds_to_ptab else peds_to_ptab[k]
             key = inflection.camelize(key, uppercase_first_letter=False)
```

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/manager_test.py` & `patent_client-3.2.6/src/patent_client/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/model.py` & `patent_client-3.2.6/src/patent_client/uspto/ptab/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -128,21 +128,21 @@
 fname_re = re.compile(r"[<>:\"/\|?*]")
 
 
 @dataclass
 class PtabDocument(Model):
     __manager__ = "patent_client.uspto.ptab.manager.PtabDocumentManager"
     document_identifier: str = field(repr=False)
-    document_category: str
-    document_type_name: str
-    document_number: int
-    document_name: str
-    document_filing_date: datetime.date
-    proceeding_number: str = field(repr=False)
-    proceeding_type_category: str = field(repr=False)
+    document_category: "Optional[str]" = None
+    document_type_name: "Optional[str]" = None
+    document_number: "Optional[int]" = None
+    document_name: "Optional[str]" = None
+    document_filing_date: "Optional[datetime.date]" = None
+    proceeding_number: "Optional[str]" = field(repr=False, default=None)
+    proceeding_type_category: "Optional[str]" = field(repr=False, default=None)
     title: "Optional[str]" = None
 
     @property
     def proceeding(self) -> "patent_client.uspto.ptab.model.PtabProceeding":
         """The PTAB proceeding associated with the document"""
         return get_model("patent_client.uspto.ptab.model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
@@ -158,14 +158,15 @@
         with session.get(
             f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download", verify=False
         ) as r:
             r.raise_for_status()
             with out_path.open("wb") as f:
                 for chunk in r.iter_content(chunk_size=8192):
                     f.write(chunk)
+        return out_path
 
 
 @dataclass
 class PtabDecision(Model):
     __manager__ = "patent_client.uspto.ptab.manager.PtabDecisionManager"
     proceeding_number: str
     board_rulings: "List[str]" = field(default_factory=ListCollection)
```

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/ptabApiV2.json` & `patent_client-3.2.6/src/patent_client/uspto/ptab/ptabApiV2.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/ptab/schema.py` & `patent_client-3.2.6/src/patent_client/uspto/ptab/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/api.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/manager.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/model.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/model_test.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/query.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/query_config.csv` & `patent_client-3.2.6/src/patent_client/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/query_test.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/schema.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/schema_test.py` & `patent_client-3.2.6/src/patent_client/uspto/public_search/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio.json` & `patent_client-3.2.6/src/patent_client/uspto/public_search/test/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio_expected.json` & `patent_client-3.2.6/src/patent_client/uspto/public_search/test/biblio_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs.json` & `patent_client-3.2.6/src/patent_client/uspto/public_search/test/docs.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs_expected.json` & `patent_client-3.2.6/src/patent_client/uspto/public_search/test/docs_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/__init__.py` & `patent_client-3.2.6/src/patent_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/base/manager.py` & `patent_client-3.2.6/src/patent_client/util/base/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/base/model.py` & `patent_client-3.2.6/src/patent_client/util/base/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 
     # def __init__(self, *args, **kwargs):
     #    try:
     #        return super().__init__(*args, **kwargs)
     #    except TypeError as e:
     #        raise TypeError(f"{e.args[0]}\nargs:{args}\nkwargs:{kwargs}")
 
-    def fields(self):
+    @classmethod
+    def fields(cls):
         """Return list of fields"""
-        return fields(self)
+        return fields(cls)
 
     def __iter__(self):
         return self.items()
 
     def items(self):
         if self.__default_fields__:
             fields = self.__default_fields__
```

### Comparing `patent_client-3.2.4/src/patent_client/util/base/model_test.py` & `patent_client-3.2.6/src/patent_client/util/base/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/base/related.py` & `patent_client-3.2.6/src/patent_client/util/base/related.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/base/util.py` & `patent_client-3.2.6/src/patent_client/util/base/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-3.2.6/src/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-3.2.6/src/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.json` & `patent_client-3.2.6/src/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.txt` & `patent_client-3.2.6/src/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/model.py` & `patent_client-3.2.6/src/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/parser.py` & `patent_client-3.2.6/src/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/claims/parser_test.py` & `patent_client-3.2.6/src/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/datetime/date_parse.py` & `patent_client-3.2.6/src/patent_client/util/datetime/date_parse.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/datetime/date_parse_test.py` & `patent_client-3.2.6/src/patent_client/util/datetime/date_parse_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/datetime/functional.py` & `patent_client-3.2.6/src/patent_client/util/datetime/functional.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/datetime/regex_helper.py` & `patent_client-3.2.6/src/patent_client/util/datetime/regex_helper.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/format.py` & `patent_client-3.2.6/src/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/src/patent_client/util/test.py` & `patent_client-3.2.6/src/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.4/PKG-INFO` & `patent_client-3.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 3.2.4
+Version: 3.2.6
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

