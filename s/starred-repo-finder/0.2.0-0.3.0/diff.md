# Comparing `tmp/starred_repo_finder-0.2.0.tar.gz` & `tmp/starred_repo_finder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred_repo_finder-0.2.0.tar", last modified: Mon Jul 10 02:53:47 2023, max compression
+gzip compressed data, was "starred_repo_finder-0.3.0.tar", last modified: Mon Jul 10 03:34:04 2023, max compression
```

## Comparing `starred_repo_finder-0.2.0.tar` & `starred_repo_finder-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/starred_repo_finder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/starred_repo_finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/starred_repo_finder/starred_repo_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/tests/test_starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/starred_repo_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/starred_repo_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/starred_repo_finder/starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 03:34:04.000000 starred_repo_finder-0.3.0/starred_repo_finder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:34:04.795269 starred_repo_finder-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 03:33:52.000000 starred_repo_finder-0.3.0/tests/test_starred_repo_finder.py
```

### Comparing `starred_repo_finder-0.2.0/LICENSE` & `starred_repo_finder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.2.0/PKG-INFO` & `starred_repo_finder-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: starred_repo_finder
-Version: 0.2.0
-Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
-Home-page: https://github.com/tylercb/starred_repo_finder
-Author: Tyler Hanway
-Author-email: hanway.tyler@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Starred Repo Finder
 
 A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 
 ## Installation
 
 ```bash
@@ -143,30 +128,52 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
-See [examples/sveltejs-svelte.csv](examples/sveltejs-svelte.csv) for the output.
+See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `duckdb/duckdb` repo to a JSON file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=json duckdb/duckdb > examples/duckdb-duckdb.json
 ```
 
