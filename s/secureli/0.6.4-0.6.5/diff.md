# Comparing `tmp/secureli-0.6.4.tar.gz` & `tmp/secureli-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.6.4.tar", max compression
+gzip compressed data, was "secureli-0.6.5.tar", max compression
```

## Comparing `secureli-0.6.4.tar` & `secureli-0.6.5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0    11343 2023-06-29 20:20:50.106968 secureli-0.6.4/LICENSE
--rw-r--r--   0        0        0    11614 2023-06-29 20:20:50.106968 secureli-0.6.4/README.md
--rw-r--r--   0        0        0     2043 2023-06-29 20:20:50.106968 secureli-0.6.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    34252 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10730 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-29 20:20:50.106968 secureli-0.6.4/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0     1271 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      748 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      619 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1363 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      437 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0     1349 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2275 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/language_support.py
--rw-r--r--   0        0        0     4413 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-06-29 20:20:50.110968 secureli-0.6.4/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-07 19:15:45.529776 secureli-0.6.5/LICENSE
+-rw-r--r--   0        0        0    11614 2023-07-07 19:15:45.529776 secureli-0.6.5/README.md
+-rw-r--r--   0        0        0     2043 2023-07-07 19:15:45.533776 secureli-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10672 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/actions/update.py
+-rw-r--r--   0        0        0     6450 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0     1271 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      748 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      619 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1363 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      437 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0     1349 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/language_config.py
+-rw-r--r--   0        0        0    16779 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4479 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-07 19:15:45.533776 secureli-0.6.5/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.5/PKG-INFO
```

### Comparing `secureli-0.6.4/LICENSE` & `secureli-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/README.md` & `secureli-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/pyproject.toml` & `secureli-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.6.4"
+version = "0.6.5"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.6.4/secureli/abstractions/echo.py` & `secureli-0.6.5/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/abstractions/lexer_guesser.py` & `secureli-0.6.5/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/actions/action.py` & `secureli-0.6.5/secureli/actions/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 from typing import Optional
 
 import pydantic
 
 from secureli.abstractions.echo import EchoAbstraction, Color
 from secureli.abstractions.pre_commit import (
     InstallFailedError,
-    LanguageNotSupportedError,
 )
 from secureli.repositories.secureli_config import (
     SecureliConfig,
     SecureliConfigRepository,
 )
 from secureli.services.language_analyzer import LanguageAnalyzerService, AnalyzeResult
 from secureli.services.language_support import LanguageSupportService
 from secureli.services.scanner import ScannerService, ScanMode
 from secureli.services.updater import UpdaterService
-from secureli.abstractions.pre_commit import PreCommitAbstraction
+from secureli.services.language_config import LanguageNotSupportedError
 
 
 class VerifyOutcome(str, Enum):
     INSTALL_CANCELED = "install-canceled"
     INSTALL_FAILED = "install-failed"
     INSTALL_SUCCEEDED = "install-succeeded"
     UPGRADE_CANCELED = "upgrade-canceled"
@@ -56,23 +55,21 @@
         self,
         echo: EchoAbstraction,
         language_analyzer: LanguageAnalyzerService,
         language_support: LanguageSupportService,
         scanner: ScannerService,
         secureli_config: SecureliConfigRepository,
         updater: UpdaterService,
-        pre_commit: PreCommitAbstraction,
     ):
         self.echo = echo
         self.language_analyzer = language_analyzer
         self.language_support = language_support
         self.scanner = scanner
         self.secureli_config = secureli_config
         self.updater = updater
-        self.pre_commit = pre_commit
 
 
 class Action(ABC):
     """The base Action class for any action that can analyze, install and update SeCureLI's configuration."""
 
     def __init__(self, action_deps: ActionDependencies):
         self.action_deps = action_deps
@@ -97,16 +94,18 @@
             )
 
             # Check for a new version and prompt for upgrade if available
             if available_version != config.version_installed:
                 return self._upgrade_secureli(config, available_version, always_yes)
 
             # Validates the current .pre-commit-config.yaml against the generated config
