# Comparing `tmp/pytest-randomly-3.8.0.tar.gz` & `tmp/pytest-randomly-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-randomly-3.8.0.tar", last modified: Mon May 10 11:00:18 2021, max compression
+gzip compressed data, was "pytest-randomly-3.9.0.tar", last modified: Thu Aug 12 21:39:53 2021, max compression
```

## Comparing `pytest-randomly-3.8.0.tar` & `pytest-randomly-3.9.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-05-10 11:00:18.949999 pytest-randomly-3.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     4534 2021-05-10 11:00:11.000000 pytest-randomly-3.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1074 2021-02-07 17:48:42.000000 pytest-randomly-3.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      258 2021-03-19 11:45:22.000000 pytest-randomly-3.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     9213 2021-05-10 11:00:18.950416 pytest-randomly-3.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     6713 2021-05-10 11:00:00.000000 pytest-randomly-3.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)     6741 2021-02-07 17:48:42.000000 pytest-randomly-3.8.0/logo.png
--rw-r--r--   0 chainz     (501) staff       (20)      172 2021-02-07 17:48:42.000000 pytest-randomly-3.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1399 2021-05-10 11:00:18.951515 pytest-randomly-3.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 17:48:42.000000 pytest-randomly-3.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-05-10 11:00:18.945789 pytest-randomly-3.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-05-10 11:00:18.949498 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     9213 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      410 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       39 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       61 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       16 2021-05-10 11:00:18.000000 pytest-randomly-3.8.0/src/pytest_randomly.egg-info/top_level.txt
--rw-r--r--   0 chainz     (501) staff       (20)     6784 2021-05-10 11:00:00.000000 pytest-randomly-3.8.0/src/pytest_randomly.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-08-12 21:39:53.992901 pytest-randomly-3.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     4592 2021-08-12 21:39:46.000000 pytest-randomly-3.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1074 2021-02-07 17:48:42.000000 pytest-randomly-3.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      295 2021-08-12 21:39:35.000000 pytest-randomly-3.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     7841 2021-08-12 21:39:53.993047 pytest-randomly-3.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     6714 2021-07-07 16:41:57.000000 pytest-randomly-3.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     6741 2021-02-07 17:48:42.000000 pytest-randomly-3.9.0/logo.png
+-rw-r--r--   0 chainz     (501) staff       (20)      493 2021-08-12 21:39:35.000000 pytest-randomly-3.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1424 2021-08-12 21:39:53.993794 pytest-randomly-3.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 17:48:42.000000 pytest-randomly-3.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-08-12 21:39:53.988032 pytest-randomly-3.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-08-12 21:39:53.990890 pytest-randomly-3.9.0/src/pytest_randomly/
+-rw-r--r--   0 chainz     (501) staff       (20)     7626 2021-08-12 21:39:35.000000 pytest-randomly-3.9.0/src/pytest_randomly/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-12 21:39:35.000000 pytest-randomly-3.9.0/src/pytest_randomly/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-08-12 21:39:53.992674 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     7841 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      448 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       39 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/entry_points.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       61 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       16 2021-08-12 21:39:53.000000 pytest-randomly-3.9.0/src/pytest_randomly.egg-info/top_level.txt
```

### Comparing `pytest-randomly-3.8.0/HISTORY.rst` & `pytest-randomly-3.9.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+3.9.0 (2021-08-12)
+------------------
+
+* Add type hints.
+
 3.8.0 (2021-05-10)
 ------------------
 
 * Support Python 3.10.
 
 3.7.0 (2021-04-11)
 ------------------
