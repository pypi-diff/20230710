# Comparing `tmp/yaccounts-1.1.1.tar.gz` & `tmp/yaccounts-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.1.tar", last modified: Sun Jul  9 19:47:59 2023, max compression
+gzip compressed data, was "yaccounts-1.1.2.tar", last modified: Mon Jul 10 15:17:38 2023, max compression
```

## Comparing `yaccounts-1.1.1.tar` & `yaccounts-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.692198 yaccounts-1.1.1/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-09 19:47:59.692198 yaccounts-1.1.1/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-09 19:47:59.692198 yaccounts-1.1.1/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      385 2023-07-09 19:46:51.000000 yaccounts-1.1.1/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.682198 yaccounts-1.1.1/test/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-09 19:46:51.000000 yaccounts-1.1.1/test/test.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.682198 yaccounts-1.1.1/yaccounts/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 06:17:46.000000 yaccounts-1.1.1/yaccounts/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3166 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/analyzer.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1995 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/config.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    11149 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/operating_unit.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-07 06:17:46.000000 yaccounts-1.1.1/yaccounts/utils.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-08 21:56:14.000000 yaccounts-1.1.1/yaccounts/workbook.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2975 2023-07-08 21:56:14.000000 yaccounts-1.1.1/yaccounts/worksheet.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.692198 yaccounts-1.1.1/yaccounts.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 15:17:38.957820 yaccounts-1.1.2/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 15:17:38.957820 yaccounts-1.1.2/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      395 2023-07-10 15:17:36.000000 yaccounts-1.1.2/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.947820 yaccounts-1.1.2/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-10 14:33:50.000000 yaccounts-1.1.2/test/test.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/yaccounts/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3628 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/analyzer.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2001 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/config.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     9762 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/operating_unit.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/utils.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/workbook.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2683 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/worksheet.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/yaccounts.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.1/test/test.py` & `yaccounts-1.1.2/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.1/yaccounts/analyzer.py` & `yaccounts-1.1.2/yaccounts/analyzer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 import pandas as pd
 
-from .config import CODES_IGNORED, all_handled_codes
+from .config import CODES_IGNORED, COL_NAME_AMOUNT, all_expense_codes, all_handled_codes
 from .utils import filter_df_on_operating_units
 from .workbook import Workbook
 
 
 class CsvDataAnalyzer:
     def __init__(self, csv_path, split_notebooks=False) -> None:
         self.csv_path = csv_path
@@ -81,7 +81,16 @@
     def find(self, operating_unit, year=None):
         operating_uints = [
             ou for ou in self.get_all_operating_units() if ou.operating_unit == str(operating_unit)
         ]
         if year:
             operating_uints = [ou for ou in operating_uints if ou.year == year]
         return operating_uints
+
+    def get_previous_expenditures(self, operating_unit, year):
+        """Return the sum of expenditures for this year and all previous years"""
+        return self.df[
+            (self.df["Operating Unit"] == operating_unit)
+            & (self.df["Fiscal Year"] <= year)
+            & (self.df["JRNL Line Ledger"] == "ACTUALS")
+            & (self.df["Account"].isin(all_expense_codes()))
+        ][COL_NAME_AMOUNT].sum()
```

### Comparing `yaccounts-1.1.1/yaccounts/config.py` & `yaccounts-1.1.2/yaccounts/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 )
 CODES_CAPITAL = (1625, 1725, 8930, 9126, 9127, 9136, 9137)
 CODES_OVERHEAD = (8990, 8991)
 
 CODES_INTEREST = (4711,)
 
 # Income only applies to non-budgeted accounts
-CODES_INCOME = (9250, 9260)
+CODES_INCOME = (9250, 9260, 3500)
 
 # Non-budgeted accounts, don't normally use BUDGET lines and they
 # can be removed, except for these codes
 CODES_NON_BUDGETED_BUDGET_CODES = (10,)
 
 # These codes aren't used by anything and can be removed from the data
 CODES_IGNORED = (1010, 1235, 2000, 2210, 4220, 4200)
