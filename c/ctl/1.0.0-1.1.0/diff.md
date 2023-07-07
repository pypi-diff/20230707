# Comparing `tmp/ctl-1.0.0.tar.gz` & `tmp/ctl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctl-1.0.0.tar", last modified: Sun Jan 24 06:52:49 2021, max compression
+gzip compressed data, was "ctl-1.1.0.tar", max compression
```

## Comparing `ctl-1.0.0.tar` & `ctl-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0    11357 2020-10-31 16:51:19.362551 ctl-1.0.0/LICENSE
--rw-r--r--   0        0        0     1431 2021-01-24 06:50:24.974508 ctl-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12540 2021-01-24 06:40:34.781732 ctl-1.0.0/src/ctl/__init__.py
--rw-r--r--   0        0        0     3387 2021-01-24 06:40:34.781732 ctl-1.0.0/src/ctl/auth.py
--rwxr-xr-x   0        0        0      421 2020-10-31 16:51:19.370551 ctl-1.0.0/src/ctl/bin/ctl_venv_build
--rwxr-xr-x   0        0        0      291 2020-10-31 16:51:19.370551 ctl-1.0.0/src/ctl/bin/ctl_venv_copy
--rwxr-xr-x   0        0        0      604 2020-10-31 16:51:19.370551 ctl-1.0.0/src/ctl/bin/ctl_venv_sync
--rw-r--r--   0        0        0     5143 2021-01-24 06:40:34.782733 ctl-1.0.0/src/ctl/cli.py
--rw-r--r--   0        0        0       32 2020-10-31 16:51:19.370551 ctl-1.0.0/src/ctl/config/__init__.py
--rw-r--r--   0        0        0     3363 2021-01-24 06:40:34.782733 ctl-1.0.0/src/ctl/config/schema.py
--rw-r--r--   0        0        0      729 2021-01-13 14:58:39.241911 ctl-1.0.0/src/ctl/docs.py
--rw-r--r--   0        0        0     1537 2021-01-13 14:58:39.241911 ctl-1.0.0/src/ctl/events.py
--rw-r--r--   0        0        0     1048 2021-01-13 14:58:39.242911 ctl-1.0.0/src/ctl/exceptions.py
--rw-r--r--   0        0        0     1800 2021-01-13 14:58:39.242911 ctl-1.0.0/src/ctl/log.py
--rw-r--r--   0        0        0     8308 2021-01-24 06:40:34.783733 ctl-1.0.0/src/ctl/plugins/__init__.py
--rw-r--r--   0        0        0       78 2020-10-31 16:51:19.371551 ctl-1.0.0/src/ctl/plugins/all.py
--rw-r--r--   0        0        0     5091 2021-01-24 06:40:34.783733 ctl-1.0.0/src/ctl/plugins/chain.py
--rw-r--r--   0        0        0    11410 2021-01-24 06:40:34.784732 ctl-1.0.0/src/ctl/plugins/changelog.py
--rw-r--r--   0        0        0     5674 2021-01-24 06:40:34.784732 ctl-1.0.0/src/ctl/plugins/command.py
--rw-r--r--   0        0        0     1749 2021-01-24 06:40:34.784732 ctl-1.0.0/src/ctl/plugins/config.py
--rw-r--r--   0        0        0     1730 2021-01-24 06:40:34.784732 ctl-1.0.0/src/ctl/plugins/copy.py
--rw-r--r--   0        0        0     2627 2021-01-24 06:40:34.785733 ctl-1.0.0/src/ctl/plugins/email.py
--rw-r--r--   0        0        0     9441 2021-01-24 06:40:34.785733 ctl-1.0.0/src/ctl/plugins/git.py
--rw-r--r--   0        0        0     3205 2021-01-24 06:40:34.785733 ctl-1.0.0/src/ctl/plugins/log.py
--rw-r--r--   0        0        0     2478 2021-01-24 06:40:34.786733 ctl-1.0.0/src/ctl/plugins/log_alert.py
--rw-r--r--   0        0        0     1494 2021-01-24 06:40:34.786733 ctl-1.0.0/src/ctl/plugins/log_git.py
--rw-r--r--   0        0        0      741 2021-01-24 06:40:34.786733 ctl-1.0.0/src/ctl/plugins/log_user.py
--rw-r--r--   0        0        0     3608 2021-01-24 06:40:34.787732 ctl-1.0.0/src/ctl/plugins/pypi.py
--rw-r--r--   0        0        0     4805 2021-01-24 06:40:34.787732 ctl-1.0.0/src/ctl/plugins/release.py
--rw-r--r--   0        0        0     4803 2021-01-24 06:40:34.787732 ctl-1.0.0/src/ctl/plugins/repository.py
--rw-r--r--   0        0        0     4169 2021-01-24 06:40:34.788732 ctl-1.0.0/src/ctl/plugins/template.py
--rw-r--r--   0        0        0     6501 2021-01-24 06:40:34.788732 ctl-1.0.0/src/ctl/plugins/venv.py
--rw-r--r--   0        0        0    11795 2021-01-24 06:40:34.788732 ctl-1.0.0/src/ctl/plugins/version.py
--rw-r--r--   0        0        0     7462 2021-01-24 06:40:34.789733 ctl-1.0.0/src/ctl/plugins/walk_dir.py
--rw-r--r--   0        0        0        0 2020-10-31 16:51:19.374551 ctl-1.0.0/src/ctl/util/__init__.py
--rw-r--r--   0        0        0     2427 2021-01-13 14:58:39.248911 ctl-1.0.0/src/ctl/util/template.py
--rw-r--r--   0        0        0     1435 2021-01-13 14:58:39.248911 ctl-1.0.0/src/ctl/util/versioning.py
--rw-r--r--   0        0        0     1167 2021-01-24 06:52:49.650909 ctl-1.0.0/setup.py
--rw-r--r--   0        0        0     1045 2021-01-24 06:52:49.651183 ctl-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-10-31 16:51:19.362551 ctl-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1689 2023-07-07 21:49:36.399364 ctl-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12537 2023-07-07 21:04:39.135911 ctl-1.1.0/src/ctl/__init__.py
+-rw-r--r--   0        0        0     3390 2023-07-07 21:04:39.136911 ctl-1.1.0/src/ctl/auth.py
+-rwxr-xr-x   0        0        0      421 2020-10-31 16:51:19.370551 ctl-1.1.0/src/ctl/bin/ctl_venv_build
+-rwxr-xr-x   0        0        0      291 2020-10-31 16:51:19.370551 ctl-1.1.0/src/ctl/bin/ctl_venv_copy
+-rwxr-xr-x   0        0        0      604 2020-10-31 16:51:19.370551 ctl-1.1.0/src/ctl/bin/ctl_venv_sync
+-rw-r--r--   0        0        0     5143 2021-01-24 06:40:34.782733 ctl-1.1.0/src/ctl/cli.py
+-rw-r--r--   0        0        0       32 2020-10-31 16:51:19.370551 ctl-1.1.0/src/ctl/config/__init__.py
+-rw-r--r--   0        0        0     3363 2021-01-24 06:40:34.782733 ctl-1.1.0/src/ctl/config/schema.py
+-rw-r--r--   0        0        0      719 2023-07-07 21:04:39.136911 ctl-1.1.0/src/ctl/docs.py
+-rw-r--r--   0        0        0     1537 2021-01-13 14:58:39.241911 ctl-1.1.0/src/ctl/events.py
+-rw-r--r--   0        0        0     1048 2021-01-13 14:58:39.242911 ctl-1.1.0/src/ctl/exceptions.py
+-rw-r--r--   0        0        0     1800 2021-01-13 14:58:39.242911 ctl-1.1.0/src/ctl/log.py
+-rw-r--r--   0        0        0     8311 2023-07-07 21:04:39.138911 ctl-1.1.0/src/ctl/plugins/__init__.py
+-rw-r--r--   0        0        0       78 2020-10-31 16:51:19.371551 ctl-1.1.0/src/ctl/plugins/all.py
+-rw-r--r--   0        0        0     5094 2023-07-07 21:04:39.138911 ctl-1.1.0/src/ctl/plugins/chain.py
+-rw-r--r--   0        0        0    11897 2023-07-07 21:04:39.139911 ctl-1.1.0/src/ctl/plugins/changelog.py
+-rw-r--r--   0        0        0     5671 2023-07-07 21:04:39.139911 ctl-1.1.0/src/ctl/plugins/command.py
+-rw-r--r--   0        0        0     1741 2023-07-07 21:04:39.139911 ctl-1.1.0/src/ctl/plugins/config.py
+-rw-r--r--   0        0        0     1730 2021-01-24 06:40:34.784732 ctl-1.1.0/src/ctl/plugins/copy.py
+-rw-r--r--   0        0        0     2626 2023-07-07 21:04:39.140911 ctl-1.1.0/src/ctl/plugins/email.py
+-rw-r--r--   0        0        0     9724 2023-07-07 21:04:39.140911 ctl-1.1.0/src/ctl/plugins/git.py
+-rw-r--r--   0        0        0     3203 2023-07-07 21:04:39.140911 ctl-1.1.0/src/ctl/plugins/log.py
+-rw-r--r--   0        0        0     2477 2023-07-07 21:04:39.141911 ctl-1.1.0/src/ctl/plugins/log_alert.py
+-rw-r--r--   0        0        0     1493 2023-07-07 21:04:39.141911 ctl-1.1.0/src/ctl/plugins/log_git.py
+-rw-r--r--   0        0        0      741 2021-01-24 06:40:34.786733 ctl-1.1.0/src/ctl/plugins/log_user.py
+-rw-r--r--   0        0        0     3994 2023-07-07 21:04:39.141911 ctl-1.1.0/src/ctl/plugins/pypi.py
+-rw-r--r--   0        0        0     4799 2023-07-07 21:04:39.141911 ctl-1.1.0/src/ctl/plugins/release.py
+-rw-r--r--   0        0        0     4895 2023-07-07 21:04:39.141911 ctl-1.1.0/src/ctl/plugins/repository.py
+-rw-r--r--   0        0        0     5921 2023-07-07 21:04:39.142911 ctl-1.1.0/src/ctl/plugins/semver2.py
+-rw-r--r--   0        0        0     4246 2023-07-07 21:04:39.142911 ctl-1.1.0/src/ctl/plugins/template.py
+-rw-r--r--   0        0        0     6492 2023-07-07 21:04:39.142911 ctl-1.1.0/src/ctl/plugins/venv.py
+-rw-r--r--   0        0        0     5326 2023-07-07 21:04:39.142911 ctl-1.1.0/src/ctl/plugins/version.py
+-rw-r--r--   0        0        0     8226 2023-07-07 21:04:39.143911 ctl-1.1.0/src/ctl/plugins/version_base.py
+-rw-r--r--   0        0        0     7457 2023-07-07 21:04:39.143911 ctl-1.1.0/src/ctl/plugins/walk_dir.py
+-rw-r--r--   0        0        0        0 2020-10-31 16:51:19.374551 ctl-1.1.0/src/ctl/util/__init__.py
+-rw-r--r--   0        0        0     2426 2023-07-07 21:04:39.143911 ctl-1.1.0/src/ctl/util/template.py
+-rw-r--r--   0        0        0     2479 2023-07-07 21:04:39.144911 ctl-1.1.0/src/ctl/util/versioning.py
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 ctl-1.1.0/PKG-INFO
```

### Comparing `ctl-1.0.0/LICENSE` & `ctl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/pyproject.toml` & `ctl-1.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,83 @@
 # Cannot use this for packaging: see https://github.com/20c/ctl/issues/24
 # currently used only for linting
 
 [tool.poetry]
 name = "ctl"
 repository = "https://github.com/20c/ctl"
