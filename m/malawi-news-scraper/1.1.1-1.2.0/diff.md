# Comparing `tmp/malawi-news-scraper-1.1.1.tar.gz` & `tmp/malawi-news-scraper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malawi-news-scraper-1.1.1.tar", last modified: Fri Jul  7 20:23:54 2023, max compression
+gzip compressed data, was "malawi-news-scraper-1.2.0.tar", last modified: Mon Jul 10 06:15:00 2023, max compression
```

## Comparing `malawi-news-scraper-1.1.1.tar` & `malawi-news-scraper-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:23:54.413915 malawi-news-scraper-1.1.1/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.1.1/LICENSE
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       27 2023-07-07 18:00:31.000000 malawi-news-scraper-1.1.1/MANIFEST.in
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 20:23:54.413915 malawi-news-scraper-1.1.1/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.1.1/README.md
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1129 2023-07-07 20:23:24.000000 malawi-news-scraper-1.1.1/pyproject.toml
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-07 20:23:54.413915 malawi-news-scraper-1.1.1/setup.cfg
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:23:54.409916 malawi-news-scraper-1.1.1/src/
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:23:54.413915 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 20:23:54.000000 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      447 2023-07-07 20:23:54.000000 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-07 20:23:54.000000 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       87 2023-07-07 20:23:54.000000 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/requires.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-07 20:23:54.000000 malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:23:54.413915 malawi-news-scraper-1.1.1/src/scrapers/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      287 2023-07-07 20:23:24.000000 malawi-news-scraper-1.1.1/src/scrapers/__init__.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     2044 2023-07-07 20:01:58.000000 malawi-news-scraper-1.1.1/src/scrapers/base_feed_scraper.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      298 2023-07-07 20:02:31.000000 malawi-news-scraper-1.1.1/src/scrapers/base_parser.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      114 2023-07-07 19:36:50.000000 malawi-news-scraper-1.1.1/src/scrapers/config.toml
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      162 2023-07-07 20:23:09.000000 malawi-news-scraper-1.1.1/src/scrapers/malawi_voice.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      160 2023-07-07 20:22:50.000000 malawi-news-scraper-1.1.1/src/scrapers/maravi_post.py
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-10 06:15:00.702382 malawi-news-scraper-1.2.0/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.2.0/LICENSE
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       27 2023-07-07 18:00:31.000000 malawi-news-scraper-1.2.0/MANIFEST.in
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-10 06:15:00.702382 malawi-news-scraper-1.2.0/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.2.0/README.md
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1129 2023-07-10 06:14:44.000000 malawi-news-scraper-1.2.0/pyproject.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-10 06:15:00.702382 malawi-news-scraper-1.2.0/setup.cfg
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-10 06:15:00.698382 malawi-news-scraper-1.2.0/src/
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-10 06:15:00.702382 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-10 06:15:00.000000 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      517 2023-07-10 06:15:00.000000 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-10 06:15:00.000000 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       87 2023-07-10 06:15:00.000000 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/requires.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-10 06:15:00.000000 malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-10 06:15:00.702382 malawi-news-scraper-1.2.0/src/scrapers/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      607 2023-07-10 06:14:44.000000 malawi-news-scraper-1.2.0/src/scrapers/__init__.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     2965 2023-07-09 09:11:50.000000 malawi-news-scraper-1.2.0/src/scrapers/base_feed_scraper.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      298 2023-07-07 20:02:31.000000 malawi-news-scraper-1.2.0/src/scrapers/base_parser.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      249 2023-07-09 09:00:35.000000 malawi-news-scraper-1.2.0/src/scrapers/config.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      155 2023-07-09 09:02:00.000000 malawi-news-scraper-1.2.0/src/scrapers/malawi24.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      162 2023-07-07 20:23:09.000000 malawi-news-scraper-1.2.0/src/scrapers/malawi_voice.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      160 2023-07-07 23:19:41.000000 malawi-news-scraper-1.2.0/src/scrapers/maravi_post.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      155 2023-07-07 23:17:15.000000 malawi-news-scraper-1.2.0/src/scrapers/mwnation.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      145 2023-07-09 08:16:15.000000 malawi-news-scraper-1.2.0/src/scrapers/pij.py
```

### Comparing `malawi-news-scraper-1.1.1/LICENSE` & `malawi-news-scraper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malawi-news-scraper-1.1.1/PKG-INFO` & `malawi-news-scraper-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.1.1/pyproject.toml` & `malawi-news-scraper-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
-requires = ['setuptools>=1.1.1', 'wheel']
+requires = ['setuptools>=1.2.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'malawi-news-scraper'
-version = '1.1.1'
+version = '1.2.0'
 description = 'Scrape news from known news outlets in Malawi'
 readme = 'README.md'
 authors = [{ name = 'Hopson Gausi', email = 'hopgausi@gmail.com' }]
 license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
 ]
 keywords = ['News scraper', 'scraper', 'malawi']
 dependencies = [
-    'feedparser >= 1.1.1',
+    'feedparser >= 1.2.0',
     'html2text',
     'beautifulsoup4'
 ]
 requires-python = '>=3.11'
 
 [project.optional-dependencies]
 dev = ['black', 'bumpver', 'isort', 'pip-tools', 'pytest']
 
 [project.urls]
 Homepage = 'https://github.com/hopgausi/malawi-news-scraper'
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.2.0"
 version_pattern = 'MAJOR.MINOR.PATCH'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `malawi-news-scraper-1.1.1/src/malawi_news_scraper.egg-info/PKG-INFO` & `malawi-news-scraper-1.2.0/src/malawi_news_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.1.1/src/scrapers/base_feed_scraper.py` & `malawi-news-scraper-1.2.0/src/scrapers/base_feed_scraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         sanitized_news = []
         news_list = parsed_xml_news.entries
         for news in news_list:
             title = news['title']
             link = news['link']
             author = news['author']
             published_date = news['published']
-            cover_image = self._get_image_url(news['content'][0]['value'])
+            content = news['content'][0]['value'] if len(news.get('content', [])) > 0 else ''
+            cover_image = self._get_image_url(content)
             sanitized_news.append({
                 'title': title,
                 'link': link,
                 'author': author,
                 'published_date': published_date,
                 'cover_image': cover_image,
             })
@@ -46,13 +47,31 @@
         soup = BeautifulSoup(content, 'html.parser')
         img_tag = soup.find_all('img')
         img = img_tag[0]['src'] if len(img_tag) > 0 else ''
         return img
     
     def _get_source_details(self, feed: dict) -> dict:
         """Returns the source details for the news, that is, the site the feed is being scraped from"""
+        name = feed['title']
+        link = feed['link']
+        if len(name) == 0:
+            name = self._get_source_name(link)
         source_details = {
-            'name': feed['title'],
-            'url': feed['link'],
-            'mission_statement': feed['subtitle'],
+            'name': name,
+            'url': link,
+            'mission_statement': feed['subtitle'] if len(feed['subtitle']) > 0 else self._get_mission_statement(name),
         }
-        return source_details
+        return source_details
+
+    def _get_source_name(self, link):
+        """Returns source name of the news based on link provided should the feed have no defined source name"""
+        name = ''
+        if 'investigativeplatform-mw' in link:
+            name = 'Platform For Investigative Journalism'
+        return name
+    
+    def _get_mission_statement(self, source_name):
+        """Returns source mission statement of the news based on source name provided should the feed have no defined source statement"""
+        statement = ''
+        if source_name == 'Platform For Investigative Journalism':
+            statement = 'Digging Truth. Lighting Democracy'
+        return statement
```

