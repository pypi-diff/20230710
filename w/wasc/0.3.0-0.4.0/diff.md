# Comparing `tmp/wasc-0.3.0.tar.gz` & `tmp/wasc-0.4.0.tar.gz`

## Comparing `wasc-0.3.0.tar` & `wasc-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 wasc-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 wasc-0.3.0/requirements_dev.txt
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wasc-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wasc-0.3.0/data/checkers.csv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.3.0/data/example_websites.csv
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 wasc-0.3.0/data/sub_list.csv
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/checkers.md
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/index.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/license.md
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/releases.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__main__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/abstract_checker.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/checker_factory.py
--rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/default_checkers.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/utils.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/cli/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_checker.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_checker_factory.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/data/checkers_example.csv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/data/url_example.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wasc-0.3.0/.gitignore
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 wasc-0.3.0/README.md
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 wasc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wasc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 wasc-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 wasc-0.4.0/requirements_dev.txt
+-rw-r--r--   0        0        0    61569 2020-02-02 00:00:00.000000 wasc-0.4.0/test_culture.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wasc-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wasc-0.4.0/data/checkers.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.4.0/data/example_websites.csv
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 wasc-0.4.0/data/sub_list.csv
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/checkers.md
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/license.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/releases.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__main__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/abstract_checker.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/checker_factory.py
+-rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/checkers.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/utils.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/cli/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_checker.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_checker_factory.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/data/checkers_example.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/data/url_example.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wasc-0.4.0/.gitignore
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 wasc-0.4.0/README.md
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 wasc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 wasc-0.4.0/PKG-INFO
```

### Comparing `wasc-0.3.0/.github/workflows/docs.yml` & `wasc-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/docs/checkers.md` & `wasc-0.4.0/docs/checkers.md`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/docs/index.md` & `wasc-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/docs/license.md` & `wasc-0.4.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/src/wasc/abstract_checker.py` & `wasc-0.4.0/src/wasc/abstract_checker.py`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/src/wasc/checker_factory.py` & `wasc-0.4.0/src/wasc/checker_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 -------
 CheckerFactory
 
 Objects
 -------
 checker_factory
 """
-import wasc.default_checkers as dft
+import wasc.checkers as chk
 
 
 class CheckerFactory :
     """CheckerFactory
     Implements a Factory design pattern to record and to create Checkers objects
 
     Attributes
@@ -103,15 +103,18 @@
         -------
         : bool
         True is the checker name is known
         """
         return checker_name in self.__checker_dict
 
 checker_factory = CheckerFactory()
-checker_factory.register("DFTT01", dft.DFTT01)
-checker_factory.register("DFTT02", dft.DFTT02)
-checker_factory.register("AccessRateChecker", dft.AccessRateChecker)
-checker_factory.register("LangChecker", dft.LangChecker)
-checker_factory.register("DoctypeChecker", dft.DoctypeChecker)
-checker_factory.register("AccessChecker", dft.AccessChecker)
-checker_factory.register("AccessLinkChecker", dft.AccessLinkChecker)
-checker_factory.register("LegalChecker", dft.LegalChecker)
+checker_factory.register("HeadNbChecker", chk.HeadNbChecker)
+checker_factory.register("HeadLvlChecker", chk.HeadLvlChecker)
+checker_factory.register("AccessRateChecker", chk.AccessRateChecker)
+checker_factory.register("LangChecker", chk.LangChecker)
+checker_factory.register("DoctypeChecker", chk.DoctypeChecker)
+checker_factory.register("AccessChecker", chk.AccessChecker)
+checker_factory.register("AccessLinkChecker", chk.AccessLinkChecker)
+checker_factory.register("LegalChecker", chk.LegalChecker)
+checker_factory.register("HeaderChecker", chk.HeaderChecker)
+checker_factory.register("FooterChecker", chk.FooterChecker)
+checker_factory.register("ContactLinkChecker", chk.ContactLinkChecker)
```

### Comparing `wasc-0.3.0/src/wasc/default_checkers.py` & `wasc-0.4.0/src/wasc/checkers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,43 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
-"""
-Module default_checker
 
-Provides custom classes of checkers inherited from AbstractChecker.
-Checkers are used to analyze the content of web pages as Beautiful soup objects.
-Present Checkers were defined with the help of François le Berre.
-
-Classes
--------
-DFTT01(AbstractChecker) :
-    Test the presence of tags <HEAD>
-DFTT02(AbstractChecker) :
-    Test the depth of tags <HEAD>
-AccessChecker(AbstractChecker) :
-    Test the presence of "Accessibilité" in the page
-AccessLinkChecker(AbstractChecker) :
-    Test if a link exist to the accessibility page
-AccessRateChecker(AbstractChecker) :
-    Test the presence of a compliance rate (%) on the accessibility statement
-LegalChecker(AbstractChecker) :
-    Test the presence of "mention légales" link on the web page
-LangChecker(AbstractChecker) :
-    Test the presence of the language in the header of the HTML page
-DoctypeChecker(AbstractChecker) :
-    Test the presence of Doctype in the web page
-"""
-import functools
 import re
 
 import bs4
-import requests
+from trafilatura import fetch_url
 
 from wasc.abstract_checker import AbstractChecker
 from wasc.utils import HEADER, check_and_correct_url, find_link
 
+PRESENT = "présent"
 FAIL = "échec"
+OK = 200
 mentions = "non|partiellement|totalement"
 ACCESS_PATTERN = re.compile("Accessibilité[ \xa0]:[ \xa0](" + mentions + ")[ \xa0]conforme", re.IGNORECASE)
 
-class DFTT01(AbstractChecker) :
-    """DFTT01
-    A class to test the presence of <head> tags.
-    This class inherits from the AbstrastChecker.
+class HeadNbChecker(AbstractChecker) :
+    """HeadNbChecker
+    A class to test the number of <head> tags in a page.
 
     Attributes
     ----------
     name : str
         The name of the checker, i.e. a small identifier used in config files
     description : str
         The description of the checker, used in output
 
     Methods
     -------
     execute(self, web_page, url) -> dict :
-        return the result of the checker
+        return the number of <head> tags (expected 1)
     """
     def __init__(self) :