-version = "1.0.0"
+version = "1.1.0"
 description = "Full control of your environment"
 authors = ["20C <code@20c.com>"]
 license = "Apache-2.0"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Documentation",
 ]
 
+packages = [
+    { include = "ctl", from = "src" },
+]
 
 
 [tool.poetry.scripts]
 ctl = "ctl.cli:main"
 
-
 [tool.poetry.dependencies]
-#python = ">=3.6.1, <4"
-python = "^3.6"
-munge = "^1"
-confu = "^1.4"
-grainy = "^1.4"
-git-url-parse = "^1.1"
-pluginmgr = "^1"
+python = "^3.8"
+
+confu = ">=1.4"
+git-url-parse = ">=1.1"
+grainy = ">=1.4"
+munge = ">=1"
+natsort = ">=8"
+pluginmgr = ">=1"
+semver = "<=3"
 
 [tool.poetry.dev-dependencies]
-# docs
-markdown-include = "^0.6.0"
-mkdocs = "^1.1.2"
-pymdgen = "^0.2.3"
-# tests
-codecov = "^2.1.10"
-coverage = "^5.3"
-pytest = "^6.1.2"
+# testing
+coverage = ">=5"
+pytest = ">=6"
 pytest-cov = "^2.10.1"
 pytest-filedata = "^0.4.0"
-tox = "^3.20.1"
-Jinja2 = "^2.11.2"
-tmpl = "^0.3.0"
-twine = "^3.3.0"
-# pipenv-setup requires an old specific version of black to install
-# pipenv-setup = "^3.1.1"
-PyYAML = "^5.3.1"
+tox = ">=3"
+tox-gh-actions = ">=2"
+
+jinja2 = ">=2"
+tmpl = ">=1"
+twine = ">=3"
+PyYAML = ">1"
+tomlkit = "<1"
+
 # linting