```

### Comparing `pytest-randomly-3.8.0/LICENSE` & `pytest-randomly-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-randomly-3.8.0/PKG-INFO` & `pytest-randomly-3.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest-randomly
-Version: 3.8.0
+Version: 3.9.0
 Summary: Pytest plugin to randomly order tests and control random.seed.
 Home-page: https://github.com/pytest-dev/pytest-randomly
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/pytest-dev/pytest-randomly/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
-Description: ===============
-        pytest-randomly
-        ===============
-        
-        .. image:: https://img.shields.io/github/workflow/status/pytest-dev/pytest-randomly/CI/main?style=for-the-badge
-           :target: https://github.com/pytest-dev/pytest-randomly/actions?workflow=CI
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-randomly.svg?style=for-the-badge
-           :target: https://pypi.org/project/pytest-randomly/
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
-           :target: https://github.com/psf/black
-        
-        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
-           :target: https://github.com/pre-commit/pre-commit
-           :alt: pre-commit
-        
-        .. figure:: https://raw.githubusercontent.com/pytest-dev/pytest-randomly/main/logo.png
-           :scale: 50%
-           :alt: Randomness power.
-        
-        Pytest plugin to randomly order tests and control ``random.seed``.
-        
-        Features
-        ========
-        
-        All of these features are on by default but can be disabled with flags.
-        
-        * Randomly shuffles the order of test items. This is done first at the level of
-          modules, then at the level of test classes (if you have them), then at the
-          order of functions. This also works with things like doctests.
-        * Resets ``random.seed()`` at the start of every test case and test to a fixed
-          number - this defaults to ``time.time()`` from the start of your test run,
-          but you can pass in ``--randomly-seed`` to repeat a randomness-induced
-          failure.
-        * If
-          `factory boy <https://factoryboy.readthedocs.io/en/latest/reference.html>`_
-          is installed, its random state is reset at the start of every test. This
-          allows for repeatable use of its random 'fuzzy' features.
-        * If `faker <https://pypi.org/project/faker>`_ is installed, its random
-          state is reset at the start of every test. This is also for repeatable fuzzy
-          data in tests - factory boy uses faker for lots of data. This is also done
-          if you're using the ``faker`` pytest fixture, by defining the ``faker_seed``
-          fixture
-          (`docs <https://faker.readthedocs.io/en/master/pytest-fixtures.html#seeding-configuration>`__).
-        * If `numpy <http://www.numpy.org/>`_ is installed, its random state is reset
-          at the start of every test.
-        * If additional random generators are used, they can be registered under the
-          ``pytest_randomly.random_seeder``
-          `entry point <https://packaging.python.org/specifications/entry-points/>`_ and
-          will have their seed reset at the start of every test. Register a function
-          that takes the current seed value.
-        * Works with `pytest-xdist <https://pypi.org/project/pytest-xdist/>`__.
-        
-        About
-        =====
-        
-        Randomness in testing can be quite powerful to discover hidden flaws in the
-        tests themselves, as well as giving a little more coverage to your system.
-        
-        By randomly ordering the tests, the risk of surprising inter-test dependencies
-        is reduced - a technique used in many places, for example Google's C++ test
-        runner `googletest
-        <https://code.google.com/p/googletest/wiki/V1_5_AdvancedGuide#Shuffling_the_Tests>`_.
-        Research suggests that "dependent tests do exist in practice" and a random
-        order of test executions can effectively detect such dependencies [1]_.
-        Alternatively, a reverse order of test executions, as provided by `pytest-reverse
-        <https://github.com/adamchainz/pytest-reverse>`__, may find less dependent
-        tests but can achieve a better benefit/cost ratio.
-        
-        By resetting the random seed to a repeatable number for each test, tests can
-        create data based on random numbers and yet remain repeatable, for example
-        factory boy's fuzzy values. This is good for ensuring that tests specify the
-        data they need and that the tested system is not affected by any data that is
-        filled in randomly due to not being specified.
-        
-        I have written a `blog post covering the history of
-        pytest-randomly <https://adamj.eu/tech/2018/01/08/pytest-randomly-history/>`__,
-        including how it started life as the nose plugin
-        `nose-randomly <https://github.com/adamchainz/nose-randomly>`__.
-        
-        Additionally, I appeared on the Test and Code podcast to `talk about
-        pytest-randomly <https://testandcode.com/128>`__.
-        
-        Installation
-        ============
-        
-        Install from pip with:
-        
-        .. code-block:: bash
-        
-            python -m pip install pytest-randomly
-        
-        Python 3.6 to 3.10 supported.
-        
-        ----
-        
-        **Testing a Django project?**
-        Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
-        
-        ----
-        
-        Usage
-        =====
-        
-        Pytest will automatically find the plugin and use it when you run ``pytest``.
-        The output will start with an extra line that tells you the random seed that is
-        being used:
-        
-        .. code-block:: bash
-        
-            $ pytest
-            ...
-            platform darwin -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0
-            Using --randomly-seed=1553614239
-            ...
-        
-        If the tests fail due to ordering or randomly created data, you can restart
-        them with that seed using the flag as suggested:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=1234
-        
-        Or more conveniently, use the special value ``last``:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=last
-        
-        Since the ordering is by module, then by class, you can debug inter-test
-        pollution failures by narrowing down which tests are being run to find the bad
-        interaction by rerunning just the module/class:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=1234 tests/module_that_failed/
-        
-        You can disable behaviours you don't like with the following flags:
-        
-        * ``--randomly-dont-reset-seed`` - turn off the reset of ``random.seed()`` at
-          the start of every test
-        * ``--randomly-dont-reorganize`` - turn off the shuffling of the order of tests
-        
-        The plugin appears to Pytest with the name 'randomly'. To disable it
-        altogether, you can use the ``-p`` argument, for example:
-        
-        .. code-block:: sh
-        
-            pytest -p no:randomly
-        
-        Entry Point
-        ===========
-        
-        If you're using a different randomness generator in your third party package,
-        you can register an entrypoint to be called every time ``pytest-randomly``
-        reseeds. Implement the entrypoint ``pytest_randomly.random_seeder``, referring
-        to a function/callable that takes one argument, the new seed (int).
-        
-        For example in your ``setup.cfg``:
-        
-        .. code-block:: sh
-        
-            [options.entry_points]
-            pytest_randomly.random_seeder =
-                mypackage = mypackage.reseed
-        
-        Then implement ``reseed(new_seed)``.
-        
-        References
-        ==========
-        
-        .. [1] Sai Zhang, Darioush Jalali, Jochen Wuttke, Kıvanç Muşlu, Wing Lam, Michael D. Ernst, and David Notkin. 2014. Empirically revisiting the test independence assumption. In Proceedings of the 2014 International Symposium on Software Testing and Analysis (ISSTA 2014). Association for Computing Machinery, New York, NY, USA, 385–396. doi:https://doi.org/10.1145/2610384.2610404
-        
 Keywords: pytest,random,randomize,randomise,randomly
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -194,7 +20,184 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===============
+pytest-randomly
+===============
+
+.. image:: https://img.shields.io/github/workflow/status/pytest-dev/pytest-randomly/CI/main?style=for-the-badge
+   :target: https://github.com/pytest-dev/pytest-randomly/actions?workflow=CI
+
+.. image:: https://img.shields.io/pypi/v/pytest-randomly.svg?style=for-the-badge
+   :target: https://pypi.org/project/pytest-randomly/
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+   :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+
+.. figure:: https://raw.githubusercontent.com/pytest-dev/pytest-randomly/main/logo.png
+   :scale: 50%
+   :alt: Randomness power.
+
+Pytest plugin to randomly order tests and control ``random.seed``.
+
+Features
+========
+
+All of these features are on by default but can be disabled with flags.
+
+* Randomly shuffles the order of test items. This is done first at the level of
+  modules, then at the level of test classes (if you have them), then at the
+  order of functions. This also works with things like doctests.
+* Resets ``random.seed()`` at the start of every test case and test to a fixed
+  number - this defaults to ``time.time()`` from the start of your test run,
+  but you can pass in ``--randomly-seed`` to repeat a randomness-induced
+  failure.
+* If
+  `factory boy <https://factoryboy.readthedocs.io/en/latest/reference.html>`_
+  is installed, its random state is reset at the start of every test. This
+  allows for repeatable use of its random 'fuzzy' features.
+* If `faker <https://pypi.org/project/faker>`_ is installed, its random
+  state is reset at the start of every test. This is also for repeatable fuzzy
+  data in tests - factory boy uses faker for lots of data. This is also done
+  if you're using the ``faker`` pytest fixture, by defining the ``faker_seed``
+  fixture
+  (`docs <https://faker.readthedocs.io/en/master/pytest-fixtures.html#seeding-configuration>`__).
+* If `numpy <http://www.numpy.org/>`_ is installed, its random state is reset
+  at the start of every test.
+* If additional random generators are used, they can be registered under the
+  ``pytest_randomly.random_seeder``
+  `entry point <https://packaging.python.org/specifications/entry-points/>`_ and
+  will have their seed reset at the start of every test. Register a function
+  that takes the current seed value.
+* Works with `pytest-xdist <https://pypi.org/project/pytest-xdist/>`__.
+
+About
+=====
+
+Randomness in testing can be quite powerful to discover hidden flaws in the
+tests themselves, as well as giving a little more coverage to your system.
+
+By randomly ordering the tests, the risk of surprising inter-test dependencies
+is reduced - a technique used in many places, for example Google's C++ test
+runner `googletest
+<https://code.google.com/p/googletest/wiki/V1_5_AdvancedGuide#Shuffling_the_Tests>`_.
+Research suggests that "dependent tests do exist in practice" and a random
+order of test executions can effectively detect such dependencies [1]_.
+Alternatively, a reverse order of test executions, as provided by `pytest-reverse
+<https://github.com/adamchainz/pytest-reverse>`__, may find less dependent
+tests but can achieve a better benefit/cost ratio.
+
+By resetting the random seed to a repeatable number for each test, tests can
+create data based on random numbers and yet remain repeatable, for example
+factory boy's fuzzy values. This is good for ensuring that tests specify the
+data they need and that the tested system is not affected by any data that is
+filled in randomly due to not being specified.
+
+I have written a `blog post covering the history of
+pytest-randomly <https://adamj.eu/tech/2018/01/08/pytest-randomly-history/>`__,
+including how it started life as the nose plugin
+`nose-randomly <https://github.com/adamchainz/nose-randomly>`__.
+
+Additionally, I appeared on the Test and Code podcast to `talk about
+pytest-randomly <https://testandcode.com/128>`__.
+
+Installation
+============
+
+Install from pip with:
+
+.. code-block:: bash
+
+    python -m pip install pytest-randomly
+
+Python 3.6 to 3.10 supported.
+
+----
+
+**Testing a Django project?**
+Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
+
+----
+
+Usage
+=====
+
+Pytest will automatically find the plugin and use it when you run ``pytest``.
+The output will start with an extra line that tells you the random seed that is
+being used:
+
+.. code-block:: bash
+
+    $ pytest
+    ...
+    platform darwin -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0
+    Using --randomly-seed=1553614239
+    ...
+
+If the tests fail due to ordering or randomly created data, you can restart
+them with that seed using the flag as suggested:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=1234
+
+Or more conveniently, use the special value ``last``:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=last
+
+Since the ordering is by module, then by class, you can debug inter-test
+pollution failures by narrowing down which tests are being run to find the bad
+interaction by rerunning just the module/class:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=1234 tests/module_that_failed/
+
+You can disable behaviours you don't like with the following flags:
+
+* ``--randomly-dont-reset-seed`` - turn off the reset of ``random.seed()`` at
+  the start of every test
+* ``--randomly-dont-reorganize`` - turn off the shuffling of the order of tests
+
+The plugin appears to Pytest with the name 'randomly'. To disable it
+altogether, you can use the ``-p`` argument, for example:
+
+.. code-block:: sh
+
+    pytest -p no:randomly
+
+Entry Point
+===========
+
+If you're using a different randomness generator in your third party package,
+you can register an entrypoint to be called every time ``pytest-randomly``
+reseeds. Implement the entrypoint ``pytest_randomly.random_seeder``, referring
+to a function/callable that takes one argument, the new seed (int).
+
+For example in your ``setup.cfg``:
+
+.. code-block:: ini
+
+    [options.entry_points]
+    pytest_randomly.random_seeder =
+        mypackage = mypackage.reseed
+
+Then implement ``reseed(new_seed)``.
+
+References
+==========
+
+.. [1] Sai Zhang, Darioush Jalali, Jochen Wuttke, Kıvanç Muşlu, Wing Lam, Michael D. Ernst, and David Notkin. 2014. Empirically revisiting the test independence assumption. In Proceedings of the 2014 International Symposium on Software Testing and Analysis (ISSTA 2014). Association for Computing Machinery, New York, NY, USA, 385–396. doi:https://doi.org/10.1145/2610384.2610404
+
+
```

### Comparing `pytest-randomly-3.8.0/README.rst` & `pytest-randomly-3.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 If you're using a different randomness generator in your third party package,
 you can register an entrypoint to be called every time ``pytest-randomly``
 reseeds. Implement the entrypoint ``pytest_randomly.random_seeder``, referring
 to a function/callable that takes one argument, the new seed (int).
 
 For example in your ``setup.cfg``:
 
