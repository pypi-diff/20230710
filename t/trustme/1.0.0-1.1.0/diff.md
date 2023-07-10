# Comparing `tmp/trustme-1.0.0.tar.gz` & `tmp/trustme-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustme-1.0.0.tar", last modified: Mon May  1 06:16:17 2023, max compression
+gzip compressed data, was "trustme-1.1.0.tar", last modified: Mon Jul 10 06:51:13 2023, max compression
```

## Comparing `trustme-1.0.0.tar` & `trustme-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.662828 trustme-1.0.0/
--rw-r--r--   0 q         (1000) q         (1000)      118 2021-10-04 05:59:43.000000 trustme-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 q         (1000) q         (1000)      185 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE
--rw-r--r--   0 q         (1000) q         (1000)    11358 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE.APACHE2
--rw-r--r--   0 q         (1000) q         (1000)     1046 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE.MIT
--rw-r--r--   0 q         (1000) q         (1000)      180 2021-10-04 05:59:43.000000 trustme-1.0.0/MANIFEST.in
--rw-r--r--   0 q         (1000) q         (1000)     5581 2023-05-01 06:16:17.661828 trustme-1.0.0/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)     4385 2022-06-07 05:49:38.000000 trustme-1.0.0/README.rst
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/
--rw-r--r--   0 q         (1000) q         (1000)      611 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/Makefile
--rw-r--r--   0 q         (1000) q         (1000)      809 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/make.bat
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/_static/
--rw-r--r--   0 q         (1000) q         (1000)        0 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/source/_static/.gitkeep
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/_templates/
--rw-r--r--   0 q         (1000) q         (1000)      212 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/source/_templates/need-help.html
--rw-r--r--   0 q         (1000) q         (1000)     5333 2022-06-07 05:49:38.000000 trustme-1.0.0/docs/source/conf.py
--rw-r--r--   0 q         (1000) q         (1000)     9184 2023-05-01 06:09:23.000000 trustme-1.0.0/docs/source/index.rst
--rw-r--r--   0 q         (1000) q         (1000)     2357 2022-06-07 05:49:38.000000 trustme-1.0.0/docs/source/trustme-trio-example.py
--rw-r--r--   0 q         (1000) q         (1000)     1605 2023-04-24 05:34:31.000000 trustme-1.0.0/pyproject.toml
--rw-r--r--   0 q         (1000) q         (1000)       38 2023-05-01 06:16:17.662828 trustme-1.0.0/setup.cfg
--rw-r--r--   0 q         (1000) q         (1000)     1538 2023-05-01 06:01:58.000000 trustme-1.0.0/setup.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.657828 trustme-1.0.0/src/
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.660828 trustme-1.0.0/src/trustme/
--rw-r--r--   0 q         (1000) q         (1000)    19643 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/__init__.py
--rw-r--r--   0 q         (1000) q         (1000)       31 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/__main__.py
--rw-r--r--   0 q         (1000) q         (1000)     3072 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/_cli.py
--rw-r--r--   0 q         (1000) q         (1000)       22 2023-05-01 06:01:58.000000 trustme-1.0.0/src/trustme/_version.py
--rw-r--r--   0 q         (1000) q         (1000)        0 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/py.typed
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.661828 trustme-1.0.0/src/trustme.egg-info/
--rw-r--r--   0 q         (1000) q         (1000)     5581 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)      623 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/SOURCES.txt
--rw-r--r--   0 q         (1000) q         (1000)        1 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/dependency_links.txt
--rw-r--r--   0 q         (1000) q         (1000)       28 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/requires.txt
--rw-r--r--   0 q         (1000) q         (1000)        8 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/top_level.txt
--rw-r--r--   0 q         (1000) q         (1000)      863 2023-04-24 05:35:28.000000 trustme-1.0.0/test-requirements.txt
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.661828 trustme-1.0.0/tests/
--rw-r--r--   0 q         (1000) q         (1000)     3253 2023-04-17 10:20:58.000000 trustme-1.0.0/tests/test_cli.py
--rw-r--r--   0 q         (1000) q         (1000)    16905 2023-04-24 05:34:31.000000 trustme-1.0.0/tests/test_trustme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.035565 trustme-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 06:51:02.000000 trustme-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 06:51:02.000000 trustme-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 06:51:02.000000 trustme-1.1.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 06:51:02.000000 trustme-1.1.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 06:51:02.000000 trustme-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-07-10 06:51:13.035565 trustme-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-10 06:51:02.000000 trustme-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.031565 trustme-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.031565 trustme-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.031565 trustme-1.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.031565 trustme-1.1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/source/_templates/need-help.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-10 06:51:02.000000 trustme-1.1.0/docs/source/trustme-trio-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-10 06:51:02.000000 trustme-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:51:13.035565 trustme-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-10 06:51:02.000000 trustme-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.031565 trustme-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.035565 trustme-1.1.0/src/trustme/
+-rw-r--r--   0 runner    (1001) docker     (123)    19513 2023-07-10 06:51:02.000000 trustme-1.1.0/src/trustme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 06:51:02.000000 trustme-1.1.0/src/trustme/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-10 06:51:02.000000 trustme-1.1.0/src/trustme/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 06:51:02.000000 trustme-1.1.0/src/trustme/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:02.000000 trustme-1.1.0/src/trustme/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.035565 trustme-1.1.0/src/trustme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-07-10 06:51:13.000000 trustme-1.1.0/src/trustme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-10 06:51:13.000000 trustme-1.1.0/src/trustme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:51:13.000000 trustme-1.1.0/src/trustme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 06:51:13.000000 trustme-1.1.0/src/trustme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 06:51:13.000000 trustme-1.1.0/src/trustme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 06:51:02.000000 trustme-1.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:51:13.035565 trustme-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-10 06:51:02.000000 trustme-1.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-07-10 06:51:02.000000 trustme-1.1.0/tests/test_trustme.py
```

### Comparing `trustme-1.0.0/LICENSE.APACHE2` & `trustme-1.1.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/LICENSE.MIT` & `trustme-1.1.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/PKG-INFO` & `trustme-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: trustme
-Version: 1.0.0
+Version: 1.1.0
 Summary: #1 quality TLS certs while you wait, for the discerning tester
 Home-page: https://github.com/python-trio/trustme
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
 License: MIT OR Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: LICENSE.APACHE2
 License-File: LICENSE.MIT
 
 .. note that this README gets 'include'ed into the main documentation
 
 ==============================================
