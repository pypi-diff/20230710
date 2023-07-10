# Comparing `tmp/arch_github_package-0.0.6.tar.gz` & `tmp/arch_github_package-0.0.7.tar.gz`

## Comparing `arch_github_package-0.0.6.tar` & `arch_github_package-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/arch_github_package/__init__.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/arch_github_package/gh.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/arch_github_package/main.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/arch_github_package/pm.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/arch_github_package/state.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/README.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 arch_github_package-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/arch_github_package/__init__.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/arch_github_package/gh.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/arch_github_package/main.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/arch_github_package/pm.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/arch_github_package/state.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/README.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 arch_github_package-0.0.7/PKG-INFO
```

### Comparing `arch_github_package-0.0.6/arch_github_package/gh.py` & `arch_github_package-0.0.7/arch_github_package/gh.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/arch_github_package/main.py` & `arch_github_package-0.0.7/arch_github_package/main.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/arch_github_package/pm.py` & `arch_github_package-0.0.7/arch_github_package/pm.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 import typer
 
 
 class Pkgbuild:
     def __init__(self, repo, project_name, project_description, version):
         self.repo = repo
         self.pkgname = project_name + "-github"
-        self.pkgdesc = project_description.replace("'", "\\'")
+        for i in '"`$':
+            project_description = project_description.replace(i, "\\"+i)
+        self.pkgdesc = project_description
         self.pkgver = version
         self.build_dir = Path(tempfile.mkdtemp(prefix="pkgbuild-"+self.pkgname+"-"))
         self.maintainer = "arch-github-package <https://github.com/jinliu/arch-github-package>"
 
     def get_build_dir(self):
         return self.build_dir
     
     def create_pkgbuild(self, tarball_name, sha256sum):
         pkgbuild = \
 f"""# Maintainer: {self.maintainer}
 pkgname={self.pkgname}
 pkgver={self.pkgver}
 pkgrel=1
-pkgdesc='{self.pkgdesc}'
+pkgdesc="{self.pkgdesc}"
 arch=('x86_64')
 url="https://github.com/{self.repo}"
 license=('custom')
 source=({tarball_name})
 sha256sums=('{sha256sum}')
 package() {{
 """
```

### Comparing `arch_github_package-0.0.6/arch_github_package/state.py` & `arch_github_package-0.0.7/arch_github_package/state.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/.gitignore` & `arch_github_package-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/LICENSE` & `arch_github_package-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/README.md` & `arch_github_package-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.6/pyproject.toml` & `arch_github_package-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arch-github-package"
-version = "0.0.6"
+version = "0.0.7"
 description = "Convert GitHub project releases to Archlinux package, with autoupdate."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   { name="Jin Liu", email="m.liu.jin@gmail.com" },
 ]
 keywords = ["arch", "archlinux", "AUR", "github", "package", "package-manager"]
```

### Comparing `arch_github_package-0.0.6/PKG-INFO` & `arch_github_package-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-github-package
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert GitHub project releases to Archlinux package, with autoupdate.
 Project-URL: Repository, https://github.com/jinliu/arch-github-package
 Project-URL: Bug Tracker, https://github.com/jinliu/arch-github-package/issues
 Author-email: Jin Liu <m.liu.jin@gmail.com>
 License-File: LICENSE
 Keywords: AUR,arch,archlinux,github,package,package-manager
 Classifier: Development Status :: 2 - Pre-Alpha
```