-bandit = "^1.6.2"
-black = "^20.8b1"
-isort = "^5.7.0"
-flake8 = "^3.8.4"
-# pyupgrade requires 3.6.1+...
-# pyupgrade = "^2.7.4"
-# pyupgrade-directories = "^0.0.3"
+# bandit = ">=1.6.2"
+black = ">=20"
+isort = ">=5.7"
+flake8 = ">=3.8"
+mypy = ">=0.950"
+pre-commit = ">=2.13"
+pyupgrade = ">=2.19"
+
+# docs
+markdown = "*"
+markdown-include = ">=0.5,<1"
+mkdocs = ">=1.2.3"
+
+
+[tool.poetry.plugins."markdown.extensions"]
+pymdgen = "pymdgen.md:Extension"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3
```

### Comparing `ctl-1.0.0/src/ctl/__init__.py` & `ctl-1.1.0/src/ctl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         super().__init__(*args, **kwargs)
 
 
 plugin = PluginManager("ctl.plugins")
 
 
 def plugin_cli_arguments(ctlr, parser, plugin_config):
-
     """
     set up cli arguments for the plugin
     """
 
     # get plugin class
 
     plugin_class = ctlr.get_plugin_class(plugin_config.get("type"))
@@ -71,15 +70,14 @@
     read a config file from config_dir
     """
     conf_path = os.path.expanduser(config_dir)
     if not os.path.exists(conf_path):
         raise OSError(f"config dir not found at {conf_path}")
 
     for codec, filename in munge.find_datafile(config_name, conf_path):
-
         if tmpl:
             # if twentyc.tmpl was imported, render config before
             # loading it.
 
             engine = tmpl.get_engine("jinja2")(search_path=os.path.dirname(filename))
             engine.engine.undefined = IgnoreUndefined
             # TODO need a streamlined way to load in template filters
@@ -207,15 +205,15 @@
     def _new_home(self, home):
         # TODO check config for popped options
         self.home = os.path.abspath(home)
 
         user_home = os.path.expanduser("~")
 
         self.tmpdir = os.path.abspath(os.path.join(self.home, "tmp"))
-        self.cachedir = os.path.abspath(os.path.join(user_home, ".ctl", "cache"))
+        self.cachedir = os.path.abspath(os.path.join(user_home, ".cache", "ctl"))
         self.user_home = user_home
 
         if not os.path.exists(self.tmpdir):
             os.makedirs(self.tmpdir)
 
         if not os.path.exists(self.cachedir):
             os.makedirs(self.cachedir)
@@ -268,15 +266,14 @@
         raise ValueError(f"unknown plugin: {name}")
 
     # don't allow updating the config, there's too many undefined
     # things that could happen
     # def set_config_dir(self):
 
     def __init__(self, ctx=None, config_dir=None, full_init=True):
-
         self.init_context(ctx=ctx, config_dir=config_dir)
         self.init_logging()
 
         if self.config.errors:
             return self.log_config_issues()
 
         self.init_permissions()
```

### Comparing `ctl-1.0.0/src/ctl/auth.py` & `ctl-1.1.0/src/ctl/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,30 +39,29 @@
     def __call__(self, fn):
         level = self.level
         namespace_ = self.namespace
         explicit = self.explicit
 
         @wraps(fn)
         def wrapped(self, *args, **kwargs):
-
             # format the namespace using the plugin instance
             # and any arguments passed to the decorated method
             namespace_args = {
                 "plugin": self,
                 "plugin_name": self.pluginmgr_config.get("name"),
             }
             namespace_args.update(**kwargs)
             namespace = namespace_.format(**namespace_args)
 
             # obtain required permission level
             if level is None:
                 # level is not specified at all in the decorator,
                 # in which case we obtain from plugin config and default to 'r'
                 permissions = self.config.get("permissions", {}).get(fn.__name__, "r")
-            elif isinstance(level, collections.Callable):
+            elif isinstance(level, collections.abc.Callable):
                 # level is specified and a function, call it and set from there
                 permissions = level(self)
             else:
                 # level is specified and will be taken from decroator directly
                 permissions = level
 
             # check permissions
```

### Comparing `ctl-1.0.0/src/ctl/bin/ctl_venv_sync` & `ctl-1.1.0/src/ctl/bin/ctl_venv_sync`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/cli.py` & `ctl-1.1.0/src/ctl/cli.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/config/schema.py` & `ctl-1.1.0/src/ctl/config/schema.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/docs.py` & `ctl-1.1.0/src/ctl/docs.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,9 +19,9 @@
             if isinstance(attr, confu.schema.Attribute):
                 attr.pymdgen_type_info = self.confu_type_info(attr)
         return cls
 
     def confu_type_info(self, attr):
         attr_name = attr.__class__.__name__
         if getattr(attr, "item", None):
-            return "{}<{}>".format(attr_name, self.confu_type_info(attr.item))
+            return f"{attr_name}<{self.confu_type_info(attr.item)}>"
         return attr_name
```

### Comparing `ctl-1.0.0/src/ctl/events.py` & `ctl-1.1.0/src/ctl/events.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/exceptions.py` & `ctl-1.1.0/src/ctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/log.py` & `ctl-1.1.0/src/ctl/log.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/plugins/__init__.py` & `ctl-1.1.0/src/ctl/plugins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     ConfigSchema = PluginConfigSchema
     ConfigSchema.help = "Base plugin config schema"
 
     #    def init(self):
     #        pass
 
     def __init__(self, plugin_config, ctx, *args, **kwargs):
-
         """
         **Argument(s)**:
 
         - plugin_config (`dict`)
         - ctx: ctl context (`Ctl`)
 
         Any unknown arguments will be kept in `self.args`
@@ -240,15 +239,15 @@
             env = tmpl["env"]
         return tmpl["engine"]._render_str_to_str(content, env)
 
     def get_op(self, op):
         if not op:
             # TODO UsageError
             raise ValueError("operation not defined")
-        elif not isinstance(getattr(self, op, None), collections.Callable):
+        elif not isinstance(getattr(self, op, None), collections.abc.Callable):
             # TODO Usage Error
             raise ValueError("invalid operation")
 
         fn = getattr(self, op)
 
         if not getattr(fn, "exposed", False):
             raise OperationNotExposed(op)
```

### Comparing `ctl-1.0.0/src/ctl/plugins/chain.py` & `ctl-1.1.0/src/ctl/plugins/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
             if self.end == stage["stage"]:
                 self.log.info(f"end {self.end}")
                 return
 
         self.log.info(f"completed chain `{self.plugin_name}`")
 
     def execute_stage(self, stage, num=1, total=1):
-
         """
         Execute a stage
 
         **Arguments**
 
         - stage (`dict`): chain config (see `ChainConfig`)
         - num (`int`): stage number in the chain
@@ -158,15 +157,15 @@
         """
 
         self.log.info(
             "exec {stage} [{num}/{total}]".format(s=self, num=num, total=total, **stage)
         )
         plugin = self.other_plugin(stage["plugin"])
         fn = getattr(plugin, stage["action"]["name"], None)
