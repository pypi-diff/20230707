# Comparing `tmp/nextflowpy-0.6.0-py3-none-any.whl.zip` & `tmp/nextflowpy-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 29020 bytes, number of entries: 14
--rw-r--r--  2.0 unx      312 b- defN 23-Apr-07 01:24 nextflow/__init__.py
--rw-r--r--  2.0 unx     8434 b- defN 23-Apr-08 16:27 nextflow/command.py
+Zip file size: 29087 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-07 18:58 nextflow/__init__.py
+-rw-r--r--  2.0 unx     8731 b- defN 23-Jul-07 18:57 nextflow/command.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Feb-09 15:42 nextflow/exceptions.py
 -rw-r--r--  2.0 unx     9133 b- defN 22-Oct-31 17:04 nextflow/execution.py
--rw-r--r--  2.0 unx     1155 b- defN 23-Apr-07 01:25 nextflow/io.py
+-rw-r--r--  2.0 unx     1155 b- defN 23-May-24 20:50 nextflow/io.py
 -rw-r--r--  2.0 unx     3862 b- defN 23-Apr-07 01:28 nextflow/log.py
--rw-r--r--  2.0 unx     3190 b- defN 23-Apr-08 14:23 nextflow/models.py
+-rw-r--r--  2.0 unx     3190 b- defN 23-May-24 20:50 nextflow/models.py
 -rw-r--r--  2.0 unx     7652 b- defN 22-Oct-31 17:06 nextflow/pipeline.py
 -rw-r--r--  2.0 unx     6989 b- defN 22-Oct-31 17:04 nextflow/utils.py
--rw-r--r--  2.0 unx    35148 b- defN 23-May-24 20:49 nextflowpy-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    11710 b- defN 23-May-24 20:49 nextflowpy-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 20:49 nextflowpy-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-24 20:49 nextflowpy-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1079 b- defN 23-May-24 20:49 nextflowpy-0.6.0.dist-info/RECORD
-14 files, 88913 bytes uncompressed, 27254 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11829 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1079 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/RECORD
+14 files, 89329 bytes uncompressed, 27321 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: nextflow/pipeline.py
 Comment: 
 
 Filename: nextflow/utils.py
 Comment: 
 
-Filename: nextflowpy-0.6.0.dist-info/LICENSE
+Filename: nextflowpy-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: nextflowpy-0.6.0.dist-info/METADATA
+Filename: nextflowpy-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: nextflowpy-0.6.0.dist-info/WHEEL
+Filename: nextflowpy-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: nextflowpy-0.6.0.dist-info/top_level.txt
+Filename: nextflowpy-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nextflowpy-0.6.0.dist-info/RECORD
+Filename: nextflowpy-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextflow/__init__.py

```diff
@@ -1,11 +1,11 @@
 from shutil import which
 from .exceptions import NextflowNotInstalledError
 from .command import run, run_and_poll
 
 __author__ = "Sam Ireland"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 if not which("nextflow"):
     raise NextflowNotInstalledError(
         "Nextflow is either not installed, not in PATH, or is not executable."
     )
```

## nextflow/command.py

