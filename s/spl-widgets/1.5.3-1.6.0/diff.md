# Comparing `tmp/spl_widgets-1.5.3.tar.gz` & `tmp/spl_widgets-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.5.3.tar", last modified: Sun Jun 11 17:13:03 2023, max compression
+gzip compressed data, was "spl_widgets-1.6.0.tar", last modified: Mon Jul 10 21:02:31 2023, max compression
```

## Comparing `spl_widgets-1.5.3.tar` & `spl_widgets-1.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.201003 spl_widgets-1.5.3/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.3/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-06-11 17:13:03.200852 spl_widgets-1.5.3/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.3/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.3/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-06-11 17:13:03.201047 spl_widgets-1.5.3/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1229 2023-06-11 17:12:37.000000 spl_widgets-1.5.3/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.191795 spl_widgets-1.5.3/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.193911 spl_widgets-1.5.3/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.3/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.3/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195527 spl_widgets-1.5.3/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    13677 2023-05-26 16:37:32.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    15285 2023-05-26 16:35:21.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-05-26 16:37:26.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.3/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195658 spl_widgets-1.5.3/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.3/src/spl_widgets/data/cmudict.sqlite
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.3/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.3/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.3/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.3/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.3/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.3/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.200666 spl_widgets-1.5.3/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-05-26 17:14:58.000000 spl_widgets-1.5.3/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.5.3/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.5.3/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195089 spl_widgets-1.5.3/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      803 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       28 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.986881 spl_widgets-1.6.0/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.6.0/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:02:31.986560 spl_widgets-1.6.0/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.6.0/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.6.0/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:02:31.987007 spl_widgets-1.6.0/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-10 21:02:14.000000 spl_widgets-1.6.0/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.950394 spl_widgets-1.6.0/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.957962 spl_widgets-1.6.0/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.6.0/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.6.0/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.963612 spl_widgets-1.6.0/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    16323 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.6.0/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.981820 spl_widgets-1.6.0/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.6.0/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-09 17:07:05.000000 spl_widgets-1.6.0/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.6.0/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.6.0/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.6.0/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.6.0/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.6.0/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.6.0/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.986074 spl_widgets-1.6.0/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.6.0/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.6.0/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.961066 spl_widgets-1.6.0/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.5.3/LICENSE` & `spl_widgets-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/README.md` & `spl_widgets-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/setup.py` & `spl_widgets-1.6.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.5.3",
+    version="1.6.0",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     package_dir={"": "src"},
     packages=["spl_widgets", "spl_widgets.autoscorer", "spl_widgets.util"],
-    install_requires=['pandas', 'tkinterdnd2', 'openpyxl'],
+    install_requires=['pandas', 'tkinterdnd2-universal', 'openpyxl'],
     python_requires=">=3.8",
     entry_points='''
         [console_scripts]
         gorilla_clean=spl_widgets.gorilla_clean:main
         tuner=spl_widgets.tuner:main
         stk_swx=spl_widgets.stk_swx:main
         batch_tune=spl_widgets.batch_tune:main
         jukemake=spl_widgets.jukemake:main
         autoscorer=spl_widgets.autoscorer.autoscorer_gui:main
     ''',
     include_package_data=True,
-    package_data={'': ['data/*.sqlite']}
+    package_data={'': ['data/*']}
 )
```

### Comparing `spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from pathlib import Path
 
 import pandas as pd
 from openpyxl import Workbook
 from openpyxl.worksheet import dimensions
 from openpyxl.worksheet.worksheet import Worksheet
 
-from typing import TypeAlias
+from typing import TypeAlias, Literal
 
 from spl_widgets.autoscorer.tokenize_to_ipa import *
 from spl_widgets.util.color_util import to_rich_text
 
 AutoscorerTokens: TypeAlias =  list[ tuple[str, int, bool|None] ]
+ScoringMode: TypeAlias = Literal['preferred-transcription', 'best-match']
 
 # this version of the autoscorer uses a token list instead of a string, allowing
 # for the treatment of 2+ wide characters (e.g. diphthongs) as single tokens
 def score_transcription(
     sentence_ipa: list[str],
     transcription_ipa: list[str],
     _prev_scored: AutoscorerTokens = ...,
@@ -205,30 +206,39 @@
             f"({RED}{token}{CLEARSTYLE})"
         )
         incr += 1
 
     evaluation = "".join(transcription_chars)   # combine all tokens for evaluation
     return (score, best_poss_score, evaluation)
 