-        if not isinstance(fn, collections.Callable):
+        if not isinstance(fn, collections.abc.Callable):
             raise AttributeError(
                 "Action `{action.name}` does not exist in plugin `{plugin}".format(
                     **stage
                 )
             )
 
         kwargs = {}
```

### Comparing `ctl-1.0.0/src/ctl/plugins/changelog.py` & `ctl-1.1.0/src/ctl/plugins/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import argparse
 import os.path
 import re
 
 import confu.schema
 import munge
+from natsort import natsorted
 
 import ctl
 from ctl.auth import expose
 from ctl.docs import pymdgen_confu_types
 from ctl.plugins import ExecutablePlugin
 
 CHANGELOG_SECTIONS = ("added", "fixed", "changed", "deprecated", "removed", "security")
@@ -83,15 +84,14 @@
     """
 
     class ConfigSchema(ExecutablePlugin.ConfigSchema):
         config = ChangeLogPluginConfig()
 
     @classmethod
     def add_arguments(cls, parser, plugin_config, confu_cli_args):
-
         generate_parser = argparse.ArgumentParser(add_help=False)
         group = generate_parser.add_argument_group()
         group.add_argument(
             "--print",
             action="store_true",
             help="if set no file will be generated and output will be printed "
             " to console instead.",
@@ -147,14 +147,28 @@
 
         if "md_file" in kwargs:
             kwargs["md_file"] = os.path.abspath(kwargs["md_file"])
 
         fn = self.get_op(kwargs.get("op"))
         fn(**kwargs)
 
+    def sort_changelog(self, changelog):
+        """
+        Takes a changelog `dict` and sorts keys by version using
+        natural sort
+
+        Returns the sorted `dict`
+        """
+
+        changelog_list = []
+        for key in natsorted(list(changelog.keys()), reverse=True):
+            changelog_list.append((key, changelog.get(key)))
+
+        return dict(changelog_list)
+
     @expose("ctl.{plugin_name}.release")
     def release(self, version, data_file, **kwargs):
         """
         Adds the specified release to the changelog.
 
         This will validate and move all items under "unreleased"
         to a new section for the specified release version
@@ -176,14 +190,16 @@
 
         if not release_section:
             raise ValueError("No items exist in unreleased to be moved")
 
         changelog[version] = release_section
         changelog["Unreleased"] = {section: [] for section in CHANGELOG_SECTIONS}
 
+        changelog = self.sort_changelog(changelog)
+
         ext = os.path.splitext(data_file)[1][1:]
         codec = munge.get_codec(ext)
 
         with open(data_file, "w+") as fh:
             codec().dump(changelog, fh)
 
         self.log.info(f"Updated {data_file}")
@@ -297,15 +313,15 @@
         out = ["# Changelog"]
 
         releases = [
             {"version": version.capitalize(), "changes": changes}
             for version, changes in list(data.items())
         ]
 
-        releases = sorted(releases, key=lambda i: i.get("version"), reverse=True)
+        releases = natsorted(releases, key=lambda i: i.get("version"), reverse=True)
 
         for release in releases:
             out.extend(["", "", "## {version}".format(**release)])
             sections = {}
             for change_type, items in list(release.get("changes", {}).items()):
                 if len(items):
                     sections[change_type] = [f"- {item}" for item in items]
@@ -354,15 +370,15 @@
             elif match_title:
                 change_list = version_container[match_title.group(1).lower()] = []
                 continue
             elif match_change:
                 change_list.append(match_change.group(1))
                 continue
 
-        return changelog
+        return self.sort_changelog(changelog)
 
     def version_exists(self, data_file, version):
         """
         Checks if the specified release exists in the changelog
 
         **Arguments**
```

### Comparing `ctl-1.0.0/src/ctl/plugins/command.py` & `ctl-1.1.0/src/ctl/plugins/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,28 +121,26 @@
     # namespace will be built using the name of the
     # plugin instance
     #
     # required permissions will be obtained from `permissions` key
     # in the plugin's config, and default to `r` if not specified
     @expose("ctl.{plugin_name}")
     def execute(self, **kwargs):
-
         """
         execute the command(s) specified in the plugin
         config `command` list
 
         *overrides and calls `ExecutablePlugin.execute`*
         """
 
         super().execute(**kwargs)
         command = self.get_config("command")
         self._run_commands(command, **kwargs)
 
     def _run_commands(self, command, **kwargs):
-
         """
         execute a list of commands
 
         this is called automatically during `execute`
 
         **Argument(s)**
 
@@ -161,15 +159,14 @@
             if rc:
                 self.log.error(f"command {cmd} failed with {rc}")
                 return False
 
         # TODO: should return True here?
 
     def _exec(self, command):
-
         """
         execute a single command
 
         this is called automatically during `_run_commands`
 
         **Argument(s)**
```

### Comparing `ctl-1.0.0/src/ctl/plugins/config.py` & `ctl-1.1.0/src/ctl/plugins/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def option_name(path, delimiter="--"):
     """returns a cli option name from attribute path"""
     return "--{}".format(delimiter.join(path).replace("_", "-"))
 
 
 def destination_name(path, delimiter="__"):
     """returns a cli option destination name from attribute path"""
-    return "{}".format(delimiter.join(path))
+    return f"{delimiter.join(path)}"
 
 
 def list_options(schema):
     rv = []
 
     def optionize(attribute, path):
         if not attribute.cli:
```

### Comparing `ctl-1.0.0/src/ctl/plugins/copy.py` & `ctl-1.1.0/src/ctl/plugins/copy.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/plugins/email.py` & `ctl-1.1.0/src/ctl/plugins/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         subject = kwargs.get("subject", self.config.get("subject"))
         recipients = kwargs.get("recipients", self.config.get("recipients", []))
         sender = kwargs.get("sender", self.config.get("sender"))
         for recipient in recipients:
             self._send(body, subject, sender, recipient)
 
     def _send(self, body, subject, sender, recipient, **kwargs):
-
         """
         Send email, private method use `send` instead
 
         **Arguments**
 
         - body (`str`): message body
         - subject (`str`): message subject
```

### Comparing `ctl-1.0.0/src/ctl/plugins/git.py` & `ctl-1.1.0/src/ctl/plugins/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     For information on the configuration schema please check
     the `RepositoryPlugin` documenation
     """
 
     @property
     def uuid(self):
-        """ return recent commit hash of the repo """
+        """return recent commit hash of the repo"""
         command = self.command("rev-parse", "--short", "HEAD")
         return self.run_git_command(command)[0].strip()
 
     @property
     def is_cloned(self):
         """
         returns whether or not the checkout_path location is a valid
@@ -100,15 +100,14 @@
             if f"{exc}".find("fatal: Needed a single revision") > -1:
                 return False
             raise
         return True
 
     @classmethod
     def add_arguments(cls, parser, plugin_config, confu_cli_args):