-See [examples/duckdb-duckdb.json](examples/duckdb-duckdb.json) for the output.
+See [examples/duckdb-duckdb.json](https://github.com/tylercb/starred_repo_finder/blob/main/examples/duckdb-duckdb.json) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `Ionaru/easy-markdown-editor` repo to a markdown file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=markdown Ionaru/easy-markdown-editor > examples/ionaru-easy-markdown-editor.md
 ```
 
-See [examples/ionaru-easy-markdown-editor.md](examples/ionaru-easy-markdown-editor.md) for the output.
+See [examples/ionaru-easy-markdown-editor.md](https://github.com/tylercb/starred_repo_finder/blob/main/examples/ionaru-easy-markdown-editor.md) for the output.
+
+## Acknowledgements
+
+- [ClickHouse Playground](https://clickhouse.com/docs/en/getting-started/playground)
+- [ClickHouse Query](https://play.clickhouse.com/play)
+- [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events)
+
+## Contributing
+
+Contributions are welcome! Negative feedback is also welcome, but please be constructive. If you have a feature request, please open an issue first to discuss it. If you want to contribute code, please open an issue first to discuss it. If you want to contribute documentation, please open an issue first to discuss it. If you want to contribute an example, please open an issue first to discuss it. If you want to contribute a bug fix, please open an issue first to discuss it. If you want to contribute a test, please open an issue first to discuss it. If you want to contribute anything else, please open an issue first to discuss it. If you want to contribute a donation, please open an issue first to discuss it.
+
+## License
+
+[MIT](LICENSE)
```

### Comparing `starred_repo_finder-0.2.0/README.md` & `starred_repo_finder-0.3.0/starred_repo_finder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: starred-repo-finder
+Version: 0.3.0
+Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
+Home-page: https://github.com/tylercb/starred_repo_finder
+Author: Tyler Hanway
+Author-email: hanway.tyler@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Starred Repo Finder
 
 A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 
 ## Installation
 
 ```bash
@@ -128,30 +143,52 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
-See [examples/sveltejs-svelte.csv](examples/sveltejs-svelte.csv) for the output.
+See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `duckdb/duckdb` repo to a JSON file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=json duckdb/duckdb > examples/duckdb-duckdb.json
 ```
 
-See [examples/duckdb-duckdb.json](examples/duckdb-duckdb.json) for the output.
+See [examples/duckdb-duckdb.json](https://github.com/tylercb/starred_repo_finder/blob/main/examples/duckdb-duckdb.json) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `Ionaru/easy-markdown-editor` repo to a markdown file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=markdown Ionaru/easy-markdown-editor > examples/ionaru-easy-markdown-editor.md
 ```
 
-See [examples/ionaru-easy-markdown-editor.md](examples/ionaru-easy-markdown-editor.md) for the output.
+See [examples/ionaru-easy-markdown-editor.md](https://github.com/tylercb/starred_repo_finder/blob/main/examples/ionaru-easy-markdown-editor.md) for the output.
+
+## Acknowledgements
+
+- [ClickHouse Playground](https://clickhouse.com/docs/en/getting-started/playground)
+- [ClickHouse Query](https://play.clickhouse.com/play)
+- [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events)
+
+## Contributing
+
+Contributions are welcome! Negative feedback is also welcome, but please be constructive. If you have a feature request, please open an issue first to discuss it. If you want to contribute code, please open an issue first to discuss it. If you want to contribute documentation, please open an issue first to discuss it. If you want to contribute an example, please open an issue first to discuss it. If you want to contribute a bug fix, please open an issue first to discuss it. If you want to contribute a test, please open an issue first to discuss it. If you want to contribute anything else, please open an issue first to discuss it. If you want to contribute a donation, please open an issue first to discuss it.
+
+## License
+
+[MIT](LICENSE)
```

### Comparing `starred_repo_finder-0.2.0/setup.py` & `starred_repo_finder-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="starred_repo_finder",
-    version="0.2.0",
+    version="0.3.0",
     description="A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tylercb/starred_repo_finder",
     author="Tyler Hanway",
     author_email="hanway.tyler@gmail.com",
     license="MIT",
```

### Comparing `starred_repo_finder-0.2.0/starred_repo_finder/starred_repo_finder.py` & `starred_repo_finder-0.3.0/starred_repo_finder/starred_repo_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     # Don't use rich for csv, json, or markdown output
     if output_format in ["csv", "json", "markdown"]:
         print(output)
     else:
         console.print(output)
 
 
-def run(repo_name, limit, order_by, stargazers, forkers, ratio, output_format):
+def run(repo_name, limit =  100, order_by = "stargazers", stargazers = None, forkers = None, ratio = None, output_format = "table"):
     """
     Run the script.
     """
     query = build_query(repo_name, limit, order_by, stargazers, forkers, ratio)
 
     # Make the request
     params = {"user": "explorer"}
```

### Comparing `starred_repo_finder-0.2.0/starred_repo_finder.egg-info/PKG-INFO` & `starred_repo_finder-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starred-repo-finder
-Version: 0.2.0
+Name: starred_repo_finder
+Version: 0.3.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -143,30 +143,52 @@
 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 93 | 6 | 15.5 |
 | [vinta/awesome-python](https://github.com/vinta/awesome-python) | 170 | 11 | 15.45 |
 | [strapi/strapi](https://github.com/strapi/strapi) | 77 | 5 | 15.4 |
 | [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) | 92 | 6 | 15.33 |
 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | 76 | 5 | 15.2 |
 | [florinpop17/app-ideas](https://github.com/florinpop17/app-ideas) | 75 | 5 | 15.0 |
 
+#### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
+
+```bash
+$ starred_repo_finder Elderjs/elderjs
+```
+
+![Screenshot](https://github.com/tylercb/starred_repo_finder/raw/main/screenshot.png)
+
 #### Write the top 100 shared GitHub repositories by stars for stargazers of the `sveltejs/svelte` repo to a CSV file:
 
 ```bash
 $ starred_repo_finder --limit=100 --format=csv sveltejs/svelte > examples/sveltejs-svelte.csv
 ```
 
-See [examples/sveltejs-svelte.csv](examples/sveltejs-svelte.csv) for the output.
+See [examples/sveltejs-svelte.csv](https://github.com/tylercb/starred_repo_finder/blob/main/examples/sveltejs-svelte.csv) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `duckdb/duckdb` repo to a JSON file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=json duckdb/duckdb > examples/duckdb-duckdb.json
 ```
 
-See [examples/duckdb-duckdb.json](examples/duckdb-duckdb.json) for the output.
+See [examples/duckdb-duckdb.json](https://github.com/tylercb/starred_repo_finder/blob/main/examples/duckdb-duckdb.json) for the output.
 
 #### Write the top 50 shared GitHub repositories by stars for stargazers of the `Ionaru/easy-markdown-editor` repo to a markdown file:
 
 ```bash
 $ starred_repo_finder --limit=50 --format=markdown Ionaru/easy-markdown-editor > examples/ionaru-easy-markdown-editor.md
 ```
 
-See [examples/ionaru-easy-markdown-editor.md](examples/ionaru-easy-markdown-editor.md) for the output.
+See [examples/ionaru-easy-markdown-editor.md](https://github.com/tylercb/starred_repo_finder/blob/main/examples/ionaru-easy-markdown-editor.md) for the output.
+
+## Acknowledgements
+
+- [ClickHouse Playground](https://clickhouse.com/docs/en/getting-started/playground)
+- [ClickHouse Query](https://play.clickhouse.com/play)
+- [GitHub Events Dataset](https://clickhouse.com/docs/en/getting-started/example-datasets/github-events)
+
+## Contributing
+
+Contributions are welcome! Negative feedback is also welcome, but please be constructive. If you have a feature request, please open an issue first to discuss it. If you want to contribute code, please open an issue first to discuss it. If you want to contribute documentation, please open an issue first to discuss it. If you want to contribute an example, please open an issue first to discuss it. If you want to contribute a bug fix, please open an issue first to discuss it. If you want to contribute a test, please open an issue first to discuss it. If you want to contribute anything else, please open an issue first to discuss it. If you want to contribute a donation, please open an issue first to discuss it.
+
+## License
+
+[MIT](LICENSE)
```

### Comparing `starred_repo_finder-0.2.0/tests/test_starred_repo_finder.py` & `starred_repo_finder-0.3.0/tests/test_starred_repo_finder.py`

 * *Files identical despite different names*

