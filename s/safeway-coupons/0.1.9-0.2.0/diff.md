# Comparing `tmp/safeway_coupons-0.1.9.tar.gz` & `tmp/safeway_coupons-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeway_coupons-0.1.9.tar", max compression
+gzip compressed data, was "safeway_coupons-0.2.0.tar", max compression
```

## Comparing `safeway_coupons-0.1.9.tar` & `safeway_coupons-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/LICENSE
--rw-r--r--   0        0        0     4760 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/README.md
--rw-r--r--   0        0        0     2458 2022-11-05 07:23:15.846940 safeway_coupons-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      166 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/safeway_coupons/__init__.py
--rw-r--r--   0        0        0       22 2022-11-05 07:23:15.850941 safeway_coupons-0.1.9/safeway_coupons/__version__.py
--rw-r--r--   0        0        0      161 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/safeway_coupons/accounts.py
--rw-r--r--   0        0        0     2496 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/safeway_coupons/app.py
--rw-r--r--   0        0        0     2066 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/safeway_coupons/client.py
--rw-r--r--   0        0        0     2138 2022-11-05 07:22:05.035852 safeway_coupons-0.1.9/safeway_coupons/config.py
--rw-r--r--   0        0        0     2435 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/email.py
--rw-r--r--   0        0        0      955 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/errors.py
--rw-r--r--   0        0        0     1029 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/methods.py
--rw-r--r--   0        0        0     2103 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/models.py
--rw-r--r--   0        0        0        0 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/py.typed
--rw-r--r--   0        0        0     3388 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/safeway.py
--rw-r--r--   0        0        0     2936 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/session.py
--rw-r--r--   0        0        0     2645 2022-11-05 07:22:05.039852 safeway_coupons-0.1.9/safeway_coupons/utils.py
--rw-r--r--   0        0        0     5805 1970-01-01 00:00:00.000000 safeway_coupons-0.1.9/setup.py
--rw-r--r--   0        0        0     5812 1970-01-01 00:00:00.000000 safeway_coupons-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 03:57:38.656391 safeway_coupons-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5424 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/README.md
+-rw-r--r--   0        0        0     2457 2023-07-10 03:58:12.445020 safeway_coupons-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-10 03:58:12.445020 safeway_coupons-0.2.0/safeway_coupons/__version__.py
+-rw-r--r--   0        0        0      161 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/accounts.py
+-rw-r--r--   0        0        0     2889 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/app.py
+-rw-r--r--   0        0        0     2129 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/client.py
+-rw-r--r--   0        0        0     2138 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/config.py
+-rw-r--r--   0        0        0     2960 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/email.py
+-rw-r--r--   0        0        0     1025 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/errors.py
+-rw-r--r--   0        0        0     1029 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/methods.py
+-rw-r--r--   0        0        0     2103 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/py.typed
+-rw-r--r--   0        0        0     3528 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/safeway.py
+-rw-r--r--   0        0        0     5646 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/session.py
+-rw-r--r--   0        0        0      846 2023-07-10 03:57:38.660390 safeway_coupons-0.2.0/safeway_coupons/utils.py
+-rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 safeway_coupons-0.2.0/setup.py
+-rw-r--r--   0        0        0     6559 1970-01-01 00:00:00.000000 safeway_coupons-0.2.0/PKG-INFO
```

### Comparing `safeway_coupons-0.1.9/LICENSE` & `safeway_coupons-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.1.9/README.md` & `safeway_coupons-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 [![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]
 [![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]
 
 **safeway-coupons** is a script that will log in to an account on safeway.com,
 and attempt to select all of the "Safeway for U" electronic coupons on the site
 so they don't have to each be clicked manually.
 
+## Design notes
+
+Safeway's sign in page is protected by a web application firewall (WAF).
+safeway-coupons performs authentication using a headless instance of Google
+Chrome. Authentication may fail based on your IP's reputation, either by
+presenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons
+currently does not have support for prompting the user to solve CAPTCHAs.
+
+Once a signed in session is established, coupon clipping is performed using HTTP
+requests via [requests][requests].
+
 ## Installation and usage with Docker
 
 A Docker container is provided which runs safeway-coupons with cron. The cron
 schedule and your Safeway account details may be configured using environment
 variables, or with an accounts file.
 
 Example `docker-compose.yaml` with configuration via environment variables:
@@ -61,26 +72,31 @@
 
 ```console
 docker-compose logs -f
 ```
 
 ## Installation from PyPI
 
+### Prerequisites
+
+* Google Chrome (for authentication performed via Selenium).
+* Optional: `sendmail` (for email support)
+
+### Installation
+
 [safeway-coupons is available on PyPI][pypi]:
 
 ```console
 pip install safeway-coupons
 ```
 
-`sendmail` is needed for email support.
+### Usage
 
 For best results, run this program once a day or so with a cron daemon.
 
-### Usage
-
 For full usage options, run
 
 ```console
 safeway-coupons --help
 ```
 
 ### Configuration
@@ -159,7 +175,8 @@
 [cookie-python]: https://github.com/smkent/cookie-python
 [cookiecutter]: https://github.com/cookiecutter/cookiecutter
 [gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain
 [pipx]: https://pypa.github.io/pipx/
 [poetry]: https://python-poetry.org/docs/#installation
 [pypi]: https://pypi.org/project/safeway-coupons/
 [repo]: https://github.com/smkent/safeway-coupons
+[requests]: https://requests.readthedocs.io/en/latest/
```

### Comparing `safeway_coupons-0.1.9/pyproject.toml` & `safeway_coupons-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 [build-system]
 requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "safeway-coupons"
-version = "0.1.9"
+version = "0.2.0"
 description = "Automatic coupon clipper for Safeway's online \"Safeway for U\" coupons"
 license = "GPL-3.0-or-later"
 authors = ["Stephen Kent <smkent@smkent.net>"]
 readme = "README.md"
 repository = "https://github.com/smkent/safeway-coupons"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-dataclasses-json = "^0.5.7"
-pre-commit = "*"
-requests = "^2.28.1"
+dataclasses-json = "*"
+requests = "*"
+selenium = "^4.10"
+webdriver-manager = "^3.8.6"
+undetected-chromedriver = "^3.5.0"
 
 [tool.poetry.dev-dependencies]
 bandit = {extras = ["toml"], version = "*"}
 black = "*"
 cruft = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-pyproject = "*"
 flake8-simplify = "*"
 isort = "*"
 mypy = "*"
 pep8-naming = "*"
 poethepoet = "*"
-py = "1.11.0"  # https://github.com/Teemu/pytest-sugar/issues/241
+pre-commit = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-github-actions-annotate-failures = "*"
 pytest-sugar = "*"
-types-requests = "^2.28.9"
-pytest-mock = "^3.8.2"
-responses = "^0.21.0"
+types-requests = "*"
+pytest-mock = "*"
+responses = "*"
 
 [tool.poetry.scripts]
 safeway-coupons = "safeway_coupons.app:main"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `safeway_coupons-0.1.9/safeway_coupons/app.py` & `safeway_coupons-0.2.0/safeway_coupons/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import sys
 from http.client import HTTPConnection
+from pathlib import Path
 
 from .config import Config
 from .safeway import SafewayCoupons
 
 
 def _parse_args() -> argparse.Namespace:
     description = 'Automatic coupon clipper for "Safeway for U" coupons'
@@ -16,14 +17,25 @@
         metavar="file",
         help=(
             "Path to configuration file containing Safeway "
             "accounts information"
         ),
     )
     arg_parser.add_argument(
+        "-D",
+        "--debug-dir",
+        dest="debug_dir",
+        metavar="directory",
+        default=".",
+        help=(
+            "Destination directory for debug output files, "
+            "such as browser screenshots (default: %(default)s)"
+        ),
+    )
+    arg_parser.add_argument(
         "-d",
         "--debug",
         dest="debug_level",
         action="count",
         default=0,
         help=(
             "Print debugging information on stdout. Specify "
@@ -75,14 +87,15 @@
         print("Error: No Safeway account(s) configured", file=sys.stderr)
         sys.exit(1)
     if args.debug_level >= 2:
         HTTPConnection.debuglevel = 1
     sc = SafewayCoupons(
         send_email=args.send_email,
         debug_level=args.debug_level,
+        debug_dir=Path(args.debug_dir) if args.debug_dir else None,
         sleep_level=args.sleep_level,
         dry_run=args.dry_run,
         max_clip_count=args.max_clip_count,
     )
     try:
         for account in accounts:
             sc.clip_for_account(account)
```

### Comparing `safeway_coupons-0.1.9/safeway_coupons/client.py` & `safeway_coupons-0.2.0/safeway_coupons/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import random
+from pathlib import Path
 from typing import List, Optional
 
 import requests
 
 from .accounts import Account
 from .errors import ClipError, HTTPError
 from .methods import ClipRequest, ClipResponse
 from .models import Offer, OfferList
 from .session import BaseSession, LoginSession
 
 
 class SafewayClient(BaseSession):
-    def __init__(self, account: Account) -> None:
-        self.session = LoginSession(account)
+    def __init__(self, account: Account, debug_dir: Optional[Path]) -> None:
+        self.session = LoginSession(account, debug_dir)
         self.requests.headers.update(
             {
                 "Authorization": f"Bearer {self.session.access_token}",
                 "X-SW" "Y_AP" "I_K" "EY": "em" "j" "ou",
                 "X-SW" "Y_VERSION": "1.1",
                 "X-SW" "Y-APPLICATION-TYPE": "web",
             }
```

### Comparing `safeway_coupons-0.1.9/safeway_coupons/config.py` & `safeway_coupons-0.2.0/safeway_coupons/config.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.1.9/safeway_coupons/email.py` & `safeway_coupons-0.2.0/safeway_coupons/email.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 import collections
+import mimetypes
 import os
 import subprocess
-from email.mime.text import MIMEText
+from email.message import EmailMessage
+from pathlib import Path
 from typing import List, Optional
 
 from .accounts import Account
 from .errors import ClipError, Error, TooManyClipErrors
 from .models import Offer
 
 
 def _send_email(
     account: Account,
     subject: str,
     mail_message: List[str],
     debug_level: int,
     send_email: bool,
+    attachments: Optional[List[Path]] = None,
 ) -> None:
     mail_message_str = os.linesep.join(mail_message)
     if debug_level >= 1:
         if send_email:
             print(f"Sending email to {account.mail_to}")
         else:
             print(f"Would send email to {account.mail_to}")
         print(">>>>>>")
         print(mail_message_str)
         print("<<<<<<")
     if not send_email:
         return
-    email_data = MIMEText(mail_message_str)
-    email_data["To"] = account.mail_to
-    email_data["From"] = account.mail_from
+    msg = EmailMessage()
+    msg["To"] = account.mail_to
+    msg["From"] = account.mail_from
     if subject:
-        email_data["Subject"] = subject
+        msg["Subject"] = subject
+    msg.set_content(mail_message_str)
+    for attachment in attachments or []:
+        mt = mimetypes.guess_type(attachment.name)[0]
+        main, sub = mt.split("/", 1) if mt else ("application", "octet-stream")
+        msg.add_attachment(
+            attachment.read_bytes(),
+            filename=attachment.name,
+            maintype=main,
+            subtype=sub,
+        )
     p = subprocess.Popen(
         ["/usr/sbin/sendmail", "-f", account.mail_to, "-t"],
         stdin=subprocess.PIPE,
     )
-    p.communicate(bytes(email_data.as_string(), "UTF-8"))
+    p.communicate(bytes(msg.as_string(), "UTF-8"))
 
 
 def email_clip_results(
     account: Account,
     offers: List[Offer],
     error: Optional[Error],
     clip_errors: Optional[List[ClipError]],
@@ -73,8 +86,15 @@
         f"Safeway account: {account.username}",
         f"Error: {error}",
     ]
     if isinstance(error, TooManyClipErrors) and error.clipped_offers:
         mail_message += ["Clipped coupons:", ""]
         for offer in error.clipped_offers:
             mail_message += str(offer)
-    _send_email(account, mail_subject, mail_message, debug_level, send_email)
+    _send_email(
+        account,
+        mail_subject,
+        mail_message,
+        debug_level,
+        send_email,
+        attachments=getattr(error, "attachments", None),
+    )
```

### Comparing `safeway_coupons-0.1.9/safeway_coupons/errors.py` & `safeway_coupons-0.2.0/safeway_coupons/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from pathlib import Path
 from typing import List, Optional
 
 import requests
 
 from .accounts import Account
 from .models import Offer
 
@@ -11,14 +12,15 @@
 class Error(Exception):
     exception: Exception
 
 
 @dataclass
 class AuthenticationFailure(Error):
     account: Account
+    attachments: Optional[List[Path]] = None
 
     def __str__(self) -> str:
         return f"Authentication Failure ({self.exception})"
 
 
 @dataclass
 class HTTPError(Error):
```

### Comparing `safeway_coupons-0.1.9/safeway_coupons/methods.py` & `safeway_coupons-0.2.0/safeway_coupons/methods.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.1.9/safeway_coupons/models.py` & `safeway_coupons-0.2.0/safeway_coupons/models.py`

 * *Files identical despite different names*

### Comparing `safeway_coupons-0.1.9/safeway_coupons/safeway.py` & `safeway_coupons-0.2.0/safeway_coupons/safeway.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List
+from pathlib import Path
+from typing import List, Optional
 
 from .accounts import Account
 from .client import SafewayClient
 from .email import email_clip_results, email_error
 from .errors import ClipError, Error, TooManyClipErrors
 from .models import Offer, OfferStatus
 from .utils import yield_delay
@@ -11,32 +12,34 @@
 
 
 class SafewayCoupons:
     def __init__(
         self,
         send_email: bool = True,
         debug_level: int = 0,
+        debug_dir: Optional[Path] = None,
         sleep_level: int = 0,
         dry_run: bool = False,
         max_clip_count: int = 0,
         max_clip_errors: int = CLIP_ERROR_MAX,
     ) -> None:
         self.send_email = send_email
         self.debug_level = debug_level
+        self.debug_dir = debug_dir
         self.sleep_level = sleep_level
         self.dry_run = dry_run
         self.max_clip_count = max_clip_count
         self.max_clip_errors = max_clip_errors
 
     def clip_for_account(self, account: Account) -> None:
         print(f"Clipping coupons for Safeway account {account.username}")
-        swy = SafewayClient(account)
-        clipped_offers: List[Offer] = []
-        clip_errors: List[ClipError] = []
         try:
+            swy = SafewayClient(account, self.debug_dir)
+            clipped_offers: List[Offer] = []
+            clip_errors: List[ClipError] = []
             offers = swy.get_offers()
             unclipped_offers = [
                 o for o in offers if o.status == OfferStatus.Unclipped
             ]
             if not unclipped_offers:
                 print("Nothing to do")
                 return
```

### Comparing `safeway_coupons-0.1.9/setup.py` & `safeway_coupons-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 packages = \
 ['safeway_coupons']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dataclasses-json>=0.5.7,<0.6.0', 'pre-commit', 'requests>=2.28.1,<3.0.0']
+['dataclasses-json',
+ 'requests',
+ 'selenium>=4.10,<5.0',
+ 'undetected-chromedriver>=3.5.0,<4.0.0',
+ 'webdriver-manager>=3.8.6,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['safeway-coupons = safeway_coupons.app:main']}
 
 setup_kwargs = {
     'name': 'safeway-coupons',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Automatic coupon clipper for Safeway\'s online "Safeway for U" coupons',
-    'long_description': '# Automatic Safeway coupon clipper\n\n[![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]\n[![Build](https://img.shields.io/github/checks-status/smkent/safeway-coupons/main?label=build)][gh-actions]\n[![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]\n[![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]\n\n**safeway-coupons** is a script that will log in to an account on safeway.com,\nand attempt to select all of the "Safeway for U" electronic coupons on the site\nso they don\'t have to each be clicked manually.\n\n## Installation and usage with Docker\n\nA Docker container is provided which runs safeway-coupons with cron. The cron\nschedule and your Safeway account details may be configured using environment\nvariables, or with an accounts file.\n\nExample `docker-compose.yaml` with configuration via environment variables:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com\n      SAFEWAY_ACCOUNT_PASSWORD: very_secret\n      SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com\n      SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com\n    restart: unless-stopped\n```\n\nExample `docker-compose.yaml` with configuration via accounts file:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNTS_FILE: /accounts_file\n    restart: unless-stopped\n    volumes:\n      - path/to/safeway_accounts_file:/accounts_file:ro\n```\n\nStart the container by running:\n\n```console\ndocker-compose up -d\n```\n\nDebugging information can be viewed in the container log:\n\n```console\ndocker-compose logs -f\n```\n\n## Installation from PyPI\n\n[safeway-coupons is available on PyPI][pypi]:\n\n```console\npip install safeway-coupons\n```\n\n`sendmail` is needed for email support.\n\nFor best results, run this program once a day or so with a cron daemon.\n\n### Usage\n\nFor full usage options, run\n\n```console\nsafeway-coupons --help\n```\n\n### Configuration\n\n**safeway-coupons** can clip coupons for one or more Safeway accounts in a\nsingle run, depending on the configuration method used.\n\nIf a sender email address is configured, a summary email will be sent for each\nSafeway account via `sendmail`. The email recipient defaults to the Safeway\naccount email address, but can be overridden for each account.\n\nAccounts are searched via the following methods in the listed order. Only one\naccount configuration method may be used at a time.\n\n#### With environment variables\n\nA single Safeway account can be configured with environment variables:\n\n* `SAFEWAY_ACCOUNT_USERNAME`: Account email address (required)\n* `SAFEWAY_ACCOUNT_PASSWORD`: Account password (required)\n* `SAFEWAY_ACCOUNT_MAIL_FROM`: Sender address for email summary\n* `SAFEWAY_ACCOUNT_MAIL_TO`: Recipient address for email summary\n\n#### With config file\n\nMultiple Safeway accounts can be provided in an ini-style config file, with a\nsection for each account. For example:\n\n```ini\nemail_sender = sender@example.com   ; optional\n\n[safeway.account@example.com]       ; required\npassword = 12345                    ; required\nnotify = your.email@example.com     ; optional\n```\n\nProvide the path to your config file using the `-c` or `--accounts-config`\noption:\n\n```console\nsafeway-coupons -c path/to/config/file\n```\n\n## Development\n\n### [Poetry][poetry] installation\n\nVia [`pipx`][pipx]:\n\n```console\npip install pipx\npipx install poetry\npipx inject poetry poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\nVia `pip`:\n\n```console\npip install poetry\npoetry self add poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\n### Development tasks\n\n* Setup: `poetry install`\n* Run static checks: `poetry run poe lint` or\n  `poetry run pre-commit run --all-files`\n* Run static checks and tests: `poetry run poe test`\n\n---\n\nCreated from [smkent/cookie-python][cookie-python] using\n[cookiecutter][cookiecutter]\n\n[codecov]: https://codecov.io/gh/smkent/safeway-coupons\n[cookie-python]: https://github.com/smkent/cookie-python\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain\n[pipx]: https://pypa.github.io/pipx/\n[poetry]: https://python-poetry.org/docs/#installation\n[pypi]: https://pypi.org/project/safeway-coupons/\n[repo]: https://github.com/smkent/safeway-coupons\n',
+    'long_description': '# Automatic Safeway coupon clipper\n\n[![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]\n[![Build](https://img.shields.io/github/checks-status/smkent/safeway-coupons/main?label=build)][gh-actions]\n[![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]\n[![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]\n\n**safeway-coupons** is a script that will log in to an account on safeway.com,\nand attempt to select all of the "Safeway for U" electronic coupons on the site\nso they don\'t have to each be clicked manually.\n\n## Design notes\n\nSafeway\'s sign in page is protected by a web application firewall (WAF).\nsafeway-coupons performs authentication using a headless instance of Google\nChrome. Authentication may fail based on your IP\'s reputation, either by\npresenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons\ncurrently does not have support for prompting the user to solve CAPTCHAs.\n\nOnce a signed in session is established, coupon clipping is performed using HTTP\nrequests via [requests][requests].\n\n## Installation and usage with Docker\n\nA Docker container is provided which runs safeway-coupons with cron. The cron\nschedule and your Safeway account details may be configured using environment\nvariables, or with an accounts file.\n\nExample `docker-compose.yaml` with configuration via environment variables:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNT_USERNAME: your.safeway.account.email@example.com\n      SAFEWAY_ACCOUNT_PASSWORD: very_secret\n      SAFEWAY_ACCOUNT_MAIL_FROM: your.email@example.com\n      SAFEWAY_ACCOUNT_MAIL_TO: your.email@example.com\n    restart: unless-stopped\n```\n\nExample `docker-compose.yaml` with configuration via accounts file:\n\n```yaml\nversion: "3.7"\n\nservices:\n  safeway-coupons:\n    image: ghcr.io/smkent/safeway-coupons:latest\n    environment:\n      CRON_SCHEDULE: "0 2 * * *"  # Run at 2:00 AM each day\n      SMTPHOST: your.smtp.host\n      SAFEWAY_ACCOUNTS_FILE: /accounts_file\n    restart: unless-stopped\n    volumes:\n      - path/to/safeway_accounts_file:/accounts_file:ro\n```\n\nStart the container by running:\n\n```console\ndocker-compose up -d\n```\n\nDebugging information can be viewed in the container log:\n\n```console\ndocker-compose logs -f\n```\n\n## Installation from PyPI\n\n### Prerequisites\n\n* Google Chrome (for authentication performed via Selenium).\n* Optional: `sendmail` (for email support)\n\n### Installation\n\n[safeway-coupons is available on PyPI][pypi]:\n\n```console\npip install safeway-coupons\n```\n\n### Usage\n\nFor best results, run this program once a day or so with a cron daemon.\n\nFor full usage options, run\n\n```console\nsafeway-coupons --help\n```\n\n### Configuration\n\n**safeway-coupons** can clip coupons for one or more Safeway accounts in a\nsingle run, depending on the configuration method used.\n\nIf a sender email address is configured, a summary email will be sent for each\nSafeway account via `sendmail`. The email recipient defaults to the Safeway\naccount email address, but can be overridden for each account.\n\nAccounts are searched via the following methods in the listed order. Only one\naccount configuration method may be used at a time.\n\n#### With environment variables\n\nA single Safeway account can be configured with environment variables:\n\n* `SAFEWAY_ACCOUNT_USERNAME`: Account email address (required)\n* `SAFEWAY_ACCOUNT_PASSWORD`: Account password (required)\n* `SAFEWAY_ACCOUNT_MAIL_FROM`: Sender address for email summary\n* `SAFEWAY_ACCOUNT_MAIL_TO`: Recipient address for email summary\n\n#### With config file\n\nMultiple Safeway accounts can be provided in an ini-style config file, with a\nsection for each account. For example:\n\n```ini\nemail_sender = sender@example.com   ; optional\n\n[safeway.account@example.com]       ; required\npassword = 12345                    ; required\nnotify = your.email@example.com     ; optional\n```\n\nProvide the path to your config file using the `-c` or `--accounts-config`\noption:\n\n```console\nsafeway-coupons -c path/to/config/file\n```\n\n## Development\n\n### [Poetry][poetry] installation\n\nVia [`pipx`][pipx]:\n\n```console\npip install pipx\npipx install poetry\npipx inject poetry poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\nVia `pip`:\n\n```console\npip install poetry\npoetry self add poetry-dynamic-versioning poetry-pre-commit-plugin\n```\n\n### Development tasks\n\n* Setup: `poetry install`\n* Run static checks: `poetry run poe lint` or\n  `poetry run pre-commit run --all-files`\n* Run static checks and tests: `poetry run poe test`\n\n---\n\nCreated from [smkent/cookie-python][cookie-python] using\n[cookiecutter][cookiecutter]\n\n[codecov]: https://codecov.io/gh/smkent/safeway-coupons\n[cookie-python]: https://github.com/smkent/cookie-python\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain\n[pipx]: https://pypa.github.io/pipx/\n[poetry]: https://python-poetry.org/docs/#installation\n[pypi]: https://pypi.org/project/safeway-coupons/\n[repo]: https://github.com/smkent/safeway-coupons\n[requests]: https://requests.readthedocs.io/en/latest/\n',
     'author': 'Stephen Kent',
     'author_email': 'smkent@smkent.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smkent/safeway-coupons',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `safeway_coupons-0.1.9/PKG-INFO` & `safeway_coupons-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeway-coupons
-Version: 0.1.9
+Version: 0.2.0
 Summary: Automatic coupon clipper for Safeway's online "Safeway for U" coupons
 Home-page: https://github.com/smkent/safeway-coupons
 License: GPL-3.0-or-later
 Author: Stephen Kent
 Author-email: smkent@smkent.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,17 +13,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
-Requires-Dist: pre-commit
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: dataclasses-json
+Requires-Dist: requests
+Requires-Dist: selenium (>=4.10,<5.0)
+Requires-Dist: undetected-chromedriver (>=3.5.0,<4.0.0)
+Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Project-URL: Repository, https://github.com/smkent/safeway-coupons
 Description-Content-Type: text/markdown
 
 # Automatic Safeway coupon clipper
 
 [![PyPI](https://img.shields.io/pypi/v/safeway-coupons)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/safeway-coupons)][pypi]
@@ -31,14 +33,25 @@
 [![codecov](https://codecov.io/gh/smkent/safeway-coupons/branch/main/graph/badge.svg)][codecov]
 [![GitHub stars](https://img.shields.io/github/stars/smkent/safeway-coupons?style=social)][repo]
 
 **safeway-coupons** is a script that will log in to an account on safeway.com,
 and attempt to select all of the "Safeway for U" electronic coupons on the site
 so they don't have to each be clicked manually.
 
+## Design notes
+
+Safeway's sign in page is protected by a web application firewall (WAF).
+safeway-coupons performs authentication using a headless instance of Google
+Chrome. Authentication may fail based on your IP's reputation, either by
+presenting a CAPTCHA or denying sign in attempts altogether. safeway-coupons
+currently does not have support for prompting the user to solve CAPTCHAs.
+
+Once a signed in session is established, coupon clipping is performed using HTTP
+requests via [requests][requests].
+
 ## Installation and usage with Docker
 
 A Docker container is provided which runs safeway-coupons with cron. The cron
 schedule and your Safeway account details may be configured using environment
 variables, or with an accounts file.
 
 Example `docker-compose.yaml` with configuration via environment variables:
@@ -86,26 +99,31 @@
 
 ```console
 docker-compose logs -f
 ```
 
 ## Installation from PyPI
 
+### Prerequisites
+
+* Google Chrome (for authentication performed via Selenium).
+* Optional: `sendmail` (for email support)
+
+### Installation
+
 [safeway-coupons is available on PyPI][pypi]:
 
 ```console
 pip install safeway-coupons
 ```
 
-`sendmail` is needed for email support.
+### Usage
 
 For best results, run this program once a day or so with a cron daemon.
 
-### Usage
-
 For full usage options, run
 
 ```console
 safeway-coupons --help
 ```
 
 ### Configuration
@@ -184,8 +202,9 @@
 [cookie-python]: https://github.com/smkent/cookie-python
 [cookiecutter]: https://github.com/cookiecutter/cookiecutter
 [gh-actions]: https://github.com/smkent/safeway-coupons/actions?query=branch%3Amain
 [pipx]: https://pypa.github.io/pipx/
 [poetry]: https://python-poetry.org/docs/#installation
 [pypi]: https://pypi.org/project/safeway-coupons/
 [repo]: https://github.com/smkent/safeway-coupons
+[requests]: https://requests.readthedocs.io/en/latest/
```

