# Comparing `tmp/yaccounts-1.1.0.tar.gz` & `tmp/yaccounts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.0.tar", last modified: Sat Jul  8 21:48:11 2023, max compression
+gzip compressed data, was "yaccounts-1.1.1.tar", last modified: Sun Jul  9 19:47:59 2023, max compression
```

## Comparing `yaccounts-1.1.0.tar` & `yaccounts-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-08 21:48:11.477444 yaccounts-1.1.0/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-08 21:48:11.477444 yaccounts-1.1.0/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      385 2023-07-08 21:29:14.000000 yaccounts-1.1.0/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/test/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      655 2023-07-08 21:20:04.000000 yaccounts-1.1.0/test/test.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/yaccounts/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 06:17:46.000000 yaccounts-1.1.0/yaccounts/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3087 2023-07-08 21:17:41.000000 yaccounts-1.1.0/yaccounts/analyzer.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1741 2023-07-08 19:41:53.000000 yaccounts-1.1.0/yaccounts/config.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    10112 2023-07-08 21:24:22.000000 yaccounts-1.1.0/yaccounts/operating_unit.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-07 06:17:46.000000 yaccounts-1.1.0/yaccounts/utils.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-07 07:06:47.000000 yaccounts-1.1.0/yaccounts/workbook.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2975 2023-07-07 07:56:06.000000 yaccounts-1.1.0/yaccounts/worksheet.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/yaccounts.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.692198 yaccounts-1.1.1/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-09 19:47:59.692198 yaccounts-1.1.1/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-09 19:47:59.692198 yaccounts-1.1.1/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      385 2023-07-09 19:46:51.000000 yaccounts-1.1.1/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.682198 yaccounts-1.1.1/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-09 19:46:51.000000 yaccounts-1.1.1/test/test.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.682198 yaccounts-1.1.1/yaccounts/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 06:17:46.000000 yaccounts-1.1.1/yaccounts/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3166 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/analyzer.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1995 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/config.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    11149 2023-07-09 19:46:51.000000 yaccounts-1.1.1/yaccounts/operating_unit.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-07 06:17:46.000000 yaccounts-1.1.1/yaccounts/utils.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-08 21:56:14.000000 yaccounts-1.1.1/yaccounts/workbook.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2975 2023-07-08 21:56:14.000000 yaccounts-1.1.1/yaccounts/worksheet.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-09 19:47:59.692198 yaccounts-1.1.1/yaccounts.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-09 19:47:59.000000 yaccounts-1.1.1/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.0/yaccounts/analyzer.py` & `yaccounts-1.1.1/yaccounts/analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,45 +15,45 @@
 
         # Convert Operating Unit to string
         self.df["Operating Unit"] = self.df["Operating Unit"].apply(str)
 
         # Filter out ignored codes (account in CODES_IGNORED)
         self.df = self.df[~self.df["Account"].isin(CODES_IGNORED)]
 
-        self.operating_units = [str(ou) for ou in self.df["Operating Unit"].unique()]
+        self.operating_units = sorted([str(ou) for ou in self.df["Operating Unit"].unique()])
         print(f"Operating Units Found in CSV: {', '.join(self.operating_units)}")
 
         self.workbooks_initialized = False
         self.workbooks = []
 
         self.check_unhandled_codes()
 
     def add_workbook(self, path):
         self.workbooks_initialized = True
         workbook = Workbook(path)
         workbook.analyzer = self
         self.workbooks.append(workbook)
         return workbook
 
-    def _one_operating_unit_per_workbook(self):
+    def _setup_default_workbooks(self):
         if self.split_notebooks:
             # Create a new workbook for each operating unit
             for operating_unit in self.operating_units:
                 self.add_workbook(pathlib.Path.cwd() / (operating_unit + ".xlsx")).add_worksheet(
                     operating_unit
                 ).add_operating_unit(operating_unit)
         else:
             # Create a single workbook with all operating units
             wb = self.add_workbook(pathlib.Path.cwd() / "all.xlsx")
             for operating_unit in self.operating_units:
                 wb.add_worksheet(operating_unit).add_operating_unit(operating_unit)
 
     def run(self):
         if not self.workbooks_initialized:
-            self._one_operating_unit_per_workbook()
+            self._setup_default_workbooks()
 
         for workbook in self.workbooks:
             workbook.run(filter_df_on_operating_units(self.df, workbook.get_operating_units()))
 
     def check_unhandled_codes(self):
         # Get all account codes that were not handled
         unhandled_codes = sorted(
@@ -66,19 +66,22 @@
         # TODO: Add to spreadsheet instead of raising exception
 
         if unhandled_codes:
             raise Exception(
                 f"Unhandled account codes: {','.join([str(c) for c in unhandled_codes])}.  See https://finserve.byu.edu/account-revenue-expense"
             )
 
-    def find(self, operating_unit, year=None):
-        operating_uints = [
+    def get_all_operating_units(self):
+        return [
             ou
             for workbook in self.workbooks
             for worksheet in workbook.worksheets
             for ou in worksheet.operating_units
-            if ou.operating_unit == operating_unit
+        ]
+
+    def find(self, operating_unit, year=None):
+        operating_uints = [
+            ou for ou in self.get_all_operating_units() if ou.operating_unit == str(operating_unit)
         ]
         if year:
-            # Filter on year
             operating_uints = [ou for ou in operating_uints if ou.year == year]
         return operating_uints
```

### Comparing `yaccounts-1.1.0/yaccounts/config.py` & `yaccounts-1.1.1/yaccounts/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 CODES_STUDENT_WAGES = (
     5510,
     5599,
     5610,
     5720,
     5812,
-    5980,
     5572,
     5570,
     5672,
-    5670,
     5600,
-    5699,
     5750,
-    5950,
-    5960,
     8905,
 )
-CODES_STUDENT_BENEFITS = (5999,)
+
+# These student benefits aren't attached to an individual student
+# name, so they must be separated out
+CODES_STUDENT_BENEFITS = (5670, 5699, 5950, 5960, 5970, 5999)
+
 CODES_STUDENT_TUITION = (6300, 6303, 6304, 6309, 6319, 6390)
 CODES_FACULTY_SPRING_SUMMER = (5920, 5260, 5220)
 CODES_TRAVEL = (6190, 7000, 7010, 7030, 7050, 7060, 7070, 7080)
 CODES_SUPPLIES = (
     2200,
+    5980,
     6000,
     6005,
     6100,
     6109,
     6110,
     6120,
     6125,
@@ -50,25 +50,24 @@
     6499,
     8940,
 )
 CODES_CAPITAL = (1625, 1725, 8930, 9126, 9127, 9136, 9137)
 CODES_OVERHEAD = (8990, 8991)
 
 CODES_INTEREST = (4711,)
-# CODES_BALANCE_FORWARD = (10, 30)
-CODES_INCOME = (
-    3500,
-    4200,
-    5970,
-    9250,
-    9260,
-)
 
-# CODES_BUDGET_ONLY = (10,)
-CODES_IGNORED = (30, 1010, 1235, 2000, 2210, 4220, 5700)
+# Income only applies to non-budgeted accounts
+CODES_INCOME = (9250, 9260)
+
+# Non-budgeted accounts, don't normally use BUDGET lines and they
+# can be removed, except for these codes
+CODES_NON_BUDGETED_BUDGET_CODES = (10,)
+
+# These codes aren't used by anything and can be removed from the data
+CODES_IGNORED = (1010, 1235, 2000, 2210, 4220, 4200)
 
 COL_NAME_AMOUNT = "JRNL Monetary Amount -no scrn aggregation"
 
 COLOR_STUDENT_WAGES = "rosybrown"
 COLOR_STUDENT_BENEFITS = "moccasin"
 COLOR_STUDENT_TUITION = "moccasin"
 COLOR_FACULTY = "lightskyblue"
```

### Comparing `yaccounts-1.1.0/yaccounts/operating_unit.py` & `yaccounts-1.1.1/yaccounts/operating_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 class OperatingUnit:
     def __init__(
         self,
         worksheet,
         operating_unit,
         year,
         name=None,
-        rolling_budget=None,
+        budgeted_account=None,
         previous_expenditures=0,
     ) -> None:
         self.worksheet = worksheet
         self.operating_unit = operating_unit
         self.name = name
         self.previous_expenditures = previous_expenditures
         self.year = year
 
-        if rolling_budget is None:
-            self.rolling_budget = operating_unit.startswith("R")
+        if budgeted_account is None:
+            self.budgeted_account = operating_unit.startswith("R")
         else:
-            self.rolling_budget = rolling_budget
+            self.budgeted_account = budgeted_account
 
         # Create a new dataframe with months of the year as column headers
         self.df_gen = pd.DataFrame(
             columns=("Type", *[calendar.month_abbr[i] for i in range(1, 13)])
         )
 
         self.row_colors = {}
@@ -48,19 +48,24 @@
 
     def run(self, df):
         self.df = df
         if self.year:
             # Filter df on 'Fiscal Year' column
             self.df = self.df[self.df["Fiscal Year"] == self.year]
 
+        if self.budgeted_account:
+            self.verify_no_income()
+        else:
+            self.filter_out_budgeted_data()
+
         print(
             f"Running Operating Unit:{self.operating_unit} {('(' + str(self.year) + ')') if self.year else ''}",
         )
 
-        if self.rolling_budget:
+        if self.budgeted_account:
             self.previous_expenditures_total = (
                 (
                     self.previous_expenditures.total_expenses
                     + self.previous_expenditures.previous_expenditures_total
                 )
                 if isinstance(self.previous_expenditures, OperatingUnit)
                 else self.previous_expenditures
@@ -77,30 +82,31 @@
         self.add_row("Capital Equipment", CODES_CAPITAL, color=COLOR_CAPITAL)
         self.add_row("Overhead", CODES_OVERHEAD, color=COLOR_OVERHEAD)
         self.row_total_expenses = self.add_row(
             "Total Expeneses", all_expense_codes(), color=COLOR_TOTAL_EXPENSES
         )
         self.add_empty_row()
 
-        self.add_row("Interest", CODES_INTEREST, actuals_coeff=-1)
+        if not self.budgeted_account:
+            self.add_row("Interest", CODES_INTEREST, actuals_coeff=-1)
+
         self.add_row(
-            "Budget (New/Carryover)",
-            [],
+            "New Budgets or Carryover" if self.budgeted_account else "Transfor Income / Carryover",
+            CODES_INCOME,
             budgets_coeff=1,
-            actuals_coeff=0,
+            actuals_coeff=-1,
         )
-        self.add_row("Transfers", CODES_INCOME, actuals_coeff=-1)
+
         self.row_total_income = self.add_row(
             "Total Income",
             CODES_INTEREST + CODES_INCOME,
             color=COLOR_TOTAL_INCOME,
             budgets_coeff=1,
             actuals_coeff=-1,
         )
-
         self.add_empty_row()
 
         # Add a sum column that sums the values in each row, starting with the 2nd column,
         # skipping rows where "Type" is empty
 
         # Calculate the sum for rows where 'Type' column is not empty
         columns_to_sum = self.df_gen.columns[1:]  # Get all columns starting from the second column
@@ -199,30 +205,30 @@
 
         if color:
             self.row_colors[len(self.df_gen)] = color
 
         return self.df_gen.tail(1).index[0]
 
     def add_balance_row(self):
-        if self.rolling_budget:
+        if self.budgeted_account:
             self.df_gen.loc[len(self.df_gen)] = {
                 "Type": "Previous Expenditures",
                 calendar.month_abbr[1]: self.previous_expenditures_total,
             }
 
         self.df_gen.loc[len(self.df_gen)] = {"Type": "Balance (end of month)"}
 
         # # Iterate through columns and calcuate the balance, which is the total income minus the total expenses
         for month in range(1, 13):
             income = self.df_gen.iloc[self.row_total_income][month]
             expenses = self.df_gen.iloc[self.row_total_expenses][month]
 
             if month > 1:
                 prev_balance = self.df_gen.iloc[len(self.df_gen) - 1, month - 1]
-            elif self.rolling_budget:
+            elif self.budgeted_account:
                 prev_balance = -self.df_gen.iloc[len(self.df_gen) - 2, month]
             else:
                 prev_balance = 0
 
             balance = income - expenses + prev_balance
             self.df_gen.iloc[len(self.df_gen) - 1, month] = balance
             if month == 12:
@@ -235,36 +241,56 @@
         df_students = self.df[
             (self.df["Account"].isin(CODES_STUDENT_WAGES))
             & (self.df["JRNL Line Ledger"] == "ACTUALS")
         ]
 
         # Get unique list of value in 'JRNL Line Descr' column
         students_raw = df_students["JRNL Line Descr"].unique()
-        students = defaultdict(list)
+        self.students = defaultdict(list)
         for student in students_raw:
             match = re.search("([A-Za-z]+)[, ]+([A-Za-z]+)", student)
             if not match:
                 raise Exception(f"Could not parse student name: {student}")
-            student_key = f"  {match.group(2).title()} {match.group(1).title()}"
-            students[student_key].append(student)
+            student_key = f"{match.group(2).title()} {match.group(1).title()}"
+            self.students[student_key].append(student)
 
         # Create a new dictionary with the student wages by month
         student_data = {
-            "Type": [s for s in sorted(students.keys())],
+            "Type": [f"  {s}" for s in sorted(self.students.keys())],
             **{
                 calendar.month_abbr[month]: [
                     df_students.loc[
                         (df_students["Accounting Period"] == month)
-                        & (df_students["JRNL Line Descr"].isin(students[student]))
+                        & (df_students["JRNL Line Descr"].isin(self.students[student]))
                     ]["JRNL Monetary Amount -no scrn aggregation"].sum()
-                    for student in sorted(students.keys())
+                    for student in sorted(self.students.keys())
                 ]
                 for month in range(1, 13)
             },
         }
         self.df_gen = pd.concat((self.df_gen, pd.DataFrame(student_data)), ignore_index=True)
 
         # Add new row index to hidden rows
         if self.hide_student_wages:
             self.hidden_rows.extend(
                 range(len(self.df_gen) - len(student_data["Type"]) + 1, len(self.df_gen) + 1)
             )
+
+    def verify_no_income(self):
+        # Ensure df contains no CODES_INCOME
+        if self.df[self.df["Account"].isin(CODES_INCOME + CODES_INTEREST)].shape[0] > 0:
+            raise Exception(
+                f"Budgeted account {self.operating_unit} contains income. "
+                "Budgeted accounts should only contain expenses."
+            )
+
+    def filter_out_budgeted_data(self):
+        # Filter out budgeted data.  Only include ACTUALS or BUDGET with code in CODES_NON_BUDGETED_BUDGET_CODES
+        self.df = self.df[
+            (
+                (self.df["JRNL Line Ledger"] == "ACTUALS")
+                | (
+                    (self.df["JRNL Line Ledger"] == "BUDGETS")
+                    & (self.df["Account"].isin(CODES_NON_BUDGETED_BUDGET_CODES))
+                )
+            )
+        ]
```

### Comparing `yaccounts-1.1.0/yaccounts/workbook.py` & `yaccounts-1.1.1/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.0/yaccounts/worksheet.py` & `yaccounts-1.1.1/yaccounts/worksheet.py`

 * *Files identical despite different names*