```diff
@@ -19,14 +19,15 @@
     :param str pipeline_path: the absolute path to the pipeline .nf file.
     :param str run_path: the location to run the pipeline in.
     :param function runner: a function to run the pipeline command.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
+    :param str timezone: the timezone to use for the log.
     :rtype: ``nextflow.models.Execution``"""
 
     return list(_run(*args, poll=False, **kwargs))[0]
 
 
 def run_and_poll(*args, **kwargs):
     """Runs a pipeline and polls it for updates. Yields the execution after each
@@ -35,28 +36,29 @@
     :param str pipeline_path: the absolute path to the pipeline .nf file.
     :param str run_path: the location to run the pipeline in.
     :param function runner: a function to run the pipeline command.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
+    :param str timezone: the timezone to use for the log.
     :param int sleep: the number of seconds to wait between polls.
     :rtype: ``nextflow.models.Execution``"""
 
     for execution in _run(*args, poll=True, **kwargs):
         yield execution
 
 
 def _run(
         pipeline_path, poll=False, run_path=None, runner=None, version=None,
-        configs=None, params=None, profiles=None, sleep=1
+        configs=None, params=None, profiles=None, timezone=None, sleep=1
 ):
     if not run_path: run_path = os.path.abspath(".")
     nextflow_command = make_nextflow_command(
-        run_path, pipeline_path, version, configs, params, profiles
+        run_path, pipeline_path, version, configs, params, profiles, timezone
     )
     if runner:
         process = None
         runner(nextflow_command)
     else:
         process = subprocess.Popen(
             nextflow_command, universal_newlines=True, shell=True        
@@ -68,47 +70,50 @@
         if execution and poll: yield execution
         process_finished = not process or process.poll() is not None
         if execution and execution.return_code and process_finished:
             if not poll: yield execution
             break
 
 
-def make_nextflow_command(run_path, pipeline_path, version, configs, params, profiles):
+def make_nextflow_command(run_path, pipeline_path, version, configs, params, profiles, timezone):
     """Generates the `nextflow run` commmand.
     
     :param str run_path: the location to run the pipeline in.
     :param str pipeline_path: the absolute path to the pipeline .nf file.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
+    :param str timezone: the timezone to use.
     :rtype: ``str``"""
 
-    env = make_nextflow_command_env_string(version)
+    env = make_nextflow_command_env_string(version, timezone)
     if env: env += " "
     nf = "nextflow -Duser.country=US"
     configs = make_nextflow_command_config_string(configs)
     if configs: configs += " "
     params = make_nextflow_command_params_string(params)
     profiles = make_nextflow_command_profiles_string(profiles)
     command = f"{env}{nf} {configs}run {pipeline_path} {params} {profiles}"
     if run_path: command = f"cd {run_path}; {command}"
     command = command.rstrip() + " >stdout.txt 2>stderr.txt; echo $? >rc.txt"
     return command
 
 
-def make_nextflow_command_env_string(version):
+def make_nextflow_command_env_string(version, timezone):
     """Creates the environment variable setting portion of the nextflow run
     command string.
     
-    :param list configs: any config files to be applied.
+    :param str version: the nextflow version to use.
+    :param str timezone: the timezone to use.
     :rtype: ``str``"""
 
     env = {"NXF_ANSI_LOG": "false"}
     if version: env["NXF_VER"] = version
+    if timezone: env["TZ"] = timezone
     return " ".join([f"{k}={v}" for k, v in env.items()])
 
 
 def make_nextflow_command_config_string(configs):
     """Creates the config setting portion of the nextflow run command string.
     Absolute paths are recommended.
```

## Comparing `nextflowpy-0.6.0.dist-info/LICENSE` & `nextflowpy-0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nextflowpy-0.6.0.dist-info/METADATA` & `nextflowpy-0.6.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflowpy
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python wrapper around Nextflow.
 Home-page: https://github.com/goodwright/nextflow.py
 Author: Sam Ireland
 Author-email: sam@goodwright.com
 License: GPLv3+
 Keywords: nextflow bioinformatics pipeline
 Platform: UNKNOWN
@@ -45,15 +45,15 @@
 nextflow.py is a Python wrapper around the Nextflow pipeline framework. It lets
 you run Nextflow pipelines from Python code.
 
 Example
 -------
 
    >>> import nextflow
-   >>> execution = nextflow.run(path="main.nf", params={"param1": "123"})
+   >>> execution = nextflow.run("main.nf", params={"param1": "123"})
    >>> print(execution.status)
 
 
 Installing
 ----------
 
 pip
@@ -105,41 +105,34 @@
 
 Running
 ~~~~~~~
 
 To run a pipeline, the ``run`` function is used. The only required
 parameter is the path to the pipeline file:
 
-    >>> pipeline = nextflow.Pipeline("pipelines/my-pipeline.nf")
-    >>> execution = pipeline.run()
+    >>> pipeline = nextflow.run("pipelines/my-pipeline.nf")
 
 This will return an ``Execution`` object, which represents the pipeline
 execution that just took place (see below for details on this object). You can
 customise the execution with various options:
 
-    >>> execution = pipeline.run(location="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"])
+    >>> execution = pipeline.run(run_path="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"])
 
-* ``location`` - The location to run the pipeline from, which by default is just
-    the current working directory.
+* ``run_path`` - The location to run the pipeline from, which by default is just the current working directory.
 
-* ``params`` - A dictionary of parameters to pass to the pipeline as command.
-    In the above example, this would run the pipeline with ``--param1=123``.
+* ``params`` - A dictionary of parameters to pass to the pipeline as command. In the above example, this would run the pipeline with ``--param1=123``.
+
+* ``profiles`` - A list of Nextflow profiles to use when running the pipeline. These are defined in the ``nextflow.config`` file, and can be used to configure things like the executor to use, or the container engine to use. In the above example, this would run the pipeline with ``-profile docker,test``.
+
+* ``version`` - The version of Nextflow to use when running the pipeline. By default, the version of Nextflow installed on the system is used, but this can be overridden with this parameter.
+
+* ``configs`` - A list of config files to use when running the pipeline. These are merged with the config files specified in the pipeline itself, and can be used to override any of the settings in the pipeline config.
+
+* ``timezone`` - A timezone to pass to Nextflow - this determines the timestamps used in the log file.
 
