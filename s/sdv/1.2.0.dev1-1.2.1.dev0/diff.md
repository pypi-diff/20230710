# Comparing `tmp/sdv-1.2.0.dev1.tar.gz` & `tmp/sdv-1.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdv-1.2.0.dev1.tar", last modified: Wed Jun  7 18:57:18 2023, max compression
+gzip compressed data, was "sdv-1.2.1.dev0.tar", last modified: Mon Jul 10 21:07:50 2023, max compression
```

## Comparing `sdv-1.2.0.dev1.tar` & `sdv-1.2.1.dev0.tar`

### file list

```diff
@@ -1,657 +1,657 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.669325 sdv-1.2.0.dev1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    69753 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    80589 2023-06-07 18:57:18.669595 sdv-1.2.0.dev1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.531666 sdv-1.2.0.dev1/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/Makefile
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.532636 sdv-1.2.0.dev1/docs/api_reference/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.533117 sdv-1.2.0.dev1/docs/api_reference/constraints/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.552514 sdv-1.2.0.dev1/docs/api_reference/constraints/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/base.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/constraints/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/evaluation.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.553017 sdv-1.2.0.dev1/docs/api_reference/lite/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.554771 sdv-1.2.0.dev1/docs/api_reference/lite/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.0.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/lite/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/api_reference/lite/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.555437 sdv-1.2.0.dev1/docs/api_reference/metadata/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.563780 sdv-1.2.0.dev1/docs/api_reference/metadata/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/dataset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metadata/table.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.565037 sdv-1.2.0.dev1/docs/api_reference/metrics/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.601733 sdv-1.2.0.dev1/docs/api_reference/metrics/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/demos.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/relational.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/api_reference/metrics/timeseries.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.602259 sdv-1.2.0.dev1/docs/api_reference/relational/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.603335 sdv-1.2.0.dev1/docs/api_reference/relational/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/relational/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.603750 sdv-1.2.0.dev1/docs/api_reference/sampling/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.604337 sdv-1.2.0.dev1/docs/api_reference/sampling/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sampling/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/sdv.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.605323 sdv-1.2.0.dev1/docs/api_reference/tabular/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.613580 sdv-1.2.0.dev1/docs/api_reference/tabular/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/copulas.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/tabular/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.613972 sdv-1.2.0.dev1/docs/api_reference/timeseries/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.615146 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/api_reference/timeseries/par.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/conf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.615840 sdv-1.2.0.dev1/docs/developer_guides/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/docs/developer_guides/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/overview.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.616710 sdv-1.2.0.dev1/docs/developer_guides/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/developer_guides/sdv/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.617398 sdv-1.2.0.dev1/docs/getting_started/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/getting_started/quickstart.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.629065 sdv-1.2.0.dev1/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/CTGAN-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/Copulas-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/DataCebo-Blue.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.0.dev1/docs/images/DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/DeepEcho-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/RDT-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/Real-vs-Synthetic-Evaluation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDGym-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDMetrics-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDV-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/SDV-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/SDV.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/Single-Table-Metadata-Example.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/images/custom_constraint.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/datacebo-logo-dark-mode.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/images/datacebo-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/google_colab.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/hma1_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/metadata_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/metadata_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/mybinder.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.0.dev1/docs/images/quickstart_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.0.dev1/docs/images/rdt_main_tranformation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/images/slack.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/make.bat
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631152 sdv-1.2.0.dev1/docs/savefig/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_3.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.0.dev1/docs/savefig/experience_years_3.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.524823 sdv-1.2.0.dev1/docs/sdv_theme/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631402 sdv-1.2.0.dev1/docs/sdv_theme/static/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/sdv_theme/static/slack-32.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.631652 sdv-1.2.0.dev1/docs/user_guides/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.632964 sdv-1.2.0.dev1/docs/user_guides/benchmarking/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/datasets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/docker.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/run.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/benchmarking/synthesizers.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.633739 sdv-1.2.0.dev1/docs/user_guides/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/evaluation_framework.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/evaluation/synthetic_data_metrics.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.634806 sdv-1.2.0.dev1/docs/user_guides/relational/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/relational/relational_metadata.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.638035 sdv-1.2.0.dev1/docs/user_guides/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/custom_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/gaussian_copula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/handling_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/table_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/tabular_preset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.0.dev1/docs/user_guides/single_table/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.638700 sdv-1.2.0.dev1/docs/user_guides/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.0.dev1/docs/user_guides/timeseries/par.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.639898 sdv-1.2.0.dev1/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-06-06 20:54:02.000000 sdv-1.2.0.dev1/sdv/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.642558 sdv-1.2.0.dev1/sdv/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18056 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/constraints/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/constraints/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    53574 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/constraints/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5822 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/constraints/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.644002 sdv-1.2.0.dev1/sdv/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    34822 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/data_processing/data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/sdv/data_processing/datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/data_processing/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.644575 sdv-1.2.0.dev1/sdv/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/datasets/local.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/errors.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.645120 sdv-1.2.0.dev1/sdv/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/evaluation/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.645444 sdv-1.2.0.dev1/sdv/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/lite/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.647597 sdv-1.2.0.dev1/sdv/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/metadata/anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/metadata/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/metadata/single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/metadata/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/sdv/metadata/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.648575 sdv-1.2.0.dev1/sdv/metrics/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/relational.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/metrics/timeseries.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.649280 sdv-1.2.0.dev1/sdv/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20699 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/multi_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23027 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/multi_table/hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.650300 sdv-1.2.0.dev1/sdv/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      103 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8638 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/sdv/sampling/hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/sdv/sampling/independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/sdv/sampling/tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.650695 sdv-1.2.0.dev1/sdv/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/sequential/par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.652288 sdv-1.2.0.dev1/sdv/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/sdv/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45383 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/sdv/single_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/sdv/single_table/copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/single_table/copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/sdv/single_table/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/single_table/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/sdv/single_table/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/sdv/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.641094 sdv-1.2.0.dev1/sdv.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    80589 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35730 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1479 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-06-07 18:57:18.000000 sdv-1.2.0.dev1/sdv.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-06-07 18:57:18.670143 sdv-1.2.0.dev1/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3853 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.652726 sdv-1.2.0.dev1/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653101 sdv-1.2.0.dev1/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653357 sdv-1.2.0.dev1/tests/integration/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/integration/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/dataset.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.653672 sdv-1.2.0.dev1/tests/integration/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/datasets/test_demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.654191 sdv-1.2.0.dev1/tests/integration/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.654484 sdv-1.2.0.dev1/tests/integration/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/tests/integration/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.655225 sdv-1.2.0.dev1/tests/integration/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.655542 sdv-1.2.0.dev1/tests/integration/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22620 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/tests/integration/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.656222 sdv-1.2.0.dev1/tests/integration/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.657530 sdv-1.2.0.dev1/tests/integration/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/custom_constraints.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29343 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/integration/single_table/test_ctgan.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.657713 sdv-1.2.0.dev1/tests/readme_test/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.0.dev1/tests/readme_test/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.658443 sdv-1.2.0.dev1/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.659978 sdv-1.2.0.dev1/tests/unit/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6700 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/constraints/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.661084 sdv-1.2.0.dev1/tests/unit/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    79609 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/data_processing/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.661640 sdv-1.2.0.dev1/tests/unit/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/test_demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/datasets/test_local.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.662002 sdv-1.2.0.dev1/tests/unit/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.662332 sdv-1.2.0.dev1/tests/unit/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.664714 sdv-1.2.0.dev1/tests/unit/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.665571 sdv-1.2.0.dev1/tests/unit/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41567 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/multi_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    28011 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.666673 sdv-1.2.0.dev1/tests/unit/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.0.dev1/tests/unit/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13830 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-05 19:46:25.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.0.dev1/tests/unit/sampling/test_tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.667345 sdv-1.2.0.dev1/tests/unit/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-07 18:57:18.669050 sdv-1.2.0.dev1/tests/unit/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-01 02:59:19.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 18:56:41.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.0.dev1/tests/unit/single_table/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-06 20:45:58.000000 sdv-1.2.0.dev1/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-05-25 15:59:25.000000 sdv-1.2.0.dev1/tests/unit/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.0.dev1/tests/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.263517 sdv-1.2.1.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.1.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    69753 2023-06-20 19:05:28.000000 sdv-1.2.1.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.1.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    80539 2023-07-10 21:07:50.263777 sdv-1.2.1.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.137098 sdv-1.2.1.dev0/docs/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/Makefile
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.138242 sdv-1.2.1.dev0/docs/api_reference/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.138786 sdv-1.2.1.dev0/docs/api_reference/constraints/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.158897 sdv-1.2.1.dev0/docs/api_reference/constraints/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/base.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/api_reference/constraints/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/evaluation.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/api_reference/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.159396 sdv-1.2.1.dev0/docs/api_reference/lite/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.161354 sdv-1.2.1.dev0/docs/api_reference/lite/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.1.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/api_reference/lite/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/api_reference/lite/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.162199 sdv-1.2.1.dev0/docs/api_reference/metadata/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.170486 sdv-1.2.1.dev0/docs/api_reference/metadata/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/dataset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/metadata/table.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.171748 sdv-1.2.1.dev0/docs/api_reference/metrics/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.207710 sdv-1.2.1.dev0/docs/api_reference/metrics/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/demos.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/relational.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/api_reference/metrics/timeseries.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.208145 sdv-1.2.1.dev0/docs/api_reference/relational/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.209208 sdv-1.2.1.dev0/docs/api_reference/relational/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/relational/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.209606 sdv-1.2.1.dev0/docs/api_reference/sampling/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.210181 sdv-1.2.1.dev0/docs/api_reference/sampling/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/sampling/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/sampling/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/sdv.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.211142 sdv-1.2.1.dev0/docs/api_reference/tabular/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.218820 sdv-1.2.1.dev0/docs/api_reference/tabular/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/copulas.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/tabular/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.219288 sdv-1.2.1.dev0/docs/api_reference/timeseries/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.220484 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/api_reference/timeseries/par.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/conf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.221201 sdv-1.2.1.dev0/docs/developer_guides/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/docs/developer_guides/contributing.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/developer_guides/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/developer_guides/overview.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.222081 sdv-1.2.1.dev0/docs/developer_guides/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/developer_guides/sdv/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/developer_guides/sdv/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/developer_guides/sdv/metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/developer_guides/sdv/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.222718 sdv-1.2.1.dev0/docs/getting_started/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/getting_started/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/getting_started/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/getting_started/quickstart.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/history.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.233498 sdv-1.2.1.dev0/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/CTGAN-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/Copulas-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/DataCebo-Blue.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.1.dev0/docs/images/DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/DeepEcho-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/RDT-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/images/Real-vs-Synthetic-Evaluation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/SDGym-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/SDMetrics-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/SDV-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/images/SDV-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/SDV.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/images/Single-Table-Metadata-Example.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/images/custom_constraint.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/images/datacebo-logo-dark-mode.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/images/datacebo-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/google_colab.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.1.dev0/docs/images/hma1_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.1.dev0/docs/images/metadata_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.1.dev0/docs/images/metadata_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/mybinder.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.1.dev0/docs/images/quickstart_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.1.dev0/docs/images/rdt_main_tranformation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/images/slack.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/docs/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/make.bat
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.235387 sdv-1.2.1.dev0/docs/savefig/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_3.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.1.dev0/docs/savefig/experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.1.dev0/docs/savefig/experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.1.dev0/docs/savefig/experience_years_3.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.129047 sdv-1.2.1.dev0/docs/sdv_theme/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.235718 sdv-1.2.1.dev0/docs/sdv_theme/static/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/sdv_theme/static/slack-32.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.235976 sdv-1.2.1.dev0/docs/user_guides/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.237244 sdv-1.2.1.dev0/docs/user_guides/benchmarking/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/datasets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/docker.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/run.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/benchmarking/synthesizers.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.237983 sdv-1.2.1.dev0/docs/user_guides/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/user_guides/evaluation/evaluation_framework.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/user_guides/evaluation/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/user_guides/evaluation/synthetic_data_metrics.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.239011 sdv-1.2.1.dev0/docs/user_guides/relational/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/relational/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/relational/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/user_guides/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/relational/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/relational/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/relational/relational_metadata.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.241997 sdv-1.2.1.dev0/docs/user_guides/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/custom_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/gaussian_copula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/handling_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/table_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/tabular_preset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.1.dev0/docs/user_guides/single_table/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.242570 sdv-1.2.1.dev0/docs/user_guides/timeseries/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/docs/user_guides/timeseries/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.1.dev0/docs/user_guides/timeseries/par.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.243033 sdv-1.2.1.dev0/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-06-07 20:46:27.000000 sdv-1.2.1.dev0/sdv/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.244848 sdv-1.2.1.dev0/sdv/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18056 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/constraints/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/constraints/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54000 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/constraints/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5830 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/constraints/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.245734 sdv-1.2.1.dev0/sdv/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    34822 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/data_processing/data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.1.dev0/sdv/data_processing/datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/data_processing/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/data_processing/numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/data_processing/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.246188 sdv-1.2.1.dev0/sdv/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/datasets/demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/datasets/local.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/errors.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.246659 sdv-1.2.1.dev0/sdv/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/evaluation/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/evaluation/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.246998 sdv-1.2.1.dev0/sdv/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/sdv/lite/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.248219 sdv-1.2.1.dev0/sdv/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/sdv/metadata/anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/metadata/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/metadata/metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/metadata/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/metadata/single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/metadata/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.1.dev0/sdv/metadata/visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.248960 sdv-1.2.1.dev0/sdv/metrics/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/metrics/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/metrics/demos.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/metrics/relational.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/metrics/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/metrics/timeseries.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.249479 sdv-1.2.1.dev0/sdv/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20683 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/multi_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15744 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/multi_table/hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.250112 sdv-1.2.1.dev0/sdv/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      302 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8640 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/sampling/hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/sampling/independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/sdv/sampling/tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.250409 sdv-1.2.1.dev0/sdv/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/sdv/sequential/par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.251513 sdv-1.2.1.dev0/sdv/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45468 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/sdv/single_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/single_table/copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/sdv/single_table/copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/sdv/single_table/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/single_table/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/sdv/single_table/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/sdv/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.243987 sdv-1.2.1.dev0/sdv.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    80539 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35730 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1489 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-10 21:07:50.000000 sdv-1.2.1.dev0/sdv.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-07-10 21:07:50.264390 sdv-1.2.1.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3814 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.251786 sdv-1.2.1.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.252059 sdv-1.2.1.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.252328 sdv-1.2.1.dev0/tests/integration/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/integration/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/dataset.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.252756 sdv-1.2.1.dev0/tests/integration/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/datasets/test_demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.253371 sdv-1.2.1.dev0/tests/integration/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.253679 sdv-1.2.1.dev0/tests/integration/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/tests/integration/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.254392 sdv-1.2.1.dev0/tests/integration/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/integration/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.254696 sdv-1.2.1.dev0/tests/integration/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23356 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/tests/integration/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.255234 sdv-1.2.1.dev0/tests/integration/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.256254 sdv-1.2.1.dev0/tests/integration/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/single_table/custom_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    36264 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/tests/integration/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/integration/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/integration/single_table/test_ctgan.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.256443 sdv-1.2.1.dev0/tests/readme_test/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.1.dev0/tests/readme_test/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.256974 sdv-1.2.1.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.257680 sdv-1.2.1.dev0/tests/unit/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/unit/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.1.dev0/tests/unit/constraints/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/constraints/test_tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6848 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/tests/unit/constraints/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.258496 sdv-1.2.1.dev0/tests/unit/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    79609 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.1.dev0/tests/unit/data_processing/test_datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/data_processing/test_numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/data_processing/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.258929 sdv-1.2.1.dev0/tests/unit/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/datasets/test_demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/datasets/test_local.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.259256 sdv-1.2.1.dev0/tests/unit/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.259548 sdv-1.2.1.dev0/tests/unit/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/unit/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/unit/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.260393 sdv-1.2.1.dev0/tests/unit/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/unit/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/unit/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/metadata/test_metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.260900 sdv-1.2.1.dev0/tests/unit/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41567 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/multi_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19731 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/tests/unit/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.261699 sdv-1.2.1.dev0/tests/unit/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.1.dev0/tests/unit/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13827 2023-07-10 21:05:50.000000 sdv-1.2.1.dev0/tests/unit/sampling/test_hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/sampling/test_independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.1.dev0/tests/unit/sampling/test_tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.262045 sdv-1.2.1.dev0/tests/unit/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/unit/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 21:07:50.263376 sdv-1.2.1.dev0/tests/unit/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/single_table/test_copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/unit/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/unit/single_table/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.1.dev0/tests/unit/single_table/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-06-07 20:46:09.000000 sdv-1.2.1.dev0/tests/unit/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.1.dev0/tests/utils.py
```

### Comparing `sdv-1.2.0.dev1/CONTRIBUTING.rst` & `sdv-1.2.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/HISTORY.md` & `sdv-1.2.1.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/LICENSE` & `sdv-1.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/PKG-INFO` & `sdv-1.2.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.0.dev1
+Version: 1.2.1.dev0
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: pomegranate
 License-File: LICENSE
 License-File: AUTHORS.rst
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev1 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.1.dev0 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7,<3.11 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev Provides-Extra:
-pomegranate License-File: LICENSE License-File: AUTHORS.rst
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.11
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+dev Provides-Extra: pomegranate License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
         [![Dev Status](https://img.shields.io/badge/Dev%20Status-5%20--
             %20Production%2fStable-green)](https://pypi.org/search/
 ?c=Development+Status+%3A%3A+5+-+Production%2FStable) [![PyPi Shield](https://
    img.shields.io/pypi/v/SDV.svg)](https://pypi.python.org/pypi/SDV) [![Unit
```

### Comparing `sdv-1.2.0.dev1/README.md` & `sdv-1.2.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/Makefile` & `sdv-1.2.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/constraints/tabular.rst` & `sdv-1.2.1.dev0/docs/api_reference/constraints/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst` & `sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst` & `sdv-1.2.1.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metadata/dataset.rst` & `sdv-1.2.1.dev0/docs/api_reference/metadata/dataset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metadata/table.rst` & `sdv-1.2.1.dev0/docs/api_reference/metadata/table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/relational.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/relational.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/tabular.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/metrics/timeseries.rst` & `sdv-1.2.1.dev0/docs/api_reference/metrics/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst` & `sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst` & `sdv-1.2.1.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/conf.py` & `sdv-1.2.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/developer_guides/contributing.rst` & `sdv-1.2.1.dev0/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/developer_guides/overview.rst` & `sdv-1.2.1.dev0/docs/developer_guides/overview.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/developer_guides/sdv/constraints.rst` & `sdv-1.2.1.dev0/docs/developer_guides/sdv/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/developer_guides/sdv/metadata.rst` & `sdv-1.2.1.dev0/docs/developer_guides/sdv/metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/developer_guides/sdv/tabular.rst` & `sdv-1.2.1.dev0/docs/developer_guides/sdv/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/getting_started/install.rst` & `sdv-1.2.1.dev0/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/getting_started/quickstart.rst` & `sdv-1.2.1.dev0/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/CTGAN-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/CTGAN-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/Copulas-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/Copulas-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/DataCebo-Blue.png` & `sdv-1.2.1.dev0/docs/images/DataCebo-Blue.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/DataCebo.png` & `sdv-1.2.1.dev0/docs/images/DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/DeepEcho-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/DeepEcho-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/RDT-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/RDT-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/Real-vs-Synthetic-Evaluation.png` & `sdv-1.2.1.dev0/docs/images/Real-vs-Synthetic-Evaluation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/SDGym-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/SDGym-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/SDMetrics-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/SDMetrics-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/SDV-DataCebo.png` & `sdv-1.2.1.dev0/docs/images/SDV-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/SDV-logo.png` & `sdv-1.2.1.dev0/docs/images/SDV-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/SDV.png` & `sdv-1.2.1.dev0/docs/images/SDV.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/Single-Table-Metadata-Example.png` & `sdv-1.2.1.dev0/docs/images/Single-Table-Metadata-Example.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/custom_constraint.png` & `sdv-1.2.1.dev0/docs/images/custom_constraint.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/datacebo-logo-dark-mode.png` & `sdv-1.2.1.dev0/docs/images/datacebo-logo-dark-mode.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/datacebo-logo.png` & `sdv-1.2.1.dev0/docs/images/datacebo-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/google_colab.png` & `sdv-1.2.1.dev0/docs/images/google_colab.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/hma1_1.png` & `sdv-1.2.1.dev0/docs/images/hma1_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/metadata_1.png` & `sdv-1.2.1.dev0/docs/images/metadata_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/metadata_2.png` & `sdv-1.2.1.dev0/docs/images/metadata_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/mybinder.png` & `sdv-1.2.1.dev0/docs/images/mybinder.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/quickstart_1.png` & `sdv-1.2.1.dev0/docs/images/quickstart_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/rdt_main_tranformation.png` & `sdv-1.2.1.dev0/docs/images/rdt_main_tranformation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/images/slack.png` & `sdv-1.2.1.dev0/docs/images/slack.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/index.rst` & `sdv-1.2.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/make.bat` & `sdv-1.2.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_1.png` & `sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_2.png` & `sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/copulagan_experience_years_3.png` & `sdv-1.2.1.dev0/docs/savefig/copulagan_experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/experience_years_1.png` & `sdv-1.2.1.dev0/docs/savefig/experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/experience_years_2.png` & `sdv-1.2.1.dev0/docs/savefig/experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/savefig/experience_years_3.png` & `sdv-1.2.1.dev0/docs/savefig/experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/sdv_theme/static/slack-32.png` & `sdv-1.2.1.dev0/docs/sdv_theme/static/slack-32.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/datasets.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/datasets.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/docker.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/docker.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/index.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/install.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/run.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/run.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/benchmarking/synthesizers.rst` & `sdv-1.2.1.dev0/docs/user_guides/benchmarking/synthesizers.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/evaluation/evaluation_framework.rst` & `sdv-1.2.1.dev0/docs/user_guides/evaluation/evaluation_framework.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/relational/constraints.rst` & `sdv-1.2.1.dev0/docs/user_guides/relational/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/relational/hma1.rst` & `sdv-1.2.1.dev0/docs/user_guides/relational/hma1.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/relational/relational_metadata.rst` & `sdv-1.2.1.dev0/docs/user_guides/relational/relational_metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/copulagan.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/copulagan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/ctgan.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/ctgan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/custom_constraints.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/custom_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/gaussian_copula.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/gaussian_copula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/handling_constraints.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/handling_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/index.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/tabular_preset.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/tabular_preset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/single_table/tvae.rst` & `sdv-1.2.1.dev0/docs/user_guides/single_table/tvae.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/docs/user_guides/timeseries/par.rst` & `sdv-1.2.1.dev0/docs/user_guides/timeseries/par.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/__init__.py` & `sdv-1.2.1.dev0/sdv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # configure logging for the library with a null handler (nothing is printed by default). See
 # http://docs.python-guide.org/en/latest/writing/logging/
 
 """Top-level package for SDV."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.2.0.dev1'
+__version__ = '1.2.1.dev0'
 
 
 import sys
 import warnings
 from operator import attrgetter
 
 from pkg_resources import iter_entry_points
```

### Comparing `sdv-1.2.0.dev1/sdv/constraints/__init__.py` & `sdv-1.2.1.dev0/sdv/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/constraints/base.py` & `sdv-1.2.1.dev0/sdv/constraints/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/constraints/errors.py` & `sdv-1.2.1.dev0/sdv/constraints/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/constraints/tabular.py` & `sdv-1.2.1.dev0/sdv/constraints/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,17 +677,20 @@
                 Table data.
 
         Returns:
             pandas.DataFrame:
                 Transformed data.
         """
         column = table_data[self._column_name].to_numpy()
-        diff_column = abs(column - self._value)
         if self._is_datetime:
+            column = cast_to_datetime64(column)
+            diff_column = abs(column - self._value)
             diff_column = diff_column.astype(np.float64)
+        else:
+            diff_column = abs(column - self._value)
 
         self._diff_column_name = create_unique_name(self._diff_column_name, table_data.columns)
         table_data[self._diff_column_name] = np.log(diff_column + 1)
         return table_data.drop(self._column_name, axis=1)
 
     def _reverse_transform(self, table_data):
         """Reverse transform the table data.
@@ -705,15 +708,15 @@
                 Transformed data.
         """
         diff_column = np.exp(table_data[self._diff_column_name]) - 1
         if self._dtype != np.dtype('float'):
             diff_column = diff_column.round()
 
         if self._is_datetime:
-            diff_column = diff_column.astype('timedelta64[ns]')
+            diff_column = convert_to_timedelta(diff_column)
 
         if self._operator in [np.greater, np.greater_equal]:
             original_column = self._value + diff_column
         else:
             original_column = self._value - diff_column
 
         table_data[self._column_name] = pd.Series(original_column).astype(self._dtype)
@@ -910,17 +913,18 @@
             table_data (pandas.DataFrame):
                 Table data.
 
         Returns:
             pandas.DataFrame:
                 Transformed data.
         """
-        low = table_data[self.low_column_name]
-        middle = table_data[self.middle_column_name]
-        high = table_data[self.high_column_name]
+        # Using ``to_numpy`` since ``get_datetime_diff`` requires ``numpy.ndarray``
+        low = table_data[self.low_column_name].to_numpy()
+        middle = table_data[self.middle_column_name].to_numpy()
+        high = table_data[self.high_column_name].to_numpy()
 
         if self._is_datetime:
             low_diff_column = get_datetime_diff(middle, low, self._dtype)
             high_diff_column = get_datetime_diff(high, middle, self._dtype)
         else:
             low_diff_column = middle - low
             high_diff_column = high - middle
@@ -1111,14 +1115,17 @@
 
         Returns:
             pandas.Series:
                 Whether each row is valid.
         """
         data = table_data[self._column_name]
 
+        if self._is_datetime:
+            data = cast_to_datetime64(data)
+
         satisfy_low_bound = np.logical_or(
             self._operator(self._low_value, data),
             np.isnan(self._low_value),
         )
         satisfy_high_bound = np.logical_or(
             self._operator(data, self._high_value),
             np.isnan(self._high_value),
@@ -1140,15 +1147,19 @@
             table_data (pandas.DataFrame):
                 Table data.
 
         Returns:
             pandas.DataFrame:
                 Transformed data.
         """
-        data = logit(table_data[self._column_name], self._low_value, self._high_value)
+        data = table_data[self._column_name]
+        if self._is_datetime:
+            data = cast_to_datetime64(table_data[self._column_name])
+
+        data = logit(data, self._low_value, self._high_value)
         table_data[self._transformed_column] = data
         table_data = table_data.drop(self._column_name, axis=1)
 
         return table_data
 
     def _reverse_transform(self, table_data):
         """Reverse transform the table data.
```

### Comparing `sdv-1.2.0.dev1/sdv/constraints/utils.py` & `sdv-1.2.1.dev0/sdv/constraints/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
     Return:
         ``numpy.datetime64`` value or values.
     """
     if isinstance(value, str):
         value = pd.to_datetime(value).to_datetime64()
     elif isinstance(value, pd.Series):
-        value.apply(lambda x: pd.to_datetime(x).to_datetime64())
         value = value.astype('datetime64[ns]')
     elif isinstance(value, (np.ndarray, list)):
         value = np.array([
             pd.to_datetime(item).to_datetime64()
+            if not pd.isna(item)
+            else pd.NaT.to_datetime64()
             for item in value
         ])
 
     return value
 
 
 def matches_datetime_format(value, datetime_format):
```

### Comparing `sdv-1.2.0.dev1/sdv/data_processing/data_processor.py` & `sdv-1.2.1.dev0/sdv/data_processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/data_processing/datetime_formatter.py` & `sdv-1.2.1.dev0/sdv/data_processing/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/data_processing/errors.py` & `sdv-1.2.1.dev0/sdv/data_processing/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/data_processing/numerical_formatter.py` & `sdv-1.2.1.dev0/sdv/data_processing/numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/data_processing/utils.py` & `sdv-1.2.1.dev0/sdv/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/datasets/demo.py` & `sdv-1.2.1.dev0/sdv/datasets/demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/datasets/local.py` & `sdv-1.2.1.dev0/sdv/datasets/local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/errors.py` & `sdv-1.2.1.dev0/sdv/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/evaluation/multi_table.py` & `sdv-1.2.1.dev0/sdv/evaluation/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/evaluation/single_table.py` & `sdv-1.2.1.dev0/sdv/evaluation/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/lite/single_table.py` & `sdv-1.2.1.dev0/sdv/lite/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/anonymization.py` & `sdv-1.2.1.dev0/sdv/metadata/anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/metadata_upgrader.py` & `sdv-1.2.1.dev0/sdv/metadata/metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/multi_table.py` & `sdv-1.2.1.dev0/sdv/metadata/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/single_table.py` & `sdv-1.2.1.dev0/sdv/metadata/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/utils.py` & `sdv-1.2.1.dev0/sdv/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/metadata/visualization.py` & `sdv-1.2.1.dev0/sdv/metadata/visualization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/multi_table/base.py` & `sdv-1.2.1.dev0/sdv/multi_table/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 
         return pbar_args
 
     def _print(self, text='', **kwargs):
         if self.verbose:
             print(text, **kwargs)  # noqa: T001
 
-    def __init__(self, metadata, locales=None, synthesizer_kwargs=None, verbose=True):
+    def __init__(self, metadata, locales=None, synthesizer_kwargs=None):
         self.metadata = metadata
         self.metadata.validate()
         self.locales = locales
-        self.verbose = verbose
+        self.verbose = False
         self._table_synthesizers = {}
         self._table_parameters = defaultdict(dict)
         if synthesizer_kwargs is not None:
             warn_message = (
                 'The `synthesizer_kwargs` parameter is deprecated as of SDV 1.2.0 and does not '
                 'affect the synthesizer. Please use the `set_table_parameters` method instead.'
             )
```

### Comparing `sdv-1.2.0.dev1/sdv/sampling/hierarchical_sampler.py` & `sdv-1.2.1.dev0/sdv/sampling/hierarchical_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 Number of rows to sample.
 
         Returns:
             pandas.DataFrame:
                 Sampled rows, shape (, num_rows)
         """
         num_rows = num_rows or synthesizer._num_rows
-        return synthesizer._sample_batch(num_rows, remove_extra_columns=False)
+        return synthesizer._sample_batch(int(num_rows), keep_extra_columns=True)
 
     def _get_num_rows_from_parent(self, parent_row, child_name, foreign_key):
         """Get the number of rows to sample for the child from the parent row."""
         num_rows_key = f'__{child_name}__{foreign_key}__num_rows'
         num_rows = 0
         if num_rows_key in parent_row.keys():
             num_rows = parent_row[num_rows_key]
```

### Comparing `sdv-1.2.0.dev1/sdv/sampling/independent_sampler.py` & `sdv-1.2.1.dev0/sdv/sampling/independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/sampling/tabular.py` & `sdv-1.2.1.dev0/sdv/sampling/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/sequential/par.py` & `sdv-1.2.1.dev0/sdv/sequential/par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/single_table/base.py` & `sdv-1.2.1.dev0/sdv/single_table/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,28 +590,30 @@
                 The dictionary of conditioning values in the original format.
             transformed_conditions (dict):
                 The dictionary of conditioning values transformed to the model format.
             float_rtol (float):
                 Maximum tolerance when considering a float match.
             previous_rows (pandas.DataFrame):
                 Valid rows sampled in the previous iterations.
-            remove_extra_columns (bool):
+            keep_extra_columns (bool):
                 Whether to keep extra columns from the sampled data. Defaults to False.
 
         Returns:
             tuple:
                 * pandas.DataFrame:
                     Rows from the sampled data that match the conditions.
                 * int:
                     Number of rows that are considered valid.
         """
-        if not self._random_state_set:
+        if self._model and not self._random_state_set:
             self._set_random_state(FIXED_RNG_SEED)
 
-        if self._data_processor.get_sdtypes(primary_keys=False):
+        need_sample = self._data_processor.get_sdtypes(primary_keys=False) or keep_extra_columns
+        if self._model and need_sample:
+
             if conditions is None:
                 raw_sampled = self._sample(num_rows)
             else:
                 try:
                     raw_sampled = self._sample(num_rows, transformed_conditions)
                 except NotImplementedError:
                     raw_sampled = self._sample(num_rows)
@@ -678,15 +680,15 @@
                 Maximum tolerance when considering a float match.
             progress_bar (tqdm.tqdm or None):
                 The progress bar to update when sampling. If None, a new tqdm progress
                 bar will be created.
             output_file_path (str or None):
                 The file to periodically write sampled rows to. If None, does not write
                 rows anywhere.
-            remove_extra_columns (bool):
+            keep_extra_columns (bool):
                 Whether to keep extra columns from the sampled data. Defaults to False.
 
         Returns:
             pandas.DataFrame:
                 Sampled data.
         """
         num_rows_to_sample = batch_size
```

### Comparing `sdv-1.2.0.dev1/sdv/single_table/copulagan.py` & `sdv-1.2.1.dev0/sdv/single_table/copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/single_table/copulas.py` & `sdv-1.2.1.dev0/sdv/single_table/copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/single_table/ctgan.py` & `sdv-1.2.1.dev0/sdv/single_table/ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/single_table/utils.py` & `sdv-1.2.1.dev0/sdv/single_table/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv/utils.py` & `sdv-1.2.1.dev0/sdv/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv.egg-info/PKG-INFO` & `sdv-1.2.1.dev0/sdv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.0.dev1
+Version: 1.2.1.dev0
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: pomegranate
 License-File: LICENSE
 License-File: AUTHORS.rst
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.0.dev1 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.1.dev0 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7,<3.11 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev Provides-Extra:
-pomegranate License-File: LICENSE License-File: AUTHORS.rst
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.11
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+dev Provides-Extra: pomegranate License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
         [![Dev Status](https://img.shields.io/badge/Dev%20Status-5%20--
             %20Production%2fStable-green)](https://pypi.org/search/
 ?c=Development+Status+%3A%3A+5+-+Production%2FStable) [![PyPi Shield](https://
    img.shields.io/pypi/v/SDV.svg)](https://pypi.python.org/pypi/SDV) [![Unit
```

### Comparing `sdv-1.2.0.dev1/sdv.egg-info/SOURCES.txt` & `sdv-1.2.1.dev0/sdv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/sdv.egg-info/requires.txt` & `sdv-1.2.1.dev0/sdv.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 rdt<2,>=1.5.0
 sdmetrics<0.11,>=0.10.0
 cloudpickle<3.0,>=2.1.0
 boto3<2,>=1.15.0
 botocore<2,>=1.18
 
 [:python_version < "3.10"]
-numpy<2,>=1.20.0
+numpy<1.25.0,>=1.20.0
 pandas>=1.1.3
 
 [:python_version >= "3.10"]
-numpy<2,>=1.23.3
+numpy<1.25.0,>=1.23.3
 pandas>=1.5.0
 
 [dev]
 bumpversion<0.6,>=0.5.3
 pip>=9.0.1
 watchdog<0.9,>=0.8.3
 docutils<0.18,>=0.12
```

### Comparing `sdv-1.2.0.dev1/setup.cfg` & `sdv-1.2.1.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0.dev1
+current_version = 1.2.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdv-1.2.0.dev1/setup.py` & `sdv-1.2.1.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 with open('HISTORY.md', encoding='utf-8') as history_file:
     history = history_file.read()
 
 
 install_requires = [
     'Faker>=10,<15',
     'graphviz>=0.13.2,<1',
-    "numpy>=1.20.0,<2;python_version<'3.10'",
-    "numpy>=1.23.3,<2;python_version>='3.10'",
+    "numpy>=1.20.0,<1.25.0;python_version<'3.10'",
+    "numpy>=1.23.3,<1.25.0;python_version>='3.10'",
     "pandas>=1.1.3;python_version<'3.10'",
     "pandas>=1.5.0;python_version>='3.10'",
     'tqdm>=4.15,<5',
     'copulas>=0.9.0,<0.10',
     'ctgan>=0.7.2,<0.8',
     'deepecho>=0.4.1,<0.5',
     'rdt>=1.5.0,<2',
@@ -107,15 +107,14 @@
     author_email='info@sdv.dev',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: Free for non-commercial use',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     description='Generate synthetic data for single table, multi table and sequential data',
     extras_require={
@@ -127,15 +126,15 @@
     install_requires=install_requires,
     keywords='sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table',
     license='BSL-1.1',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     name='sdv',
     packages=find_packages(include=['sdv', 'sdv.*']),
-    python_requires='>=3.7,<3.11',
+    python_requires='>=3.8,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDV',
-    version='1.2.0.dev1',
+    version='1.2.1.dev0',
     zip_safe=False,
 )
```

### Comparing `sdv-1.2.0.dev1/tests/integration/data_processing/test_data_processor.py` & `sdv-1.2.1.dev0/tests/integration/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/dataset.py` & `sdv-1.2.1.dev0/tests/integration/dataset.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/datasets/test_demo.py` & `sdv-1.2.1.dev0/tests/integration/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/evaluation/test_multi_table.py` & `sdv-1.2.1.dev0/tests/integration/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/evaluation/test_single_table.py` & `sdv-1.2.1.dev0/tests/integration/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/lite/test_single_table.py` & `sdv-1.2.1.dev0/tests/integration/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/metadata/test_anonymization.py` & `sdv-1.2.1.dev0/tests/integration/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/metadata/test_multi_table.py` & `sdv-1.2.1.dev0/tests/integration/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/metadata/test_single_table.py` & `sdv-1.2.1.dev0/tests/integration/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/multi_table/test_hma.py` & `sdv-1.2.1.dev0/tests/integration/multi_table/test_hma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import re
 
 import numpy as np
 import pandas as pd
 import pkg_resources
 import pytest
 from faker import Faker
 
@@ -682,7 +683,32 @@
     synthesizer.validate(datasets)
     synthesizer.fit(datasets)
     synthetic_data = synthesizer.sample(scale=1)
     synthesizer.validate(synthetic_data)
 
     for table in metadata.tables:
         assert set(synthetic_data[table].columns) == set(datasets[table].columns)
+
+
+def test_progress_bar_print(capsys):
+    """Test that the progress bar prints correctly."""
+    # Setup
+    data, metadata = download_demo('multi_table', 'got_families')
+    hmasynthesizer = HMASynthesizer(metadata)
+
+    key_phrases = [
+        r'Preprocess Tables:',
+        r'Learning relationships:',
+        r"\(1/2\) Tables 'characters' and 'character_families' \('character_id'\):",
+        r"\(2/2\) Tables 'families' and 'character_families' \('family_id'\):"
+    ]
+
+    # Run
+    hmasynthesizer.fit(data)
+    hmasynthesizer.sample(0.5)
+
+    captured = capsys.readouterr()
+
+    # Assert
+    for pattern in key_phrases:
+        match = re.search(pattern, captured.out + captured.err)
+        assert match is not None
```

### Comparing `sdv-1.2.0.dev1/tests/integration/sequential/test_par.py` & `sdv-1.2.1.dev0/tests/integration/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/single_table/custom_constraints.py` & `sdv-1.2.1.dev0/tests/integration/single_table/custom_constraints.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/single_table/test_base.py` & `sdv-1.2.1.dev0/tests/integration/single_table/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -806,14 +806,271 @@
     synthesizer.validate(sampled)
     _sampled = sampled[~sampled['checkout_date'].isna()]
     assert all(
         pd.to_datetime(_sampled['checkin_date']) < pd.to_datetime(_sampled['checkout_date'])
     )
 
 
+def test_inequality_constraint_with_datetimes_and_nones():
+    """Test that the ``Inequality`` constraint works with ``None`` and ``datetime``."""
+    # Setup
+    data = pd.DataFrame(data={
+        'A': [None, None, '2020-01-02', '2020-03-04'] * 2,
+        'B': [None, '2021-03-04', '2021-12-31', None] * 2
+    })
+
+    metadata = SingleTableMetadata.load_from_dict({
+        'columns': {
+            'A': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'},
+            'B': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'}
+        }
+    })
+
+    metadata.validate()
+    synth = GaussianCopulaSynthesizer(metadata)
+    synth.add_constraints([
+        {
+            'constraint_class': 'Inequality',
+            'constraint_parameters': {
+                'low_column_name': 'A',
+                'high_column_name': 'B'
+            }
+        }
+    ])
+    synth.validate(data)
+
+    # Run
+    synth.fit(data)
+    sampled = synth.sample(10)
+
+    # Assert
+    expected_sampled = pd.DataFrame({
+        'A': {
+            0: '2020-01-02',
+            1: '2019-10-30',
+            2: np.nan,
+            3: np.nan,
+            4: '2020-01-02',
+            5: np.nan,
+            6: '2019-10-30',
+            7: np.nan,
+            8: '2020-01-02',
+            9: np.nan
+        },
+        'B': {
+            0: '2021-12-30',
+            1: '2021-10-27',
+            2: '2021-10-27',
+            3: '2021-10-27',
+            4: np.nan,
+            5: '2021-10-27',
+            6: '2021-10-27',
+            7: '2021-12-30',
+            8: np.nan,
+            9: '2021-10-27'
+        }
+    })
+    pd.testing.assert_frame_equal(expected_sampled, sampled)
+
+
+def test_scalar_inequality_constraint_with_datetimes_and_nones():
+    """Test that the ``ScalarInequality`` constraint works with ``None`` and ``datetime``."""
+    # Setup
+    data = pd.DataFrame(data={
+        'A': [None, None, '2020-01-02', '2020-03-04'],
+        'B': [None, '2021-03-04', '2021-12-31', None]
+    })
+
+    metadata = SingleTableMetadata.load_from_dict({
+        'columns': {
+            'A': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'},
+            'B': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'}
+        }
+    })
+
+    metadata.validate()
+    synth = GaussianCopulaSynthesizer(metadata)
+    synth.add_constraints([
+        {
+            'constraint_class': 'ScalarInequality',
+            'constraint_parameters': {
+                'column_name': 'A',
+                'relation': '>=',
+                'value': '2019-01-01'
+            }
+        }
+    ])
+    synth.validate(data)
+
+    # Run
+    synth.fit(data)
+    sampled = synth.sample(5)
+
+    # Assert
+    expected_sampled = pd.DataFrame({
+        'A': {
+            0: np.nan,
+            1: '2020-01-19',
+            2: np.nan,
+            3: '2020-01-29',
+            4: '2020-01-31',
+        },
+        'B': {
+            0: '2021-07-28',
+            1: '2021-07-14',
+            2: '2021-07-26',
+            3: '2021-07-02',
+            4: '2021-06-06',
+        }
+    })
+    pd.testing.assert_frame_equal(expected_sampled, sampled)
+
+
+def test_scalar_range_constraint_with_datetimes_and_nones():
+    """Test that the ``ScalarRange`` constraint works with ``None`` and ``datetime``."""
+    # Setup
+    data = pd.DataFrame(data={
+        'A': [None, None, '2020-01-02', '2020-03-04'],
+        'B': [None, '2021-03-04', '2021-12-31', None]
+    })
+
+    metadata = SingleTableMetadata.load_from_dict({
+        'columns': {
+            'A': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'},
+            'B': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'}
+        }
+    })
+
+    metadata.validate()
+    synth = GaussianCopulaSynthesizer(metadata)
+    synth.add_constraints([
+        {
+            'constraint_class': 'ScalarRange',
+            'constraint_parameters': {
+                'column_name': 'A',
+                'low_value': '2019-10-30',
+                'high_value': '2020-03-04',
+                'strict_boundaries': False
+            }
+        }
+    ])
+    synth.validate(data)
+
+    # Run
+    synth.fit(data)
+    sampled = synth.sample(10)
+
+    # Assert
+    expected_sampled = pd.DataFrame({
+        'A': {
+            0: '2020-03-03',
+            1: np.nan,
+            2: '2020-03-03',
+            3: np.nan,
+            4: np.nan,
+            5: '2020-03-03',
+            6: np.nan,
+            7: np.nan,
+            8: np.nan,
+            9: '2020-02-27',
+        },
+        'B': {
+            0: np.nan,
+            1: np.nan,
+            2: np.nan,
+            3: np.nan,
+            4: np.nan,
+            5: '2021-04-14',
+            6: np.nan,
+            7: '2021-05-21',
+            8: np.nan,
+            9: np.nan,
+        }
+    })
+    pd.testing.assert_frame_equal(expected_sampled, sampled)
+
+
+def test_range_constraint_with_datetimes_and_nones():
+    """Test that the ``Range`` constraint works with ``None`` and ``datetime``."""
+    # Setup
+    data = pd.DataFrame(data={
+        'A': [None, None, '2020-01-02', '2020-03-04'],
+        'B': [None, '2021-03-04', '2021-12-31', None],
+        'C': [None, '2022-03-04', '2022-12-31', None],
+    })
+
+    metadata = SingleTableMetadata.load_from_dict({
+        'columns': {
+            'A': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'},
+            'B': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'},
+            'C': {'sdtype': 'datetime', 'datetime_format': '%Y-%m-%d'}
+        }
+    })
+
+    metadata.validate()
+    synth = GaussianCopulaSynthesizer(metadata)
+    synth.add_constraints([
+        {
+            'constraint_class': 'Range',
+            'constraint_parameters': {
+                'low_column_name': 'A',
+                'middle_column_name': 'B',
+                'high_column_name': 'C',
+                'strict_boundaries': False
+            }
+        }
+    ])
+    synth.validate(data)
+
+    # Run
+    synth.fit(data)
+    sampled = synth.sample(10)
+
+    # Assert
+    expected_sampled = pd.DataFrame({
+        'A': {
+            0: '2020-01-02',
+            1: '2020-01-02',
+            2: np.nan,
+            3: '2020-01-02',
+            4: '2019-10-30',
+            5: np.nan,
+            6: '2020-01-02',
+            7: '2019-10-30',
+            8: '2019-10-30',
+            9: np.nan
+        },
+        'B': {
+            0: '2021-12-30',
+            1: '2021-12-30',
+            2: '2021-10-27',
+            3: np.nan,
+            4: '2021-10-27',
+            5: '2021-10-27',
+            6: np.nan,
+            7: '2021-10-27',
+            8: np.nan,
+            9: '2021-10-27'
+        },
+        'C': {
+            0: '2022-12-30',
+            1: '2022-12-30',
+            2: '2022-10-27',
+            3: np.nan,
+            4: '2022-10-27',
+            5: '2022-10-27',
+            6: np.nan,
+            7: '2022-10-27',
+            8: np.nan,
+            9: '2022-10-27'
+        }
+    })
+    pd.testing.assert_frame_equal(expected_sampled, sampled)
+
+
 def test_inequality_constraint_all_possible_nans_configurations():
     """Test that the inequality constraint works with all possible NaN configurations."""
     # Setup
     data = pd.DataFrame(data={
         'A': [0, 1, np.nan, np.nan, 2],
         'B': [2, np.nan, 3, np.nan, 3]
     })
```

### Comparing `sdv-1.2.0.dev1/tests/integration/single_table/test_copulas.py` & `sdv-1.2.1.dev0/tests/integration/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/integration/single_table/test_ctgan.py` & `sdv-1.2.1.dev0/tests/integration/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/readme_test/README.md` & `sdv-1.2.1.dev0/tests/readme_test/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/constraints/test_base.py` & `sdv-1.2.1.dev0/tests/unit/constraints/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/constraints/test_tabular.py` & `sdv-1.2.1.dev0/tests/unit/constraints/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/constraints/test_utils.py` & `sdv-1.2.1.dev0/tests/unit/constraints/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,26 +104,34 @@
     Output:
         - A single np.datetime64
         - A list of np.datetime64
         - A series of np.datetime64
     """
     # Setup
     string_value = '2021-02-02'
-    list_value = [np.nan, '2021-02-02']
-    series_value = pd.Series(['2021-02-02'])
+    list_value = [None, np.nan, '2021-02-02']
+    series_value = pd.Series(['2021-02-02', None, pd.NaT])
 
     # Run
     string_out = cast_to_datetime64(string_value)
     list_out = cast_to_datetime64(list_value)
     series_out = cast_to_datetime64(series_value)
 
     # Assert
     expected_string_output = np.datetime64('2021-02-02')
-    expected_series_output = pd.Series(np.datetime64('2021-02-02'))
-    expected_list_output = np.array([np.datetime64('NaT'), '2021-02-02'], dtype='datetime64[ns]')
+    expected_series_output = pd.Series([
+        np.datetime64('2021-02-02'),
+        np.datetime64('NaT'),
+        np.datetime64('NaT')
+    ])
+    expected_list_output = np.array([
+        np.datetime64('NaT'),
+        np.datetime64('NaT'),
+        '2021-02-02'
+    ], dtype='datetime64[ns]')
     np.testing.assert_array_equal(expected_list_output, list_out)
     pd.testing.assert_series_equal(expected_series_output, series_out)
     assert expected_string_output == string_out
 
 
 def test_matches_datetime_format():
     """Test the ``matches_datetime_format`` method.
```

### Comparing `sdv-1.2.0.dev1/tests/unit/data_processing/test_data_processor.py` & `sdv-1.2.1.dev0/tests/unit/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/data_processing/test_datetime_formatter.py` & `sdv-1.2.1.dev0/tests/unit/data_processing/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/data_processing/test_numerical_formatter.py` & `sdv-1.2.1.dev0/tests/unit/data_processing/test_numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/data_processing/test_utils.py` & `sdv-1.2.1.dev0/tests/unit/data_processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/datasets/test_demo.py` & `sdv-1.2.1.dev0/tests/unit/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/datasets/test_local.py` & `sdv-1.2.1.dev0/tests/unit/datasets/test_local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/evaluation/test_multi_table.py` & `sdv-1.2.1.dev0/tests/unit/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/evaluation/test_single_table.py` & `sdv-1.2.1.dev0/tests/unit/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/lite/test_single_table.py` & `sdv-1.2.1.dev0/tests/unit/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/metadata/test_anonymization.py` & `sdv-1.2.1.dev0/tests/unit/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/metadata/test_metadata_upgrader.py` & `sdv-1.2.1.dev0/tests/unit/metadata/test_metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/metadata/test_multi_table.py` & `sdv-1.2.1.dev0/tests/unit/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/metadata/test_single_table.py` & `sdv-1.2.1.dev0/tests/unit/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/multi_table/test_base.py` & `sdv-1.2.1.dev0/tests/unit/multi_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/multi_table/test_hma.py` & `sdv-1.2.1.dev0/tests/unit/multi_table/test_hma.py`

 * *Files 20% similar despite different names*

```diff
@@ -87,26 +87,14 @@
             '__nesreca__id_upravna_enota__num_rows': [1, 1, 1, 1]
         })
         instance._get_pbar_args.assert_called_once_with(
             desc="(1/2) Tables 'A' and 'B' ('user_id')")
 
         pd.testing.assert_frame_equal(result, expected)
 
-    def test__get_foreign_keys(self):
-        """Test that this method returns the foreign keys for a given table name and child name."""
-        # Setup
-        metadata = get_multi_table_metadata()
-        instance = HMASynthesizer(metadata)
-
-        # Run
-        result = instance._get_foreign_keys('nesreca', 'oseba')
-
-        # Assert
-        assert result == ['id_nesreca']
-
     def test__get_all_foreign_keys(self):
         """Test that this method returns all the foreign keys for a given table name."""
         # Setup
         metadata = get_multi_table_metadata()
         instance = HMASynthesizer(metadata)
 
         # Run
@@ -280,29 +268,26 @@
 
         assert list(call_augmented_data) == list(data)
         assert call_table_name == 'upravna_enota'
 
     def test__finalize(self):
         """Test that the finalize method applies the final touches to the generated data.
 
-        The process consists of applying the propper data types to each table, and finding
-        foreign keys if those are not present in the current sampled data.
+        The process consists of applying the propper data types to each table, and dropping
+        extra columns not present in the metadata.
         """
         # Setup
         instance = Mock()
         metadata = Mock()
         metadata._get_parent_map.return_value = {
             'sessions': ['users'],
             'transactions': ['sessions']
         }
         instance.metadata = metadata
 
-        instance._get_foreign_keys.side_effect = [['user_id'], ['session_id']]
-        instance._find_parent_ids.return_value = pd.Series(['a', 'a', 'b'], name='session_id')
-
         sampled_data = {
             'users': pd.DataFrame({
                 'user_id': pd.Series([0, 1, 2], dtype=np.int64),
                 'name': pd.Series(['John', 'Doe', 'Johanna'], dtype=object),
                 'additional_column': pd.Series([0.1, 0.2, 0.3], dtype=float),
                 'another_additional_column': pd.Series([0.1, 0.2, 0.5], dtype=float),
             }),
@@ -310,14 +295,15 @@
                 'user_id': pd.Series([1, 2, 1], dtype=np.int64),
                 'session_id': pd.Series(['a', 'b', 'c'], dtype=object),
                 'os': pd.Series(['linux', 'mac', 'win'], dtype=object),
                 'country': pd.Series(['us', 'us', 'es'], dtype=object),
             }),
             'transactions': pd.DataFrame({
                 'transaction_id': pd.Series([1, 2, 3], dtype=np.int64),
+                'session_id': pd.Series(['a', 'a', 'b'], dtype=object),
             }),
         }
 
         users_synth = Mock()
         users_synth._data_processor._dtypes = {'user_id': np.int64, 'name': str}
         sessions_synth = Mock()
         sessions_synth._data_processor._dtypes = {
@@ -384,319 +370,44 @@
             'loc': 0.5,
             'num_rows': 10.0,
             'scale': 0.25
         }
 
         assert result == expected_result
 