-def get_results(sentence_ipa: str, transcription: str, scoring_mode: str) -> tuple[ list[str], tuple[int, AutoscorerTokens] ]:
+def get_results(
+    sentence_ipa: str,
+    transcription: str,
+    scoring_mode: ScoringMode
+    ) -> tuple[ list[str], tuple[int, AutoscorerTokens] ]:
     
     if scoring_mode == "preferred-transcription":
         transcription_ipa = str_to_ipa(transcription, True)
         return (transcription_ipa, score_transcription(sentence_ipa, transcription_ipa))
 
     elif scoring_mode == "best-match":
         poss_results = []
         poss_transcription_ipas = [*map(arpa_to_ipa, to_arpabet_all(transcription))]
 
         for ipa in poss_transcription_ipas:
             poss_results.append( (ipa, score_transcription(sentence_ipa, ipa)) )
 
         return max(poss_results, key = lambda n: n[1][0])
 
-def process_inputs(inputs: list[tuple[str,str]], ws: Worksheet, ideal_ipa: list[str] = ..., **kwargs) -> None:
+def process_inputs(
+    inputs: list[tuple[str,str]],
+    ws: Worksheet,
+    scoring_mode: ScoringMode,
+    ideal_ipa: list[str] = ...
+    ) -> None:
     
     # utility function to make populating rows of the output file faster
     def fill_row(row: int, values: tuple[str,...]):
         for i, col in enumerate("ABCDEF"):
             ws[f"{col}{row}"] = values[i]
 
     # write header
@@ -243,21 +253,19 @@
     # get a tentative value for a column width to resize to
     col_width = max(max(len(k) for k in  n) for n in inputs)
     col_width = max(20, col_width)                              # ensuring headers are not cropped
 
     total_score = [0,0]
 
     (sentences, transcriptions) = [*zip(*inputs)]
-    if ideal_ipa == ...:
+    if ideal_ipa is ...:
         sentence_ipas = [*map(str_to_ipa, sentences)]
     else:
         sentence_ipas = [*map(tokenize_ipa, ideal_ipa)]
 
-    scoring_mode = kwargs.get("scoring_mode", "preferred-transcription")
-
     # iterate over the target-transcription pairs
     row=2                                               # doing it this way to use row outside of the loop's scope after
     for (sentence, sentence_ipa, transcription) in zip(sentences, sentence_ipas, transcriptions):
 
         # debug
         # print(f"TARGET: {sentence} | {sentence_ipa}", f"\nSUBJECT: {transcription} | {transcription_ipa}\n\n")
 
@@ -296,15 +304,21 @@
     for col in "ABCDEF":
         dim_holder[col] = dimensions.ColumnDimension(
             ws, col, width=col_width, bestFit = True
         )
 
     ws.column_dimensions = dim_holder
 
-def main(df: pd.DataFrame = ..., out_dir: str = ..., out_fn: str = ..., ideal_ipa: list[str] = ...):
+def main(
+    df: pd.DataFrame = ...,
+    out_dir: str = ...,
+    out_fn: str = ...,
+    ideal_ipa: list[str] = ...,
+    scoring_mode: ScoringMode = "preferred-transcription"
+    ):
 
     root = Tk()
     root.withdraw()
 
     wb = Workbook()
     wb.remove(wb.active)
 
@@ -327,14 +341,14 @@
     target = df["Target"]   # get target sentences
 
     # iterate through subject columns
     for col in df.columns[1:]:
         ws = wb.create_sheet(col)
 
         inputs: list[tuple[str,str]] = [ *zip(target, df[col]) ]
-        process_inputs(inputs, ws, ideal_ipa)
+        process_inputs(inputs, ws, scoring_mode, ideal_ipa)
 
     outpath = Path(out_dir, f"{out_fn}.xlsx")
     wb.save(outpath)
 
 if __name__ == "__main__":
     main()
```

### Comparing `spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from pathlib import Path
 from subprocess import run
 import re
 import pandas as pd
 
 from spl_widgets.util.gui_util import RadioFrame, MarginListBox, HelpLinkLabel
-from spl_widgets.autoscorer import autoscore
+# from spl_widgets.autoscorer import autoscore
+import autoscore
 
 HL = "*"*29
 
 class AutoscorerGUI:
     scoring_mode_radios: RadioFrame
     input_data_listbox: MarginListBox
     ideal_ipa_listbox: MarginListBox
@@ -61,15 +62,30 @@
                 AutoscorerGUI.show_error_popup(
                     "[ERROR]: All subject files must have the same list of target sentences (see terminal for details)"
                 )
                 return False
 
             return True
 
