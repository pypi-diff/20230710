# Comparing `tmp/reliably_cli-0.8.7-py3-none-any.whl.zip` & `tmp/reliably_cli-0.8.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 22737 bytes, number of entries: 24
--rw-r--r--  2.0 unx     3602 b- defN 16-Jan-01 00:00 reliably_cli-0.8.7.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 reliably_cli-0.8.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 16-Jan-01 00:00 reliably_cli-0.8.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 reliably_cli-0.8.7.dist-info/licenses/LICENSE
+Zip file size: 22728 bytes, number of entries: 24
+-rw-r--r--  2.0 unx     3602 b- defN 16-Jan-01 00:00 reliably_cli-0.8.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 reliably_cli-0.8.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 16-Jan-01 00:00 reliably_cli-0.8.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 reliably_cli-0.8.8.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx      114 b- defN 16-Jan-01 00:00 reliably_cli/__init__.py
 -rw-r--r--  2.0 unx      890 b- defN 16-Jan-01 00:00 reliably_cli/__main__.py
 -rw-r--r--  2.0 unx      166 b- defN 16-Jan-01 00:00 reliably_cli/__version__.py
 -rw-r--r--  2.0 unx     1221 b- defN 16-Jan-01 00:00 reliably_cli/agent/__init__.py
 -rw-r--r--  2.0 unx     1545 b- defN 16-Jan-01 00:00 reliably_cli/agent/cli.py
 -rw-r--r--  2.0 unx     2775 b- defN 16-Jan-01 00:00 reliably_cli/agent/plan/__init__.py
 -rw-r--r--  2.0 unx     1352 b- defN 16-Jan-01 00:00 reliably_cli/agent/plan/providers/__init__.py
@@ -16,11 +16,11 @@
 -rw-r--r--  2.0 unx     3619 b- defN 16-Jan-01 00:00 reliably_cli/config/cli.py
 -rw-r--r--  2.0 unx     4224 b- defN 16-Jan-01 00:00 reliably_cli/config/types.py
 -rw-r--r--  2.0 unx      615 b- defN 16-Jan-01 00:00 reliably_cli/format.py
 -rw-r--r--  2.0 unx      126 b- defN 16-Jan-01 00:00 reliably_cli/log.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 reliably_cli/services/__init__.py
 -rw-r--r--  2.0 unx      211 b- defN 16-Jan-01 00:00 reliably_cli/services/cli.py
 -rw-r--r--  2.0 unx     2398 b- defN 16-Jan-01 00:00 reliably_cli/services/org.py
--rw-r--r--  2.0 unx    12433 b- defN 16-Jan-01 00:00 reliably_cli/services/plan.py
+-rw-r--r--  2.0 unx    12438 b- defN 16-Jan-01 00:00 reliably_cli/services/plan.py
 -rw-r--r--  2.0 unx     2761 b- defN 16-Jan-01 00:00 reliably_cli/types.py
-?rw-------  2.0 unx     2039 b- defN 16-Jan-01 00:00 reliably_cli-0.8.7.dist-info/RECORD
-24 files, 57389 bytes uncompressed, 19419 bytes compressed:  66.2%
+?rw-------  2.0 unx     2039 b- defN 16-Jan-01 00:00 reliably_cli-0.8.8.dist-info/RECORD
+24 files, 57394 bytes uncompressed, 19410 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
-Filename: reliably_cli-0.8.7.dist-info/METADATA
+Filename: reliably_cli-0.8.8.dist-info/METADATA
 Comment: 
 
-Filename: reliably_cli-0.8.7.dist-info/WHEEL
+Filename: reliably_cli-0.8.8.dist-info/WHEEL
 Comment: 
 
-Filename: reliably_cli-0.8.7.dist-info/entry_points.txt
+Filename: reliably_cli-0.8.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: reliably_cli-0.8.7.dist-info/licenses/LICENSE
+Filename: reliably_cli-0.8.8.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: reliably_cli/__init__.py
 Comment: 
 
 Filename: reliably_cli/__main__.py
 Comment: 
@@ -63,11 +63,11 @@
 
 Filename: reliably_cli/services/plan.py
 Comment: 
 
 Filename: reliably_cli/types.py
 Comment: 
 
-Filename: reliably_cli-0.8.7.dist-info/RECORD
+Filename: reliably_cli-0.8.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reliably_cli/services/plan.py

```diff
@@ -203,15 +203,15 @@
         env_id = str(plan.definition.environment.id)
         load_environment(env_id, target_dir)
 
 
 def load_environment(environment_id: str, target_dir: str) -> None:
     with api_client() as client:
         r = client.get(f"/environments/{environment_id}/clear")
-        env = Environment.parse_obj(r.json())
+        env = Environment.model_validate(r.json())
         if env:
             path_mapping = {}
             for s in env.secrets:
                 if isinstance(s, EnvironmentSecretAsFile):
                     new_path = Path(target_dir, s.path.lstrip("/"))
                     new_path.parent.mkdir(mode=0o710, parents=True)
                     new_path.write_text(s.value.get_secret_value())
```