-    def test__process_samples(self):
-        """Test the ``_process_samples``.
-
-        Test that the method retrieves the ``data_processor`` from the fitted ``table_synthesizer``
-        and performs a ``reverse_transform`` and returns the data in the real space.
-        """
-        # Setup
-        sampled_rows = pd.DataFrame({
-            'name': [0.1, 0.25, 0.35],
-            'a': [1.0, 0.25, 0.5],
-            'b': [0.2, 0.6, 0.9],
-            'loc': [0.5, 0.1, 0.2],
-            'num_rows': [1, 2, 3],
-            'scale': [0.25, 0.35, 0.15]
-        })
-        instance = Mock()
-        users_synthesizer = Mock()
-        users_synthesizer._data_processor.reverse_transform.return_value = pd.DataFrame({
-            'user_id': [0, 1, 2],
-            'name': ['John', 'Doe', 'Johanna']
-        })
-        instance._table_synthesizers = {'users': users_synthesizer}
-
-        # Run
-        result = HMASynthesizer._process_samples(instance, 'users', sampled_rows)
-
-        # Assert
-        expected_result = pd.DataFrame({
-            'user_id': [0, 1, 2],
-            'name': ['John', 'Doe', 'Johanna'],
-            'a': [1.0, 0.25, 0.5],
-            'b': [0.2, 0.6, 0.9],
-            'loc': [0.5, 0.1, 0.2],
-            'num_rows': [1, 2, 3],
-            'scale': [0.25, 0.35, 0.15]
-        })
-        result = result.reindex(sorted(result.columns), axis=1)
-        expected_result = expected_result.reindex(sorted(expected_result.columns), axis=1)
-        pd.testing.assert_frame_equal(result, expected_result)
-
-    def test__sample_rows(self):
-        """Test sample rows.
-
-        Test that sampling rows will return the reverse transformed data with the extension columns
-        sampled by the model.
-        """
-        # Setup
-        synthesizer = Mock()
-        instance = Mock()
-
-        # Run
-        result = HMASynthesizer._sample_rows(instance, synthesizer, 'users', 10)
-
-        # Assert
-        assert result == instance._process_samples.return_value
-        instance._process_samples.assert_called_once_with(
-            'users',
-            synthesizer._sample.return_value
-        )
-        synthesizer._sample.assert_called_once_with(10)
-
-    def test__get_child_synthesizer(self):
+    def test__recreate_child_synthesizer(self):
         """Test that this method returns a synthesizer for the given child table."""
         # Setup
         instance = Mock()
         parent_row = 'row'
         table_name = 'users'
