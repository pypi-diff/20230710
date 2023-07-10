# Comparing `tmp/b2restore-1.9.4.tar.gz` & `tmp/b2restore-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b2restore-1.9.4.tar", last modified: Mon Nov 11 06:01:53 2019, max compression
+gzip compressed data, was "b2restore-1.9.5.tar", last modified: Thu Jan 28 03:24:05 2021, max compression
```

## Comparing `b2restore-1.9.4.tar` & `b2restore-1.9.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2019-11-11 06:01:53.000000 b2restore-1.9.4/
--rw-r--r--   0 mark      (1000) mark      (1000)     8574 2019-11-11 06:01:53.000000 b2restore-1.9.4/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     6703 2019-11-11 05:48:20.000000 b2restore-1.9.4/README.md
--rwxr-xr-x   0 mark      (1000) mark      (1000)       80 2018-05-11 00:08:18.000000 b2restore-1.9.4/b2restore
--rwxr-xr-x   0 mark      (1000) mark      (1000)     1273 2018-09-02 02:12:28.000000 b2restore-1.9.4/b2restore-create-dummy-files
--rwxr-xr-x   0 mark      (1000) mark      (1000)     1431 2018-09-02 02:00:13.000000 b2restore-1.9.4/b2restore-create-git
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2019-11-11 06:01:53.000000 b2restore-1.9.4/b2restore.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     8574 2019-11-11 06:01:53.000000 b2restore-1.9.4/b2restore.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      223 2019-11-11 06:01:53.000000 b2restore-1.9.4/b2restore.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2019-11-11 06:01:53.000000 b2restore-1.9.4/b2restore.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       10 2019-11-11 06:01:53.000000 b2restore-1.9.4/b2restore.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     7049 2018-09-03 00:46:49.000000 b2restore-1.9.4/b2restore.py
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2019-11-11 06:01:53.000000 b2restore-1.9.4/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1060 2019-11-11 05:50:32.000000 b2restore-1.9.4/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-01-28 03:24:05.245596 b2restore-1.9.5/
+-rw-r--r--   0 mark      (1000) mark      (1000)     8589 2021-01-28 03:24:05.245596 b2restore-1.9.5/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     6710 2020-02-18 23:34:12.000000 b2restore-1.9.5/README.md
+-rwxr-xr-x   0 mark      (1000) mark      (1000)     1273 2018-09-02 02:12:28.000000 b2restore-1.9.5/b2restore-create-dummy-files
+-rwxr-xr-x   0 mark      (1000) mark      (1000)     1431 2018-09-02 02:00:13.000000 b2restore-1.9.5/b2restore-create-git
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-01-28 03:24:05.245596 b2restore-1.9.5/b2restore.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     8589 2021-01-28 03:24:05.000000 b2restore-1.9.5/b2restore.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      249 2021-01-28 03:24:05.000000 b2restore-1.9.5/b2restore.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-01-28 03:24:05.000000 b2restore-1.9.5/b2restore.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2021-01-28 03:24:05.000000 b2restore-1.9.5/b2restore.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       10 2021-01-28 03:24:05.000000 b2restore-1.9.5/b2restore.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     7049 2020-04-16 04:01:54.000000 b2restore-1.9.5/b2restore.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2021-01-28 03:24:05.245596 b2restore-1.9.5/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1166 2021-01-20 22:48:39.000000 b2restore-1.9.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `b2restore-1.9.4/PKG-INFO` & `b2restore-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: b2restore
-Version: 1.9.4
+Version: 1.9.5
 Summary: Program to recreate Backblaze B2 file archive atspecified date+time
 Home-page: https://github.com/bulletmark/b2restore
 Author: Mark Blakeney
-Author-email: mark@irsaere.net
+Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Description: ## B2RESTORE
         
         [b2restore](http://github.com/bulletmark/b2restore) is a command line
         utility which can be used with [rclone](https://rclone.org/) to
         manually restore a [Backblaze B2](https://www.backblaze.com/b2/) archive
         for any given date and time. Alternatively, you can create a git
@@ -33,20 +33,19 @@
         
         This utility is typically used with [rclone](https://rclone.org/).
         Simply `rclone sync` or `rclone copy` the B2 bucket or sub-paths from
         the bucket which you want to restore. You **MUST** specify
         `--b2-versions` to include all file versions, e.g:
         
         ```