-
         shared_parser = argparse.ArgumentParser(add_help=False)
         group = shared_parser.add_mutually_exclusive_group(required=False)
         group.add_argument("--repo-url", type=str)
         group.add_argument("--checkout-path", type=str)
 
         # subparser that routes operation
         sub = parser.add_subparsers(title="Operation", dest="op")
@@ -122,15 +121,14 @@
         # operation `checkout`
         op_checkout_parser = sub.add_parser(
             "checkout", help="checkout tag or branch", parents=[shared_parser]
         )
         op_checkout_parser.add_argument("tag", nargs=1, help="tag or branch")
 
     def execute(self, **kwargs):
-
         """
         Execute plugin operation
 
         **Keyword Arguments**
 
         - op (`str`): operation to execute - needs to be exposed
         - checkout_path (`str`): override repo_url config param
@@ -274,29 +272,38 @@
         self.log.debug("Cloned {s.repo_url} in {s.checkout_path}".format(s=self))
 
     @expose("ctl.{plugin_name}.pull")
     def pull(self, **kwargs):
         """
         Pull the repo
         """
-        self.log.debug(f"PULL {self.checkout_path}")
-        command_pull = self.command("pull")
+
+        branch = self.get_config("branch")
+        remote = self.get_config("remote")
+
+        self.log.debug(f"PULL {self.checkout_path} {remote}/{branch}")
+        self.checkout(branch)
+        command_pull = self.command("pull", remote, branch)
         self.run_git_command(command_pull)
-        self.log.debug(f"PULL {self.checkout_path} complete")
+        self.log.debug(f"PULL {self.checkout_path} {remote}/{branch} complete")
 
     def push(self, **kwargs):
         """
         Push commits
         """
-        self.log.debug(f"PUSH {self.checkout_path}")
-        command_push = self.command("push", "origin", self.branch)
+
+        branch = self.get_config("branch")
+        remote = self.get_config("remote")
+
+        self.log.debug(f"PUSH {self.checkout_path} {remote} {branch}")
+        command_push = self.command("push", remote, branch)
         if kwargs.get("tags"):
             command_push += ["--tags"]
         self.run_git_command(command_push)
-        self.log.debug(f"PUSH {self.checkout_path} complete")
+        self.log.debug(f"PUSH {self.checkout_path} {remote} {branch} complete")
 
     def tag(self, version, message, **kwargs):
         """
         Tag the currently active branch
 
         **Arguments**
```

### Comparing `ctl-1.0.0/src/ctl/plugins/log.py` & `ctl-1.1.0/src/ctl/plugins/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             logger_name = logger_config.get("logger")
             self.attach_to_logger(logger_name)
             self.configure_logger(logger_name, logger_config)
 
         self.loggers = loggers
 
     def configure_logger(self, logger_name, logger_config):
-
         """
         Configure python logger from plugin config
 
         If your logger config attribute specifies things like formatting
         and handlers the targeted logger will be configured accordingly
 
         This is called automatically during `init`
@@ -84,15 +83,14 @@
                 "format", LogPluginLoggerConfig.format.default
             )
             fh = logging.FileHandler(filename=filename, mode="a+")
             fh.setFormatter(logging.Formatter(formatter))
             logger.addHandler(fh)
 
     def attach_to_logger(self, logger_name):
-
         """
         Attach plugin to python logger
 
         **Arguments**
 
         - logger_name (`str`)
         """
```

### Comparing `ctl-1.0.0/src/ctl/plugins/log_alert.py` & `ctl-1.1.0/src/ctl/plugins/log_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     """
 
     def init(self):
         super().init()
         self.messages = []
 
     def alert(self, **kwargs):
-
         """
         Send alert through another plugin
 
         **Keyword arguments**
 
         - levels (`list`): list of logging levels that will cause
           triggering of this alert. As soon as there is at least
```

### Comparing `ctl-1.0.0/src/ctl/plugins/log_git.py` & `ctl-1.1.0/src/ctl/plugins/log_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             filepath = logger.get("file")
             if filepath and filepath[0] != "/":
                 logger["file"] = os.path.join(self.git.checkout_path, filepath)
 
         super().init()
 
     def apply(self, message, level):
-
         """
         Add git information to log message
 
         **Arguments**
 
         - message (`str`): log message
         - level (`str`): log severity level
```

### Comparing `ctl-1.0.0/src/ctl/plugins/log_user.py` & `ctl-1.1.0/src/ctl/plugins/log_user.py`

 * *Files identical despite different names*

### Comparing `ctl-1.0.0/src/ctl/plugins/pypi.py` & `ctl-1.1.0/src/ctl/plugins/pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,26 @@
         self._upload()
 
     def _build_dist(self, **kwargs):
         """
         Build dist
         """
 
-        command = ["rm dist/* -rf", "python setup.py sdist"]
+        command = ["rm dist/* -rf"]
+
+        path = self.repository.checkout_path
+
+        if os.path.exists(os.path.join(path, "setup.py")):
+            command.append("python setup.py sdist")
+            command.append("python setup.py bdist_wheel")
+        elif os.path.exists(os.path.join(path, "poetry.lock")):
+            command.append("poetry build")
+        else:
+            raise OSError("Could find neither setup.py nor poetry.lock")
+
         self._run_commands(command)
 
     def _validate(self, **kwargs):
         """
         Build dist and validate
         """
```

### Comparing `ctl-1.0.0/src/ctl/plugins/release.py` & `ctl-1.1.0/src/ctl/plugins/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     """
 
     class ConfigSchema(ctl.plugins.PluginBase.ConfigSchema):
         config = ReleasePluginConfig()
 
     @classmethod
     def add_arguments(cls, parser, plugin_config, confu_cli_args):
-
         shared_parser = argparse.ArgumentParser(add_help=False)
         group = shared_parser.add_argument_group()
 
         group.add_argument(
             "version",
             nargs=1,
             type=str,
@@ -101,15 +100,14 @@
             self.repository.checkout(self.version)
             op = self.get_op(kwargs.get("op"))
             op(**kwargs)
         finally:
             self.repository.checkout(self.orig_branch)
 
     def set_repository(self, repository):
-
         """
         Set release repository. Distributions will be built from that
         repository.
 
         Currently only supports `git` type repositories
 
         **Attributes**
@@ -155,13 +153,13 @@
     def validate(self, **kwargs):
         """
         Build and validate the package
         """
         self._validate(**kwargs)
 
     def _release(self, **kwargs):
-        """ should run release logic """
+        """should run release logic"""
         raise NotImplementedError()
 
     def _validate(self, **kwargs):
-        """ should run build and validation logic """
+        """should run build and validation logic"""
         raise NotImplementedError()
```

### Comparing `ctl-1.0.0/src/ctl/plugins/repository.py` & `ctl-1.1.0/src/ctl/plugins/repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 
 import confu.schema
 import giturlparse
 
 from ctl.docs import pymdgen_confu_types
 from ctl.plugins import ExecutablePlugin