-        super().__init__("DFTT01", "Nombre de <head>")
+        super().__init__("HeadNbChecker", "Nombre de <head>")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
         Gets the number of <head> tags in the web page
 
         Parameters
         ----------
@@ -74,38 +49,20 @@
         Returns
         -------
          : int
             The number of <head> tags
         """
         return len(web_page.find_all(name="head"))
 
-class DFTT02(AbstractChecker) :
-    """DFTT02
-    A class to get the depth of <head> tags in a web page.
-    This class inherits from the AbstrastChecker.
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the result of the checker
+class HeadLvlChecker(AbstractChecker) :
+    """HeadLvlChecker
+    Get the depth of <head> tags in a web page.
     """
     def __init__(self) :
-        """
-        It constructs all the necessary attributes for the DFTT02 class
-
-        Parameters
-        ----------
-        None
-        """
-        super().__init__("DFTT02", "Profondeur des <head>")
+        super().__init__("HeadLvlChecker", "Profondeurs des <head>")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
         Returns the depth of <head> tags of the web page
 
         Parameters
         ----------
@@ -120,36 +77,17 @@
             The list of depth of head tags
         """
         head_tag = web_page.find_all("head")
         return [len(list(tag.parents)) - 1 for tag in head_tag] if head_tag else []
 
 class AccessChecker(AbstractChecker) :
     """AccessChecker
-    Check the presence of "Accessibilité" mention on the web page.
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the level string or "non conforme"
+    Check the presence of "Accessibilité" RGAA4 mention on the web page.
     """
     def __init__(self) :
-        """
-        Sets the name and description of AccessChecker
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("AccessChecker", "Mention accessibilité")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
         If there is a mention "Accessibilité", returns the level of accessibility,
         else "non conforme"
 
@@ -168,36 +106,17 @@
         mention = web_page.find_all(string = ACCESS_PATTERN)
         if mention :
             return mention[0].split(":")[1].strip()
         return FAIL
 
 class AccessLinkChecker(AbstractChecker) :
     """AccessLinkChecker
-    Check that "Accessibilité" present on the web page is a link.
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the link URL
+    Check if a link ot an accessibility statement exists
     """
     def __init__(self) :
-        """
-        It constructs all the necessary attributes for the AccessLinkChecker class
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("AccessLinkChecker", "Lien accessibilité")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
         Search for a link to the accessibility page, either :
         * if the mention "Accessibilité" is a link
         * if there exists a link to root_url/accessibilite
@@ -223,50 +142,30 @@
                 return link
         # 2 - Find text "Déclaration d'accessibilité" and check if it's a link
         access_tag = web_page.find(string = "Déclaration d'accessibilité")
         if access_tag :
             link = find_link(access_tag, root_url)
             if link :
                 return link
-        # 3 - Check if there exists a link to a standard adresse root_url/accessibilite
-        standard_link = check_and_correct_url("accessibilite", root_url)
+        # 3 - Check if there exists a link that ends with accessibilite or accessibility
         link_tags = web_page.find_all("a")
         for tag in link_tags:
             try :
-                if check_and_correct_url(tag.attrs["href"], root_url) == standard_link:
-                    return standard_link
+                current_link = check_and_correct_url(tag.attrs["href"], root_url)
+                if current_link.endswith("accessibility") or current_link.endswith("accessibilite"):
+                    return current_link
             except KeyError :
                 pass
         return FAIL
 
 class AccessRateChecker(AbstractChecker) :
     """AccessRateChecker
-    A class to represent the test of presence of compliance rate (%) on the accessibility statement
-    web page. This class inherits from the AbstrastChecker class.
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the result of the checker
+    Get compliance rate (%) on the accessibility statement (if it exists)
     """
     def __init__(self) :
-        """
-        It constructs all the necessary attributes for the AccessRateChecker class
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("AccessRateChecker", "Taux d'accessibilité")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
         This method performs the test on the beautifulsoup object passed in parameter and determines
         if there is a compliance rate (%) on the accessibility statement web page or not
 
@@ -275,84 +174,40 @@
         web_page : bs4.BeautifulSoup
             The BeautifulSoup object created from url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        dict :