-.. code-block:: sh
+.. code-block:: ini
 
     [options.entry_points]
     pytest_randomly.random_seeder =
         mypackage = mypackage.reseed
 
 Then implement ``reseed(new_seed)``.
```

### Comparing `pytest-randomly-3.8.0/logo.png` & `pytest-randomly-3.9.0/logo.png`

 * *Files identical despite different names*

### Comparing `pytest-randomly-3.8.0/setup.cfg` & `pytest-randomly-3.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest-randomly
-version = 3.8.0
+version = 3.9.0
 description = Pytest plugin to randomly order tests and control random.seed.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/pytest-dev/pytest-randomly
 project_urls = 
@@ -26,22 +26,25 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 license_file = LICENSE
 
 [options]
 package_dir = 
 	=src
-py_modules = pytest_randomly
+packages = find:
 include_package_data = True
 install_requires = 
 	importlib-metadata >= 3.6.0 ; python_version < "3.10"
 	pytest
 python_requires = >=3.6
 zip_safe = False
 
+[options.packages.find]
+where = src
+
 [options.entry_points]
 pytest11 = 
 	randomly = pytest_randomly
 
 [flake8]
 max-line-length = 80
 select = E,F,W,B,B950,C,I
```

### Comparing `pytest-randomly-3.8.0/src/pytest_randomly.egg-info/PKG-INFO` & `pytest-randomly-3.9.0/src/pytest_randomly.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest-randomly
-Version: 3.8.0
+Version: 3.9.0
 Summary: Pytest plugin to randomly order tests and control random.seed.
 Home-page: https://github.com/pytest-dev/pytest-randomly
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/pytest-dev/pytest-randomly/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
-Description: ===============
-        pytest-randomly
-        ===============
-        
-        .. image:: https://img.shields.io/github/workflow/status/pytest-dev/pytest-randomly/CI/main?style=for-the-badge
-           :target: https://github.com/pytest-dev/pytest-randomly/actions?workflow=CI
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-randomly.svg?style=for-the-badge
-           :target: https://pypi.org/project/pytest-randomly/
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
-           :target: https://github.com/psf/black
-        
-        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
-           :target: https://github.com/pre-commit/pre-commit
-           :alt: pre-commit
-        
-        .. figure:: https://raw.githubusercontent.com/pytest-dev/pytest-randomly/main/logo.png
-           :scale: 50%
-           :alt: Randomness power.
-        
-        Pytest plugin to randomly order tests and control ``random.seed``.
-        
-        Features
-        ========
-        
-        All of these features are on by default but can be disabled with flags.
-        
-        * Randomly shuffles the order of test items. This is done first at the level of
-          modules, then at the level of test classes (if you have them), then at the
-          order of functions. This also works with things like doctests.
-        * Resets ``random.seed()`` at the start of every test case and test to a fixed
-          number - this defaults to ``time.time()`` from the start of your test run,
-          but you can pass in ``--randomly-seed`` to repeat a randomness-induced
-          failure.
-        * If
-          `factory boy <https://factoryboy.readthedocs.io/en/latest/reference.html>`_
-          is installed, its random state is reset at the start of every test. This
-          allows for repeatable use of its random 'fuzzy' features.
-        * If `faker <https://pypi.org/project/faker>`_ is installed, its random
-          state is reset at the start of every test. This is also for repeatable fuzzy
-          data in tests - factory boy uses faker for lots of data. This is also done
-          if you're using the ``faker`` pytest fixture, by defining the ``faker_seed``
-          fixture
-          (`docs <https://faker.readthedocs.io/en/master/pytest-fixtures.html#seeding-configuration>`__).
-        * If `numpy <http://www.numpy.org/>`_ is installed, its random state is reset
-          at the start of every test.
-        * If additional random generators are used, they can be registered under the
-          ``pytest_randomly.random_seeder``
-          `entry point <https://packaging.python.org/specifications/entry-points/>`_ and
-          will have their seed reset at the start of every test. Register a function
-          that takes the current seed value.
-        * Works with `pytest-xdist <https://pypi.org/project/pytest-xdist/>`__.
-        
-        About
-        =====
-        
-        Randomness in testing can be quite powerful to discover hidden flaws in the
-        tests themselves, as well as giving a little more coverage to your system.
-        
-        By randomly ordering the tests, the risk of surprising inter-test dependencies
-        is reduced - a technique used in many places, for example Google's C++ test
-        runner `googletest
-        <https://code.google.com/p/googletest/wiki/V1_5_AdvancedGuide#Shuffling_the_Tests>`_.
-        Research suggests that "dependent tests do exist in practice" and a random
-        order of test executions can effectively detect such dependencies [1]_.
-        Alternatively, a reverse order of test executions, as provided by `pytest-reverse
-        <https://github.com/adamchainz/pytest-reverse>`__, may find less dependent
-        tests but can achieve a better benefit/cost ratio.
-        
-        By resetting the random seed to a repeatable number for each test, tests can
-        create data based on random numbers and yet remain repeatable, for example
-        factory boy's fuzzy values. This is good for ensuring that tests specify the
-        data they need and that the tested system is not affected by any data that is
-        filled in randomly due to not being specified.
-        
-        I have written a `blog post covering the history of
-        pytest-randomly <https://adamj.eu/tech/2018/01/08/pytest-randomly-history/>`__,
-        including how it started life as the nose plugin
-        `nose-randomly <https://github.com/adamchainz/nose-randomly>`__.
-        
-        Additionally, I appeared on the Test and Code podcast to `talk about
-        pytest-randomly <https://testandcode.com/128>`__.
-        
-        Installation
-        ============
-        
-        Install from pip with:
-        
-        .. code-block:: bash
-        
-            python -m pip install pytest-randomly
-        
-        Python 3.6 to 3.10 supported.
-        
-        ----
-        
-        **Testing a Django project?**
-        Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
-        
-        ----
-        
-        Usage
-        =====
-        
-        Pytest will automatically find the plugin and use it when you run ``pytest``.
-        The output will start with an extra line that tells you the random seed that is
-        being used:
-        
-        .. code-block:: bash
-        
-            $ pytest
-            ...
-            platform darwin -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0
-            Using --randomly-seed=1553614239
-            ...
-        
-        If the tests fail due to ordering or randomly created data, you can restart
-        them with that seed using the flag as suggested:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=1234
-        
-        Or more conveniently, use the special value ``last``:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=last
-        
-        Since the ordering is by module, then by class, you can debug inter-test
-        pollution failures by narrowing down which tests are being run to find the bad
-        interaction by rerunning just the module/class:
-        
-        .. code-block:: bash
-        
-            pytest --randomly-seed=1234 tests/module_that_failed/
-        
-        You can disable behaviours you don't like with the following flags:
-        
-        * ``--randomly-dont-reset-seed`` - turn off the reset of ``random.seed()`` at
-          the start of every test
-        * ``--randomly-dont-reorganize`` - turn off the shuffling of the order of tests
-        
-        The plugin appears to Pytest with the name 'randomly'. To disable it
-        altogether, you can use the ``-p`` argument, for example:
-        
-        .. code-block:: sh
-        
-            pytest -p no:randomly
-        
-        Entry Point
-        ===========
-        
-        If you're using a different randomness generator in your third party package,
-        you can register an entrypoint to be called every time ``pytest-randomly``
-        reseeds. Implement the entrypoint ``pytest_randomly.random_seeder``, referring
-        to a function/callable that takes one argument, the new seed (int).
-        
-        For example in your ``setup.cfg``:
-        
-        .. code-block:: sh
-        
-            [options.entry_points]
-            pytest_randomly.random_seeder =
-                mypackage = mypackage.reseed
-        
-        Then implement ``reseed(new_seed)``.
-        
-        References
-        ==========
-        
-        .. [1] Sai Zhang, Darioush Jalali, Jochen Wuttke, Kıvanç Muşlu, Wing Lam, Michael D. Ernst, and David Notkin. 2014. Empirically revisiting the test independence assumption. In Proceedings of the 2014 International Symposium on Software Testing and Analysis (ISSTA 2014). Association for Computing Machinery, New York, NY, USA, 385–396. doi:https://doi.org/10.1145/2610384.2610404
-        
 Keywords: pytest,random,randomize,randomise,randomly
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -194,7 +20,184 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===============
+pytest-randomly
+===============
+
+.. image:: https://img.shields.io/github/workflow/status/pytest-dev/pytest-randomly/CI/main?style=for-the-badge
+   :target: https://github.com/pytest-dev/pytest-randomly/actions?workflow=CI
+
+.. image:: https://img.shields.io/pypi/v/pytest-randomly.svg?style=for-the-badge
+   :target: https://pypi.org/project/pytest-randomly/
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+   :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+
+.. figure:: https://raw.githubusercontent.com/pytest-dev/pytest-randomly/main/logo.png
+   :scale: 50%
+   :alt: Randomness power.
+
+Pytest plugin to randomly order tests and control ``random.seed``.
+
+Features
+========
+
+All of these features are on by default but can be disabled with flags.
+
+* Randomly shuffles the order of test items. This is done first at the level of
+  modules, then at the level of test classes (if you have them), then at the
+  order of functions. This also works with things like doctests.
+* Resets ``random.seed()`` at the start of every test case and test to a fixed
+  number - this defaults to ``time.time()`` from the start of your test run,
+  but you can pass in ``--randomly-seed`` to repeat a randomness-induced
+  failure.
+* If
+  `factory boy <https://factoryboy.readthedocs.io/en/latest/reference.html>`_
+  is installed, its random state is reset at the start of every test. This
+  allows for repeatable use of its random 'fuzzy' features.
+* If `faker <https://pypi.org/project/faker>`_ is installed, its random
+  state is reset at the start of every test. This is also for repeatable fuzzy
+  data in tests - factory boy uses faker for lots of data. This is also done
+  if you're using the ``faker`` pytest fixture, by defining the ``faker_seed``
+  fixture
+  (`docs <https://faker.readthedocs.io/en/master/pytest-fixtures.html#seeding-configuration>`__).
+* If `numpy <http://www.numpy.org/>`_ is installed, its random state is reset
+  at the start of every test.
+* If additional random generators are used, they can be registered under the
+  ``pytest_randomly.random_seeder``
+  `entry point <https://packaging.python.org/specifications/entry-points/>`_ and
+  will have their seed reset at the start of every test. Register a function
+  that takes the current seed value.
+* Works with `pytest-xdist <https://pypi.org/project/pytest-xdist/>`__.
+
+About
+=====
+
+Randomness in testing can be quite powerful to discover hidden flaws in the
+tests themselves, as well as giving a little more coverage to your system.
+
+By randomly ordering the tests, the risk of surprising inter-test dependencies
+is reduced - a technique used in many places, for example Google's C++ test
+runner `googletest
+<https://code.google.com/p/googletest/wiki/V1_5_AdvancedGuide#Shuffling_the_Tests>`_.
+Research suggests that "dependent tests do exist in practice" and a random
+order of test executions can effectively detect such dependencies [1]_.
+Alternatively, a reverse order of test executions, as provided by `pytest-reverse
+<https://github.com/adamchainz/pytest-reverse>`__, may find less dependent
+tests but can achieve a better benefit/cost ratio.
+
+By resetting the random seed to a repeatable number for each test, tests can
+create data based on random numbers and yet remain repeatable, for example
+factory boy's fuzzy values. This is good for ensuring that tests specify the
+data they need and that the tested system is not affected by any data that is
+filled in randomly due to not being specified.
+
+I have written a `blog post covering the history of
+pytest-randomly <https://adamj.eu/tech/2018/01/08/pytest-randomly-history/>`__,
+including how it started life as the nose plugin
+`nose-randomly <https://github.com/adamchainz/nose-randomly>`__.
+
+Additionally, I appeared on the Test and Code podcast to `talk about
+pytest-randomly <https://testandcode.com/128>`__.
+
+Installation
+============
+
+Install from pip with:
+
+.. code-block:: bash
+
+    python -m pip install pytest-randomly
+
+Python 3.6 to 3.10 supported.
+
+----
+
+**Testing a Django project?**
+Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
+
+----
+
+Usage
+=====
+
+Pytest will automatically find the plugin and use it when you run ``pytest``.
+The output will start with an extra line that tells you the random seed that is
+being used:
+
+.. code-block:: bash
+
+    $ pytest
+    ...
+    platform darwin -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0
+    Using --randomly-seed=1553614239
+    ...
+
+If the tests fail due to ordering or randomly created data, you can restart
+them with that seed using the flag as suggested:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=1234
+
+Or more conveniently, use the special value ``last``:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=last
+
+Since the ordering is by module, then by class, you can debug inter-test
+pollution failures by narrowing down which tests are being run to find the bad
+interaction by rerunning just the module/class:
+
+.. code-block:: bash
+
+    pytest --randomly-seed=1234 tests/module_that_failed/
+
+You can disable behaviours you don't like with the following flags:
+
+* ``--randomly-dont-reset-seed`` - turn off the reset of ``random.seed()`` at
+  the start of every test
+* ``--randomly-dont-reorganize`` - turn off the shuffling of the order of tests
+
+The plugin appears to Pytest with the name 'randomly'. To disable it
+altogether, you can use the ``-p`` argument, for example:
+
+.. code-block:: sh
+
+    pytest -p no:randomly
+
+Entry Point
+===========
+
+If you're using a different randomness generator in your third party package,
+you can register an entrypoint to be called every time ``pytest-randomly``
+reseeds. Implement the entrypoint ``pytest_randomly.random_seeder``, referring
+to a function/callable that takes one argument, the new seed (int).
+
+For example in your ``setup.cfg``:
+
+.. code-block:: ini
+
+    [options.entry_points]
+    pytest_randomly.random_seeder =
+        mypackage = mypackage.reseed
+
+Then implement ``reseed(new_seed)``.
+
+References
+==========
+
+.. [1] Sai Zhang, Darioush Jalali, Jochen Wuttke, Kıvanç Muşlu, Wing Lam, Michael D. Ernst, and David Notkin. 2014. Empirically revisiting the test independence assumption. In Proceedings of the 2014 International Symposium on Software Testing and Analysis (ISSTA 2014). Association for Computing Machinery, New York, NY, USA, 385–396. doi:https://doi.org/10.1145/2610384.2610404
+
+
```

### Comparing `pytest-randomly-3.8.0/src/pytest_randomly.py` & `pytest-randomly-3.9.0/src/pytest_randomly/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import argparse
 import hashlib
 import random
 import sys