-from ctl.util.versioning import version_tuple
 
 
 @pymdgen_confu_types()
 class PluginConfig(confu.schema.Schema):
     """
     Configuration schema for `RepositoryPlugin`
     """
@@ -21,18 +20,22 @@
     repo_url = confu.schema.Str(cli=False)
     checkout_path = confu.schema.Directory(
         default="",
         blank=True,
         help="checkout to this local "
         "location - if not specified "
         "will default to "
-        "~/.ctl/cache/{repo_url}",
+        "~/.cache/ctl/repo/{repo_url}",
     )
 
-    branch = confu.schema.Str(help="Checkout this branch", default="master")
+    branch = confu.schema.Str(
+        help="Checkout this branch (just branch name, use `remote` attribute to specify origin)",
+        default="master",
+    )
+    remote = confu.schema.Str(help="Checkout this remote", default="origin")
 
 
 class RepositoryPlugin(ExecutablePlugin):
     """
     Interface for repository type plugins
     """
 
@@ -40,37 +43,37 @@
         config = PluginConfig()
 
     def __repr__(self):
         return f"Repository `{self.plugin_name}`"
 
     @property
     def uuid(self):
-        """ should return current commit hash/id """
+        """should return current commit hash/id"""
         raise NotImplementedError()
 
     @property
     def version(self):
-        """ current version as it exists in `version_file` """
+        """current version as it exists in `version_file`"""
         try:
             print(("Reading version from", self.version_file))
             with open(self.version_file) as fh:
-                version = version_tuple(fh.read().strip())
+                version = fh.read().strip()
         except FileNotFoundError:
             self.log.debug(f"No version file found at {self.version_file}")
-            return (0, 0, 0)
+            return "0.0.0"
         return version
 
     @property
     def version_file(self):
-        """ location of version file """
+        """location of version file"""
         return os.path.join(self.repo_ctl_dir, "VERSION")
 
     @property
     def repo_ctl_dir(self):
-        """ location of ctl directory inside repository """
+        """location of ctl directory inside repository"""
         return os.path.join(self.checkout_path, "Ctl")
 
     @property
     def is_cloned(self):
         """
         should return True or False depending on whether the repository
         is already cloned at checkout_path or not
@@ -115,52 +118,51 @@
     def clone(self, **kwargs):
         """
         Should clone the repository according to config parameters `repo_url` and `checkout_path`
         """
         raise NotImplementedError()
 
     def pull(self, **kwargs):
-        """ Should pull the repository """
+        """Should pull the repository"""
         raise NotImplementedError()
 
     def push(self, **kwargs):
-        """ Should push changes to the remote """
+        """Should push changes to the remote"""
         raise NotImplementedError()
 
     def tag(self, version, **kwargs):
-        """ Should tag the current branch """
+        """Should tag the current branch"""
         raise NotImplementedError()
 
     def checkout(self, branch, **kwargs):
-        """ Should checkout a branch by name """
+        """Should checkout a branch by name"""
         raise NotImplementedError()
 
     def merge(self, branch_a, branch_b, **kwargs):
-        """ Should merge branch b into branch a """
+        """Should merge branch b into branch a"""
         raise NotImplementedError()
 
     def init(self):
         self.repo_url = self.get_config("repo_url")
         self.checkout_path = self.get_config("checkout_path")
 
         branch = self.get_config("branch")
 
         if not self.checkout_path:
-
             parsed_url = giturlparse.parse(self.repo_url)
 
             # print("pathname", parsed_url.pathname)
             # print("href", parsed_url.href)
             # print("user", parsed_url.user)
             # print("name", parsed_url.name)
             # print("owner", parsed_url.owner)
             # print("resource", parsed_url.resource)
 
             self.checkout_path = os.path.join(
-                self.ctl.cachedir, parsed_url.resource, parsed_url.pathname
+                self.ctl.cachedir, "repo", parsed_url.resource, parsed_url.pathname
             )
 
         # while checkout patch can be relative in the config, we want
         # it to be absolute from here on out
         self.checkout_path = os.path.abspath(self.checkout_path)
 
         self.clone()
```

### Comparing `ctl-1.0.0/src/ctl/plugins/template.py` & `ctl-1.1.0/src/ctl/plugins/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         cli=False,
         help="list of files containing template " "variables to import",
     )
 
 
 def update(a, b):
     for key, value in list(b.items()):
-        if isinstance(value, collections.Mapping):
+        if isinstance(value, collections.abc.Mapping):
             a[key] = update(a.get(key, {}), value)
         else:
             a[key] = value
     return a
 
 
 @ctl.plugin.register("template")
@@ -154,7 +154,9 @@
 
         out_dir = os.path.dirname(self.output(path))
         if not os.path.isdir(out_dir):
             os.makedirs(out_dir)
         self.log.info(self.output(path))
         self.engine.render(path, out_dir=self.output(), env=self.tmpl_env)
         self.debug_append("rendered", self.output(path))
+
+        os.chmod(self.output(path), os.stat(self.source(path)).st_mode)
```

### Comparing `ctl-1.0.0/src/ctl/plugins/venv.py` & `ctl-1.1.0/src/ctl/plugins/venv.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,17 @@
 
         **Keyword Arguments**
 
         - path (`str`): path to check (should be virtuelenv root directory)
         """
 
         if not self.venv_exists(path):
-            raise UsageError("No virtualenv found at {}".format(path or self.output))
+            raise UsageError(f"No virtualenv found at {path or self.output}")
 
     def execute(self, **kwargs):
-
         self.kwargs = kwargs
 
         python_version = self.get_config("python_version")
         pipfile = self.get_config("pipfile")
 
         self.python_version = self.render_tmpl(python_version)
         self.pipfile = self.render_tmpl(pipfile)
```

### Comparing `ctl-1.0.0/src/ctl/plugins/version.py` & `ctl-1.1.0/src/ctl/plugins/version_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,63 +2,51 @@
 Plugin that allows you to handle repository versioning
 """
 
 import argparse
 import os
 
 import confu.schema
+import munge
 
 import ctl
-from ctl.auth import expose
 from ctl.docs import pymdgen_confu_types
-from ctl.exceptions import OperationNotExposed, PluginOperationStopped, UsageError
+from ctl.exceptions import PluginOperationStopped, UsageError
 from ctl.plugins import ExecutablePlugin
 from ctl.plugins.changelog import ChangelogVersionMissing
 from ctl.plugins.changelog import temporary_plugin as temporary_changelog_plugin
-from ctl.plugins.git import temporary_plugin as temporary_git_plugin
 from ctl.plugins.repository import RepositoryPlugin
-from ctl.util.versioning import bump_semantic, version_string
+from ctl.util.versioning import version_string
 
 
 @pymdgen_confu_types()
-class VersionPluginConfig(confu.schema.Schema):
+class VersionBasePluginConfig(confu.schema.Schema):
     """
