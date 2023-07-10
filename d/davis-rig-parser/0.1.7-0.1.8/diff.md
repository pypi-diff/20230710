# Comparing `tmp/davis_rig_parser-0.1.7.tar.gz` & `tmp/davis_rig_parser-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davis_rig_parser-0.1.7.tar", last modified: Thu Jul  6 15:44:25 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.1.8.tar", last modified: Mon Jul 10 17:53:11 2023, max compression
```

## Comparing `davis_rig_parser-0.1.7.tar` & `davis_rig_parser-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.1.7/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.540785 davis_rig_parser-0.1.7/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.7/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18459 2023-07-06 15:43:14.000000 davis_rig_parser-0.1.7/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-06 15:43:28.000000 davis_rig_parser-0.1.7/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.7/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.1.8/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.848085 davis_rig_parser-0.1.8/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.8/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18431 2023-07-10 17:32:59.000000 davis_rig_parser-0.1.8/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-10 17:51:34.000000 davis_rig_parser-0.1.8/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.8/tests/test.py
```

### Comparing `davis_rig_parser-0.1.7/README.md` & `davis_rig_parser-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `davis_rig_parser-0.1.7/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.1.8/davis_rig_parser/davis_rig_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,19 +221,18 @@
 
         #Check data with detail sheeet
         detail_row = np.array(np.where(detail_df.Date==Detail_Dict['StartDate'].strip()))
         for case in range(detail_row.shape[1]):
             if detail_df.Notes[detail_row[:,case][0]].lower() in \
                 Detail_Dict['FileName'][Detail_Dict['FileName'].rfind('_')+1:].lower()\
                 and detail_df.Animal[detail_row[:,case][0]] in Detail_Dict['Animal']:
-                
-                    
+
                 #Add details to dataframe    
-				df.insert(loc=1, column='Notes', value=detail_df['Notes'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
-				df.insert(loc=2, column='Condition', value=detail_df['Condition'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
+                df.insert(loc=1, column='Notes', value=detail_df['Notes'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
+                df.insert(loc=2, column='Condition', value=detail_df['Condition'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
                 break
                 
     if len(file_check) == 0:
         #Add blank columns
         df.insert(loc=1, column='Notes', value='')
         df.insert(loc=2, column='Condition', value='')
 
@@ -367,15 +366,15 @@
             #Merge the data into a list
             merged_data.append(dfFull)
     
     #Append dataframe with animal's details
     merged_df = pd.concat(merged_data)
     
     #Format to capitalize first letter of labels
-    merged_df['Condition'] = merged_df.Condition.str.title()
+    #merged_df['Condition'] = merged_df.Condition.str.title()
     
     #Extract dataframe for ease of handling
     df = merged_df
     #Untack all the ILIs across all bouts to performa math
     df_lists = df[['Bouts']].unstack().apply(pd.Series)
     #replace 0s with nans so that bout count makes 0 licks 0 bouts too
     df_lists = df_lists.replace(0, np.nan)
@@ -384,25 +383,25 @@
     
     #replace all 0s with NaNs (arise due to licking once in the beginning with long pause)
     df_lists.replace(0,np.nan,inplace = True)
     df['Bouts_mean']=np.array(df_lists.mean(axis = 1, skipna = True))
     
     #Work on ILI means
     df_lists = df[['ILIs']].unstack().apply(pd.Series)
-    
+
     all_trials = []
     for row in range(df_lists.shape[0]):
-    
         trial_ILI = []
-        trial_ILI = [np.insert(trial_ILI,len(trial_ILI),df_lists.iloc[row][i]) for i in \
-                     range(0,int(np.array(df_lists.iloc[row].shape)))]
+        for element in df_lists.iloc[row]:
+            if isinstance(element, list):  # Only append if the element is a list
+                trial_ILI.append(element)
         flatt_trial = list(itertools.chain(*trial_ILI))
-        #exclude nan vals
-        all_trials.append(np.array([i for i in flatt_trial if not np.isnan(i)]))  # Remove NaNs from the list before appending
-    
+        # exclude nan vals
+        all_trials.append([i for i in flatt_trial if not np.isnan(i)])  # Remove NaNs from the list before appending
+
     #Store ILIs extended into dataframe
     df['ILI_all'] = all_trials
     
     df['Animal'] = df['Animal'].str.strip()
     df['LENGTH'] = df['LENGTH'].str.strip().astype(int)
     
     #Save dataframe for later use/plotting/analyses
```