-        mkdir b2files
         rclone sync --b2-versions --fast-list --transfers=4 $* B2:mybucket b2files
         ```
         
         The above command will copy all files and available versions to the
-        `b2files` directory. You only need to do this once.
+        created `b2files` directory. You only need to do this once.
         
         ### CREATION OF SNAPSHOT AT GIVEN TIME
         
         Given the above `rclone` initial copy, you run this utility to
         create a snapshot of the directory tree for the time you are interested
         in.
         
@@ -151,19 +150,19 @@
         It is also good to get a feel for how `b2restore` works, what it does,
         and whether it suits your needs without requiring you to first perform
         an onerous huge download of your entire B2 archive.
         
         Here is an example usage:
         
         ```
-        rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files allfiles
-        b2restore allfiles b2
-        du -shl b2 # (see how much storage tree of latest versions uses)
-        b2restore -t 2018-05-10T12:00.00 allfiles b2
-        du -shl b2 # (see how much storage tree of yesterdays versions uses)
+        rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files b2files
+        b2restore b2files outdir
+        du -shl outdir # (see how much storage tree of latest versions uses)
+        b2restore -t 2018-05-10T12:00.00 b2files outdir
+        du -shl outdir # (see how much storage tree of yesterdays versions uses)
         ```
         
         #### B2RESTORE-CREATE-DUMMY-FILES COMMAND LINE OPTIONS
         
         ```
         Usage: b2restore-create-dummy-files [-options] outdir
         Reads B2 file list (from lsl output) from standard input to create