-    def process_output_combined(self, input_files: dict[str, Path]):
+    def get_ideal_ipas(self, subject_df: pd.DataFrame, ideal_ipa_path: tuple[str, Path] = ...) -> tuple[str, list[str]]:
+        scoring_mode = "preferred-transcription"
+        ideal_ipas = ...
+            
+        if ideal_ipa_path is not ...:
+            (fn, fp) = ideal_ipa_path
+            ideal_ipas_df = pd.read_excel(fp, header=0)
+            ideal_ipas_df.columns = ["Target", "IPA"]
+
+            if self.validate_df("IDEAL IPA FILE: "+fn, ideal_ipas_df, subject_df):
+                scoring_mode = "best-match"
+                ideal_ipas = ideal_ipas_df["IPA"]
+        
+        return (scoring_mode, ideal_ipas)
+
+    def process_output_combined(self, input_files: dict[str, Path], ideal_ipa_path: tuple[str, Path] = ...):
         df = None
         for (fn, fp) in input_files:
             subject_df = pd.read_excel(fp, header=0)
 
             if df is None:
                 subject_df.sort_values(by=["Target"], inplace=True, ignore_index = True)
                 df = subject_df
@@ -78,30 +94,28 @@
             if self.validate_df(fn, subject_df, df) == False:
                 return
 
             subj_header = subject_df.columns[1]
             subj_transcriptions = subject_df[subj_header]
             df[subj_header] = subj_transcriptions
 
-        if self.ideal_ipa_listbox.size() == 0:
-            ideal_ipas = ...
-
+        (scoring_mode, ideal_ipas) = self.get_ideal_ipas(df, ideal_ipa_path)
 
         outpath = Path(filedialog.asksaveasfilename(
             filetypes = [("Excel Files", "*.xlsx")],
             title = "Save Autoscorer Output to File"
         ))
         if outpath == "":
             self.show_error_popup("[EXIT]: User bailed while saving autoscored file")
             return False
 
         out_dir = outpath.parent
         out_fn = outpath.stem
 
-        autoscore.main( df, out_dir, out_fn, ideal_ipas )
+        autoscore.main( df, out_dir, out_fn, ideal_ipas, scoring_mode )
 
         self.output_data_listbox.add_item(outpath)
         self.output_data_listbox.insert(tk.END, HL) # horizontal line separating output batches
 
     def process_output_separate(self, input_files: list[tuple[str, Path]]):
 
         frames = []
@@ -134,27 +148,32 @@
 
             outfp = Path(output_dir, out_fn+".xlsx")
             self.output_data_listbox.add_item(outfp)
 
         self.output_data_listbox.insert(tk.END, HL)
 
     def autoscore_with_data(self):
-        # print("Autoscoring!")
+
+        if self.ideal_ipa_listbox.size() > 0:
+            ideal_ipa_path = [*self.ideal_ipa_listbox.data_items.items()][0]
+            
+        else:
+            ideal_ipa_path = ...
 
         # validate data
         if self.input_data_listbox.size() == 0:
             return self.show_error_popup("[ERROR]: No input files received")
 
         input_files = [*self.input_data_listbox.data_items.items()]
         combine_output = self.combine_output.get()
 
         if combine_output:
-            self.process_output_combined(input_files)
+            self.process_output_combined(input_files, ideal_ipa_path)
         else:
-            self.process_output_separate(input_files)
+            self.process_output_separate(input_files, ideal_ipa_path)
 
     def make_help_window(self):
         self.help_window = tk.Toplevel(self.master)
         self.help_window.title("Autoscorer GUI Help Menu")
         self.help_app = AutoscorerHelpWindow(self.help_window)
 
     def update_scoring_mode_radios(self):
@@ -276,15 +295,14 @@
 
         self.combine_output = tk.BooleanVar(value=True)
         combine_output_checkbox = tk.Checkbutton(
             options_frame,
             text = "Combine output into a single file",
             variable=self.combine_output,
             onvalue = True, offvalue = False,
-            # command = lambda: print(self.combine_output.get())
         )
         combine_output_checkbox.pack(side="top", padx = 5, pady=(0,3))
 
         self.scoring_mode_radios = RadioFrame(
             options_frame,
             options = ["Best-Match Transcription", "Preferred Transcription"],
             label_text = "Autoscorer Scoring Mode"
@@ -335,37 +353,40 @@
             text="Autoscored Output File(s)"
         )
         output_data_label.pack_frame(pady=(0,5))
 
         def add_output_file(listbox: MarginListBox, data: dict, filepath: Path):
             fn = filepath.name
 
