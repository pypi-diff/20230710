# Comparing `tmp/safeway_coupons-0.2.2.tar.gz` & `tmp/safeway_coupons-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeway_coupons-0.2.2.tar", max compression
+gzip compressed data, was "safeway_coupons-0.2.3.tar", max compression
```

## Comparing `safeway_coupons-0.2.2.tar` & `safeway_coupons-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/LICENSE
--rw-r--r--   0        0        0     5424 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/README.md
--rw-r--r--   0        0        0     2457 2023-07-10 06:00:06.107554 safeway_coupons-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      166 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/__init__.py
--rw-r--r--   0        0        0       22 2023-07-10 06:00:06.107554 safeway_coupons-0.2.2/safeway_coupons/__version__.py
--rw-r--r--   0        0        0      161 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/accounts.py
--rw-r--r--   0        0        0     2889 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/app.py
--rw-r--r--   0        0        0     2129 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/client.py
--rw-r--r--   0        0        0     2138 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/config.py
--rw-r--r--   0        0        0     2960 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/email.py
--rw-r--r--   0        0        0     1025 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/errors.py
--rw-r--r--   0        0        0     1029 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/methods.py
--rw-r--r--   0        0        0     2103 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/models.py
--rw-r--r--   0        0        0        0 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/py.typed
--rw-r--r--   0        0        0     3528 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/safeway.py
--rw-r--r--   0        0        0     5849 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/session.py
--rw-r--r--   0        0        0      846 2023-07-10 05:59:23.827257 safeway_coupons-0.2.2/safeway_coupons/utils.py
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 safeway_coupons-0.2.2/setup.py
--rw-r--r--   0        0        0     6559 1970-01-01 00:00:00.000000 safeway_coupons-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5424 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/README.md
+-rw-r--r--   0        0        0     2457 2023-07-10 06:34:28.120574 safeway_coupons-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-10 06:34:28.124574 safeway_coupons-0.2.3/safeway_coupons/__version__.py
+-rw-r--r--   0        0        0      161 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/accounts.py
+-rw-r--r--   0        0        0     2889 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/app.py
+-rw-r--r--   0        0        0     2129 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/client.py
+-rw-r--r--   0        0        0     2138 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/config.py
+-rw-r--r--   0        0        0     2960 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/email.py
+-rw-r--r--   0        0        0     1025 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/errors.py
+-rw-r--r--   0        0        0     1029 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/methods.py
+-rw-r--r--   0        0        0     2103 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/py.typed
+-rw-r--r--   0        0        0     3528 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/safeway.py
+-rw-r--r--   0        0        0     6067 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/session.py
+-rw-r--r--   0        0        0      846 2023-07-10 06:33:44.027172 safeway_coupons-0.2.3/safeway_coupons/utils.py
+-rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 safeway_coupons-0.2.3/setup.py
+-rw-r--r--   0        0        0     6559 1970-01-01 00:00:00.000000 safeway_coupons-0.2.3/PKG-INFO
```

### Comparing `safeway_coupons-0.2.2/LICENSE` & `safeway_coupons-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/README.md` & `safeway_coupons-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/pyproject.toml` & `safeway_coupons-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "safeway-coupons"
-version = "0.2.2"
+version = "0.2.3"
 description = "Automatic coupon clipper for Safeway's online \"Safeway for U\" coupons"
 license = "GPL-3.0-or-later"
 authors = ["Stephen Kent <smkent@smkent.net>"]
 readme = "README.md"
 repository = "https://github.com/smkent/safeway-coupons"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `safeway_coupons-0.2.2/safeway_coupons/app.py` & `safeway_coupons-0.2.3/safeway_coupons/app.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/client.py` & `safeway_coupons-0.2.3/safeway_coupons/client.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/config.py` & `safeway_coupons-0.2.3/safeway_coupons/config.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/email.py` & `safeway_coupons-0.2.3/safeway_coupons/email.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/errors.py` & `safeway_coupons-0.2.3/safeway_coupons/errors.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/methods.py` & `safeway_coupons-0.2.3/safeway_coupons/methods.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/models.py` & `safeway_coupons-0.2.3/safeway_coupons/models.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/safeway.py` & `safeway_coupons-0.2.3/safeway_coupons/safeway.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/safeway_coupons/session.py` & `safeway_coupons-0.2.3/safeway_coupons/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from typing import Any, List, Optional
 
 import requests
 import selenium.webdriver.support.expected_conditions as ec
 import undetected_chromedriver as uc  # type: ignore
 from selenium.common.exceptions import (
+    NoSuchElementException,
     StaleElementReferenceException,
     TimeoutException,
 )
 from selenium.webdriver.remote.webdriver import By
 from selenium.webdriver.support.wait import WebDriverWait
 
 from .accounts import Account
@@ -89,20 +90,24 @@
             try:
                 driver.implicitly_wait(10)
                 wait = WebDriverWait(driver, 10)
                 # Navigate to the website URL
                 url = "https://www.safeway.com"
                 print("Connect to safeway.com")
                 driver.get(url)
-                button = driver.find_element(
-                    By.XPATH, "//button [contains(text(), 'Necessary Only')]"
-                )
-                if button:
-                    print("Decline cookie prompt")
-                    button.click()
+                try:
+                    button = driver.find_element(
+                        By.XPATH,
+                        "//button [contains(text(), 'Necessary Only')]",
+                    )
+                    if button:
+                        print("Decline cookie prompt")
+                        button.click()
+                except NoSuchElementException:
+                    print("Skipping cookie prompt which is not present")
                 print("Open Sign In sidebar")
                 wait.until(
                     ec.visibility_of_element_located(
                         (By.XPATH, "//span [contains(text(), 'Sign In')]")
                     )
                 ).click()
                 print("Open Sign In form")
```