## Comparing `reliably_cli-0.8.7.dist-info/METADATA` & `reliably_cli-0.8.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliably-cli
-Version: 0.8.7
+Version: 0.8.8
 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch <sylvain@reliably.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reliably-cli Version: 0.8.7 Summary: Reliably CLI
+Metadata-Version: 2.1 Name: reliably-cli Version: 0.8.8 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch
 reliably.com> License: Apache-2.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Development Status :: 4 - Beta Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities Project-URL: Homepage, https://reliably.com/
```

## Comparing `reliably_cli-0.8.7.dist-info/licenses/LICENSE` & `reliably_cli-0.8.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `reliably_cli-0.8.7.dist-info/RECORD` & `reliably_cli-0.8.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-reliably_cli-0.8.7.dist-info/METADATA,sha256=ZSq5X_6WUlapdi0ll2HOSGMws1PxR3d01luCSSCal-4,3602
-reliably_cli-0.8.7.dist-info/WHEEL,sha256=g58cvAsF5_9d0VXJuk7F0rhl6nAjUc5P9vx880WkZtI,90
-reliably_cli-0.8.7.dist-info/entry_points.txt,sha256=8jAAtHdbYV5awh7IiNkY1FbkaSqM3Gik_FEcEqkQ1d4,56
-reliably_cli-0.8.7.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+reliably_cli-0.8.8.dist-info/METADATA,sha256=4XXxOJS6xdVs3drj0GiOUzHXpbeX_V1huk8pNmdrDvA,3602
+reliably_cli-0.8.8.dist-info/WHEEL,sha256=g58cvAsF5_9d0VXJuk7F0rhl6nAjUc5P9vx880WkZtI,90
+reliably_cli-0.8.8.dist-info/entry_points.txt,sha256=8jAAtHdbYV5awh7IiNkY1FbkaSqM3Gik_FEcEqkQ1d4,56
+reliably_cli-0.8.8.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 reliably_cli/__init__.py,sha256=HFq_SCA_RUga5AGceKSZ_YSAiT93qqEMK5Y4IaXQng8,114
 reliably_cli/__main__.py,sha256=1FrWD5pKH5zaZlLNNhRhMpZXsXEvzyWeVy0C4OZxBfk,890
 reliably_cli/__version__.py,sha256=WFBbHIlbb-F214FFjtW1xDe_4jCXZ4T2yM5tQRqF8fI,166
 reliably_cli/agent/__init__.py,sha256=6tPrPONJnMyxYKJHxieIap5j3d54sRkKtJElD0tj9Y0,1221
 reliably_cli/agent/cli.py,sha256=mAE9HnRIcNrWFIZ7LPpaU4anJNVl7HbYYznXnVXnjMc,1545
 reliably_cli/agent/plan/__init__.py,sha256=0vqfETLpWtIM4t3Vzrq_IOdZEyt-fCcmgYGW2gNmON8,2775
 reliably_cli/agent/plan/providers/__init__.py,sha256=LRksrizsgth5mIBKvHxxn5L429HNAWdF24k_LANoA4U,1352
@@ -15,10 +15,10 @@
 reliably_cli/config/cli.py,sha256=qAKEODgEGso9kKfRgTHhcvpmcZIDFkBmWd5g98Hp1GE,3619
 reliably_cli/config/types.py,sha256=1zcLYgtNT3l5WyiTjYMatbbnWafTBoXQZmmw6mdnJp4,4224
 reliably_cli/format.py,sha256=JrQzam_1or-YGl9zh8SWRQEwYKtI5tJdpDNpYELmHMg,615
 reliably_cli/log.py,sha256=jnRxvSIRsmUdIEGItA4F314YqE5TsXMKnAKmMAwbx3o,126
 reliably_cli/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 reliably_cli/services/cli.py,sha256=mXyYkAUqCEfZ4Sa0FwToR11b33bn2pnpQSzw6XJ5HVI,211
 reliably_cli/services/org.py,sha256=rEFZCb7bWGArrZhplQhajm5oO4ZLQ2m0ITyWy5iyCn0,2398
-reliably_cli/services/plan.py,sha256=ABsNOkDwCA1uXOUM_xEg8gpgVsWJ-IJGWxZQ1LMj3ms,12433
+reliably_cli/services/plan.py,sha256=xKRExhptBo4ILwinGejPjUEzz6aZxPUI5yr93GfdeEQ,12438
 reliably_cli/types.py,sha256=-Xp2_15kbS91Li6D4q7KCvK1nY5zWJlkXVOVo6n4bsg,2761
-reliably_cli-0.8.7.dist-info/RECORD,,
+reliably_cli-0.8.8.dist-info/RECORD,,
```

