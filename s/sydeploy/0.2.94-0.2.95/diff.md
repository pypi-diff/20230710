# Comparing `tmp/sydeploy-0.2.94-py3-none-any.whl.zip` & `tmp/sydeploy-0.2.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7335 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:29 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-10 04:29 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-10 04:29 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:29 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:29 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2309 b- defN 23-Jul-10 04:29 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:29 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     4370 b- defN 23-Jul-10 04:29 sydeploy/commands/build/python-package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-10 04:29 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-10 04:29 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:29 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx      807 b- defN 23-Jul-10 04:29 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/LICENSE
--rw-r--r--  2.0 unx      283 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1516 b- defN 23-Jul-10 04:29 sydeploy-0.2.94.dist-info/RECORD
-18 files, 11457 bytes uncompressed, 4801 bytes compressed:  58.1%
+Zip file size: 7324 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:44 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-10 04:44 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-10 04:44 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:44 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:44 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2307 b- defN 23-Jul-10 04:44 sydeploy/commands/authenticate/codeartifact.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:44 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     4370 b- defN 23-Jul-10 04:44 sydeploy/commands/build/python-package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-10 04:44 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-10 04:44 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:44 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx      807 b- defN 23-Jul-10 04:44 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/LICENSE
+-rw-r--r--  2.0 unx      283 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1516 b- defN 23-Jul-10 04:44 sydeploy-0.2.95.dist-info/RECORD
+18 files, 11455 bytes uncompressed, 4790 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/LICENSE
+Filename: sydeploy-0.2.95.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/METADATA
+Filename: sydeploy-0.2.95.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/WHEEL
+Filename: sydeploy-0.2.95.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/entry_points.txt
+Filename: sydeploy-0.2.95.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/top_level.txt
+Filename: sydeploy-0.2.95.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.2.94.dist-info/RECORD
+Filename: sydeploy-0.2.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/authenticate/codeartifact.py

```diff
@@ -8,15 +8,15 @@
     pip = "pip" + str(sys.version_info[0])
     return run(args=f"{pip} config get global.index-url", shell=True, capture_output=True).stdout.decode("utf-8").strip()
 
 
 def set_index_url(body, extra: bool = False):
     pip = "pip" + str(sys.version_info[0])
     index_url = "extra-index-url" if extra else "index-url"
-    check_call([pip, "config", "set", f"globals.{index_url}", body])
+    check_call([pip, "config", "set", f"global.{index_url}", body])
 
 
 @impose
 def pip(domain: str = None, repo: str = None, region: str = None):
     if domain is None or repo is None:
         raise Exception("A domain and a repo must be defined for CodeArtifact.")
     region = "" if region is None else f"--region {region}"
@@ -29,15 +29,15 @@
                    f"authorizationToken --output text", shell=True, capture_output=True)
     res = res.stdout.decode("utf-8").strip()
 
     # By default, AWS CodeArtifact overrides the PIP config file
     # I assume that this is a bug, but for the meantime, the solution
     # is to take the remote host, save it temporarily,
     # let aws replace it, and then switch it
-    new_index_url = f"https://{res}@{domain}-{account_id}.d.codeartifact.us-west-2.amazonaws.com/pypi/{repo}/simple/"
+    new_index_url = f"https://{res}@{domain}-{account_id}.d.codeartifact.{region}.amazonaws.com/pypi/{repo}/simple/"
     set_index_url(new_index_url, extra=True)
 
 
 @impose
 def twine(domain: str = None, repo: str = None, region: str = None):
     if domain is None or repo is None or region is None:
         raise Exception("A domain, repository, and region must be defined for authentication with CodeArtifact.")
```

## Comparing `sydeploy-0.2.94.dist-info/LICENSE` & `sydeploy-0.2.95.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.2.94.dist-info/RECORD` & `sydeploy-0.2.95.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/authenticate/codeartifact.py,sha256=FpvFg4epcA4NgqguQLrdVidVbw7I66TbLE1L7-KxdCw,2309
+sydeploy/commands/authenticate/codeartifact.py,sha256=B9Pd0UiOhgqL3EzET6EkruEk3X_DS6LcUWgframZTz0,2307
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python-package.py,sha256=6ti1iLGToUVivx_b0x7SIuilpwU0fPBS4aFH_NKXDWU,4370
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.2.94.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.2.94.dist-info/METADATA,sha256=Gz83pkmNqDy1CQrO0LgRmQaVs6u1a_69jG0obWeXIts,283
-sydeploy-0.2.94.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.2.94.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.2.94.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.2.94.dist-info/RECORD,,
+sydeploy-0.2.95.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.2.95.dist-info/METADATA,sha256=d05FTC0bLfiE1i6e_9RZ89yuxZOT_3df9cG2UHtbJ6Y,283
+sydeploy-0.2.95.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.2.95.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.2.95.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.2.95.dist-info/RECORD,,
```