-    Configuration schema for `VersionPlugin`
+    Configuration schema for `VersionBasePlugin`
     """
 
     repository = confu.schema.Str(
         help="name of repository type plugin or path " "to a repository checkout",
         default=None,
         cli=False,
     )
 
-    branch_dev = confu.schema.Str(
-        default="master",
-        help="the branch to merge from when the " "--merge-release flag is present",
-    )
-
-    branch_release = confu.schema.Str(
-        default="master",
-        help="the breanch to merge to when " "the --merge-release flag is present",
-    )
-
     changelog_validate = confu.schema.Bool(
         default=True,
         help="If a changelog data file (CHANGELOG.yaml) exists, validate before tagging",
     )
 
 
-@ctl.plugin.register("version")
-class VersionPlugin(ExecutablePlugin):
+class VersionBasePlugin(ExecutablePlugin):
     """
     manage repository versioning
     """
 
     class ConfigSchema(ExecutablePlugin.ConfigSchema):
-        config = VersionPluginConfig()
+        config = VersionBasePluginConfig()
 
     @classmethod
     def add_repo_argument(cls, parser, plugin_config):
         """
         The `repository` cli parameter needs to be available
         on all operations. However since it is an optional
         positional parameter that cames at the end using shared
@@ -73,32 +61,23 @@
         - parser (`argparse.ArgParser`)
         - plugin_config (`dict`)
         """
         parser.add_argument(
             "repository",
             nargs="?",
             type=str,
-            help=VersionPluginConfig().repository.help,
+            help=VersionBasePluginConfig().repository.help,
             default=plugin_config.get("repository"),
         )
 
     @classmethod
     def add_arguments(cls, parser, plugin_config, confu_cli_args):
-
         shared_parser = argparse.ArgumentParser(add_help=False)
-
         release_parser = argparse.ArgumentParser(add_help=False)
         group = release_parser.add_mutually_exclusive_group(required=False)
-        group.add_argument(
-            "--release",
-            action="store_true",
-            help="if set will also "
-            "perform `merge_release` operation and tag in the specified "
-            "release branch instead of the currently active branch",
-        )
 
         group.add_argument(
             "--init",
             action="store_true",
             help="automatically create " "Ctl/VERSION file if it does not exist",
         )
 
@@ -111,95 +90,54 @@
             help="tag with a specified version",
             parents=[shared_parser, release_parser],
         )
         op_tag_parser.add_argument(
             "version", nargs=1, type=str, help="version string to tag with"
         )
 
+        confu_cli_args.add(op_tag_parser, "changelog_validate")
         cls.add_repo_argument(op_tag_parser, plugin_config)
 
         # operation `bump`
         op_bump_parser = sub.add_parser(
             "bump",
             help="bump semantic version",
             parents=[shared_parser, release_parser],
         )
         op_bump_parser.add_argument(
             "version",
             nargs=1,
             type=str,
-            choices=["major", "minor", "patch", "dev"],
+            choices=["major", "minor", "patch", "prerelease"],
             help="bumps the specified version segment by 1",
         )
 
-        op_bump_parser.add_argument(
-            "--no-auto-dev",
-            help="disable automatic bumping of dev "
-            "version after bumping `major`, `minor` or `patch`",
-            action="store_true",
-        )
-
         confu_cli_args.add(op_bump_parser, "changelog_validate")
-
         cls.add_repo_argument(op_bump_parser, plugin_config)
 
-        # operations `merge_release`
-        op_mr_parser = sub.add_parser(
-            "merge_release",
-            help="merge dev branch into release branch " "(branches defined in config)",
-            parents=[shared_parser],
-        )
-
-        cls.add_repo_argument(op_mr_parser, plugin_config)
+        return {
+            "group": group,
+            "sub": sub,
+            "shared_parser": shared_parser,
+            "release_parser": release_parser,
+            "op_tag_parser": op_tag_parser,
+            "op_bump_parser": op_bump_parser,
+        }
 
     @property
     def init_version(self):
         """
         `True` if a `Ctl/VERSION` file should be created if it's missing
         """
         return getattr(self, "_init_version", False)
 
     @init_version.setter
     def init_version(self, value):
         self._init_version = value
 
-    @property
-    def no_auto_dev(self):
-        """
-        `True` if we do **NOT** want to automatically bump a dev version when a major
-        minor or patch version is bumped
-        """
-        return getattr(self, "_no_auto_dev", False)
-
-    @no_auto_dev.setter
-    def no_auto_dev(self, value):
-        self._no_auto_dev = value
-
-    def execute(self, **kwargs):
-
-        super().execute(**kwargs)
-
-        branch_dev = self.get_config("branch_dev")
-        branch_release = self.get_config("branch_release")
-        self.no_auto_dev = kwargs.get("no_auto_dev", False)
-        self.init_version = kwargs.get("init", False)
-
-        if "version" in kwargs and isinstance(kwargs["version"], list):
-            kwargs["version"] = kwargs["version"][0]
-
-        kwargs["repo"] = self.get_config("repository")
-
-        op = kwargs.get("op")
-        fn = self.get_op(op)
-
-        if not getattr(fn, "exposed", False):
-            raise OperationNotExposed(op)
-
-        fn(**kwargs)
-
     def repository(self, target):
         """
         Return plugin instance for repository
 
         **Arguments**
 
         - target (`str`): name of a configured repository type plugin
@@ -234,110 +172,62 @@
             raise UsageError(
                 "Ctl/VERSION file does not exist. You can set the --init flag to create "
                 "it automatically."
             )
 
         return plugin
 
-    @expose("ctl.{plugin_name}.merge_release")
-    def merge_release(self, repo, **kwargs):
+    def update_version_files(self, repo_plugin, version, files):
         """
-        Merge branch self.branch_dev into branch self.branch_release in the specified
-        repo
-
-        **Arguments**
-
-        - repo (`str`): name of existing repository type plugin instance
+        Finds the various files in a repo that will need to
+        have new version values written, such as Ctl/VERSION
+        and pyproject.toml
         """
-        from_branch = self.get_config("branch_dev")
-        to_branch = self.get_config("branch_release")
-        if from_branch == to_branch:
-            self.log.debug("dev and release branch are identical, no need to merge")
-            return
-
-        repo_plugin = self.repository(repo)
-        self.log.info(f"Merging branch '{from_branch}' into branch '{to_branch}'")
-        repo_plugin.merge(from_branch, to_branch)
-        repo_plugin.push()
 