```

### Comparing `yaccounts-1.1.1/yaccounts/operating_unit.py` & `yaccounts-1.1.2/yaccounts/operating_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,18 @@
     def __init__(
         self,
         worksheet,
         operating_unit,
         year,
         name=None,
         budgeted_account=None,
-        previous_expenditures=0,
     ) -> None:
         self.worksheet = worksheet
         self.operating_unit = operating_unit
         self.name = name
-        self.previous_expenditures = previous_expenditures
         self.year = year
 
         if budgeted_account is None:
             self.budgeted_account = operating_unit.startswith("R")
         else:
             self.budgeted_account = budgeted_account
 
@@ -39,14 +37,19 @@
         self.hidden_rows = []
 
         # Default options
         self.set_options()
 
         self.df = None
 
+        if self.budgeted_account:
+            self.previous_expenditures = self.analyzer.get_previous_expenditures(
+                self.operating_unit, self.year - 1
+            )
+
     def set_options(self, hide_student_wages=False):
         self.hide_student_wages = hide_student_wages
 
     def run(self, df):
         self.df = df
         if self.year:
             # Filter df on 'Fiscal Year' column
@@ -57,44 +60,35 @@
         else:
             self.filter_out_budgeted_data()
 
         print(
             f"Running Operating Unit:{self.operating_unit} {('(' + str(self.year) + ')') if self.year else ''}",
         )
 
-        if self.budgeted_account:
-            self.previous_expenditures_total = (
-                (
-                    self.previous_expenditures.total_expenses
-                    + self.previous_expenditures.previous_expenditures_total
-                )
-                if isinstance(self.previous_expenditures, OperatingUnit)
-                else self.previous_expenditures
-            )
-
         # Add student wage data
         self.add_row("Student Wages", CODES_STUDENT_WAGES, color=COLOR_STUDENT_WAGES)
         self.create_student_wages()
         self.add_row("Student Benefits", CODES_STUDENT_BENEFITS, color=COLOR_STUDENT_BENEFITS)
         self.add_row("Student Tuition", CODES_STUDENT_TUITION, color=COLOR_STUDENT_TUITION)
         self.add_row("Faculty Spr/Sum", CODES_FACULTY_SPRING_SUMMER, color=COLOR_FACULTY)
         self.add_row("Travel", CODES_TRAVEL, color=COLOR_TRAVEL)
         self.add_row("Supplies/Misc", CODES_SUPPLIES, color=COLOR_SUPPLIES)
         self.add_row("Capital Equipment", CODES_CAPITAL, color=COLOR_CAPITAL)
         self.add_row("Overhead", CODES_OVERHEAD, color=COLOR_OVERHEAD)
         self.row_total_expenses = self.add_row(
             "Total Expeneses", all_expense_codes(), color=COLOR_TOTAL_EXPENSES
         )