+from types import ModuleType
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
 
+from _pytest.config import Config
+from _pytest.config.argparsing import Parser
+from _pytest.nodes import Item
 from pytest import Collector, fixture
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
@@ -45,26 +50,26 @@
 except ImportError:
     have_numpy = False
 
 
 default_seed = random.Random().getrandbits(32)
 
 
-def seed_type(string):
+def seed_type(string: str) -> Union[str, int]:
     if string in ("default", "last"):
         return string
     try:
         return int(string)
     except ValueError:
         raise argparse.ArgumentTypeError(
-            "{} is not an integer or the string 'last'".format(repr(string))
+            f"{repr(string)} is not an integer or the string 'last'"
         )
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("randomly", "Randomizes tests")
     group._addoption(
         "--randomly-seed",
         action="store",
         dest="randomly_seed",
         default="default",
         type=seed_type,
@@ -87,49 +92,52 @@
         action="store_false",
         dest="randomly_reorganize",
         default=True,
         help="Stop pytest-randomly from randomly reorganizing the test order.",
     )
 
 
-def pytest_configure(config):
+def pytest_configure(config: Config) -> None:
     if config.pluginmanager.hasplugin("xdist"):
         config.pluginmanager.register(XdistHooks())
 
     seed_value = config.getoption("randomly_seed")
     if seed_value == "last":
