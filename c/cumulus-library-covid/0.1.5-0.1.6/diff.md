# Comparing `tmp/cumulus_library_covid-0.1.5.tar.gz` & `tmp/cumulus_library_covid-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_covid-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_covid-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_covid-0.1.5.tar` & `cumulus_library_covid-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1048 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/__init__.py
--rw-r--r--   0        0        0     3741 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/count.py
--rw-r--r--   0        0        0     6155 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/count.sql
--rw-r--r--   0        0        0     2678 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_age_general.sql
--rw-r--r--   0        0        0      600 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
--rw-r--r--   0        0        0      192 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
--rw-r--r--   0        0        0     4154 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
--rw-r--r--   0        0        0     1586 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_ed_note.sql
--rw-r--r--   0        0        0     8576 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr.sql
--rw-r--r--   0        0        0     1522 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
--rw-r--r--   0        0        0     2022 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
--rw-r--r--   0        0        0     2747 2023-07-10 13:53:43.764383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
--rw-r--r--   0        0        0      794 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_study_period.sql
--rw-r--r--   0        0        0      731 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_symptom.py
--rw-r--r--   0        0        0    16063 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_symptom.sql
--rw-r--r--   0        0        0     1115 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/manifest.toml
--rw-r--r--   0        0        0      864 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_dx.sql
--rw-r--r--   0        0        0     1569 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_pcr.sql
--rw-r--r--   0        0        0     1540 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
--rw-r--r--   0        0        0     1031 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_study_period.sql
--rw-r--r--   0        0        0     2277 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_symptom.sql
--rw-r--r--   0        0        0     2522 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/typesystem.py
--rw-r--r--   0        0        0     1905 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
--rw-r--r--   0        0        0     5415 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
--rw-r--r--   0        0        0     3376 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
--rw-r--r--   0        0        0     4037 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
--rw-r--r--   0        0        0     4602 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
--rw-r--r--   0        0        0     3369 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
--rw-r--r--   0        0        0     8196 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
--rw-r--r--   0        0        0     1099 2023-07-10 13:53:43.768383 cumulus_library_covid-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/__init__.py
+-rw-r--r--   0        0        0     3816 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/count.py
+-rw-r--r--   0        0        0     7943 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/count.sql
+-rw-r--r--   0        0        0     2678 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_age_general.sql
+-rw-r--r--   0        0        0      600 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
+-rw-r--r--   0        0        0      192 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
+-rw-r--r--   0        0        0     4154 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
+-rw-r--r--   0        0        0     1586 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_ed_note.sql
+-rw-r--r--   0        0        0     8576 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr.sql
+-rw-r--r--   0        0        0     1522 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
+-rw-r--r--   0        0        0     2022 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
+-rw-r--r--   0        0        0     2747 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
+-rw-r--r--   0        0        0      794 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_study_period.sql
+-rw-r--r--   0        0        0      731 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_symptom.py
+-rw-r--r--   0        0        0    16063 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_symptom.sql
+-rw-r--r--   0        0        0     1115 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/manifest.toml
+-rw-r--r--   0        0        0      864 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_dx.sql
+-rw-r--r--   0        0        0     1569 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_pcr.sql
+-rw-r--r--   0        0        0     1540 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
+-rw-r--r--   0        0        0     1031 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_study_period.sql
+-rw-r--r--   0        0        0     2277 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_symptom.sql
+-rw-r--r--   0        0        0     2522 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/typesystem.py
+-rw-r--r--   0        0        0     1905 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
+-rw-r--r--   0        0        0     5415 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
+-rw-r--r--   0        0        0     3376 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
+-rw-r--r--   0        0        0     4037 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
+-rw-r--r--   0        0        0     4602 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
+-rw-r--r--   0        0        0     3369 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
+-rw-r--r--   0        0        0     8196 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
+-rw-r--r--   0        0        0     1099 2023-07-10 14:53:57.758326 cumulus_library_covid-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.6/PKG-INFO
```

### Comparing `cumulus_library_covid-0.1.5/README.md` & `cumulus_library_covid-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/count.py` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/count.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 def count_symptom(duration="week"):
     """
     covid_symptom__count_symptom_week
     covid_symptom__count_symptom_month
     """
     view_name = table("count_symptom", duration)
-    from_table = table("symptom")
+    from_table = table("symptom_nlp")
     cols = [
         f"author_{duration}",
         "symptom_display",
         "variant_era",
         "age_group",
         "gender",
         "race_display",
@@ -130,11 +130,13 @@
         [
             count_dx("month"),
             count_dx("week"),
             count_pcr("month"),
             count_pcr("week"),
             count_study_period("month"),
             count_study_period("week"),
+            count_symptom("week"),
+            count_symptom("month"),
             count_prevalence_ed("month"),
             count_prevalence_ed("week"),
         ]
     )
```

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/count.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/count.sql`

 * *Files 14% similar despite different names*

```diff
@@ -175,14 +175,96 @@
     gender,
     age_group,
     race_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
