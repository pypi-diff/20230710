# Comparing `tmp/starred_repo_finder-0.3.0.tar.gz` & `tmp/starred_repo_finder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred_repo_finder-0.3.0.tar", last modified: Mon Jul 10 03:34:04 2023, max compression
+gzip compressed data, was "starred_repo_finder-0.4.0.tar", last modified: Mon Jul 10 04:13:26 2023, max compression
```

## Comparing `starred_repo_finder-0.3.0.tar` & `starred_repo_finder-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/starred_repo_finder/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/starred_repo_finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/starred_repo_finder/starred_repo_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/tests/test_starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/starred_repo_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/starred_repo_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/starred_repo_finder/starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/tests/test_starred_repo_finder.py
```

### Comparing `starred_repo_finder-0.3.0/LICENSE` & `starred_repo_finder-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.3.0/PKG-INFO` & `starred_repo_finder-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred_repo_finder
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Starred Repo Finder
 
 A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 
+Features:
+
+- Find all repositories that are starred by the stargazers of a given repository
+- Filter results by minimum number of stargazers, forkers, and ratio of stargazers to forkers
+- Order results by stargazers, forkers, and ratio of stargazers to forkers
+- Output results in table, CSV, JSON, and markdown formats
+- Uses the [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events) and [ClickHouse](https://clickhouse.com) to query the data
+
 ## Installation
 
 ```bash
 pip install starred-repo-finder
 ```
 
 ## Build
@@ -45,14 +53,15 @@
 ```
 
 ## Usage
 
 Command line usage:
 
 ```bash
+$ starred_repo_finder --help
 usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
@@ -70,14 +79,22 @@
                         Minimum ratio of stargazers to forkers to include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
                         Output format (default: table). Options: table, csv, json, markdown
 ```
 
 ## Examples
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Find the top 10 shared GitHub repositories by stars for stargazers of the `facebook/react` repo, from repos with a minimum of 10,000 stargazers, 1,000 forkers, and a ratio of at least 10 stargazers to each forkers:
 
 ```bash
 $ starred_repo_finder --limit=10 --order=ratio --stargazers=10000 --forkers=1000 --ratio=10 --format=markdown facebook/react
 ```
 
 | Project | Stargazers | Forkers | Ratio |
@@ -143,22 +160,14 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
-#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
-
-```bash
-$ starred_repo_finder Elderjs/elderjs
-```
-
-![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
-
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
 See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
```

### Comparing `starred_repo_finder-0.3.0/README.md` & `starred_repo_finder-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Starred Repo Finder
 
 A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 
+Features:
+
+- Find all repositories that are starred by the stargazers of a given repository
+- Filter results by minimum number of stargazers, forkers, and ratio of stargazers to forkers
+- Order results by stargazers, forkers, and ratio of stargazers to forkers
+- Output results in table, CSV, JSON, and markdown formats
+- Uses the [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events) and [ClickHouse](https://clickhouse.com) to query the data
+
 ## Installation
 
 ```bash
 pip install starred-repo-finder
 ```
 
 ## Build
@@ -30,14 +38,15 @@
 ```
 
 ## Usage
 
 Command line usage:
 
 ```bash
+$ starred_repo_finder --help
 usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
@@ -55,14 +64,22 @@
                         Minimum ratio of stargazers to forkers to include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
                         Output format (default: table). Options: table, csv, json, markdown
 ```
 
 ## Examples
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Find the top 10 shared GitHub repositories by stars for stargazers of the `facebook/react` repo, from repos with a minimum of 10,000 stargazers, 1,000 forkers, and a ratio of at least 10 stargazers to each forkers:
 
 ```bash
 $ starred_repo_finder --limit=10 --order=ratio --stargazers=10000 --forkers=1000 --ratio=10 --format=markdown facebook/react
 ```
 
 | Project | Stargazers | Forkers | Ratio |
@@ -128,22 +145,14 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
-#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
-
-```bash
-$ starred_repo_finder Elderjs/elderjs
-```
-
-![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
-
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
 See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
```

### Comparing `starred_repo_finder-0.3.0/setup.py` & `starred_repo_finder-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="starred_repo_finder",
-    version="0.3.0",
+    version="0.4.0",
     description="A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tylercb/starred_repo_finder",
     author="Tyler Hanway",
     author_email="hanway.tyler@gmail.com",
     license="MIT",
```

### Comparing `starred_repo_finder-0.3.0/starred_repo_finder/starred_repo_finder.py` & `starred_repo_finder-0.4.0/starred_repo_finder/starred_repo_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,34 @@
     """
     Print the results to the console in the specified format.
     """
     if not results:
         console.print("No results found", style="bold red")
         return
 
-    _, output = convert_and_format_results(results, output_format)
+    results, output = convert_and_format_results(results, output_format)
 
     # Don't use rich for csv, json, or markdown output
     if output_format in ["csv", "json", "markdown"]:
         print(output)
     else:
         console.print(output)
 
+    return results
 
-def run(repo_name, limit =  100, order_by = "stargazers", stargazers = None, forkers = None, ratio = None, output_format = "table"):
+
+def run(
+    repo_name,
+    limit=100,
+    order_by="stargazers",
+    stargazers=None,
+    forkers=None,
+    ratio=None,
+    output_format="table",
+):
     """
     Run the script.
     """
     query = build_query(repo_name, limit, order_by, stargazers, forkers, ratio)
 
     # Make the request
     params = {"user": "explorer"}
```

### Comparing `starred_repo_finder-0.3.0/starred_repo_finder.egg-info/PKG-INFO` & `starred_repo_finder-0.4.0/starred_repo_finder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred-repo-finder
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Starred Repo Finder
 
 A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 
+Features:
+
+- Find all repositories that are starred by the stargazers of a given repository
+- Filter results by minimum number of stargazers, forkers, and ratio of stargazers to forkers
+- Order results by stargazers, forkers, and ratio of stargazers to forkers
+- Output results in table, CSV, JSON, and markdown formats
+- Uses the [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events) and [ClickHouse](https://clickhouse.com) to query the data
+
 ## Installation
 
 ```bash
 pip install starred-repo-finder
 ```
 
 ## Build
@@ -45,14 +53,15 @@
 ```
 
 ## Usage
 
 Command line usage:
 
 ```bash
+$ starred_repo_finder --help
 usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
@@ -70,14 +79,22 @@
                         Minimum ratio of stargazers to forkers to include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
                         Output format (default: table). Options: table, csv, json, markdown
 ```
 
 ## Examples
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Find the top 10 shared GitHub repositories by stars for stargazers of the `facebook/react` repo, from repos with a minimum of 10,000 stargazers, 1,000 forkers, and a ratio of at least 10 stargazers to each forkers:
 
 ```bash
 $ starred_repo_finder --limit=10 --order=ratio --stargazers=10000 --forkers=1000 --ratio=10 --format=markdown facebook/react
 ```
 
 | Project | Stargazers | Forkers | Ratio |
@@ -143,22 +160,14 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
-#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
-
-```bash
-$ starred_repo_finder Elderjs/elderjs
-```
-
-![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
-
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
 See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
```

### Comparing `starred_repo_finder-0.3.0/tests/test_starred_repo_finder.py` & `starred_repo_finder-0.4.0/tests/test_starred_repo_finder.py`

 * *Files identical despite different names*