-            The name of the checker is the key and the value is either False if there is no
-            compliance rate (%), or the compliance rate (%)
+        str :
+            the compliance rate (%), or "échec" if not found
         """
-        checker_04 = AccessLinkChecker()
-        access_url = checker_04.execute(web_page, root_url)
-        if not access_url :
-            return False
-        response = requests.get(access_url, headers=HEADER, timeout = 1)
-        if response.status_code == requests.codes.ok :
-            access_page = bs4.BeautifulSoup(response.content, "html.parser")
-        else :
-            msg = f"The status_code is {response.status_code}, check the URL : {access_url}"
-            raise ValueError(msg)
-        for access_string in access_page.stripped_strings :
-            match_string = re.search(r"Résultats des tests.*",access_string, \
-                                     flags = re.IGNORECASE)
-            if not match_string :
-                continue
-            if isinstance(access_page, bs4.NavigableString):
-                access_tag = access_page.find(string = re.compile("Résultats des tests",\
-                                                                   re.IGNORECASE)).parent
-            iter_limit = 10
-            while iter_limit and isinstance(access_tag, bs4.Tag) :
-                for tag in access_tag.next_siblings :
-                    if isinstance(tag, bs4.Tag) and tag.name :
-                        statement = tag.find(string = re.compile("%"))
-                        if statement :
-                            statement_str = str(statement)
-                            try:
-                                index = statement_str.index("%")
-                                counter = 0
-                                for j in range(index-1, index-10, -1) :
-                                    if statement_str[j] in "0123456789 ,." :
-                                        counter += 1
-                                    else :
-                                        break
-                                compliance_tmp = statement_str[index - counter:index + 1].split(" ")
-                                compliance = functools.reduce(lambda x, y : x + y, compliance_tmp)
-                                return compliance
-                            except ValueError:
-                                continue
-                access_tag = access_tag.parent
-                iter_limit -= 1
-        return False
+        link_url = AccessLinkChecker().execute(web_page, root_url)
+        if link_url == FAIL:
+            return FAIL
+        try:
+            response = fetch_url(link_url, decode=False)
+            if response.status == OK :
+                link_page = bs4.BeautifulSoup(response.data, "html.parser")
+                motif = re.compile(r"%", re.IGNORECASE)
+                percent_tags = link_page.find_all(string = motif)
+                for tag in percent_tags:
+                    if "conformité" in tag:
+                        m = re.search(r"\s(100|(\d{1,2}([\.\,]\d+)*))\ *%", str(tag))
+                        if m:
+                            return str(m[1]) + "%"
+        except Exception as e:
+            return FAIL
+        return FAIL
 
 class LegalChecker(AbstractChecker) :
     """LegalChecker
     Test the presence of "Mentions légales" link on the web page.
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the link to the page or fail
     """
     def __init__(self) :
-        """
-        It constructs all the necessary attributes for the LegalChecker class
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("LegalChecker", "Mentions légales")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
         Try to find :
         * text "Mentions légales" (case insensitive) and check if a link exists
         * try the url root_url + "/mentions-legales" and check if a link exists
@@ -373,47 +228,33 @@
         motif = re.compile("Mentions* l[eé]gales*", re.IGNORECASE)
         legal_tags = web_page.find_all(string = motif)
         for tag in legal_tags:
             legal_tag = tag
             while legal_tag and legal_tag.name != "a" and legal_tag.name != "html":
                 legal_tag = legal_tag.parent
             try :
-                return check_and_correct_url(legal_tag.attrs["href"], root_url)
+                legal_link = check_and_correct_url(legal_tag.attrs["href"], root_url)
+                if root_url != legal_link:
+                    return check_and_correct_url(legal_tag.attrs["href"], root_url)
             except KeyError :
                 pass
         legal_link = check_and_correct_url("mentions-legales", root_url)
-        response = requests.get(legal_link, headers=HEADER, timeout = 1)
-        if response.status_code == requests.codes.ok :
-            return legal_link
+        try:
+            response = fetch_url(legal_link, decode=False)
+            if response.status == OK :
+                return legal_link
+        except Exception:
+            return FAIL
         return FAIL
 
 class LangChecker(AbstractChecker) :
     """LangChecker
     Check the presence of attribute lang in the html tag of the website
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return the lang string or "non conforme"
     """
     def __init__(self) :
-        """
-        Sets the name and description of LangChecker
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("LangChecker", "Lang")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
         If the language is specified in the html tag, returns a string
         corresponding to the language of the web page, else "non conforme"
 
@@ -433,37 +274,17 @@
             if isinstance(web_page.html, bs4.Tag):
                 return web_page.html.attrs["lang"]
         except KeyError :
             return FAIL
 
 class DoctypeChecker(AbstractChecker) :
     """DoctypeChecker
-    Check the presence of DOCTYPE at the beginning of HTML document
-    (before <html>) + the type is html
-
-    Attributes
-    ----------
-    name : str
-        The name of the checker
-    description : str
-        Description of the checker
-
-    Methods
-    -------
-    execute(self, web_page, url) :
-        return "html" or "non conforme"
+    Check the presence of <!DOCTYPE html> at the beginning of HTML document (before <html>)
     """
     def __init__(self) :
-        """
-        Sets the name and description of DoctypeChecker
-
-        Parameters
-        ----------
-        None
-        """
         super().__init__("DoctypeChecker", "Doctype")
 
     def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
         Check the presence of doctype in html document
 
         Parameters
@@ -471,16 +292,16 @@
         web_page : bs4.BeautifulSoup
             The BeautifulSoup object created url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        bool :
-            True if Doctype is present, before <html> and has "html" value
+        str :
+            return "html" if valid else "échec"
         """
         current_pos = 0
         doctype_pos = 1
         html_pos = 0
         doctype_found = False
         for item in web_page.contents:
             if isinstance(item, bs4.Doctype):