-    @expose("ctl.{plugin_name}.tag")
-    def tag(self, version, repo, **kwargs):
-        """
-        tag a version according to version specified
+        types = ["ctl", "pyproject"]
 
-        **Arguments**
-
-        - version (`str`): tag version (eg. 1.0.0)
-        - repo (`str`): name of existing repository type plugin instance
-
-        **Keyword Arguments**
+        for typ in types:
+            fn = getattr(self, f"update_{typ}_version")
+            path = fn(repo_plugin, version)
+            if path:
+                files.append(path)
 
-        - release (`bool`): if `True` also run `merge_release`
+    def update_ctl_version(self, repo_plugin, version):
+        """
+        Writes a new version to the Ctl/VERSION files
         """
-        repo_plugin = self.repository(repo)
-        repo_plugin.pull()
-
-        if not repo_plugin.is_clean:
-            raise UsageError("Currently checked out branch is not clean")
-
-        if kwargs.get("release"):
-            self.merge_release(repo=repo)
-            repo_plugin.checkout(self.get_config("branch_release") or "master")
-
-        self.log.info(f"Preparing to tag {repo_plugin.checkout_path} as {version}")
-        if not os.path.exists(repo_plugin.repo_ctl_dir):
-            os.makedirs(repo_plugin.repo_ctl_dir)
 
         with open(repo_plugin.version_file, "w") as fh:
             fh.write(version)
+        return repo_plugin.version_file
 
-        repo_plugin.commit(
-            files=["Ctl/VERSION"], message=f"Version {version}", push=True
-        )
-        repo_plugin.tag(version, message=version, push=True)
-
-    @expose("ctl.{plugin_name}.bump")
-    def bump(self, version, repo, **kwargs):
+    def update_pyproject_version(self, repo_plugin, version):
         """
-        bump a version according to semantic version
-
-        **Arguments**
-
-        - version (`str`): major, minor, patch or dev
-        - repo (`str`): name of existing repository type plugin instance
+        Writes a new version to the pyproject.toml file
+        if it exists
         """
 
-        repo_plugin = self.repository(repo)
-        repo_plugin.pull()
-
-        if version not in ["major", "minor", "patch", "dev"]:
-            raise ValueError(f"Invalid semantic version: {version}")
-
-        is_dev = version == "dev"
-
-        current = repo_plugin.version
-        version = bump_semantic(current, version)
-
-        self.log.info(
-            "Bumping semantic version: {} to {}".format(
-                version_string(current), version_string(version)
+        try:
+            pyproject_path = os.path.join(repo_plugin.checkout_path, "pyproject.toml")
+            pyproject = munge.load_datafile(
+                "pyproject.toml", search_path=(repo_plugin.checkout_path)
             )
-        )
+            pyproject["tool"]["poetry"]["version"] = version
 
-        if self.get_config("changelog_validate") and not is_dev:
-            self.validate_changelog(repo, version)
+            codec = munge.get_codec("toml")
 
-        self.tag(version=version_string(version), repo=repo, **kwargs)
+            with open(pyproject_path, "w") as fh:
+                codec().dump(pyproject, fh)
+            return pyproject_path
 
-        if not is_dev and not self.no_auto_dev:
-            self.log.info("Creating dev tag")
-            self.bump(version="dev", repo=repo, **kwargs)
+        except OSError as exc:
+            if "not found" in str(exc):
+                return
 
     def validate_changelog(self, repo, version, data_file="CHANGELOG.yaml"):
-
         """
         Checks for the existance of a changelog data file
         like CHANGELOG.yaml or CHANGELOG.json and
         if found will validate that the specified
         version exists.
 
         Will raise a KeyError on validation failure
```

### Comparing `ctl-1.0.0/src/ctl/plugins/walk_dir.py` & `ctl-1.1.0/src/ctl/plugins/walk_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 
     """
 
     class ConfigSchema(ctl.plugins.PluginBase.ConfigSchema):
         config = WalkDirPluginConfig("config")
 
     def prepare(self, **kwargs):
-
         """
         prepare plugin for execution
 
         !!! note "Output directory"
             output directory from `config.output` will be created
             if it does not exist
 
@@ -98,15 +97,14 @@
 
         self.log.info(f"Skip dotfiles: {self.skip_dotfiles}")
 
         if not os.path.exists(self._output):
             os.makedirs(self._output)
 
     def source(self, path=None):
-
         """
         Returns the source path
 
         Plugin's `prepare` method needs to have been called.
 
         **Keyword Arguments**
 
@@ -119,15 +117,14 @@
         """
 
         if path:
             return os.path.join(self._source, path)
         return self._source
 
     def output(self, path=None):
-
         """
         Returns the output path
 
         Plugin's `prepare` method needs to have been called.
 
         **Keyword Arguments**
 
@@ -142,15 +139,14 @@
         if not self._output:
             return path
         if path:
             return os.path.join(self._output, path)
         return self._output
 
     def execute(self, **kwargs):
-
         """
         Execute the plugin
 
         *overrides and calls `ExecutablePlugin.execute`*
         """
 
         super().execute(**kwargs)
@@ -162,15 +158,15 @@
             raise ValueError("No source directory specified")
 
         if self._output:
             self._output = self.render_tmpl(self._output)
 
         self._source = self.render_tmpl(self._source)
 
-        self.source_regex = fr"^{self.source()}/"
+        self.source_regex = rf"^{self.source()}/"
 
         self.process_files()
 
     def process_files(self):
         """
         Walks the subdirectories of the source path
         and processes the files.
@@ -182,15 +178,14 @@
         for subdir in self.walk_dirs:
             for dirpath, dirnames, filenames in os.walk(self.source(subdir)):
                 path = re.sub(self.source_regex, "", dirpath)
 
                 for filepath, filename in [
                     (os.path.join(path, _f), _f) for _f in filenames
                 ]:
-
                     if self.skip_dotfiles and filename[0] == ".":
                         continue
 
                     if not self.ignored(filepath, path):
                         self.prepare_file(filepath, path)
                         self.process_file(filepath, path)
```

### Comparing `ctl-1.0.0/src/ctl/util/template.py` & `ctl-1.1.0/src/ctl/util/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,15 +85,14 @@
             __int__
         ) = (
             __float__
         ) = (
             __complex__
         ) = __pow__ = __rpow__ = __sub__ = __rsub__ = _fail_with_undefined_error
 
-
 except ImportError:
 
     class IgnoreUndefined:
         pass
 
 
 def filter_escape_regex(value, **kwargs):
```

### Comparing `ctl-1.0.0/PKG-INFO` & `ctl-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ctl
-Version: 1.0.0
+Version: 1.1.0
 Summary: Full control of your environment
 Home-page: https://github.com/20c/ctl
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
-Requires-Dist: confu (>=1.4,<2.0)
-Requires-Dist: git-url-parse (>=1.1,<2.0)
-Requires-Dist: grainy (>=1.4,<2.0)
-Requires-Dist: munge (>=1,<2)
-Requires-Dist: pluginmgr (>=1,<2)
+Requires-Dist: confu (>=1.4)
+Requires-Dist: git-url-parse (>=1.1)
+Requires-Dist: grainy (>=1.4)
+Requires-Dist: munge (>=1)
+Requires-Dist: natsort (>=8)
+Requires-Dist: pluginmgr (>=1)
+Requires-Dist: semver (<=3)
 Project-URL: Repository, https://github.com/20c/ctl
```