@@ -58,15 +58,15 @@
 
 **Install:** ``pip install -U trustme``
 
 **Documentation:** https://trustme.readthedocs.io
 
 **Bug tracker and source code:** https://github.com/python-trio/trustme
 
-**Tested on:** Python 3.7+, CPython and PyPy
+**Tested on:** Python 3.8+, CPython and PyPy
 
 **License:** MIT or Apache 2, your choice.
 
 **Code of conduct:** Contributors are requested to follow our `code of
 conduct
 <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
 in all project spaces.
@@ -84,36 +84,36 @@
    # ----- Creating certs -----
 
    # Look, you just created your certificate authority!
    ca = trustme.CA()
 
    # And now you issued a cert signed by this fake CA
    # https://en.wikipedia.org/wiki/Example.org
-   server_cert = ca.issue_cert(u"test-host.example.org")
+   server_cert = ca.issue_cert("test-host.example.org")
 
    # That's it!
 
    # ----- Using your shiny new certs -----
 
    # You can configure SSL context objects to trust this CA:
    ca.configure_trust(ssl_context)
    # Or configure them to present the server certificate
    server_cert.configure_cert(ssl_context)
    # You can use standard library or PyOpenSSL context objects here,
    # trustme is happy either way.
 
    # ----- or -----
-                
+
    # Save the PEM-encoded data to a file to use in non-Python test
    # suites:
    ca.cert_pem.write_to_path("ca.pem")
    server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
-   
+
    # ----- or -----
-                
+
    # Put the PEM-encoded data in a temporary file, for libraries that
    # insist on that:
    with ca.cert_pem.tempfile() as ca_temp_path:
        requests.get("https://...", verify=ca_temp_path)
 
 Command line usage:
```

### Comparing `trustme-1.0.0/README.rst` & `trustme-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 **Install:** ``pip install -U trustme``
 
 **Documentation:** https://trustme.readthedocs.io
 
 **Bug tracker and source code:** https://github.com/python-trio/trustme
 