@@ -490,7 +311,67 @@
                     return FAIL
             elif isinstance(item, bs4.Tag) and item.name == "html":
                 html_pos = current_pos
             current_pos += 1
         if doctype_found and doctype_pos < html_pos:
             return "html"
         return FAIL
+
+class HeaderChecker(AbstractChecker) :
+    """HeaderChecker
+    Check the presence of a unique <header> tag
+    """
+    def __init__(self) :
+        super().__init__("HeaderChecker", "Header")
+
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
+        """
+        Check the presence of a unique <header> tag in web_page
+
+        Returns
+        -------
+        str :
+            return "present" if valid else "échec"
+        """
+        return PRESENT if len(web_page.find_all(name="header")) == 1 else FAIL
+
+class FooterChecker(AbstractChecker) :
+    """FooterChecker
+    Check the presence of a unique <footer> tag
+    """
+    def __init__(self) :
+        super().__init__("FooterChecker", "Footer")
+
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
+        """
+        Check the presence of a unique <footer> tag in web_page
+
+        Returns
+        -------
+        str :
+            return "present" if valid else "échec"
+        """
+        return PRESENT if len(web_page.find_all(name="footer")) == 1 else FAIL
+
+class ContactLinkChecker(AbstractChecker) :
+    """ContactLinkChecker
+    Check the presence of a unique <footer> tag
+    """
+    def __init__(self) :
+        super().__init__("ContactLinkChecker", "Lien Contact")
+
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
+        """
+        Check the presence of a unique <footer> tag in web_page
+
+        Returns
+        -------
+        str :
+            return "present" if valid else "échec"
+        """
+        link_tags = web_page.find_all(href=re.compile("(contact|ecrire)"))
+        for tag in link_tags:
+            try :
+                return check_and_correct_url(tag.attrs["href"], root_url)
+            except KeyError :
+                pass
+        return FAIL
```

### Comparing `wasc-0.3.0/src/wasc/utils.py` & `wasc-0.4.0/src/wasc/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,31 +64,33 @@
         The URL of the desired web page
     """
 
     # remove trailing backslash
     target_url = target_url.strip("/")
     root_url = root_url.strip("/")
 
-    # If not truncated
+    # If target startswith "http"
     if target_url.startswith("http") :
         return target_url
 
-    # Else if the root_url end overlap the target_url start
-    target_subpath = target_url.split("/")
-    root_subpath = root_url.split("/")
-    if target_subpath[0] == root_subpath[-1]:
-        return root_url + "/" + "/".join(target_subpath[1:])
-
-    # Else concatenate
-    return root_url + "/" + target_url
+    # If target startswith "www"
+    if target_url.startswith("www") :
+        return root_url.split(":")[0] + "://" + target_url
+
+    # Else find an overlap
+    for i in range(1, min(len(target_url), len(root_url))):
+        if target_url.find(root_url[-i:]) == 0:
+            break
+    # if no overlap, concatenate
+    if i+1 == min(len(target_url), len(root_url)):
+        return root_url + "/" + target_url
+    # else remove overlapping part and concatenate
+    else:
+        return root_url[:-i] + target_url
 
 def find_link(access_tag, root_url):
     while access_tag and access_tag.name != "a" and access_tag.name != "html":
         access_tag = access_tag.parent
     try :
         return check_and_correct_url(access_tag.attrs["href"], root_url)
     except KeyError :
         pass
-
-def report_to_csv(reports, checkers_list):
-    res = []
-    return res
```

### Comparing `wasc-0.3.0/src/wasc/cli/__init__.py` & `wasc-0.4.0/src/wasc/cli/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 import sys
 
 import bs4
 import click
 import pandas as pd
 import requests
 from tqdm import tqdm
+from trafilatura.downloads import add_to_compressed_dict, buffered_downloads, load_download_buffer
 
 from wasc.__about__ import __version__
 from wasc.checker_factory import checker_factory
 from wasc.utils import HEADER, read_checkers, read_websites
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
-DEFAULT_CHECKERS = ["AccessChecker", "AccessLinkChecker", "DoctypeChecker", "LangChecker", "LegalChecker"]
+DEFAULT_CHECKERS = [
+    "AccessChecker", "AccessLinkChecker", "AccessRateChecker",
+    "DoctypeChecker", "LangChecker", "LegalChecker",
+    "ContactLinkChecker"
+]
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("websites", type=click.Path(exists=True))
 @click.option("-c", "--checkers", type=click.Path(exists=True),
               help="Checkers list to use")
-@click.option("-o", "--output", default=sys.stdout,
-              type=click.File("w"),
-              help="Output file [default=stdout]")
 @click.option("-f", "--output_format", default = "json",
               type=click.Choice(["json", "csv"], case_sensitive=False),
               help="Output format [default=json]")
+@click.option("-o", "--output", default=sys.stdout,
+              type=click.File("w"),
+              help="Output file [default=stdout]")
 @click.version_option(version=__version__, prog_name="wasc")
 def wasc(websites, checkers, output, output_format):
     """
     Websites Accessibility Criteria Checker,
     helps to evaluate accessibility criteria on a list of websites
 
     WEBSITES is a CSV file containing a list of websites as couples
@@ -46,32 +51,59 @@
     checkers_list = [checker_factory.create(checker_name) for checker_name in checker_names]
 
     # Sets column names for DataFrame using checkers descriptions
     column_names = ["Organisation", "URL", "Erreur"] + [checker.description for checker in checkers_list]
 
     # Reads the list of web sites
     websites = read_websites(websites)