-            listbox.insert(0, fn)
+            listbox.insert(tk.END, fn)
             data[fn] = filepath
 
         self.output_data_listbox = MarginListBox(
             output_frame,
             add_output_file,
             None,
             include_minus_button=False,
             pack_args={"expand": True},
             height=10, width=20
         )
         self.output_data_listbox.pack_frame(
             side="top", fill="y", expand=True
         )
 
-        def defocus_hl(e: tk.Event):
+        def defocus_hl(listbox: MarginListBox):
+
+            if (curselected:=listbox.curselection()) == (): # nothing selected
+                return
 
-            listbox: MarginListBox = e.widget
-            if listbox.get(listbox.curselection()) == HL:
+            if listbox.get(curselected) == HL:
                 listbox.selection_clear(0, tk.END)
 
         self.output_data_listbox.bind(
-            "<<ListboxSelect>>", defocus_hl
+            "<<ListboxSelect>>",
+            lambda x: defocus_hl(x.widget)
         )
 
         self.output_data_listbox.bind(                   # bind double-clicking on a listbox item to open that file
             "<Double-1>",
             lambda x: self.open_file(x.widget)
         )
 
@@ -410,33 +431,33 @@
 
         notebook_tab_FILE_INPUT = tk.Frame(
             self.help_notebook,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_FILE_INPUT.pack(fill="both", expand=True)
-
+        # TODO: ADD INPUT HELP TEXT HERE
         
 
         notebook_tab_SCORING_MODE = tk.Frame(
             self.help_notebook,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_SCORING_MODE.pack(fill="both", expand=True)
-
+        # TODO: ADD SCORING MODE HELP TEXT HERE
 
 
         notebook_tab_FILE_OUTPUT = tk.Frame(
             self.help_notebook,
             highlightbackground="black",
             highlightthickness=1
         )
         notebook_tab_FILE_OUTPUT.pack(fill="both", expand=True)
-
+        # TODO: ADD OUTPUT HELP TEXT HERE
 
         self.help_notebook.add(notebook_tab_FILE_INPUT, text="File Input", sticky="nsew")
         self.help_notebook.add(notebook_tab_SCORING_MODE, text="Scoring Mode Options", sticky="nsew")
         self.help_notebook.add(notebook_tab_FILE_OUTPUT, text="File Output", sticky="nsew")
 
         help_quitbutton = tk.Button(
             help_main_frame,
```

### Comparing `spl_widgets-1.5.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.6.0/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/batch_tune.py` & `spl_widgets-1.6.0/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.6.0/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.6.0/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/jukemake.py` & `spl_widgets-1.6.0/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/misc_util.py` & `spl_widgets-1.6.0/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/stk_swx.py` & `spl_widgets-1.6.0/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/tune_freq.py` & `spl_widgets-1.6.0/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/tuner.py` & `spl_widgets-1.6.0/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/util/color_util.py` & `spl_widgets-1.6.0/src/spl_widgets/util/color_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # This regex is largely simplified now & does not use exact ANSI escape codes
 # because there is literally no reason to, these will never be printed to terminal 
 
 # instead, I use an abbreviated version: \Rabc\C is a red "abc" instead of \x1b[31mabc\x1b[39m
 # because isn't that just so much better
 
-# to get a sense for this working use https://regex101.com/r/LjUtFx/1
+# to get a sense for this working use https://regex101.com/r/B0LoLF/1
 COLOR_TEXT_RE = r"(?:\\([RGY]))?([^\\]+)(?:\\C)?"
 
 # colors are ARGB, so first 2 are alpha channel
 RED = InlineFont(color="009F2B00")
 GREEN = InlineFont(color="0004BD04")
 YELLOW = InlineFont(color="00D37506")
```

### Comparing `spl_widgets-1.5.3/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.6.0/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.6.0/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.3/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.6.0/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 src/spl_widgets.egg-info/entry_points.txt
 src/spl_widgets.egg-info/requires.txt
 src/spl_widgets.egg-info/top_level.txt
 src/spl_widgets/autoscorer/autoscore.py
 src/spl_widgets/autoscorer/autoscorer_gui.py
 src/spl_widgets/autoscorer/tokenize_to_ipa.py
 src/spl_widgets/data/cmudict.sqlite
+src/spl_widgets/data/help_text.json
 src/spl_widgets/util/color_util.py
 src/spl_widgets/util/gui_util.py
 src/spl_widgets/util/sqlite_db.py
```

