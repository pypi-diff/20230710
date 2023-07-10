# Comparing `tmp/secureli-0.6.8.tar.gz` & `tmp/secureli-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.6.8.tar", max compression
+gzip compressed data, was "secureli-0.6.9.tar", max compression
```

## Comparing `secureli-0.6.8.tar` & `secureli-0.6.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11343 2023-07-10 18:40:57.045127 secureli-0.6.8/LICENSE
--rw-r--r--   0        0        0    11614 2023-07-10 18:40:57.045127 secureli-0.6.8/README.md
--rw-r--r--   0        0        0     2043 2023-07-10 18:40:57.049127 secureli-0.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0     6906 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10672 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/actions/update.py
--rw-r--r--   0        0        0     6450 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/main.py
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0     1271 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      748 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      619 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1363 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      437 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0     1349 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0    12318 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/language_config.py
--rw-r--r--   0        0        0    16779 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/language_support.py
--rw-r--r--   0        0        0     4479 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0      254 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/hash.py
--rw-r--r--   0        0        0     1372 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-07-10 18:40:57.049127 secureli-0.6.8/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-10 20:30:46.617324 secureli-0.6.9/LICENSE
+-rw-r--r--   0        0        0    11614 2023-07-10 20:30:46.617324 secureli-0.6.9/README.md
+-rw-r--r--   0        0        0     2043 2023-07-10 20:30:46.617324 secureli-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    11925 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/update.py
+-rw-r--r--   0        0        0     6450 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     3632 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0     1271 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      748 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      619 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1363 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      437 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0     1349 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_config.py
+-rw-r--r--   0        0        0    16779 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4545 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3048 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.9/PKG-INFO
```

### Comparing `secureli-0.6.8/LICENSE` & `secureli-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/README.md` & `secureli-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/pyproject.toml` & `secureli-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.6.8"
+version = "0.6.9"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.6.8/secureli/abstractions/echo.py` & `secureli-0.6.9/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/abstractions/lexer_guesser.py` & `secureli-0.6.9/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/abstractions/pre_commit.py` & `secureli-0.6.9/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/actions/action.py` & `secureli-0.6.9/secureli/actions/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from secureli.abstractions.echo import EchoAbstraction, Color
 from secureli.abstractions.pre_commit import (
     InstallFailedError,
 )
 from secureli.repositories.secureli_config import (
     SecureliConfig,
     SecureliConfigRepository,
+    VerifyConfigOutcome,
 )
 from secureli.services.language_analyzer import LanguageAnalyzerService, AnalyzeResult
 from secureli.services.language_support import LanguageSupportService
 from secureli.services.scanner import ScannerService, ScanMode
 from secureli.services.updater import UpdaterService
 from secureli.services.language_config import LanguageNotSupportedError
 
@@ -80,41 +81,49 @@
         """
         Installs, upgrades or verifies the current SeCureLI installation
         :param folder_path: The folder path to initialize the repo for
         :param reset: If true, disregard existing configuration and start fresh
         :param always_yes: Assume "Yes" to all prompts
         """
 
+        if self.action_deps.secureli_config.verify() == VerifyConfigOutcome.OUT_OF_DATE:
+            update_config = self._update_secureli_config_only(always_yes)
+            if update_config.outcome != VerifyOutcome.UPDATE_SUCCEEDED:
+                self.action_deps.echo.error(f"SeCureLI could not be verified.")
+                return VerifyResult(
+                    outcome=update_config.outcome,
+                )
+
         config = SecureliConfig() if reset else self.action_deps.secureli_config.load()
 