+        assert config.cache is not None
         seed = config.cache.get("randomly_seed", default_seed)
     elif seed_value == "default":
         if hasattr(config, "workerinput"):
             # pytest-xdist: use seed generated on main.
-            seed = config.workerinput["randomly_seed"]
+            seed = config.workerinput["randomly_seed"]  # type: ignore [attr-defined]
         else:
             seed = default_seed
     else:
         seed = seed_value
+    assert config.cache is not None
     config.cache.set("randomly_seed", seed)
     config.option.randomly_seed = seed
 
 
 class XdistHooks:
     # Hooks for xdist only, registered when needed in pytest_configure()
     # https://docs.pytest.org/en/latest/writing_plugins.html#optionally-using-hooks-from-3rd-party-plugins  # noqa: B950
 
-    def pytest_configure_node(self, node):
-        node.workerinput["randomly_seed"] = node.config.getoption("randomly_seed")
+    def pytest_configure_node(self, node: Item) -> None:
+        seed = node.config.getoption("randomly_seed")
+        node.workerinput["randomly_seed"] = seed  # type: ignore [attr-defined]
 
 
-random_states = {}
-np_random_states = {}
+random_states: Dict[int, object] = {}
+np_random_states: Dict[int, Any] = {}
 
 
-entrypoint_reseeds = None
+entrypoint_reseeds: Optional[List[Callable[[int], None]]] = None
 
 
-def _reseed(config, offset=0):
+def _reseed(config: Config, offset: int = 0) -> None:
     global entrypoint_reseeds
     seed = config.getoption("randomly_seed") + offset
     if seed not in random_states:
         random.seed(seed)
         random_states[seed] = random.getstate()
     else:
         random.setstate(random_states[seed])
