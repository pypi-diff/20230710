# Comparing `tmp/edc-phq9-0.1.8.tar.gz` & `tmp/edc-phq9-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-phq9-0.1.8.tar", last modified: Sun Sep 25 22:11:23 2022, max compression
+gzip compressed data, was "edc-phq9-0.1.9.tar", last modified: Wed May 24 17:07:34 2023, max compression
```

## Comparing `edc-phq9-0.1.8.tar` & `edc-phq9-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.312485 edc-phq9-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.303979 edc-phq9-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.307394 edc-phq9-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-01-05 14:54:30.000000 edc-phq9-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:11:23.312598 edc-phq9-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      650 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.309925 edc-phq9-0.1.8/edc_phq9/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      891 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/edc_phq9/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      396 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      383 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      305 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      351 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      126 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1156 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/edc_phq9/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      885 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/model_admin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3236 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/edc_phq9/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.310700 edc-phq9-0.1.8/edc_phq9/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.311805 edc-phq9-0.1.8/edc_phq9/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.312320 edc-phq9-0.1.8/edc_phq9/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-08-26 02:19:49.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1329 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.310606 edc-phq9-0.1.8/edc_phq9.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1155 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-01-05 15:20:02.000000 edc-phq9-0.1.8/edc_phq9.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        9 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2085 2022-08-26 02:19:49.000000 edc-phq9-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1228 2022-09-25 22:11:23.312945 edc-phq9-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.075961 edc-phq9-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.067546 edc-phq9-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.071272 edc-phq9-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 22:19:44.000000 edc-phq9-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:17:52.000000 edc-phq9-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 22:19:44.000000 edc-phq9-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-06-01 22:19:44.000000 edc-phq9-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-01-05 14:54:30.000000 edc-phq9-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 22:19:44.000000 edc-phq9-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1491 2023-05-24 17:07:34.076057 edc-phq9-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      650 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:17:52.000000 edc-phq9-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.073293 edc-phq9-0.1.9/edc_phq9/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      890 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/edc_phq9/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      396 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      383 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      305 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      351 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      126 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1156 2022-09-25 22:11:15.000000 edc-phq9-0.1.9/edc_phq9/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      885 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/model_admin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3235 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/edc_phq9/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      654 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/edc_phq9/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.074256 edc-phq9-0.1.9/edc_phq9/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.075356 edc-phq9-0.1.9/edc_phq9/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.075796 edc-phq9-0.1.9/edc_phq9/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-08-26 02:19:49.000000 edc-phq9-0.1.9/edc_phq9/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1329 2022-06-01 22:19:44.000000 edc-phq9-0.1.9/edc_phq9/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-01-06 03:46:37.000000 edc-phq9-0.1.9/edc_phq9/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:07:34.074115 edc-phq9-0.1.9/edc_phq9.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1491 2023-05-24 17:07:34.000000 edc-phq9-0.1.9/edc_phq9.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1147 2023-05-24 17:07:34.000000 edc-phq9-0.1.9/edc_phq9.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:07:34.000000 edc-phq9-0.1.9/edc_phq9.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-01-05 15:20:02.000000 edc-phq9-0.1.9/edc_phq9.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        9 2023-05-24 17:07:34.000000 edc-phq9-0.1.9/edc_phq9.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1762 2023-05-24 17:07:25.000000 edc-phq9-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2085 2022-08-26 02:19:49.000000 edc-phq9-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1135 2023-05-24 17:07:34.076347 edc-phq9-0.1.9/setup.cfg
```

### Comparing `edc-phq9-0.1.8/.github/workflows/build.yml` & `edc-phq9-0.1.9/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,20 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10']
-        django-version: ['3.2', '4.0', '4.1', 'dev']
-
+        python-version: ['3.10', '3.11']
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
@@ -28,28 +29,27 @@
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
-
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -61,11 +61,11 @@
 
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
-      - name: Upload coverage
-        uses: codecov/codecov-action@v1
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-phq9-0.1.8/.gitignore` & `edc-phq9-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/.pre-commit-config.yaml` & `edc-phq9-0.1.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-phq9-0.1.8/LICENSE` & `edc-phq9-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/PKG-INFO` & `edc-phq9-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-phq9
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for PHQ9 in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-phq9
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc phq9,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc PHQ9
```

### Comparing `edc-phq9-0.1.8/README.rst` & `edc-phq9-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/admin.py` & `edc-phq9-0.1.9/edc_phq9/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,11 +28,10 @@
 
 
 @admin.register(Phq9, site=edc_phq9_admin)
 class Phq9Admin(
     Phq9ModelAdminMixin,
     SimpleHistoryAdmin,
 ):
-
     form = Phq9Form
 
     fieldsets = get_fieldsets()
```

### Comparing `edc-phq9-0.1.8/edc_phq9/fieldsets.py` & `edc-phq9-0.1.9/edc_phq9/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/forms.py` & `edc-phq9-0.1.9/edc_phq9/forms.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/model_admin_mixins.py` & `edc-phq9-0.1.9/edc_phq9/model_admin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/model_mixins.py` & `edc-phq9-0.1.9/edc_phq9/model_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from edc_constants.choices import YES_NO
 from edc_constants.constants import NOT_APPLICABLE, YES
 
 from .choices import PHQ_CHOICES
 
 
 class Phq9ModelMixin(models.Model):
-
     ph9_performed = models.CharField(
         verbose_name="Is the PH9 assessment being performed?",
         max_length=15,
         choices=YES_NO,
         default=YES,
     )
```

### Comparing `edc-phq9-0.1.8/edc_phq9/models.py` & `edc-phq9-0.1.9/edc_phq9/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 class Phq9(
     UniqueSubjectIdentifierFieldMixin,
     Phq9ModelMixin,
     SiteModelMixin,
     BaseUuidModel,
 ):
-
     report_datetime = models.DateTimeField(default=get_utcnow)
 
     on_site = CurrentSiteManager()
     objects = models.Manager()
     history = HistoricalRecords()
 
     class Meta(Phq9ModelMixin.Meta, BaseUuidModel.Meta):
```

### Comparing `edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-private.pem` & `edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-private.pem` & `edc-phq9-0.1.9/edc_phq9/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9/tests/tests/tests.py` & `edc-phq9-0.1.9/edc_phq9/tests/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/edc_phq9.egg-info/PKG-INFO` & `edc-phq9-0.1.9/edc_phq9.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-phq9
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for PHQ9 in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-phq9
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc phq9,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc PHQ9
```

### Comparing `edc-phq9-0.1.8/edc_phq9.egg-info/SOURCES.txt` & `edc-phq9-0.1.9/edc_phq9.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .pre-commit-config.yaml
 .yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
-VERSION
 codecov.yml
 pyproject.toml
 runtests.py
 setup.cfg
 .github/workflows/build.yml
 edc_phq9/__init__.py
 edc_phq9/admin.py
```

### Comparing `edc-phq9-0.1.8/pyproject.toml` & `edc-phq9-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,70 +3,72 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_phq9"]
 
 [tool.coverage.paths]
 source = ["edc_phq9"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{38,39,310}-dj{32,40,41,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.8: py38
-    3.9: py39, lint
     3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
-    4.0: dj40
     4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-phq9-0.1.8/runtests.py` & `edc-phq9-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.8/setup.cfg` & `edc-phq9-0.1.9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 description = Classes for PHQ9 in clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc phq9, CRF, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	examples*
```