-        foreign_key = 'session_id'
+        parent_table_name = 'sessions'
         table_meta = Mock()
+        table_synthesizer = Mock()
         instance.metadata.tables = {'users': table_meta}
+        instance.metadata._get_foreign_keys.return_value = ['session_id']
         instance._table_parameters = {'users': {'a': 1}}
+        instance._table_synthesizers = {'users': table_synthesizer}
 
         # Run
-        synthesizer = HMASynthesizer._get_child_synthesizer(
+        synthesizer = HMASynthesizer._recreate_child_synthesizer(
             instance,
-            parent_row,
             table_name,
-            foreign_key
+            parent_table_name,
+            parent_row,
         )
 
         # Assert
         assert synthesizer == instance._synthesizer.return_value
+        assert synthesizer._data_processor == table_synthesizer._data_processor
         instance._synthesizer.assert_called_once_with(table_meta, a=1)
         synthesizer._set_parameters.assert_called_once_with(
             instance._extract_parameters.return_value
         )
-        instance._extract_parameters.assert_called_once_with(parent_row, table_name, foreign_key)
-
-    def test__sample_child_rows(self):
-        """Test the sampling of child rows when sampled data is empty."""
-        # Setup
-        instance = Mock()
-        instance._get_foreign_keys.return_value = ['user_id']
-        instance._extract_parameters.return_value = {
-            'a': 1.0,
-            'b': 0.2,
-            'loc': 0.5,
-            'num_rows': 10.0,
-            'scale': 0.25
-        }
-
-        metadata = Mock()
-        sessions_meta = Mock()
-        users_meta = Mock()
-        users_meta.primary_key.return_value = 'user_id'
-        metadata.tables = {
-            'users': users_meta,
-            'sessions': sessions_meta
-        }
-        instance.metadata = metadata
-        instance._synthesizer_kwargs = {'a': 0.1, 'b': 0.5, 'loc': 0.25}
-
-        instance._sample_rows.return_value = pd.DataFrame({
-            'session_id': ['a', 'b', 'c'],
-            'os': ['linux', 'mac', 'win'],
-            'country': ['us', 'us', 'es'],
-        })
-        parent_row = pd.DataFrame({
-            'user_id': [1, 2, 3],
-            'name': ['John', 'Doe', 'Johanna']
-        })
-        sampled_data = {}
-
-        # Run
-        HMASynthesizer._sample_child_rows(instance, 'sessions', 'users', parent_row, sampled_data)
-
-        # Assert
-        expected_result = pd.DataFrame({
-            'session_id': ['a', 'b', 'c'],
-            'os': ['linux', 'mac', 'win'],
-            'country': ['us', 'us', 'es'],
-            'user_id': [1, 2, 3]
-        })
-        pd.testing.assert_frame_equal(sampled_data['sessions'], expected_result)
-
-    def test__sample_child_rows_with_sampled_data(self):
-        """Test the sampling of child rows when sampled data contains values.
-
-        The new sampled data has to be concatenated to the current sampled data.
-        """
-        # Setup
-        instance = Mock()
-        instance._get_foreign_keys.return_value = ['user_id']
-        instance._extract_parameters.return_value = {
-            'a': 1.0,
-            'b': 0.2,
-            'loc': 0.5,
-            'num_rows': 10.0,
-            'scale': 0.25
-        }
-
-        metadata = Mock()
-        sessions_meta = Mock()
-        users_meta = Mock()
-        users_meta.primary_key.return_value = 'user_id'
-        metadata.tables = {
-            'users': users_meta,
-            'sessions': sessions_meta
-        }
-        instance.metadata = metadata
-        instance._synthesizer_kwargs = {'a': 0.1, 'b': 0.5, 'loc': 0.25}
-
-        instance._sample_rows.return_value = pd.DataFrame({
-            'session_id': ['a', 'b', 'c'],
-            'os': ['linux', 'mac', 'win'],
-            'country': ['us', 'us', 'es'],
-        })
-        parent_row = pd.DataFrame({
-            'user_id': [1, 2, 3],
-            'name': ['John', 'Doe', 'Johanna']
-        })
-        sampled_data = {
-            'sessions': pd.DataFrame({
-                'user_id': [0, 1, 0],
-                'session_id': ['d', 'e', 'f'],
-                'os': ['linux', 'mac', 'win'],
-                'country': ['us', 'us', 'es'],
-            })
-        }
-
-        # Run
-        HMASynthesizer._sample_child_rows(instance, 'sessions', 'users', parent_row, sampled_data)
-
-        # Assert
-        expected_result = pd.DataFrame({
-            'user_id': [0, 1, 0, 1, 2, 3],
-            'session_id': ['d', 'e', 'f', 'a', 'b', 'c'],
-            'os': ['linux', 'mac', 'win', 'linux', 'mac', 'win'],
-            'country': ['us', 'us', 'es', 'us', 'us', 'es'],
-        })
-        pd.testing.assert_frame_equal(sampled_data['sessions'], expected_result)
-
-    def test__sample_children(self):
-        """Test that child tables are being sampled recursively."""
-        # Setup
-        def update_sampled_data(child_name, table_name, row, sampled_data):
-            sampled_data['sessions'] = pd.DataFrame({
-                'user_id': [1],
-                'session_id': ['d'],
-                'os': ['linux'],
-                'country': ['us'],
-            })
-
-        metadata = Mock()
-        metadata._get_child_map.return_value = {'users': ['sessions']}
-        instance = Mock()
-        table_rows = pd.DataFrame({
-            'user_id': [1, 2, 3],
-            'name': ['John', 'Doe', 'Johanna']
-        })
-        sampled_data = {}
-        instance.metadata = metadata
-        instance._sample_child_rows.side_effect = update_sampled_data
-
-        # Run
-        HMASynthesizer._sample_children(instance, 'users', sampled_data, table_rows)
-
-        # Assert
-        assert instance._sample_child_rows.call_count == 3
-        sample_calls = instance._sample_child_rows.call_args_list
-        pd.testing.assert_series_equal(
-            sample_calls[0][0][2],
-            pd.Series({'user_id': 1, 'name': 'John'}, name=0)
-        )
-        pd.testing.assert_series_equal(
-            sample_calls[1][0][2],
-            pd.Series({'user_id': 2, 'name': 'Doe'}, name=1)
-        )
-        pd.testing.assert_series_equal(
-            sample_calls[2][0][2],
-            pd.Series({'user_id': 3, 'name': 'Johanna'}, name=2)
-        )
-
-    def test__sample_table(self):
-        """Test sampling a table.
-
-        The ``sample_table`` method will call sample children and return the sampled data
-        dictionary.
-        """
-        # Setup
-        def sample_children(table_name, sampled_data, table_rows):
-            sampled_data['sessions'] = pd.DataFrame({
-                'user_id': [1, 1, 3],
-                'session_id': ['a', 'b', 'c'],
-                'os': ['windows', 'linux', 'mac'],
-                'country': ['us', 'us', 'es']
-            })
-            sampled_data['transactions'] = pd.DataFrame({
-                'transaction_id': [1, 2, 3],
-                'session_id': ['a', 'a', 'b']
-            })
-
-        instance = Mock()
-        instance._table_sizes = {'users': 10}
-        instance._table_synthesizers = {'users': Mock()}
-        instance._sample_children.side_effect = sample_children
-        instance._sample_rows.return_value = pd.DataFrame({
-            'user_id': [1, 2, 3],
-            'name': ['John', 'Doe', 'Johanna']
-        })
-
-        # Run
-        result = HMASynthesizer._sample_table(instance, 'users')
-
-        # Assert
-        expected_result = {
-            'users': pd.DataFrame({
-                'user_id': [1, 2, 3],
-                'name': ['John', 'Doe', 'Johanna'],
-            }),
-            'sessions': pd.DataFrame({
-                'user_id': [1, 1, 3],
-                'session_id': ['a', 'b', 'c'],
-                'os': ['windows', 'linux', 'mac'],
-                'country': ['us', 'us', 'es'],
-            }),
-            'transactions': pd.DataFrame({
-                'transaction_id': [1, 2, 3],
-                'session_id': ['a', 'a', 'b']
-            })
-        }
-        for result_frame, expected_frame in zip(result.values(), expected_result.values()):
-            pd.testing.assert_frame_equal(result_frame, expected_frame)
-
-    def test__sample(self):
-        """Test that the ``_sample_table`` is called for tables that don't have parents."""
-        # Setup
-        instance = Mock()
-        instance.metadata._get_parent_map.return_value = {
-            'sessions': ['users'],
-            'transactions': ['sessions']
-        }
-        instance.metadata.tables = {
-            'users': Mock(),
-            'sessions': Mock(),
-            'transactions': Mock(),
-        }
-
-        # Run
-        result = HMASynthesizer._sample(instance)
-
-        # Assert
-        assert result == instance._finalize.return_value
-        instance._sample_table.assert_called_once_with('users', scale=1, sampled_data={})
-        instance._finalize.assert_called_once_with({})
+        instance._extract_parameters.assert_called_once_with(parent_row, table_name, 'session_id')
 
     def test_get_learned_distributions(self):
         """Test that ``get_learned_distributions`` returns a dict.
 
         Test that it returns a dictionary with the name of the columns and the learned
         distribution and its parameters.
         """
@@ -748,7 +459,52 @@
 
         # Run and Assert
         error_msg = re.escape(
             "Distributions have not been learned yet. Please fit your model first using 'fit'."
         )
         with pytest.raises(ValueError, match=error_msg):
             instance.get_learned_distributions('upravna_enota')
+
+    def test__add_foreign_key_columns(self):
+        """Test that the ``_add_foreign_key_columns`` method adds foreign keys."""
+        # Setup
+        instance = Mock()
+        metadata = Mock()
+        metadata._get_foreign_keys.return_value = ['primary_user_id', 'secondary_user_id']
+        instance.metadata = metadata
+
+        instance._find_parent_ids.return_value = pd.Series([2, 1, 2], name='secondary_user_id')
+
+        parent_table = pd.DataFrame({
+            'user_id': pd.Series([0, 1, 2], dtype=np.int64),
+            'name': pd.Series(['John', 'Doe', 'Johanna'], dtype=object),
+        })
+        child_table = pd.DataFrame({
+            'transaction_id': pd.Series([1, 2, 3], dtype=np.int64),
+            'primary_user_id': pd.Series([0, 0, 1], dtype=np.int64)
+        })
+
+        instance._table_synthesizers = {
+            'users': Mock(),
+            'transactions': Mock()
+        }
+
+        # Run
+        HMASynthesizer._add_foreign_key_columns(
+            instance,
+            child_table,
+            parent_table,
+            'transactions',
+            'users')
+
+        # Assert
+        expected_parent_table = pd.DataFrame({
+            'user_id': pd.Series([0, 1, 2], dtype=np.int64),
+            'name': pd.Series(['John', 'Doe', 'Johanna'], dtype=object),
+        })
+        expected_child_table = pd.DataFrame({
+            'transaction_id': pd.Series([1, 2, 3], dtype=np.int64),
+            'primary_user_id': pd.Series([0, 0, 1], dtype=np.int64),
+            'secondary_user_id': pd.Series([2, 1, 2], dtype=np.int64)
+        })
+        pd.testing.assert_frame_equal(expected_parent_table, parent_table)
+        pd.testing.assert_frame_equal(expected_child_table, child_table)
```

### Comparing `sdv-1.2.0.dev1/tests/unit/sampling/test_hierarchical_sampler.py` & `sdv-1.2.1.dev0/tests/unit/sampling/test_hierarchical_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # Run
         result = BaseHierarchicalSampler._sample_rows(instance, synthesizer, 10)
 
         # Assert
         assert result == synthesizer._sample_batch.return_value
         synthesizer._sample_batch.assert_called_once_with(
             10,
-            remove_extra_columns=False
+            keep_extra_columns=True
         )
 
     def test__get_num_rows_from_parent(self):
         """Test that the number of child rows is extracted from the parent row."""
         # Setup
         parent_row = pd.Series({
             '__sessions__user_id__num_rows': 10,
```

### Comparing `sdv-1.2.0.dev1/tests/unit/sampling/test_independent_sampler.py` & `sdv-1.2.1.dev0/tests/unit/sampling/test_independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/sampling/test_tabular.py` & `sdv-1.2.1.dev0/tests/unit/sampling/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/sequential/test_par.py` & `sdv-1.2.1.dev0/tests/unit/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/single_table/test_base.py` & `sdv-1.2.1.dev0/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/single_table/test_copulagan.py` & `sdv-1.2.1.dev0/tests/unit/single_table/test_copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/single_table/test_copulas.py` & `sdv-1.2.1.dev0/tests/unit/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/single_table/test_ctgan.py` & `sdv-1.2.1.dev0/tests/unit/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/single_table/test_utils.py` & `sdv-1.2.1.dev0/tests/unit/single_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/test___init__.py` & `sdv-1.2.1.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/unit/test_utils.py` & `sdv-1.2.1.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.0.dev1/tests/utils.py` & `sdv-1.2.1.dev0/tests/utils.py`

 * *Files identical despite different names*