@@ -152,54 +160,53 @@
         entrypoint_reseeds = [
             e.load() for e in entry_points(group="pytest_randomly.random_seeder")
         ]
     for reseed in entrypoint_reseeds:
         reseed(seed)
 
 
-def _truncate_seed_for_numpy(seed):
+def _truncate_seed_for_numpy(seed: int) -> int:
     seed = abs(seed)
     if seed <= 2 ** 32 - 1:
         return seed
 
     seed_bytes = seed.to_bytes(seed.bit_length(), "big")
     return int.from_bytes(hashlib.sha512(seed_bytes).digest()[: 32 // 8], "big")
 
 
-def pytest_report_header(config):
+def pytest_report_header(config: Config) -> str:
     seed = config.getoption("randomly_seed")
     _reseed(config)
-    return "Using --randomly-seed={}".format(seed)
+    return f"Using --randomly-seed={seed}"
 
 
-def pytest_runtest_setup(item):
+def pytest_runtest_setup(item: Item) -> None:
     if item.config.getoption("randomly_reset_seed"):
         _reseed(item.config, -1)
 
 
-def pytest_runtest_call(item):
+def pytest_runtest_call(item: Item) -> None:
     if item.config.getoption("randomly_reset_seed"):
         _reseed(item.config)
 
 
-def pytest_runtest_teardown(item):
+def pytest_runtest_teardown(item: Item) -> None:
     if item.config.getoption("randomly_reset_seed"):
         _reseed(item.config, 1)
 
 
-def pytest_collection_modifyitems(config, items):
+def pytest_collection_modifyitems(config: Config, items: List[Item]) -> None:
     if not config.getoption("randomly_reorganize"):
         return
 
     _reseed(config)
 
-    module_items = []
-
-    current_module = None
-    current_items = []
+    module_items: List[List[Item]] = []
+    current_module: Optional[ModuleType] = None
+    current_items: List[Item] = []
     for item in items:
 
         try:
             item_module = getattr(item, "module", None)
         except (ImportError, Collector.CollectError):
             item_module = None
 
@@ -215,44 +222,47 @@
     module_items.append(shuffle_by_class(current_items))
 
     random.shuffle(module_items)
 
     items[:] = reduce_list_of_lists(module_items)
 
 
-def shuffle_by_class(items):
-    class_items = []
-    current_cls = None
-    current_items = []
+def shuffle_by_class(items: List[Item]) -> List[Item]:
+    class_items: List[List[Item]] = []
+    current_cls: Optional[Type[Any]] = None
+    current_items: List[Item] = []
 
     for item in items:
         if current_cls is None:
             current_cls = getattr(item, "cls", None)
 
         if getattr(item, "cls", None) != current_cls:
             random.shuffle(current_items)
             class_items.append(current_items)
             current_items = [item]
-            current_cls = item.cls
+            current_cls = item.cls  # type: ignore [attr-defined]
         else:
             current_items.append(item)
 
     random.shuffle(current_items)
     class_items.append(current_items)
 
     random.shuffle(class_items)
 
     return reduce_list_of_lists(class_items)
 
 
-def reduce_list_of_lists(lists):
+T = TypeVar("T")
+
+
+def reduce_list_of_lists(lists: List[List[T]]) -> List[T]:
     new_list = []
     for list_ in lists:
         new_list.extend(list_)
     return new_list
 
 
 if have_faker:
 
     @fixture(autouse=True)
-    def faker_seed(pytestconfig):
+    def faker_seed(pytestconfig: Config) -> None:
         return pytestconfig.getoption("randomly_seed")
```