-        if not config.overall_language or not config.version_installed:
+        if not config.languages or not config.version_installed:
             return self._install_secureli(folder_path, always_yes)
         else:
             available_version = self.action_deps.language_support.version_for_language(
-                config.overall_language
+                config.languages[0]
             )
 
             # Check for a new version and prompt for upgrade if available
             if available_version != config.version_installed:
                 return self._upgrade_secureli(config, available_version, always_yes)
 
             # Validates the current .pre-commit-config.yaml against the generated config
             config_validation_result = (
                 self.action_deps.language_support.validate_config(
-                    language=config.overall_language
+                    language=config.languages[0]
                 )
             )
 
             # If config mismatch between available version and current version prompt for upgrade
             if not config_validation_result.successful:
                 self.action_deps.echo.print(config_validation_result.output)
                 return self._update_secureli(always_yes)
 
             self.action_deps.echo.print(
-                f"SeCureLI is installed and up-to-date (language = {config.overall_language})"
+                f"SeCureLI is installed and up-to-date (language = {config.languages[0]})"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.UP_TO_DATE,
                 config=config,
             )
 
     def _upgrade_secureli(
@@ -139,15 +148,15 @@
             return VerifyResult(
                 outcome=VerifyOutcome.UPGRADE_CANCELED,
                 config=config,
             )
 
         try:
             metadata = self.action_deps.language_support.apply_support(
-                config.overall_language
+                config.languages[0]
             )
 
             # Update config with new version installed and save it
             config.version_installed = metadata.version
             self.action_deps.secureli_config.save(config)
             self.action_deps.echo.print("SeCureLI has been upgraded successfully")
             return VerifyResult(
@@ -195,49 +204,51 @@
                 raise ValueError("No supported languages found in current repository")
 
             self.action_deps.echo.print("Detected the following languages:")
             for language, percentage in analyze_result.language_proportions.items():
                 self.action_deps.echo.print(
                     f"- {language}: {percentage:.0%}", color=Color.MAGENTA, bold=True
                 )
-            overall_language = list(analyze_result.language_proportions.keys())[0]
+            overall_language = list(analyze_result.language_proportions.keys())
             self.action_deps.echo.print(
-                f"Overall Detected Language: {overall_language}"
+                f"Overall Detected Language: {overall_language[0]}"
             )
 
-            metadata = self.action_deps.language_support.apply_support(overall_language)
+            metadata = self.action_deps.language_support.apply_support(
+                overall_language[0]
+            )
 
         except (ValueError, LanguageNotSupportedError, InstallFailedError) as e:
             self.action_deps.echo.error(
                 f"SeCureLI could not be installed due to an error: {str(e)}"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.INSTALL_FAILED,
             )
 
         config = SecureliConfig(
-            overall_language=overall_language,
+            languages=overall_language,
             version_installed=metadata.version,
         )
         self.action_deps.secureli_config.save(config)
 
         if secret_test_id := metadata.security_hook_id:
             self.action_deps.echo.print(
-                f"{config.overall_language} supports secrets detection; running {secret_test_id}."
+                f"{config.languages[0]} supports secrets detection; running {secret_test_id}."
             )
             self.action_deps.scanner.scan_repo(
                 ScanMode.ALL_FILES, specific_test=secret_test_id
             )
         else:
             self.action_deps.echo.warning(
-                f"{config.overall_language} does not support secrets detection, skipping"
+                f"{config.languages[0]} does not support secrets detection, skipping"
             )
 
         self.action_deps.echo.print(
-            f"SeCureLI has been installed successfully (language = {config.overall_language})"
+            f"SeCureLI has been installed successfully (language = {config.languages[0]})"
         )
 
         return VerifyResult(
             outcome=VerifyOutcome.INSTALL_SUCCEEDED,
             config=config,
             analyze_result=analyze_result,
         )
@@ -263,7 +274,27 @@
         details = update_result.output
         self.action_deps.echo.print(details)
 
         if update_result.successful:
             return VerifyResult(outcome=VerifyOutcome.UPDATE_SUCCEEDED)
         else:
             return VerifyResult(outcome=VerifyOutcome.UPDATE_FAILED)
+
+    def _update_secureli_config_only(self, always_yes: bool) -> VerifyResult:
+        self.action_deps.echo.print("SeCureLI is using an out-of-date config.")
+        response = always_yes or self.action_deps.echo.confirm(
+            "Update config only now?",
+            default_response=True,
+        )
+        if not response:
+            self.action_deps.echo.error("User canceled update process")
+            return VerifyResult(
+                outcome=VerifyOutcome.UPDATE_CANCELED,
+            )
+
+        try:
+            updated_config = self.action_deps.secureli_config.update()
+            self.action_deps.secureli_config.save(updated_config)
+
+            return VerifyResult(outcome=VerifyOutcome.UPDATE_SUCCEEDED)
+        except:
+            return VerifyResult(outcome=VerifyOutcome.UPDATE_FAILED)
```

### Comparing `secureli-0.6.8/secureli/actions/build.py` & `secureli-0.6.9/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/actions/initializer.py` & `secureli-0.6.9/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/actions/scan.py` & `secureli-0.6.9/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/actions/setup.py` & `secureli-0.6.9/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/actions/update.py` & `secureli-0.6.9/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/container.py` & `secureli-0.6.9/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/main.py` & `secureli-0.6.9/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/repositories/repo_files.py` & `secureli-0.6.9/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/repositories/settings.py` & `secureli-0.6.9/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/build.txt` & `secureli-0.6.9/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/go-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/go-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.6.9/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/read_resource.py` & `secureli-0.6.9/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/resources/slugify.py` & `secureli-0.6.9/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/git_ignore.py` & `secureli-0.6.9/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/language_analyzer.py` & `secureli-0.6.9/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/language_config.py` & `secureli-0.6.9/secureli/services/language_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/language_support.py` & `secureli-0.6.9/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/logging.py` & `secureli-0.6.9/secureli/services/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,23 +75,25 @@
     def success(self, action: LogAction) -> LogEntry:
         """
         Capture that a successful conclusion has been reached for an action
         :param action: The action that succeeded
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
-            self.language_support.get_configuration(secureli_config.overall_language)
-            if secureli_config.overall_language
+            self.language_support.get_configuration(secureli_config.languages[0])
+            if secureli_config.languages
             else None
         )
         log_entry = LogEntry(
             status=LogStatus.success,
             action=action,
             hook_config=hook_config,
-            primary_language=secureli_config.overall_language,
+            primary_language=secureli_config.languages[0]
+            if secureli_config.languages
+            else None,
         )
         self._log(log_entry)
 
         return log_entry
 
     def failure(
         self,
@@ -104,29 +106,29 @@
         Capture a failure against an action, with details
         :param action: The action that failed
         :param details: Details about the failure
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
             None
-            if not secureli_config.overall_language
-            else self.language_support.get_configuration(
-                secureli_config.overall_language
-            )
+            if not secureli_config.languages
+            else self.language_support.get_configuration(secureli_config.languages[0])
         )
         log_entry = LogEntry(
             status=LogStatus.failure,
             action=action,
             failure=LogFailure(
                 details=details,
             ),
             total_failure_count=total_failure_count,
             failure_count_details=individual_failure_count,
             hook_config=hook_config,
-            primary_language=secureli_config.overall_language,
+            primary_language=secureli_config.languages[0]
+            if secureli_config.languages
+            else None,
         )
         self._log(log_entry)
 
         return log_entry
 
     def _log(self, log_entry: LogEntry):
         """Commit a log entry to the branch log file"""
```

### Comparing `secureli-0.6.8/secureli/services/scanner.py` & `secureli-0.6.9/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/secureli_ignore.py` & `secureli-0.6.9/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/services/updater.py` & `secureli-0.6.9/secureli/services/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,15 @@
     def update(self):
         """
         Updates secureli with the latest local configuration.
         :return: ExecuteResult, indicating success or failure.
         """
         secureli_config = self.config.load()
         output = "Updating .pre-commit-config.yaml...\n"
-        install_result = self.pre_commit.install(
-            language=secureli_config.overall_language
-        )
+        install_result = self.pre_commit.install(language=secureli_config.languages[0])
         if not install_result.successful:
             output += "Failed to update .pre-commit-config.yaml prior to hook install\n"
             return UpdateResult(successful=install_result.successful, output=output)
 
         hook_install_result = self.pre_commit.update()
         output += hook_install_result.output
```

### Comparing `secureli-0.6.8/secureli/settings.py` & `secureli-0.6.9/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/utilities/git_meta.py` & `secureli-0.6.9/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/utilities/patterns.py` & `secureli-0.6.9/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/secureli/utilities/usage_stats.py` & `secureli-0.6.9/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.8/PKG-INFO` & `secureli-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.6.8
+Version: 0.6.9
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