-**Tested on:** Python 3.7+, CPython and PyPy
+**Tested on:** Python 3.8+, CPython and PyPy
 
 **License:** MIT or Apache 2, your choice.
 
 **Code of conduct:** Contributors are requested to follow our `code of
 conduct
 <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
 in all project spaces.
@@ -55,36 +55,36 @@
    # ----- Creating certs -----
 
    # Look, you just created your certificate authority!
    ca = trustme.CA()
 
    # And now you issued a cert signed by this fake CA
    # https://en.wikipedia.org/wiki/Example.org
-   server_cert = ca.issue_cert(u"test-host.example.org")
+   server_cert = ca.issue_cert("test-host.example.org")
 
    # That's it!
 
    # ----- Using your shiny new certs -----
 
    # You can configure SSL context objects to trust this CA:
    ca.configure_trust(ssl_context)
    # Or configure them to present the server certificate
    server_cert.configure_cert(ssl_context)
    # You can use standard library or PyOpenSSL context objects here,
    # trustme is happy either way.
 
    # ----- or -----
-                
+
    # Save the PEM-encoded data to a file to use in non-Python test
    # suites:
    ca.cert_pem.write_to_path("ca.pem")
    server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
-   
+
    # ----- or -----
-                
+
    # Put the PEM-encoded data in a temporary file, for libraries that
    # insist on that:
    with ca.cert_pem.tempfile() as ca_temp_path:
        requests.get("https://...", verify=ca_temp_path)
 
 Command line usage:
```

### Comparing `trustme-1.0.0/docs/Makefile` & `trustme-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/docs/make.bat` & `trustme-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/docs/source/conf.py` & `trustme-1.1.0/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     "python": ('https://docs.python.org/3', None),
     # https://github.com/pyca/pyopenssl/issues/1046
     "pyopenssl": ('https://www.pyopenssl.org/en/20.0.1/', None),
     "trio": ('https://trio.readthedocs.io/en/latest/', None),
 }
 
 autodoc_member_order = "bysource"
+autodoc_typehints = "both"
+autodoc_typehints_description_target = "documented"
 
 # Tell sphinx to treat bare backticks like `foo` as :py:obj:`foo`
 default_role = 'py:obj'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
```

### Comparing `trustme-1.0.0/docs/source/index.rst` & `trustme-1.1.0/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ====================
 
 Here's a fully working example you can run to see how :mod:`trustme`
 works. It demonstrates a simple TLS server and client that connect to
 each other using :mod:`trustme`\-generated certs.
 
 This example requires `Trio <https://trio.readthedocs.io>`__ (``pip
-install -U trio``) and Python 3.7+. Note that while :mod:`trustme` is
+install -U trio``) and Python 3.8+. Note that while :mod:`trustme` is
 maintained by the Trio project, :mod:`trustme` is happy to work with
 any networking library.
 
 The key lines are the calls to :meth:`~CA.configure_trust`,
 :meth:`~LeafCert.configure_cert` – try commenting them out one at a
 time to see what happens! Also notice that the hostname
 ``test-host.example.org`` appears twice – try changing one of the
@@ -118,14 +118,30 @@
    :undoc-members:
 
 Change history
 ==============
 
 .. towncrier release notes start
 
+Trustme 1.1.0 (2023-07-10)
+--------------------------
+
+Features
+~~~~~~~~
+
+- Allow `os.PathLike` in typing of `Blob.write_to_path`. (`#606 <https://github.com/python-trio/trustme/issues/606>`__)
+- Add support for PyPy 3.10 and Python 3.12. (`#609 <https://github.com/python-trio/trustme/issues/609>`__)
+
+
+Deprecations and Removals
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Remove support for Python 3.7. (`#609 <https://github.com/python-trio/trustme/issues/609>`__)
+
+
 Trustme 1.0.0 (2023-04-24)
 ------------------------------
 
 Features
 ~~~~~~~~
 
 - Support for ECDSA keys in certificates and use them by default. The type of key used for certificates can be controlled by the ``key_type`` parameter on the multiple methods that generate certificates. ECDSA certificates as they can be generated significantly faster. (`#559 <https://github.com/python-trio/trustme/issues/559>`__)
```

### Comparing `trustme-1.0.0/docs/source/trustme-trio-example.py` & `trustme-1.1.0/docs/source/trustme-trio-example.py`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/pyproject.toml` & `trustme-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/setup.py` & `trustme-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,30 @@
     license="MIT OR Apache-2.0",
     packages=find_packages(where="src"),
     package_data={
         'trustme': ['py.typed'],
     },
     package_dir={'': 'src'},
     url="https://github.com/python-trio/trustme",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "cryptography>=3.1",
         "idna>=2.0",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: System :: Networking",
         "Topic :: Security :: Cryptography",
         "Topic :: Software Development :: Testing",
     ])
```

