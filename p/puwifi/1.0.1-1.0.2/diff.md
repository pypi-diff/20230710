# Comparing `tmp/puwifi-1.0.1.tar.gz` & `tmp/puwifi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puwifi-1.0.1.tar", last modified: Mon Jul 10 17:28:55 2023, max compression
+gzip compressed data, was "puwifi-1.0.2.tar", last modified: Mon Jul 10 18:02:36 2023, max compression
```

## Comparing `puwifi-1.0.1.tar` & `puwifi-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:28:55.405964 puwifi-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.1/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:28:55.405964 puwifi-1.0.1/.github/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:28:55.405964 puwifi-1.0.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.1/.github/workflows/pylint.yml
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 15:42:18.000000 puwifi-1.0.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:12:43.000000 puwifi-1.0.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3655 2023-07-10 17:28:55.405964 puwifi-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3047 2023-07-10 17:26:05.000000 puwifi-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:28:55.405964 puwifi-1.0.1/puwifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3655 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 17:28:55.000000 puwifi-1.0.1/puwifi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9143 2023-07-10 17:14:08.000000 puwifi-1.0.1/puwifi.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-10 15:39:31.000000 puwifi-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.1/renovate.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 17:28:55.405964 puwifi-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.2/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/.github/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/workflows/pylint.yml
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.2/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-07-10 18:02:36.755962 puwifi-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3185 2023-07-10 18:00:00.000000 puwifi-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/puwifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-07-10 17:52:26.000000 puwifi-1.0.2/puwifi.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-10 18:01:15.000000 puwifi-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.2/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:02:36.755962 puwifi-1.0.2/setup.cfg
```

### Comparing `puwifi-1.0.1/.github/workflows/codeql-analysis.yml` & `puwifi-1.0.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/.github/workflows/pylint.yml` & `puwifi-1.0.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/.gitignore` & `puwifi-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/.pylintrc` & `puwifi-1.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/LICENSE` & `puwifi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/README.md` & `puwifi-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,95 @@
 # PU-wifi
-A python program written by [@saicharankandukuri](https://github.com/SaicharanKandukuri/puwifi) to keep you device connected to parul university wifi
-![LookingAroundGIF](https://user-images.githubusercontent.com/68287637/146674077-b5b823be-8146-4770-a2e7-7ced5a04843c.gif)
+A python program written by that simulates puwifi authentication request process to keep you device connected to parul university wifi
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
 -->
 
 
 [![CodeQL](https://github.com/SaicharanKandukuri/puwifi/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/SaicharanKandukuri/puwifi/actions/workflows/codeql-analysis.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/saicharankandukuri/puwifi/badge)](https://www.codefactor.io/repository/github/saicharankandukuri/puwifi)
 [![Pylint](https://github.com/SaicharanKandukuri/puwifi/actions/workflows/pylint.yml/badge.svg)](https://github.com/SaicharanKandukuri/puwifi/actions/workflows/pylint.yml)
 
-# Installation
+- supported OS: `Linux`, `Windows`, `MacOS` and `Android` (with `Termux`)
+- supported python versions: `python3.6` and above
+
+
+## Installation
+
+### with `pip`
+
+- make sure you installed `python` and `pip` in your OS
+
+```bash
+pip install puwifi
+```
+
+### Manuall Installation
 - make sure you installed python in your OS
+
 ```bash
 git clone https://github.com/SaicharanKandukuri/puwifi
 cd puwifi
 pip install -r requirements.txt
 ```
-# Usage
+## Usage
 
-### General
+#### General
 
-#### ♾️ Forever login mode `-k`
+##### ♾️ Forever login mode `-k`
 this is what the aim of repo
 
 `-k` or `--keep-alive` attribute is say script to run a forever loop!
 > scripts tries to contact `google.com` if connection fails script tries to send login request to host *i.e: 10.0.0.1* with username & password provied with `-u` & `-p` arguments
 ```cmd
 python3 puwifi.py -k -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
 
-#### 🪵 One-time login `-l`
+##### 🪵 One-time login `-l`
 you can login with `-l` or `--login` argument
 ```cmd
 python3 puwifi.py -l -u YOUR_USERNAME -p YOUR_PASSWORD
 ```
-#### 💥 Logout from puwifi
+##### 💥 Logout from puwifi
 for logout use option `-o` or `--logout` argument
 ```cmd
 python3 puwifi.py -o -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
 <!--
 > idk why logout requires username and password too! ( vunerability ? )
 --> 
 
-![PusheenCatGIF](https://user-images.githubusercontent.com/68287637/146673862-cdb4f86e-c55b-470e-aa3f-b98dd362c6fb.gif)
-###### go watch your videos now
 <hr>
 
-# Finally
+## Finally
 This repo is made fully on self-intrest cause iam a student in parul university, wifi here is `great&fast` but a bit tricky
 ![RepeatJumpGIF](https://user-images.githubusercontent.com/68287637/146674165-5d586b3c-dfce-41d7-8ebe-54917b27fb91.gif)
 
 so instead of playing dino i made this script by re-enginerring an year old puwifi login website & used some of knowledge to make this script happen
 
 ### follow me on
-😺 [github](https://github.com/SaicharanKandukuri), 
-| 🦜 [Twitter](https://twitter.com/AtonZman1x1)
-| 📸 follow me on Instagram: `atonzman1x1`
-| 🎮 Add me on discord: `SAICHARAN KANDUKURI#3741`
+
+- 😺 [github](https://github.com/SaicharanKandukuri), 
+
+- 🦜 [Twitter](https://twitter.com/AtonZman1x1)
+
+- 📸 follow me on Instagram: `atonzman1x1`
+
+- 🎮 Add me on discord: `SAICHARAN KANDUKURI#3741`
 
 🌟 If this work of me helped you make sure you start this repo, or buy me a juice of coffee when we meet 🥤
 
 
 > ⚠️ Dont use practices used in this code for any kind of mischievous things. i need wifi working
+>
+
+![PusheenCatGIF](https://user-images.githubusercontent.com/68287637/146673862-cdb4f86e-c55b-470e-aa3f-b98dd362c6fb.gif)
+###### go watch your videos now
+
 
 <hr>
 
 ###### (©️) MIT License @SaicharanKandukuri
```

### Comparing `puwifi-1.0.1/puwifi.py` & `puwifi-1.0.2/puwifi.py`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.1/pyproject.toml` & `puwifi-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="puwifi"
-version="1.0.1"
+version="1.0.2"
 
 authors = [
     { name="SaicharanKandukuri", email="saicharankandukuri1x1@gmail.com"}
 ]
 
 description = "⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever"
 readme = "README.md"
```

