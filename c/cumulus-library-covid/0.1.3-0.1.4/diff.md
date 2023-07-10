# Comparing `tmp/cumulus_library_covid-0.1.3.tar.gz` & `tmp/cumulus_library_covid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_covid-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_covid-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_covid-0.1.3.tar` & `cumulus_library_covid-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1062 2023-05-30 20:14:21.539236 cumulus_library_covid-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:14:21.539306 cumulus_library_covid-0.1.3/cumulus_library_covid/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:14:21.539386 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/__init__.py
--rw-r--r--   0        0        0     3473 2023-07-05 20:21:01.776802 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.py
--rw-r--r--   0        0        0     4429 2023-07-05 20:21:01.777002 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.sql
--rw-r--r--   0        0        0     2678 2023-07-05 20:21:01.777174 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_general.sql
--rw-r--r--   0        0        0      600 2023-07-05 20:21:01.777331 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
--rw-r--r--   0        0        0      192 2023-07-05 20:21:01.777487 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
--rw-r--r--   0        0        0     4154 2023-07-05 20:21:01.777645 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
--rw-r--r--   0        0        0     1586 2023-07-05 20:21:01.777801 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_ed_note.sql
--rw-r--r--   0        0        0     8576 2023-07-05 20:21:01.777962 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr.sql
--rw-r--r--   0        0        0     1522 2023-07-05 20:21:01.778121 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
--rw-r--r--   0        0        0     2022 2023-07-05 20:21:01.778280 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
--rw-r--r--   0        0        0     2747 2023-07-05 20:21:01.778440 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
--rw-r--r--   0        0        0      794 2023-07-05 19:43:06.938136 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_study_period.sql
--rw-r--r--   0        0        0      731 2023-07-05 19:43:06.938214 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.py
--rw-r--r--   0        0        0    16063 2023-07-05 19:43:06.938352 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.sql
--rw-r--r--   0        0        0     1115 2023-07-05 19:43:06.938524 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/manifest.toml
--rw-r--r--   0        0        0      864 2023-07-05 20:21:01.778747 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_dx.sql
--rw-r--r--   0        0        0     1569 2023-07-05 20:21:01.778943 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_pcr.sql
--rw-r--r--   0        0        0     1540 2023-07-05 19:43:06.939079 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
--rw-r--r--   0        0        0     1031 2023-07-05 20:21:01.779138 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_study_period.sql
--rw-r--r--   0        0        0     2277 2023-07-05 20:21:01.779326 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_symptom.sql
--rw-r--r--   0        0        0     2522 2023-07-05 19:43:06.939445 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/typesystem.py
--rw-r--r--   0        0        0     1905 2023-07-05 19:43:06.939507 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
--rw-r--r--   0        0        0     5415 2023-07-05 19:43:06.939562 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
--rw-r--r--   0        0        0     3376 2023-07-05 19:43:06.939664 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
--rw-r--r--   0        0        0     4037 2023-07-05 19:43:06.939753 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
--rw-r--r--   0        0        0     4602 2023-07-05 19:43:06.939807 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
--rw-r--r--   0        0        0     3369 2023-07-05 19:43:06.939974 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
--rw-r--r--   0        0        0     8196 2023-07-05 19:43:06.940040 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
--rw-r--r--   0        0        0     1099 2023-07-05 20:27:29.283253 cumulus_library_covid-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/count.py
+-rw-r--r--   0        0        0     4369 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/count.sql
+-rw-r--r--   0        0        0     2678 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_age_general.sql
+-rw-r--r--   0        0        0      600 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
+-rw-r--r--   0        0        0      192 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
+-rw-r--r--   0        0        0     4154 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
+-rw-r--r--   0        0        0     1586 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_ed_note.sql
+-rw-r--r--   0        0        0     8576 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr.sql
+-rw-r--r--   0        0        0     1522 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
+-rw-r--r--   0        0        0     2022 2023-07-10 13:22:10.093747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
+-rw-r--r--   0        0        0     2747 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
+-rw-r--r--   0        0        0      794 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_study_period.sql
+-rw-r--r--   0        0        0      731 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_symptom.py
+-rw-r--r--   0        0        0    16063 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_symptom.sql
+-rw-r--r--   0        0        0     1115 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/manifest.toml
+-rw-r--r--   0        0        0      864 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_dx.sql
+-rw-r--r--   0        0        0     1569 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_pcr.sql
+-rw-r--r--   0        0        0     1540 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
+-rw-r--r--   0        0        0     1031 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_study_period.sql
+-rw-r--r--   0        0        0     2277 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_symptom.sql
+-rw-r--r--   0        0        0     2522 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/typesystem.py
+-rw-r--r--   0        0        0     1905 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
+-rw-r--r--   0        0        0     5415 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
+-rw-r--r--   0        0        0     3376 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
+-rw-r--r--   0        0        0     4037 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
+-rw-r--r--   0        0        0     4602 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
+-rw-r--r--   0        0        0     3369 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
+-rw-r--r--   0        0        0     8196 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
+-rw-r--r--   0        0        0     1099 2023-07-10 13:22:10.097747 cumulus_library_covid-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.4/PKG-INFO
```

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.py` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/count.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/count.sql`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_dx_week AS
+CREATE TABLE covid_symptom__count_dx_week AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         cond_week,
         enc_class_code,
         age_at_visit,
@@ -21,15 +21,15 @@
     ed_note,
     variant_era
 FROM powerset
 WHERE cnt_subject >= 10
 ORDER BY cnt DESC;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_dx_month AS
+CREATE TABLE covid_symptom__count_dx_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         cond_month,
         enc_class_code,
         age_at_visit,
@@ -47,15 +47,15 @@
     ed_note,
     variant_era
 FROM powerset
 WHERE cnt_subject >= 10
 ORDER BY cnt DESC;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_pcr_week AS
+CREATE TABLE covid_symptom__count_pcr_week AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         covid_pcr_week,
         covid_pcr_result_display,
         variant_era,
@@ -86,15 +86,15 @@
     gender,
     race_display
 FROM powerset
 WHERE cnt_subject >= 10
 ORDER BY cnt DESC;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_pcr_month AS
+CREATE TABLE covid_symptom__count_pcr_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         covid_pcr_month,
         covid_pcr_result_display,
         variant_era,
@@ -125,15 +125,15 @@
     gender,
     race_display
 FROM powerset
 WHERE cnt_subject >= 10
 ORDER BY cnt DESC;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_study_period_week AS
+CREATE TABLE covid_symptom__count_study_period_week AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         start_week,
         variant_era,
         ed_note,
@@ -153,15 +153,15 @@
     age_group,
     race_display
 FROM powerset
 WHERE cnt_subject >= 10
 ORDER BY cnt DESC;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW covid_symptom__count_study_period_month AS
+CREATE TABLE covid_symptom__count_study_period_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         start_month,
         variant_era,
         ed_note,
```

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_general.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_age_general.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_pediatric.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_age_pediatric.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_dx_snomed.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_dx_snomed.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_ed_note.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_ed_note.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_custom.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_custom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_negative.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_negative.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_positive.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_pcr_positive.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_study_period.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.py` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_symptom.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/define_symptom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/manifest.toml` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_dx.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_dx.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_pcr.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_pcr.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_study_period.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_symptom.sql` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/table_symptom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/typesystem.py` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json` & `cumulus_library_covid-0.1.4/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.3/pyproject.toml` & `cumulus_library_covid-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library-covid"
-version = "0.1.3"
+version = "0.1.4"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "cumulus-library >= 0.3.0",
     "sqlfluff == 2.0.2"
 ]
```

### Comparing `cumulus_library_covid-0.1.3/PKG-INFO` & `cumulus_library_covid-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library-covid
-Version: 0.1.3
+Version: 0.1.4
 Summary: SQL generation for cumulus covid symptom analysis
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -32,12 +32,12 @@
 
 ## Publications
 
 The following publications leveraged this module:
 
 __A computable phenotype for patients with SARS-CoV2 testing that occurred outside the hospital__
 Lijing Wang, Amy Zipursky, Alon Geva, Andrew J. McMurry, Kenneth D. Mandl, Timothy A. Miller
-medRxiv 2023.01.19.23284738; doi: https://doi.org/10.1101/2023.01.19.23284738 (Preprint)
+JAMIA Open, 2023;, ooad047,doi: https://doi.org/10.1093/jamiaopen/ooad047 
 
 __The SMART Text2FHIR Pipeline__
 Timothy A. Miller, Andrew J. McMurry, James Jones, Daniel Gottlieb, Kenneth D. Mandl
 medRxiv 2023.03.21.23287499; doi: https://doi.org/10.1101/2023.03.21.23287499 (Preprint)
```