+CREATE TABLE covid_symptom__count_symptom_week AS
+WITH powerset AS (
+    SELECT
+        count(DISTINCT subject_ref) AS cnt_subject,
+        count(DISTINCT encounter_ref) AS cnt_encounter,
+        author_week,
+        symptom_display,
+        variant_era,
+        age_group,
+        gender,
+        race_display,
+        enc_class_code,
+        ed_note
+    FROM covid_symptom__symptom_nlp
+    GROUP BY
+        cube(
+            author_week,
+            symptom_display,
+            variant_era,
+            age_group,
+            gender,
+            race_display,
+            enc_class_code,
+            ed_note
+        )
+)
+
+SELECT
+    cnt_encounter AS cnt,
+    author_week,
+    symptom_display,
+    variant_era,
+    age_group,
+    gender,
+    race_display,
+    enc_class_code,
+    ed_note
+FROM powerset
+WHERE cnt_subject >= 10;
+
+-- ###########################################################
+CREATE TABLE covid_symptom__count_symptom_month AS
+WITH powerset AS (
+    SELECT
+        count(DISTINCT subject_ref) AS cnt_subject,
+        count(DISTINCT encounter_ref) AS cnt_encounter,
+        author_month,
+        symptom_display,
+        variant_era,
+        age_group,
+        gender,
+        race_display,
+        enc_class_code,
+        ed_note
+    FROM covid_symptom__symptom_nlp
+    GROUP BY
+        cube(
+            author_month,
+            symptom_display,
+            variant_era,
+            age_group,
+            gender,
+            race_display,
+            enc_class_code,
+            ed_note
+        )
+)
+
+SELECT
+    cnt_encounter AS cnt,
+    author_month,
+    symptom_display,
+    variant_era,
+    age_group,
+    gender,
+    race_display,
+    enc_class_code,
+    ed_note
+FROM powerset
+WHERE cnt_subject >= 10;
+
+-- ###########################################################
 CREATE TABLE covid_symptom__count_prevalence_ed_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         author_month,
         covid_dx,
```

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_age_general.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_age_general.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_age_pediatric.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_age_pediatric.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_dx_snomed.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_dx_snomed.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_ed_note.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_ed_note.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_custom.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_custom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_negative.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_negative.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_pcr_positive.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_pcr_positive.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_study_period.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_symptom.py` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_symptom.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/define_symptom.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/define_symptom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/manifest.toml` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_dx.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_dx.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_pcr.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_pcr.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_study_period.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/table_symptom.sql` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/table_symptom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/typesystem.py` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json` & `cumulus_library_covid-0.1.6/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.5/pyproject.toml` & `cumulus_library_covid-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library-covid"
-version = "0.1.5"
+version = "0.1.6"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "cumulus-library >= 0.3.0",
     "sqlfluff == 2.0.2"
 ]
```

### Comparing `cumulus_library_covid-0.1.5/PKG-INFO` & `cumulus_library_covid-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library-covid
-Version: 0.1.5
+Version: 0.1.6
 Summary: SQL generation for cumulus covid symptom analysis
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