### Comparing `safeway_coupons-0.2.2/safeway_coupons/utils.py` & `safeway_coupons-0.2.3/safeway_coupons/utils.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.2.2/setup.py` & `safeway_coupons-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webdriver-manager>=3.8.6,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['safeway-coupons = safeway_coupons.app:main']}
 
 setup_kwargs = {
     'name': 'safeway-coupons',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Automatic coupon clipper for Safeway\'s online "Safeway for U" coupons',
     'long_description': '# Automatic Safeway coupon clipper\n\n[![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]\n[![Build](https://img.shields.io/github/checks-status/smkent/safeway-coupons/main?label=build)][gh-actions]\n[![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]\n[![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]\n\n**safeway-coupons** is a script that will log in to an account on safeway.com,\nand attempt to select all of the "Safeway for U" electronic coupons on the site\nso they don\'t have to each be clicked manually.\n\n## Design notes\n\nSafeway\'s sign in page is protected by a web application firewall (WAF).\nsafeway-coupons performs authentication using a headless instance of Google\nChrome. Authentication may fail based on your IP\'s reputation, either by\npresenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons\ncurrently does not have support for prompting the user to solve CAPTCHAs.\n\nOnce a signed in session is established, coupon clipping is performed using HTTP\nrequests via [requests][requests].\n\n## Installation and usage with Docker\n\nA Docker container is provided which runs safeway-coupons with cron. The cron\nschedule and your Safeway account details may be configured using environment\nvariables, or with an accounts file.\n\nExample `docker-compose.yaml` with configuration via environment variables:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com\n      SAFEWAY_ACCOUNT_PASSWORD: very_secret\n      SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com\n      SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com\n    restart: unless-stopped\n```\n\nExample `docker-compose.yaml` with configuration via accounts file:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNTS_FILE: /accounts_file\n    restart: unless-stopped\n    volumes:\n      - path/to/safeway_accounts_file:/accounts_file:ro\n```\n\nStart the container by running:\n\n```console\ndocker-compose up -d\n```\n\nDebugging information can be viewed in the container log:\n\n```console\ndocker-compose logs -f\n```\n\n## Installation from PyPI\n\n### Prerequisites\n\n* Google Chrome (for authentication performed via Selenium).\n* Optional: `sendmail` (for email support)\n\n### Installation\n\n[safeway-coupons is available on PyPI][pypi]:\n\n```console\npip install safeway-coupons\n```\n\n### Usage\n\nFor best results, run this program once a day or so with a cron daemon.\n\nFor full usage options, run\n\n```console\nsafeway-coupons --help\n```\n\n### Configuration\n\n**safeway-coupons** can clip coupons for one or more Safeway accounts in a\nsingle run, depending on the configuration method used.\n\nIf a sender email address is configured, a summary email will be sent for each\nSafeway account via `sendmail`. The email recipient defaults to the Safeway\naccount email address, but can be overridden for each account.\n\nAccounts are searched via the following methods in the listed order. Only one\naccount configuration method may be used at a time.\n\n#### With environment variables\n\nA single Safeway account can be configured with environment variables:\n\n* `SAFEWAY_ACCOUNT_USERNAME`: Account email address (required)\n* `SAFEWAY_ACCOUNT_PASSWORD`: Account password (required)\n* `SAFEWAY_ACCOUNT_MAIL_FROM`: Sender address for email summary\n* `SAFEWAY_ACCOUNT_MAIL_TO`: Recipient address for email summary\n\n#### With config file\n\nMultiple Safeway accounts can be provided in an ini-style config file, with a\nsection for each account. For example:\n\n```ini\nemail_sender = sender@example.com   ; optional\n\n[safeway.account@example.com]       ; required\npassword = 12345                    ; required\nnotify = your.email@example.com     ; optional\n```\n\nProvide the path to your config file using the `-c` or `--accounts-config`\noption:\n\n```console\nsafeway-coupons -c path/to/config/file\n```\n\n## Development\n\n### [Poetry][poetry] installation\n\nVia [`pipx`][pipx]:\n\n```console\npip install pipx\npipx install poetry\npipx inject poetry poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\nVia `pip`:\n\n```console\npip install poetry\npoetry self add poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\n### Development tasks\n\n* Setup: `poetry install`\n* Run static checks: `poetry run poe lint` or\n  `poetry run pre-commit run --all-files`\n* Run static checks and tests: `poetry run poe test`\n\n---\n\nCreated from [smkent/cookie-python][cookie-python] using\n[cookiecutter][cookiecutter]\n\n[codecov]: https://codecov.io/gh/smkent/safeway-coupons\n[cookie-python]: https://github.com/smkent/cookie-python\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain\n[pipx]: https://pypa.github.io/pipx/\n[poetry]: https://python-poetry.org/docs/#installation\n[pypi]: https://pypi.org/project/safeway-coupons/\n[repo]: https://github.com/smkent/safeway-coupons\n[requests]: https://requests.readthedocs.io/en/latest/\n',
     'author': 'Stephen Kent',
     'author_email': 'smkent@smkent.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smkent/safeway-coupons',
```

### Comparing `safeway_coupons-0.2.2/PKG-INFO` & `safeway_coupons-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeway-coupons
-Version: 0.2.2
+Version: 0.2.3
 Summary: Automatic coupon clipper for Safeway's online "Safeway for U" coupons
 Home-page: https://github.com/smkent/safeway-coupons
 License: GPL-3.0-or-later
 Author: Stephen Kent
 Author-email: smkent@smkent.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

