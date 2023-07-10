# Comparing `tmp/kfish-99.0.202307100657-py3-none-any.whl.zip` & `tmp/kfish-99.0.202307101241-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7501 bytes, number of entries: 6
--rw-r--r--  2.0 unx     9013 b- defN 23-Jul-10 06:48 kfish/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jul-10 06:57 kfish-99.0.202307100657.dist-info/LICENSE
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-10 06:57 kfish-99.0.202307100657.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 06:57 kfish-99.0.202307100657.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-10 06:57 kfish-99.0.202307100657.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-10 06:57 kfish-99.0.202307100657.dist-info/RECORD
-6 files, 21280 bytes uncompressed, 6571 bytes compressed:  69.1%
+Zip file size: 7500 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     9018 b- defN 23-Jul-10 12:33 kfish/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-10 12:41 kfish-99.0.202307101241.dist-info/LICENSE
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-10 12:41 kfish-99.0.202307101241.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 12:41 kfish-99.0.202307101241.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-10 12:41 kfish-99.0.202307101241.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-10 12:41 kfish-99.0.202307101241.dist-info/RECORD
+6 files, 21285 bytes uncompressed, 6570 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kfish/__init__.py
 Comment: 
 
-Filename: kfish-99.0.202307100657.dist-info/LICENSE
+Filename: kfish-99.0.202307101241.dist-info/LICENSE
 Comment: 
 
-Filename: kfish-99.0.202307100657.dist-info/METADATA
+Filename: kfish-99.0.202307101241.dist-info/METADATA
 Comment: 
 
-Filename: kfish-99.0.202307100657.dist-info/WHEEL
+Filename: kfish-99.0.202307101241.dist-info/WHEEL
 Comment: 
 
-Filename: kfish-99.0.202307100657.dist-info/top_level.txt
+Filename: kfish-99.0.202307101241.dist-info/top_level.txt
 Comment: 
 
-Filename: kfish-99.0.202307100657.dist-info/RECORD
+Filename: kfish-99.0.202307101241.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kfish/__init__.py

```diff
@@ -50,15 +50,15 @@
         self.headers = {'Content-Type': 'application/json', 'Accept': 'application/json'}
         if insecure:
             ssl._create_default_https_context = ssl._create_unverified_context
         url = url.replace('idrac-virtualmedia', 'https').replace('ilo5-virtualmedia', 'https')
         self.model, self.url, self.user, self.password = get_info(url, user, password)
         if self.debug:
             print(f"Using base url {self.url}")
-        p = urlparse(url)
+        p = urlparse(self.url)
         self.baseurl = f"{p.scheme}://{p.netloc}"
         credentials = base64.b64encode(bytes(f'{self.user}:{self.password}', 'ascii')).decode('utf-8')
         self.headers["Authorization"] = f"Basic {credentials}"
         self.manager_url = None
 
     def get_manager_url(self):
         request = Request(self.url, headers=self.headers)
```

## Comparing `kfish-99.0.202307100657.dist-info/LICENSE` & `kfish-99.0.202307101241.dist-info/LICENSE`

 * *Files identical despite different names*