```

### Comparing `b2restore-1.9.4/README.md` & `b2restore-1.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,19 @@
 
 This utility is typically used with [rclone](https://rclone.org/).
 Simply `rclone sync` or `rclone copy` the B2 bucket or sub-paths from
 the bucket which you want to restore. You **MUST** specify
 `--b2-versions` to include all file versions, e.g:
 
 ```
-mkdir b2files
 rclone sync --b2-versions --fast-list --transfers=4 $* B2:mybucket b2files
 ```
 
 The above command will copy all files and available versions to the
-`b2files` directory. You only need to do this once.
+created `b2files` directory. You only need to do this once.
 
 ### CREATION OF SNAPSHOT AT GIVEN TIME
 
 Given the above `rclone` initial copy, you run this utility to
 create a snapshot of the directory tree for the time you are interested
 in.
 
@@ -143,19 +142,19 @@
 It is also good to get a feel for how `b2restore` works, what it does,
 and whether it suits your needs without requiring you to first perform
 an onerous huge download of your entire B2 archive.
 
 Here is an example usage:
 
 ```
-rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files allfiles
-b2restore allfiles b2
-du -shl b2 # (see how much storage tree of latest versions uses)
-b2restore -t 2018-05-10T12:00.00 allfiles b2
-du -shl b2 # (see how much storage tree of yesterdays versions uses)
+rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files b2files
+b2restore b2files outdir
+du -shl outdir # (see how much storage tree of latest versions uses)
+b2restore -t 2018-05-10T12:00.00 b2files outdir
+du -shl outdir # (see how much storage tree of yesterdays versions uses)
 ```
 
 #### B2RESTORE-CREATE-DUMMY-FILES COMMAND LINE OPTIONS
 
 ```
 Usage: b2restore-create-dummy-files [-options] outdir
 Reads B2 file list (from lsl output) from standard input to create
```

### Comparing `b2restore-1.9.4/b2restore-create-dummy-files` & `b2restore-1.9.5/b2restore-create-dummy-files`

 * *Files identical despite different names*

### Comparing `b2restore-1.9.4/b2restore-create-git` & `b2restore-1.9.5/b2restore-create-git`

 * *Files identical despite different names*

### Comparing `b2restore-1.9.4/b2restore.egg-info/PKG-INFO` & `b2restore-1.9.5/b2restore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: b2restore
-Version: 1.9.4
+Version: 1.9.5
 Summary: Program to recreate Backblaze B2 file archive atspecified date+time
 Home-page: https://github.com/bulletmark/b2restore
 Author: Mark Blakeney
-Author-email: mark@irsaere.net
+Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Description: ## B2RESTORE
         
         [b2restore](http://github.com/bulletmark/b2restore) is a command line
         utility which can be used with [rclone](https://rclone.org/) to
         manually restore a [Backblaze B2](https://www.backblaze.com/b2/) archive
         for any given date and time. Alternatively, you can create a git
@@ -33,20 +33,19 @@
         
         This utility is typically used with [rclone](https://rclone.org/).
         Simply `rclone sync` or `rclone copy` the B2 bucket or sub-paths from
         the bucket which you want to restore. You **MUST** specify
         `--b2-versions` to include all file versions, e.g:
         
         ```
-        mkdir b2files
         rclone sync --b2-versions --fast-list --transfers=4 $* B2:mybucket b2files
         ```
         
         The above command will copy all files and available versions to the
-        `b2files` directory. You only need to do this once.
+        created `b2files` directory. You only need to do this once.
         
         ### CREATION OF SNAPSHOT AT GIVEN TIME
         
         Given the above `rclone` initial copy, you run this utility to
         create a snapshot of the directory tree for the time you are interested
         in.
         
@@ -151,19 +150,19 @@
         It is also good to get a feel for how `b2restore` works, what it does,
         and whether it suits your needs without requiring you to first perform
         an onerous huge download of your entire B2 archive.
         
         Here is an example usage:
         
         ```
-        rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files allfiles
-        b2restore allfiles b2
-        du -shl b2 # (see how much storage tree of latest versions uses)
-        b2restore -t 2018-05-10T12:00.00 allfiles b2
-        du -shl b2 # (see how much storage tree of yesterdays versions uses)
+        rclone lsl --b2-versions B2:mybucket | b2restore-create-dummy-files b2files
+        b2restore b2files outdir
+        du -shl outdir # (see how much storage tree of latest versions uses)
+        b2restore -t 2018-05-10T12:00.00 b2files outdir
+        du -shl outdir # (see how much storage tree of yesterdays versions uses)
         ```
         
         #### B2RESTORE-CREATE-DUMMY-FILES COMMAND LINE OPTIONS
         
         ```
         Usage: b2restore-create-dummy-files [-options] outdir
         Reads B2 file list (from lsl output) from standard input to create
```

### Comparing `b2restore-1.9.4/b2restore.py` & `b2restore-1.9.5/b2restore.py`

 * *Files identical despite different names*

### Comparing `b2restore-1.9.4/setup.py` & `b2restore-1.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 name = 'b2restore'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 executable = stat.S_IEXEC | stat.S_IXGRP | stat.S_IXOTH
 
 setup(
     name=name,
-    version='1.9.4',
+    version='1.9.5',
     description='Program to recreate Backblaze B2 file archive at'
             'specified date+time',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/bulletmark/{}'.format(name),
     author='Mark Blakeney',
-    author_email='mark@irsaere.net',
+    author_email='mark.blakeney@bullet-systems.net',
     keywords='backblaze b2',
     license='GPLv3',
     py_modules=[module],
     python_requires='>=3.5',
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     data_files=[
         ('share/{}'.format(name), ['README.md']),
     ],
+    entry_points={
+        'console_scripts': ['{}={}:main'.format(name, module)],
+    },
     scripts=[f.name for f in here.iterdir() if f.name.startswith(name)
         and f.is_file() and f.stat().st_mode & executable],
 )
```