-            config_validation_result = self.action_deps.pre_commit.validate_config(
-                language=config.overall_language
+            config_validation_result = (
+                self.action_deps.language_support.validate_config(
+                    language=config.overall_language
+                )
             )
 
             # If config mismatch between available version and current version prompt for upgrade
             if not config_validation_result.successful:
                 self.action_deps.echo.print(config_validation_result.output)
                 return self._update_secureli(always_yes)
```

### Comparing `secureli-0.6.4/secureli/actions/build.py` & `secureli-0.6.5/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/actions/initializer.py` & `secureli-0.6.5/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/actions/scan.py` & `secureli-0.6.5/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/actions/setup.py` & `secureli-0.6.5/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/actions/update.py` & `secureli-0.6.5/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/container.py` & `secureli-0.6.5/secureli/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from secureli.services.git_ignore import GitIgnoreService
 from secureli.services.language_analyzer import LanguageAnalyzerService
 from secureli.services.language_support import LanguageSupportService
 from secureli.services.logging import LoggingService
 from secureli.services.scanner import ScannerService
 from secureli.services.updater import UpdaterService
 from secureli.services.secureli_ignore import SecureliIgnoreService
+from secureli.services.language_config import LanguageConfigService
 from secureli.settings import Settings
 
 
 class Container(containers.DeclarativeContainer):
     """
     Arrange various dependencies and instruct the system on how to wire them up.
     """
@@ -77,47 +78,54 @@
     """Guesses the lexer within a given file"""
     lexer_guesser = providers.Factory(PygmentsLexerGuesser)
 
     """Wraps the execution and management of pre-commit in our consuming repo"""
     pre_commit_abstraction = providers.Factory(
         PreCommitAbstraction,
         command_timeout_seconds=config.language_support.command_timeout_seconds,
-        data_loader=read_resource,
-        ignored_file_patterns=secureli_ignored_file_patterns,
-        pre_commit_settings=config.pre_commit,
     )
 
     # Services
 
     """Analyzes a set of files to try to determine the most common languages"""
 
     """
     Manages the repository's git ignore file, making sure secureli-managed
     files are ignored
     """
     git_ignore_service = providers.Factory(GitIgnoreService)
 
+    language_config_service = providers.Factory(
+        LanguageConfigService,
+        data_loader=read_resource,
+        pre_commit_settings=config.pre_commit,
+        command_timeout_seconds=config.language_support.command_timeout_seconds,
+        ignored_file_patterns=secureli_ignored_file_patterns,
+    )
+
     """Identifies the configuration version for the language and installs it"""
     language_support_service = providers.Factory(
         LanguageSupportService,
         pre_commit_hook=pre_commit_abstraction,
         git_ignore=git_ignore_service,
+        language_config=language_config_service,
+        data_loader=read_resource,
     )
 
     """Analyzes a given repo to try to identify the most common language"""
     language_analyzer_service = providers.Factory(
         LanguageAnalyzerService,
         repo_files=repo_files_repository,
         lexer_guesser=lexer_guesser,
     )
 
     """Logs branch-level secureli log entries to the disk"""
     logging_service = providers.Factory(
         LoggingService,
-        pre_commit=pre_commit_abstraction,
+        language_support=language_support_service,
         secureli_config=secureli_config_repository,
     )
 
     """The service that scans the repository using pre-commit configuration"""
     scanner_service = providers.Factory(
         ScannerService,
         pre_commit=pre_commit_abstraction,
@@ -135,15 +143,14 @@
         ActionDependencies,
         echo=echo,
         language_analyzer=language_analyzer_service,
         language_support=language_support_service,
         scanner=scanner_service,
         secureli_config=secureli_config_repository,
         updater=updater_service,
-        pre_commit=pre_commit_abstraction,
     )
 
     """The Build Action, used to render the build_data using the echo"""
     build_action = providers.Factory(
         BuildAction,
         build_data=build_data,
         echo=echo,
```

### Comparing `secureli-0.6.4/secureli/main.py` & `secureli-0.6.5/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/repositories/repo_files.py` & `secureli-0.6.5/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/repositories/secureli_config.py` & `secureli-0.6.5/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/repositories/settings.py` & `secureli-0.6.5/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/build.txt` & `secureli-0.6.5/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/go-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/go-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.6.5/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/read_resource.py` & `secureli-0.6.5/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/resources/slugify.py` & `secureli-0.6.5/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/services/git_ignore.py` & `secureli-0.6.5/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/services/language_analyzer.py` & `secureli-0.6.5/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/services/logging.py` & `secureli-0.6.5/secureli/services/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 from uuid import uuid4
 
 import pydantic
 
-from secureli.abstractions.pre_commit import PreCommitAbstraction, HookConfiguration
+from secureli.services.language_support import LanguageSupportService, HookConfiguration
 from secureli.repositories.secureli_config import SecureliConfigRepository
 from secureli.utilities.git_meta import current_branch_name, git_user_email, origin_url
 from secureli.utilities.secureli_meta import secureli_version
 
 
 def generate_unique_id() -> str:
     """
@@ -62,28 +62,28 @@
 
 
 class LoggingService:
     """Enables capturing secureli KPI log entries to a local file for future upload"""
 
     def __init__(
         self,
-        pre_commit: PreCommitAbstraction,
+        language_support: LanguageSupportService,
         secureli_config: SecureliConfigRepository,
     ):
-        self.pre_commit = pre_commit
+        self.language_support = language_support
         self.secureli_config = secureli_config
 
     def success(self, action: LogAction) -> LogEntry:
         """
         Capture that a successful conclusion has been reached for an action
         :param action: The action that succeeded
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
-            self.pre_commit.get_configuration(secureli_config.overall_language)
+            self.language_support.get_configuration(secureli_config.overall_language)
             if secureli_config.overall_language
             else None
         )
         log_entry = LogEntry(
             status=LogStatus.success,
             action=action,
             hook_config=hook_config,
@@ -105,15 +105,17 @@
         :param action: The action that failed
         :param details: Details about the failure
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
             None
             if not secureli_config.overall_language
-            else self.pre_commit.get_configuration(secureli_config.overall_language)
+            else self.language_support.get_configuration(
+                secureli_config.overall_language
+            )
         )
         log_entry = LogEntry(
             status=LogStatus.failure,
             action=action,
             failure=LogFailure(
                 details=details,
             ),
```

### Comparing `secureli-0.6.4/secureli/services/scanner.py` & `secureli-0.6.5/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/services/secureli_ignore.py` & `secureli-0.6.5/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/services/updater.py` & `secureli-0.6.5/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/settings.py` & `secureli-0.6.5/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/utilities/git_meta.py` & `secureli-0.6.5/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/utilities/patterns.py` & `secureli-0.6.5/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/secureli/utilities/usage_stats.py` & `secureli-0.6.5/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.4/PKG-INFO` & `secureli-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.6.4
+Version: 0.6.5
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

