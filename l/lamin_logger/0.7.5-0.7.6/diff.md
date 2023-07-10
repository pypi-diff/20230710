# Comparing `tmp/lamin_logger-0.7.5.tar.gz` & `tmp/lamin_logger-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.5.tar` & `lamin_logger-0.7.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.5/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.5/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.5/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.5/docs/api.md
--rw-r--r--   0        0        0     4969 2023-07-05 09:32:52.130076 lamin_logger-0.7.5/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.5/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.5/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.5/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-07-05 09:32:45.858118 lamin_logger-0.7.5/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.5/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.5/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.7.5/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.7.5/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7515 2023-07-05 09:32:09.707180 lamin_logger-0.7.5/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.5/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.5/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.5/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.5/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.5/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.5/tests/test_lookup.py
--rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.5/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.5/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.5/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.6/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.6/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.6/docs/api.md
+-rw-r--r--   0        0        0     5120 2023-07-10 09:56:13.936880 lamin_logger-0.7.6/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.6/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.6/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.6/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-07-10 09:56:03.461997 lamin_logger-0.7.6/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.6/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.6/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.7.6/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.7.6/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7541 2023-07-10 09:54:24.354366 lamin_logger-0.7.6/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.6/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3524 2023-07-10 09:54:24.354688 lamin_logger-0.7.6/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.6/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.6/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.6/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.6/tests/test_lookup.py
+-rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.6/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.6/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.6/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.6/PKG-INFO
```

### Comparing `lamin_logger-0.7.5/.github/workflows/build.yml` & `lamin_logger-0.7.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/.gitignore` & `lamin_logger-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/.pre-commit-config.yaml` & `lamin_logger-0.7.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/LICENSE` & `lamin_logger-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/docs/changelog.md` & `lamin_logger-0.7.6/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⚡️ Speed up search 150x | [35](https://github.com/laminlabs/lamin-logger/pull/35) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-10 | 0.7.6
 🐛 Fix existing_categories for map_synonyms | [34](https://github.com/laminlabs/lamin-logger/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-05 | 0.7.5
 🚑️ Fix for multiple matches in map_synonyms | [33](https://github.com/laminlabs/lamin-logger/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-02 | 0.7.4
 🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
 🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
```

### Comparing `lamin_logger-0.7.5/docs/quickstart.ipynb` & `lamin_logger-0.7.6/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_core.py` & `lamin_logger-0.7.6/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_inspect.py` & `lamin_logger-0.7.6/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_logger.py` & `lamin_logger-0.7.6/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_lookup.py` & `lamin_logger-0.7.6/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.6/lamin_logger/_map_synonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,16 @@
         keep : {'first', 'last', False}, default 'first'
             Determines which duplicates to mark as `pandas.DataFrame.duplicated`
         sep: Splits all values of the agg_col by this separator.
 
     Returns:
         a pandas.Series index by the split values from the aggregated column
     """
-    df = df[[target_col, agg_col]].drop_duplicates()
+    df = df[[target_col, agg_col]].drop_duplicates().dropna(subset=[agg_col])
+
     # subset to df with only non-empty strings in the agg_col
     df = df.loc[not_empty_none_na(df[agg_col]).index]
 
     df[agg_col] = df[agg_col].str.split(sep)
     df_explode = df.explode(agg_col)
     # remove rows with same values in agg_col and target_col
     df_explode = df_explode[df_explode[agg_col] != df_explode[target_col]]
```

### Comparing `lamin_logger-0.7.5/lamin_logger/_python_version.py` & `lamin_logger-0.7.6/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/lamin_logger/_search.py` & `lamin_logger-0.7.6/lamin_logger/_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,43 +42,48 @@
         if return_ranked_results:
             return df
         else:
             return None
 
     # search against each of the synonyms
     if (synonyms_field in df.columns) and (synonyms_field != field):
+        # creates field_value:synonym
         mapper = explode_aggregated_column_to_map(
             df,
             agg_col=synonyms_field,  # type:ignore
             target_col=field,
             keep=keep,
             sep=synonyms_sep,
         )
         if keep is False:
             mapper = mapper.explode()
-        for v in df[field]:
-            if v not in mapper:
-                mapper.loc[v] = v
+        # adds field_value:field_value
+        df_field = pd.Series(df[field].values, index=df[field], name=field)
+        df_field.index.name = synonyms_field
+        df_field = df_field[df_field.index.difference(mapper.index)]
+        mapper = pd.concat([mapper, df_field])
         df_exp = mapper.reset_index()
         target_column = synonyms_field
     else:
         if synonyms_field == field:
             logger.warning(
                 "Input field is the same as synonyms field, skipping synonyms matching"
             )
-        df_exp = df.copy()
+        df_exp = df[[field]].copy()
         target_column = field
 
     # add matching scores as a __ratio__ column
     df_exp["__ratio__"] = _fuzz_ratio(
         string=string, iterable=df_exp[target_column], case_sensitive=case_sensitive
     )
+    # only keep the max score between field and synonyms for each entry
     df_exp_grouped = (
-        df_exp.groupby(field).max().sort_values("__ratio__", ascending=False)
+        df_exp.groupby(field).max("__ratio__").sort_values("__ratio__", ascending=False)
     )
+    # subset to original field values (as synonyms were mixed in before)
     df_exp_grouped = df_exp_grouped[df_exp_grouped.index.isin(df[field])]
     df_scored = df.set_index(field).loc[df_exp_grouped.index]
     df_scored["__ratio__"] = df_exp_grouped["__ratio__"]
 
     if return_ranked_results:
         return df_scored.sort_values("__ratio__", ascending=False)
     else:
```

### Comparing `lamin_logger-0.7.5/pyproject.toml` & `lamin_logger-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/tests/test_inspect.py` & `lamin_logger-0.7.6/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/tests/test_lookup.py` & `lamin_logger-0.7.6/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/tests/test_map_synonyms.py` & `lamin_logger-0.7.6/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/tests/test_search.py` & `lamin_logger-0.7.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.5/PKG-INFO` & `lamin_logger-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.5
+Version: 0.7.6
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