+
         self.add_empty_row()
 
         if not self.budgeted_account:
             self.add_row("Interest", CODES_INTEREST, actuals_coeff=-1)
 
         self.add_row(
-            "New Budgets or Carryover" if self.budgeted_account else "Transfor Income / Carryover",
+            "New Budgets or Carryover" if self.budgeted_account else "Transfer Income / Carryover",
             CODES_INCOME,
             budgets_coeff=1,
             actuals_coeff=-1,
         )
 
         self.row_total_income = self.add_row(
             "Total Income",
@@ -116,58 +110,30 @@
 
         # Save total expenses, which is found in the self.row_total_expenses, "Sum" column
         self.total_expenses = self.df_gen.iloc[self.row_total_expenses]["Sum"]
 
         self.add_balance_row()
         self.add_empty_row()
 
-        # self.df_gen["Sum"] = self.df_gen.apply(
-        #     lambda row: row["Value"] if row["Type"] else None, axis=1
-        # )
-
-        # Add extra row to top of df_gen called "Students"
-        # header_row = ["Students"] + [""] * (num_students)
-        # df_gen = pd.concat((header_row, df_gen), ignore_index=True)
-
-        # Export df_gen to Excel
-        # df_gen.to_excel("out.xlsx", index=False)
-
-        # # Create a new Excel file and add a worksheet.
-        # workbook = xlsxwriter.Workbook(f"{operating_unit}.xlsx")
-        # worksheet = workbook.add_worksheet()
-
-        # formattedWorksheet = FormattedWorksheet(sheet, workbook, df_gen, hasIndex=True)
-
-        # sheet.insert_row(header_row, 0)
-        # sheet.write_row(1, 1, header_row)
         title_name = self.operating_unit
         if self.name:
             title_name = f"{self.name} ({title_name})"
         if self.year:
             title_name = f"{title_name} - {self.year}"
         self.worksheet.write_to_sheet(self.df_gen, title_name, self.hidden_rows, self.row_colors)
 
-        # sheet.set_row(student_total_row, cell_format=blue_fill_format)
-
     def add_empty_row(self):
         # Add an empty row of None values
-        # self.df_gen = pd.concat((self.df_gen, pd.DataFrame([[""] * 13])), ignore_index=True)
         empty_data = {
             "Type": [""],
             **{calendar.month_abbr[month]: [np.nan] for month in range(1, 13)},
         }
 
         self.df_gen = pd.concat((self.df_gen, pd.DataFrame(empty_data)), ignore_index=True)
 
-        # self.df_gen.insert(
-        #     len(self.df_gen), pd.Series([np.nan] * len(self.df_gen.columns)), ignore_index=True
-        # )
-
-        # self.df_gen = pd.concat((self.df_gen, pd.DataFrame([[""] * 13])), ignore_index=True)
-
     def add_row(
         self,
         row_name,
         account_codes,
         budgets_coeff=0,
         actuals_coeff=1,
         color=None,
@@ -208,15 +174,15 @@
 
         return self.df_gen.tail(1).index[0]
 
     def add_balance_row(self):
         if self.budgeted_account:
             self.df_gen.loc[len(self.df_gen)] = {
                 "Type": "Previous Expenditures",
-                calendar.month_abbr[1]: self.previous_expenditures_total,
+                calendar.month_abbr[1]: self.previous_expenditures,
             }
 
         self.df_gen.loc[len(self.df_gen)] = {"Type": "Balance (end of month)"}
 
         # # Iterate through columns and calcuate the balance, which is the total income minus the total expenses
         for month in range(1, 13):
             income = self.df_gen.iloc[self.row_total_income][month]
@@ -290,7 +256,11 @@
                 (self.df["JRNL Line Ledger"] == "ACTUALS")
                 | (
                     (self.df["JRNL Line Ledger"] == "BUDGETS")
                     & (self.df["Account"].isin(CODES_NON_BUDGETED_BUDGET_CODES))
                 )
             )
         ]
+
+    @property
+    def analyzer(self):
+        return self.worksheet.workbook.analyzer
```

### Comparing `yaccounts-1.1.1/yaccounts/workbook.py` & `yaccounts-1.1.2/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.1/yaccounts/worksheet.py` & `yaccounts-1.1.2/yaccounts/worksheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,27 @@
 class Worksheet:
     def __init__(self, workbook, sheet) -> None:
         self.workbook = workbook
         self.operating_units = []
         self.sheet = sheet
         self.next_start_row = 0
 
-        # self.name = name
-        # if name is None:
-        #     self.name = ",".join([ou.operating_unit for ou in self.operating_units])
-
-    def add_operating_unit(self, operating_unit, name=None, year=None, previous_expenditures=0):
+    def add_operating_unit(self, operating_unit, name=None, year=None):
         if year is None:
             # Get all years for this operating unit from the dataframe
             years = sorted(
                 self.workbook.analyzer.df[
                     self.workbook.analyzer.df["Operating Unit"] == operating_unit
                 ]["Fiscal Year"].unique()
             )
         else:
             years = ensure_tuple(year)
 
-        prev = previous_expenditures
         for year in years:
-            prev = OperatingUnit(self, operating_unit, year, name=name, previous_expenditures=prev)
-            self.operating_units.append(prev)
-        # return operating_unit_obj
+            self.operating_units.append(OperatingUnit(self, operating_unit, year, name=name))
 
     def format_cell(self, row, col, format):
         self.sheet.conditional_format(row, col, row, col, {"type": "no_errors", "format": format})
 
     def format_row(self, row, format):
         self.sheet.conditional_format(row, 0, row, 13, {"type": "no_errors", "format": format})
         #     sheet.write_blank(row, i, sheet[row, i].value, color)
```