-* ``profiles`` - A list of Nextflow profiles to use when running the pipeline.
-    These are defined in the ``nextflow.config`` file, and can be used to
-    configure things like the executor to use, or the container engine to use.
-    In the above example, this would run the pipeline with ``-profile docker,test``.
-
-* ``version`` - The version of Nextflow to use when running the pipeline. By
-    default, the version of Nextflow installed on the system is used, but this
-    can be overridden with this parameter.
-
-* ``configs`` - A list of config files to use when running the pipeline. These
-    are merged with the config files specified in the pipeline itself, and can
-    be used to override any of the settings in the pipeline config.
 
 Custom Runners
 ~~~~~~~~~~~~~~
 
 When you run a pipeline with nextflow.py, it will generate the command string
 that you would use at the command line if you were running the pipeline
 manually. This will be some variant of ``nextflow run some-pipeline.nf``, and
@@ -167,15 +160,15 @@
 The function described above will run the pipeline and wait while it does, with
 the completed ``Execution`` being returned only at the end.
 
 An alternate method is to use ``run_and_poll``, which returns an
 ``Execution`` object every few seconds representing the state of the
 pipeline execution at that moment in time, as a generator::
 
-    for execution in pipeline.run_and_poll(sleep=2, location="./rundir", params={"param1": "123"}):
+    for execution in pipeline.run_and_poll(sleep=2, run_path="./rundir", params={"param1": "123"}):
         print("Processing intermediate execution")
 
 By default, an ``Execution`` will be returned every second, but you can
 adjust this as required with the ``sleep`` paramater. This is useful if you want
 to get information about the progress of the pipeline execution as it proceeds.
 
 Executions
@@ -251,14 +244,22 @@
    'published' via some channel, and those which weren't. It is not possible to
    distinguish these once execution is complete, so nextflow.py reports all
    output files, not just those which are 'published'.
 
 Changelog
 ---------
 
+Release 0.6.1
+~~~~~~~~~~~~~
+
+`7 July, 2023`
+
+* Added option to specify timezone to Nextflow.
+
+
 Release 0.6.0
 ~~~~~~~~~~~~~
 
 `24th May, 2023`
 
 * Added ability to use custom runners for starting jobs.
 * Removed pipeline class to.
```

## Comparing `nextflowpy-0.6.0.dist-info/RECORD` & `nextflowpy-0.6.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-nextflow/__init__.py,sha256=rWMFIKhJxd9_oaAaE64NzrflsqhW9Do5E-DZrdMVArk,312
-nextflow/command.py,sha256=koY550dLTTt9QOmiQ-ahGUK91LcjnOLNazvRVL0yuTE,8434
+nextflow/__init__.py,sha256=4Vhw_FLq67wnFF2oGLff-WYhIaEcBd6reTx--D83eR4,312
+nextflow/command.py,sha256=bHJ382e43utvSwJUnJhzeEGUcN0Ahx7Fy7HPpTLXrTs,8731
 nextflow/exceptions.py,sha256=ktaEfdLca9Bk52CtJoKYMkGaXLrQ9dZVfYh0QtSC9lk,148
 nextflow/execution.py,sha256=j_wsEuqyZafY3BapmhQBkxAmEJsnq9X-a8ADW3Bs0LA,9133
 nextflow/io.py,sha256=8BuYCRGfsI8_oGRkeY3hjTcT4CC_8eFk21Db-Zo5UIk,1155
 nextflow/log.py,sha256=uuL2bMUmuh2iplkfnX6Ch-LgDiWEcZLNxPvEO761yyU,3862
 nextflow/models.py,sha256=v64scmkKaXpidcLcMZSucpDeGVBBFMZmMaZIng_Vu-0,3190
 nextflow/pipeline.py,sha256=XUCsUtcGW3Ou6resfZJIWGkc5rfAq4gAY-jmZ4md9xo,7652
 nextflow/utils.py,sha256=7jSVHEc57_dZb8ZUNVrpUxIQTs3cp7wLQU9R-r-K6OE,6989
-nextflowpy-0.6.0.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-nextflowpy-0.6.0.dist-info/METADATA,sha256=_oupFvwbcTk5k0mujcodETGP-c7yGdoKKiW3Ixnen98,11710
-nextflowpy-0.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nextflowpy-0.6.0.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
-nextflowpy-0.6.0.dist-info/RECORD,,
+nextflowpy-0.6.1.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+nextflowpy-0.6.1.dist-info/METADATA,sha256=30xzdG-8ahwEwiY_G5lDUOozQXI14bb0Dn-88_PokPE,11829
+nextflowpy-0.6.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nextflowpy-0.6.1.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
+nextflowpy-0.6.1.dist-info/RECORD,,
```