+    websites_dict = dict(zip([ws[1].strip("/") for ws in websites], [ws[0] for ws in websites]))
+    url_list = [ws[1] for ws in websites]
 
     # Launch analysis
     click.echo(f"Analysis of {len(websites)} websites...")
+    threads = 8
+    dl_dict = add_to_compressed_dict(url_list)
+    mybuffer, dl_dict = load_download_buffer(dl_dict)
     results = []
-    for i in tqdm(range(len(websites))):
-        label, url = websites[i]
-        bs_obj, error = "", ""
-        try:
-            response = requests.get(url, headers=HEADER, timeout = 1)
-            if response.status_code == requests.codes.ok :
-                bs_obj = bs4.BeautifulSoup(response.content, "html.parser")
+    with tqdm(total=len(url_list)) as pbar:
+        for url, response in buffered_downloads(mybuffer, threads, decode=False):
+            label = websites_dict[url.strip("/")]
+            bs_obj = None
+            error = ""
+            if response:
+                if response.status == 200 :
+                    bs_obj = bs4.BeautifulSoup(response.data, "html.parser")
+                else:
+                    error = "HTML Error Status " + str(response.status)
             else:
-                error = "HTML Error Status " + str(response.status_code)
-        except Exception as e:
-            error = str(e)
-        starter = [label, url, error]
-        analysis = [checker.execute(bs_obj, url) if bs_obj else "" for checker in checkers_list]
-        results.append(starter + analysis)
+                error = "Problème lors du téléchargement"
+            starter = [label, url, error]
+            analysis = ["échec" for _ in checkers_list]
+            if not error:
+                analysis = [checker.execute(bs_obj, url) if bs_obj else "" for checker in checkers_list]
+            results.append(starter + analysis)
+            pbar.update(1)
+    # results = []
+    # for i in tqdm(range(len(websites))):
+    #     label, url = websites[i]
+    #     bs_obj = None
+    #     error = ""
+    #     try:
+    #         response = requests.get(url, headers=HEADER, timeout = 1)
+    #         if response.status_code == requests.codes.ok :
+    #             bs_obj = bs4.BeautifulSoup(response.content, "html.parser")
+    #         else:
+    #             error = "HTML Error Status " + str(response.status_code)
+    #     except Exception as e:
+    #         error = str(e)
+    #     starter = [label, url, error]
+    #     analysis = ["échec" for _ in checkers_list]
+    #     if not error:
+    #         analysis = [checker.execute(bs_obj, url) if bs_obj else "" for checker in checkers_list]
+    #     results.append(starter + analysis)
 
     # Creates the DataFrame from results
     df = pd.DataFrame(results, columns=column_names)
     df.set_index(["Organisation"], inplace=True)
 
     # Output results given -o output and -f output_format
     if output == sys.stdout:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wasc-0.3.0/tests/test_checker.py` & `wasc-0.4.0/tests/test_checker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-
+# SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
+#
+# SPDX-License-Identifier: CECILL-2.1
 from bs4 import BeautifulSoup
 
-import wasc.default_checkers as dft
+import wasc.checkers as dft
 
 BS_PARSER = "html.parser"
-FAIL = "échec"
 
-DEFAULT_HTML_HEAD = "<!DOCTYPE html><html><body><div>"
+DEFAULT_HTML_HEAD = "<!DOCTYPE html><html><head></head><body><div>"
 DEFAULT_HTML_TAIL = "</div></body></html>"
 DEFAULT_HTML_ROOT = "https://www.example.com"
+
 class TestDoctypeChecker:
     def test_doctype_checker_init(self):
         doctype_checker = dft.DoctypeChecker()
         assert doctype_checker.name == "DoctypeChecker"
         assert doctype_checker.description == "Doctype"
 
     def test_doctype_checker_valid(self):
@@ -21,21 +23,21 @@
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert doctype_checker.execute(basic_webpage, "") == "html"
 
     def test_doctype_checker_bad_doctype(self):
         test_html = "<!DOCTYPE notvalid><html></html>"
         doctype_checker = dft.DoctypeChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert doctype_checker.execute(basic_webpage, "") == FAIL
+        assert doctype_checker.execute(basic_webpage, "") == dft.FAIL
 
     def test_doctype_checker_no_doctype(self):
         test_html = "<html></html>"
         doctype_checker = dft.DoctypeChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert doctype_checker.execute(basic_webpage, "") == FAIL
+        assert doctype_checker.execute(basic_webpage, "") == dft.FAIL
 
 class TestLangChecker:
     def test_lang_checker_init(self):
         lang_checker = dft.LangChecker()
         assert lang_checker.name == "LangChecker"
         assert lang_checker.description == "Lang"
 
@@ -45,33 +47,33 @@
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert lang_checker.execute(basic_webpage, "") == "fr"
 
     def test_lang_checker_empty(self):
         test_html = "<!DOCTYPE html><html></html>"
         lang_checker = dft.LangChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert lang_checker.execute(basic_webpage, "") == FAIL
+        assert lang_checker.execute(basic_webpage, "") == dft.FAIL
 
 class TestAccessChecker:
     def test_access_checker_init(self):
         access_checker = dft.AccessChecker()
         assert access_checker.name == "AccessChecker"
         assert access_checker.description == "Mention accessibilité"
 
     def test_access_checker_fail1(self):
         test_html = DEFAULT_HTML_HEAD + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_checker.execute(basic_webpage, "") == FAIL
