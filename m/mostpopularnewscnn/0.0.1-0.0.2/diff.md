# Comparing `tmp/mostpopularnewscnn-0.0.1.tar.gz` & `tmp/mostpopularnewscnn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostpopularnewscnn-0.0.1.tar", last modified: Wed Jul  5 15:50:23 2023, max compression
+gzip compressed data, was "mostpopularnewscnn-0.0.2.tar", last modified: Mon Jul 10 13:44:20 2023, max compression
```

## Comparing `mostpopularnewscnn-0.0.1.tar` & `mostpopularnewscnn-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 15:50:23.363831 mostpopularnewscnn-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-01 14:10:17.000000 mostpopularnewscnn-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-07-05 15:50:23.362830 mostpopularnewscnn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-07-05 15:41:42.000000 mostpopularnewscnn-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 15:50:23.346835 mostpopularnewscnn-0.0.1/mostpopularnewscnn/
--rw-rw-rw-   0        0        0     2598 2023-07-01 15:28:14.000000 mostpopularnewscnn-0.0.1/mostpopularnewscnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:50:23.359831 mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-07-05 15:50:23.000000 mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-05 15:50:23.000000 mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 15:50:23.000000 mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 15:50:23.000000 mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-07-05 15:49:56.000000 mostpopularnewscnn-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 15:50:23.364831 mostpopularnewscnn-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.621883 mostpopularnewscnn-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-01 14:10:17.000000 mostpopularnewscnn-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1127 2023-07-10 13:44:20.620883 mostpopularnewscnn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-08 13:50:59.000000 mostpopularnewscnn-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.607884 mostpopularnewscnn-0.0.2/mostpopularnewscnn/
+-rw-rw-rw-   0        0        0     2199 2023-07-10 13:29:11.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:44:20.618884 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/
+-rw-rw-rw-   0        0        0     1127 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-10 13:44:20.000000 mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-07-10 13:41:31.000000 mostpopularnewscnn-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:44:20.622883 mostpopularnewscnn-0.0.2/setup.cfg
```

### Comparing `mostpopularnewscnn-0.0.1/LICENSE` & `mostpopularnewscnn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mostpopularnewscnn-0.0.1/PKG-INFO` & `mostpopularnewscnn-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostpopularnewscnn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package will get the most popular news in CNN Indonesia
 Author-email: Tri Prasetyo Kusumo Aji <ajikprasetyo22@gmail.com>
 Project-URL: Homepage, https://github.com/jetkesuma/most-popular-news-cnn-id
 Project-URL: Medium, https://medium.com/@kusumo999666
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,7 +16,13 @@
 # Most Popular News CNN Indonesia
 This package will get the most popular news in CNN Indonesia
 
 ## HOW IT WORK?
 This package will scrape from [CNN Indonesia](https://www.cnnindonesia.com/) to get most popular news in CNN Indonesia 
 
 This package uses beatifulsoup4 and requests then produces output in the form of json which can be used in web and mobile applications
+
+'''
+if __name__ == '__main__':
+    result = data_extraction()
+    show_data(result)
+'''
```

### Comparing `mostpopularnewscnn-0.0.1/mostpopularnewscnn/__init__.py` & `mostpopularnewscnn-0.0.2/mostpopularnewscnn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import requests
 from bs4 import BeautifulSoup
 
+description = 'to get the most popular news in cnnindonesia.com'
 
 def data_extraction():
-    """
-    1. SBY tidak masalah jika Jokowi tidak suka dengan anies baswedan
-    2. Video: Bangunan 13 lantai Runtuh di Mesir, 4 Orang Terluka
-    3. Prabowo mendadak dipanggil jokowi, Gelar pertemuan Tertutup di Istana
-    4. Surya Paloh yakin anies tak akan jadi tersangka jelang pilpres 2024
-    5. Bahas Politik, Prabowo ditanya jokowi soal rencana ke depan
-    6. Erick thohir Ungkap kekurangan JIS untuk Venue Piala Dunia U-175
-    :return:
-    """
     try:
         content = requests.get('https://www.cnnindonesia.com/')
     except Exception:
         return None
     if content.status_code == 200:
         soup = BeautifulSoup(content.text, 'html.parser')
         oke = soup.find('div', {'class': 'headline__terpopuler-list'})
```

### Comparing `mostpopularnewscnn-0.0.1/mostpopularnewscnn.egg-info/PKG-INFO` & `mostpopularnewscnn-0.0.2/mostpopularnewscnn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostpopularnewscnn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package will get the most popular news in CNN Indonesia
 Author-email: Tri Prasetyo Kusumo Aji <ajikprasetyo22@gmail.com>
 Project-URL: Homepage, https://github.com/jetkesuma/most-popular-news-cnn-id
 Project-URL: Medium, https://medium.com/@kusumo999666
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,7 +16,13 @@
 # Most Popular News CNN Indonesia
 This package will get the most popular news in CNN Indonesia
 
 ## HOW IT WORK?
 This package will scrape from [CNN Indonesia](https://www.cnnindonesia.com/) to get most popular news in CNN Indonesia 
 
 This package uses beatifulsoup4 and requests then produces output in the form of json which can be used in web and mobile applications
+
+'''
+if __name__ == '__main__':
+    result = data_extraction()
+    show_data(result)
+'''
```

### Comparing `mostpopularnewscnn-0.0.1/pyproject.toml` & `mostpopularnewscnn-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.31.0", "beautifulsoup4>= 4.12.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mostpopularnewscnn"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tri Prasetyo Kusumo Aji", email="ajikprasetyo22@gmail.com" },
 ]
 description = "This package will get the most popular news in CNN Indonesia"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