### Comparing `trustme-1.0.0/src/trustme/__init__.py` & `trustme-1.1.0/src/trustme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,20 +142,20 @@
 
     def bytes(self) -> bytes:
         """Returns the data as a `bytes` object.
 
         """
         return self._data
 
-    def write_to_path(self, path: str, append: bool = False) -> None:
+    def write_to_path(self, path: Union[str, "os.PathLike[str]"], append: bool = False) -> None:
         """Writes the data to the file at the given path.
 
         Args:
-          path (str): The path to write to.
-          append (bool): If False (the default), replace any existing file
+          path: The path to write to.
+          append: If False (the default), replace any existing file
                with the given name. If True, append to any existing file.
 
         """
         if append:
             mode = "ab"
         else:
             mode = "wb"
@@ -182,15 +182,15 @@
           <http://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification>`__)::
 
            ca = trustme.CA()
            with ca.cert_pem.tempfile() as ca_cert_path:
                requests.get("https://localhost/...", verify=ca_cert_path)
 
         Args:
-          dir (str or None): Passed to `tempfile.NamedTemporaryFile`.
+          dir: Passed to `tempfile.NamedTemporaryFile`.
 
         """
         # On Windows, you can't re-open a NamedTemporaryFile that's still
         # open. Which seems like it completely defeats the purpose of having a
         # NamedTemporaryFile? Oh well...
         # https://bugs.python.org/issue14243
         f = NamedTemporaryFile(suffix=".pem", dir=dir, delete=False)
@@ -225,15 +225,15 @@
 
 class CA:
     """A certificate authority."""
     _certificate: x509.Certificate
 
     def __init__(
         self,
-        parent_cert: Optional["CA"] = None,
+        parent_cert: Optional[CA] = None,
         path_length: int = 9,
         organization_name: Optional[str] = None,
         organization_unit_name: Optional[str] = None,
         key_type: KeyType = KeyType.ECDSA,
     ) -> None:
         self.parent_cert = parent_cert
         self._private_key = key_type._generate_key()
@@ -438,21 +438,20 @@
                 cert.public_bytes(Encoding.PEM),
                 chain_to_ca,
             )
 
     # For backwards compatibility
     issue_server_cert = issue_cert
 
-    def configure_trust(self, ctx: Union[ssl.SSLContext, "OpenSSL.SSL.Context"]) -> None:
+    def configure_trust(self, ctx: Union[ssl.SSLContext, OpenSSL.SSL.Context]) -> None:
         """Configure the given context object to trust certificates signed by
         this CA.
 
         Args:
-          ctx (ssl.SSLContext or OpenSSL.SSL.Context): The SSL context to be
-              modified.
+          ctx: The SSL context to be modified.
 
         """
         if isinstance(ctx, ssl.SSLContext):
             ctx.load_verify_locations(
                 cadata=self.cert_pem.bytes().decode("ascii"))
         elif _smells_like_pyopenssl(ctx):
             from OpenSSL import crypto
@@ -469,16 +468,16 @@
     def from_pem(cls, cert_bytes: bytes, private_key_bytes: bytes) -> "CA":
         """Build a CA from existing cert and private key.
 
         This is useful if your test suite has an existing certificate authority and
         you're not ready to switch completely to trustme just yet.
 
         Args:
-          cert_bytes (bytes): The bytes of the certificate in PEM format
-          private_key_bytes (bytes): The bytes of the private key in PEM format
+          cert_bytes: The bytes of the certificate in PEM format
+          private_key_bytes: The bytes of the private key in PEM format
         """
         ca = cls()
         ca.parent_cert = None
         ca._certificate = x509.load_pem_x509_certificate(cert_bytes)
         ca._private_key = load_pem_private_key(private_key_bytes, password=None)  # type: ignore[assignment]
 
         return ca
@@ -506,20 +505,19 @@
     def __init__(self, private_key_pem: bytes, server_cert_pem: bytes, chain_to_ca: List[bytes]) -> None:
         self.private_key_pem = Blob(private_key_pem)
         self.cert_chain_pems = [
             Blob(pem) for pem in [server_cert_pem] + chain_to_ca]
         self.private_key_and_cert_chain_pem = (
             Blob(private_key_pem + server_cert_pem + b''.join(chain_to_ca)))
 
-    def configure_cert(self, ctx: Union[ssl.SSLContext, "OpenSSL.SSL.Context"]) -> None:
+    def configure_cert(self, ctx: Union[ssl.SSLContext, OpenSSL.SSL.Context]) -> None:
         """Configure the given context object to present this certificate.
 
         Args:
-          ctx (ssl.SSLContext or OpenSSL.SSL.Context): The SSL context to be
-              modified.
+          ctx: The SSL context to be modified.
 
         """
         if isinstance(ctx, ssl.SSLContext):
             # Currently need a temporary file for this, see:
             #   https://bugs.python.org/issue16487
             with self.private_key_and_cert_chain_pem.tempfile() as path:
                 ctx.load_cert_chain(path)
```

### Comparing `trustme-1.0.0/src/trustme/_cli.py` & `trustme-1.1.0/src/trustme/_cli.py`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/src/trustme.egg-info/PKG-INFO` & `trustme-1.1.0/src/trustme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: trustme
-Version: 1.0.0
+Version: 1.1.0
 Summary: #1 quality TLS certs while you wait, for the discerning tester
 Home-page: https://github.com/python-trio/trustme
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
 License: MIT OR Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: LICENSE.APACHE2
 License-File: LICENSE.MIT
 
 .. note that this README gets 'include'ed into the main documentation
 
 ==============================================
@@ -58,15 +58,15 @@
 
 **Install:** ``pip install -U trustme``
 
 **Documentation:** https://trustme.readthedocs.io
 
 **Bug tracker and source code:** https://github.com/python-trio/trustme
 
-**Tested on:** Python 3.7+, CPython and PyPy
+**Tested on:** Python 3.8+, CPython and PyPy
 
 **License:** MIT or Apache 2, your choice.
 
 **Code of conduct:** Contributors are requested to follow our `code of
 conduct
 <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
 in all project spaces.
@@ -84,36 +84,36 @@
    # ----- Creating certs -----
 
    # Look, you just created your certificate authority!
    ca = trustme.CA()
 
    # And now you issued a cert signed by this fake CA
    # https://en.wikipedia.org/wiki/Example.org
-   server_cert = ca.issue_cert(u"test-host.example.org")
+   server_cert = ca.issue_cert("test-host.example.org")
 
    # That's it!
 
    # ----- Using your shiny new certs -----
 
    # You can configure SSL context objects to trust this CA:
    ca.configure_trust(ssl_context)
    # Or configure them to present the server certificate
    server_cert.configure_cert(ssl_context)
    # You can use standard library or PyOpenSSL context objects here,
    # trustme is happy either way.
 
    # ----- or -----
-                
+
    # Save the PEM-encoded data to a file to use in non-Python test
    # suites:
    ca.cert_pem.write_to_path("ca.pem")
    server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
-   
+
    # ----- or -----
-                
+
    # Put the PEM-encoded data in a temporary file, for libraries that
    # insist on that:
    with ca.cert_pem.tempfile() as ca_temp_path:
        requests.get("https://...", verify=ca_temp_path)
 
 Command line usage:
```

### Comparing `trustme-1.0.0/src/trustme.egg-info/SOURCES.txt` & `trustme-1.1.0/src/trustme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/test-requirements.txt` & `trustme-1.1.0/test-requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile test-requirements.in
+#    pip-compile --resolver=backtracking test-requirements.in
 #
 attrs==23.1.0
     # via service-identity
 cffi==1.15.1
     # via cryptography
-coverage[toml]==7.2.3
+coverage[toml]==7.2.7
     # via -r test-requirements.in
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   -r test-requirements.in
     #   pyopenssl
     #   service-identity
 idna==3.4
     # via -r test-requirements.in
 iniconfig==2.0.0
     # via pytest
 packaging==23.1
     # via pytest
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pyasn1-modules
     #   service-identity
 pyasn1-modules==0.3.0
     # via service-identity
 pycparser==2.21
     # via cffi
-pyopenssl==23.1.1
+pyopenssl==23.2.0
     # via -r test-requirements.in
-pytest==7.3.1
+pytest==7.4.0
     # via -r test-requirements.in
-service-identity==21.1.0
+service-identity==23.1.0
     # via -r test-requirements.in
-six==1.16.0
-    # via service-identity
```

### Comparing `trustme-1.0.0/tests/test_cli.py` & `trustme-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `trustme-1.0.0/tests/test_trustme.py` & `trustme-1.1.0/tests/test_trustme.py`

 * *Files identical despite different names*

