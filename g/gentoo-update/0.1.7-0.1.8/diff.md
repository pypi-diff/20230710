# Comparing `tmp/gentoo-update-0.1.7.tar.gz` & `tmp/gentoo-update-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.7.tar", last modified: Sun Jul  2 21:04:33 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.8.tar", last modified: Mon Jul 10 07:03:51 2023, max compression
```

## Comparing `gentoo-update-0.1.7.tar` & `gentoo-update-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/gentoo_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6057 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/scripts/updater.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/shell_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/gentoo_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7390 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.7/LICENSE` & `gentoo-update-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.7/PKG-INFO` & `gentoo-update-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.7
+Version: 0.1.8
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -55,10 +55,15 @@
 ```
 
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
+* Reading last update report (currently only successful update report):
+```bash
+gentoo-update --report
+```
+
 The detailed explanation of command flags can be found in `--help`.  
 Information on testing can be found in tests directory 
 [readme](tests/README.md)
```

### Comparing `gentoo-update-0.1.7/README.md` & `gentoo-update-0.1.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,10 +40,15 @@
 ```
 
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
+* Reading last update report (currently only successful update report):
+```bash
+gentoo-update --report
+```
+
 The detailed explanation of command flags can be found in `--help`.  
 Information on testing can be found in tests directory 
 [readme](tests/README.md)
```

### Comparing `gentoo-update-0.1.7/gentoo_update/gentoo_update.py` & `gentoo-update-0.1.8/gentoo_update/gentoo_update.py`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.7/gentoo_update/scripts/updater.sh` & `gentoo-update-0.1.8/gentoo_update/scripts/updater.sh`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,57 @@
 fi
 CONFIG_UPDATE_MODE="${4}"
 DAEMON_RESTART="${5}"
 CLEAN="${6}"
 READ_ELOGS="${7}"
 READ_NEWS="${8}"
 
+# ------------------- CHECK_DISK_USAGE ------------------- #
+function check_disk_usage() {
+    mount_point_found=false
+
+    while read -r line; do
+        if [[ "${line}" = \#* ]] || [[ -z "${line}" ]]; then
+            continue
+        fi
+
+        mount_point=$(echo "${line}" | awk '{print $2}')
+
+        if [[ ${mount_point} = "/tmp" || ${mount_point} = "swap" ]]; then
+            continue
+        fi
+
+        if [[ ! -d "${mount_point}" ]]; then
+            echo "Warning: mount point ${mount_point} does not exist."
+            continue
+        fi
+
+        mount_point_found=true
+
+        df -h "${mount_point}" |
+            awk -v OFS=", " 'NR==2 {print "Disk usage for " "'"${mount_point}"'"" ===> Total=" $2, "Used=" $3, "Free=" $4, "Percent used=" $5}'
+
+    done </etc/fstab
+
+    if [[ $mount_point_found == false ]]; then
+        df -h "/" |
+            awk -v OFS=", " 'NR==2 {print "Disk usage for " "/"" ===> Total=" $2, "Used=" $3, "Free=" $4, "Percent used=" $5}'
+    fi
+}
+
+function check_disk_usage_before_update() {
+    echo -e "\n{{ CALCULATE DISK USAGE 1 }}\n"
+    check_disk_usage
+}
+
+function check_disk_usage_after_update() {
+    echo -e "\n{{ CALCULATE DISK USAGE 2 }}\n"
+    check_disk_usage
+}
+
 # ------------------ SYNC_PORTAGE_TREE ------------------- #
 function sync_tree() {
     echo -e "{{ SYNC PORTAGE TREE }}\n"
 
     # Update main Portage tree
     echo "Syncing Portage Tree"
     emerge --sync
@@ -210,14 +253,22 @@
     else
         echo "not reading news"
     fi
 }
 
 # --------------------- RUN_PROGRAM ---------------------- #
 case ${FUNCTION} in
+check_disk_usage_before_update)
+    "$@"
+    exit
+    ;;
+check_disk_usage_after_update)
+    "$@"
+    exit
+    ;;
 sync_tree)
     "$@"
     exit
     ;;
 emerge_pretend)
     "$@"
     exit
```

### Comparing `gentoo-update-0.1.7/gentoo_update/shell_runner.py` & `gentoo-update-0.1.8/gentoo_update/shell_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,22 +195,24 @@
         Run every function in update.sh one by one.
 
         Args:
             *args (str): Arguments for the shell script.
                          They need to be handled by the script.
         """
         script_stages = [
+            "check_disk_usage_before_update",
             "sync_tree",
             "emerge_pretend",
             "update",
             "config_update",
             "clean_up",
             "check_restart",
             "get_logs",
             "get_news",
+            "check_disk_usage_after_update",
         ]
         for stage in script_stages:
             command = [self.script_path] + [stage] + list(args)
             self.run_shell_function(command)
 
         final_message = f"gentoo-update is done! Log:file: {self.log_filename}"
         self.logger.info(final_message)
```

### Comparing `gentoo-update-0.1.7/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.8/gentoo_update.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.7
+Version: 0.1.8
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -55,10 +55,15 @@
 ```
 
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
+* Reading last update report (currently only successful update report):
+```bash
+gentoo-update --report
+```
+
 The detailed explanation of command flags can be found in `--help`.  
 Information on testing can be found in tests directory 
 [readme](tests/README.md)
```

### Comparing `gentoo-update-0.1.7/setup.cfg` & `gentoo-update-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.7/tests/test_updater.py` & `gentoo-update-0.1.8/tests/test_updater.py`

 * *Files identical despite different names*