+        assert access_checker.execute(basic_webpage, "") == dft.FAIL
 
     def test_access_checker_fail2(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : conforme partiellement" + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_checker.execute(basic_webpage, "") == FAIL
+        assert access_checker.execute(basic_webpage, "") == dft.FAIL
 
     def test_access_checker_valid_non(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : non conforme" + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert access_checker.execute(basic_webpage, "") == "non conforme"
 
@@ -90,44 +92,82 @@
 class TestAccessLinkChecker:
     def test_access_link_checker_init(self):
         access_link_checker = dft.AccessLinkChecker()
         assert access_link_checker.name == "AccessLinkChecker"
         assert access_link_checker.description == "Lien accessibilité"
 
     def test_access_link_checker_valid_mention(self):
-        test_link = '<a href="/misc/accessibilite/">Accessibilité : totalement conforme</a>'
+        test_link = '<a href="/accessibilite/">Accessibilité : non conforme</a>'
         test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        answer = DEFAULT_HTML_ROOT + "/misc/accessibilite"
+        answer = DEFAULT_HTML_ROOT + "/accessibilite"
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_access_link_checker_fail_mention(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : totalement conforme" + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
 
     def test_access_link_checker_valid_other(self):
         test_html = DEFAULT_HTML_HEAD + '<a href="/accessibilite/">Accessibilité</a>' + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == DEFAULT_HTML_ROOT + "/accessibilite"
 
     def test_access_link_checker_fail_other(self):
         test_html = DEFAULT_HTML_HEAD + '<a href="/misc/accessibilite/">Accessibilité</a>' + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
+        answer = DEFAULT_HTML_ROOT + "/misc/accessibilite"
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_access_link_checker_fail_href(self):
         test_html = DEFAULT_HTML_HEAD + "<a>Accessibilité</a>" + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+
+    def test_access_link_checker_decla(self):
+        test_link = '<a href="/misc/accessibilite/">Déclaration d\'accessibilité</a>'
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        access_link_checker = dft.AccessLinkChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = DEFAULT_HTML_ROOT + "/misc/accessibilite"
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+
+class TestAccessRateChecker:
+    def test_access_rate_checker_init(self):
+        access_rate_checker = dft.AccessRateChecker()
+        assert access_rate_checker.name == "AccessRateChecker"
+        assert access_rate_checker.description == "Taux d'accessibilité"
+
+    def test_access_rate_checker_valid(self):
+        """
+        Be Careful, this test use a real url that may change over time
+        """
+        test_link = '<a href="/misc/accessibilite/">Accessibilité : totalement conforme</a>'
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        access_rate_checker = dft.AccessRateChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert access_rate_checker.execute(basic_webpage, "https://design.numerique.gouv.fr") == "100%"
+
+    def test_access_rate_checker_fail_link(self):
+        test_html = DEFAULT_HTML_HEAD + "Accessibilité : non conforme" + DEFAULT_HTML_TAIL
+        access_rate_checker = dft.AccessRateChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+
+    def test_access_rate_checker_fail_link2(self):
+        test_link = '<a href="/misc/accessibilite/">Accessibilité : totalement conforme</a>'
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        access_rate_checker = dft.AccessRateChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
 
 class TestLegalChecker:
     def test_mention_legales_checker_init(self):
         mention_legales_checker = dft.LegalChecker()
         assert mention_legales_checker.name == "LegalChecker"
         assert mention_legales_checker.description == "Mentions légales"
 
@@ -145,15 +185,106 @@
         answer = DEFAULT_HTML_ROOT + "/misc/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_mention_legales_fail_mention(self):
         test_html = DEFAULT_HTML_HEAD + "Mentions légales" + DEFAULT_HTML_TAIL
         mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
+        assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
 
     def test_mention_legales_valid_dftlink(self):
         test_html = DEFAULT_HTML_HEAD + "foo" + DEFAULT_HTML_TAIL
         mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = "https://www.gouvernement.fr/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, "https://www.gouvernement.fr/") == answer
+
+class TestHeadNbChecker:
+    def test_head_nb_checker_init(self):
+        head_nb_checker = dft.HeadNbChecker()
+        assert head_nb_checker.name == "HeadNbChecker"
+        assert head_nb_checker.description == "Nombre de <head>"
+    def test_head_nb_valid_01(self):
+        test_html = DEFAULT_HTML_HEAD + DEFAULT_HTML_TAIL
+        head_nb_checker = dft.HeadNbChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = 1
+        assert head_nb_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+    def test_head_nb_valid_02(self):
+        test_html = DEFAULT_HTML_HEAD + "<head></head>" + DEFAULT_HTML_TAIL
+        head_nb_checker = dft.HeadNbChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = 2
+        assert head_nb_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+    def test_head_nb_fail(self):
+        test_html = "<!DOCTYPE html><html><body></body></html>"
+        head_nb_checker = dft.HeadNbChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = 0
+        assert head_nb_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+
+class TestHeadLvlChecker:
+    def test_head_lvl_checker_init(self):
+        head_lvl_checker = dft.HeadLvlChecker()
+        assert head_lvl_checker.name == "HeadLvlChecker"
+        assert head_lvl_checker.description == "Profondeurs des <head>"
+    def test_head_lvl_valid_01(self):
+        test_html = DEFAULT_HTML_HEAD + DEFAULT_HTML_TAIL
+        head_lvl_checker = dft.HeadLvlChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = [1]
+        assert head_lvl_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+    def test_head_lvl_valid_02(self):
+        test_html = DEFAULT_HTML_HEAD + "<head></head>" + DEFAULT_HTML_TAIL
+        head_lvl_checker = dft.HeadLvlChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = [1,3]
+        assert head_lvl_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+    def test_head_lvl_fail(self):
+        test_html = "<!DOCTYPE html><html><body></body></html>"
+        head_lvl_checker = dft.HeadLvlChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        answer = []
+        assert head_lvl_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
+
+class TestHeaderChecker:
+    def test_header_checker_init(self):
+        header_checker = dft.HeaderChecker()
+        assert header_checker.name == "HeaderChecker"
+        assert header_checker.description == "Header"
+
+    def test_header_checker_fail(self):
+        test_html = "<!DOCTYPE html><html><body></body></html>"
+        header_checker = dft.HeaderChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+
+    def test_header_checker_present(self):
+        test_html = "<!DOCTYPE html><html><body><header></header></body></html>"
+        header_checker = dft.HeaderChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.PRESENT
+
+class TestFooterChecker:
+    def test_footer_checker_init(self):
+        footer_checker = dft.FooterChecker()
+        assert footer_checker.name == "FooterChecker"
+        assert footer_checker.description == "Footer"
+
+    def test_footer_checker_fail(self):
+        test_html = "<!DOCTYPE html><html><body></body></html>"
+        footer_checker = dft.FooterChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+
+    def test_footer_checker_present(self):
+        test_html = "<!DOCTYPE html><html><body><footer></footer></body></html>"
+        footer_checker = dft.FooterChecker()
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.PRESENT
+
+class TestContactLinkChecker:
+    def test_contact_link_checker_init(self):
+        contact_link_checker = dft.ContactLinkChecker()
+        assert contact_link_checker.name == "ContactLinkChecker"
+        assert contact_link_checker.description == "Lien Contact"
+
```

### Comparing `wasc-0.3.0/tests/test_checker_factory.py` & `wasc-0.4.0/tests/test_checker_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
+#
+# SPDX-License-Identifier: CECILL-2.1
 import wasc.checker_factory as fact
 
 FAIL = "échec"
 class TmpChecker:
     pass
 
 class TestCheckerFactory:
@@ -18,16 +21,7 @@
         tmp_obj = tmp_factory.create("tmp_name")
         assert isinstance(tmp_obj, TmpChecker)
     def test_checker_factory_available(self):
         tmp_factory = fact.CheckerFactory()
         tmp_factory.register("tmp_name", TmpChecker)
         check_list = tmp_factory.available()
         assert check_list == ["tmp_name"]
-    def test_default_checkers(self):
-        expected_list = {
-            "DFTT01", "DFTT02",
-            "AccessChecker", "AccessLinkChecker", "AccessRateChecker",
-            "LegalChecker", "LangChecker", "DoctypeChecker"
-        }
-        default_factory = fact.checker_factory
-        check_list = default_factory.available()
-        assert set(check_list) == expected_list
```

### Comparing `wasc-0.3.0/tests/test_utils.py` & `wasc-0.4.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+# SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
+#
+# SPDX-License-Identifier: CECILL-2.1
 import pytest
 
 from wasc import utils
 
 
 class TestReadCheckers:
     def test_no_file(self):
         with pytest.raises(FileNotFoundError):
             utils.read_checkers("foo.txt")
     def test_read_crit_example(self):
         expected_checkers = {
-            "DFTT01", "DFTT02",
+            "HeadNbChecker", "HeadLvlChecker",
             "AccessChecker", "AccessLinkChecker", "AccessRateChecker",
             "LegalChecker", "LangChecker", "DoctypeChecker"
         }
         read_checkers = utils.read_checkers("tests/data/checkers_example.csv")
         assert isinstance(read_checkers, list)
         assert set(read_checkers) == expected_checkers
```

### Comparing `wasc-0.3.0/LICENSE.txt` & `wasc-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wasc-0.3.0/README.md` & `wasc-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,45 +6,73 @@
 -----
 
 **Table of Contents**
 
 - [Web Accessibility Simple Checker](#web-accessibility-simple-checker)
   - [](#)
   - [Installation](#installation)
+  - [Usage](#usage)
+  - [Documentation](#documentation)
   - [License](#license)
   - [Developpement](#developpement)
     - [Dependencies](#dependencies)
     - [Running wasc with hatch](#running-wasc-with-hatch)
     - [Testing wasc with hatch](#testing-wasc-with-hatch)
 
 ## Installation
 
 ```console
 pip install wasc
 ```
+## Usage
 
+```bash
+Usage: wasc [OPTIONS] WEBSITES
+
+  Websites Accessibility Criteria Checker, helps to 
+  evaluate accessibility on a list of websites
+
+  WEBSITES is a CSV file containing a list of websites 
+  as couples "label";"URL"
+
+Options:
+  -c, --checkers PATH             Path to the list of checkers
+  -f, --output_format [json|csv]  Output format [default=json]
+  -o, --output FILENAME           Output file [default=stdout]
+  --version                       Show the version and exit.
+  -h, --help                      Show this message and exit.
+```
+
+Example files are given in `data` directory
+
+## Documentation
+
+Documentation is available [here](https://atelierpartage.github.io/wasc/)
 ## License
 
 `wasc` is distributed under the terms of the [CECILL-2.1](https://spdx.org/licenses/CECILL-2.1.html) license by the following licensors :
 * Juliette Francis
 * François le Berre
 * Guillaume Collet
 
 `wasc` main contact is [contact@latelierpartage.fr](mailto:contact@latelierpartage.fr)
 
 For details about the license, see file [LICENSE.txt](https://github.com/atelierPartage/wasc/blob/main/LICENSE.txt)
+
 ## Developpement
 
 Full source code is available on github : [https://github.com/gcollet/wasc](https://github.com/gcollet/wasc)
 The project is developed under hatch project manager ([hatch.pypa.io](https://hatch.pypa.io/latest/))
 
 ### Dependencies
 `hatch` project manager is mandatory. The other dependencies are managed with hatch environment system.
 
 It is **not necessary** to install dependencies using `pip install -r requirements_dev.txt` but the file is present if needed.
 ### Running wasc with hatch
 In `wasc` directory, use hatch to run wasc in the default environnement :
+
 `hatch run wasc data/url_example.csv`
 
 ### Testing wasc with hatch
 In `wasc` directory, use hatch to test wasc files in the default environnement :
-`hatch run test test_all`
+
+`hatch run test_all`
```

### Comparing `wasc-0.3.0/pyproject.toml` & `wasc-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "click",
   "beautifulsoup4",
-  "requests",
   "tqdm",
-  "pandas"
+  "pandas",
+  "trafilatura"
 ]
 
 [project.urls]
 Documentation = "https://github.com/gcollet/wasc#readme"
 Issues = "https://github.com/gcollet/wasc/issues"
 Source = "https://github.com/gcollet/wasc"
```

### Comparing `wasc-0.3.0/PKG-INFO` & `wasc-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Web Accessibility Simple Checker
 Project-URL: Documentation, https://github.com/gcollet/wasc#readme
 Project-URL: Issues, https://github.com/gcollet/wasc/issues
 Project-URL: Source, https://github.com/gcollet/wasc
 Author-email: Guillaume Collet <bilouweb@free.fr>, Juliette Francis <juliette.francis@etudiant.univ-rennes.fr>
 License-Expression: CECILL-2.1
 License-File: LICENSE.txt
@@ -18,61 +18,89 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
 Requires-Dist: click
 Requires-Dist: pandas
-Requires-Dist: requests
 Requires-Dist: tqdm
+Requires-Dist: trafilatura
 Description-Content-Type: text/markdown
 
 # Web Accessibility Simple Checker
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wasc.svg)](https://pypi.org/project/wasc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wasc.svg)](https://pypi.org/project/wasc)
 [![Docs](https://github.com/atelierPartage/wasc/actions/workflows/docs.yml/badge.svg)](https://github.com/atelierPartage/wasc/actions/workflows/docs.yml)
 -----
 
 **Table of Contents**
 
 - [Web Accessibility Simple Checker](#web-accessibility-simple-checker)
   - [](#)
   - [Installation](#installation)
+  - [Usage](#usage)
+  - [Documentation](#documentation)
   - [License](#license)
   - [Developpement](#developpement)
     - [Dependencies](#dependencies)
     - [Running wasc with hatch](#running-wasc-with-hatch)
     - [Testing wasc with hatch](#testing-wasc-with-hatch)
 
 ## Installation
 
 ```console
 pip install wasc
 ```
+## Usage
 
+```bash
+Usage: wasc [OPTIONS] WEBSITES
+
+  Websites Accessibility Criteria Checker, helps to 
+  evaluate accessibility on a list of websites
+
+  WEBSITES is a CSV file containing a list of websites 
+  as couples "label";"URL"
+
+Options:
+  -c, --checkers PATH             Path to the list of checkers
+  -f, --output_format [json|csv]  Output format [default=json]
+  -o, --output FILENAME           Output file [default=stdout]
+  --version                       Show the version and exit.
+  -h, --help                      Show this message and exit.
+```
+
+Example files are given in `data` directory
+
+## Documentation
+
+Documentation is available [here](https://atelierpartage.github.io/wasc/)
 ## License
 
 `wasc` is distributed under the terms of the [CECILL-2.1](https://spdx.org/licenses/CECILL-2.1.html) license by the following licensors :
 * Juliette Francis
 * François le Berre
 * Guillaume Collet
 
 `wasc` main contact is [contact@latelierpartage.fr](mailto:contact@latelierpartage.fr)
 
 For details about the license, see file [LICENSE.txt](https://github.com/atelierPartage/wasc/blob/main/LICENSE.txt)
+
 ## Developpement
 
 Full source code is available on github : [https://github.com/gcollet/wasc](https://github.com/gcollet/wasc)
 The project is developed under hatch project manager ([hatch.pypa.io](https://hatch.pypa.io/latest/))
 
 ### Dependencies
 `hatch` project manager is mandatory. The other dependencies are managed with hatch environment system.
 
 It is **not necessary** to install dependencies using `pip install -r requirements_dev.txt` but the file is present if needed.
 ### Running wasc with hatch
 In `wasc` directory, use hatch to run wasc in the default environnement :
+
 `hatch run wasc data/url_example.csv`
 
 ### Testing wasc with hatch
 In `wasc` directory, use hatch to test wasc files in the default environnement :
-`hatch run test test_all`
+
+`hatch run test_all`
```

