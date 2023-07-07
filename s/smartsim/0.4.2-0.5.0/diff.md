# Comparing `tmp/smartsim-0.4.2.tar.gz` & `tmp/smartsim-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsim-0.4.2.tar", last modified: Wed Apr 12 20:48:46 2023, max compression
+gzip compressed data, was "smartsim-0.5.0.tar", last modified: Fri Jul  7 00:28:52 2023, max compression
```

## Comparing `smartsim-0.4.2.tar` & `smartsim-0.5.0.tar`

### file list

```diff
@@ -1,158 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 20:48:40.000000 smartsim-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 20:48:40.000000 smartsim-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-12 20:48:40.000000 smartsim-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-04-12 20:48:46.147744 smartsim-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-04-12 20:48:40.000000 smartsim-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-12 20:48:40.000000 smartsim-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 20:48:40.000000 smartsim-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:48:46.147744 smartsim-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-12 20:48:40.000000 smartsim-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.115744 smartsim-0.4.2/smartsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_install/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_install/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/buildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.111744 smartsim-0.4.2/smartsim/_core/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/bin/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/bin/modules/FindTensorFlow.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    71337 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/keydb.conf
--rw-r--r--   0 runner    (1001) docker     (123)    85544 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/redis6.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/control/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25793 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/jobmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/colocated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/modelwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltLauncher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/colocated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/local/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfLauncher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfParser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsLauncher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsParser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmLauncher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmParser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.131744 smartsim-0.4.2/smartsim/_core/launcher/step/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/alpsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/cobaltStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/localStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/lsfStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/mpiStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/pbsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/slurmStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/stepInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/stepMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/taskManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.131744 smartsim-0.4.2/smartsim/_core/launcher/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/launcherUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.135744 smartsim-0.4.2/smartsim/_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.135744 smartsim-0.4.2/smartsim/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40661 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/database/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/entity/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/dbnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/dbobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/entityList.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/error/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/error/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18232 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/torch/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/alpsSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/cobaltSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/lsfSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/mpiSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/mpirunSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/palsSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/pbsSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/slurmSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/tf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/wlm/
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-07 00:28:48.000000 smartsim-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 00:28:48.000000 smartsim-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 00:28:48.000000 smartsim-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    33938 2023-07-07 00:28:52.701927 smartsim-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-07-07 00:28:48.000000 smartsim-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-07 00:28:48.000000 smartsim-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 00:28:52.701927 smartsim-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-07 00:28:48.000000 smartsim-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.689933 smartsim-0.5.0/smartsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/_install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_install/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/_install/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    20354 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_install/buildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/_install/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.689933 smartsim-0.5.0/smartsim/_core/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/bin/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/bin/modules/FindTensorFlow.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71337 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/config/keydb.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   106517 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/config/redis.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/control/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26859 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/control/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/control/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/control/jobmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/control/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/entrypoints/colocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/entrypoints/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/generation/modelwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim/_core/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/colocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/lsf/lsfCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/lsf/lsfLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/lsf/lsfParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/pbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/alpsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/cobaltStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/localStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/lsfStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/mpiStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/pbsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/slurmStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/step/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/stepInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/stepMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/taskManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/launcher/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/util/launcherUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/launcher/util/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/_core/utils/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32544 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/database/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.697929 smartsim-0.5.0/smartsim/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/dbnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/dbobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/entityList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/entity/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/error/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/error/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32850 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/ml/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/tf/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/tf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/ml/torch/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/alpsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/cobaltSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/lsfSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/mpiSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/mpirunSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/palsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/pbsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/settings/slurmSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.701927 smartsim-0.5.0/smartsim/wlm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/wlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/wlm/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-07 00:28:48.000000 smartsim-0.5.0/smartsim/wlm/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:28:52.693931 smartsim-0.5.0/smartsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33938 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 00:28:52.000000 smartsim-0.5.0/smartsim.egg-info/top_level.txt
```

### Comparing `smartsim-0.4.2/LICENSE.md` & `smartsim-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/Makefile` & `smartsim-0.5.0/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,20 @@
 
 # help: check-lint                     - run static analysis checks
 .PHONY: check-lint
 check-lint:
 	@pylint --rcfile=.pylintrc ./smartsim
 
 
+# help: check-mypy                     - run static type check
+.PHONY: check-mypy
+check-mypy:
+	@mypy --config-file=./pyproject.toml
+
+
 # help:
 # help: Documentation
 # help: -------
 
 # help: docs                           - generate project documentation
 .PHONY: docs
 docs:
```

### Comparing `smartsim-0.4.2/PKG-INFO` & `smartsim-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsim
-Version: 0.4.2
+Version: 0.5.0
 Summary: AI Workflows for Science
 Home-page: https://github.com/CrayLabs/SmartSim
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartSim
 Project-URL: Documentation, https://www.craylabs.org
@@ -105,16 +105,16 @@
         
         The documentation has a number of tutorials that make it easy to get used to SmartSim locally
         before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
         # click on link to open jupyter lab
         ```
         
         # SmartSim Infrastructure Library
         
         The Infrastructure Library (IL), the ``smartsim`` python package,
         facilitates the launch of Machine Learning and simulation
@@ -458,15 +458,15 @@
         
         Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
         docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
         ```
         Each of the following examples can be found in the
         [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
         
         ## Online Analysis
         
         Using SmartSim, HPC applications can be monitored in real time by streaming data
@@ -783,8 +783,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: mypy
 Provides-Extra: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.4.2 Summary: AI Workflows for
+Metadata-Version: 2.1 Name: smartsim Version: 0.5.0 Summary: AI Workflows for
 Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
 Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
 License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
 SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
 
@@ -56,16 +56,16 @@
 inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
 (#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
 documentation has a number of tutorials that make it easy to get used to
 SmartSim locally before using it on your system. Each tutorial is a Jupyter
 notebook that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
-ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+ghcr.io/craylabs/smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.1 # click on link to open jupyter lab ``` #
 SmartSim Infrastructure Library The Infrastructure Library (IL), the
 ``smartsim`` python package, facilitates the launch of Machine Learning and
 simulation workflows. The Python interface of the IL creates, configures,
 launches and monitors applications. ## Experiments The [Experiment](https://
 www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
 interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
 api/smartsim_api.html#experiment) users can create references to user
@@ -201,15 +201,15 @@
 smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
 workflows. The following are simple examples of how to use SmartSim and
 SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
 that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
 ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following examples can be
 found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
 getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
 applications can be monitored in real time by streaming data from the
 application to the database. SmartRedis clients can retrieve the data, process,
 analyze it, and finally store any updated data back to the database for use by
 other clients. The following is an example of how a user could monitor and
 analyze a simulation. The example here uses the Python client; however,
@@ -339,8 +339,8 @@
 {Deep learning, Numerical simulation, Climate modeling, High performance
 computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: ml
+markdown Provides-Extra: dev Provides-Extra: mypy Provides-Extra: ml
```

### Comparing `smartsim-0.4.2/README.md` & `smartsim-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
 The documentation has a number of tutorials that make it easy to get used to SmartSim locally
 before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
 [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
 which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
 
 ```bash
-docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
-docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
 # click on link to open jupyter lab
 ```
 
 # SmartSim Infrastructure Library
 
 The Infrastructure Library (IL), the ``smartsim`` python package,
 facilitates the launch of Machine Learning and simulation
@@ -448,15 +448,15 @@
 
 Each tutorial is a Jupyter notebook that can be run through the
 [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
 which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
 
 ```bash
 docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
 ```
 Each of the following examples can be found in the
 [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
 
 ## Online Analysis
 
 Using SmartSim, HPC applications can be monitored in real time by streaming data
```

#### html2text {}

```diff
@@ -51,16 +51,16 @@
 inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
 (#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
 documentation has a number of tutorials that make it easy to get used to
 SmartSim locally before using it on your system. Each tutorial is a Jupyter
 notebook that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
-ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+ghcr.io/craylabs/smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.1 # click on link to open jupyter lab ``` #
 SmartSim Infrastructure Library The Infrastructure Library (IL), the
 ``smartsim`` python package, facilitates the launch of Machine Learning and
 simulation workflows. The Python interface of the IL creates, configures,
 launches and monitors applications. ## Experiments The [Experiment](https://
 www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
 interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
 api/smartsim_api.html#experiment) users can create references to user
@@ -196,15 +196,15 @@
 smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
 workflows. The following are simple examples of how to use SmartSim and
 SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
 that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
 ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following examples can be
 found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
 getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
 applications can be monitored in real time by streaming data from the
 application to the database. SmartRedis clients can retrieve the data, process,
 analyze it, and finally store any updated data back to the database for use by
 other clients. The following is an example of how a user could monitor and
 analyze a simulation. The example here uses the Python client; however,
```

### Comparing `smartsim-0.4.2/pyproject.toml` & `smartsim-0.5.0/smartsim/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,48 +20,17 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import sys
 
-[build-system]
-requires = ["setuptools", "wheel", "cmake>=3.13"]
-build-backend = "setuptools.build_meta"
+# -*- coding: utf-8 -*-
+from .version import __version__ as __version__
 
-[tool.black]
-target-version = ['py37', 'py38']
-exclude = '''
-(
-  | \.egg
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.nox
-  | \.tox
-  | \.venv
-  | _build
-  | build
-  | dist
-  | setup.py
-)
-'''
+if sys.version_info < (3, 8):  # pragma: no cover
+    sys.exit("Python 3.8 or greater must be used with SmartSim.")
 
-[tool.pytest.ini_options]
-log_cli = true
-log_cli_level = "debug"
-
-[tool.isort]
-# supress circular import warning
-skip = ["tests/test_configs/circular_config"]
-
-[tool.coverage.run]
-source = ["smartsim"]
-# see test_configs/*_cov.cfg for "omit"
-
-[tool.coverage.report]
-ignore_errors = true
-# see test_configs/*_cov.cfg for "exclude_lines"
-
-[tool.coverage.html]
-directory = "htmlcov"
+# Main API module
+from .experiment import Experiment
```

### Comparing `smartsim-0.4.2/setup.cfg` & `smartsim-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/setup.py` & `smartsim-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -157,18 +157,17 @@
     def has_ext_modules(_placeholder):
         return True
 
 
 # Define needed dependencies for the installation
 deps = [
     "psutil>=5.7.2",
-    "coloredlogs==10.0",
+    "coloredlogs>=10.0",
     "tabulate>=0.8.9",
-    "redis-py-cluster==2.1.3",
-    "redis==3.5.3",
+    "redis>=4.5",
     "tqdm>=4.50.2",
     "filelock>=3.4.2",
     "protobuf~=3.20",
 ]
 
 # Add SmartRedis at specific version
 deps.append("smartredis>={}".format(versions.SMARTREDIS))
@@ -178,14 +177,23 @@
         "black>=20.8b1",
         "isort>=5.6.4",
         "pylint>=2.6.0",
         "pytest>=6.0.0",
         "pytest-cov>=2.10.1",
         "click==8.0.2",
     ],
+    "mypy": [
+        "mypy>=1.3.0",
+        "types-psutil",
+        "types-redis",
+        "types-tabulate",
+        "types-tqdm",
+        "types-tensorflow",
+        "types-setuptools",
+    ],
     # see smartsim/_core/_install/buildenv.py for more details
     "ml": versions.ml_extras_required(),
 }
 
 
 # rest in setup.cfg
 setup(
```

### Comparing `smartsim-0.4.2/smartsim/__init__.py` & `smartsim-0.5.0/smartsim/_core/_cli/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,11 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import sys
+from smartsim._core._cli.cli import main
 
-# -*- coding: utf-8 -*-
-from .version import __version__ as __version__
-
-if sys.version_info < (3, 8):  # pragma: no cover
-    sys.exit("Python 3.8 or greater must be used with SmartSim.")
-
-# Main API module
-from .experiment import Experiment
+if __name__ == "__main__":
+    main()
```

### Comparing `smartsim-0.4.2/smartsim/_core/__init__.py` & `smartsim-0.5.0/smartsim/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/__init__.py` & `smartsim-0.5.0/smartsim/_core/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/__main__.py` & `smartsim-0.5.0/smartsim/database/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,11 +20,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from smartsim._core._cli.cli import main
-
-if __name__ == "__main__":
-    main()
+from .orchestrator import Orchestrator
```

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/build.py` & `smartsim-0.5.0/smartsim/_core/_cli/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,33 +26,35 @@
 
 import argparse
 import os
 import sys
 from pathlib import Path
 
 import pkg_resources
+import typing as t
 from tabulate import tabulate
 
 from smartsim._core._cli.utils import color_bool, pip_install
 from smartsim._core._install import builder
-from smartsim._core._install.buildenv import BuildEnv, SetupError, Version_, Versioner
+from smartsim._core._install.buildenv import BuildEnv, SetupError, Version_, Versioner, DbEngine
 from smartsim._core._install.builder import BuildError
 from smartsim._core.config import CONFIG
 from smartsim._core.utils.helpers import installed_redisai_backends
 from smartsim.error import SSConfigError
 from smartsim.log import get_logger
 
 smart_logger_format = "[%(name)s] %(levelname)s %(message)s"
 logger = get_logger("Smart", fmt=smart_logger_format)
 
 # NOTE: all smartsim modules need full paths as the smart cli
 #       may be installed into a different directory.
 
 
-def _install_torch_from_pip(versions, device="cpu", verbose=False):
+
+def _install_torch_from_pip(versions: Versioner, device: str = "cpu", verbose: bool = False) -> None:
 
     packages = []
     end_point = None
 
     if sys.platform == "darwin":
         if device == "gpu":
             logger.warning("GPU support is not available on Mac OS X")
@@ -72,15 +74,15 @@
     packages.append(f"torch=={versions.TORCH}{device_suffix}")
     packages.append(f"torchvision=={versions.TORCHVISION}{device_suffix}")
 
     pip_install(packages, end_point=end_point, verbose=verbose)
 
 
 class Build:
-    def __init__(self):
+    def __init__(self) -> None:
         parser = argparse.ArgumentParser()
         parser.add_argument(
             "-v",
             action="store_true",
             default=False,
             help="Enable verbose build process",
         )
@@ -150,34 +152,37 @@
                 logger.info("Only installing Python packages...skipping build")
                 self.build_env = BuildEnv(checks=False)
                 if not args.no_pt:
                     self.install_torch(device=args.device)
             else:
                 logger.info("Checking for build tools...")
                 self.build_env = BuildEnv()
-
+                
                 if self.verbose:
                     logger.info("Build Environment:")
                     env = self.build_env.as_dict()
-                    print(tabulate(env, headers=env.keys(), tablefmt="github"), "\n")
+                    env_vars = list(env.keys())
+                    print(tabulate(env, headers=env_vars, tablefmt="github"), "\n")
+
                 if self.keydb:
                     self.versions.REDIS = Version_("6.2.0")
                     self.versions.REDIS_URL = "https://github.com/EQ-Alpha/KeyDB"
                     self.versions.REDIS_BRANCH = "v6.2.0"
                     CONFIG.conf_path = Path(CONFIG.core_path, "config", "keydb.conf")
                     if not CONFIG.conf_path.resolve().is_file():
                         raise SSConfigError(
                             "Database configuration file at REDIS_CONF could not be found"
                         )
 
                 if self.verbose:
-                    db_name = "KEYDB" if self.keydb else "REDIS"
+                    db_name: DbEngine = "KEYDB" if self.keydb else "REDIS"
                     logger.info("Version Information:")
                     vers = self.versions.as_dict(db_name=db_name)
-                    print(tabulate(vers, headers=vers.keys(), tablefmt="github"), "\n")
+                    version_names = list(vers.keys())
+                    print(tabulate(vers, headers=version_names, tablefmt="github"), "\n")
 
                 # REDIS/KeyDB
                 self.build_database()
 
                 # REDISAI
                 self.build_redis_ai(
                     str(args.device),
@@ -197,15 +202,15 @@
 
         except (SetupError, BuildError) as e:
             logger.error(str(e))
             sys.exit(1)
 
         logger.info("SmartSim build complete!")
 
-    def build_database(self):
+    def build_database(self) -> None:
         # check database installation
         database_name = "KeyDB" if self.keydb else "Redis"
         database_builder = builder.DatabaseBuilder(
             self.build_env(), self.build_env.MALLOC, self.build_env.JOBS, self.verbose
         )
         if not database_builder.is_built:
             logger.info(
@@ -214,16 +219,22 @@
             database_builder.build_from_git(
                 self.versions.REDIS_URL, self.versions.REDIS_BRANCH
             )
             database_builder.cleanup()
         logger.info(f"{database_name} build complete!")
 
     def build_redis_ai(
-        self, device, torch=True, tf=True, onnx=False, torch_dir=None, libtf_dir=None
-    ):
+        self,
+        device: str,
+        torch: bool = True,
+        tf: bool = True,
+        onnx: bool = False,
+        torch_dir: t.Union[str, Path, None] = None,
+        libtf_dir: t.Union[str, Path, None] = None
+    ) -> None:
 
         # make sure user isn't trying to do something silly on MacOS
         if self.build_env.PLATFORM == "darwin" and device == "gpu":
             raise BuildError("SmartSim does not support GPU on MacOS")
 
         # decide which runtimes to build
         print("\nML Backends Requested")
@@ -264,16 +275,16 @@
 
         if tf:
             if libtf_dir:
                 libtf_dir = Path(libtf_dir).resolve()
 
         rai_builder = builder.RedisAIBuilder(
             build_env=self.build_env(),
-            torch_dir=str(torch_dir) if torch_dir else None,
-            libtf_dir=str(libtf_dir) if libtf_dir else None,
+            torch_dir=str(torch_dir) if torch_dir else "",
+            libtf_dir=str(libtf_dir) if libtf_dir else "",
             build_torch=torch,
             build_tf=tf,
             build_onnx=onnx,
             jobs=self.build_env.JOBS,
             verbose=self.verbose,
         )
 
@@ -309,22 +320,22 @@
             # NOTE: have the option to add other builds here in the future
             # like "from_tarball"
             rai_builder.build_from_git(
                 self.versions.REDISAI_URL, self.versions.REDISAI_BRANCH, device
             )
             logger.info("ML Backends and RedisAI build complete!")
 
-    def infer_torch_device(self):
+    def infer_torch_device(self) -> str:
         backend_torch_path = f"{CONFIG.lib_path}/backends/redisai_torch"
         device = "cpu"
         if Path(f"{backend_torch_path}/lib/libtorch_cuda.so").is_file():
             device = "gpu"
         return device
 
-    def install_torch(self, device="cpu"):
+    def install_torch(self, device: str = "cpu") -> None:
         """Torch shared libraries installed by pip are used in the build
         for SmartSim backends so we download them here.
         """
 
         if not self.build_env.check_installed("torch", self.versions.TORCH):
             inferred_device = self.infer_torch_device()
             if (inferred_device == "gpu") and (device == "cpu"):
@@ -349,15 +360,15 @@
                     msg = (
                         "Torch GPU installed in python environment but requested Torch CPU. "
                         + " Run `pip uninstall torch torchvision` and run `smart build` again"
                     )
                     logger.error(msg)  # error because this is usually fatal
             logger.info(f"Torch {self.versions.TORCH} installed in Python environment")
 
-    def check_onnx_install(self):
+    def check_onnx_install(self) -> None:
         """Check Python environment for ONNX installation"""
         if not self.versions.ONNX:
             py_version = sys.version_info
             msg = (
                 "An onnx wheel is not available for "
                 f"Python {py_version.major}.{py_version.minor}. "
                 "Instead consider using Python 3.8 or 3.9 with Onnx "
@@ -376,15 +387,15 @@
             else:
                 logger.info(
                     f"ONNX {self.versions.ONNX} installed in Python environment"
                 )
         except SetupError as e:
             logger.warning(str(e))
 
-    def check_tf_install(self):
+    def check_tf_install(self) -> None:
         """Check Python environment for TensorFlow installation"""
 
         try:
             if not self.build_env.check_installed(
                 "tensorflow", self.versions.TENSORFLOW
             ):
                 msg = (
@@ -395,15 +406,15 @@
             else:
                 logger.info(
                     f"TensorFlow {self.versions.TENSORFLOW} installed in Python environment"
                 )
         except SetupError as e:
             logger.warning(str(e))
 
-    def check_backends_install(self):
+    def check_backends_install(self) -> None:
         """Checks if backends have already been installed.
         Logs details on how to proceed forward
         if the RAI_PATH environment variable is set or if
         backends have already been installed.
         """
         if os.environ.get("RAI_PATH"):
             if installed_redisai_backends():
```

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/clean.py` & `smartsim-0.5.0/smartsim/_core/_cli/clean.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from smartsim.log import get_logger
 
 smart_logger_format = "[%(name)s] %(levelname)s %(message)s"
 logger = get_logger("Smart", fmt=smart_logger_format)
 
 
 class Clean:
-    def __init__(self, clean_all=False):
+    def __init__(self, clean_all: bool = False) -> None:
         parser = argparse.ArgumentParser(
             description="Remove previous ML runtime installation"
         )
         parser.add_argument(
             "--clobber",
             action="store_true",
             default=False,
@@ -48,15 +48,15 @@
         )
         args = parser.parse_args(sys.argv[2:])
 
         self._core_path = get_install_path() / "_core"
         clobber = args.clobber or clean_all
         self.clean(_all=clobber)
 
-    def clean(self, _all=False):
+    def clean(self, _all: bool = False) -> None:
         """Remove pre existing installations of ML runtimes
 
         :param _all: Remove all non-python dependencies
         :type _all: bool, optional
         """
 
         build_temp = self._core_path / ".third-party"
```

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/cli.py` & `smartsim-0.5.0/smartsim/_core/_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 import sys
 
 from smartsim._core._cli.build import Build
 from smartsim._core._cli.clean import Clean
 from smartsim._core._cli.utils import get_install_path
 
 
-def _usage():
+def _usage() -> str:
     usage = [
         "smart <command> [<args>]\n",
         "Commands:",
         "\tbuild       Build SmartSim dependencies (Redis, RedisAI, ML runtimes)",
         "\tclean       Remove previous ML runtime installation",
         "\tclobber     Remove all previous dependency installations",
         "\nDeveloper:",
         "\tsite        Print the installation site of SmartSim",
         "\tdbcli       Print the path to the redis-cli binary" "\n\n",
     ]
     return "\n".join(usage)
 
 
 class SmartCli:
-    def __init__(self):
+    def __init__(self) -> None:
         parser = argparse.ArgumentParser(
             description="SmartSim command line interface", usage=_usage()
         )
 
         parser.add_argument("command", help="Subcommand to run")
 
         # smart
@@ -63,35 +63,35 @@
 
         args = parser.parse_args(sys.argv[1:2])
         if not hasattr(self, args.command):
             parser.print_help()
             sys.exit(0)
         getattr(self, args.command)()
 
-    def build(self):
+    def build(self) -> None:
         Build()
         sys.exit(0)
 
-    def clean(self):
+    def clean(self) -> None:
         Clean()
         sys.exit(0)
 
-    def clobber(self):
+    def clobber(self) -> None:
         Clean(clean_all=True)
         sys.exit(0)
 
-    def site(self):
+    def site(self) -> None:
         print(get_install_path())
         sys.exit(0)
 
-    def dbcli(self):
+    def dbcli(self) -> None:
         bin_path = get_install_path() / "_core" / "bin"
         for option in bin_path.iterdir():
             if option.name in ("redis-cli", "keydb-cli"):
                 print(option)
                 sys.exit(0)
         print("Database (Redis or KeyDB) dependencies not found")
         sys.exit(1)
 
 
-def main():
+def main() -> None:
     SmartCli()
```

### Comparing `smartsim-0.4.2/smartsim/_core/_cli/utils.py` & `smartsim-0.5.0/smartsim/_core/_cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,60 +21,61 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import subprocess
+import typing as t
 from pathlib import Path
 
 from smartsim._core._install.buildenv import SetupError
 from smartsim._core._install.builder import BuildError
 from smartsim._core.utils import colorize
 from smartsim.log import get_logger
 
 smart_logger_format = "[%(name)s] %(levelname)s %(message)s"
 logger = get_logger("Smart", fmt=smart_logger_format)
 
 
-def get_install_path():
+def get_install_path() -> Path:
     try:
         import smartsim as _
     except (ImportError, ModuleNotFoundError):
         raise SetupError("Could not import SmartSim") from None
 
     # find the path to the setup script
     package_path = Path(_.__path__[0]).resolve()
     if not package_path.is_dir():
         raise SetupError("Could not find SmartSim installation site")
 
     return package_path
 
 
-def color_bool(trigger=True):
+def color_bool(trigger: bool = True) -> str:
     _color = "green" if trigger else "red"
     return colorize(str(trigger), color=_color)
 
 
-def pip_install(packages, end_point=None, verbose=False):
+def pip_install(packages: t.List[str], end_point: t.Optional[str] = None, verbose: bool = False) -> None:
     """Install a pip package to be used in the SmartSim build
     Currently only Torch shared libraries are re-used for the build
     """
+    # form pip install command
+    cmd = ["python", "-m", "pip", "install"]
+    cmd.extend(packages)
     if end_point:
-        packages.append(f"-f {end_point}")
-    packages = " ".join(packages)
+        cmd.extend(["-f", end_point])
 
-    # form pip install command
-    cmd = ["python", "-m", "pip", "install", packages]
-    cmd = " ".join(cmd)
+    cmd_arg = " ".join(cmd)
 
     if verbose:
         logger.info(f"Installing packages {packages}...")
     proc = subprocess.Popen(
-        cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        cmd_arg, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     )
     _, err = proc.communicate()
     returncode = int(proc.returncode)
     if returncode != 0:
         error = f"{packages} installation failed with exitcode {returncode}\n"
         error += err.decode("utf-8")
         raise BuildError(error)
```

### Comparing `smartsim-0.4.2/smartsim/_core/_install/__init__.py` & `smartsim-0.5.0/smartsim/_core/_install/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc` & `smartsim-0.5.0/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 12 20:48:40 2023 UTC, .py size: 19671 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,1013 +1,1063 @@
-00000000: 550d 0d0a 0000 0000 2819 3764 d74c 0000  U.......(.7d.L..
+00000000: 550d 0d0a 0000 0000 405c a764 824f 0000  U.......@\.d.O..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
-00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6401 6c09 5a09 6400 6404 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
-00000080: 0100 650a 6a0b 6a0c 5a0c 650a 6a0b 6a0d  ..e.j.j.Z.e.j.j.
-00000090: 5a0d 4700 6405 6406 8400 6406 650e 8303  Z.G.d.d...d.e...
-000000a0: 5a0f 4700 6407 6408 8400 6408 6510 8303  Z.G.d.d...d.e...
-000000b0: 5a11 6409 640a 8400 5a12 4700 640b 640c  Z.d.d...Z.G.d.d.
-000000c0: 8400 640c 6511 8303 5a13 4700 640d 640e  ..d.e...Z.G.d.d.
-000000d0: 8400 640e 8302 5a14 4700 640f 6410 8400  ..d...Z.G.d.d...
-000000e0: 6410 8302 5a15 6401 5300 2911 e900 0000  d...Z.d.S.).....
-000000f0: 004e a901 da04 5061 7468 2901 da08 4974  .N....Path)...It
-00000100: 6572 6162 6c65 2901 da09 7061 636b 6167  erable)...packag
-00000110: 696e 6763 0000 0000 0000 0000 0000 0000  ingc............
-00000120: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
-00000130: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
-00000140: 0029 03da 0a53 6574 7570 4572 726f 7261  .)...SetupErrora
-00000150: 0f02 0000 4120 7369 6d70 6c65 2065 7863  ....A simple exc
-00000160: 6570 7469 6f6e 2063 6c61 7373 2066 6f72  eption class for
-00000170: 2065 7272 6f72 7320 696e 205f 696e 7374   errors in _inst
-00000180: 616c 6c2e 6275 696c 6465 6e76 2066 696c  all.buildenv fil
-00000190: 652e 0a20 2020 2054 6869 7320 6973 2070  e..    This is p
-000001a0: 7269 6d61 7269 6c79 2075 7365 6420 746f  rimarily used to
-000001b0: 2069 6e74 6572 7275 7074 2074 6865 2073   interrupt the s
-000001c0: 6574 7570 2e70 7920 6275 696c 6420 696e  etup.py build in
-000001d0: 2063 6173 650a 2020 2020 6f66 2061 2066   case.    of a f
-000001e0: 6169 6c75 7265 2c20 616e 6420 6973 2063  ailure, and is c
-000001f0: 6175 6768 7420 6672 6571 7565 6e74 6c79  aught frequently
-00000200: 2069 6e20 7468 6520 434c 4920 7768 6963   in the CLI whic
-00000210: 6820 6174 7465 6d70 7473 0a20 2020 2074  h attempts.    t
-00000220: 6f20 7375 7070 7265 7373 2061 6e64 206c  o suppress and l
-00000230: 6f67 2074 6865 2065 7272 6f72 7320 7468  og the errors th
-00000240: 726f 776e 2068 6572 652e 0a0a 2020 2020  rown here...    
-00000250: 4f6e 6520 6e6f 7465 2069 7320 7468 6174  One note is that
-00000260: 2074 6869 7320 6572 726f 7220 6d75 7374   this error must
-00000270: 2062 6520 696d 706f 7274 6564 2066 726f   be imported fro
-00000280: 6d20 6865 7265 2074 6f20 6265 0a20 2020  m here to be.   
-00000290: 2063 6175 6768 7420 616e 6420 6e6f 7420   caught and not 
-000002a0: 6465 6669 6e65 6420 616e 7977 6865 7265  defined anywhere
-000002b0: 2065 6c73 652e 2053 696e 6365 2077 6520   else. Since we 
-000002c0: 7573 6520 7468 6973 2063 6c61 7373 0a20  use this class. 
-000002d0: 2020 2069 6e20 7468 6520 696e 7374 616c     in the instal
-000002e0: 6c61 7469 6f6e 2c20 6861 7669 6e67 2061  lation, having a
-000002f0: 2073 6570 6172 6174 6520 6572 726f 7220   separate error 
-00000300: 6669 6c65 2077 6f75 6c64 206d 6561 6e0a  file would mean.
-00000310: 2020 2020 616e 6f74 6865 7220 6d6f 6475      another modu
-00000320: 6c65 2074 6f20 6d61 6e75 616c 6c79 2069  le to manually i
-00000330: 6d70 6f72 7420 696e 746f 2073 6574 7570  mport into setup
-00000340: 2e70 790a 0a20 2020 2053 6565 2073 6574  .py..    See set
-00000350: 7570 2e70 7920 666f 7220 6d6f 7265 0a20  up.py for more. 
-00000360: 2020 204e 2904 da08 5f5f 6e61 6d65 5f5f     N)...__name__
-00000370: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000380: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000390: 635f 5fa9 0072 0b00 0000 720b 0000 00fa  c__..r....r.....
-000003a0: 472f 686f 6d65 2f72 756e 6e65 722f 776f  G/home/runner/wo
-000003b0: 726b 2f53 6d61 7274 5369 6d2f 536d 6172  rk/SmartSim/Smar
-000003c0: 7453 696d 2f73 6d61 7274 7369 6d2f 5f63  tSim/smartsim/_c
-000003d0: 6f72 652f 5f69 6e73 7461 6c6c 2f62 7569  ore/_install/bui
-000003e0: 6c64 656e 762e 7079 7206 0000 002f 0000  ldenv.pyr..../..
-000003f0: 0073 0400 0000 0801 040d 7206 0000 0063  .s........r....c
-00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0300 0000 0000 0000 7388 0000 0065 005a  ........s....e.Z
-00000420: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
-00000430: 0465 0564 0464 0584 0083 015a 0665 0564  .e.d.d.....Z.e.d
-00000440: 0664 0784 0083 015a 0765 0564 0864 0984  .d.....Z.e.d.d..
-00000450: 0083 015a 0865 0564 0a64 0b84 0083 015a  ...Z.e.d.d.....Z
-00000460: 0987 0066 0164 0c64 0d84 085a 0a87 0066  ...f.d.d...Z...f
-00000470: 0164 0e64 0f84 085a 0b87 0066 0164 1064  .d.d...Z...f.d.d
-00000480: 1184 085a 0c87 0066 0164 1264 1384 085a  ...Z...f.d.d...Z
-00000490: 0d87 0066 0164 1464 1584 085a 0e87 0004  ...f.d.d...Z....
-000004a0: 005a 0f53 0029 16da 0856 6572 7369 6f6e  .Z.S.)...Version
-000004b0: 5f7a 7841 2073 7562 636c 6173 7320 6f66  _zxA subclass of
-000004c0: 2070 6b67 5f72 6573 6f75 7263 6573 2e70   pkg_resources.p
-000004d0: 6163 6b61 6769 6e67 2e76 6572 7369 6f6e  ackaging.version
-000004e0: 2e56 6572 7369 6f6e 2074 6861 740a 2020  .Version that.  
-000004f0: 2020 696e 636c 7564 6573 2073 6f6d 6520    includes some 
-00000500: 6865 6c70 6572 206d 6574 686f 6473 2066  helper methods f
-00000510: 6f72 2063 6f6d 7061 7269 6e67 2076 6572  or comparing ver
-00000520: 7369 6f6e 732e 0a20 2020 2063 0200 0000  sions..    c....
-00000530: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000540: 4300 0000 734e 0000 0074 007c 0174 0183  C...sN...t.|.t..
-00000550: 0272 0e7c 0153 0074 007c 0174 0283 0272  .r.|.S.t.|.t...r
-00000560: 2074 017c 0183 0153 0074 007c 0174 0383   t.|...S.t.|.t..
-00000570: 0272 4274 0164 01a0 0464 0264 0384 007c  .rBt.d...d.d...|
-00000580: 0144 0083 01a1 0183 0153 0074 057c 0183  .D.......S.t.|..
-00000590: 0182 0164 0053 0029 044e da01 2e63 0100  ...d.S.).N...c..
-000005a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000005b0: 0000 7300 0000 7316 0000 007c 005d 0e7d  ..s...s....|.].}
-000005c0: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
-000005d0: 00a9 014e 2901 da03 7374 7229 02da 022e  ...N)...str)....
-000005e0: 30da 0469 7465 6d72 0b00 0000 720b 0000  0..itemr....r...
-000005f0: 0072 0c00 0000 da09 3c67 656e 6578 7072  .r......<genexpr
-00000600: 3e4c 0000 0073 0400 0000 0400 0200 7a2f  >L...s........z/
-00000610: 5665 7273 696f 6e5f 2e5f 636f 6e76 6572  Version_._conver
-00000620: 745f 746f 5f76 6572 7369 6f6e 2e3c 6c6f  t_to_version.<lo
-00000630: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
-00000640: 06da 0a69 7369 6e73 7461 6e63 65da 0756  ...isinstance..V
-00000650: 6572 7369 6f6e 7210 0000 0072 0400 0000  ersionr....r....
-00000660: da04 6a6f 696e da0e 496e 7661 6c69 6456  ..join..InvalidV
-00000670: 6572 7369 6f6e 2902 da04 7365 6c66 da04  ersion)...self..
-00000680: 7665 7273 720b 0000 0072 0b00 0000 720c  versr....r....r.
-00000690: 0000 00da 135f 636f 6e76 6572 745f 746f  ....._convert_to
-000006a0: 5f76 6572 7369 6f6e 4600 0000 730e 0000  _versionF...s...
-000006b0: 0000 010a 0104 010a 0108 010a 0118 027a  ...............z
-000006c0: 1c56 6572 7369 6f6e 5f2e 5f63 6f6e 7665  .Version_._conve
-000006d0: 7274 5f74 6f5f 7665 7273 696f 6e63 0100  rt_to_versionc..
-000006e0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-000006f0: 0000 4300 0000 731a 0000 0074 0074 01a0  ..C...s....t.t..
-00000700: 027c 00a1 016a 03a0 0464 01a1 0164 0219  .|...j...d...d..
-00000710: 0083 0153 0029 034e 720e 0000 0072 0100  ...S.).Nr....r..
-00000720: 0000 a905 da03 696e 74da 0d70 6b67 5f72  ......int..pkg_r
-00000730: 6573 6f75 7263 6573 da0d 7061 7273 655f  esources..parse_
-00000740: 7665 7273 696f 6eda 0c62 6173 655f 7665  version..base_ve
-00000750: 7273 696f 6eda 0573 706c 6974 a901 7218  rsion..split..r.
-00000760: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000770: 0000 da05 6d61 6a6f 7250 0000 0073 0200  ....majorP...s..
-00000780: 0000 0004 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
-00000790: 616a 6f72 6301 0000 0000 0000 0000 0000  ajorc...........
-000007a0: 0001 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
-000007b0: 0000 7400 7401 a002 7c00 a101 6a03 a004  ..t.t...|...j...
-000007c0: 6401 a101 6402 1900 8301 5300 2903 4e72  d...d.....S.).Nr
-000007d0: 0e00 0000 e901 0000 0072 1b00 0000 7221  .........r....r!
-000007e0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-000007f0: 0000 da05 6d69 6e6f 7256 0000 0073 0200  ....minorV...s..
-00000800: 0000 0002 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
-00000810: 696e 6f72 6301 0000 0000 0000 0000 0000  inorc...........
-00000820: 0001 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
-00000830: 0000 7400 7401 a002 7c00 a101 6a03 a004  ..t.t...|...j...
-00000840: 6401 a101 6402 1900 8301 5300 a903 4e72  d...d.....S...Nr
-00000850: 0e00 0000 e902 0000 0072 1b00 0000 7221  .........r....r!
-00000860: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000870: 0000 da05 6d69 6372 6f5a 0000 0073 0200  ....microZ...s..
-00000880: 0000 0002 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
-00000890: 6963 726f 6301 0000 0000 0000 0000 0000  icroc...........
-000008a0: 0001 0000 0004 0000 0043 0000 0073 1800  .........C...s..
-000008b0: 0000 7400 7401 a002 7c00 a101 8301 a003  ..t.t...|.......
-000008c0: 6401 a101 6402 1900 5300 7225 0000 0029  d...d...S.r%...)
-000008d0: 0472 1000 0000 721d 0000 0072 1e00 0000  .r....r....r....
-000008e0: 7220 0000 0072 2100 0000 720b 0000 0072  r ...r!...r....r
-000008f0: 0b00 0000 720c 0000 00da 0570 6174 6368  ....r......patch
-00000900: 5e00 0000 7302 0000 0000 037a 0e56 6572  ^...s......z.Ver
-00000910: 7369 6f6e 5f2e 7061 7463 6863 0200 0000  sion_.patchc....
-00000920: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-00000930: 0300 0000 733c 0000 007a 1674 007c 0083  ....s<...z.t.|..
-00000940: 01a0 017c 00a0 027c 01a1 01a1 0157 0053  ...|...|.....W.S
-00000950: 0004 0074 036b 0a72 3601 0001 0001 0074  ...t.k.r6......t
-00000960: 0483 00a0 017c 01a1 0106 0059 0053 0058  .....|.....Y.S.X
-00000970: 0064 0053 0072 0f00 0000 2905 7215 0000  .d.S.r....).r...
-00000980: 00da 065f 5f67 745f 5f72 1a00 0000 7217  ...__gt__r....r.
-00000990: 0000 00da 0573 7570 6572 a902 7218 0000  .....super..r...
-000009a0: 005a 0363 6d70 a901 da09 5f5f 636c 6173  .Z.cmp....__clas
-000009b0: 735f 5f72 0b00 0000 720c 0000 0072 2900  s__r....r....r).
-000009c0: 0000 6300 0000 7308 0000 0000 0102 0116  ..c...s.........
-000009d0: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
-000009e0: 6774 5f5f 6302 0000 0000 0000 0000 0000  gt__c...........
-000009f0: 0002 0000 0008 0000 0003 0000 0073 3c00  .............s<.
-00000a00: 0000 7a16 7400 7c00 8301 a001 7c00 a002  ..z.t.|.....|...
-00000a10: 7c01 a101 a101 5700 5300 0400 7403 6b0a  |.....W.S...t.k.
-00000a20: 7236 0100 0100 0100 7404 8300 a001 7c01  r6......t.....|.
-00000a30: a101 0600 5900 5300 5800 6400 5300 720f  ....Y.S.X.d.S.r.
-00000a40: 0000 0029 0572 1500 0000 da06 5f5f 6c74  ...).r......__lt
-00000a50: 5f5f 721a 0000 0072 1700 0000 722a 0000  __r....r....r*..
-00000a60: 0072 2b00 0000 722c 0000 0072 0b00 0000  .r+...r,...r....
-00000a70: 720c 0000 0072 2e00 0000 6900 0000 7308  r....r....i...s.
-00000a80: 0000 0000 0102 0116 010e 017a 0f56 6572  ...........z.Ver
-00000a90: 7369 6f6e 5f2e 5f5f 6c74 5f5f 6302 0000  sion_.__lt__c...
-00000aa0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00000ab0: 0003 0000 0073 3c00 0000 7a16 7400 7c00  .....s<...z.t.|.
-00000ac0: 8301 a001 7c00 a002 7c01 a101 a101 5700  ....|...|.....W.
-00000ad0: 5300 0400 7403 6b0a 7236 0100 0100 0100  S...t.k.r6......
-00000ae0: 7404 8300 a001 7c01 a101 0600 5900 5300  t.....|.....Y.S.
-00000af0: 5800 6400 5300 720f 0000 0029 0572 1500  X.d.S.r....).r..
-00000b00: 0000 da06 5f5f 6571 5f5f 721a 0000 0072  ....__eq__r....r
-00000b10: 1700 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
-00000b20: 0000 0072 0b00 0000 720c 0000 0072 2f00  ...r....r....r/.
-00000b30: 0000 6f00 0000 7308 0000 0000 0102 0116  ..o...s.........
-00000b40: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
-00000b50: 6571 5f5f 6302 0000 0000 0000 0000 0000  eq__c...........
-00000b60: 0002 0000 0008 0000 0003 0000 0073 3c00  .............s<.
-00000b70: 0000 7a16 7400 7c00 8301 a001 7c00 a002  ..z.t.|.....|...
-00000b80: 7c01 a101 a101 5700 5300 0400 7403 6b0a  |.....W.S...t.k.
-00000b90: 7236 0100 0100 0100 7404 8300 a001 7c01  r6......t.....|.
-00000ba0: a101 0600 5900 5300 5800 6400 5300 720f  ....Y.S.X.d.S.r.
-00000bb0: 0000 0029 0572 1500 0000 da06 5f5f 6765  ...).r......__ge
-00000bc0: 5f5f 721a 0000 0072 1700 0000 722a 0000  __r....r....r*..
-00000bd0: 0072 2b00 0000 722c 0000 0072 0b00 0000  .r+...r,...r....
-00000be0: 720c 0000 0072 3000 0000 7500 0000 7308  r....r0...u...s.
-00000bf0: 0000 0000 0102 0116 010e 017a 0f56 6572  ...........z.Ver
-00000c00: 7369 6f6e 5f2e 5f5f 6765 5f5f 6302 0000  sion_.__ge__c...
-00000c10: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00000c20: 0003 0000 0073 3c00 0000 7a16 7400 7c00  .....s<...z.t.|.
-00000c30: 8301 a001 7c00 a002 7c01 a101 a101 5700  ....|...|.....W.
-00000c40: 5300 0400 7403 6b0a 7236 0100 0100 0100  S...t.k.r6......
-00000c50: 7404 8300 a001 7c01 a101 0600 5900 5300  t.....|.....Y.S.
-00000c60: 5800 6400 5300 720f 0000 0029 0572 1500  X.d.S.r....).r..
-00000c70: 0000 da06 5f5f 6c65 5f5f 721a 0000 0072  ....__le__r....r
-00000c80: 1700 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
-00000c90: 0000 0072 0b00 0000 720c 0000 0072 3100  ...r....r....r1.
-00000ca0: 0000 7b00 0000 7308 0000 0000 0102 0116  ..{...s.........
-00000cb0: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
-00000cc0: 6c65 5f5f 2910 7207 0000 0072 0800 0000  le__).r....r....
-00000cd0: 7209 0000 0072 0a00 0000 721a 0000 00da  r....r....r.....
-00000ce0: 0870 726f 7065 7274 7972 2200 0000 7224  .propertyr"...r$
-00000cf0: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00000d00: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
-00000d10: 0072 3100 0000 da0d 5f5f 636c 6173 7363  .r1.....__classc
-00000d20: 656c 6c5f 5f72 0b00 0000 720b 0000 0072  ell__r....r....r
-00000d30: 2c00 0000 720c 0000 0072 0d00 0000 4100  ,...r....r....A.
-00000d40: 0000 731e 0000 0008 0104 0408 0a02 010a  ..s.............
-00000d50: 0502 010a 0302 010a 0302 010a 040c 060c  ................
-00000d60: 060c 060c 0672 0d00 0000 6302 0000 0000  .....r....c.....
-00000d70: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000d80: 0000 0073 0e00 0000 7400 6a01 a002 7c00  ...s....t.j...|.
-00000d90: 7c01 a102 5300 720f 0000 0029 03da 026f  |...S.r....)...o
-00000da0: 73da 0765 6e76 6972 6f6e da03 6765 7429  s..environ..get)
-00000db0: 02da 0376 6172 da07 6465 6661 756c 7472  ...var..defaultr
-00000dc0: 0b00 0000 720b 0000 0072 0c00 0000 da07  ....r....r......
-00000dd0: 6765 745f 656e 7682 0000 0073 0200 0000  get_env....s....
-00000de0: 0001 7239 0000 0063 0000 0000 0000 0000  ..r9...c........
-00000df0: 0000 0000 0000 0000 0b00 0000 4000 0000  ............@...
-00000e00: 73bc 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000e10: 0364 0264 0364 0464 0564 0664 0764 0864  .d.d.d.d.d.d.d.d
-00000e20: 0964 0a64 0b9c 0964 0c64 0d64 0e64 0e64  .d.d...d.d.d.d.d
-00000e30: 0f64 0d64 0864 1064 1164 0b9c 0964 129c  .d.d.d.d.d...d..
-00000e40: 025a 0465 056a 0664 136b 0572 8a65 04a0  .Z.e.j.d.k.r.e..
-00000e50: 0764 14a1 0101 0065 0464 1519 00a0 0764  .d.....e.d.....d
-00000e60: 16a1 0101 0065 0464 1519 00a0 0764 17a1  .....e.d.....d..
-00000e70: 0101 0065 0464 1519 00a0 0764 18a1 0101  ...e.d.....d....
-00000e80: 0065 0464 1519 00a0 0764 19a1 0101 0065  .e.d.....d.....e
-00000e90: 056a 0864 1a6b 0272 a065 04a0 0764 1464  .j.d.k.r.e...d.d
-00000ea0: 1ba1 0201 0064 1c64 1d84 005a 0964 1e64  .....d.d...Z.d.d
-00000eb0: 1f84 005a 0a64 2064 2184 005a 0b64 1b53  ...Z.d d!..Z.d.S
-00000ec0: 0029 22da 0e52 6564 6973 4149 5665 7273  .)"..RedisAIVers
-00000ed0: 696f 6e61 ff01 0000 4120 7375 6263 6c61  iona....A subcla
-00000ee0: 7373 206f 6620 5665 7273 696f 6e5f 2074  ss of Version_ t
-00000ef0: 6861 7420 686f 6c64 7320 7468 6520 6465  hat holds the de
-00000f00: 7065 6e64 656e 6379 2073 6574 7320 666f  pendency sets fo
-00000f10: 7220 5265 6469 7341 490a 0a20 2020 2074  r RedisAI..    t
-00000f20: 6869 7320 636c 6173 7320 7365 7276 6573  his class serves
-00000f30: 2074 776f 2070 7572 706f 7365 733a 0a0a   two purposes:..
-00000f40: 2020 2020 312e 2049 7420 6973 2075 7365      1. It is use
-00000f50: 6420 746f 2070 6f70 756c 6174 6520 7468  d to populate th
-00000f60: 6520 5b6d 6c5d 2060 6065 7874 7261 735f  e [ml] ``extras_
-00000f70: 7265 7175 6972 6560 6020 6f66 2074 6865  require`` of the
-00000f80: 2073 6574 7570 2e70 792e 0a20 2020 2054   setup.py..    T
-00000f90: 6869 7320 6973 2062 6563 6175 7365 2074  his is because t
-00000fa0: 6865 2052 6564 6973 4149 2076 6572 7369  he RedisAI versi
-00000fb0: 6f6e 2077 696c 6c20 6465 7465 726d 696e  on will determin
-00000fc0: 6520 7768 6963 6820 4d4c 2062 6173 6564  e which ML based
-00000fd0: 0a20 2020 2064 6570 656e 6465 6e63 6965  .    dependencie
-00000fe0: 7320 6172 6520 7265 7175 6972 6564 2e0a  s are required..
-00000ff0: 0a20 2020 2032 2e20 5573 6564 2074 6f20  .    2. Used to 
-00001000: 7365 7420 7468 6520 6465 6661 756c 7420  set the default 
-00001010: 7661 6c75 6573 2066 6f72 2050 7954 6f72  values for PyTor
-00001020: 6368 2c20 5446 2c20 616e 6420 4f4e 4e58  ch, TF, and ONNX
-00001030: 0a20 2020 2067 6976 656e 2074 6865 2053  .    given the S
-00001040: 4d41 5254 5349 4d5f 5245 4449 5341 4920  MARTSIM_REDISAI 
-00001050: 656e 7620 7661 7220 7365 7420 6279 2074  env var set by t
-00001060: 6865 2075 7365 722e 0a0a 2020 2020 4e4f  he user...    NO
-00001070: 5445 3a20 546f 7263 6820 7265 7175 6972  TE: Torch requir
-00001080: 6573 2061 6464 6974 696f 6e61 6c20 696e  es additional in
-00001090: 666f 726d 6174 696f 6e20 6465 7065 6e64  formation depend
-000010a0: 696e 6720 6f6e 2077 6865 7468 6572 0a20  ing on whether. 
-000010b0: 2020 2043 5055 206f 7220 4750 5520 7375     CPU or GPU su
-000010c0: 7070 6f72 7420 6973 2072 6571 7565 7374  pport is request
-000010d0: 6564 0a20 2020 207a 0532 2e36 2e32 7a05  ed.    z.2.6.2z.
-000010e0: 312e 392e 307a 0631 2e31 302e 337a 0631  1.9.0z.1.10.3z.1
-000010f0: 2e31 302e 307a 0531 2e30 2e32 7a05 312e  .10.0z.1.0.2z.1.
-00001100: 392e 317a 042b 6370 757a 062b 6375 3131  9.1z.+cpuz.+cu11
-00001110: 317a 0630 2e31 302e 3129 09da 0a74 656e  1z.0.10.1)...ten
-00001120: 736f 7266 6c6f 77da 046f 6e6e 78da 0873  sorflow..onnx..s
-00001130: 6b6c 326f 6e6e 78da 0b6f 6e6e 786d 6c74  kl2onnx..onnxmlt
-00001140: 6f6f 6c73 fa0c 7363 696b 6974 2d6c 6561  ools..scikit-lea
-00001150: 726e da05 746f 7263 68da 1074 6f72 6368  rn..torch..torch
-00001160: 5f63 7075 5f73 7566 6669 78da 1174 6f72  _cpu_suffix..tor
-00001170: 6368 5f63 7564 615f 7375 6666 6978 da0b  ch_cuda_suffix..
-00001180: 746f 7263 6876 6973 696f 6e7a 0532 2e38  torchvisionz.2.8
-00001190: 2e30 7a06 312e 3131 2e30 7a06 312e 3131  .0z.1.11.0z.1.11
-000011a0: 2e31 7a05 312e 312e 317a 062b 6375 3131  .1z.1.1.1z.+cu11
-000011b0: 337a 0630 2e31 322e 3029 02fa 0531 2e32  3z.0.12.0)...1.2
-000011c0: 2e35 fa05 312e 322e 3729 02e9 0300 0000  .5..1.2.7)......
-000011d0: e90a 0000 0072 4400 0000 7245 0000 0072  .....rD...rE...r
-000011e0: 3c00 0000 723d 0000 0072 3e00 0000 723f  <...r=...r>...r?
-000011f0: 0000 00da 0664 6172 7769 6e4e 6302 0000  .....darwinNc...
-00001200: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-00001210: 0043 0000 0073 6c00 0000 7400 6401 6402  .C...sl...t.d.d.
-00001220: 8400 7c00 6a01 4400 8301 8301 7d02 7c02  ..|.j.D.....}.|.
-00001230: 7c01 6b04 722a 7402 6403 7c02 9b00 9d02  |.k.r*t.d.|.....
-00001240: 8301 8201 7c01 7c00 6a01 6b07 7262 7c01  ....|.|.j.k.rb|.
-00001250: a003 6404 a101 7246 6405 7c00 5f04 7168  ..d...rFd.|._.qh
-00001260: 7402 6406 7c01 9b00 6407 7c00 6a01 a005  t.d.|...d.|.j...
-00001270: a100 9b00 9d04 8301 8201 6e06 7c01 7c00  ..........n.|.|.
-00001280: 5f04 6400 5300 2908 4e63 0100 0000 0000  _.d.S.).Nc......
-00001290: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-000012a0: 0000 7316 0000 007c 005d 0e7d 0174 007c  ..s....|.].}.t.|
-000012b0: 0183 0156 0001 0071 0264 0053 0072 0f00  ...V...q.d.S.r..
-000012c0: 0000 2901 720d 0000 0029 0272 1100 0000  ..).r....).r....
-000012d0: da03 7665 7272 0b00 0000 720b 0000 0072  ..verr....r....r
-000012e0: 0c00 0000 7213 0000 00ba 0000 0073 0400  ....r........s..
-000012f0: 0000 0400 0200 7a2a 5265 6469 7341 4956  ......z*RedisAIV
-00001300: 6572 7369 6f6e 2e5f 5f69 6e69 745f 5f2e  ersion.__init__.
-00001310: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00001320: 723e 7a31 5265 6469 7341 4920 7665 7273  r>z1RedisAI vers
-00001330: 696f 6e20 6d75 7374 2062 6520 6772 6561  ion must be grea
-00001340: 7465 7220 7468 616e 206f 7220 6571 7561  ter than or equa
-00001350: 6c20 746f 207a 0331 2e32 7245 0000 007a  l to z.1.2rE...z
-00001360: 1849 6e76 616c 6964 2052 6564 6973 4149  .Invalid RedisAI
-00001370: 2076 6572 7369 6f6e 207a 0e2e 204f 7074   version z.. Opt
-00001380: 696f 6e73 2061 7265 2029 06da 036d 696e  ions are )...min
-00001390: da08 6465 6661 756c 7473 7206 0000 00da  ..defaultsr.....
-000013a0: 0a73 7461 7274 7377 6974 68da 0776 6572  .startswith..ver
-000013b0: 7369 6f6e da04 6b65 7973 2903 7218 0000  sion..keys).r...
-000013c0: 0072 1900 0000 5a0f 6d69 6e5f 7261 695f  .r....Z.min_rai_
-000013d0: 7665 7273 696f 6e72 0b00 0000 720b 0000  versionr....r...
-000013e0: 0072 0c00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
-000013f0: b900 0000 7318 0000 0000 0114 0108 0102  ....s...........
-00001400: 0108 ff04 030a 010a 0308 0202 0114 ff06  ................
-00001410: 047a 1752 6564 6973 4149 5665 7273 696f  .z.RedisAIVersio
-00001420: 6e2e 5f5f 696e 6974 5f5f 6302 0000 0000  n.__init__c.....
-00001430: 0000 0000 0000 0002 0000 0009 0000 0043  ...............C
-00001440: 0000 0073 4a00 0000 7a12 7c00 6a00 7c00  ...sJ...z.|.j.|.
-00001450: 6a01 1900 7c01 1900 5700 5300 0400 7402  j...|...W.S...t.
-00001460: 6b0a 7244 0100 0100 0100 7403 6401 7404  k.rD......t.d.t.
-00001470: 7c00 8301 6a05 9b00 6402 7c01 9b00 6403  |...j...d.|...d.
-00001480: 9d05 8301 6400 8202 5900 6e02 5800 6400  ....d...Y.n.X.d.
-00001490: 5300 2904 4efa 0127 7a1b 2720 6f62 6a65  S.).N..'z.' obje
-000014a0: 6374 2068 6173 206e 6f20 6174 7472 6962  ct has no attrib
-000014b0: 7574 6520 277a e427 0a0a 5468 6973 2069  ute 'z.'..This i
-000014c0: 7320 6c69 6b65 6c79 2061 2070 726f 626c  s likely a probl
-000014d0: 656d 2077 6974 6820 7468 6520 536d 6172  em with the Smar
-000014e0: 7453 696d 2062 7569 6c64 2070 726f 6365  tSim build proce
-000014f0: 7373 3b69 6620 7468 6973 2070 726f 626c  ss;if this probl
-00001500: 656d 2070 6572 7369 7374 7320 706c 6561  em persists plea
-00001510: 7365 206c 6f67 2061 206e 6577 2069 7373  se log a new iss
-00001520: 7565 2061 7420 6874 7470 733a 2f2f 6769  ue at https://gi
-00001530: 7468 7562 2e63 6f6d 2f43 7261 794c 6162  thub.com/CrayLab
-00001540: 732f 536d 6172 7453 696d 2f69 7373 7565  s/SmartSim/issue
-00001550: 7320 6f72 2067 6574 2069 6e20 636f 6e74  s or get in cont
-00001560: 6163 7420 7769 7468 2075 7320 6174 2068  act with us at h
-00001570: 7474 7073 3a2f 2f77 7777 2e63 7261 796c  ttps://www.crayl
-00001580: 6162 732e 6f72 672f 646f 6373 2f63 6f6d  abs.org/docs/com
-00001590: 6d75 6e69 7479 2e68 746d 6c29 0672 4b00  munity.html).rK.
-000015a0: 0000 724d 0000 00da 084b 6579 4572 726f  ..rM.....KeyErro
-000015b0: 72da 0e41 7474 7269 6275 7465 4572 726f  r..AttributeErro
-000015c0: 72da 0474 7970 6572 0700 0000 2902 7218  r..typer....).r.
-000015d0: 0000 00da 046e 616d 6572 0b00 0000 720b  .....namer....r.
-000015e0: 0000 0072 0c00 0000 da0b 5f5f 6765 7461  ...r......__geta
-000015f0: 7474 725f 5fcb 0000 0073 1000 0000 0001  ttr__....s......
-00001600: 0201 1201 0e01 0201 16ff 0207 02f9 7a1a  ..............z.
-00001610: 5265 6469 7341 4956 6572 7369 6f6e 2e5f  RedisAIVersion._
-00001620: 5f67 6574 6174 7472 5f5f 6301 0000 0000  _getattr__c.....
-00001630: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00001640: 0000 0073 1000 0000 7c00 6a00 7c00 6a01  ...s....|.j.|.j.
-00001650: 1900 a002 a100 5300 720f 0000 0029 0372  ......S.r....).r
-00001660: 4b00 0000 724d 0000 00da 0463 6f70 7972  K...rM.....copyr
-00001670: 2100 0000 720b 0000 0072 0b00 0000 720c  !...r....r....r.
-00001680: 0000 00da 0c67 6574 5f64 6566 6175 6c74  .....get_default
-00001690: 73d8 0000 0073 0200 0000 0001 7a1b 5265  s....s......z.Re
-000016a0: 6469 7341 4956 6572 7369 6f6e 2e67 6574  disAIVersion.get
-000016b0: 5f64 6566 6175 6c74 7329 0c72 0700 0000  _defaults).r....
-000016c0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-000016d0: 4b00 0000 da03 7379 73da 0c76 6572 7369  K.....sys..versi
-000016e0: 6f6e 5f69 6e66 6fda 0370 6f70 da08 706c  on_info..pop..pl
-000016f0: 6174 666f 726d 724f 0000 0072 5500 0000  atformrO...rU...
-00001700: 7257 0000 0072 0b00 0000 720b 0000 0072  rW...r....r....r
-00001710: 0b00 0000 720c 0000 0072 3a00 0000 8600  ....r....r:.....
-00001720: 0000 7342 0000 0008 0104 1102 0102 0102  ..sB............
-00001730: 0102 0102 0102 0102 0102 0102 f704 0c02  ................
-00001740: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00001750: f704 f406 190a 010a 010e 010e 010e 010e  ................
-00001760: 020a 010c 0208 1208 0d72 3a00 0000 6300  .........r:...c.
-00001770: 0000 0000 0000 0000 0000 0000 0000 0008  ................
-00001780: 0000 0040 0000 0073 2201 0000 6500 5a01  ...@...s"...e.Z.
-00001790: 6400 5a02 6401 5a03 6504 6402 8301 5a05  d.Z.d.Z.e.d...Z.
-000017a0: 6504 6506 6403 6404 8302 8301 5a07 6504  e.e.d.d.....Z.e.
-000017b0: 6506 6405 6406 8302 8301 5a08 6506 6407  e.d.d.....Z.e.d.
-000017c0: 6408 8302 5a09 6504 6506 6409 640a 8302  d...Z.e.e.d.d...
-000017d0: 8301 5a0a 6506 640b 640c 8302 5a0b 6506  ..Z.e.d.d...Z.e.
-000017e0: 640d 650a 8302 5a0c 650d 6506 640e 640f  d.e...Z.e.e.d.d.
-000017f0: 8302 8301 5a0e 6506 6410 6411 8302 5a0f  ....Z.e.d.d...Z.
-00001800: 6506 6412 6413 650e 9b00 9d02 8302 5a10  e.d.d.e.......Z.
-00001810: 6504 6506 6414 650e 6a11 8302 8301 5a12  e.e.d.e.j.....Z.
-00001820: 6504 6506 6415 650e 6a13 8302 8301 5a14  e.e.d.e.j.....Z.
-00001830: 6504 6506 6416 650e 6a15 8302 8301 5a16  e.e.d.e.j.....Z.
-00001840: 6504 6506 6417 650e 6a17 8302 8301 5a18  e.e.d.e.j.....Z.
-00001850: 6504 650e 6a19 8301 5a1a 7a0e 6504 650e  e.e.j...Z.z.e.e.
-00001860: 6a1b 8301 5a1c 5700 6e18 0400 651d 6b0a  j...Z.W.n...e.k.
-00001870: 72f4 0100 0100 0100 6418 5a1c 5900 6e02  r.......d.Z.Y.n.
-00001880: 5800 6423 641a 641b 8401 5a1e 641c 641d  X.d#d.d...Z.d.d.
-00001890: 8400 5a1f 6520 641e 9c01 641f 6420 8404  ..Z.e d...d.d ..
-000018a0: 5a21 6421 6422 8400 5a22 6418 5300 2924  Z!d!d"..Z"d.S.)$
-000018b0: da09 5665 7273 696f 6e65 7261 6c03 0000  ..Versioneral...
-000018c0: 5665 7273 696f 6e65 7220 6973 2072 6573  Versioner is res
-000018d0: 706f 6e73 6962 6c65 2066 6f72 206d 616e  ponsible for man
-000018e0: 6167 696e 6720 616c 6c20 7468 6520 7665  aging all the ve
-000018f0: 7273 696f 6e73 0a20 2020 2077 6974 6869  rsions.    withi
-00001900: 6e20 536d 6172 7453 696d 2069 6e63 6c75  n SmartSim inclu
-00001910: 6469 6e67 2053 6d61 7274 5369 6d20 6974  ding SmartSim it
-00001920: 7365 6c66 2e0a 0a20 2020 2053 6d61 7274  self...    Smart
-00001930: 5369 6d27 7320 7665 7273 696f 6e20 6973  Sim's version is
-00001940: 2077 7269 7474 656e 2069 6e74 6f20 7665   written into ve
-00001950: 7273 696f 6e2e 7079 2075 706f 6e20 7069  rsion.py upon pi
-00001960: 7020 696e 7374 616c 6c0a 2020 2020 6279  p install.    by
-00001970: 2075 7369 6e67 2074 6869 7320 636c 6173   using this clas
-00001980: 7320 696e 2073 6574 7570 2e70 792e 2042  s in setup.py. B
-00001990: 7920 7365 7474 696e 6720 534d 4152 5453  y setting SMARTS
-000019a0: 494d 5f53 5546 4649 582c 0a20 2020 2074  IM_SUFFIX,.    t
-000019b0: 6865 2076 6572 7369 6f6e 2077 696c 6c20  he version will 
-000019c0: 6265 2077 7269 7474 656e 2061 7320 6120  be written as a 
-000019d0: 2264 6972 7479 2220 7665 7273 696f 6e20  "dirty" version 
-000019e0: 7769 7468 2074 6865 0a20 2020 2067 6974  with the.    git
-000019f0: 2d73 6861 2061 7070 656e 6465 642e 0a20  -sha appended.. 
-00001a00: 2020 2069 2e65 2e0a 2020 2020 2020 2020     i.e..        
-00001a10: 6578 706f 7274 2053 4d41 5254 5349 4d5f  export SMARTSIM_
-00001a20: 5355 4646 4958 3d6e 6967 6874 6c79 0a20  SUFFIX=nightly. 
-00001a30: 2020 2020 2020 2070 6970 2069 6e73 7461         pip insta
-00001a40: 6c6c 202d 6520 2e0a 2020 2020 2020 2020  ll -e ..        
-00001a50: 736d 6172 7473 696d 2e5f 5f76 6572 7369  smartsim.__versi
-00001a60: 6f6e 5f5f 203d 3d20 302e 332e 322b 6e69  on__ == 0.3.2+ni
-00001a70: 6768 746c 792d 3366 6532 3366 660a 0a20  ghtly-3fe23ff.. 
-00001a80: 2020 2056 6572 7369 6f6e 6572 206d 616e     Versioner man
-00001a90: 6167 6573 2074 6869 7264 2070 6172 7479  ages third party
-00001aa0: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
-00001ab0: 6420 7468 6569 7220 7665 7273 696f 6e73  d their versions
-00001ac0: 0a20 2020 2061 7320 7765 6c6c 2e20 5468  .    as well. Th
-00001ad0: 6573 6520 7665 7273 696f 6e73 2061 7265  ese versions are
-00001ae0: 2075 7365 6420 6279 2074 6865 2060 6073   used by the ``s
-00001af0: 6d61 7274 6060 2063 6c69 2069 6e20 7468  mart`` cli in th
-00001b00: 650a 2020 2020 6060 736d 6172 7420 6275  e.    ``smart bu
-00001b10: 696c 6460 6020 636f 6d6d 616e 6420 746f  ild`` command to
-00001b20: 2064 6574 6572 6d69 6e65 2077 6869 6368   determine which
-00001b30: 2064 6570 656e 6465 6e63 7920 7665 7273   dependency vers
-00001b40: 696f 6e73 0a20 2020 2074 6f20 6c6f 6f6b  ions.    to look
-00001b50: 2066 6f72 2061 6e64 2064 6f77 6e6c 6f61   for and downloa
-00001b60: 642e 0a0a 2020 2020 4465 6661 756c 7420  d...    Default 
-00001b70: 7665 7273 696f 6e73 2066 6f72 2053 6d61  versions for Sma
-00001b80: 7274 5369 6d2c 2053 6d61 7274 5265 6469  rtSim, SmartRedi
-00001b90: 732c 2052 6564 6973 2c20 616e 6420 5265  s, Redis, and Re
-00001ba0: 6469 7341 4920 6172 650a 2020 2020 616c  disAI are.    al
-00001bb0: 6c20 7365 7420 6865 7265 2e20 5365 7474  l set here. Sett
-00001bc0: 696e 6720 6120 6465 6661 756c 7420 7665  ing a default ve
-00001bd0: 7273 696f 6e20 666f 7220 5265 6469 7341  rsion for RedisA
-00001be0: 4920 616c 736f 2064 6963 7461 7465 730a  I also dictates.
-00001bf0: 2020 2020 6465 6661 756c 7420 7665 7273      default vers
-00001c00: 696f 6e73 206f 6620 7468 6520 6d61 6368  ions of the mach
-00001c10: 696e 6520 6c65 6172 6e69 6e67 206c 6962  ine learning lib
-00001c20: 7261 7269 6573 2e0a 2020 2020 7a05 332e  raries..    z.3.
-00001c30: 382e 305a 1053 4d41 5254 5349 4d5f 5645  8.0Z.SMARTSIM_VE
-00001c40: 5253 494f 4e7a 0530 2e34 2e32 5a12 534d  RSIONz.0.4.2Z.SM
-00001c50: 4152 5452 4544 4953 5f56 4552 5349 4f4e  ARTREDIS_VERSION
-00001c60: 7a05 302e 342e 30da 0f53 4d41 5254 5349  z.0.4.0..SMARTSI
-00001c70: 4d5f 5355 4646 4958 da00 5a0e 534d 4152  M_SUFFIX..Z.SMAR
-00001c80: 5453 494d 5f52 4544 4953 7a05 372e 302e  TSIM_REDISz.7.0.
-00001c90: 355a 1253 4d41 5254 5349 4d5f 5245 4449  5Z.SMARTSIM_REDI
-00001ca0: 535f 5552 4c7a 2368 7474 7073 3a2f 2f67  S_URLz#https://g
-00001cb0: 6974 6875 622e 636f 6d2f 7265 6469 732f  ithub.com/redis/
-00001cc0: 7265 6469 732e 6769 742f 5a15 534d 4152  redis.git/Z.SMAR
-00001cd0: 5453 494d 5f52 4544 4953 5f42 5241 4e43  TSIM_REDIS_BRANC
-00001ce0: 485a 1053 4d41 5254 5349 4d5f 5245 4449  HZ.SMARTSIM_REDI
-00001cf0: 5341 4972 4500 0000 5a14 534d 4152 5453  SAIrE...Z.SMARTS
-00001d00: 494d 5f52 4544 4953 4149 5f55 524c 7a27  IM_REDISAI_URLz'
-00001d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001d20: 6f6d 2f52 6564 6973 4149 2f52 6564 6973  om/RedisAI/Redis
-00001d30: 4149 2e67 6974 2f5a 1753 4d41 5254 5349  AI.git/Z.SMARTSI
-00001d40: 4d5f 5245 4449 5341 495f 4252 414e 4348  M_REDISAI_BRANCH
-00001d50: da01 765a 0e53 4d41 5254 5349 4d5f 544f  ..vZ.SMARTSIM_TO
-00001d60: 5243 485a 1153 4d41 5254 5349 4d5f 544f  RCHZ.SMARTSIM_TO
-00001d70: 5243 4856 4953 da10 544f 5243 485f 4350  RCHVIS..TORCH_CP
-00001d80: 555f 5355 4646 4958 da11 544f 5243 485f  U_SUFFIX..TORCH_
-00001d90: 4355 4441 5f53 5546 4649 584e da05 5245  CUDA_SUFFIXN..RE
-00001da0: 4449 5363 0200 0000 0000 0000 0000 0000  DISc............
-00001db0: 0500 0000 0600 0000 4300 0000 7356 0000  ........C...sV..
-00001dc0: 0064 0164 027c 0164 0364 0464 0567 067d  .d.d.|.d.d.d.g.}
-00001dd0: 027c 006a 007c 006a 017c 006a 027c 006a  .|.j.|.j.|.j.|.j
-00001de0: 037c 006a 047c 006a 0567 067d 037c 006a  .|.j.|.j.g.}.|.j
-00001df0: 0672 487c 02a0 0764 06a1 0101 007c 03a0  .rH|...d.....|..
-00001e00: 077c 006a 06a1 0101 007c 027c 0364 079c  .|.j.....|.|.d..
-00001e10: 027d 047c 0453 0029 084e da08 534d 4152  .}.|.S.).N..SMAR
-00001e20: 5453 494d da0a 534d 4152 5452 4544 4953  TSIM..SMARTREDIS
-00001e30: da07 5245 4449 5341 49da 0554 4f52 4348  ..REDISAI..TORCH
-00001e40: da0a 5445 4e53 4f52 464c 4f57 da04 4f4e  ..TENSORFLOW..ON
-00001e50: 4e58 2902 5a08 5061 636b 6167 6573 5a08  NX).Z.PackagesZ.
-00001e60: 5665 7273 696f 6e73 2908 7263 0000 0072  Versions).rc...r
-00001e70: 6400 0000 7262 0000 0072 6500 0000 7266  d...rb...re...rf
-00001e80: 0000 0072 6700 0000 7268 0000 00da 0661  ...rg...rh.....a
-00001e90: 7070 656e 6429 0572 1800 0000 5a07 6462  ppend).r....Z.db
-00001ea0: 5f6e 616d 65da 0870 6163 6b61 6765 73da  _name..packages.
-00001eb0: 0876 6572 7369 6f6e 7372 1900 0000 720b  .versionsr....r.
-00001ec0: 0000 0072 0b00 0000 720c 0000 00da 0761  ...r....r......a
-00001ed0: 735f 6469 6374 1801 0000 7326 0000 0000  s_dict....s&....
-00001ee0: 0202 0102 0102 0102 0102 0102 fa04 0904  ................
-00001ef0: 0104 0104 0104 0104 0104 fa04 0806 010a  ................
-00001f00: 010c 010a 017a 1156 6572 7369 6f6e 6572  .....z.Versioner
-00001f10: 2e61 735f 6469 6374 6301 0000 0000 0000  .as_dictc.......
-00001f20: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
-00001f30: 0073 3c00 0000 7c00 6a00 a001 a100 7d01  .s<...|.j.....}.
-00001f40: 6401 6402 6403 6404 6704 7d02 7c02 4400  d.d.d.d.g.}.|.D.
-00001f50: 5d0e 7d03 7c01 a002 7c03 a101 0100 711a  ].}.|...|.....q.
-00001f60: 6405 6406 8400 7c01 a003 a100 4400 8301  d.d...|.....D...
-00001f70: 5300 2907 7a74 4f70 7469 6f6e 616c 204d  S.).ztOptional M
-00001f80: 4c2f 444c 2064 6570 656e 6465 6e63 6965  L/DL dependencie
-00001f90: 7320 7765 2073 7567 6765 7374 2066 6f72  s we suggest for
-00001fa0: 2074 6865 2075 7365 722e 0a0a 2020 2020   the user...    
-00001fb0: 2020 2020 5468 6520 6465 6661 756c 7473      The defaults
-00001fc0: 2061 7265 2062 6173 6564 206f 6e20 7468   are based on th
-00001fd0: 6520 5265 6469 7341 4920 7665 7273 696f  e RedisAI versio
-00001fe0: 6e0a 2020 2020 2020 2020 7240 0000 0072  n.        r@...r
-00001ff0: 4300 0000 7241 0000 0072 4200 0000 6301  C...rA...rB...c.
-00002000: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00002010: 0000 0053 0000 0073 1e00 0000 6700 7c00  ...S...s....g.|.
-00002020: 5d16 5c02 7d01 7d02 7c01 9b00 6400 7c02  ].\.}.}.|...d.|.
-00002030: 9b00 9d03 9102 7104 5300 2901 7a02 3d3d  ......q.S.).z.==
-00002040: 720b 0000 0029 0372 1100 0000 da03 6c69  r....).r......li
-00002050: 6272 1900 0000 720b 0000 0072 0b00 0000  br....r....r....
-00002060: 720c 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00002070: 3e44 0100 0073 0400 0000 0600 0600 7a30  >D...s........z0
-00002080: 5665 7273 696f 6e65 722e 6d6c 5f65 7874  Versioner.ml_ext
-00002090: 7261 735f 7265 7175 6972 6564 2e3c 6c6f  ras_required.<lo
-000020a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000020b0: 2904 7265 0000 0072 5700 0000 725a 0000  ).re...rW...rZ..
-000020c0: 00da 0569 7465 6d73 2904 7218 0000 005a  ...items).r....Z
-000020d0: 0b6d 6c5f 6465 6661 756c 7473 5a0d 5f74  .ml_defaultsZ._t
-000020e0: 6f72 6368 5f66 6965 6c64 73da 0566 6965  orch_fields..fie
-000020f0: 6c64 720b 0000 0072 0b00 0000 720c 0000  ldr....r....r...
-00002100: 00da 126d 6c5f 6578 7472 6173 5f72 6571  ...ml_extras_req
-00002110: 7569 7265 642f 0100 0073 1200 0000 0005  uired/...s......
-00002120: 0a08 0201 0201 0201 02fc 0406 0801 0c02  ................
-00002130: 7a1c 5665 7273 696f 6e65 722e 6d6c 5f65  z.Versioner.ml_e
-00002140: 7874 7261 735f 7265 7175 6972 6564 2901  xtras_required).
-00002150: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
-00002160: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00002170: 0073 4800 0000 7a2c 7400 6a01 6401 6402  .sH...z,t.j.d.d.
-00002180: 6403 6703 7c01 6404 8d02 a002 6405 a101  d.g.|.d.....d...
-00002190: a003 a100 7d02 7c02 6406 6407 8502 1900  ....}.|.d.d.....
-000021a0: 5700 5300 0400 7404 6b0a 7242 0100 0100  W.S...t.k.rB....
-000021b0: 0100 5900 6408 5300 5800 6406 5300 2909  ..Y.d.S.X.d.S.).
-000021c0: 7a25 4765 7420 7468 6520 6769 7420 7368  z%Get the git sh
-000021d0: 6120 6f66 2074 6865 2063 7572 7265 6e74  a of the current
-000021e0: 2062 7261 6e63 68da 0367 6974 7a09 7265   branch..gitz.re
-000021f0: 762d 7061 7273 655a 0448 4541 4429 01da  v-parseZ.HEAD)..
-00002200: 0363 7764 da05 6173 6369 694e e907 0000  .cwd..asciiN....
-00002210: 0072 5e00 0000 2905 da0a 7375 6270 726f  .r^...)...subpro
-00002220: 6365 7373 da0c 6368 6563 6b5f 6f75 7470  cess..check_outp
-00002230: 7574 da06 6465 636f 6465 da05 7374 7269  ut..decode..stri
-00002240: 70da 0945 7863 6570 7469 6f6e 2903 7218  p..Exception).r.
-00002250: 0000 00da 0c73 6574 7570 5f70 795f 6469  .....setup_py_di
-00002260: 725a 0373 6861 720b 0000 0072 0b00 0000  rZ.shar....r....
-00002270: 720c 0000 00da 0767 6574 5f73 6861 4601  r......get_shaF.
-00002280: 0000 7310 0000 0000 0202 0214 0102 ff06  ..s.............
-00002290: ff02 050e 010e 027a 1156 6572 7369 6f6e  .......z.Version
-000022a0: 6572 2e67 6574 5f73 6861 6302 0000 0000  er.get_shac.....
-000022b0: 0000 0000 0000 0006 0000 0009 0000 0043  ...............C
-000022c0: 0000 0073 8e00 0000 7c00 6a00 7d02 7c00  ...s....|.j.}.|.
-000022d0: 6a01 7242 7c00 a002 7c01 a101 7d03 7c03  j.rB|...|...}.|.
-000022e0: 7232 7c02 9b00 6401 7c00 6a01 9b00 6402  r2|...d.|.j...d.
-000022f0: 7c03 9b00 9d05 7d02 6e10 7c02 9b00 6401  |.....}.n.|...d.
-00002300: 7c00 6a01 9b00 9d03 7d02 7c01 6403 1b00  |.j.....}.|.d...
-00002310: 6404 1b00 7d04 7403 7c04 6405 8302 8f2c  d...}.t.|.d....,
-00002320: 7d05 7c05 a004 6406 a101 0100 7c05 a004  }.|...d.....|...
-00002330: 6407 a101 0100 7c05 a004 6408 7c02 9b00  d.....|...d.|...
-00002340: 6409 9d03 a101 0100 5700 3500 5100 5200  d.......W.5.Q.R.
-00002350: 5800 7c02 5300 290a 7a83 0a20 2020 2020  X.|.S.).z..     
-00002360: 2020 2057 7269 7465 2076 6572 7369 6f6e     Write version
-00002370: 2069 6e66 6f20 746f 2076 6572 7369 6f6e   info to version
-00002380: 2e70 790a 0a20 2020 2020 2020 2055 7365  .py..        Use
-00002390: 2067 6974 5f73 6861 2069 6e20 7468 6520   git_sha in the 
-000023a0: 6361 7365 2077 6865 7265 2073 6d61 7274  case where smart
-000023b0: 7369 6d20 7375 6666 6978 2069 7320 7365  sim suffix is se
-000023c0: 7420 696e 2074 6865 2065 6e76 6972 6f6e  t in the environ
-000023d0: 6d65 6e74 0a20 2020 2020 2020 20fa 012b  ment.        ..+
-000023e0: 720e 0000 00da 0873 6d61 7274 7369 6d7a  r......smartsimz
-000023f0: 0a76 6572 7369 6f6e 2e70 79da 0177 7a33  .version.py..wz3
-00002400: 2320 5468 6973 2066 696c 6520 6973 2061  # This file is a
-00002410: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
-00002420: 6572 6174 6564 2062 7920 7365 7475 702e  erated by setup.
-00002430: 7079 0a7a 2323 2064 6f20 6e6f 7420 6564  py.z## do not ed
-00002440: 6974 2074 6869 7320 6669 6c65 206d 616e  it this file man
-00002450: 7561 6c6c 792e 0a0a 7a0f 5f5f 7665 7273  ually...z.__vers
-00002460: 696f 6e5f 5f20 3d20 277a 0227 0a29 0572  ion__ = 'z.'.).r
-00002470: 6300 0000 725d 0000 0072 7d00 0000 da04  c...r]...r}.....
-00002480: 6f70 656e da05 7772 6974 6529 0672 1800  open..write).r..
-00002490: 0000 727c 0000 0072 4d00 0000 5a07 6769  ..r|...rM...Z.gi
-000024a0: 745f 7368 615a 0c76 6572 7369 6f6e 5f66  t_shaZ.version_f
-000024b0: 696c 65da 0166 720b 0000 0072 0b00 0000  ile..fr....r....
-000024c0: 720c 0000 00da 0d77 7269 7465 5f76 6572  r......write_ver
-000024d0: 7369 6f6e 5301 0000 7318 0000 0000 0606  sionS...s.......
-000024e0: 0106 010a 0104 0118 0310 020c 010c 010a  ................
-000024f0: 010a 021c 017a 1756 6572 7369 6f6e 6572  .....z.Versioner
-00002500: 2e77 7269 7465 5f76 6572 7369 6f6e 2901  .write_version).
-00002510: 7262 0000 0029 2372 0700 0000 7208 0000  rb...)#r....r...
-00002520: 0072 0900 0000 720a 0000 0072 0d00 0000  .r....r....r....
-00002530: da0a 5059 5448 4f4e 5f4d 494e 7239 0000  ..PYTHON_MINr9..
-00002540: 0072 6300 0000 7264 0000 0072 5d00 0000  .rc...rd...r]...
-00002550: 7262 0000 00da 0952 4544 4953 5f55 524c  rb.....REDIS_URL
-00002560: 5a0c 5245 4449 535f 4252 414e 4348 723a  Z.REDIS_BRANCHr:
-00002570: 0000 0072 6500 0000 5a0b 5245 4449 5341  ...re...Z.REDISA
-00002580: 495f 5552 4c5a 0e52 4544 4953 4149 5f42  I_URLZ.REDISAI_B
-00002590: 5241 4e43 4872 4000 0000 7266 0000 0072  RANCHr@...rf...r
-000025a0: 4300 0000 5a0b 544f 5243 4856 4953 494f  C...Z.TORCHVISIO
-000025b0: 4e72 4100 0000 7260 0000 0072 4200 0000  NrA...r`...rB...
-000025c0: 7261 0000 0072 3b00 0000 7267 0000 0072  ra...r;...rg...r
-000025d0: 3c00 0000 7268 0000 0072 5200 0000 726c  <...rh...rR...rl
-000025e0: 0000 0072 7100 0000 7210 0000 0072 7d00  ...rq...r....r}.
-000025f0: 0000 7284 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00002600: 0072 0b00 0000 720c 0000 0072 5c00 0000  .r....r....r\...
-00002610: dc00 0000 733a 0000 0008 0104 1708 030e  ....s:..........
-00002620: 010e 010a 030e 010a 010a 030e 0102 0102  ................
-00002630: 0002 ff04 0310 0410 0110 0110 0102 010a  ................
-00002640: ff04 060a 0102 010e 010e 010a 020a 1708  ................
-00002650: 170e 0d72 5c00 0000 6300 0000 0000 0000  ...r\...c.......
-00002660: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00002670: 0073 f000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002680: 5a03 6504 6a05 a006 6402 6403 a102 5a07  Z.e.j...d.d...Z.
-00002690: 6504 6a05 a006 6404 6405 a102 5a08 6504  e.j...d.d...Z.e.
-000026a0: 6a05 a006 6406 6407 a102 5a09 6504 6a05  j...d.d...Z.e.j.
-000026b0: a006 6408 6407 a102 5a0a 6504 6a05 a006  ..d.d...Z.e.j...
-000026c0: 6409 640a a102 5a0b 6504 6a05 a006 640b  d.d...Z.e.j...d.
-000026d0: 640c a102 5a0c 650d 6504 6a05 a006 640d  d...Z.e.e.j...d.
-000026e0: 640e a102 8301 5a0e 650f 6a10 5a11 6429  d.....Z.e.j.Z.d)
-000026f0: 6410 6411 8401 5a12 6412 6413 8400 5a13  d.d...Z.d.d...Z.
-00002700: 6414 6415 8400 5a14 6416 6417 8400 5a15  d.d...Z.d.d...Z.
-00002710: 6516 6418 6419 8400 8301 5a17 641a 641b  e.d.d.....Z.d.d.
-00002720: 8400 5a18 641c 641d 8400 5a19 641e 641f  ..Z.d.d...Z.d.d.
-00002730: 8400 5a1a 6516 6420 6421 8400 8301 5a1b  ..Z.e.d d!....Z.
-00002740: 651c 6422 6423 8400 8301 5a1d 6424 6425  e.d"d#....Z.d$d%
-00002750: 8400 5a1e 651c 642a 6427 6428 8401 8301  ..Z.e.d*d'd(....
-00002760: 5a1f 6426 5300 292b da08 4275 696c 6445  Z.d&S.)+..BuildE
-00002770: 6e76 6137 0200 0045 6e76 6972 6f6e 6d65  nva7...Environme
-00002780: 6e74 2066 6f72 2062 7569 6c64 696e 6720  nt for building 
-00002790: 7468 6972 642d 7061 7274 7920 6465 7065  third-party depe
-000027a0: 6e64 656e 6369 6573 0a0a 2020 2020 4275  ndencies..    Bu
-000027b0: 696c 6445 6e76 2070 726f 7669 6465 7320  ildEnv provides 
-000027c0: 6120 6d65 7468 6f64 2066 6f72 2063 6f6e  a method for con
-000027d0: 6669 6775 7269 6e67 2068 6f77 2074 6865  figuring how the
-000027e0: 2074 6869 7264 2d70 6172 7479 0a20 2020   third-party.   
-000027f0: 2064 6570 656e 6465 6e63 6965 7320 7769   dependencies wi
-00002800: 7468 696e 2053 6d61 7274 5369 6d20 6172  thin SmartSim ar
-00002810: 6520 6275 696c 742c 206e 616d 656c 7920  e built, namely 
-00002820: 5265 6469 732f 4b65 7944 420a 2020 2020  Redis/KeyDB.    
-00002830: 616e 6420 5265 6469 7341 492e 0a0a 2020  and RedisAI...  
-00002840: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
-00002850: 7420 7661 7269 6162 6c65 7320 6c69 7374  t variables list
-00002860: 6564 2068 6572 6520 6361 6e20 6265 2073  ed here can be s
-00002870: 6574 2074 6f20 636f 6e74 726f 6c20 7468  et to control th
-00002880: 650a 2020 2020 5265 6469 7320 6275 696c  e.    Redis buil
-00002890: 6420 696e 2074 6865 2070 6970 2077 6865  d in the pip whe
-000028a0: 656c 2062 7569 6c64 2061 7320 7765 6c6c  el build as well
-000028b0: 2061 7320 7468 6520 5265 6469 7320 616e   as the Redis an
-000028c0: 6420 5265 6469 7341 490a 2020 2020 6275  d RedisAI.    bu
-000028d0: 696c 6420 6578 6563 7574 6564 2062 7920  ild executed by 
-000028e0: 7468 6520 434c 492e 0a0a 2020 2020 4275  the CLI...    Bu
-000028f0: 696c 6420 746f 6f6c 7320 6172 6520 616c  ild tools are al
-00002900: 736f 2063 6865 636b 6564 2066 6f72 2068  so checked for h
-00002910: 6572 6520 616e 6420 6966 2074 6865 7920  ere and if they 
-00002920: 6172 6520 6e6f 7420 666f 756e 640a 2020  are not found.  
-00002930: 2020 7468 656e 2061 2053 6574 7570 4572    then a SetupEr
-00002940: 726f 7220 6973 2072 6169 7365 642e 0a0a  ror is raised...
-00002950: 2020 2020 4164 6469 6e67 2074 6865 202d      Adding the -
-00002960: 7620 666c 6167 2074 6f20 6060 736d 6172  v flag to ``smar
-00002970: 7420 6275 696c 6460 6020 7769 6c6c 2073  t build`` will s
-00002980: 686f 7720 7468 6520 6275 696c 6420 656e  how the build en
-00002990: 7669 726f 6e6d 656e 740a 2020 2020 6265  vironment.    be
-000029a0: 696e 6720 7573 6564 2e0a 2020 2020 da02  ing used..    ..
-000029b0: 4343 5a03 6763 63da 0343 5858 7a03 672b  CCZ.gcc..CXXz.g+
-000029c0: 2bda 0643 464c 4147 5372 5e00 0000 da08  +..CFLAGSr^.....
-000029d0: 4358 5846 4c41 4753 da06 4d41 4c4c 4f43  CXXFLAGS..MALLOC
-000029e0: da04 6c69 6263 5a0a 4255 494c 445f 4a4f  ..libcZ.BUILD_JO
-000029f0: 4253 7223 0000 005a 094e 4f5f 4348 4543  BSr#...Z.NO_CHEC
-00002a00: 4b53 7201 0000 0054 6302 0000 0000 0000  KSr....Tc.......
-00002a10: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00002a20: 0073 1000 0000 7c01 720c 7c00 a000 a100  .s....|.r.|.....
-00002a30: 0100 6400 5300 720f 0000 0029 01da 1263  ..d.S.r....)...c
-00002a40: 6865 636b 5f64 6570 656e 6465 6e63 6965  heck_dependencie
-00002a50: 7329 0272 1800 0000 da06 6368 6563 6b73  s).r......checks
-00002a60: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00002a70: 4f00 0000 8b01 0000 7304 0000 0000 0104  O.......s.......
-00002a80: 017a 1142 7569 6c64 456e 762e 5f5f 696e  .z.BuildEnv.__in
-00002a90: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00002aa0: 0003 0000 0007 0000 0043 0000 0073 3c00  .........C...s<.
-00002ab0: 0000 6401 6402 6403 6404 6405 7c00 6a00  ..d.d.d.d.d.|.j.
-00002ac0: 7c00 6a01 6707 7d01 7402 7c00 6a03 8301  |.j.g.}.t.|.j...
-00002ad0: 6406 6b02 7238 7c01 4400 5d0e 7d02 7c00  d.k.r8|.D.].}.|.
-00002ae0: a004 7c02 a101 0100 7128 6400 5300 2907  ..|.....q(d.S.).
-00002af0: 4e72 7300 0000 7a07 6769 742d 6c66 73da  Nrs...z.git-lfs.
-00002b00: 046d 616b 655a 0477 6765 745a 0563 6d61  .makeZ.wgetZ.cma
-00002b10: 6b65 7201 0000 0029 0572 8800 0000 7289  ker....).r....r.
-00002b20: 0000 0072 1c00 0000 da06 4348 4543 4b53  ...r......CHECKS
-00002b30: da16 6368 6563 6b5f 6275 696c 645f 6465  ..check_build_de
-00002b40: 7065 6e64 656e 6379 2903 7218 0000 00da  pendency).r.....
-00002b50: 0464 6570 73da 0364 6570 720b 0000 0072  .deps..depr....r
-00002b60: 0b00 0000 720c 0000 0072 8e00 0000 8f01  ....r....r......
-00002b70: 0000 7308 0000 0000 0116 010e 0108 017a  ..s............z
-00002b80: 1b42 7569 6c64 456e 762e 6368 6563 6b5f  .BuildEnv.check_
-00002b90: 6465 7065 6e64 656e 6369 6573 6301 0000  dependenciesc...
-00002ba0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00002bb0: 0043 0000 0073 2a00 0000 7400 6a01 a002  .C...s*...t.j...
-00002bc0: a100 7d01 7c01 a003 7c00 6a04 7c00 6a05  ..}.|...|.j.|.j.
-00002bd0: 7c00 6a06 7c00 6a07 6401 9c04 a101 0100  |.j.|.j.d.......
-00002be0: 7c01 5300 2902 4e29 0472 8800 0000 7289  |.S.).N).r....r.
-00002bf0: 0000 0072 8a00 0000 728b 0000 0029 0872  ...r....r....).r
-00002c00: 3400 0000 7235 0000 0072 5600 0000 da06  4...r5...rV.....
-00002c10: 7570 6461 7465 7288 0000 0072 8900 0000  updater....r....
-00002c20: 728a 0000 0072 8b00 0000 2902 7218 0000  r....r....).r...
-00002c30: 00da 0365 6e76 720b 0000 0072 0b00 0000  ...envr....r....
-00002c40: 720c 0000 00da 085f 5f63 616c 6c5f 5f95  r......__call__.
-00002c50: 0100 0073 1200 0000 0002 0a01 0402 0401  ...s............
-00002c60: 0401 0401 04fc 04ff 0408 7a11 4275 696c  ..........z.Buil
-00002c70: 6445 6e76 2e5f 5f63 616c 6c5f 5f63 0100  dEnv.__call__c..
-00002c80: 0000 0000 0000 0000 0000 0400 0000 0800  ................
-00002c90: 0000 4300 0000 7346 0000 0064 0164 0264  ..C...sF...d.d.d
-00002ca0: 0364 0464 0564 0664 0764 0867 087d 017c  .d.d.d.d.d.g.}.|
-00002cb0: 006a 007c 006a 017c 006a 027c 006a 037c  .j.|.j.|.j.|.j.|
-00002cc0: 006a 047c 006a 057c 006a 067c 006a 0767  .j.|.j.|.j.|.j.g
-00002cd0: 087d 027c 017c 0264 099c 027d 037c 0353  .}.|.|.d...}.|.S
-00002ce0: 0029 0a4e 7288 0000 0072 8900 0000 728a  .).Nr....r....r.
-00002cf0: 0000 0072 8b00 0000 728c 0000 00da 044a  ...r....r......J
-00002d00: 4f42 535a 0e50 5954 484f 4e5f 5645 5253  OBSZ.PYTHON_VERS
-00002d10: 494f 4eda 0850 4c41 5446 4f52 4d29 02da  ION..PLATFORM)..
-00002d20: 0b45 6e76 6972 6f6e 6d65 6e74 5a06 5661  .EnvironmentZ.Va
-00002d30: 6c75 6573 2908 7288 0000 0072 8900 0000  lues).r....r....
-00002d40: 728a 0000 0072 8b00 0000 728c 0000 0072  r....r....r....r
-00002d50: 9800 0000 da0e 7079 7468 6f6e 5f76 6572  ......python_ver
-00002d60: 7369 6f6e 7299 0000 0029 0472 1800 0000  sionr....).r....
-00002d70: da09 7661 7269 6162 6c65 73da 0676 616c  ..variables..val
-00002d80: 7565 7372 9600 0000 720b 0000 0072 0b00  uesr....r....r..
-00002d90: 0000 720c 0000 0072 6c00 0000 a201 0000  ..r....rl.......
-00002da0: 7328 0000 0000 0202 0102 0102 0102 0102  s(..............
-00002db0: 0102 0102 0102 f804 0b04 0104 0104 0104  ................
-00002dc0: 0104 0104 0104 0104 f804 0a0a 017a 1042  .............z.B
-00002dd0: 7569 6c64 456e 762e 6173 5f64 6963 7463  uildEnv.as_dictc
-00002de0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002df0: 0200 0000 4300 0000 7308 0000 0074 00a0  ....C...s....t..
-00002e00: 01a1 0053 0072 0f00 0000 2902 725b 0000  ...S.r....).r[..
-00002e10: 0072 9b00 0000 7221 0000 0072 0b00 0000  .r....r!...r....
-00002e20: 720b 0000 0072 0c00 0000 729b 0000 00ba  r....r....r.....
-00002e30: 0100 0073 0200 0000 0002 7a17 4275 696c  ...s......z.Buil
-00002e40: 6445 6e76 2e70 7974 686f 6e5f 7665 7273  dEnv.python_vers
-00002e50: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
-00002e60: 0400 0000 0600 0000 4300 0000 732c 0000  ........C...s,..
-00002e70: 0074 006a 017d 0274 027c 026a 039b 0064  .t.j.}.t.|.j...d
-00002e80: 017c 026a 049b 0064 017c 026a 059b 009d  .|.j...d.|.j....
-00002e90: 0583 017d 037c 037c 016b 0453 0029 027a  ...}.|.|.k.S.).z
-00002ea0: 2244 6574 6563 7420 6966 2073 7973 7465  "Detect if syste
-00002eb0: 6d20 5079 7468 6f6e 2069 7320 746f 6f20  m Python is too 
-00002ec0: 6f6c 6472 0e00 0000 2906 7258 0000 0072  oldr....).rX...r
-00002ed0: 5900 0000 720d 0000 0072 2200 0000 7224  Y...r....r"...r$
-00002ee0: 0000 0072 2700 0000 2904 7218 0000 005a  ...r'...).r....Z
-00002ef0: 0a70 7974 686f 6e5f 6d69 6e5a 0673 7973  .python_minZ.sys
-00002f00: 5f70 795a 0d73 7973 7465 6d5f 7079 7468  _pyZ.system_pyth
-00002f10: 6f6e 720b 0000 0072 0b00 0000 720c 0000  onr....r....r...
-00002f20: 00da 1469 735f 636f 6d70 6174 6962 6c65  ...is_compatible
-00002f30: 5f70 7974 686f 6ebe 0100 0073 0600 0000  _python....s....
-00002f40: 0002 0601 1e01 7a1d 4275 696c 6445 6e76  ......z.BuildEnv
-00002f50: 2e69 735f 636f 6d70 6174 6962 6c65 5f70  .is_compatible_p
-00002f60: 7974 686f 6e63 0100 0000 0000 0000 0000  ythonc..........
-00002f70: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-00002f80: 0000 007c 006a 0064 016b 0653 0029 024e  ...|.j.d.k.S.).N
-00002f90: 2903 da05 7769 6e33 32da 0663 7967 7769  )...win32..cygwi
-00002fa0: 6e5a 046d 7379 73a9 0172 9900 0000 7221  nZ.msys..r....r!
-00002fb0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00002fc0: 0000 da0a 6973 5f77 696e 646f 7773 c401  ....is_windows..
-00002fd0: 0000 7302 0000 0000 017a 1342 7569 6c64  ..s......z.Build
-00002fe0: 456e 762e 6973 5f77 696e 646f 7773 6301  Env.is_windowsc.
-00002ff0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00003000: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
-00003010: 6401 6b02 5300 2902 4e72 4800 0000 72a1  d.k.S.).NrH...r.
-00003020: 0000 0072 2100 0000 720b 0000 0072 0b00  ...r!...r....r..
-00003030: 0000 720c 0000 00da 0869 735f 6d61 636f  ..r......is_maco
-00003040: 73c7 0100 0073 0200 0000 0001 7a11 4275  s....s......z.Bu
-00003050: 696c 6445 6e76 2e69 735f 6d61 636f 7363  ildEnv.is_macosc
-00003060: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00003070: 0200 0000 4300 0000 7334 0000 0064 0164  ....C...s4...d.d
-00003080: 0284 007d 0164 0364 0484 007d 027c 0183  ...}.d.d...}.|..
-00003090: 007d 037c 0373 207c 0283 007d 037c 0373  .}.|.s |...}.|.s
-000030a0: 2c74 0064 0583 0182 0174 017c 0383 0153  ,t.d.....t.|...S
-000030b0: 0029 067a 5346 696e 6420 7468 6520 7061  .).zSFind the pa
-000030c0: 7468 2074 6f20 7468 6520 636d 616b 6520  th to the cmake 
-000030d0: 6469 7265 6374 6f72 7920 7769 7468 696e  directory within
-000030e0: 2061 0a20 2020 2020 2020 2070 6970 2069   a.        pip i
-000030f0: 6e73 7461 6c6c 6564 2070 7974 6f72 6368  nstalled pytorch
-00003100: 2070 6163 6b61 6765 6300 0000 0000 0000   packagec.......
-00003110: 0000 0000 0004 0000 0008 0000 0053 0000  .............S..
-00003120: 0073 5e00 0000 7a42 6401 6402 6c00 7d00  .s^...zBd.d.l.}.
-00003130: 6403 6404 8400 7c00 6a01 4400 8301 7d01  d.d...|.j.D...}.
-00003140: 7c01 4400 5d1e 7d02 7c02 6405 1b00 7d03  |.D.].}.|.d...}.
-00003150: 7c03 a002 a100 721e 7c03 0200 0100 5700  |.....r.|.....W.
-00003160: 5300 711e 5700 6402 5300 0400 7403 6b0a  S.q.W.d.S...t.k.
-00003170: 7258 0100 0100 0100 5900 6402 5300 5800  rX......Y.d.S.X.
-00003180: 6402 5300 2906 7a1c 4669 6e64 2074 6872  d.S.).z.Find thr
-00003190: 6f75 6768 2069 6d70 6f72 7469 6e67 2074  ough importing t
-000031a0: 6f72 6368 7201 0000 004e 6301 0000 0000  orchr....Nc.....
-000031b0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-000031c0: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-000031d0: 7400 7c01 8301 9102 7104 5300 720b 0000  t.|.....q.S.r...
-000031e0: 0072 0200 0000 a902 7211 0000 00da 0170  .r......r......p
-000031f0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00003200: 6e00 0000 d401 0000 7304 0000 0006 0002  n.......s.......
-00003210: 007a 4942 7569 6c64 456e 762e 746f 7263  .zIBuildEnv.torc
-00003220: 685f 636d 616b 655f 7061 7468 2e3c 6c6f  h_cmake_path.<lo
-00003230: 6361 6c73 3e2e 5f74 6f72 6368 5f69 6d70  cals>._torch_imp
-00003240: 6f72 745f 7061 7468 2e3c 6c6f 6361 6c73  ort_path.<locals
-00003250: 3e2e 3c6c 6973 7463 6f6d 703e 7a11 7368  >.<listcomp>z.sh
-00003260: 6172 652f 636d 616b 652f 546f 7263 6829  are/cmake/Torch)
-00003270: 0472 4000 0000 da08 5f5f 7061 7468 5f5f  .r@.....__path__
-00003280: da06 6973 5f64 6972 da13 4d6f 6475 6c65  ..is_dir..Module
-00003290: 4e6f 7446 6f75 6e64 4572 726f 7229 04da  NotFoundError)..
-000032a0: 0174 5a0b 746f 7263 685f 7061 7468 73da  .tZ.torch_paths.
-000032b0: 055f 7061 7468 da0a 746f 7263 685f 7061  ._path..torch_pa
-000032c0: 7468 720b 0000 0072 0b00 0000 720c 0000  thr....r....r...
-000032d0: 00da 125f 746f 7263 685f 696d 706f 7274  ..._torch_import
-000032e0: 5f70 6174 68cf 0100 0073 1400 0000 0002  _path....s......
-000032f0: 0201 0802 1001 0801 0801 0801 0c01 0601  ................
-00003300: 0e01 7a35 4275 696c 6445 6e76 2e74 6f72  ..z5BuildEnv.tor
-00003310: 6368 5f63 6d61 6b65 5f70 6174 682e 3c6c  ch_cmake_path.<l
-00003320: 6f63 616c 733e 2e5f 746f 7263 685f 696d  ocals>._torch_im
-00003330: 706f 7274 5f70 6174 6863 0000 0000 0000  port_pathc......
-00003340: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-00003350: 0000 7356 0000 0064 0164 0284 0074 00a0  ..sV...d.d...t..
-00003360: 01a1 0044 0083 017d 0074 0274 006a 0383  ...D...}.t.t.j..
-00003370: 01a0 04a1 0072 307c 00a0 0574 0274 006a  .....r0|...t.t.j
-00003380: 0383 01a1 0101 007c 0044 005d 1c7d 017c  .......|.D.].}.|
-00003390: 0164 031b 007d 027c 02a0 04a1 0072 347c  .d...}.|.....r4|
-000033a0: 0202 0001 0053 0071 3464 0453 0029 057a  .....S.q4d.S.).z
-000033b0: 2066 696e 6420 746f 7263 6820 7468 726f   find torch thro
-000033c0: 7567 6820 7369 7465 2070 6163 6b61 6765  ugh site package
-000033d0: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
-000033e0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-000033f0: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
-00003400: 0453 0072 0b00 0000 7202 0000 0072 a400  .S.r....r....r..
-00003410: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00003420: 0072 6e00 0000 df01 0000 7304 0000 0006  .rn.......s.....
-00003430: 0002 007a 4742 7569 6c64 456e 762e 746f  ...zGBuildEnv.to
-00003440: 7263 685f 636d 616b 655f 7061 7468 2e3c  rch_cmake_path.<
-00003450: 6c6f 6361 6c73 3e2e 5f74 6f72 6368 5f73  locals>._torch_s
-00003460: 6974 655f 7061 7468 2e3c 6c6f 6361 6c73  ite_path.<locals
-00003470: 3e2e 3c6c 6973 7463 6f6d 703e 7a17 746f  >.<listcomp>z.to
-00003480: 7263 682f 7368 6172 652f 636d 616b 652f  rch/share/cmake/
-00003490: 546f 7263 684e 2906 da04 7369 7465 da0f  TorchN)...site..
-000034a0: 6765 7473 6974 6570 6163 6b61 6765 7372  getsitepackagesr
-000034b0: 0300 0000 da09 5553 4552 5f53 4954 4572  ......USER_SITEr
-000034c0: a700 0000 7269 0000 0029 035a 0a73 6974  ....ri...).Z.sit
-000034d0: 655f 7061 7468 7372 aa00 0000 72ab 0000  e_pathsr....r...
-000034e0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-000034f0: da10 5f74 6f72 6368 5f73 6974 655f 7061  .._torch_site_pa
-00003500: 7468 dd01 0000 7310 0000 0000 0212 030e  th....s.........
-00003510: 0110 0208 0108 0108 010a 017a 3342 7569  ...........z3Bui
-00003520: 6c64 456e 762e 746f 7263 685f 636d 616b  ldEnv.torch_cmak
-00003530: 655f 7061 7468 2e3c 6c6f 6361 6c73 3e2e  e_path.<locals>.
-00003540: 5f74 6f72 6368 5f73 6974 655f 7061 7468  _torch_site_path
-00003550: 7a21 436f 756c 6420 6e6f 7420 6c6f 6361  z!Could not loca
-00003560: 7465 2074 6f72 6368 2063 6d61 6b65 2070  te torch cmake p
-00003570: 6174 6829 0272 0600 0000 7210 0000 0029  ath).r....r....)
-00003580: 0472 1800 0000 72ac 0000 0072 b000 0000  .r....r....r....
-00003590: 72ab 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000035a0: 0c00 0000 da10 746f 7263 685f 636d 616b  ......torch_cmak
-000035b0: 655f 7061 7468 ca01 0000 7310 0000 0000  e_path....s.....
-000035c0: 0508 0e08 0e06 0104 0106 0104 0108 017a  ...............z
-000035d0: 1942 7569 6c64 456e 762e 746f 7263 685f  .BuildEnv.torch_
-000035e0: 636d 616b 655f 7061 7468 6300 0000 0000  cmake_pathc.....
-000035f0: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
-00003600: 0000 0073 bc00 0000 7400 6a01 a002 6401  ...s....t.j...d.
-00003610: 6402 a102 7400 6a01 a002 6403 6402 a102  d...t.j...d.d...
-00003620: 7400 6a01 a002 6404 6402 a102 7400 6a01  t.j...d.d...t.j.
-00003630: a002 6405 6402 a102 6406 9c04 7d00 6401  ..d.d...d...}.d.
-00003640: 6403 6702 7d01 6405 6404 6702 7d02 7403  d.g.}.d.d.g.}.t.
-00003650: 6407 6408 8400 7c01 4400 8301 8301 7d03  d.d...|.D.....}.
-00003660: 7403 6409 6408 8400 7c02 4400 8301 8301  t.d.d...|.D.....
-00003670: 7d04 7c03 7376 7c04 7376 6402 5300 7c03  }.|.sv|.svd.S.|.
-00003680: 7298 7c04 7398 7c00 6403 1900 7c00 6405  r.|.s.|.d...|.d.
-00003690: 3c00 7c00 6401 1900 7c00 6404 3c00 6e20  <.|.d...|.d.<.n 
-000036a0: 7c04 72b8 7c03 73b8 7c00 6405 1900 7c00  |.r.|.s.|.d...|.
-000036b0: 6403 3c00 7c00 6404 1900 7c00 6401 3c00  d.<.|.d...|.d.<.
-000036c0: 7c00 5300 290a 612f 0100 0043 6f6c 6c65  |.S.).a/...Colle
-000036d0: 6374 2074 6865 2065 6e76 6972 6f6e 6d65  ct the environme
-000036e0: 6e74 2076 6172 6961 626c 6573 206e 6565  nt variables nee
-000036f0: 6465 6420 666f 7220 4361 6666 6520 2850  ded for Caffe (P
-00003700: 7974 6f72 6368 290a 2020 2020 2020 2020  ytorch).        
-00003710: 616e 6420 7468 726f 7720 616e 2065 7272  and throw an err
-00003720: 6f72 2069 6620 7468 6579 2061 7265 206e  or if they are n
-00003730: 6f74 2066 6f75 6e64 0a0a 2020 2020 2020  ot found..      
-00003740: 2020 5370 6563 6966 6963 616c 6c79 206d    Specifically m
-00003750: 616b 6520 7375 7265 2074 6f20 7365 7420  ake sure to set 
-00003760: 6174 206c 6561 7374 206f 6e65 2073 6574  at least one set
-00003770: 206f 663a 0a20 2020 2020 2020 2020 2020   of:.           
-00003780: 202d 2043 5544 4e4e 5f4c 4942 5241 5259   - CUDNN_LIBRARY
-00003790: 2061 6e64 2043 5544 4e4e 5f49 4e43 4c55   and CUDNN_INCLU
-000037a0: 4445 5f44 4952 0a20 2020 2020 2020 2020  DE_DIR.         
-000037b0: 2020 2020 2020 206f 720a 2020 2020 2020         or.      
-000037c0: 2020 2020 2020 2d20 4355 444e 4e5f 4c49        - CUDNN_LI
-000037d0: 4252 4152 595f 5041 5448 2061 6e64 2043  BRARY_PATH and C
-000037e0: 5544 4e4e 5f49 4e43 4c55 4445 5f50 4154  UDNN_INCLUDE_PAT
-000037f0: 480a 2020 2020 2020 2020 da0d 4355 444e  H.        ..CUDN
-00003800: 4e5f 4c49 4252 4152 594e da11 4355 444e  N_LIBRARYN..CUDN
-00003810: 4e5f 494e 434c 5544 455f 4449 52da 1243  N_INCLUDE_DIR..C
-00003820: 5544 4e4e 5f4c 4942 5241 5259 5f50 4154  UDNN_LIBRARY_PAT
-00003830: 48da 1243 5544 4e4e 5f49 4e43 4c55 4445  H..CUDNN_INCLUDE
-00003840: 5f50 4154 4829 0472 b200 0000 72b3 0000  _PATH).r....r...
-00003850: 0072 b400 0000 72b5 0000 0063 0100 0000  .r....r....c....
-00003860: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00003870: 5300 0000 7316 0000 0067 007c 005d 0e7d  S...s....g.|.].}
-00003880: 017c 0174 006a 016b 0691 0271 0453 0072  .|.t.j.k...q.S.r
-00003890: 0b00 0000 a902 7234 0000 0072 3500 0000  ......r4...r5...
-000038a0: a902 7211 0000 0072 3700 0000 720b 0000  ..r....r7...r...
-000038b0: 0072 0b00 0000 720c 0000 0072 6e00 0000  .r....r....rn...
-000038c0: 0502 0000 7304 0000 0006 0002 007a 2a42  ....s........z*B
-000038d0: 7569 6c64 456e 762e 6765 745f 6375 646e  uildEnv.get_cudn
-000038e0: 6e5f 656e 762e 3c6c 6f63 616c 733e 2e3c  n_env.<locals>.<
-000038f0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
-00003900: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00003910: 0000 7316 0000 0067 007c 005d 0e7d 017c  ..s....g.|.].}.|
-00003920: 0174 006a 016b 0691 0271 0453 0072 0b00  .t.j.k...q.S.r..
-00003930: 0000 72b6 0000 0072 b700 0000 720b 0000  ..r....r....r...
-00003940: 0072 0b00 0000 720c 0000 0072 6e00 0000  .r....r....rn...
-00003950: 0602 0000 7304 0000 0006 0002 0029 0472  ....s........).r
-00003960: 3400 0000 7235 0000 0072 3600 0000 da03  4...r5...r6.....
-00003970: 616c 6c29 0572 9600 0000 5a10 746f 7263  all).r....Z.torc
-00003980: 685f 6375 646e 6e5f 7661 7273 5a10 6361  h_cudnn_varsZ.ca
-00003990: 6666 655f 6375 646e 6e5f 7661 7273 5a09  ffe_cudnn_varsZ.
-000039a0: 746f 7263 685f 7365 745a 0963 6166 6665  torch_setZ.caffe
-000039b0: 5f73 6574 720b 0000 0072 0b00 0000 720c  _setr....r....r.
-000039c0: 0000 00da 0d67 6574 5f63 7564 6e6e 5f65  .....get_cudnn_e
-000039d0: 6e76 f201 0000 7324 0000 0000 0b0c 010c  nv....s$........
-000039e0: 010c 010c fc06 0608 0108 0212 0112 0408  ................
-000039f0: 0104 0108 010c 010e 0108 010c 010c 017a  ...............z
-00003a00: 1642 7569 6c64 456e 762e 6765 745f 6375  .BuildEnv.get_cu
-00003a10: 646e 6e5f 656e 7663 0200 0000 0000 0000  dnn_envc........
-00003a20: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
-00003a30: 7346 0000 007a 1c74 006a 017c 0164 0167  sF...z.t.j.|.d.g
-00003a40: 0274 006a 0274 006a 0264 028d 0301 0057  .t.j.t.j.d.....W
-00003a50: 006e 2404 0074 036b 0a72 4001 0001 0001  .n$..t.k.r@.....
-00003a60: 0074 047c 019b 0064 039d 0283 0164 0082  .t.|...d.....d..
-00003a70: 0259 006e 0258 0064 0053 0029 044e 7a09  .Y.n.X.d.S.).Nz.
-00003a80: 2d2d 7665 7273 696f 6e29 02da 0673 7464  --version)...std
-00003a90: 6f75 74da 0673 7464 6572 727a 2420 6d75  out..stderrz$ mu
-00003aa0: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
-00003ab0: 746f 2062 7569 6c64 2053 6d61 7274 5369  to build SmartSi
-00003ac0: 6d29 0572 7700 0000 da0a 6368 6563 6b5f  m).rw.....check_
-00003ad0: 6361 6c6c da07 4445 564e 554c 4cda 074f  call..DEVNULL..O
-00003ae0: 5345 7272 6f72 7206 0000 0029 0272 1800  SErrorr....).r..
-00003af0: 0000 da07 636f 6d6d 616e 6472 0b00 0000  ....commandr....
-00003b00: 720b 0000 0072 0c00 0000 7292 0000 0014  r....r....r.....
-00003b10: 0200 0073 1000 0000 0002 0201 0401 0601  ...s............
-00003b20: 0401 04fd 0a05 0e01 7a1f 4275 696c 6445  ........z.BuildE
-00003b30: 6e76 2e63 6865 636b 5f62 7569 6c64 5f64  nv.check_build_d
-00003b40: 6570 656e 6465 6e63 794e 6302 0000 0000  ependencyNc.....
-00003b50: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
-00003b60: 0000 0073 8000 0000 7a62 7400 7401 a002  ...s....zbt.t...
-00003b70: 7c00 a101 6a03 8301 7d02 7c01 725e 7c02  |...j...}.|.r^|.
-00003b80: 6a04 7c01 6a04 6b03 732e 7c02 6a05 7c01  j.|.j.k.s.|.j.|.
-00003b90: 6a05 6b03 725e 6401 7c00 9b00 6402 9d03  j.k.r^d.|...d...
-00003ba0: 7c00 9b00 6403 7c01 9b00 6404 7c00 9b00  |...d.|...d.|...
-00003bb0: 6403 7c02 9b00 6405 9d08 1700 7d03 7406  d.|...d.....}.t.
-00003bc0: 7c03 8301 8201 5700 6406 5300 0400 7401  |.....W.d.S...t.
-00003bd0: 6a07 6b0a 727a 0100 0100 0100 5900 6407  j.k.rz......Y.d.
-00003be0: 5300 5800 6408 5300 2909 7a7f 4368 6563  S.X.d.S.).z.Chec
-00003bf0: 6b20 6966 2061 2070 6163 6b61 6765 2069  k if a package i
-00003c00: 7320 696e 7374 616c 6c65 642e 2049 6620  s installed. If 
-00003c10: 7665 7273 696f 6e20 6973 2070 726f 7669  version is provi
-00003c20: 6465 642c 2063 6865 636b 2069 660a 2020  ded, check if.  
-00003c30: 2020 2020 2020 6974 2773 2061 2063 6f6d        it's a com
-00003c40: 7061 7469 626c 6520 7665 7273 696f 6e2e  patible version.
-00003c50: 2028 6d61 6a6f 7220 616e 6420 6d69 6e6f   (major and mino
-00003c60: 7220 7468 6520 7361 6d65 297a 1949 6e63  r the same)z.Inc
-00003c70: 6f6d 7061 7469 626c 6520 7665 7273 696f  ompatible versio
-00003c80: 6e20 666f 7220 7a0b 2064 6574 6563 7465  n for z. detecte
-00003c90: 642e 0afa 0120 7a0f 2072 6571 7565 7374  d.... z. request
-00003ca0: 6564 2062 7574 207a 0b20 696e 7374 616c  ed but z. instal
-00003cb0: 6c65 642e 5446 4e29 0872 0d00 0000 721d  led.TFN).r....r.
-00003cc0: 0000 00da 1067 6574 5f64 6973 7472 6962  .....get_distrib
-00003cd0: 7574 696f 6e72 4d00 0000 7222 0000 0072  utionrM...r"...r
-00003ce0: 2400 0000 7206 0000 00da 1444 6973 7472  $...r......Distr
-00003cf0: 6962 7574 696f 6e4e 6f74 466f 756e 6429  ibutionNotFound)
-00003d00: 04da 0770 6163 6b61 6765 724d 0000 005a  ...packagerM...Z
-00003d10: 0969 6e73 7461 6c6c 6564 da03 6d73 6772  .installed..msgr
-00003d20: 0b00 0000 720b 0000 0072 0c00 0000 da0f  ....r....r......
-00003d30: 6368 6563 6b5f 696e 7374 616c 6c65 641f  check_installed.
-00003d40: 0200 0073 1800 0000 0004 0201 1001 0402  ...s............
-00003d50: 1802 0a01 1aff 02ff 0204 0801 0601 1001  ................
-00003d60: 7a18 4275 696c 6445 6e76 2e63 6865 636b  z.BuildEnv.check
-00003d70: 5f69 6e73 7461 6c6c 6564 2901 5429 014e  _installed).T).N
-00003d80: 2920 7207 0000 0072 0800 0000 7209 0000  ) r....r....r...
-00003d90: 0072 0a00 0000 7234 0000 0072 3500 0000  .r....r4...r5...
-00003da0: 7236 0000 0072 8800 0000 7289 0000 0072  r6...r....r....r
-00003db0: 8a00 0000 728b 0000 0072 8c00 0000 7298  ....r....r....r.
-00003dc0: 0000 0072 1c00 0000 7291 0000 0072 5800  ...r....r....rX.
-00003dd0: 0000 725b 0000 0072 9900 0000 724f 0000  ..r[...r....rO..
-00003de0: 0072 8e00 0000 7297 0000 0072 6c00 0000  .r....r....rl...
-00003df0: 7232 0000 0072 9b00 0000 729e 0000 0072  r2...r....r....r
-00003e00: a200 0000 72a3 0000 0072 b100 0000 da0c  ....r....r......
-00003e10: 7374 6174 6963 6d65 7468 6f64 72b9 0000  staticmethodr...
-00003e20: 0072 9200 0000 72c5 0000 0072 0b00 0000  .r....r....r....
-00003e30: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00003e40: 8700 0000 6b01 0000 7332 0000 0008 0104  ....k...s2......
-00003e50: 120e 010e 010e 010e 030e 010e 0312 0106  ................
-00003e60: 020a 0408 0608 0d08 1802 010a 0308 0608  ................
-00003e70: 0308 0302 010a 2702 010a 2108 0b02 0172  ......'...!....r
-00003e80: 8700 0000 2916 7234 0000 0072 5b00 0000  ....).r4...r[...
-00003e90: 72ad 0000 0072 7700 0000 7258 0000 00da  r....rw...rX....
-00003ea0: 0770 6174 686c 6962 7203 0000 00da 0674  .pathlibr......t
-00003eb0: 7970 696e 6772 0400 0000 721d 0000 0072  ypingr....r....r
-00003ec0: 0500 0000 724d 0000 0072 1500 0000 7217  ....rM...r....r.
-00003ed0: 0000 0072 7b00 0000 7206 0000 0072 1000  ...r{...r....r..
-00003ee0: 0000 720d 0000 0072 3900 0000 723a 0000  ..r....r9...r:..
-00003ef0: 0072 5c00 0000 7287 0000 0072 0b00 0000  .r\...r....r....
-00003f00: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00003f10: 083c 6d6f 6475 6c65 3e1b 0000 0073 2200  .<module>....s".
-00003f20: 0000 0801 0801 0801 0801 0801 0c01 0c02  ................
-00003f30: 0801 0c02 0801 0808 1012 1041 0804 1056  ...........A...V
-00003f40: 0e7f 0010                                ....
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a06 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6402 6c07 6d08 5a08 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
+00000070: 6d09 5a09 0100 6400 6401 6c0a 5a0a 6400  m.Z...d.d.l.Z.d.
+00000080: 6404 6c0a 6d0b 5a0b 0100 650b 6a0c 6a0d  d.l.m.Z...e.j.j.
+00000090: 5a0d 650b 6a0c 6a0e 5a0e 6506 6a0f 6405  Z.e.j.j.Z.e.j.d.
+000000a0: 1900 5a10 4700 6406 6407 8400 6407 6511  ..Z.G.d.d...d.e.
+000000b0: 8303 5a12 4700 6408 6409 8400 6409 6513  ..Z.G.d.d...d.e.
+000000c0: 8303 5a14 6513 6513 6513 640a 9c03 640b  ..Z.e.e.e.d...d.
+000000d0: 640c 8404 5a15 4700 640d 640e 8400 640e  d...Z.G.d.d...d.
+000000e0: 6514 8303 5a16 4700 640f 6410 8400 6410  e...Z.G.d.d...d.
+000000f0: 8302 5a17 4700 6411 6412 8400 6412 8302  ..Z.G.d.d...d...
+00000100: 5a18 6401 5300 2913 e900 0000 004e a901  Z.d.S.)......N..
+00000110: da04 5061 7468 2901 da08 4974 6572 6162  ..Path)...Iterab
+00000120: 6c65 2901 da09 7061 636b 6167 696e 6729  le)...packaging)
+00000130: 02da 0552 4544 4953 5a05 4b45 5944 4263  ...REDISZ.KEYDBc
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+00000160: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+00000170: 0a53 6574 7570 4572 726f 7261 0f02 0000  .SetupErrora....
+00000180: 4120 7369 6d70 6c65 2065 7863 6570 7469  A simple excepti
+00000190: 6f6e 2063 6c61 7373 2066 6f72 2065 7272  on class for err
+000001a0: 6f72 7320 696e 205f 696e 7374 616c 6c2e  ors in _install.
+000001b0: 6275 696c 6465 6e76 2066 696c 652e 0a20  buildenv file.. 
+000001c0: 2020 2054 6869 7320 6973 2070 7269 6d61     This is prima
+000001d0: 7269 6c79 2075 7365 6420 746f 2069 6e74  rily used to int
+000001e0: 6572 7275 7074 2074 6865 2073 6574 7570  errupt the setup
+000001f0: 2e70 7920 6275 696c 6420 696e 2063 6173  .py build in cas
+00000200: 650a 2020 2020 6f66 2061 2066 6169 6c75  e.    of a failu
+00000210: 7265 2c20 616e 6420 6973 2063 6175 6768  re, and is caugh
+00000220: 7420 6672 6571 7565 6e74 6c79 2069 6e20  t frequently in 
+00000230: 7468 6520 434c 4920 7768 6963 6820 6174  the CLI which at
+00000240: 7465 6d70 7473 0a20 2020 2074 6f20 7375  tempts.    to su
+00000250: 7070 7265 7373 2061 6e64 206c 6f67 2074  ppress and log t
+00000260: 6865 2065 7272 6f72 7320 7468 726f 776e  he errors thrown
+00000270: 2068 6572 652e 0a0a 2020 2020 4f6e 6520   here...    One 
+00000280: 6e6f 7465 2069 7320 7468 6174 2074 6869  note is that thi
+00000290: 7320 6572 726f 7220 6d75 7374 2062 6520  s error must be 
+000002a0: 696d 706f 7274 6564 2066 726f 6d20 6865  imported from he
+000002b0: 7265 2074 6f20 6265 0a20 2020 2063 6175  re to be.    cau
+000002c0: 6768 7420 616e 6420 6e6f 7420 6465 6669  ght and not defi
+000002d0: 6e65 6420 616e 7977 6865 7265 2065 6c73  ned anywhere els
+000002e0: 652e 2053 696e 6365 2077 6520 7573 6520  e. Since we use 
+000002f0: 7468 6973 2063 6c61 7373 0a20 2020 2069  this class.    i
+00000300: 6e20 7468 6520 696e 7374 616c 6c61 7469  n the installati
+00000310: 6f6e 2c20 6861 7669 6e67 2061 2073 6570  on, having a sep
+00000320: 6172 6174 6520 6572 726f 7220 6669 6c65  arate error file
+00000330: 2077 6f75 6c64 206d 6561 6e0a 2020 2020   would mean.    
+00000340: 616e 6f74 6865 7220 6d6f 6475 6c65 2074  another module t
+00000350: 6f20 6d61 6e75 616c 6c79 2069 6d70 6f72  o manually impor
+00000360: 7420 696e 746f 2073 6574 7570 2e70 790a  t into setup.py.
+00000370: 0a20 2020 2053 6565 2073 6574 7570 2e70  .    See setup.p
+00000380: 7920 666f 7220 6d6f 7265 0a20 2020 204e  y for more.    N
+00000390: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000003a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000003b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fa9  name__..__doc__.
+000003c0: 0072 0c00 0000 720c 0000 00fa 472f 686f  .r....r.....G/ho
+000003d0: 6d65 2f72 756e 6e65 722f 776f 726b 2f53  me/runner/work/S
+000003e0: 6d61 7274 5369 6d2f 536d 6172 7453 696d  martSim/SmartSim
+000003f0: 2f73 6d61 7274 7369 6d2f 5f63 6f72 652f  /smartsim/_core/
+00000400: 5f69 6e73 7461 6c6c 2f62 7569 6c64 656e  _install/builden
+00000410: 762e 7079 7207 0000 002f 0000 0073 0400  v.pyr..../...s..
+00000420: 0000 0801 040d 7207 0000 0063 0000 0000  ......r....c....
+00000430: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000440: 0000 0000 73f4 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000450: 0264 015a 0365 046a 0565 0665 0765 086a  .d.Z.e.j.e.e.e.j
+00000460: 096a 0a19 0065 086a 096a 0a66 0319 0065  .j...e.j.j.f...e
+00000470: 046a 0b64 029c 0264 0364 0484 045a 0c65  .j.d...d.d...Z.e
+00000480: 0d65 0e64 059c 0164 0664 0784 0483 015a  .e.d...d.d.....Z
+00000490: 0f65 0d65 0e64 059c 0164 0864 0984 0483  .e.e.d...d.d....
+000004a0: 015a 1065 0d65 0e64 059c 0164 0a64 0b84  .Z.e.e.d...d.d..
+000004b0: 0483 015a 1165 0d65 0664 059c 0164 0c64  ...Z.e.e.d...d.d
+000004c0: 0d84 0483 015a 1265 046a 0b65 1364 0e9c  .....Z.e.j.e.d..
+000004d0: 0287 0066 0164 0f64 1084 0c5a 1465 046a  ...f.d.d...Z.e.j
+000004e0: 0b65 1364 0e9c 0287 0066 0164 1164 1284  .e.d.....f.d.d..
+000004f0: 0c5a 1565 046a 0b65 1364 0e9c 0287 0066  .Z.e.j.e.d.....f
+00000500: 0164 1364 1484 0c5a 1665 046a 0b65 1364  .d.d...Z.e.j.e.d
+00000510: 0e9c 0287 0066 0164 1564 1684 0c5a 1765  .....f.d.d...Z.e
+00000520: 046a 0b65 1364 0e9c 0287 0066 0164 1764  .j.e.d.....f.d.d
+00000530: 1884 0c5a 1887 0004 005a 1953 0029 19da  ...Z.....Z.S.)..
+00000540: 0856 6572 7369 6f6e 5f7a 7841 2073 7562  .Version_zxA sub
+00000550: 636c 6173 7320 6f66 2070 6b67 5f72 6573  class of pkg_res
+00000560: 6f75 7263 6573 2e70 6163 6b61 6769 6e67  ources.packaging
+00000570: 2e76 6572 7369 6f6e 2e56 6572 7369 6f6e  .version.Version
+00000580: 2074 6861 740a 2020 2020 696e 636c 7564   that.    includ
+00000590: 6573 2073 6f6d 6520 6865 6c70 6572 206d  es some helper m
+000005a0: 6574 686f 6473 2066 6f72 2063 6f6d 7061  ethods for compa
+000005b0: 7269 6e67 2076 6572 7369 6f6e 732e 0a20  ring versions.. 
+000005c0: 2020 20a9 02da 0476 6572 73da 0672 6574     ....vers..ret
+000005d0: 7572 6e63 0200 0000 0000 0000 0000 0000  urnc............
+000005e0: 0200 0000 0500 0000 4300 0000 734e 0000  ........C...sN..
+000005f0: 0074 007c 0174 0183 0272 0e7c 0153 0074  .t.|.t...r.|.S.t
+00000600: 007c 0174 0283 0272 2074 017c 0183 0153  .|.t...r t.|...S
+00000610: 0074 007c 0174 0383 0272 4274 0164 01a0  .t.|.t...rBt.d..
+00000620: 0464 0264 0384 007c 0144 0083 01a1 0183  .d.d...|.D......
+00000630: 0153 0074 057c 0183 0182 0164 0053 0029  .S.t.|.....d.S.)
+00000640: 044e da01 2e63 0100 0000 0000 0000 0000  .N...c..........
+00000650: 0000 0200 0000 0300 0000 7300 0000 7316  ..........s...s.
+00000660: 0000 007c 005d 0e7d 0174 007c 0183 0156  ...|.].}.t.|...V
+00000670: 0001 0071 0264 0053 00a9 014e 2901 da03  ...q.d.S...N)...
+00000680: 7374 7229 02da 022e 30da 0469 7465 6d72  str)....0..itemr
+00000690: 0c00 0000 720c 0000 0072 0d00 0000 da09  ....r....r......
+000006a0: 3c67 656e 6578 7072 3e4c 0000 0073 0400  <genexpr>L...s..
+000006b0: 0000 0400 0200 7a2f 5665 7273 696f 6e5f  ......z/Version_
+000006c0: 2e5f 636f 6e76 6572 745f 746f 5f76 6572  ._convert_to_ver
+000006d0: 7369 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c67  sion.<locals>.<g
+000006e0: 656e 6578 7072 3e29 06da 0a69 7369 6e73  enexpr>)...isins
+000006f0: 7461 6e63 65da 0756 6572 7369 6f6e 7214  tance..Versionr.
+00000700: 0000 0072 0400 0000 da04 6a6f 696e da0e  ...r......join..
+00000710: 496e 7661 6c69 6456 6572 7369 6f6e 2902  InvalidVersion).
+00000720: da04 7365 6c66 7210 0000 0072 0c00 0000  ..selfr....r....
+00000730: 720c 0000 0072 0d00 0000 da13 5f63 6f6e  r....r......_con
+00000740: 7665 7274 5f74 6f5f 7665 7273 696f 6e46  vert_to_versionF
+00000750: 0000 0073 0e00 0000 0001 0a01 0401 0a01  ...s............
+00000760: 0801 0a01 1802 7a1c 5665 7273 696f 6e5f  ......z.Version_
+00000770: 2e5f 636f 6e76 6572 745f 746f 5f76 6572  ._convert_to_ver
+00000780: 7369 6f6e a901 7211 0000 0063 0100 0000  sion..r....c....
+00000790: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000007a0: 4300 0000 731a 0000 0074 0074 01a0 027c  C...s....t.t...|
+000007b0: 00a1 016a 03a0 0464 01a1 0164 0219 0083  ...j...d...d....
+000007c0: 0153 0029 034e 7212 0000 0072 0100 0000  .S.).Nr....r....
+000007d0: a905 da03 696e 74da 0d70 6b67 5f72 6573  ....int..pkg_res
+000007e0: 6f75 7263 6573 da0d 7061 7273 655f 7665  ources..parse_ve
+000007f0: 7273 696f 6eda 0c62 6173 655f 7665 7273  rsion..base_vers
+00000800: 696f 6eda 0573 706c 6974 a901 721c 0000  ion..split..r...
+00000810: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000820: da05 6d61 6a6f 7250 0000 0073 0200 0000  ..majorP...s....
+00000830: 0004 7a0e 5665 7273 696f 6e5f 2e6d 616a  ..z.Version_.maj
+00000840: 6f72 6301 0000 0000 0000 0000 0000 0001  orc.............
+00000850: 0000 0004 0000 0043 0000 0073 1a00 0000  .......C...s....
+00000860: 7400 7401 a002 7c00 a101 6a03 a004 6401  t.t...|...j...d.
+00000870: a101 6402 1900 8301 5300 2903 4e72 1200  ..d.....S.).Nr..
+00000880: 0000 e901 0000 0072 1f00 0000 7225 0000  .......r....r%..
+00000890: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000008a0: da05 6d69 6e6f 7256 0000 0073 0200 0000  ..minorV...s....
+000008b0: 0002 7a0e 5665 7273 696f 6e5f 2e6d 696e  ..z.Version_.min
+000008c0: 6f72 6301 0000 0000 0000 0000 0000 0001  orc.............
+000008d0: 0000 0004 0000 0043 0000 0073 1a00 0000  .......C...s....
+000008e0: 7400 7401 a002 7c00 a101 6a03 a004 6401  t.t...|...j...d.
+000008f0: a101 6402 1900 8301 5300 a903 4e72 1200  ..d.....S...Nr..
+00000900: 0000 e902 0000 0072 1f00 0000 7225 0000  .......r....r%..
+00000910: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000920: da05 6d69 6372 6f5a 0000 0073 0200 0000  ..microZ...s....
+00000930: 0002 7a0e 5665 7273 696f 6e5f 2e6d 6963  ..z.Version_.mic
+00000940: 726f 6301 0000 0000 0000 0000 0000 0001  roc.............
+00000950: 0000 0004 0000 0043 0000 0073 1800 0000  .......C...s....
+00000960: 7400 7401 a002 7c00 a101 8301 a003 6401  t.t...|.......d.
+00000970: a101 6402 1900 5300 7229 0000 0029 0472  ..d...S.r)...).r
+00000980: 1400 0000 7221 0000 0072 2200 0000 7224  ....r!...r"...r$
+00000990: 0000 0072 2500 0000 720c 0000 0072 0c00  ...r%...r....r..
+000009a0: 0000 720d 0000 00da 0570 6174 6368 5e00  ..r......patch^.
+000009b0: 0000 7302 0000 0000 037a 0e56 6572 7369  ..s......z.Versi
+000009c0: 6f6e 5f2e 7061 7463 6829 02da 0363 6d70  on_.patch)...cmp
+000009d0: 7211 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000009e0: 0000 0200 0000 0800 0000 0300 0000 733c  ..............s<
+000009f0: 0000 007a 1674 007c 0083 01a0 017c 00a0  ...z.t.|.....|..
+00000a00: 027c 01a1 01a1 0157 0053 0004 0074 036b  .|.....W.S...t.k
+00000a10: 0a72 3601 0001 0001 0074 0483 00a0 017c  .r6......t.....|
+00000a20: 01a1 0106 0059 0053 0058 0064 0053 0072  .....Y.S.X.d.S.r
+00000a30: 1300 0000 2905 7219 0000 00da 065f 5f67  ....).r......__g
+00000a40: 745f 5f72 1d00 0000 721b 0000 00da 0573  t__r....r......s
+00000a50: 7570 6572 a902 721c 0000 0072 2d00 0000  uper..r....r-...
+00000a60: a901 da09 5f5f 636c 6173 735f 5f72 0c00  ....__class__r..
+00000a70: 0000 720d 0000 0072 2e00 0000 6300 0000  ..r....r....c...
+00000a80: 7308 0000 0000 0102 0116 010e 017a 0f56  s............z.V
+00000a90: 6572 7369 6f6e 5f2e 5f5f 6774 5f5f 6302  ersion_.__gt__c.
+00000aa0: 0000 0000 0000 0000 0000 0002 0000 0008  ................
+00000ab0: 0000 0003 0000 0073 3c00 0000 7a16 7400  .......s<...z.t.
+00000ac0: 7c00 8301 a001 7c00 a002 7c01 a101 a101  |.....|...|.....
+00000ad0: 5700 5300 0400 7403 6b0a 7236 0100 0100  W.S...t.k.r6....
+00000ae0: 0100 7404 8300 a001 7c01 a101 0600 5900  ..t.....|.....Y.
+00000af0: 5300 5800 6400 5300 7213 0000 0029 0572  S.X.d.S.r....).r
+00000b00: 1900 0000 da06 5f5f 6c74 5f5f 721d 0000  ......__lt__r...
+00000b10: 0072 1b00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+00000b20: 7231 0000 0072 0c00 0000 720d 0000 0072  r1...r....r....r
+00000b30: 3300 0000 6900 0000 7308 0000 0000 0102  3...i...s.......
+00000b40: 0116 010e 017a 0f56 6572 7369 6f6e 5f2e  .....z.Version_.
+00000b50: 5f5f 6c74 5f5f 6302 0000 0000 0000 0000  __lt__c.........
+00000b60: 0000 0002 0000 0008 0000 0003 0000 0073  ...............s
+00000b70: 3c00 0000 7a16 7400 7c00 8301 a001 7c00  <...z.t.|.....|.
+00000b80: a002 7c01 a101 a101 5700 5300 0400 7403  ..|.....W.S...t.
+00000b90: 6b0a 7236 0100 0100 0100 7404 8300 a001  k.r6......t.....
+00000ba0: 7c01 a101 0600 5900 5300 5800 6400 5300  |.....Y.S.X.d.S.
+00000bb0: 7213 0000 0029 0572 1900 0000 da06 5f5f  r....).r......__
+00000bc0: 6571 5f5f 721d 0000 0072 1b00 0000 722f  eq__r....r....r/
+00000bd0: 0000 0072 3000 0000 7231 0000 0072 0c00  ...r0...r1...r..
+00000be0: 0000 720d 0000 0072 3400 0000 6f00 0000  ..r....r4...o...
+00000bf0: 7308 0000 0000 0102 0116 010e 017a 0f56  s............z.V
+00000c00: 6572 7369 6f6e 5f2e 5f5f 6571 5f5f 6302  ersion_.__eq__c.
+00000c10: 0000 0000 0000 0000 0000 0002 0000 0008  ................
+00000c20: 0000 0003 0000 0073 3c00 0000 7a16 7400  .......s<...z.t.
+00000c30: 7c00 8301 a001 7c00 a002 7c01 a101 a101  |.....|...|.....
+00000c40: 5700 5300 0400 7403 6b0a 7236 0100 0100  W.S...t.k.r6....
+00000c50: 0100 7404 8300 a001 7c01 a101 0600 5900  ..t.....|.....Y.
+00000c60: 5300 5800 6400 5300 7213 0000 0029 0572  S.X.d.S.r....).r
+00000c70: 1900 0000 da06 5f5f 6765 5f5f 721d 0000  ......__ge__r...
+00000c80: 0072 1b00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+00000c90: 7231 0000 0072 0c00 0000 720d 0000 0072  r1...r....r....r
+00000ca0: 3500 0000 7500 0000 7308 0000 0000 0102  5...u...s.......
+00000cb0: 0116 010e 017a 0f56 6572 7369 6f6e 5f2e  .....z.Version_.
+00000cc0: 5f5f 6765 5f5f 6302 0000 0000 0000 0000  __ge__c.........
+00000cd0: 0000 0002 0000 0008 0000 0003 0000 0073  ...............s
+00000ce0: 3c00 0000 7a16 7400 7c00 8301 a001 7c00  <...z.t.|.....|.
+00000cf0: a002 7c01 a101 a101 5700 5300 0400 7403  ..|.....W.S...t.
+00000d00: 6b0a 7236 0100 0100 0100 7404 8300 a001  k.r6......t.....
+00000d10: 7c01 a101 0600 5900 5300 5800 6400 5300  |.....Y.S.X.d.S.
+00000d20: 7213 0000 0029 0572 1900 0000 da06 5f5f  r....).r......__
+00000d30: 6c65 5f5f 721d 0000 0072 1b00 0000 722f  le__r....r....r/
+00000d40: 0000 0072 3000 0000 7231 0000 0072 0c00  ...r0...r1...r..
+00000d50: 0000 720d 0000 0072 3600 0000 7b00 0000  ..r....r6...{...
+00000d60: 7308 0000 0000 0102 0116 010e 017a 0f56  s............z.V
+00000d70: 6572 7369 6f6e 5f2e 5f5f 6c65 5f5f 291a  ersion_.__le__).
+00000d80: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000d90: 0b00 0000 da01 74da 0555 6e69 6f6e 7214  ......t..Unionr.
+00000da0: 0000 0072 0400 0000 7205 0000 00da 0776  ...r....r......v
+00000db0: 6572 7369 6f6e 7219 0000 00da 0341 6e79  ersionr......Any
+00000dc0: 721d 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00000dd0: 2000 0000 7226 0000 0072 2800 0000 722b   ...r&...r(...r+
+00000de0: 0000 0072 2c00 0000 da04 626f 6f6c 722e  ...r,.....boolr.
+00000df0: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
+00000e00: 0000 7236 0000 00da 0d5f 5f63 6c61 7373  ..r6.....__class
+00000e10: 6365 6c6c 5f5f 720c 0000 0072 0c00 0000  cell__r....r....
+00000e20: 7231 0000 0072 0d00 0000 720e 0000 0041  r1...r....r....A
+00000e30: 0000 0073 1e00 0000 0801 0404 2a0a 0201  ...s........*...
+00000e40: 1005 0201 1003 0201 1003 0201 1004 1606  ................
+00000e50: 1606 1606 1606 720e 0000 0029 03da 0376  ......r....)...v
+00000e60: 6172 da07 6465 6661 756c 7472 1100 0000  ar..defaultr....
+00000e70: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000e80: 0004 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
+00000e90: 6a01 a002 7c00 7c01 a102 5300 7213 0000  j...|.|...S.r...
+00000ea0: 0029 03da 026f 73da 0765 6e76 6972 6f6e  .)...os..environ
+00000eb0: da03 6765 7429 0272 3e00 0000 723f 0000  ..get).r>...r?..
+00000ec0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000ed0: da07 6765 745f 656e 7682 0000 0073 0200  ..get_env....s..
+00000ee0: 0000 0001 7243 0000 0063 0000 0000 0000  ....rC...c......
+00000ef0: 0000 0000 0000 0000 0000 0b00 0000 4000  ..............@.
+00000f00: 0000 73dc 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000f10: 015a 0364 0264 0364 0464 0564 0664 0764  .Z.d.d.d.d.d.d.d
+00000f20: 0864 0964 0a64 0b9c 0964 0c64 0d64 0e64  .d.d.d...d.d.d.d
+00000f30: 0e64 0f64 0d64 0864 1064 1164 0b9c 0964  .d.d.d.d.d.d...d
+00000f40: 129c 025a 0465 056a 0664 136b 0572 8a65  ...Z.e.j.d.k.r.e
+00000f50: 04a0 0764 14a1 0101 0065 0464 1519 00a0  ...d.....e.d....
+00000f60: 0764 16a1 0101 0065 0464 1519 00a0 0764  .d.....e.d.....d
+00000f70: 17a1 0101 0065 0464 1519 00a0 0764 18a1  .....e.d.....d..
+00000f80: 0101 0065 0464 1519 00a0 0764 19a1 0101  ...e.d.....d....
+00000f90: 0065 056a 0864 1a6b 0272 a065 04a0 0764  .e.j.d.k.r.e...d
+00000fa0: 1464 1ba1 0201 0065 0964 1b64 1c9c 0264  .d.....e.d.d...d
+00000fb0: 1d64 1e84 045a 0a65 0965 0964 1f9c 0264  .d...Z.e.e.d...d
+00000fc0: 2064 2184 045a 0b65 0c6a 0d65 0965 0966   d!..Z.e.j.e.e.f
+00000fd0: 0219 0064 229c 0164 2364 2484 045a 0e64  ...d"..d#d$..Z.d
+00000fe0: 1b53 0029 25da 0e52 6564 6973 4149 5665  .S.)%..RedisAIVe
+00000ff0: 7273 696f 6e61 ff01 0000 4120 7375 6263  rsiona....A subc
+00001000: 6c61 7373 206f 6620 5665 7273 696f 6e5f  lass of Version_
+00001010: 2074 6861 7420 686f 6c64 7320 7468 6520   that holds the 
+00001020: 6465 7065 6e64 656e 6379 2073 6574 7320  dependency sets 
+00001030: 666f 7220 5265 6469 7341 490a 0a20 2020  for RedisAI..   
+00001040: 2074 6869 7320 636c 6173 7320 7365 7276   this class serv
+00001050: 6573 2074 776f 2070 7572 706f 7365 733a  es two purposes:
+00001060: 0a0a 2020 2020 312e 2049 7420 6973 2075  ..    1. It is u
+00001070: 7365 6420 746f 2070 6f70 756c 6174 6520  sed to populate 
+00001080: 7468 6520 5b6d 6c5d 2060 6065 7874 7261  the [ml] ``extra
+00001090: 735f 7265 7175 6972 6560 6020 6f66 2074  s_require`` of t
+000010a0: 6865 2073 6574 7570 2e70 792e 0a20 2020  he setup.py..   
+000010b0: 2054 6869 7320 6973 2062 6563 6175 7365   This is because
+000010c0: 2074 6865 2052 6564 6973 4149 2076 6572   the RedisAI ver
+000010d0: 7369 6f6e 2077 696c 6c20 6465 7465 726d  sion will determ
+000010e0: 696e 6520 7768 6963 6820 4d4c 2062 6173  ine which ML bas
+000010f0: 6564 0a20 2020 2064 6570 656e 6465 6e63  ed.    dependenc
+00001100: 6965 7320 6172 6520 7265 7175 6972 6564  ies are required
+00001110: 2e0a 0a20 2020 2032 2e20 5573 6564 2074  ...    2. Used t
+00001120: 6f20 7365 7420 7468 6520 6465 6661 756c  o set the defaul
+00001130: 7420 7661 6c75 6573 2066 6f72 2050 7954  t values for PyT
+00001140: 6f72 6368 2c20 5446 2c20 616e 6420 4f4e  orch, TF, and ON
+00001150: 4e58 0a20 2020 2067 6976 656e 2074 6865  NX.    given the
+00001160: 2053 4d41 5254 5349 4d5f 5245 4449 5341   SMARTSIM_REDISA
+00001170: 4920 656e 7620 7661 7220 7365 7420 6279  I env var set by
+00001180: 2074 6865 2075 7365 722e 0a0a 2020 2020   the user...    
+00001190: 4e4f 5445 3a20 546f 7263 6820 7265 7175  NOTE: Torch requ
+000011a0: 6972 6573 2061 6464 6974 696f 6e61 6c20  ires additional 
+000011b0: 696e 666f 726d 6174 696f 6e20 6465 7065  information depe
+000011c0: 6e64 696e 6720 6f6e 2077 6865 7468 6572  nding on whether
+000011d0: 0a20 2020 2043 5055 206f 7220 4750 5520  .    CPU or GPU 
+000011e0: 7375 7070 6f72 7420 6973 2072 6571 7565  support is reque
+000011f0: 7374 6564 0a20 2020 207a 0532 2e36 2e32  sted.    z.2.6.2
+00001200: 7a05 312e 392e 307a 0631 2e31 302e 337a  z.1.9.0z.1.10.3z
+00001210: 0631 2e31 302e 307a 0531 2e30 2e32 7a05  .1.10.0z.1.0.2z.
+00001220: 312e 392e 317a 042b 6370 757a 062b 6375  1.9.1z.+cpuz.+cu
+00001230: 3131 317a 0630 2e31 302e 3129 09da 0a74  111z.0.10.1)...t
+00001240: 656e 736f 7266 6c6f 77da 046f 6e6e 78da  ensorflow..onnx.
+00001250: 0873 6b6c 326f 6e6e 78da 0b6f 6e6e 786d  .skl2onnx..onnxm
+00001260: 6c74 6f6f 6c73 fa0c 7363 696b 6974 2d6c  ltools..scikit-l
+00001270: 6561 726e da05 746f 7263 68da 1074 6f72  earn..torch..tor
+00001280: 6368 5f63 7075 5f73 7566 6669 78da 1174  ch_cpu_suffix..t
+00001290: 6f72 6368 5f63 7564 615f 7375 6666 6978  orch_cuda_suffix
+000012a0: da0b 746f 7263 6876 6973 696f 6e7a 0532  ..torchvisionz.2
+000012b0: 2e38 2e30 7a06 312e 3131 2e30 7a06 312e  .8.0z.1.11.0z.1.
+000012c0: 3131 2e31 7a05 312e 312e 317a 062b 6375  11.1z.1.1.1z.+cu
+000012d0: 3131 337a 0630 2e31 322e 3029 02fa 0531  113z.0.12.0)...1
+000012e0: 2e32 2e35 fa05 312e 322e 3729 02e9 0300  .2.5..1.2.7)....
+000012f0: 0000 e90a 0000 0072 4e00 0000 724f 0000  .......rN...rO..
+00001300: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+00001310: 7249 0000 00da 0664 6172 7769 6e4e 720f  rI.....darwinNr.
+00001320: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001330: 0300 0000 0600 0000 4300 0000 736c 0000  ........C...sl..
+00001340: 0074 0064 0164 0284 007c 006a 0144 0083  .t.d.d...|.j.D..
+00001350: 0183 017d 027c 027c 016b 0472 2a74 0264  ...}.|.|.k.r*t.d
+00001360: 037c 029b 009d 0283 0182 017c 017c 006a  .|.........|.|.j
+00001370: 016b 0772 627c 01a0 0364 04a1 0172 4664  .k.rb|...d...rFd
+00001380: 057c 005f 0471 6874 0264 067c 019b 0064  .|._.qht.d.|...d
+00001390: 077c 006a 01a0 05a1 009b 009d 0483 0182  .|.j............
+000013a0: 016e 067c 017c 005f 0464 0053 0029 084e  .n.|.|._.d.S.).N
+000013b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000013c0: 0003 0000 0073 0000 0073 1600 0000 7c00  .....s...s....|.
+000013d0: 5d0e 7d01 7400 7c01 8301 5600 0100 7102  ].}.t.|...V...q.
+000013e0: 6400 5300 7213 0000 0029 0172 0e00 0000  d.S.r....).r....
+000013f0: 2902 7215 0000 00da 0376 6572 720c 0000  ).r......verr...
+00001400: 0072 0c00 0000 720d 0000 0072 1700 0000  .r....r....r....
+00001410: ba00 0000 7304 0000 0004 0002 007a 2a52  ....s........z*R
+00001420: 6564 6973 4149 5665 7273 696f 6e2e 5f5f  edisAIVersion.__
+00001430: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00001440: 3c67 656e 6578 7072 3e7a 3152 6564 6973  <genexpr>z1Redis
+00001450: 4149 2076 6572 7369 6f6e 206d 7573 7420  AI version must 
+00001460: 6265 2067 7265 6174 6572 2074 6861 6e20  be greater than 
+00001470: 6f72 2065 7175 616c 2074 6f20 7a03 312e  or equal to z.1.
+00001480: 3272 4f00 0000 7a18 496e 7661 6c69 6420  2rO...z.Invalid 
+00001490: 5265 6469 7341 4920 7665 7273 696f 6e20  RedisAI version 
+000014a0: 7a0e 2e20 4f70 7469 6f6e 7320 6172 6520  z.. Options are 
+000014b0: 2906 da03 6d69 6eda 0864 6566 6175 6c74  )...min..default
+000014c0: 7372 0700 0000 da0a 7374 6172 7473 7769  sr......startswi
+000014d0: 7468 7239 0000 00da 046b 6579 7329 0372  thr9.....keys).r
+000014e0: 1c00 0000 7210 0000 005a 0f6d 696e 5f72  ....r....Z.min_r
+000014f0: 6169 5f76 6572 7369 6f6e 720c 0000 0072  ai_versionr....r
+00001500: 0c00 0000 720d 0000 00da 085f 5f69 6e69  ....r......__ini
+00001510: 745f 5fb9 0000 0073 1800 0000 0001 1401  t__....s........
+00001520: 0801 0201 08ff 0403 0a01 0a03 0802 0201  ................
+00001530: 14ff 0604 7a17 5265 6469 7341 4956 6572  ....z.RedisAIVer
+00001540: 7369 6f6e 2e5f 5f69 6e69 745f 5f29 02da  sion.__init__)..
+00001550: 046e 616d 6572 1100 0000 6302 0000 0000  .namer....c.....
+00001560: 0000 0000 0000 0002 0000 0009 0000 0043  ...............C
+00001570: 0000 0073 4a00 0000 7a12 7c00 6a00 7c00  ...sJ...z.|.j.|.
+00001580: 6a01 1900 7c01 1900 5700 5300 0400 7402  j...|...W.S...t.
+00001590: 6b0a 7244 0100 0100 0100 7403 6401 7404  k.rD......t.d.t.
+000015a0: 7c00 8301 6a05 9b00 6402 7c01 9b00 6403  |...j...d.|...d.
+000015b0: 9d05 8301 6400 8202 5900 6e02 5800 6400  ....d...Y.n.X.d.
+000015c0: 5300 2904 4efa 0127 7a1b 2720 6f62 6a65  S.).N..'z.' obje
+000015d0: 6374 2068 6173 206e 6f20 6174 7472 6962  ct has no attrib
+000015e0: 7574 6520 277a e427 0a0a 5468 6973 2069  ute 'z.'..This i
+000015f0: 7320 6c69 6b65 6c79 2061 2070 726f 626c  s likely a probl
+00001600: 656d 2077 6974 6820 7468 6520 536d 6172  em with the Smar
+00001610: 7453 696d 2062 7569 6c64 2070 726f 6365  tSim build proce
+00001620: 7373 3b69 6620 7468 6973 2070 726f 626c  ss;if this probl
+00001630: 656d 2070 6572 7369 7374 7320 706c 6561  em persists plea
+00001640: 7365 206c 6f67 2061 206e 6577 2069 7373  se log a new iss
+00001650: 7565 2061 7420 6874 7470 733a 2f2f 6769  ue at https://gi
+00001660: 7468 7562 2e63 6f6d 2f43 7261 794c 6162  thub.com/CrayLab
+00001670: 732f 536d 6172 7453 696d 2f69 7373 7565  s/SmartSim/issue
+00001680: 7320 6f72 2067 6574 2069 6e20 636f 6e74  s or get in cont
+00001690: 6163 7420 7769 7468 2075 7320 6174 2068  act with us at h
+000016a0: 7474 7073 3a2f 2f77 7777 2e63 7261 796c  ttps://www.crayl
+000016b0: 6162 732e 6f72 672f 646f 6373 2f63 6f6d  abs.org/docs/com
+000016c0: 6d75 6e69 7479 2e68 746d 6c29 0672 5500  munity.html).rU.
+000016d0: 0000 7239 0000 00da 084b 6579 4572 726f  ..r9.....KeyErro
+000016e0: 72da 0e41 7474 7269 6275 7465 4572 726f  r..AttributeErro
+000016f0: 72da 0474 7970 6572 0800 0000 2902 721c  r..typer....).r.
+00001700: 0000 0072 5900 0000 720c 0000 0072 0c00  ...rY...r....r..
+00001710: 0000 720d 0000 00da 0b5f 5f67 6574 6174  ..r......__getat
+00001720: 7472 5f5f cb00 0000 7310 0000 0000 0102  tr__....s.......
+00001730: 0112 010e 0102 0116 ff02 0702 f97a 1a52  .............z.R
+00001740: 6564 6973 4149 5665 7273 696f 6e2e 5f5f  edisAIVersion.__
+00001750: 6765 7461 7474 725f 5f72 1e00 0000 6301  getattr__r....c.
+00001760: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001770: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
+00001780: 7c00 6a01 1900 a002 a100 5300 7213 0000  |.j.......S.r...
+00001790: 0029 0372 5500 0000 7239 0000 00da 0463  .).rU...r9.....c
+000017a0: 6f70 7972 2500 0000 720c 0000 0072 0c00  opyr%...r....r..
+000017b0: 0000 720d 0000 00da 0c67 6574 5f64 6566  ..r......get_def
+000017c0: 6175 6c74 73d8 0000 0073 0200 0000 0001  aults....s......
+000017d0: 7a1b 5265 6469 7341 4956 6572 7369 6f6e  z.RedisAIVersion
+000017e0: 2e67 6574 5f64 6566 6175 6c74 7329 0f72  .get_defaults).r
+000017f0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00001800: 0000 0072 5500 0000 da03 7379 73da 0c76  ...rU.....sys..v
+00001810: 6572 7369 6f6e 5f69 6e66 6fda 0370 6f70  ersion_info..pop
+00001820: da08 706c 6174 666f 726d 7214 0000 0072  ..platformr....r
+00001830: 5800 0000 725e 0000 0072 3700 0000 da04  X...r^...r7.....
+00001840: 4469 6374 7260 0000 0072 0c00 0000 720c  Dictr`...r....r.
+00001850: 0000 0072 0c00 0000 720d 0000 0072 4400  ...r....r....rD.
+00001860: 0000 8600 0000 7342 0000 0008 0104 1102  ......sB........
+00001870: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001880: f704 0c02 0102 0102 0102 0102 0102 0102  ................
+00001890: 0102 0102 f704 f406 190a 010a 010e 010e  ................
+000018a0: 010e 010e 020a 010c 0210 1210 0d72 4400  .............rD.
+000018b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000018c0: 0000 0008 0000 0040 0000 0073 4c01 0000  .......@...sL...
+000018d0: 6500 5a01 6400 5a02 6401 5a03 6504 6402  e.Z.d.Z.d.Z.e.d.
+000018e0: 8301 5a05 6504 6506 6403 6404 8302 8301  ..Z.e.e.d.d.....
+000018f0: 5a07 6504 6506 6405 6406 8302 8301 5a08  Z.e.e.d.d.....Z.
+00001900: 6506 6407 6408 8302 5a09 6504 6506 6409  e.d.d...Z.e.e.d.
+00001910: 640a 8302 8301 5a0a 6506 640b 640c 8302  d.....Z.e.d.d...
+00001920: 5a0b 6506 640d 650a 8302 5a0c 650d 6506  Z.e.d.e...Z.e.e.
+00001930: 640e 640f 8302 8301 5a0e 6506 6410 6411  d.d.....Z.e.d.d.
+00001940: 8302 5a0f 6506 6412 6413 650e 9b00 9d02  ..Z.e.d.d.e.....
+00001950: 8302 5a10 6504 6506 6414 650e 6a11 8302  ..Z.e.e.d.e.j...
+00001960: 8301 5a12 6504 6506 6415 650e 6a13 8302  ..Z.e.e.d.e.j...
+00001970: 8301 5a14 6504 6506 6416 650e 6a15 8302  ..Z.e.e.d.e.j...
+00001980: 8301 5a16 6504 6506 6417 650e 6a17 8302  ..Z.e.e.d.e.j...
+00001990: 8301 5a18 6504 650e 6a19 8301 5a1a 7a0e  ..Z.e.e.j...Z.z.
+000019a0: 6504 650e 6a1b 8301 5a1c 5700 6e18 0400  e.e.j...Z.W.n...
+000019b0: 651d 6b0a 72f4 0100 0100 0100 6418 5a1c  e.k.r.......d.Z.
+000019c0: 5900 6e02 5800 6425 651e 651f 6a20 6521  Y.n.X.d%e.e.j e!
+000019d0: 651f 6a22 6602 1900 641a 9c02 641b 641c  e.j"f...d...d.d.
+000019e0: 8405 5a23 651f 6a24 6521 1900 641d 9c01  ..Z#e.j$e!..d...
+000019f0: 641e 641f 8404 5a25 6526 6521 6420 9c02  d.d...Z%e&e!d ..
+00001a00: 6421 6422 8404 5a27 6526 6521 6420 9c02  d!d"..Z'e&e!d ..
+00001a10: 6423 6424 8404 5a28 6418 5300 2926 da09  d#d$..Z(d.S.)&..
+00001a20: 5665 7273 696f 6e65 7261 6c03 0000 5665  Versioneral...Ve
+00001a30: 7273 696f 6e65 7220 6973 2072 6573 706f  rsioner is respo
+00001a40: 6e73 6962 6c65 2066 6f72 206d 616e 6167  nsible for manag
+00001a50: 696e 6720 616c 6c20 7468 6520 7665 7273  ing all the vers
+00001a60: 696f 6e73 0a20 2020 2077 6974 6869 6e20  ions.    within 
+00001a70: 536d 6172 7453 696d 2069 6e63 6c75 6469  SmartSim includi
+00001a80: 6e67 2053 6d61 7274 5369 6d20 6974 7365  ng SmartSim itse
+00001a90: 6c66 2e0a 0a20 2020 2053 6d61 7274 5369  lf...    SmartSi
+00001aa0: 6d27 7320 7665 7273 696f 6e20 6973 2077  m's version is w
+00001ab0: 7269 7474 656e 2069 6e74 6f20 7665 7273  ritten into vers
+00001ac0: 696f 6e2e 7079 2075 706f 6e20 7069 7020  ion.py upon pip 
+00001ad0: 696e 7374 616c 6c0a 2020 2020 6279 2075  install.    by u
+00001ae0: 7369 6e67 2074 6869 7320 636c 6173 7320  sing this class 
+00001af0: 696e 2073 6574 7570 2e70 792e 2042 7920  in setup.py. By 
+00001b00: 7365 7474 696e 6720 534d 4152 5453 494d  setting SMARTSIM
+00001b10: 5f53 5546 4649 582c 0a20 2020 2074 6865  _SUFFIX,.    the
+00001b20: 2076 6572 7369 6f6e 2077 696c 6c20 6265   version will be
+00001b30: 2077 7269 7474 656e 2061 7320 6120 2264   written as a "d
+00001b40: 6972 7479 2220 7665 7273 696f 6e20 7769  irty" version wi
+00001b50: 7468 2074 6865 0a20 2020 2067 6974 2d73  th the.    git-s
+00001b60: 6861 2061 7070 656e 6465 642e 0a20 2020  ha appended..   
+00001b70: 2069 2e65 2e0a 2020 2020 2020 2020 6578   i.e..        ex
+00001b80: 706f 7274 2053 4d41 5254 5349 4d5f 5355  port SMARTSIM_SU
+00001b90: 4646 4958 3d6e 6967 6874 6c79 0a20 2020  FFIX=nightly.   
+00001ba0: 2020 2020 2070 6970 2069 6e73 7461 6c6c       pip install
+00001bb0: 202d 6520 2e0a 2020 2020 2020 2020 736d   -e ..        sm
+00001bc0: 6172 7473 696d 2e5f 5f76 6572 7369 6f6e  artsim.__version
+00001bd0: 5f5f 203d 3d20 302e 332e 322b 6e69 6768  __ == 0.3.2+nigh
+00001be0: 746c 792d 3366 6532 3366 660a 0a20 2020  tly-3fe23ff..   
+00001bf0: 2056 6572 7369 6f6e 6572 206d 616e 6167   Versioner manag
+00001c00: 6573 2074 6869 7264 2070 6172 7479 2064  es third party d
+00001c10: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
+00001c20: 7468 6569 7220 7665 7273 696f 6e73 0a20  their versions. 
+00001c30: 2020 2061 7320 7765 6c6c 2e20 5468 6573     as well. Thes
+00001c40: 6520 7665 7273 696f 6e73 2061 7265 2075  e versions are u
+00001c50: 7365 6420 6279 2074 6865 2060 6073 6d61  sed by the ``sma
+00001c60: 7274 6060 2063 6c69 2069 6e20 7468 650a  rt`` cli in the.
+00001c70: 2020 2020 6060 736d 6172 7420 6275 696c      ``smart buil
+00001c80: 6460 6020 636f 6d6d 616e 6420 746f 2064  d`` command to d
+00001c90: 6574 6572 6d69 6e65 2077 6869 6368 2064  etermine which d
+00001ca0: 6570 656e 6465 6e63 7920 7665 7273 696f  ependency versio
+00001cb0: 6e73 0a20 2020 2074 6f20 6c6f 6f6b 2066  ns.    to look f
+00001cc0: 6f72 2061 6e64 2064 6f77 6e6c 6f61 642e  or and download.
+00001cd0: 0a0a 2020 2020 4465 6661 756c 7420 7665  ..    Default ve
+00001ce0: 7273 696f 6e73 2066 6f72 2053 6d61 7274  rsions for Smart
+00001cf0: 5369 6d2c 2053 6d61 7274 5265 6469 732c  Sim, SmartRedis,
+00001d00: 2052 6564 6973 2c20 616e 6420 5265 6469   Redis, and Redi
+00001d10: 7341 4920 6172 650a 2020 2020 616c 6c20  sAI are.    all 
+00001d20: 7365 7420 6865 7265 2e20 5365 7474 696e  set here. Settin
+00001d30: 6720 6120 6465 6661 756c 7420 7665 7273  g a default vers
+00001d40: 696f 6e20 666f 7220 5265 6469 7341 4920  ion for RedisAI 
+00001d50: 616c 736f 2064 6963 7461 7465 730a 2020  also dictates.  
+00001d60: 2020 6465 6661 756c 7420 7665 7273 696f    default versio
+00001d70: 6e73 206f 6620 7468 6520 6d61 6368 696e  ns of the machin
+00001d80: 6520 6c65 6172 6e69 6e67 206c 6962 7261  e learning libra
+00001d90: 7269 6573 2e0a 2020 2020 7a05 332e 382e  ries..    z.3.8.
+00001da0: 305a 1053 4d41 5254 5349 4d5f 5645 5253  0Z.SMARTSIM_VERS
+00001db0: 494f 4e7a 0530 2e35 2e30 5a12 534d 4152  IONz.0.5.0Z.SMAR
+00001dc0: 5452 4544 4953 5f56 4552 5349 4f4e 7a05  TREDIS_VERSIONz.
+00001dd0: 302e 342e 31da 0f53 4d41 5254 5349 4d5f  0.4.1..SMARTSIM_
+00001de0: 5355 4646 4958 da00 5a0e 534d 4152 5453  SUFFIX..Z.SMARTS
+00001df0: 494d 5f52 4544 4953 7a05 372e 302e 355a  IM_REDISz.7.0.5Z
+00001e00: 1253 4d41 5254 5349 4d5f 5245 4449 535f  .SMARTSIM_REDIS_
+00001e10: 5552 4c7a 2368 7474 7073 3a2f 2f67 6974  URLz#https://git
+00001e20: 6875 622e 636f 6d2f 7265 6469 732f 7265  hub.com/redis/re
+00001e30: 6469 732e 6769 742f 5a15 534d 4152 5453  dis.git/Z.SMARTS
+00001e40: 494d 5f52 4544 4953 5f42 5241 4e43 485a  IM_REDIS_BRANCHZ
+00001e50: 1053 4d41 5254 5349 4d5f 5245 4449 5341  .SMARTSIM_REDISA
+00001e60: 4972 4f00 0000 5a14 534d 4152 5453 494d  IrO...Z.SMARTSIM
+00001e70: 5f52 4544 4953 4149 5f55 524c 7a27 6874  _REDISAI_URLz'ht
+00001e80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001e90: 2f52 6564 6973 4149 2f52 6564 6973 4149  /RedisAI/RedisAI
+00001ea0: 2e67 6974 2f5a 1753 4d41 5254 5349 4d5f  .git/Z.SMARTSIM_
+00001eb0: 5245 4449 5341 495f 4252 414e 4348 da01  REDISAI_BRANCH..
+00001ec0: 765a 0e53 4d41 5254 5349 4d5f 544f 5243  vZ.SMARTSIM_TORC
+00001ed0: 485a 1153 4d41 5254 5349 4d5f 544f 5243  HZ.SMARTSIM_TORC
+00001ee0: 4856 4953 da10 544f 5243 485f 4350 555f  HVIS..TORCH_CPU_
+00001ef0: 5355 4646 4958 da11 544f 5243 485f 4355  SUFFIX..TORCH_CU
+00001f00: 4441 5f53 5546 4649 584e 7206 0000 0029  DA_SUFFIXNr....)
+00001f10: 02da 0764 625f 6e61 6d65 7211 0000 0063  ...db_namer....c
+00001f20: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00001f30: 0600 0000 4300 0000 7356 0000 0064 0164  ....C...sV...d.d
+00001f40: 027c 0164 0364 0464 0567 067d 027c 006a  .|.d.d.d.g.}.|.j
+00001f50: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
+00001f60: 047c 006a 0567 067d 037c 006a 0672 487c  .|.j.g.}.|.j.rH|
+00001f70: 02a0 0764 06a1 0101 007c 03a0 077c 006a  ...d.....|...|.j
+00001f80: 06a1 0101 007c 027c 0364 079c 027d 047c  .....|.|.d...}.|
+00001f90: 0453 0029 084e da08 534d 4152 5453 494d  .S.).N..SMARTSIM
+00001fa0: da0a 534d 4152 5452 4544 4953 da07 5245  ..SMARTREDIS..RE
+00001fb0: 4449 5341 49da 0554 4f52 4348 da0a 5445  DISAI..TORCH..TE
+00001fc0: 4e53 4f52 464c 4f57 da04 4f4e 4e58 2902  NSORFLOW..ONNX).
+00001fd0: 5a08 5061 636b 6167 6573 5a08 5665 7273  Z.PackagesZ.Vers
+00001fe0: 696f 6e73 2908 726d 0000 0072 6e00 0000  ions).rm...rn...
+00001ff0: 7206 0000 0072 6f00 0000 7270 0000 0072  r....ro...rp...r
+00002000: 7100 0000 7272 0000 00da 0661 7070 656e  q...rr.....appen
+00002010: 6429 0572 1c00 0000 726c 0000 00da 0870  d).r....rl.....p
+00002020: 6163 6b61 6765 73da 0876 6572 7369 6f6e  ackages..version
+00002030: 7372 1000 0000 720c 0000 0072 0c00 0000  sr....r....r....
+00002040: 720d 0000 00da 0761 735f 6469 6374 1801  r......as_dict..
+00002050: 0000 7326 0000 0000 0202 0102 0102 0102  ..s&............
+00002060: 0102 0102 fa04 0904 0104 0104 0104 0104  ................
+00002070: 0104 fa04 0806 010a 010c 010a 017a 1156  .............z.V
+00002080: 6572 7369 6f6e 6572 2e61 735f 6469 6374  ersioner.as_dict
+00002090: 721e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000020a0: 0000 0400 0000 0400 0000 4300 0000 733c  ..........C...s<
+000020b0: 0000 007c 006a 00a0 01a1 007d 0164 0164  ...|.j.....}.d.d
+000020c0: 0264 0364 0467 047d 027c 0244 005d 0e7d  .d.d.g.}.|.D.].}
+000020d0: 037c 01a0 027c 03a1 0101 0071 1a64 0564  .|...|.....q.d.d
+000020e0: 0684 007c 01a0 03a1 0044 0083 0153 0029  ...|.....D...S.)
+000020f0: 077a 744f 7074 696f 6e61 6c20 4d4c 2f44  .ztOptional ML/D
+00002100: 4c20 6465 7065 6e64 656e 6369 6573 2077  L dependencies w
+00002110: 6520 7375 6767 6573 7420 666f 7220 7468  e suggest for th
+00002120: 6520 7573 6572 2e0a 0a20 2020 2020 2020  e user...       
+00002130: 2054 6865 2064 6566 6175 6c74 7320 6172   The defaults ar
+00002140: 6520 6261 7365 6420 6f6e 2074 6865 2052  e based on the R
+00002150: 6564 6973 4149 2076 6572 7369 6f6e 0a20  edisAI version. 
+00002160: 2020 2020 2020 2072 4a00 0000 724d 0000         rJ...rM..
+00002170: 0072 4b00 0000 724c 0000 0063 0100 0000  .rK...rL...c....
+00002180: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00002190: 5300 0000 731e 0000 0067 007c 005d 165c  S...s....g.|.].\
+000021a0: 027d 017d 027c 019b 0064 007c 029b 009d  .}.}.|...d.|....
+000021b0: 0391 0271 0453 0029 017a 023d 3d72 0c00  ...q.S.).z.==r..
+000021c0: 0000 2903 7215 0000 00da 036c 6962 7210  ..).r......libr.
+000021d0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+000021e0: 0000 da0a 3c6c 6973 7463 6f6d 703e 4401  ....<listcomp>D.
+000021f0: 0000 7304 0000 0006 0006 007a 3056 6572  ..s........z0Ver
+00002200: 7369 6f6e 6572 2e6d 6c5f 6578 7472 6173  sioner.ml_extras
+00002210: 5f72 6571 7569 7265 642e 3c6c 6f63 616c  _required.<local
+00002220: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
+00002230: 6f00 0000 7260 0000 0072 6300 0000 da05  o...r`...rc.....
+00002240: 6974 656d 7329 0472 1c00 0000 5a0b 6d6c  items).r....Z.ml
+00002250: 5f64 6566 6175 6c74 735a 0d5f 746f 7263  _defaultsZ._torc
+00002260: 685f 6669 656c 6473 da05 6669 656c 6472  h_fields..fieldr
+00002270: 0c00 0000 720c 0000 0072 0d00 0000 da12  ....r....r......
+00002280: 6d6c 5f65 7874 7261 735f 7265 7175 6972  ml_extras_requir
+00002290: 6564 2f01 0000 7312 0000 0000 050a 0802  ed/...s.........
+000022a0: 0102 0102 0102 fc04 0608 010c 027a 1c56  .............z.V
+000022b0: 6572 7369 6f6e 6572 2e6d 6c5f 6578 7472  ersioner.ml_extr
+000022c0: 6173 5f72 6571 7569 7265 6429 02da 0c73  as_required)...s
+000022d0: 6574 7570 5f70 795f 6469 7272 1100 0000  etup_py_dirr....
+000022e0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+000022f0: 0008 0000 0043 0000 0073 5400 0000 7a38  .....C...sT...z8
+00002300: 6401 6402 6403 6703 7d02 7400 6a01 7c02  d.d.d.g.}.t.j.|.
+00002310: 7c01 a002 a100 6404 8d02 7d03 7c03 a003  |.....d...}.|...
+00002320: 6405 a101 a004 a100 7d04 7c04 6406 6407  d.......}.|.d.d.
+00002330: 8502 1900 5700 5300 0400 7405 6b0a 724e  ....W.S...t.k.rN
+00002340: 0100 0100 0100 5900 6408 5300 5800 6406  ......Y.d.S.X.d.
+00002350: 5300 2909 7a25 4765 7420 7468 6520 6769  S.).z%Get the gi
+00002360: 7420 7368 6120 6f66 2074 6865 2063 7572  t sha of the cur
+00002370: 7265 6e74 2062 7261 6e63 68da 0367 6974  rent branch..git
+00002380: 7a09 7265 762d 7061 7273 655a 0448 4541  z.rev-parseZ.HEA
+00002390: 4429 01da 0363 7764 da05 6173 6369 694e  D)...cwd..asciiN
+000023a0: e907 0000 0072 6800 0000 2906 da0a 7375  .....rh...)...su
+000023b0: 6270 726f 6365 7373 da0c 6368 6563 6b5f  bprocess..check_
+000023c0: 6f75 7470 7574 da08 6162 736f 6c75 7465  output..absolute
+000023d0: da06 6465 636f 6465 da05 7374 7269 70da  ..decode..strip.
+000023e0: 0945 7863 6570 7469 6f6e 2905 721c 0000  .Exception).r...
+000023f0: 0072 7c00 0000 5a07 7265 765f 636d 645a  .r|...Z.rev_cmdZ
+00002400: 0767 6974 5f72 6576 5a03 7368 6172 0c00  .git_revZ.shar..
+00002410: 0000 720c 0000 0072 0d00 0000 da07 6765  ..r....r......ge
+00002420: 745f 7368 6146 0100 0073 0e00 0000 0002  t_shaF...s......
+00002430: 0201 0a01 1201 0e02 0e01 0e02 7a11 5665  ............z.Ve
+00002440: 7273 696f 6e65 722e 6765 745f 7368 6163  rsioner.get_shac
+00002450: 0200 0000 0000 0000 0000 0000 0600 0000  ................
+00002460: 0900 0000 4300 0000 7388 0000 0074 007c  ....C...s....t.|
+00002470: 006a 0183 017d 027c 006a 0272 3c7c 0264  .j...}.|.j.r<|.d
+00002480: 017c 006a 029b 009d 0237 007d 027c 00a0  .|.j.....7.}.|..
+00002490: 037c 01a1 0104 007d 0372 3c7c 0264 027c  .|.....}.r<|.d.|
+000024a0: 039b 009d 0237 007d 027c 0164 031b 0064  .....7.}.|.d...d
+000024b0: 041b 007d 0474 047c 0464 0583 028f 2c7d  ...}.t.|.d....,}
+000024c0: 057c 05a0 0564 06a1 0101 007c 05a0 0564  .|...d.....|...d
+000024d0: 07a1 0101 007c 05a0 0564 087c 029b 0064  .....|...d.|...d
+000024e0: 099d 03a1 0101 0057 0035 0051 0052 0058  .......W.5.Q.R.X
+000024f0: 007c 0253 0029 0a7a 830a 2020 2020 2020  .|.S.).z..      
+00002500: 2020 5772 6974 6520 7665 7273 696f 6e20    Write version 
+00002510: 696e 666f 2074 6f20 7665 7273 696f 6e2e  info to version.
+00002520: 7079 0a0a 2020 2020 2020 2020 5573 6520  py..        Use 
+00002530: 6769 745f 7368 6120 696e 2074 6865 2063  git_sha in the c
+00002540: 6173 6520 7768 6572 6520 736d 6172 7473  ase where smarts
+00002550: 696d 2073 7566 6669 7820 6973 2073 6574  im suffix is set
+00002560: 2069 6e20 7468 6520 656e 7669 726f 6e6d   in the environm
+00002570: 656e 740a 2020 2020 2020 2020 fa01 2b72  ent.        ..+r
+00002580: 1200 0000 da08 736d 6172 7473 696d 7a0a  ......smartsimz.
+00002590: 7665 7273 696f 6e2e 7079 da01 777a 3323  version.py..wz3#
+000025a0: 2054 6869 7320 6669 6c65 2069 7320 6175   This file is au
+000025b0: 746f 6d61 7469 6361 6c6c 7920 6765 6e65  tomatically gene
+000025c0: 7261 7465 6420 6279 2073 6574 7570 2e70  rated by setup.p
+000025d0: 790a 7a23 2320 646f 206e 6f74 2065 6469  y.z## do not edi
+000025e0: 7420 7468 6973 2066 696c 6520 6d61 6e75  t this file manu
+000025f0: 616c 6c79 2e0a 0a7a 0f5f 5f76 6572 7369  ally...z.__versi
+00002600: 6f6e 5f5f 203d 2027 7a02 270a 2906 7214  on__ = 'z.'.).r.
+00002610: 0000 0072 6d00 0000 7267 0000 0072 8700  ...rm...rg...r..
+00002620: 0000 da04 6f70 656e da05 7772 6974 6529  ....open..write)
+00002630: 0672 1c00 0000 727c 0000 0072 3900 0000  .r....r|...r9...
+00002640: 5a07 6769 745f 7368 615a 0c76 6572 7369  Z.git_shaZ.versi
+00002650: 6f6e 5f66 696c 65da 0166 720c 0000 0072  on_file..fr....r
+00002660: 0c00 0000 720d 0000 00da 0d77 7269 7465  ....r......write
+00002670: 5f76 6572 7369 6f6e 5201 0000 7316 0000  _versionR...s...
+00002680: 0000 060a 0206 0110 030e 010e 020c 010c  ................
+00002690: 010a 010a 021c 017a 1756 6572 7369 6f6e  .......z.Version
+000026a0: 6572 2e77 7269 7465 5f76 6572 7369 6f6e  er.write_version
+000026b0: 2901 7206 0000 0029 2972 0800 0000 7209  ).r....))r....r.
+000026c0: 0000 0072 0a00 0000 720b 0000 0072 0e00  ...r....r....r..
+000026d0: 0000 da0a 5059 5448 4f4e 5f4d 494e 7243  ....PYTHON_MINrC
+000026e0: 0000 0072 6d00 0000 726e 0000 0072 6700  ...rm...rn...rg.
+000026f0: 0000 7206 0000 00da 0952 4544 4953 5f55  ..r......REDIS_U
+00002700: 524c 5a0c 5245 4449 535f 4252 414e 4348  RLZ.REDIS_BRANCH
+00002710: 7244 0000 0072 6f00 0000 5a0b 5245 4449  rD...ro...Z.REDI
+00002720: 5341 495f 5552 4c5a 0e52 4544 4953 4149  SAI_URLZ.REDISAI
+00002730: 5f42 5241 4e43 4872 4a00 0000 7270 0000  _BRANCHrJ...rp..
+00002740: 0072 4d00 0000 5a0b 544f 5243 4856 4953  .rM...Z.TORCHVIS
+00002750: 494f 4e72 4b00 0000 726a 0000 0072 4c00  IONrK...rj...rL.
+00002760: 0000 726b 0000 0072 4500 0000 7271 0000  ..rk...rE...rq..
+00002770: 0072 4600 0000 7272 0000 0072 5c00 0000  .rF...rr...r\...
+00002780: da08 4462 456e 6769 6e65 7237 0000 0072  ..DbEnginer7...r
+00002790: 6500 0000 7214 0000 0072 3a00 0000 7276  e...r....r:...rv
+000027a0: 0000 00da 044c 6973 7472 7b00 0000 7203  .....Listr{...r.
+000027b0: 0000 0072 8700 0000 728e 0000 0072 0c00  ...r....r....r..
+000027c0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000027d0: 0072 6600 0000 dc00 0000 733a 0000 0008  .rf.......s:....
+000027e0: 0104 1708 030e 010e 010a 030e 010a 010a  ................
+000027f0: 030e 0102 0102 0002 ff04 0310 0410 0110  ................
+00002800: 0110 0102 010a ff04 060a 0102 010e 010e  ................
+00002810: 010a 021e 1714 1710 0c72 6600 0000 6300  .........rf...c.
+00002820: 0000 0000 0000 0000 0000 0000 0000 0006  ................
+00002830: 0000 0040 0000 0073 7c01 0000 6500 5a01  ...@...s|...e.Z.
+00002840: 6400 5a02 6401 5a03 6504 6a05 a006 6402  d.Z.d.Z.e.j...d.
+00002850: 6403 a102 5a07 6504 6a05 a006 6404 6405  d...Z.e.j...d.d.
+00002860: a102 5a08 6504 6a05 a006 6406 6407 a102  ..Z.e.j...d.d...
+00002870: 5a09 6504 6a05 a006 6408 6407 a102 5a0a  Z.e.j...d.d...Z.
+00002880: 6504 6a05 a006 6409 640a a102 5a0b 650c  e.j...d.d...Z.e.
+00002890: 6504 6a05 a006 640b 640c a102 8301 5a0d  e.j...d.d.....Z.
+000028a0: 650c 6504 6a05 a006 640d 640e a102 8301  e.e.j...d.d.....
+000028b0: 5a0e 650f 6a10 5a11 642e 6512 6410 6411  Z.e.j.Z.d.e.d.d.
+000028c0: 9c02 6412 6413 8405 5a13 6410 6414 9c01  ..d.d...Z.d.d...
+000028d0: 6415 6416 8404 5a14 6515 6a16 6517 6517  d.d...Z.e.j.e.e.
+000028e0: 6602 1900 6414 9c01 6417 6418 8404 5a18  f...d...d.d...Z.
+000028f0: 6515 6a16 6517 6515 6a19 6517 1900 6602  e.j.e.e.j.e...f.
+00002900: 1900 6414 9c01 6419 641a 8404 5a1a 651b  ..d...d.d...Z.e.
+00002910: 6517 6414 9c01 641b 641c 8404 8301 5a1c  e.d...d.d.....Z.
+00002920: 651d 6512 641d 9c02 641e 641f 8404 5a1e  e.e.d...d.d...Z.
+00002930: 6512 6414 9c01 6420 6421 8404 5a1f 6512  e.d...d d!..Z.e.
+00002940: 6414 9c01 6422 6423 8404 5a20 651b 6515  d...d"d#..Z e.e.
+00002950: 6a21 6517 1900 6414 9c01 6424 6425 8404  j!e...d...d$d%..
+00002960: 8301 5a22 6523 6515 6a21 6515 6a16 6517  ..Z"e#e.j!e.j.e.
+00002970: 6517 6602 1900 1900 6414 9c01 6426 6427  e.f.....d...d&d'
+00002980: 8404 8301 5a24 6517 6410 6428 9c02 6429  ....Z$e.d.d(..d)
+00002990: 642a 8404 5a25 6523 642f 6517 6515 6a21  d*..Z%e#d/e.e.j!
+000029a0: 6526 1900 6512 642b 9c03 642c 642d 8405  e&..e.d+..d,d-..
+000029b0: 8301 5a27 6410 5300 2930 da08 4275 696c  ..Z'd.S.)0..Buil
+000029c0: 6445 6e76 6137 0200 0045 6e76 6972 6f6e  dEnva7...Environ
+000029d0: 6d65 6e74 2066 6f72 2062 7569 6c64 696e  ment for buildin
+000029e0: 6720 7468 6972 642d 7061 7274 7920 6465  g third-party de
+000029f0: 7065 6e64 656e 6369 6573 0a0a 2020 2020  pendencies..    
+00002a00: 4275 696c 6445 6e76 2070 726f 7669 6465  BuildEnv provide
+00002a10: 7320 6120 6d65 7468 6f64 2066 6f72 2063  s a method for c
+00002a20: 6f6e 6669 6775 7269 6e67 2068 6f77 2074  onfiguring how t
+00002a30: 6865 2074 6869 7264 2d70 6172 7479 0a20  he third-party. 
+00002a40: 2020 2064 6570 656e 6465 6e63 6965 7320     dependencies 
+00002a50: 7769 7468 696e 2053 6d61 7274 5369 6d20  within SmartSim 
+00002a60: 6172 6520 6275 696c 742c 206e 616d 656c  are built, namel
+00002a70: 7920 5265 6469 732f 4b65 7944 420a 2020  y Redis/KeyDB.  
+00002a80: 2020 616e 6420 5265 6469 7341 492e 0a0a    and RedisAI...
+00002a90: 2020 2020 5468 6520 656e 7669 726f 6e6d      The environm
+00002aa0: 656e 7420 7661 7269 6162 6c65 7320 6c69  ent variables li
+00002ab0: 7374 6564 2068 6572 6520 6361 6e20 6265  sted here can be
+00002ac0: 2073 6574 2074 6f20 636f 6e74 726f 6c20   set to control 
+00002ad0: 7468 650a 2020 2020 5265 6469 7320 6275  the.    Redis bu
+00002ae0: 696c 6420 696e 2074 6865 2070 6970 2077  ild in the pip w
+00002af0: 6865 656c 2062 7569 6c64 2061 7320 7765  heel build as we
+00002b00: 6c6c 2061 7320 7468 6520 5265 6469 7320  ll as the Redis 
+00002b10: 616e 6420 5265 6469 7341 490a 2020 2020  and RedisAI.    
+00002b20: 6275 696c 6420 6578 6563 7574 6564 2062  build executed b
+00002b30: 7920 7468 6520 434c 492e 0a0a 2020 2020  y the CLI...    
+00002b40: 4275 696c 6420 746f 6f6c 7320 6172 6520  Build tools are 
+00002b50: 616c 736f 2063 6865 636b 6564 2066 6f72  also checked for
+00002b60: 2068 6572 6520 616e 6420 6966 2074 6865   here and if the
+00002b70: 7920 6172 6520 6e6f 7420 666f 756e 640a  y are not found.
+00002b80: 2020 2020 7468 656e 2061 2053 6574 7570      then a Setup
+00002b90: 4572 726f 7220 6973 2072 6169 7365 642e  Error is raised.
+00002ba0: 0a0a 2020 2020 4164 6469 6e67 2074 6865  ..    Adding the
+00002bb0: 202d 7620 666c 6167 2074 6f20 6060 736d   -v flag to ``sm
+00002bc0: 6172 7420 6275 696c 6460 6020 7769 6c6c  art build`` will
+00002bd0: 2073 686f 7720 7468 6520 6275 696c 6420   show the build 
+00002be0: 656e 7669 726f 6e6d 656e 740a 2020 2020  environment.    
+00002bf0: 6265 696e 6720 7573 6564 2e0a 2020 2020  being used..    
+00002c00: da02 4343 5a03 6763 63da 0343 5858 7a03  ..CCZ.gcc..CXXz.
+00002c10: 672b 2bda 0643 464c 4147 5372 6800 0000  g++..CFLAGSrh...
+00002c20: da08 4358 5846 4c41 4753 da06 4d41 4c4c  ..CXXFLAGS..MALL
+00002c30: 4f43 da04 6c69 6263 5a0a 4255 494c 445f  OC..libcZ.BUILD_
+00002c40: 4a4f 4253 7227 0000 005a 094e 4f5f 4348  JOBSr'...Z.NO_CH
+00002c50: 4543 4b53 7201 0000 0054 4e29 02da 0663  ECKSr....TN)...c
+00002c60: 6865 636b 7372 1100 0000 6302 0000 0000  hecksr....c.....
+00002c70: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00002c80: 0000 0073 1000 0000 7c01 720c 7c00 a000  ...s....|.r.|...
+00002c90: a100 0100 6400 5300 7213 0000 0029 01da  ....d.S.r....)..
+00002ca0: 1263 6865 636b 5f64 6570 656e 6465 6e63  .check_dependenc
+00002cb0: 6965 7329 0272 1c00 0000 729a 0000 0072  ies).r....r....r
+00002cc0: 0c00 0000 720c 0000 0072 0d00 0000 7258  ....r....r....rX
+00002cd0: 0000 008a 0100 0073 0400 0000 0001 0401  .......s........
+00002ce0: 7a11 4275 696c 6445 6e76 2e5f 5f69 6e69  z.BuildEnv.__ini
+00002cf0: 745f 5f72 1e00 0000 6301 0000 0000 0000  t__r....c.......
+00002d00: 0000 0000 0003 0000 0007 0000 0043 0000  .............C..
+00002d10: 0073 3c00 0000 6401 6402 6403 6404 6405  .s<...d.d.d.d.d.
+00002d20: 7c00 6a00 7c00 6a01 6707 7d01 7402 7c00  |.j.|.j.g.}.t.|.
+00002d30: 6a03 8301 6406 6b02 7238 7c01 4400 5d0e  j...d.k.r8|.D.].
+00002d40: 7d02 7c00 a004 7c02 a101 0100 7128 6400  }.|...|.....q(d.
+00002d50: 5300 2907 4e72 7d00 0000 7a07 6769 742d  S.).Nr}...z.git-
+00002d60: 6c66 73da 046d 616b 655a 0477 6765 745a  lfs..makeZ.wgetZ
+00002d70: 0563 6d61 6b65 7201 0000 0029 0572 9400  .cmaker....).r..
+00002d80: 0000 7295 0000 0072 2000 0000 da06 4348  ..r....r .....CH
+00002d90: 4543 4b53 da16 6368 6563 6b5f 6275 696c  ECKS..check_buil
+00002da0: 645f 6465 7065 6e64 656e 6379 2903 721c  d_dependency).r.
+00002db0: 0000 00da 0464 6570 73da 0364 6570 720c  .....deps..depr.
+00002dc0: 0000 0072 0c00 0000 720d 0000 0072 9b00  ...r....r....r..
+00002dd0: 0000 8e01 0000 7308 0000 0000 0116 010e  ......s.........
+00002de0: 0108 017a 1b42 7569 6c64 456e 762e 6368  ...z.BuildEnv.ch
+00002df0: 6563 6b5f 6465 7065 6e64 656e 6369 6573  eck_dependencies
+00002e00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002e10: 0007 0000 0043 0000 0073 2a00 0000 7400  .....C...s*...t.
+00002e20: 6a01 a002 a100 7d01 7c01 a003 7c00 6a04  j.....}.|...|.j.
+00002e30: 7c00 6a05 7c00 6a06 7c00 6a07 6401 9c04  |.j.|.j.|.j.d...
+00002e40: a101 0100 7c01 5300 2902 4e29 0472 9400  ....|.S.).N).r..
+00002e50: 0000 7295 0000 0072 9600 0000 7297 0000  ..r....r....r...
+00002e60: 0029 0872 4000 0000 7241 0000 0072 5f00  .).r@...rA...r_.
+00002e70: 0000 da06 7570 6461 7465 7294 0000 0072  ....updater....r
+00002e80: 9500 0000 7296 0000 0072 9700 0000 2902  ....r....r....).
+00002e90: 721c 0000 00da 0365 6e76 720c 0000 0072  r......envr....r
+00002ea0: 0c00 0000 720d 0000 00da 085f 5f63 616c  ....r......__cal
+00002eb0: 6c5f 5f94 0100 0073 1200 0000 0002 0a01  l__....s........
+00002ec0: 0402 0401 0401 0401 04fc 04ff 0408 7a11  ..............z.
+00002ed0: 4275 696c 6445 6e76 2e5f 5f63 616c 6c5f  BuildEnv.__call_
+00002ee0: 5f63 0100 0000 0000 0000 0000 0000 0400  _c..............
+00002ef0: 0000 0800 0000 4300 0000 734a 0000 0064  ......C...sJ...d
+00002f00: 0164 0264 0364 0464 0564 0664 0764 0867  .d.d.d.d.d.d.d.g
+00002f10: 087d 017c 006a 007c 006a 017c 006a 027c  .}.|.j.|.j.|.j.|
+00002f20: 006a 037c 006a 0474 057c 006a 0683 017c  .j.|.j.t.|.j...|
+00002f30: 006a 077c 006a 0867 087d 027c 017c 0264  .j.|.j.g.}.|.|.d
+00002f40: 099c 027d 037c 0353 0029 0a4e 7294 0000  ...}.|.S.).Nr...
+00002f50: 0072 9500 0000 7296 0000 0072 9700 0000  .r....r....r....
+00002f60: 7298 0000 00da 044a 4f42 535a 0e50 5954  r......JOBSZ.PYT
+00002f70: 484f 4e5f 5645 5253 494f 4eda 0850 4c41  HON_VERSION..PLA
+00002f80: 5446 4f52 4d29 02da 0b45 6e76 6972 6f6e  TFORM)...Environ
+00002f90: 6d65 6e74 5a06 5661 6c75 6573 2909 7294  mentZ.Values).r.
+00002fa0: 0000 0072 9500 0000 7296 0000 0072 9700  ...r....r....r..
+00002fb0: 0000 7298 0000 0072 1400 0000 72a4 0000  ..r....r....r...
+00002fc0: 00da 0e70 7974 686f 6e5f 7665 7273 696f  ...python_versio
+00002fd0: 6e72 a500 0000 2904 721c 0000 00da 0976  nr....).r......v
+00002fe0: 6172 6961 626c 6573 da06 7661 6c75 6573  ariables..values
+00002ff0: 72a2 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00003000: 0d00 0000 7276 0000 00a1 0100 0073 2800  ....rv.......s(.
+00003010: 0000 0002 0201 0201 0201 0201 0201 0201  ................
+00003020: 0201 02f8 040b 0401 0401 0401 0401 0401  ................
+00003030: 0801 0401 04f8 040a 0a01 7a10 4275 696c  ..........z.Buil
+00003040: 6445 6e76 2e61 735f 6469 6374 6301 0000  dEnv.as_dictc...
+00003050: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003060: 0043 0000 0073 0800 0000 7400 a001 a100  .C...s....t.....
+00003070: 5300 7213 0000 0029 0272 6400 0000 72a7  S.r....).rd...r.
+00003080: 0000 0072 2500 0000 720c 0000 0072 0c00  ...r%...r....r..
+00003090: 0000 720d 0000 0072 a700 0000 b901 0000  ..r....r........
+000030a0: 7302 0000 0000 027a 1742 7569 6c64 456e  s......z.BuildEn
+000030b0: 762e 7079 7468 6f6e 5f76 6572 7369 6f6e  v.python_version
+000030c0: 2902 da0a 7079 7468 6f6e 5f6d 696e 7211  )...python_minr.
+000030d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000030e0: 0400 0000 0600 0000 4300 0000 732c 0000  ........C...s,..
+000030f0: 0074 006a 017d 0274 027c 026a 039b 0064  .t.j.}.t.|.j...d
+00003100: 017c 026a 049b 0064 017c 026a 059b 009d  .|.j...d.|.j....
+00003110: 0583 017d 037c 037c 016b 0453 0029 027a  ...}.|.|.k.S.).z
+00003120: 2244 6574 6563 7420 6966 2073 7973 7465  "Detect if syste
+00003130: 6d20 5079 7468 6f6e 2069 7320 746f 6f20  m Python is too 
+00003140: 6f6c 6472 1200 0000 2906 7261 0000 0072  oldr....).ra...r
+00003150: 6200 0000 720e 0000 0072 2600 0000 7228  b...r....r&...r(
+00003160: 0000 0072 2b00 0000 2904 721c 0000 0072  ...r+...).r....r
+00003170: aa00 0000 5a06 7379 735f 7079 5a0d 7379  ....Z.sys_pyZ.sy
+00003180: 7374 656d 5f70 7974 686f 6e72 0c00 0000  stem_pythonr....
+00003190: 720c 0000 0072 0d00 0000 da14 6973 5f63  r....r......is_c
+000031a0: 6f6d 7061 7469 626c 655f 7079 7468 6f6e  ompatible_python
+000031b0: bd01 0000 7306 0000 0000 0206 011e 017a  ....s..........z
+000031c0: 1d42 7569 6c64 456e 762e 6973 5f63 6f6d  .BuildEnv.is_com
+000031d0: 7061 7469 626c 655f 7079 7468 6f6e 6301  patible_pythonc.
+000031e0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000031f0: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
+00003200: 6401 6b06 5300 2902 4e29 03da 0577 696e  d.k.S.).N)...win
+00003210: 3332 da06 6379 6777 696e 5a04 6d73 7973  32..cygwinZ.msys
+00003220: a901 72a5 0000 0072 2500 0000 720c 0000  ..r....r%...r...
+00003230: 0072 0c00 0000 720d 0000 00da 0a69 735f  .r....r......is_
+00003240: 7769 6e64 6f77 73c3 0100 0073 0200 0000  windows....s....
+00003250: 0001 7a13 4275 696c 6445 6e76 2e69 735f  ..z.BuildEnv.is_
+00003260: 7769 6e64 6f77 7363 0100 0000 0000 0000  windowsc........
+00003270: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00003280: 730a 0000 007c 006a 0064 016b 0253 0029  s....|.j.d.k.S.)
+00003290: 024e 7252 0000 0072 ae00 0000 7225 0000  .NrR...r....r%..
+000032a0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000032b0: da08 6973 5f6d 6163 6f73 c601 0000 7302  ..is_macos....s.
+000032c0: 0000 0000 017a 1142 7569 6c64 456e 762e  .....z.BuildEnv.
+000032d0: 6973 5f6d 6163 6f73 6301 0000 0000 0000  is_macosc.......
+000032e0: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
+000032f0: 0073 4c00 0000 7400 6a01 7402 1900 6401  .sL...t.j.t...d.
+00003300: 9c01 6402 6403 8404 7d01 7400 6a01 7402  ..d.d...}.t.j.t.
+00003310: 1900 6401 9c01 6404 6405 8404 7d02 7c01  ..d...d.d...}.|.
+00003320: 8300 7d03 7c03 7338 7c02 8300 7d03 7c03  ..}.|.s8|...}.|.
+00003330: 7344 7403 6406 8301 8201 7404 7c03 8301  sDt.d.....t.|...
+00003340: 5300 2907 7a53 4669 6e64 2074 6865 2070  S.).zSFind the p
+00003350: 6174 6820 746f 2074 6865 2063 6d61 6b65  ath to the cmake
+00003360: 2064 6972 6563 746f 7279 2077 6974 6869   directory withi
+00003370: 6e20 610a 2020 2020 2020 2020 7069 7020  n a.        pip 
+00003380: 696e 7374 616c 6c65 6420 7079 746f 7263  installed pytorc
+00003390: 6820 7061 636b 6167 6572 1e00 0000 6300  h packager....c.
+000033a0: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+000033b0: 0000 0053 0000 0073 5e00 0000 7a42 6401  ...S...s^...zBd.
+000033c0: 6402 6c00 7d00 6403 6404 8400 7c00 6a01  d.l.}.d.d...|.j.
+000033d0: 4400 8301 7d01 7c01 4400 5d1e 7d02 7c02  D...}.|.D.].}.|.
+000033e0: 6405 1b00 7d03 7c03 a002 a100 721e 7c03  d...}.|.....r.|.
+000033f0: 0200 0100 5700 5300 711e 5700 6402 5300  ....W.S.q.W.d.S.
+00003400: 0400 7403 6b0a 7258 0100 0100 0100 5900  ..t.k.rX......Y.
+00003410: 6402 5300 5800 6402 5300 2906 7a1c 4669  d.S.X.d.S.).z.Fi
+00003420: 6e64 2074 6872 6f75 6768 2069 6d70 6f72  nd through impor
+00003430: 7469 6e67 2074 6f72 6368 7201 0000 004e  ting torchr....N
+00003440: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00003450: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
+00003460: 7c00 5d0c 7d01 7400 7c01 8301 9102 7104  |.].}.t.|.....q.
+00003470: 5300 720c 0000 0072 0200 0000 a902 7215  S.r....r......r.
+00003480: 0000 00da 0170 720c 0000 0072 0c00 0000  .....pr....r....
+00003490: 720d 0000 0072 7800 0000 d301 0000 7304  r....rx.......s.
+000034a0: 0000 0006 0002 007a 4942 7569 6c64 456e  .......zIBuildEn
+000034b0: 762e 746f 7263 685f 636d 616b 655f 7061  v.torch_cmake_pa
+000034c0: 7468 2e3c 6c6f 6361 6c73 3e2e 5f74 6f72  th.<locals>._tor
+000034d0: 6368 5f69 6d70 6f72 745f 7061 7468 2e3c  ch_import_path.<
+000034e0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000034f0: 703e 7a11 7368 6172 652f 636d 616b 652f  p>z.share/cmake/
+00003500: 546f 7263 6829 0472 4a00 0000 da08 5f5f  Torch).rJ.....__
+00003510: 7061 7468 5f5f da06 6973 5f64 6972 da13  path__..is_dir..
+00003520: 4d6f 6475 6c65 4e6f 7446 6f75 6e64 4572  ModuleNotFoundEr
+00003530: 726f 7229 0472 3700 0000 5a0b 746f 7263  ror).r7...Z.torc
+00003540: 685f 7061 7468 73da 055f 7061 7468 da0a  h_paths.._path..
+00003550: 746f 7263 685f 7061 7468 720c 0000 0072  torch_pathr....r
+00003560: 0c00 0000 720d 0000 00da 125f 746f 7263  ....r......_torc
+00003570: 685f 696d 706f 7274 5f70 6174 68ce 0100  h_import_path...
+00003580: 0073 1400 0000 0002 0201 0802 1001 0801  .s..............
+00003590: 0801 0801 0c01 0601 0e01 7a35 4275 696c  ..........z5Buil
+000035a0: 6445 6e76 2e74 6f72 6368 5f63 6d61 6b65  dEnv.torch_cmake
+000035b0: 5f70 6174 682e 3c6c 6f63 616c 733e 2e5f  _path.<locals>._
+000035c0: 746f 7263 685f 696d 706f 7274 5f70 6174  torch_import_pat
+000035d0: 6863 0000 0000 0000 0000 0000 0000 0300  hc..............
+000035e0: 0000 0400 0000 5300 0000 735c 0000 0064  ......S...s\...d
+000035f0: 0164 0284 0074 00a0 01a1 0044 0083 017d  .d...t.....D...}
+00003600: 0074 006a 0272 3674 0374 006a 0283 01a0  .t.j.r6t.t.j....
+00003610: 04a1 0072 367c 00a0 0574 0374 006a 0283  ...r6|...t.t.j..
+00003620: 01a1 0101 007c 0044 005d 1c7d 017c 0164  .....|.D.].}.|.d
+00003630: 031b 007d 027c 02a0 04a1 0072 3a7c 0202  ...}.|.....r:|..
+00003640: 0001 0053 0071 3a64 0453 0029 057a 2066  ...S.q:d.S.).z f
+00003650: 696e 6420 746f 7263 6820 7468 726f 7567  ind torch throug
+00003660: 6820 7369 7465 2070 6163 6b61 6765 7363  h site packagesc
+00003670: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003680: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00003690: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
+000036a0: 0072 0c00 0000 7202 0000 0072 b100 0000  .r....r....r....
+000036b0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000036c0: 7800 0000 de01 0000 7304 0000 0006 0002  x.......s.......
+000036d0: 007a 4742 7569 6c64 456e 762e 746f 7263  .zGBuildEnv.torc
+000036e0: 685f 636d 616b 655f 7061 7468 2e3c 6c6f  h_cmake_path.<lo
+000036f0: 6361 6c73 3e2e 5f74 6f72 6368 5f73 6974  cals>._torch_sit
+00003700: 655f 7061 7468 2e3c 6c6f 6361 6c73 3e2e  e_path.<locals>.
+00003710: 3c6c 6973 7463 6f6d 703e 7a17 746f 7263  <listcomp>z.torc
+00003720: 682f 7368 6172 652f 636d 616b 652f 546f  h/share/cmake/To
+00003730: 7263 684e 2906 da04 7369 7465 da0f 6765  rchN)...site..ge
+00003740: 7473 6974 6570 6163 6b61 6765 73da 0955  tsitepackages..U
+00003750: 5345 525f 5349 5445 7203 0000 0072 b400  SER_SITEr....r..
+00003760: 0000 7273 0000 0029 035a 0a73 6974 655f  ..rs...).Z.site_
+00003770: 7061 7468 7372 b600 0000 72b7 0000 0072  pathsr....r....r
+00003780: 0c00 0000 720c 0000 0072 0d00 0000 da10  ....r....r......
+00003790: 5f74 6f72 6368 5f73 6974 655f 7061 7468  _torch_site_path
+000037a0: dc01 0000 7310 0000 0000 0212 0314 0110  ....s...........
+000037b0: 0208 0108 0108 010a 017a 3342 7569 6c64  .........z3Build
+000037c0: 456e 762e 746f 7263 685f 636d 616b 655f  Env.torch_cmake_
+000037d0: 7061 7468 2e3c 6c6f 6361 6c73 3e2e 5f74  path.<locals>._t
+000037e0: 6f72 6368 5f73 6974 655f 7061 7468 7a21  orch_site_pathz!
+000037f0: 436f 756c 6420 6e6f 7420 6c6f 6361 7465  Could not locate
+00003800: 2074 6f72 6368 2063 6d61 6b65 2070 6174   torch cmake pat
+00003810: 6829 0572 3700 0000 da08 4f70 7469 6f6e  h).r7.....Option
+00003820: 616c 7203 0000 0072 0700 0000 7214 0000  alr....r....r...
+00003830: 0029 0472 1c00 0000 72b8 0000 0072 bc00  .).r....r....r..
+00003840: 0000 72b7 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00003850: 0072 0d00 0000 da10 746f 7263 685f 636d  .r......torch_cm
+00003860: 616b 655f 7061 7468 c901 0000 7310 0000  ake_path....s...
+00003870: 0000 0514 0e14 0e06 0104 0106 0104 0108  ................
+00003880: 017a 1942 7569 6c64 456e 762e 746f 7263  .z.BuildEnv.torc
+00003890: 685f 636d 616b 655f 7061 7468 6300 0000  h_cmake_pathc...
+000038a0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+000038b0: 0043 0000 0073 bc00 0000 7400 6a01 a002  .C...s....t.j...
+000038c0: 6401 6402 a102 7400 6a01 a002 6403 6402  d.d...t.j...d.d.
+000038d0: a102 7400 6a01 a002 6404 6402 a102 7400  ..t.j...d.d...t.
+000038e0: 6a01 a002 6405 6402 a102 6406 9c04 7d00  j...d.d...d...}.
+000038f0: 6401 6403 6702 7d01 6405 6404 6702 7d02  d.d.g.}.d.d.g.}.
+00003900: 7403 6407 6408 8400 7c01 4400 8301 8301  t.d.d...|.D.....
+00003910: 7d03 7403 6409 6408 8400 7c02 4400 8301  }.t.d.d...|.D...
+00003920: 8301 7d04 7c03 7376 7c04 7376 640a 5300  ..}.|.sv|.svd.S.
+00003930: 7c03 7298 7c04 7398 7c00 6403 1900 7c00  |.r.|.s.|.d...|.
+00003940: 6405 3c00 7c00 6401 1900 7c00 6404 3c00  d.<.|.d...|.d.<.
+00003950: 6e20 7c04 72b8 7c03 73b8 7c00 6405 1900  n |.r.|.s.|.d...
+00003960: 7c00 6403 3c00 7c00 6404 1900 7c00 6401  |.d.<.|.d...|.d.
+00003970: 3c00 7c00 5300 290b 612f 0100 0043 6f6c  <.|.S.).a/...Col
+00003980: 6c65 6374 2074 6865 2065 6e76 6972 6f6e  lect the environ
+00003990: 6d65 6e74 2076 6172 6961 626c 6573 206e  ment variables n
+000039a0: 6565 6465 6420 666f 7220 4361 6666 6520  eeded for Caffe 
+000039b0: 2850 7974 6f72 6368 290a 2020 2020 2020  (Pytorch).      
+000039c0: 2020 616e 6420 7468 726f 7720 616e 2065    and throw an e
+000039d0: 7272 6f72 2069 6620 7468 6579 2061 7265  rror if they are
+000039e0: 206e 6f74 2066 6f75 6e64 0a0a 2020 2020   not found..    
+000039f0: 2020 2020 5370 6563 6966 6963 616c 6c79      Specifically
+00003a00: 206d 616b 6520 7375 7265 2074 6f20 7365   make sure to se
+00003a10: 7420 6174 206c 6561 7374 206f 6e65 2073  t at least one s
+00003a20: 6574 206f 663a 0a20 2020 2020 2020 2020  et of:.         
+00003a30: 2020 202d 2043 5544 4e4e 5f4c 4942 5241     - CUDNN_LIBRA
+00003a40: 5259 2061 6e64 2043 5544 4e4e 5f49 4e43  RY and CUDNN_INC
+00003a50: 4c55 4445 5f44 4952 0a20 2020 2020 2020  LUDE_DIR.       
+00003a60: 2020 2020 2020 2020 206f 720a 2020 2020           or.    
+00003a70: 2020 2020 2020 2020 2d20 4355 444e 4e5f          - CUDNN_
+00003a80: 4c49 4252 4152 595f 5041 5448 2061 6e64  LIBRARY_PATH and
+00003a90: 2043 5544 4e4e 5f49 4e43 4c55 4445 5f50   CUDNN_INCLUDE_P
+00003aa0: 4154 480a 2020 2020 2020 2020 da0d 4355  ATH.        ..CU
+00003ab0: 444e 4e5f 4c49 4252 4152 597a 1165 6e76  DNN_LIBRARYz.env
+00003ac0: 2d76 6172 2d6e 6f74 2d66 6f75 6e64 da11  -var-not-found..
+00003ad0: 4355 444e 4e5f 494e 434c 5544 455f 4449  CUDNN_INCLUDE_DI
+00003ae0: 52da 1243 5544 4e4e 5f4c 4942 5241 5259  R..CUDNN_LIBRARY
+00003af0: 5f50 4154 48da 1243 5544 4e4e 5f49 4e43  _PATH..CUDNN_INC
+00003b00: 4c55 4445 5f50 4154 4829 0472 bf00 0000  LUDE_PATH).r....
+00003b10: 72c0 0000 0072 c100 0000 72c2 0000 0063  r....r....r....c
+00003b20: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003b30: 0400 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
+00003b40: 005d 0e7d 017c 0174 006a 016b 0691 0271  .].}.|.t.j.k...q
+00003b50: 0453 0072 0c00 0000 a902 7240 0000 0072  .S.r......r@...r
+00003b60: 4100 0000 a902 7215 0000 0072 3e00 0000  A.....r....r>...
+00003b70: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00003b80: 7800 0000 0402 0000 7304 0000 0006 0002  x.......s.......
+00003b90: 007a 2a42 7569 6c64 456e 762e 6765 745f  .z*BuildEnv.get_
+00003ba0: 6375 646e 6e5f 656e 762e 3c6c 6f63 616c  cudnn_env.<local
+00003bb0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00003bc0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00003bd0: 0000 5300 0000 7316 0000 0067 007c 005d  ..S...s....g.|.]
+00003be0: 0e7d 017c 0174 006a 016b 0691 0271 0453  .}.|.t.j.k...q.S
+00003bf0: 0072 0c00 0000 72c3 0000 0072 c400 0000  .r....r....r....
+00003c00: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00003c10: 7800 0000 0502 0000 7304 0000 0006 0002  x.......s.......
+00003c20: 004e 2904 7240 0000 0072 4100 0000 7242  .N).r@...rA...rB
+00003c30: 0000 00da 0361 6c6c 2905 72a2 0000 005a  .....all).r....Z
+00003c40: 1074 6f72 6368 5f63 7564 6e6e 5f76 6172  .torch_cudnn_var
+00003c50: 735a 1063 6166 6665 5f63 7564 6e6e 5f76  sZ.caffe_cudnn_v
+00003c60: 6172 735a 0974 6f72 6368 5f73 6574 5a09  arsZ.torch_setZ.
+00003c70: 6361 6666 655f 7365 7472 0c00 0000 720c  caffe_setr....r.
+00003c80: 0000 0072 0d00 0000 da0d 6765 745f 6375  ...r......get_cu
+00003c90: 646e 6e5f 656e 76f1 0100 0073 2400 0000  dnn_env....s$...
+00003ca0: 000b 0c01 0c01 0c01 0cfc 0606 0801 0802  ................
+00003cb0: 1201 1204 0801 0401 0801 0c01 0e01 0801  ................
+00003cc0: 0c01 0c01 7a16 4275 696c 6445 6e76 2e67  ....z.BuildEnv.g
+00003cd0: 6574 5f63 7564 6e6e 5f65 6e76 2902 da07  et_cudnn_env)...
+00003ce0: 636f 6d6d 616e 6472 1100 0000 6302 0000  commandr....c...
+00003cf0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+00003d00: 0043 0000 0073 4600 0000 7a1c 7400 6a01  .C...sF...z.t.j.
+00003d10: 7c01 6401 6702 7400 6a02 7400 6a02 6402  |.d.g.t.j.t.j.d.
+00003d20: 8d03 0100 5700 6e24 0400 7403 6b0a 7240  ....W.n$..t.k.r@
+00003d30: 0100 0100 0100 7404 7c01 9b00 6403 9d02  ......t.|...d...
+00003d40: 8301 6400 8202 5900 6e02 5800 6400 5300  ..d...Y.n.X.d.S.
+00003d50: 2904 4e7a 092d 2d76 6572 7369 6f6e 2902  ).Nz.--version).
+00003d60: da06 7374 646f 7574 da06 7374 6465 7272  ..stdout..stderr
+00003d70: 7a24 206d 7573 7420 6265 2069 6e73 7461  z$ must be insta
+00003d80: 6c6c 6564 2074 6f20 6275 696c 6420 536d  lled to build Sm
+00003d90: 6172 7453 696d 2905 7281 0000 00da 0a63  artSim).r......c
+00003da0: 6865 636b 5f63 616c 6cda 0744 4556 4e55  heck_call..DEVNU
+00003db0: 4c4c da07 4f53 4572 726f 7272 0700 0000  LL..OSErrorr....
+00003dc0: 2902 721c 0000 0072 c700 0000 720c 0000  ).r....r....r...
+00003dd0: 0072 0c00 0000 720d 0000 0072 9e00 0000  .r....r....r....
+00003de0: 1302 0000 7310 0000 0000 0202 0104 0106  ....s...........
+00003df0: 0104 0104 fd0a 050e 017a 1f42 7569 6c64  .........z.Build
+00003e00: 456e 762e 6368 6563 6b5f 6275 696c 645f  Env.check_build_
+00003e10: 6465 7065 6e64 656e 6379 2903 da07 7061  dependency)...pa
+00003e20: 636b 6167 6572 3900 0000 7211 0000 0063  ckager9...r....c
+00003e30: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00003e40: 0900 0000 4300 0000 7380 0000 007a 6274  ....C...s....zbt
+00003e50: 0074 01a0 027c 00a1 016a 0383 017d 027c  .t...|...j...}.|
+00003e60: 0172 5e7c 026a 047c 016a 046b 0373 2e7c  .r^|.j.|.j.k.s.|
+00003e70: 026a 057c 016a 056b 0372 5e64 017c 009b  .j.|.j.k.r^d.|..
+00003e80: 0064 029d 037c 009b 0064 037c 019b 0064  .d...|...d.|...d
+00003e90: 047c 009b 0064 037c 029b 0064 059d 0817  .|...d.|...d....
+00003ea0: 007d 0374 067c 0383 0182 0157 0064 0653  .}.t.|.....W.d.S
+00003eb0: 0004 0074 016a 076b 0a72 7a01 0001 0001  ...t.j.k.rz.....
+00003ec0: 0059 0064 0753 0058 0064 0853 0029 097a  .Y.d.S.X.d.S.).z
+00003ed0: 7f43 6865 636b 2069 6620 6120 7061 636b  .Check if a pack
+00003ee0: 6167 6520 6973 2069 6e73 7461 6c6c 6564  age is installed
+00003ef0: 2e20 4966 2076 6572 7369 6f6e 2069 7320  . If version is 
+00003f00: 7072 6f76 6964 6564 2c20 6368 6563 6b20  provided, check 
+00003f10: 6966 0a20 2020 2020 2020 2069 7427 7320  if.        it's 
+00003f20: 6120 636f 6d70 6174 6962 6c65 2076 6572  a compatible ver
+00003f30: 7369 6f6e 2e20 286d 616a 6f72 2061 6e64  sion. (major and
+00003f40: 206d 696e 6f72 2074 6865 2073 616d 6529   minor the same)
+00003f50: 7a19 496e 636f 6d70 6174 6962 6c65 2076  z.Incompatible v
+00003f60: 6572 7369 6f6e 2066 6f72 207a 0b20 6465  ersion for z. de
+00003f70: 7465 6374 6564 2e0a fa01 207a 0f20 7265  tected.... z. re
+00003f80: 7175 6573 7465 6420 6275 7420 7a0b 2069  quested but z. i
+00003f90: 6e73 7461 6c6c 6564 2e54 464e 2908 720e  nstalled.TFN).r.
+00003fa0: 0000 0072 2100 0000 da10 6765 745f 6469  ...r!.....get_di
+00003fb0: 7374 7269 6275 7469 6f6e 7239 0000 0072  stributionr9...r
+00003fc0: 2600 0000 7228 0000 0072 0700 0000 da14  &...r(...r......
+00003fd0: 4469 7374 7269 6275 7469 6f6e 4e6f 7446  DistributionNotF
+00003fe0: 6f75 6e64 2904 72cd 0000 0072 3900 0000  ound).r....r9...
+00003ff0: 5a09 696e 7374 616c 6c65 64da 036d 7367  Z.installed..msg
+00004000: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00004010: 0f63 6865 636b 5f69 6e73 7461 6c6c 6564  .check_installed
+00004020: 1e02 0000 7318 0000 0000 0402 0110 0104  ....s...........
+00004030: 0218 020a 011a ff02 ff02 0408 0106 0110  ................
+00004040: 017a 1842 7569 6c64 456e 762e 6368 6563  .z.BuildEnv.chec
+00004050: 6b5f 696e 7374 616c 6c65 6429 0154 2901  k_installed).T).
+00004060: 4e29 2872 0800 0000 7209 0000 0072 0a00  N)(r....r....r..
+00004070: 0000 720b 0000 0072 4000 0000 7241 0000  ..r....r@...rA..
+00004080: 0072 4200 0000 7294 0000 0072 9500 0000  .rB...r....r....
+00004090: 7296 0000 0072 9700 0000 7298 0000 0072  r....r....r....r
+000040a0: 2000 0000 72a4 0000 0072 9d00 0000 7261   ...r....r....ra
+000040b0: 0000 0072 6400 0000 72a5 0000 0072 3c00  ...rd...r....r<.
+000040c0: 0000 7258 0000 0072 9b00 0000 7237 0000  ..rX...r....r7..
+000040d0: 0072 6500 0000 7214 0000 0072 a300 0000  .re...r....r....
+000040e0: 7292 0000 0072 7600 0000 723b 0000 0072  r....rv...r;...r
+000040f0: a700 0000 da05 666c 6f61 7472 ab00 0000  ......floatr....
+00004100: 72af 0000 0072 b000 0000 72bd 0000 0072  r....r....r....r
+00004110: be00 0000 da0c 7374 6174 6963 6d65 7468  ......staticmeth
+00004120: 6f64 72c6 0000 0072 9e00 0000 720e 0000  odr....r....r...
+00004130: 0072 d200 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00004140: 720c 0000 0072 0d00 0000 7293 0000 006a  r....r....r....j
+00004150: 0100 0073 3200 0000 0801 0412 0e01 0e01  ...s2...........
+00004160: 0e01 0e03 0e01 1203 1201 0602 1204 0e06  ................
+00004170: 180d 1e18 0201 1003 1006 0e03 0e03 0201  ................
+00004180: 1627 0201 2021 100b 0201 7293 0000 0029  .'.. !....r....)
+00004190: 1972 4000 0000 7264 0000 0072 b900 0000  .r@...rd...r....
+000041a0: 7281 0000 0072 6100 0000 da06 7479 7069  r....ra.....typi
+000041b0: 6e67 7237 0000 00da 0770 6174 686c 6962  ngr7.....pathlib
+000041c0: 7203 0000 0072 0400 0000 7221 0000 0072  r....r....r!...r
+000041d0: 0500 0000 7239 0000 0072 1900 0000 721b  ....r9...r....r.
+000041e0: 0000 00da 074c 6974 6572 616c 7291 0000  .....Literalr...
+000041f0: 0072 8600 0000 7207 0000 0072 1400 0000  .r....r....r....
+00004200: 720e 0000 0072 4300 0000 7244 0000 0072  r....rC...rD...r
+00004210: 6600 0000 7293 0000 0072 0c00 0000 720c  f...r....r....r.
+00004220: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+00004230: 6d6f 6475 6c65 3e1b 0000 0073 2600 0000  module>....s&...
+00004240: 0801 0801 0801 0801 0801 0801 0c01 0c02  ................
+00004250: 0801 0c02 0801 0801 0a06 1012 1041 1204  .............A..
+00004260: 1056 0e7f 000f                           .V....
```

### Comparing `smartsim-0.4.2/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc` & `smartsim-0.5.0/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 12 20:48:40 2023 UTC, .py size: 18635 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,757 +1,812 @@
-00000000: 550d 0d0a 0000 0000 2819 3764 cb48 0000  U.......(.7d.H..
+00000000: 550d 0d0a 0000 0000 405c a764 704c 0000  U.......@\.dpL..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c02  d.l.m.Z...d.d.l.
-00000070: 6d08 5a08 0100 6400 6404 6c04 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6405 6406 8400 5a0a 4700 6407 6408  ..d.d...Z.G.d.d.
-00000090: 8400 6408 650b 8303 5a0c 4700 6409 640a  ..d.e...Z.G.d.d.
-000000a0: 8400 640a 8302 5a0d 4700 640b 640c 8400  ..d...Z.G.d.d...
-000000b0: 640c 650d 8303 5a0e 4700 640d 640e 8400  d.e...Z.G.d.d...
-000000c0: 640e 650d 8303 5a0f 6401 5300 290f e900  d.e...Z.d.S.)...
-000000d0: 0000 004e 2901 da04 5061 7468 2901 da05  ...N)...Path)...
-000000e0: 7768 6963 6829 01da 0f53 7562 7072 6f63  which)...Subproc
-000000f0: 6573 7345 7272 6f72 6301 0000 0000 0000  essErrorc.......
-00000100: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000110: 0073 7600 0000 7400 7c00 8301 7d01 7c01  .sv...t.|...}.|.
-00000120: 736a 7401 6a02 a003 7c00 a101 7232 7401  sjt.j...|...r2t.
-00000130: a004 7c00 7401 6a05 a102 7232 7401 6a02  ..|.t.j...r2t.j.
-00000140: a006 7c00 a101 5300 7401 6a02 a003 7c00  ..|...S.t.j...|.
-00000150: a101 725c 7401 a004 7c00 7401 6a05 a102  ..r\t...|.t.j...
-00000160: 735c 7407 6401 7c00 9b00 6402 9d03 8301  s\t.d.|...d.....
-00000170: 8201 7408 6403 7c00 9b00 9d02 8301 8201  ..t.d.|.........
-00000180: 7401 6a02 a006 7c01 a101 5300 2904 7aed  t.j...|...S.).z.
-00000190: 5461 6b65 7320 616e 2065 7865 6375 7461  Takes an executa
-000001a0: 626c 6520 616e 6420 7265 7475 726e 7320  ble and returns 
-000001b0: 7468 6520 6675 6c6c 2070 6174 6820 746f  the full path to
-000001c0: 2074 6861 7420 6578 6563 7574 6162 6c65   that executable
-000001d0: 0a0a 2020 2020 3a70 6172 616d 2065 7865  ..    :param exe
-000001e0: 3a20 6578 6563 7574 6162 6c65 206f 7220  : executable or 
-000001f0: 6669 6c65 0a20 2020 203a 7479 7065 2065  file.    :type e
-00000200: 7865 3a20 7374 720a 2020 2020 3a72 6169  xe: str.    :rai
-00000210: 7365 7320 5479 7065 4572 726f 723a 2069  ses TypeError: i
-00000220: 6620 6669 6c65 2069 7320 6e6f 7420 616e  f file is not an
-00000230: 2065 7865 6375 7461 626c 650a 2020 2020   executable.    
-00000240: 3a72 6169 7365 7320 4669 6c65 4e6f 7446  :raises FileNotF
-00000250: 6f75 6e64 4572 726f 723a 2069 6620 6578  oundError: if ex
-00000260: 6563 7574 6162 6c65 2063 616e 6e6f 7420  ecutable cannot 
-00000270: 6265 2066 6f75 6e64 0a20 2020 207a 0646  be found.    z.F
-00000280: 696c 652c 207a 162c 2069 7320 6e6f 7420  ile, z., is not 
-00000290: 616e 2065 7865 6375 7461 626c 657a 1c43  an executablez.C
-000002a0: 6f75 6c64 206e 6f74 206c 6f63 6174 6520  ould not locate 
-000002b0: 6578 6563 7574 6162 6c65 2029 0972 0300  executable ).r..
-000002c0: 0000 da02 6f73 da04 7061 7468 da06 6973  ....os..path..is
-000002d0: 6669 6c65 da06 6163 6365 7373 da04 585f  file..access..X_
-000002e0: 4f4b da07 6162 7370 6174 68da 0954 7970  OK..abspath..Typ
-000002f0: 6545 7272 6f72 da11 4669 6c65 4e6f 7446  eError..FileNotF
-00000300: 6f75 6e64 4572 726f 7229 025a 0365 7865  oundError).Z.exe
-00000310: 5a07 696e 5f70 6174 68a9 0072 0d00 0000  Z.in_path..r....
-00000320: fa46 2f68 6f6d 652f 7275 6e6e 6572 2f77  .F/home/runner/w
-00000330: 6f72 6b2f 536d 6172 7453 696d 2f53 6d61  ork/SmartSim/Sma
-00000340: 7274 5369 6d2f 736d 6172 7473 696d 2f5f  rtSim/smartsim/_
-00000350: 636f 7265 2f5f 696e 7374 616c 6c2f 6275  core/_install/bu
-00000360: 696c 6465 722e 7079 da0f 6578 7061 6e64  ilder.py..expand
-00000370: 5f65 7865 5f70 6174 682d 0000 0073 1000  _exe_path-...s..
-00000380: 0000 000a 0801 0401 1a01 0c01 1a01 1001  ................
-00000390: 0e01 720f 0000 0063 0000 0000 0000 0000  ..r....c........
-000003a0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000003b0: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
-000003c0: 0029 02da 0a42 7569 6c64 4572 726f 724e  .)...BuildErrorN
-000003d0: 2903 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000003e0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000003f0: 6e61 6d65 5f5f 720d 0000 0072 0d00 0000  name__r....r....
-00000400: 720d 0000 0072 0e00 0000 7210 0000 0041  r....r....r....A
-00000410: 0000 0073 0200 0000 0801 7210 0000 0063  ...s......r....c
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0400 0000 4000 0000 7372 0000 0065 005a  ....@...sr...e.Z
-00000440: 0164 005a 0264 015a 0365 04a0 0564 0265  .d.Z.d.Z.e...d.e
-00000450: 046a 06a1 025a 0764 1864 0564 0684 015a  .j...Z.d.d.d...Z
-00000460: 0865 0964 0764 0884 0083 015a 0a64 0964  .e.d.d.....Z.d.d
-00000470: 0a84 005a 0b64 0b64 0c84 005a 0c64 1964  ...Z.d.d...Z.d.d
-00000480: 0d64 0e84 015a 0d64 1a64 0f64 1084 015a  .d...Z.d.d.d...Z
-00000490: 0e64 1164 1284 005a 0f64 1364 1484 005a  .d.d...Z.d.d...Z
-000004a0: 1064 1b64 1664 1784 015a 1164 1553 0029  .d.d.d...Z.d.S.)
-000004b0: 1cda 0742 7569 6c64 6572 7a2d 4261 7365  ...Builderz-Base
-000004c0: 2063 6c61 7373 2066 6f72 2062 7569 6c64   class for build
-000004d0: 696e 6720 7468 6972 642d 7061 7274 7920  ing third-party 
-000004e0: 6c69 6272 6172 6965 737a a85e 283f 3a68  librariesz.^(?:h
-000004f0: 7474 707c 6674 7029 733f 3a2f 2f28 3f3a  ttp|ftp)s?://(?:
-00000500: 283f 3a5b 412d 5a30 2d39 5d28 3f3a 5b41  (?:[A-Z0-9](?:[A
-00000510: 2d5a 302d 392d 5d7b 302c 3631 7d5b 412d  -Z0-9-]{0,61}[A-
-00000520: 5a30 2d39 5d29 3f5c 2e29 2b28 3f3a 5b41  Z0-9])?\.)+(?:[A
-00000530: 2d5a 5d7b 322c 367d 5c2e 3f7c 5b41 2d5a  -Z]{2,6}\.?|[A-Z
-00000540: 302d 392d 5d7b 322c 7d5c 2e3f 297c 6c6f  0-9-]{2,}\.?)|lo
-00000550: 6361 6c68 6f73 747c 5c64 7b31 2c33 7d5c  calhost|\d{1,3}\
-00000560: 2e5c 647b 312c 337d 5c2e 5c64 7b31 2c33  .\d{1,3}\.\d{1,3
-00000570: 7d5c 2e5c 647b 312c 337d 2928 3f3a 3a5c  }\.\d{1,3})(?::\
-00000580: 642b 293f 283f 3a2f 3f7c 5b2f 3f5d 5c53  d+)?(?:/?|[/?]\S
-00000590: 2b29 24e9 0100 0000 4663 0400 0000 0000  +)$.....Fc......
-000005a0: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
-000005b0: 0000 73bc 0000 007c 017c 005f 0074 0174  ..s....|.|._.t.t
-000005c0: 026a 03a0 0474 05a1 0183 016a 066a 067d  .j...t.....j.j.}
-000005d0: 047c 047d 0574 02a0 0764 01a1 0172 3674  .|.}.t...d...r6t
-000005e0: 0174 026a 0864 0119 0083 017d 057c 0464  .t.j.d.....}.|.d
-000005f0: 021b 007c 005f 097c 0564 031b 007c 005f  ...|._.|.d...|._
-00000600: 0a7c 0564 041b 007c 005f 0b74 0c6a 0d7c  .|.d...|._.t.j.|
-00000610: 005f 0e7c 037c 005f 0f7c 006a 0f72 6e64  ._.|.|._.|.j.rnd
-00000620: 007c 005f 0e7c 006a 09a0 10a1 0073 827c  .|._.|.j.....s.|
-00000630: 006a 09a0 11a1 0001 007c 057c 046b 0272  .j.......|.|.k.r
-00000640: b27c 006a 0aa0 10a1 0073 9e7c 006a 0aa0  .|.j.....s.|.j..
-00000650: 11a1 0001 007c 006a 0ba0 10a1 0073 b27c  .....|.j.....s.|
-00000660: 006a 0ba0 11a1 0001 007c 027c 005f 1264  .j.......|.|._.d
-00000670: 0053 0029 054e 5a11 534d 4152 5453 494d  .S.).NZ.SMARTSIM
-00000680: 5f44 4550 5f50 4154 487a 0c2e 7468 6972  _DEP_PATHz..thir
-00000690: 642d 7061 7274 79da 0362 696e da03 6c69  d-party..bin..li
-000006a0: 6229 13da 0365 6e76 7202 0000 0072 0500  b)...envr....r..
-000006b0: 0000 7206 0000 0072 0a00 0000 da08 5f5f  ..r....r......__
-000006c0: 6669 6c65 5f5f da06 7061 7265 6e74 da06  file__..parent..
-000006d0: 6765 7465 6e76 da07 656e 7669 726f 6eda  getenv..environ.
-000006e0: 0962 7569 6c64 5f64 6972 da08 6269 6e5f  .build_dir..bin_
-000006f0: 7061 7468 da08 6c69 625f 7061 7468 da0a  path..lib_path..
-00000700: 7375 6270 726f 6365 7373 da07 4445 564e  subprocess..DEVN
-00000710: 554c 4cda 036f 7574 da07 7665 7262 6f73  ULL..out..verbos
-00000720: 65da 0669 735f 6469 72da 056d 6b64 6972  e..is_dir..mkdir
-00000730: da04 6a6f 6273 2906 da04 7365 6c66 7218  ..jobs)...selfr.
-00000740: 0000 0072 2600 0000 7223 0000 005a 095f  ...r&...r#...Z._
-00000750: 636f 7265 5f64 6972 da0f 6465 7065 6e64  core_dir..depend
-00000760: 656e 6379 5f70 6174 6872 0d00 0000 720d  ency_pathr....r.
-00000770: 0000 0072 0e00 0000 da08 5f5f 696e 6974  ...r......__init
-00000780: 5f5f 5200 0000 7328 0000 0000 0306 0314  __R...s(........
-00000790: 0204 010a 010e 020a 020a 010a 0308 0106  ................
-000007a0: 0106 0106 030a 010a 0108 010a 010a 010a  ................
-000007b0: 010a 027a 1042 7569 6c64 6572 2e5f 5f69  ...z.Builder.__i
-000007c0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-000007d0: 0000 0100 0000 0100 0000 4300 0000 7308  ..........C...s.
-000007e0: 0000 0074 0082 0164 0053 00a9 014e a901  ...t...d.S...N..
-000007f0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-00000800: 4572 726f 72a9 0172 2700 0000 720d 0000  Error..r'...r...
-00000810: 0072 0d00 0000 720e 0000 00da 0869 735f  .r....r......is_
-00000820: 6275 696c 7475 0000 0073 0200 0000 0002  builtu...s......
-00000830: 7a10 4275 696c 6465 722e 6973 5f62 7569  z.Builder.is_bui
-00000840: 6c74 6301 0000 0000 0000 0000 0000 0001  ltc.............
-00000850: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
-00000860: 7400 8201 6400 5300 722a 0000 0072 2b00  t...d.S.r*...r+.
-00000870: 0000 722d 0000 0072 0d00 0000 720d 0000  ..r-...r....r...
-00000880: 0072 0e00 0000 da0e 6275 696c 645f 6672  .r......build_fr
-00000890: 6f6d 5f67 6974 7900 0000 7302 0000 0000  om_gity...s.....
-000008a0: 017a 1642 7569 6c64 6572 2e62 7569 6c64  .z.Builder.build
-000008b0: 5f66 726f 6d5f 6769 7463 0200 0000 0000  _from_gitc......
-000008c0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-000008d0: 0000 7324 0000 0074 00a0 017c 01a1 017d  ..s$...t...|...}
-000008e0: 027c 0272 127c 0253 0074 027c 019b 0064  .|.r.|.S.t.|...d
-000008f0: 019d 0283 0182 0164 0053 0029 024e 7a12  .......d.S.).Nz.
-00000900: 206e 6f74 2066 6f75 6e64 2069 6e20 5041   not found in PA
-00000910: 5448 2903 da06 7368 7574 696c 7203 0000  TH)...shutilr...
-00000920: 0072 1000 0000 2903 7227 0000 00da 0662  .r....).r'.....b
-00000930: 696e 6172 795a 0762 696e 6172 795f 720d  inaryZ.binary_r.
-00000940: 0000 0072 0d00 0000 720e 0000 00da 0b62  ...r....r......b
-00000950: 696e 6172 795f 7061 7468 7c00 0000 7308  inary_path|...s.
-00000960: 0000 0000 010a 0104 0104 017a 1342 7569  ...........z.Bui
-00000970: 6c64 6572 2e62 696e 6172 795f 7061 7468  lder.binary_path
-00000980: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00000990: 0004 0000 0043 0000 0073 3000 0000 7400  .....C...s0...t.
-000009a0: a001 7c01 7c02 a102 0100 7c03 722c 7402  ..|.|.....|.r,t.
-000009b0: 7c02 8301 a003 7404 6a05 7404 6a06 4200  |.....t.j.t.j.B.
-000009c0: 7404 6a07 4200 a101 0100 6400 5300 722a  t.j.B.....d.S.r*
-000009d0: 0000 0029 0872 3000 0000 da08 636f 7079  ...).r0.....copy
-000009e0: 6669 6c65 7202 0000 00da 0563 686d 6f64  filer......chmod
-000009f0: da04 7374 6174 da07 535f 4958 5553 52da  ..stat..S_IXUSR.
-00000a00: 0753 5f49 5755 5352 da07 535f 4952 5553  .S_IWUSR..S_IRUS
-00000a10: 5229 0472 2700 0000 da03 7372 63da 0364  R).r'.....src..d
-00000a20: 7374 da07 7365 745f 6578 6572 0d00 0000  st..set_exer....
-00000a30: 720d 0000 0072 0e00 0000 da09 636f 7079  r....r......copy
-00000a40: 5f66 696c 6582 0000 0073 0600 0000 0001  _file....s......
-00000a50: 0c01 0401 7a11 4275 696c 6465 722e 636f  ....z.Builder.co
-00000a60: 7079 5f66 696c 6563 0400 0000 0000 0000  py_filec........
-00000a70: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
-00000a80: 7366 0000 0074 007c 0183 017d 0174 007c  sf...t.|...}.t.|
-00000a90: 0283 017d 027c 026a 0164 0164 028d 0101  ...}.|.j.d.d....
-00000aa0: 007c 01a0 0264 03a1 0144 005d 3a7d 047c  .|...d...D.]:}.|
-00000ab0: 04a0 03a1 0072 4a7c 006a 047c 047c 027c  .....rJ|.j.|.|.|
-00000ac0: 046a 051b 007c 0364 048d 0301 0071 267c  .j...|.d.....q&|
-00000ad0: 006a 067c 047c 027c 046a 051b 007c 0364  .j.|.|.|.j...|.d
-00000ae0: 048d 0301 0071 2664 0053 0029 054e 5429  .....q&d.S.).NT)
-00000af0: 01da 0865 7869 7374 5f6f 6bda 012a a901  ...exist_ok..*..
-00000b00: 723b 0000 0029 0772 0200 0000 7225 0000  r;...).r....r%..
-00000b10: 00da 0467 6c6f 6272 2400 0000 da08 636f  ...globr$.....co
-00000b20: 7079 5f64 6972 da04 6e61 6d65 723c 0000  py_dir..namer<..
-00000b30: 0029 0572 2700 0000 7239 0000 0072 3a00  .).r'...r9...r:.
-00000b40: 0000 723b 0000 00da 0763 6f6e 7465 6e74  ..r;.....content
-00000b50: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000b60: 4100 0000 8700 0000 730e 0000 0000 0108  A.......s.......
-00000b70: 0108 010c 020e 0108 0118 027a 1042 7569  ...........z.Bui
-00000b80: 6c64 6572 2e63 6f70 795f 6469 7263 0200  lder.copy_dirc..
-00000b90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000ba0: 0000 4300 0000 7312 0000 0074 00a0 017c  ..C...s....t...|
-00000bb0: 006a 027c 01a1 0264 006b 0953 0072 2a00  .j.|...d.k.S.r*.
-00000bc0: 0000 2903 da02 7265 da05 6d61 7463 68da  ..)...re..match.
-00000bd0: 0975 726c 5f72 6567 6578 2902 7227 0000  .url_regex).r'..
-00000be0: 00da 0375 726c 720d 0000 0072 0d00 0000  ...urlr....r....
-00000bf0: 720e 0000 00da 0c69 735f 7661 6c69 645f  r......is_valid_
-00000c00: 7572 6c92 0000 0073 0200 0000 0001 7a14  url....s......z.
-00000c10: 4275 696c 6465 722e 6973 5f76 616c 6964  Builder.is_valid
-00000c20: 5f75 726c 6301 0000 0000 0000 0000 0000  _urlc...........
-00000c30: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-00000c40: 0000 7c00 6a00 a001 a100 721a 7402 a003  ..|.j.....r.t...
-00000c50: 7404 7c00 6a00 8301 a101 0100 6400 5300  t.|.j.......d.S.
-00000c60: 722a 0000 0029 0572 1d00 0000 7224 0000  r*...).r....r$..
-00000c70: 0072 3000 0000 da06 726d 7472 6565 da03  .r0.....rmtree..
-00000c80: 7374 7272 2d00 0000 720d 0000 0072 0d00  strr-...r....r..
-00000c90: 0000 720e 0000 00da 0763 6c65 616e 7570  ..r......cleanup
-00000ca0: 9500 0000 7304 0000 0000 010a 017a 0f42  ....s........z.B
-00000cb0: 7569 6c64 6572 2e63 6c65 616e 7570 4e63  uilder.cleanupNc
-00000cc0: 0500 0000 0000 0000 0000 0000 0800 0000  ................
-00000cd0: 0a00 0000 4300 0000 7380 0000 007c 0373  ....C...s....|.s
-00000ce0: 0a7c 006a 007d 037a 4274 016a 027c 0174  .|.j.}.zBt.j.|.t
-00000cf0: 016a 037c 037c 047c 027c 006a 0464 018d  .j.|.|.|.|.j.d..
-00000d00: 067d 057c 05a0 05a1 0064 0219 00a0 0664  .}.|.....d.....d
-00000d10: 03a1 017d 067c 056a 0764 046b 0372 4a74  ...}.|.j.d.k.rJt
-00000d20: 087c 0683 0182 0157 006e 2e04 0074 0974  .|.....W.n...t.t
-00000d30: 0a66 026b 0a72 7a01 007d 0701 007a 0c74  .f.k.rz..}...z.t
-00000d40: 087c 0783 0182 0157 0035 0064 007d 077e  .|.....W.5.d.}.~
-00000d50: 0758 0059 006e 0258 0064 0053 0029 054e  .X.Y.n.X.d.S.).N
-00000d60: 2905 da06 7374 6465 7272 da06 7374 646f  )...stderr..stdo
-00000d70: 7574 da03 6377 64da 0573 6865 6c6c 7218  ut..cwd..shellr.
-00000d80: 0000 0072 1500 0000 7a05 7574 662d 3872  ...r....z.utf-8r
-00000d90: 0100 0000 290b 7222 0000 0072 2000 0000  ....).r"...r ...
-00000da0: da05 506f 7065 6eda 0450 4950 4572 1800  ..Popen..PIPEr..
-00000db0: 0000 da0b 636f 6d6d 756e 6963 6174 65da  ....communicate.
-00000dc0: 0664 6563 6f64 65da 0a72 6574 7572 6e63  .decode..returnc
-00000dd0: 6f64 6572 1000 0000 da07 4f53 4572 726f  oder......OSErro
-00000de0: 7272 0400 0000 2908 7227 0000 00da 0363  rr....).r'.....c
-00000df0: 6d64 724f 0000 0072 2200 0000 724e 0000  mdrO...r"...rN..
-00000e00: 00da 0470 726f 63da 0565 7272 6f72 da01  ...proc..error..
-00000e10: 6572 0d00 0000 720d 0000 0072 0e00 0000  er....r....r....
-00000e20: da0b 7275 6e5f 636f 6d6d 616e 6499 0000  ..run_command...
-00000e30: 0073 2000 0000 0002 0401 0601 0201 0401  .s .............
-00000e40: 0201 0401 0201 0201 0201 04fa 0608 1201  ................
-00000e50: 0a01 0c01 1401 7a13 4275 696c 6465 722e  ......z.Builder.
-00000e60: 7275 6e5f 636f 6d6d 616e 6429 0272 1500  run_command).r..
-00000e70: 0000 4629 0146 2901 4629 0346 4e4e 2912  ..F).F).F).FNN).
-00000e80: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000e90: 075f 5f64 6f63 5f5f 7244 0000 00da 0763  .__doc__rD.....c
-00000ea0: 6f6d 7069 6c65 da0a 4947 4e4f 5245 4341  ompile..IGNORECA
-00000eb0: 5345 7246 0000 0072 2900 0000 da08 7072  SErF...r).....pr
-00000ec0: 6f70 6572 7479 722e 0000 0072 2f00 0000  opertyr....r/...
-00000ed0: 7232 0000 0072 3c00 0000 7241 0000 0072  r2...r<...rA...r
-00000ee0: 4800 0000 724b 0000 0072 5a00 0000 720d  H...rK...rZ...r.
-00000ef0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000f00: 0000 7214 0000 0045 0000 0073 1e00 0000  ..r....E...s....
-00000f10: 0801 0402 0401 0206 04f9 040a 0a23 0201  .............#..
-00000f20: 0a03 0803 0806 0a05 0a0b 0803 0804 7214  ..............r.
-00000f30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000f40: 0000 0000 0400 0000 0000 0000 733e 0000  ............s>..
-00000f50: 0065 005a 0164 005a 0264 015a 0369 0064  .e.Z.d.Z.d.Z.i.d
-00000f60: 0264 0364 0466 0487 0066 0164 0564 0684  .d.d.f...f.d.d..
-00000f70: 095a 0465 0564 0764 0884 0083 015a 0664  .Z.e.d.d.....Z.d
-00000f80: 0964 0a84 005a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
-00000f90: 0bda 0f44 6174 6162 6173 6542 7569 6c64  ...DatabaseBuild
-00000fa0: 6572 7aaf 436c 6173 7320 746f 2062 7569  erz.Class to bui
-00000fb0: 6c64 2052 6564 6973 206f 7220 4b65 7944  ld Redis or KeyD
-00000fc0: 4220 6672 6f6d 2053 6f75 7263 650a 2020  B from Source.  
-00000fd0: 2020 5375 7070 6f72 7465 6420 6275 696c    Supported buil
-00000fe0: 6420 6d65 7468 6f64 733a 0a20 2020 2020  d methods:.     
-00000ff0: 2d20 6672 6f6d 2067 6974 0a20 2020 2053  - from git.    S
-00001000: 6565 2062 7569 6c64 656e 762e 7079 2066  ee buildenv.py f
-00001010: 6f72 2062 7569 6c64 7469 6d65 2063 6f6e  or buildtime con
-00001020: 6669 6775 7261 7469 6f6e 206f 6620 5265  figuration of Re
-00001030: 6469 732f 4b65 7944 420a 2020 2020 7665  dis/KeyDB.    ve
-00001040: 7273 696f 6e20 616e 6420 7572 6c2e 0a20  rsion and url.. 
-00001050: 2020 20da 046c 6962 634e 4663 0500 0000     ..libcNFc....
-00001060: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00001070: 0300 0000 731c 0000 0074 0083 006a 017c  ....s....t...j.|
-00001080: 017c 037c 0464 018d 0301 007c 027c 005f  .|.|.d.....|.|._
-00001090: 0264 0053 0029 024e a902 7226 0000 0072  .d.S.).N..r&...r
-000010a0: 2300 0000 2903 da05 7375 7065 7272 2900  #...)...superr).
-000010b0: 0000 da06 6d61 6c6c 6f63 2905 7227 0000  ....malloc).r'..
-000010c0: 00da 0962 7569 6c64 5f65 6e76 7263 0000  ...build_envrc..
-000010d0: 0072 2600 0000 7223 0000 00a9 01da 095f  .r&...r#......._
-000010e0: 5f63 6c61 7373 5f5f 720d 0000 0072 0e00  _class__r....r..
-000010f0: 0000 7229 0000 00b5 0000 0073 0400 0000  ..r).......s....
-00001100: 0001 1201 7a18 4461 7461 6261 7365 4275  ....z.DatabaseBu
-00001110: 696c 6465 722e 5f5f 696e 6974 5f5f 6301  ilder.__init__c.
-00001120: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001130: 0000 0043 0000 0073 3800 0000 6401 6402  ...C...s8...d.d.
-00001140: 8400 7c00 6a00 a001 a100 4400 8301 7d01  ..|.j.....D...}.
-00001150: 6403 6404 6802 7d02 6405 6406 6802 7d03  d.d.h.}.d.d.h.}.
-00001160: 7c02 a002 7c01 a101 7036 7c03 a002 7c01  |...|...p6|...|.
-00001170: a101 5300 2907 7a20 4368 6563 6b20 6966  ..S.).z Check if
-00001180: 2052 6564 6973 206f 7220 4b65 7944 4220   Redis or KeyDB 
-00001190: 6973 2062 7569 6c74 6301 0000 0000 0000  is builtc.......
-000011a0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-000011b0: 0073 1200 0000 6800 7c00 5d0a 7d01 7c01  .s....h.|.].}.|.
-000011c0: 6a00 9202 7104 5300 720d 0000 0029 0172  j...q.S.r....).r
-000011d0: 4200 0000 2902 da02 2e30 da04 6669 6c65  B...)....0..file
-000011e0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-000011f0: 093c 7365 7463 6f6d 703e bc00 0000 7304  .<setcomp>....s.
-00001200: 0000 0006 0002 007a 2b44 6174 6162 6173  .......z+Databas
-00001210: 6542 7569 6c64 6572 2e69 735f 6275 696c  eBuilder.is_buil
-00001220: 742e 3c6c 6f63 616c 733e 2e3c 7365 7463  t.<locals>.<setc
-00001230: 6f6d 703e 7a0c 7265 6469 732d 7365 7276  omp>z.redis-serv
-00001240: 6572 7a09 7265 6469 732d 636c 697a 0c6b  erz.redis-cliz.k
-00001250: 6579 6462 2d73 6572 7665 727a 096b 6579  eydb-serverz.key
-00001260: 6462 2d63 6c69 2903 721e 0000 00da 0769  db-cli).r......i
-00001270: 7465 7264 6972 da08 6973 7375 6273 6574  terdir..issubset
-00001280: 2904 7227 0000 005a 0962 696e 5f66 696c  ).r'...Z.bin_fil
-00001290: 6573 5a0b 7265 6469 735f 6669 6c65 735a  esZ.redis_filesZ
-000012a0: 0b6b 6579 6462 5f66 696c 6573 720d 0000  .keydb_filesr...
-000012b0: 0072 0d00 0000 720e 0000 0072 2e00 0000  .r....r....r....
-000012c0: b900 0000 7308 0000 0000 0314 0108 0108  ....s...........
-000012d0: 017a 1844 6174 6162 6173 6542 7569 6c64  .z.DatabaseBuild
-000012e0: 6572 2e69 735f 6275 696c 7463 0300 0000  er.is_builtc....
-000012f0: 0000 0000 0000 0000 1700 0000 0a00 0000  ................
-00001300: 4300 0000 734e 0200 0064 017c 016b 0672  C...sN...d.|.k.r
-00001310: 0c64 026e 0264 037d 0374 007c 006a 017c  .d.n.d.}.t.|.j.|
-00001320: 03a0 02a1 0083 027d 0474 007c 006a 0164  .......}.t.|.j.d
-00001330: 0383 027d 0574 007c 006a 0164 0283 027d  ...}.t.|.j.d...}
-00001340: 067c 05a0 03a1 0072 4e74 04a0 0574 067c  .|.....rNt...t.|
-00001350: 0583 01a1 0101 007c 06a0 03a1 0072 6474  .......|.....rdt
-00001360: 04a0 0574 067c 0683 01a1 0101 007c 00a0  ...t.|.......|..
-00001370: 077c 01a1 0173 8274 0864 047c 039b 0064  .|...s.t.d.|...d
-00001380: 057c 019b 009d 0483 0182 017c 00a0 0964  .|.........|...d
-00001390: 06a1 0164 077c 0164 087c 0264 0964 0a7c  ...d.|.d.|.d.d.|
-000013a0: 0367 087d 077c 006a 0a7c 077c 006a 0164  .g.}.|.j.|.|.j.d
-000013b0: 0b8d 0201 007c 00a0 0964 0ca1 0164 0d74  .....|...d...d.t
-000013c0: 067c 006a 0b83 0164 0e7c 006a 0c9b 009d  .|.j...d.|.j....
-000013d0: 0267 047d 087c 006a 0a7c 0874 067c 0483  .g.}.|.j.|.t.|..
-000013e0: 0164 0b8d 0201 007c 0464 0f1b 007d 097c  .d.....|.d...}.|
-000013f0: 097c 03a0 02a1 0064 1017 001b 007d 0a7c  .|.....d.....}.|
-00001400: 006a 0d7c 03a0 02a1 0064 1017 001b 007d  .j.|.....d.....}
-00001410: 0b7c 097c 03a0 02a1 0064 1117 001b 007d  .|.|.....d.....}
-00001420: 0c7c 006a 0d7c 03a0 02a1 0064 1117 001b  .|.j.|.....d....
-00001430: 007d 0d7c 006a 0e7c 0a7c 0b64 1264 138d  .}.|.j.|.|.d.d..
-00001440: 0301 007c 006a 0e7c 0c7c 0d64 1264 138d  ...|.j.|.|.d.d..
-00001450: 0301 0074 0074 0f6a 10a0 1174 12a1 0183  ...t.t.j...t....
-00001460: 016a 136a 137d 0e74 0f6a 14a0 1564 147c  .j.j.}.t.j...d.|
-00001470: 0ea1 027d 0f74 007c 0f64 1583 02a0 16a1  ...}.t.|.d......
-00001480: 007d 107a 3474 177c 10a0 1864 16a1 0183  .}.z4t.|...d....
-00001490: 017d 1174 0074 0f6a 14a0 1564 177c 11a1  .}.t.t.j...d.|..
-000014a0: 0283 01a0 16a1 007d 1274 1974 067c 1283  .......}.t.t.|..
-000014b0: 0183 017d 1357 006e 3204 0074 1a74 1b66  ...}.W.n2..t.t.f
-000014c0: 026b 0a90 0172 e001 007d 1401 007a 0e74  .k...r...}...z.t
-000014d0: 0864 1883 017c 1482 0257 0035 0064 197d  .d...|...W.5.d.}
-000014e0: 147e 1458 0059 006e 0258 007a 3474 177c  .~.X.Y.n.X.z4t.|
-000014f0: 10a0 1864 1aa1 0183 017d 1574 0074 0f6a  ...d.....}.t.t.j
-00001500: 14a0 1564 1b7c 15a1 0283 01a0 16a1 007d  ...d.|.........}
-00001510: 1674 1974 067c 1683 0183 017d 1357 006e  .t.t.|.....}.W.n
-00001520: 3204 0074 1a74 1b66 026b 0a90 0272 4801  2..t.t.f.k...rH.
-00001530: 007d 1401 007a 0e74 0864 1c83 017c 1482  .}...z.t.d...|..
-00001540: 0257 0035 0064 197d 147e 1458 0059 006e  .W.5.d.}.~.X.Y.n
-00001550: 0258 0064 1953 0029 1d7a b542 7569 6c64  .X.d.S.).z.Build
-00001560: 2052 6564 6973 2066 726f 6d20 6769 740a   Redis from git.
-00001570: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
-00001580: 6974 5f75 726c 3a20 7572 6c20 6672 6f6d  it_url: url from
-00001590: 2077 6869 6368 2074 6f20 7265 7472 6965   which to retrie
-000015a0: 7665 2052 6564 6973 0a20 2020 2020 2020  ve Redis.       
-000015b0: 203a 7479 7065 2067 6974 5f75 726c 3a20   :type git_url: 
-000015c0: 7374 720a 2020 2020 2020 2020 3a70 6172  str.        :par
-000015d0: 616d 2062 7261 6e63 683a 2062 7261 6e63  am branch: branc
-000015e0: 6820 746f 2063 6865 636b 6f75 740a 2020  h to checkout.  
-000015f0: 2020 2020 2020 3a74 7970 6520 6272 616e        :type bran
-00001600: 6368 3a20 7374 720a 2020 2020 2020 2020  ch: str.        
-00001610: 5a05 4b65 7944 425a 056b 6579 6462 5a05  Z.KeyDBZ.keydbZ.
-00001620: 7265 6469 737a 0a4d 616c 666f 726d 6564  redisz.Malformed
-00001630: 207a 0620 5552 4c3a 20da 0367 6974 da05   z. URL: ..git..
-00001640: 636c 6f6e 65fa 082d 2d62 7261 6e63 687a  clone..--branchz
-00001650: 072d 2d64 6570 7468 da01 31a9 0172 4e00  .--depth..1..rN.
-00001660: 0000 da04 6d61 6b65 fa02 2d6a 7a07 4d41  ....make..-jz.MA
-00001670: 4c4c 4f43 3d72 3900 0000 7a07 2d73 6572  LLOC=r9...z.-ser
-00001680: 7665 727a 042d 636c 6954 723f 0000 005a  verz.-cliTr?...Z
-00001690: 1953 4d41 5254 5349 4d5f 4445 505f 494e  .SMARTSIM_DEP_IN
-000016a0: 5354 414c 4c5f 5041 5448 7216 0000 007a  STALL_PATHr....z
-000016b0: 082a 2d73 6572 7665 725a 0a52 4544 4953  .*-serverZ.REDIS
-000016c0: 5f50 4154 487a 2449 6e73 7461 6c6c 6174  _PATHz$Installat
-000016d0: 696f 6e20 6f66 2072 6564 6973 2d73 6572  ion of redis-ser
-000016e0: 7665 7220 6661 696c 6564 214e 7a05 2a2d  ver failed!Nz.*-
-000016f0: 636c 695a 0e52 4544 4953 5f43 4c49 5f50  cliZ.REDIS_CLI_P
-00001700: 4154 487a 2149 6e73 7461 6c6c 6174 696f  ATHz!Installatio
-00001710: 6e20 6f66 2072 6564 6973 2d63 6c69 2066  n of redis-cli f
-00001720: 6169 6c65 6421 291c 7202 0000 0072 1d00  ailed!).r....r..
-00001730: 0000 da05 6c6f 7765 7272 2400 0000 7230  ....lowerr$...r0
-00001740: 0000 0072 4900 0000 724a 0000 0072 4800  ...rI...rJ...rH.
-00001750: 0000 7210 0000 0072 3200 0000 725a 0000  ..r....r2...rZ..
-00001760: 0072 2600 0000 7263 0000 0072 1e00 0000  .r&...rc...r....
-00001770: 723c 0000 0072 0500 0000 7206 0000 0072  r<...r....r....r
-00001780: 0a00 0000 7219 0000 0072 1a00 0000 721c  ....r....r....r.
-00001790: 0000 00da 0367 6574 da07 7265 736f 6c76  .....get..resolv
-000017a0: 65da 046e 6578 7472 4000 0000 720f 0000  e..nextr@...r...
-000017b0: 0072 0b00 0000 720c 0000 0029 1772 2700  .r....r....).r'.
-000017c0: 0000 da07 6769 745f 7572 6cda 0662 7261  ....git_url..bra
-000017d0: 6e63 685a 0d64 6174 6162 6173 655f 6e61  nchZ.database_na
-000017e0: 6d65 5a13 6461 7461 6261 7365 5f62 7569  meZ.database_bui
-000017f0: 6c64 5f70 6174 685a 1072 6564 6973 5f62  ld_pathZ.redis_b
-00001800: 7569 6c64 5f70 6174 685a 106b 6579 6462  uild_pathZ.keydb
-00001810: 5f62 7569 6c64 5f70 6174 68da 0963 6c6f  _build_path..clo
-00001820: 6e65 5f63 6d64 da09 6275 696c 645f 636d  ne_cmd..build_cm
-00001830: 645a 1064 6174 6162 6173 655f 7372 635f  dZ.database_src_
-00001840: 6469 725a 0d73 6572 7665 725f 736f 7572  dirZ.server_sour
-00001850: 6365 5a12 7365 7276 6572 5f64 6573 7469  ceZ.server_desti
-00001860: 6e61 7469 6f6e 5a0a 636c 695f 736f 7572  nationZ.cli_sour
-00001870: 6365 5a0f 636c 695f 6465 7374 696e 6174  ceZ.cli_destinat
-00001880: 696f 6e5a 0963 6f72 655f 7061 7468 7228  ionZ.core_pathr(
-00001890: 0000 0072 1e00 0000 5a0c 6461 7461 6261  ...r....Z.databa
-000018a0: 7365 5f65 7865 5a08 6461 7461 6261 7365  se_exeZ.database
-000018b0: da01 5f72 5900 0000 5a0d 7265 6469 735f  .._rY...Z.redis_
-000018c0: 636c 695f 6578 655a 0972 6564 6973 5f63  cli_exeZ.redis_c
-000018d0: 6c69 720d 0000 0072 0d00 0000 720e 0000  lir....r....r...
-000018e0: 0072 2f00 0000 c100 0000 7360 0000 0000  .r/.......s`....
-000018f0: 0710 0110 040c 010c 0108 010e 0108 010e  ................
-00001900: 030a 0114 0408 0102 0102 0102 0102 0102  ................
-00001910: 0102 0102 f804 0a10 0408 0102 0108 010a  ................
-00001920: fc04 0612 0308 0110 0112 0110 0112 0110  ................
-00001930: 0110 0314 010e 010e 0102 010e 0116 0110  ................
-00001940: 0116 011c 0302 010e 0116 0110 0116 017a  ...............z
-00001950: 1e44 6174 6162 6173 6542 7569 6c64 6572  .DatabaseBuilder
-00001960: 2e62 7569 6c64 5f66 726f 6d5f 6769 7429  .build_from_git)
-00001970: 0972 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001980: 725b 0000 0072 2900 0000 725e 0000 0072  r[...r)...r^...r
-00001990: 2e00 0000 722f 0000 00da 0d5f 5f63 6c61  ....r/.....__cla
-000019a0: 7373 6365 6c6c 5f5f 720d 0000 0072 0d00  sscell__r....r..
-000019b0: 0000 7265 0000 0072 0e00 0000 725f 0000  ..re...r....r_..
-000019c0: 00ad 0000 0073 0a00 0000 0801 0407 1604  .....s..........
-000019d0: 0201 0a07 725f 0000 0063 0000 0000 0000  ....r_...c......
-000019e0: 0000 0000 0000 0000 0000 0800 0000 0000  ................
-000019f0: 0000 7372 0000 0065 005a 0164 005a 0264  ..sr...e.Z.d.Z.d
-00001a00: 015a 0369 0064 0264 0264 0364 0364 0464  .Z.i.d.d.d.d.d.d
-00001a10: 0564 0466 0887 0066 0164 0664 0784 095a  .d.f...f.d.d...Z
-00001a20: 0465 0564 0864 0984 0083 015a 0665 0564  .e.d.d.....Z.e.d
-00001a30: 0a64 0b84 0083 015a 0764 0c64 0d84 005a  .d.....Z.d.d...Z
-00001a40: 0864 0e64 0f84 005a 0964 1064 1184 005a  .d.d...Z.d.d...Z
-00001a50: 0a64 1264 1384 005a 0b64 1464 1584 005a  .d.d...Z.d.d...Z
-00001a60: 0c87 0004 005a 0d53 0029 16da 0e52 6564  .....Z.S.)...Red
-00001a70: 6973 4149 4275 696c 6465 727a a343 6c61  isAIBuilderz.Cla
-00001a80: 7373 2074 6f20 6275 696c 6420 5265 6469  ss to build Redi
-00001a90: 7341 4920 6672 6f6d 2053 6f75 7263 650a  sAI from Source.
-00001aa0: 2020 2020 5375 7070 6f72 7465 6420 6275      Supported bu
-00001ab0: 696c 6420 6d65 7468 6f64 3a0a 2020 2020  ild method:.    
-00001ac0: 202d 2066 726f 6d20 6769 740a 2020 2020   - from git.    
-00001ad0: 5365 6520 6275 696c 6465 6e76 2e70 7920  See buildenv.py 
-00001ae0: 666f 7220 6275 696c 6474 696d 6520 636f  for buildtime co
-00001af0: 6e66 6967 7572 6174 696f 6e20 6f66 2052  nfiguration of R
-00001b00: 6564 6973 4149 0a20 2020 2076 6572 7369  edisAI.    versi
-00001b10: 6f6e 2061 6e64 2075 726c 2e0a 2020 2020  on and url..    
-00001b20: da00 5446 4e63 0900 0000 0000 0000 0000  ..TFNc..........
-00001b30: 0000 0900 0000 0500 0000 0300 0000 734c  ..............sL
-00001b40: 0000 0074 0083 006a 017c 017c 077c 0864  ...t...j.|.|.|.d
-00001b50: 018d 0301 007c 0472 1a64 026e 0264 037c  .....|.r.d.n.d.|
-00001b60: 005f 027c 0572 2864 026e 0264 037c 005f  ._.|.r(d.n.d.|._
-00001b70: 037c 0672 3664 026e 0264 037c 005f 047c  .|.r6d.n.d.|._.|
-00001b80: 037c 005f 057c 027c 005f 0664 0053 0029  .|._.|.|._.d.S.)
-00001b90: 044e 7261 0000 0072 1500 0000 7201 0000  .Nra...r....r...
-00001ba0: 0029 0772 6200 0000 7229 0000 00da 0574  .).rb...r).....t
-00001bb0: 6f72 6368 da02 7466 da04 6f6e 6e78 da09  orch..tf..onnx..
-00001bc0: 6c69 6274 665f 6469 72da 0974 6f72 6368  libtf_dir..torch
-00001bd0: 5f64 6972 2909 7227 0000 0072 6400 0000  _dir).r'...rd...
-00001be0: 7283 0000 0072 8200 0000 5a0b 6275 696c  r....r....Z.buil
-00001bf0: 645f 746f 7263 685a 0862 7569 6c64 5f74  d_torchZ.build_t
-00001c00: 665a 0a62 7569 6c64 5f6f 6e6e 7872 2600  fZ.build_onnxr&.
-00001c10: 0000 7223 0000 0072 6500 0000 720d 0000  ..r#...re...r...
-00001c20: 0072 0e00 0000 7229 0000 0013 0100 0073  .r....r).......s
-00001c30: 0c00 0000 000b 1203 0e01 0e01 0e01 0601  ................
-00001c40: 7a17 5265 6469 7341 4942 7569 6c64 6572  z.RedisAIBuilder
-00001c50: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00001c60: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001c70: 0000 730c 0000 0074 007c 006a 0164 0183  ..s....t.|.j.d..
-00001c80: 0253 0029 024e da07 5265 6469 7341 4929  .S.).N..RedisAI)
-00001c90: 0272 0200 0000 721d 0000 0072 2d00 0000  .r....r....r-...
-00001ca0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-00001cb0: 0e72 6169 5f62 7569 6c64 5f70 6174 6827  .rai_build_path'
-00001cc0: 0100 0073 0200 0000 0002 7a1d 5265 6469  ...s......z.Redi
-00001cd0: 7341 4942 7569 6c64 6572 2e72 6169 5f62  sAIBuilder.rai_b
-00001ce0: 7569 6c64 5f70 6174 6863 0100 0000 0000  uild_pathc......
-00001cf0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00001d00: 0000 7328 0000 007c 006a 00a0 0164 01a1  ..s(...|.j...d..
-00001d10: 01a0 02a1 007d 017c 006a 00a0 0164 02a1  .....}.|.j...d..
-00001d20: 01a0 03a1 007d 027c 016f 267c 0253 0029  .....}.|.o&|.S.)
-00001d30: 034e da08 6261 636b 656e 6473 fa0a 7265  .N..backends..re
-00001d40: 6469 7361 692e 736f 2904 721f 0000 00da  disai.so).r.....
-00001d50: 086a 6f69 6e70 6174 6872 2400 0000 da07  .joinpathr$.....
-00001d60: 6973 5f66 696c 6529 0372 2700 0000 da06  is_file).r'.....
-00001d70: 7365 7276 6572 da03 636c 6972 0d00 0000  server..clir....
-00001d80: 720d 0000 0072 0e00 0000 722e 0000 002b  r....r....r....+
-00001d90: 0100 0073 0600 0000 0002 1001 1001 7a17  ...s..........z.
-00001da0: 5265 6469 7341 4942 7569 6c64 6572 2e69  RedisAIBuilder.i
-00001db0: 735f 6275 696c 7463 0100 0000 0000 0000  s_builtc........
-00001dc0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00001dd0: 733c 0000 007c 006a 0064 011b 007d 017c  s<...|.j.d...}.|
-00001de0: 01a0 01a1 0001 007c 01a0 02a1 0072 387c  .......|.....r8|
-00001df0: 01a0 03a1 0001 007c 006a 047c 006a 0564  .......|.j.|.j.d
-00001e00: 021b 007c 0164 0364 048d 0301 0064 0553  ...|.d.d.....d.S
-00001e10: 0029 067a be43 6f70 7920 7468 6520 4669  .).z.Copy the Fi
-00001e20: 6e64 5465 6e73 6f72 466c 6f77 2e63 6d61  ndTensorFlow.cma
-00001e30: 6b65 2066 696c 6520 746f 2074 6865 2062  ke file to the b
-00001e40: 7569 6c64 2064 6972 6563 746f 7279 0a20  uild directory. 
-00001e50: 2020 2020 2020 2061 7320 7468 6520 7665         as the ve
-00001e60: 7273 696f 6e20 696e 636c 7564 6564 2069  rsion included i
-00001e70: 6e20 5265 6469 7341 4920 6973 206f 7574  n RedisAI is out
-00001e80: 206f 6620 6461 7465 2066 6f72 2075 732e   of date for us.
-00001e90: 0a20 2020 2020 2020 204e 6f74 653a 206f  .        Note: o
-00001ea0: 7074 2f63 6d61 6b65 2f6d 6f64 756c 6573  pt/cmake/modules
-00001eb0: 2072 656d 6f76 6564 2069 6e20 5265 6469   removed in Redi
-00001ec0: 7341 4920 7631 2e32 2e35 0a20 2020 2020  sAI v1.2.5.     
-00001ed0: 2020 207a 266f 7074 2f63 6d61 6b65 2f6d     z&opt/cmake/m
-00001ee0: 6f64 756c 6573 2f46 696e 6454 656e 736f  odules/FindTenso
-00001ef0: 7246 6c6f 772e 636d 616b 657a 1c6d 6f64  rFlow.cmakez.mod
-00001f00: 756c 6573 2f46 696e 6454 656e 736f 7246  ules/FindTensorF
-00001f10: 6c6f 772e 636d 616b 6546 723f 0000 004e  low.cmakeFr?...N
-00001f20: 2906 7285 0000 0072 7500 0000 7289 0000  ).r....ru...r...
-00001f30: 00da 0675 6e6c 696e 6b72 3c00 0000 721e  ...unlinkr<...r.
-00001f40: 0000 0029 0272 2700 0000 5a08 7466 5f63  ...).r'...Z.tf_c
-00001f50: 6d61 6b65 720d 0000 0072 0d00 0000 720e  maker....r....r.
-00001f60: 0000 00da 0d63 6f70 795f 7466 5f63 6d61  .....copy_tf_cma
-00001f70: 6b65 3101 0000 7312 0000 0000 060a 0108  ke1...s.........
-00001f80: 0108 0108 0204 0108 0002 0002 ff7a 1c52  .............z.R
-00001f90: 6564 6973 4149 4275 696c 6465 722e 636f  edisAIBuilder.co
-00001fa0: 7079 5f74 665f 636d 616b 6563 0200 0000  py_tf_cmakec....
-00001fb0: 0000 0000 0000 0000 0b00 0000 0900 0000  ................
-00001fc0: 4300 0000 732e 0100 0074 007c 006a 01a0  C...s....t.|.j..
-00001fd0: 0274 036a 04a0 0564 0164 027c 019b 0064  .t.j...d.d.|...d
-00001fe0: 029d 03a1 02a1 0183 017d 027c 0273 2e74  .........}.|.s.t
-00001ff0: 0664 0383 0182 017c 0264 0419 0064 051b  .d.....|.d...d..
-00002000: 007d 037c 03a0 07a1 0001 007c 03a0 08a1  .}.|.......|....
-00002010: 0072 5474 09a0 0a7c 03a1 0101 0074 03a0  .rTt...|.....t..
-00002020: 0b7c 03a1 0101 0074 0c7c 006a 0d83 01a0  .|.....t.|.j....
-00002030: 07a1 007d 047c 0464 061b 007d 057c 05a0  ...}.|.d...}.|..
-00002040: 0ea1 0073 8a74 0664 077c 049b 009d 0283  ...s.t.d.|......
-00002050: 0182 0174 03a0 0f7c 057c 0364 061b 00a1  ...t...|.|.d....
-00002060: 0201 007c 0364 081b 007d 0674 03a0 0b7c  ...|.d...}.t...|
-00002070: 06a1 0101 007c 0464 081b 007d 077c 07a0  .....|.d...}.|..
-00002080: 08a1 0072 de74 007c 07a0 0264 02a1 0183  ...r.t.|...d....
-00002090: 017d 087c 0873 fe74 0664 097c 079b 009d  .}.|.s.t.d.|....
-000020a0: 0283 0182 016e 2074 007c 04a0 0264 0aa1  .....n t.|...d..
-000020b0: 0183 017d 087c 0873 fe74 0664 097c 049b  ...}.|.s.t.d.|..
-000020c0: 009d 0283 0182 017c 0844 005d 267d 097c  .......|.D.]&}.|
-000020d0: 067c 096a 101b 007d 0a7c 0aa0 11a1 0090  .|.j...}.|......
-000020e0: 0173 0274 03a0 0f7c 097c 0aa1 0201 0090  .s.t...|.|......
-000020f0: 0171 0264 0b53 0029 0c7a 8341 6464 2073  .q.d.S.).z.Add s
-00002100: 796d 626f 6c69 6320 6c69 6e6b 2074 6f20  ymbolic link to 
-00002110: 6176 6169 6c61 626c 6520 6c69 6274 656e  available libten
-00002120: 736f 7266 6c6f 7720 696e 2052 6564 6973  sorflow in Redis
-00002130: 4149 2064 6570 732e 0a0a 2020 2020 2020  AI deps...      
-00002140: 2020 3a70 6172 616d 2064 6576 6963 653a    :param device:
-00002150: 2063 7075 206f 7220 6770 750a 2020 2020   cpu or gpu.    
-00002160: 2020 2020 3a74 7970 6520 6465 7669 6365      :type device
-00002170: 3a20 7374 720a 2020 2020 2020 2020 da04  : str.        ..
-00002180: 6465 7073 723e 0000 007a 2743 6f75 6c64  depsr>...z'Could
-00002190: 206e 6f74 2066 696e 6420 5265 6469 7341   not find RedisA
-000021a0: 4920 2764 6570 7327 2064 6972 6563 746f  I 'deps' directo
-000021b0: 7279 7201 0000 005a 0d6c 6962 7465 6e73  ryr....Z.libtens
-000021c0: 6f72 666c 6f77 da07 696e 636c 7564 657a  orflow..includez
-000021d0: 2443 6f75 6c64 206e 6f74 2066 696e 6420  $Could not find 
-000021e0: 696e 636c 7564 6520 6469 7265 6374 6f72  include director
-000021f0: 7920 696e 2072 1700 0000 7a2e 436f 756c  y in r....z.Coul
-00002200: 6420 6e6f 7420 6669 6e64 206c 6962 7465  d not find libte
-00002210: 6e73 6f72 666c 6f77 206c 6962 7261 7279  nsorflow library
-00002220: 2066 696c 6573 2069 6e20 7a08 6c69 622a   files in z.lib*
-00002230: 2e73 6f2a 4e29 12da 0673 6f72 7465 6472  .so*N)...sortedr
-00002240: 8500 0000 7240 0000 0072 0500 0000 7206  ....r@...r....r.
-00002250: 0000 00da 046a 6f69 6e72 0c00 0000 7275  .....joinr....ru
-00002260: 0000 0072 2400 0000 7230 0000 0072 4900  ...r$...r0...rI.
-00002270: 0000 da08 6d61 6b65 6469 7273 7202 0000  ....makedirsr...
-00002280: 0072 8200 0000 da06 6578 6973 7473 da07  .r......exists..
-00002290: 7379 6d6c 696e 6b72 4200 0000 7289 0000  symlinkrB...r...
-000022a0: 0029 0b72 2700 0000 da06 6465 7669 6365  .).r'.....device
-000022b0: 5a0d 7261 695f 6465 7073 5f70 6174 685a  Z.rai_deps_pathZ
-000022c0: 0e72 6169 5f6c 6962 7466 5f70 6174 685a  .rai_libtf_pathZ
-000022d0: 0a6c 6962 7466 5f70 6174 685a 1069 6e63  .libtf_pathZ.inc
-000022e0: 6c75 6465 5f73 7263 5f70 6174 685a 1172  lude_src_pathZ.r
-000022f0: 6169 5f6c 6962 7466 5f6c 6962 5f64 6972  ai_libtf_lib_dir
-00002300: 5a11 7372 635f 6c69 6274 665f 6c69 625f  Z.src_libtf_lib_
-00002310: 6469 725a 0d6c 6962 7261 7279 5f66 696c  dirZ.library_fil
-00002320: 6573 5a08 7372 635f 6669 6c65 5a08 6473  esZ.src_fileZ.ds
-00002330: 745f 6669 6c65 720d 0000 0072 0d00 0000  t_filer....r....
-00002340: 720e 0000 00da 0d73 796d 6c69 6e6b 5f6c  r......symlink_l
-00002350: 6962 7466 4001 0000 7342 0000 0000 0602  ibtf@...sB......
-00002360: 011c ff04 0304 0108 050c 0108 0108 010a  ................
-00002370: 020a 010e 0308 0108 010e 0110 0408 010a  ................
-00002380: 0108 0408 010e 0104 0102 0108 ff06 040e  ................
-00002390: 0104 0102 0108 ff04 0408 010a 010a 017a  ...............z
-000023a0: 1c52 6564 6973 4149 4275 696c 6465 722e  .RedisAIBuilder.
-000023b0: 7379 6d6c 696e 6b5f 6c69 6274 6663 0400  symlink_libtfc..
-000023c0: 0000 0000 0000 0000 0000 0800 0000 0900  ................
-000023d0: 0000 4300 0000 73ec 0100 007c 006a 00a0  ..C...s....|.j..
-000023e0: 01a1 0072 1674 02a0 037c 006a 00a1 0101  ...r.t...|.j....
-000023f0: 007c 00a0 047c 01a1 0173 2e74 0564 017c  .|...|...s.t.d.|
-00002400: 019b 009d 0283 0182 017c 00a0 0664 02a1  .........|...d..
-00002410: 0164 0364 0464 0564 067c 0167 067d 0474  .d.d.d.d.|.g.}.t
-00002420: 076a 0864 076b 0272 727c 0264 086b 0272  .j.d.k.rr|.d.k.r
-00002430: 727c 006a 0972 727c 0464 0967 0137 007d  r|.j.rr|.d.g.7.}
-00002440: 0464 0464 0a64 0b67 037d 056e 147c 0464  .d.d.d.g.}.n.|.d
-00002450: 0c7c 0264 0d64 0967 0437 007d 0467 007d  .|.d.d.g.7.}.g.}
-00002460: 057c 006a 0a7c 0474 0b6a 0c7c 006a 0d64  .|.j.|.t.j.|.j.d
-00002470: 0e8d 0301 007c 0572 b27c 006a 0a7c 0574  .....|.r.|.j.|.t
-00002480: 0b6a 0c7c 006a 0064 0e8d 0301 007c 00a0  .j.|.j.d.....|..
-00002490: 0ea1 0001 007c 00a0 0664 02a1 0164 0f64  .....|...d...d.d
-000024a0: 107c 006a 0f72 d67c 006a 1073 d664 116e  .|.j.r.|.j.s.d.n
-000024b0: 0264 129b 009d 0264 1364 147c 006a 099b  .d.....d.d.|.j..
-000024c0: 009d 0264 157c 00a0 0664 16a1 017c 006a  ...d.|...d...|.j
-000024d0: 0064 171b 007c 0367 097d 067c 006a 0a7c  .d...|.g.}.|.j.|
-000024e0: 0674 0b6a 0c7c 006a 0064 0e8d 0301 007c  .t.j.|.j.d.....|
-000024f0: 006a 1090 0172 267c 00a0 117c 03a1 0101  .j...r&|...|....
-00002500: 007c 00a0 0664 02a1 0164 187c 006a 129b  .|...d...d.|.j..
-00002510: 009d 0264 107c 006a 0f9b 009d 0264 1364  ...d.|.j.....d.d
-00002520: 147c 006a 099b 009d 0264 1967 067d 077c  .|.j.....d.g.}.|
-00002530: 0364 1a6b 0290 0172 6a7c 07a0 1364 1ba1  .d.k...rj|...d..
-00002540: 0101 006e 0a7c 07a0 1364 1ca1 0101 007c  ...n.|...d.....|
-00002550: 006a 1490 0172 8c74 157c 006a 1483 017c  .j...r.t.|.j...|
-00002560: 006a 1664 1d3c 007c 07a0 177c 00a0 0664  .j.d.<.|...|...d
-00002570: 1ea1 0164 1f74 157c 006a 0064 201b 0083  ...d.t.|.j.d ...
-00002580: 0164 217c 006a 189b 0064 2267 06a1 0101  .d!|.j...d"g....
-00002590: 007c 006a 0a7c 077c 006a 0064 238d 0201  .|.j.|.|.j.d#...
-000025a0: 007c 00a0 197c 03a1 0101 007c 006a 1290  .|...|.....|.j..
-000025b0: 0172 e07c 00a0 1aa1 0001 007c 00a0 1ba1  .r.|.......|....
-000025c0: 0001 0064 2453 0029 257a f542 7569 6c64  ...d$S.)%z.Build
-000025d0: 2052 6564 6973 4149 2066 726f 6d20 6769   RedisAI from gi
-000025e0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000025f0: 2067 6974 5f75 726c 3a20 7572 6c20 6672   git_url: url fr
-00002600: 6f6d 2077 6869 6368 2074 6f20 7265 7472  om which to retr
-00002610: 6965 7665 2052 6564 6973 4149 0a20 2020  ieve RedisAI.   
-00002620: 2020 2020 203a 7479 7065 2067 6974 5f75       :type git_u
-00002630: 726c 3a20 7374 720a 2020 2020 2020 2020  rl: str.        
-00002640: 3a70 6172 616d 2062 7261 6e63 683a 2062  :param branch: b
-00002650: 7261 6e63 6820 746f 2063 6865 636b 6f75  ranch to checkou
-00002660: 740a 2020 2020 2020 2020 3a74 7970 6520  t.        :type 
-00002670: 6272 616e 6368 3a20 7374 720a 2020 2020  branch: str.    
-00002680: 2020 2020 3a70 6172 616d 2064 6576 6963      :param devic
-00002690: 653a 2063 7075 206f 7220 6770 750a 2020  e: cpu or gpu.  
-000026a0: 2020 2020 2020 3a74 7970 6520 6465 7669        :type devi
-000026b0: 6365 3a20 7374 720a 2020 2020 2020 2020  ce: str.        
-000026c0: 7a17 4d61 6c66 6f72 6d65 6420 5265 6469  z.Malformed Redi
-000026d0: 7341 4920 5552 4c3a 2072 1800 0000 7a15  sAI URL: r....z.
-000026e0: 4749 545f 4c46 535f 534b 4950 5f53 4d55  GIT_LFS_SKIP_SMU
-000026f0: 4447 453d 3172 6c00 0000 726d 0000 007a  DGE=1rl...rm...z
-00002700: 0b2d 2d72 6563 7572 7369 7665 da06 6461  .--recursive..da
-00002710: 7277 696e 7a06 7631 2e32 2e37 7284 0000  rwinz.v1.2.7r...
-00002720: 005a 0863 6865 636b 6f75 745a 2836 3334  .Z.checkoutZ(634
-00002730: 3931 3663 3732 3265 3731 3863 6336 6561  916c722e718cc6ea
-00002740: 3366 6164 3436 6536 3366 3764 3739 3866  3fad46e63f7d798f
-00002750: 3961 6463 3272 6e00 0000 7a09 2d2d 6465  9adc2rn...z.--de
-00002760: 7074 683d 3129 0272 2200 0000 724e 0000  pth=1).r"...rN..
-00002770: 007a 0957 4954 485f 5054 3d30 7a08 5749  .z.WITH_PT=0z.WI
-00002780: 5448 5f54 463d 7215 0000 0072 0100 0000  TH_TF=r....r....
-00002790: 7a0d 5749 5448 5f54 464c 4954 453d 307a  z.WITH_TFLITE=0z
-000027a0: 0957 4954 485f 4f52 543d 7a09 5645 5242  .WITH_ORT=z.VERB
-000027b0: 4f53 453d 315a 0462 6173 687a 0b67 6574  OSE=1Z.bashz.get
-000027c0: 5f64 6570 732e 7368 7a08 5749 5448 5f50  _deps.shz.WITH_P
-000027d0: 543d 7a11 5749 5448 5f55 4e49 545f 5445  T=z.WITH_UNIT_TE
-000027e0: 5354 533d 305a 0367 7075 7a05 4750 553d  STS=0Z.gpuz.GPU=
-000027f0: 317a 0547 5055 3d30 5a09 546f 7263 685f  1z.GPU=0Z.Torch_
-00002800: 4449 5272 7100 0000 7a02 2d43 da03 6f70  DIRrq...z.-C..op
-00002810: 7472 7200 0000 da05 6275 696c 6472 7000  trr.....buildrp.
-00002820: 0000 4e29 1c72 8500 0000 7224 0000 0072  ..N).r....r$...r
-00002830: 3000 0000 7249 0000 0072 4800 0000 7210  0...rI...rH...r.
-00002840: 0000 0072 3200 0000 da03 7379 73da 0870  ...r2.....sys..p
-00002850: 6c61 7466 6f72 6d72 8100 0000 725a 0000  latformr....rZ..
-00002860: 0072 2000 0000 7221 0000 0072 1d00 0000  .r ...r!...r....
-00002870: 728d 0000 0072 8000 0000 7282 0000 0072  r....r....r....r
-00002880: 9600 0000 727f 0000 00da 0661 7070 656e  ....r......appen
-00002890: 6472 8300 0000 724a 0000 0072 1800 0000  dr....rJ...r....
-000028a0: da06 6578 7465 6e64 7226 0000 00da 115f  ..extendr&....._
-000028b0: 696e 7374 616c 6c5f 6261 636b 656e 6473  install_backends
-000028c0: da10 5f6d 6f76 655f 746f 7263 685f 6c69  .._move_torch_li
-000028d0: 6273 724b 0000 0029 0872 2700 0000 7277  bsrK...).r'...rw
-000028e0: 0000 0072 7800 0000 7295 0000 0072 7900  ...rx...r....ry.
-000028f0: 0000 5a10 6368 6563 6b6f 7574 5f6f 7378  ..Z.checkout_osx
-00002900: 5f66 6978 5a07 6465 705f 636d 6472 7a00  _fixZ.dep_cmdrz.
-00002910: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00002920: 0072 2f00 0000 7701 0000 7396 0000 0000  .r/...w...s.....
-00002930: 0a0a 010c 030a 010e 0408 0102 0102 0102  ................
-00002940: 0102 0102 fa04 0a18 020a 0202 0102 0102  ................
-00002950: fd06 0702 0102 0102 0102 0102 fc06 0604  ................
-00002960: 0214 0104 0104 0102 0004 0004 ff06 0508  ................
-00002970: 0408 0102 0118 0102 010a 0102 0108 0108  ................
-00002980: 0102 f704 0c04 0102 0104 0104 fd06 0608  ................
-00002990: 010a 0308 010a 010a 0102 010a 0102 fa04  ................
-000029a0: 090a 010c 020a 0208 0110 0204 0208 0102  ................
-000029b0: 010c 0102 0106 0102 fa02 ff04 0a10 020a  ................
-000029c0: 0108 0108 017a 1d52 6564 6973 4149 4275  .....z.RedisAIBu
-000029d0: 696c 6465 722e 6275 696c 645f 6672 6f6d  ilder.build_from
-000029e0: 5f67 6974 6302 0000 0000 0000 0000 0000  _gitc...........
-000029f0: 0004 0000 0005 0000 0043 0000 0073 6c00  .........C...sl.
-00002a00: 0000 7c00 6a00 a001 6401 7c01 9b00 9d02  ..|.j...d.|.....
-00002a10: a101 a002 a100 7c00 5f03 7c00 6a03 6402  ......|._.|.j.d.
-00002a20: 1b00 7d02 7c00 6a03 6403 1b00 7d03 7c02  ..}.|.j.d...}.|.
-00002a30: a004 a100 7268 7c03 a005 a100 7268 7c00  ....rh|.....rh|.
-00002a40: 6a06 7c03 7c00 6a07 6403 1b00 6404 6405  j.|.|.j.d...d.d.
-00002a50: 8d03 0100 7c00 6a08 7c02 7c00 6a07 6402  ....|.j.|.|.j.d.
-00002a60: 1b00 6404 6405 8d03 0100 6406 5300 2907  ..d.d.....d.S.).
-00002a70: 7a72 4d6f 7665 2062 6163 6b65 6e64 206c  zrMove backend l
-00002a80: 6962 7261 7269 6573 2074 6f20 736d 6172  ibraries to smar
-00002a90: 7473 696d 2f5f 636f 7265 2f6c 6962 2f0a  tsim/_core/lib/.
-00002aa0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00002ab0: 6576 6963 653a 2063 7075 206f 7220 6370  evice: cpu or cp
-00002ac0: 750a 2020 2020 2020 2020 3a74 7970 6520  u.        :type 
-00002ad0: 6465 7669 6365 3a20 7374 720a 2020 2020  device: str.    
-00002ae0: 2020 2020 7a08 696e 7374 616c 6c2d 7287      z.install-r.
-00002af0: 0000 0072 8600 0000 5472 3f00 0000 4e29  ...r....Tr?...N)
-00002b00: 0972 8500 0000 7288 0000 0072 7500 0000  .r....r....ru...
-00002b10: 5a10 7261 695f 696e 7374 616c 6c5f 7061  Z.rai_install_pa
-00002b20: 7468 7289 0000 0072 2400 0000 7241 0000  thr....r$...rA..
-00002b30: 0072 1f00 0000 723c 0000 0029 0472 2700  .r....r<...).r'.
-00002b40: 0000 7295 0000 005a 0772 6169 5f6c 6962  ..r....Z.rai_lib
-00002b50: 5a0c 7261 695f 6261 636b 656e 6473 720d  Z.rai_backendsr.
-00002b60: 0000 0072 0d00 0000 720e 0000 0072 9e00  ...r....r....r..
-00002b70: 0000 e601 0000 7310 0000 0000 0506 0108  ......s.........
-00002b80: ff0a 030a 010a 0210 0116 017a 2052 6564  ...........z Red
-00002b90: 6973 4149 4275 696c 6465 722e 5f69 6e73  isAIBuilder._ins
-00002ba0: 7461 6c6c 5f62 6163 6b65 6e64 7363 0100  tall_backendsc..
-00002bb0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
-00002bc0: 0000 4300 0000 7368 0000 007c 006a 0064  ..C...sh...|.j.d
-00002bd0: 011b 0064 021b 007d 017c 0164 031b 007d  ...d...}.|.d...}
-00002be0: 0274 017c 006a 0283 016a 036a 036a 037d  .t.|.j...j.j.j.}
-00002bf0: 037c 0364 031b 007d 047c 006a 047c 047c  .|.d...}.|.j.|.|
-00002c00: 0264 0464 058d 0301 0074 056a 0664 066b  .d.d.....t.j.d.k
-00002c10: 0272 647c 0364 071b 007d 057c 006a 047c  .rd|.d...}.|.j.|
-00002c20: 057c 0164 071b 0064 0464 058d 0301 0064  .|.d...d.d.....d
-00002c30: 0853 0029 097a de4d 6f76 6520 7069 7020  .S.).z.Move pip 
-00002c40: 696e 7374 616c 6c20 746f 7263 6820 6c69  install torch li
-00002c50: 6272 6172 6965 730a 2020 2020 2020 2020  braries.        
-00002c60: 5369 6e63 6520 7765 2075 7365 2070 6970  Since we use pip
-00002c70: 2069 6e73 7461 6c6c 6564 2074 6f72 6368   installed torch
-00002c80: 206c 6962 7261 7269 6573 2066 6f72 2062   libraries for b
-00002c90: 7569 6c64 696e 670a 2020 2020 2020 2020  uilding.        
-00002ca0: 5265 6469 7341 492c 2077 6520 6e65 6564  RedisAI, we need
-00002cb0: 2074 6f20 6d6f 7665 2074 6865 6d20 696e   to move them in
-00002cc0: 746f 2074 6865 204c 445f 7275 6e70 6174  to the LD_runpat
-00002cd0: 6820 6f66 2072 6564 6973 6169 2e73 6f0a  h of redisai.so.
-00002ce0: 2020 2020 2020 2020 696e 2074 6865 2073          in the s
-00002cf0: 6d61 7274 7369 6d2f 5f63 6f72 652f 6c69  martsim/_core/li
-00002d00: 6220 6469 7265 6374 6f72 792e 0a20 2020  b directory..   
-00002d10: 2020 2020 2072 8600 0000 5a0d 7265 6469       r....Z.redi
-00002d20: 7361 695f 746f 7263 6872 1700 0000 5472  sai_torchr....Tr
-00002d30: 3f00 0000 7297 0000 007a 072e 6479 6c69  ?...r....z..dyli
-00002d40: 6273 4e29 0772 1f00 0000 7202 0000 0072  bsN).r....r....r
-00002d50: 8300 0000 721a 0000 0072 4100 0000 729a  ....r....rA...r.
-00002d60: 0000 0072 9b00 0000 2906 7227 0000 005a  ...r....).r'...Z
-00002d70: 1173 735f 7261 695f 746f 7263 685f 7061  .ss_rai_torch_pa
-00002d80: 7468 5a15 7373 5f72 6169 5f74 6f72 6368  thZ.ss_rai_torch
-00002d90: 5f6c 6962 5f70 6174 685a 0e70 6970 5f74  _lib_pathZ.pip_t
-00002da0: 6f72 6368 5f70 6174 685a 1270 6970 5f74  orch_pathZ.pip_t
-00002db0: 6f72 6368 5f6c 6962 5f70 6174 685a 0664  orch_lib_pathZ.d
-00002dc0: 796c 6962 7372 0d00 0000 720d 0000 0072  ylibsr....r....r
-00002dd0: 0e00 0000 729f 0000 00f5 0100 0073 1000  ....r........s..
-00002de0: 0000 0007 0e01 0806 1001 0802 1003 0a01  ................
-00002df0: 0801 7a1f 5265 6469 7341 4942 7569 6c64  ..z.RedisAIBuild
-00002e00: 6572 2e5f 6d6f 7665 5f74 6f72 6368 5f6c  er._move_torch_l
-00002e10: 6962 7329 0e72 1100 0000 7212 0000 0072  ibs).r....r....r
-00002e20: 1300 0000 725b 0000 0072 2900 0000 725e  ....r[...r)...r^
-00002e30: 0000 0072 8500 0000 722e 0000 0072 8d00  ...r....r....r..
-00002e40: 0000 7296 0000 0072 2f00 0000 729e 0000  ..r....r/...r...
-00002e50: 0072 9f00 0000 727c 0000 0072 0d00 0000  .r....r|...r....
-00002e60: 720d 0000 0072 6500 0000 720e 0000 0072  r....re...r....r
-00002e70: 7d00 0000 0b01 0000 7326 0000 0008 0104  }.......s&......
-00002e80: 0902 0102 0102 0102 0102 0102 0102 0102  ................
-00002e90: f70e 1402 010a 0302 010a 0508 0f08 3708  ..............7.
-00002ea0: 6f08 0f72 7d00 0000 2910 7205 0000 0072  o..r}...).r....r
-00002eb0: 4400 0000 7230 0000 0072 3500 0000 7220  D...r0...r5...r 
-00002ec0: 0000 0072 9a00 0000 da07 7061 7468 6c69  ...r......pathli
-00002ed0: 6272 0200 0000 7203 0000 0072 0400 0000  br....r....r....
-00002ee0: 720f 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00002ef0: 7210 0000 0072 1400 0000 725f 0000 0072  r....r....r_...r
-00002f00: 7d00 0000 720d 0000 0072 0d00 0000 720d  }...r....r....r.
-00002f10: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00002f20: 653e 1b00 0000 731a 0000 0008 0108 0108  e>....s.........
-00002f30: 0108 0108 0108 010c 010c 010c 0a08 1410  ................
-00002f40: 040e 6810 5e                             ..h.^
+00000060: 6401 6c06 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
+00000070: 0100 6400 6403 6c02 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6404 6c04 6d0b 5a0b 0100 650c 650c 6405  d.l.m.Z...e.e.d.
+00000090: 9c02 6406 6407 8404 5a0d 4700 6408 6409  ..d.d...Z.G.d.d.
+000000a0: 8400 6409 650e 8303 5a0f 4700 640a 640b  ..d.e...Z.G.d.d.
+000000b0: 8400 640b 8302 5a10 4700 640c 640d 8400  ..d...Z.G.d.d...
+000000c0: 640d 6510 8303 5a11 4700 640e 640f 8400  d.e...Z.G.d.d...
+000000d0: 640f 6510 8303 5a12 6401 5300 2910 e900  d.e...Z.d.S.)...
+000000e0: 0000 004e 2901 da04 5061 7468 2901 da05  ...N)...Path)...
+000000f0: 7768 6963 6829 01da 0f53 7562 7072 6f63  which)...Subproc
+00000100: 6573 7345 7272 6f72 2902 da03 6578 65da  essError)...exe.
+00000110: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+00000120: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000130: 7376 0000 0074 007c 0083 017d 017c 0173  sv...t.|...}.|.s
+00000140: 6a74 016a 02a0 037c 00a1 0172 3274 01a0  jt.j...|...r2t..
+00000150: 047c 0074 016a 05a1 0272 3274 016a 02a0  .|.t.j...r2t.j..
+00000160: 067c 00a1 0153 0074 016a 02a0 037c 00a1  .|...S.t.j...|..
+00000170: 0172 5c74 01a0 047c 0074 016a 05a1 0273  .r\t...|.t.j...s
+00000180: 5c74 0764 017c 009b 0064 029d 0383 0182  \t.d.|...d......
+00000190: 0174 0864 037c 009b 009d 0283 0182 0174  .t.d.|.........t
+000001a0: 016a 02a0 067c 01a1 0153 0029 047a ed54  .j...|...S.).z.T
+000001b0: 616b 6573 2061 6e20 6578 6563 7574 6162  akes an executab
+000001c0: 6c65 2061 6e64 2072 6574 7572 6e73 2074  le and returns t
+000001d0: 6865 2066 756c 6c20 7061 7468 2074 6f20  he full path to 
+000001e0: 7468 6174 2065 7865 6375 7461 626c 650a  that executable.
+000001f0: 0a20 2020 203a 7061 7261 6d20 6578 653a  .    :param exe:
+00000200: 2065 7865 6375 7461 626c 6520 6f72 2066   executable or f
+00000210: 696c 650a 2020 2020 3a74 7970 6520 6578  ile.    :type ex
+00000220: 653a 2073 7472 0a20 2020 203a 7261 6973  e: str.    :rais
+00000230: 6573 2054 7970 6545 7272 6f72 3a20 6966  es TypeError: if
+00000240: 2066 696c 6520 6973 206e 6f74 2061 6e20   file is not an 
+00000250: 6578 6563 7574 6162 6c65 0a20 2020 203a  executable.    :
+00000260: 7261 6973 6573 2046 696c 654e 6f74 466f  raises FileNotFo
+00000270: 756e 6445 7272 6f72 3a20 6966 2065 7865  undError: if exe
+00000280: 6375 7461 626c 6520 6361 6e6e 6f74 2062  cutable cannot b
+00000290: 6520 666f 756e 640a 2020 2020 7a06 4669  e found.    z.Fi
+000002a0: 6c65 2c20 7a16 2c20 6973 206e 6f74 2061  le, z., is not a
+000002b0: 6e20 6578 6563 7574 6162 6c65 7a1c 436f  n executablez.Co
+000002c0: 756c 6420 6e6f 7420 6c6f 6361 7465 2065  uld not locate e
+000002d0: 7865 6375 7461 626c 6520 2909 7203 0000  xecutable ).r...
+000002e0: 00da 026f 73da 0470 6174 68da 0669 7366  ...os..path..isf
+000002f0: 696c 65da 0661 6363 6573 73da 0458 5f4f  ile..access..X_O
+00000300: 4bda 0761 6273 7061 7468 da09 5479 7065  K..abspath..Type
+00000310: 4572 726f 72da 1146 696c 654e 6f74 466f  Error..FileNotFo
+00000320: 756e 6445 7272 6f72 2902 7205 0000 005a  undError).r....Z
+00000330: 0769 6e5f 7061 7468 a900 720f 0000 00fa  .in_path..r.....
+00000340: 462f 686f 6d65 2f72 756e 6e65 722f 776f  F/home/runner/wo
+00000350: 726b 2f53 6d61 7274 5369 6d2f 536d 6172  rk/SmartSim/Smar
+00000360: 7453 696d 2f73 6d61 7274 7369 6d2f 5f63  tSim/smartsim/_c
+00000370: 6f72 652f 5f69 6e73 7461 6c6c 2f62 7569  ore/_install/bui
+00000380: 6c64 6572 2e70 79da 0f65 7870 616e 645f  lder.py..expand_
+00000390: 6578 655f 7061 7468 2e00 0000 7310 0000  exe_path....s...
+000003a0: 0000 0a08 0104 011a 010c 011a 0110 010e  ................
+000003b0: 0172 1100 0000 6300 0000 0000 0000 0000  .r....c.........
+000003c0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+000003d0: 0c00 0000 6500 5a01 6400 5a02 6401 5300  ....e.Z.d.Z.d.S.
+000003e0: 2902 da0a 4275 696c 6445 7272 6f72 4e29  )...BuildErrorN)
+000003f0: 03da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000400: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000410: 616d 655f 5f72 0f00 0000 720f 0000 0072  ame__r....r....r
+00000420: 0f00 0000 7210 0000 0072 1200 0000 4200  ....r....r....B.
+00000430: 0000 7302 0000 0008 0172 1200 0000 6300  ..s......r....c.
+00000440: 0000 0000 0000 0000 0000 0000 0000 0008  ................
+00000450: 0000 0040 0000 0073 2001 0000 6500 5a01  ...@...s ...e.Z.
+00000460: 6400 5a02 6401 5a03 6504 a005 6402 6504  d.Z.d.Z.e...d.e.
+00000470: 6a06 a102 5a07 6420 6508 6a09 650a 6508  j...Z.d e.j.e.e.
+00000480: 6a0b 6602 1900 6508 6a0c 650d 1900 650e  j.f...e.j.e...e.
+00000490: 6405 6406 9c04 6407 6408 8405 5a0f 6510  d.d...d.d...Z.e.
+000004a0: 650e 6409 9c01 640a 640b 8404 8301 5a11  e.d...d.d.....Z.
+000004b0: 6421 650a 650a 650a 6405 640d 9c04 640e  d!e.e.e.d.d...d.
+000004c0: 640f 8405 5a12 650a 650a 6410 9c02 6411  d...Z.e.e.d...d.
+000004d0: 6412 8404 5a13 6422 6508 6a14 650a 6515  d...Z.d"e.j.e.e.
+000004e0: 6602 1900 6508 6a14 650a 6515 6602 1900  f...e.j.e.e.f...
+000004f0: 650e 6405 6413 9c04 6414 6415 8405 5a16  e.d.d...d.d...Z.
+00000500: 6423 6508 6a14 650a 6515 6602 1900 6508  d#e.j.e.e.f...e.
+00000510: 6a14 650a 6515 6602 1900 650e 6405 6413  j.e.e.f...e.d.d.
+00000520: 9c04 6416 6417 8405 5a17 650a 650e 6418  ..d.d...Z.e.e.d.
+00000530: 9c02 6419 641a 8404 5a18 6405 6409 9c01  ..d.d...Z.d.d...
+00000540: 641b 641c 8404 5a19 6424 6508 6a1a 650a  d.d...Z.d$e.j.e.
+00000550: 1900 650e 6508 6a0c 650d 1900 6508 6a14  ..e.e.j.e...e.j.
+00000560: 650a 6515 6405 6603 1900 6405 641d 9c05  e.e.d.f...d.d...
+00000570: 641e 641f 8405 5a1b 6405 5300 2925 da07  d.d...Z.d.S.)%..
+00000580: 4275 696c 6465 727a 2d42 6173 6520 636c  Builderz-Base cl
+00000590: 6173 7320 666f 7220 6275 696c 6469 6e67  ass for building
+000005a0: 2074 6869 7264 2d70 6172 7479 206c 6962   third-party lib
+000005b0: 7261 7269 6573 7aa8 5e28 3f3a 6874 7470  rariesz.^(?:http
+000005c0: 7c66 7470 2973 3f3a 2f2f 283f 3a28 3f3a  |ftp)s?://(?:(?:
+000005d0: 5b41 2d5a 302d 395d 283f 3a5b 412d 5a30  [A-Z0-9](?:[A-Z0
+000005e0: 2d39 2d5d 7b30 2c36 317d 5b41 2d5a 302d  -9-]{0,61}[A-Z0-
+000005f0: 395d 293f 5c2e 292b 283f 3a5b 412d 5a5d  9])?\.)+(?:[A-Z]
+00000600: 7b32 2c36 7d5c 2e3f 7c5b 412d 5a30 2d39  {2,6}\.?|[A-Z0-9
+00000610: 2d5d 7b32 2c7d 5c2e 3f29 7c6c 6f63 616c  -]{2,}\.?)|local
+00000620: 686f 7374 7c5c 647b 312c 337d 5c2e 5c64  host|\d{1,3}\.\d
+00000630: 7b31 2c33 7d5c 2e5c 647b 312c 337d 5c2e  {1,3}\.\d{1,3}\.
+00000640: 5c64 7b31 2c33 7d29 283f 3a3a 5c64 2b29  \d{1,3})(?::\d+)
+00000650: 3f28 3f3a 2f3f 7c5b 2f3f 5d5c 532b 2924  ?(?:/?|[/?]\S+)$
+00000660: e901 0000 0046 4e29 04da 0365 6e76 da04  .....FN)...env..
+00000670: 6a6f 6273 da07 7665 7262 6f73 6572 0600  jobs..verboser..
+00000680: 0000 6304 0000 0000 0000 0000 0000 0006  ..c.............
+00000690: 0000 0004 0000 0043 0000 0073 bc00 0000  .......C...s....
+000006a0: 7c01 7c00 5f00 7401 7402 6a03 a004 7405  |.|._.t.t.j...t.
+000006b0: a101 8301 6a06 6a06 7d04 7c04 7d05 7402  ....j.j.}.|.}.t.
+000006c0: a007 6401 a101 7236 7401 7402 6a08 6401  ..d...r6t.t.j.d.
+000006d0: 1900 8301 7d05 7c04 6402 1b00 7c00 5f09  ....}.|.d...|._.
+000006e0: 7c05 6403 1b00 7c00 5f0a 7c05 6404 1b00  |.d...|._.|.d...
+000006f0: 7c00 5f0b 740c 6a0d 7c00 5f0e 7c03 7c00  |._.t.j.|._.|.|.
+00000700: 5f0f 7c00 6a0f 726e 6400 7c00 5f0e 7c00  _.|.j.rnd.|._.|.
+00000710: 6a09 a010 a100 7382 7c00 6a09 a011 a100  j.....s.|.j.....
+00000720: 0100 7c05 7c04 6b02 72b2 7c00 6a0a a010  ..|.|.k.r.|.j...
+00000730: a100 739e 7c00 6a0a a011 a100 0100 7c00  ..s.|.j.......|.
+00000740: 6a0b a010 a100 73b2 7c00 6a0b a011 a100  j.....s.|.j.....
+00000750: 0100 7c02 7c00 5f12 6400 5300 2905 4e5a  ..|.|._.d.S.).NZ
+00000760: 1153 4d41 5254 5349 4d5f 4445 505f 5041  .SMARTSIM_DEP_PA
+00000770: 5448 7a0c 2e74 6869 7264 2d70 6172 7479  THz..third-party
+00000780: da03 6269 6eda 036c 6962 2913 7218 0000  ..bin..lib).r...
+00000790: 0072 0200 0000 7207 0000 0072 0800 0000  .r....r....r....
+000007a0: 720c 0000 00da 085f 5f66 696c 655f 5fda  r......__file__.
+000007b0: 0670 6172 656e 74da 0667 6574 656e 76da  .parent..getenv.
+000007c0: 0765 6e76 6972 6f6e da09 6275 696c 645f  .environ..build_
+000007d0: 6469 72da 0862 696e 5f70 6174 68da 086c  dir..bin_path..l
+000007e0: 6962 5f70 6174 68da 0a73 7562 7072 6f63  ib_path..subproc
+000007f0: 6573 73da 0744 4556 4e55 4c4c da03 6f75  ess..DEVNULL..ou
+00000800: 7472 1a00 0000 da06 6973 5f64 6972 da05  tr......is_dir..
+00000810: 6d6b 6469 7272 1900 0000 2906 da04 7365  mkdirr....)...se
+00000820: 6c66 7218 0000 0072 1900 0000 721a 0000  lfr....r....r...
+00000830: 005a 095f 636f 7265 5f64 6972 da0f 6465  .Z._core_dir..de
+00000840: 7065 6e64 656e 6379 5f70 6174 6872 0f00  pendency_pathr..
+00000850: 0000 720f 0000 0072 1000 0000 da08 5f5f  ..r....r......__
+00000860: 696e 6974 5f5f 5300 0000 7328 0000 0000  init__S...s(....
+00000870: 0506 0314 0204 010a 010e 020a 020a 010a  ................
+00000880: 0308 0106 0106 0106 030a 010a 0108 010a  ................
+00000890: 010a 010a 010a 027a 1042 7569 6c64 6572  .......z.Builder
+000008a0: 2e5f 5f69 6e69 745f 5fa9 0172 0600 0000  .__init__..r....
+000008b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000008c0: 0001 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
+000008d0: 8201 6400 5300 a901 4ea9 01da 134e 6f74  ..d.S...N....Not
+000008e0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+000008f0: a901 7229 0000 0072 0f00 0000 720f 0000  ..r)...r....r...
+00000900: 0072 1000 0000 da08 6973 5f62 7569 6c74  .r......is_built
+00000910: 7800 0000 7302 0000 0000 027a 1042 7569  x...s......z.Bui
+00000920: 6c64 6572 2e69 735f 6275 696c 74da 0363  lder.is_built..c
+00000930: 7075 a904 da07 6769 745f 7572 6cda 0662  pu....git_url..b
+00000940: 7261 6e63 68da 0664 6576 6963 6572 0600  ranch..devicer..
+00000950: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
+00000960: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
+00000970: 7400 8201 6400 5300 722d 0000 0072 2e00  t...d.S.r-...r..
+00000980: 0000 2904 7229 0000 0072 3400 0000 7235  ..).r)...r4...r5
+00000990: 0000 0072 3600 0000 720f 0000 0072 0f00  ...r6...r....r..
+000009a0: 0000 7210 0000 00da 0e62 7569 6c64 5f66  ..r......build_f
+000009b0: 726f 6d5f 6769 747c 0000 0073 0200 0000  rom_git|...s....
+000009c0: 0001 7a16 4275 696c 6465 722e 6275 696c  ..z.Builder.buil
+000009d0: 645f 6672 6f6d 5f67 6974 2902 da06 6269  d_from_git)...bi
+000009e0: 6e61 7279 7206 0000 0063 0200 0000 0000  naryr....c......
+000009f0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00000a00: 0000 7324 0000 0074 00a0 017c 01a1 017d  ..s$...t...|...}
+00000a10: 027c 0272 127c 0253 0074 027c 019b 0064  .|.r.|.S.t.|...d
+00000a20: 019d 0283 0182 0164 0053 0029 024e 7a12  .......d.S.).Nz.
+00000a30: 206e 6f74 2066 6f75 6e64 2069 6e20 5041   not found in PA
+00000a40: 5448 2903 da06 7368 7574 696c 7203 0000  TH)...shutilr...
+00000a50: 0072 1200 0000 2903 7229 0000 0072 3800  .r....).r)...r8.
+00000a60: 0000 5a07 6269 6e61 7279 5f72 0f00 0000  ..Z.binary_r....
+00000a70: 720f 0000 0072 1000 0000 da0b 6269 6e61  r....r......bina
+00000a80: 7279 5f70 6174 687f 0000 0073 0800 0000  ry_path....s....
+00000a90: 0001 0a01 0401 0401 7a13 4275 696c 6465  ........z.Builde
+00000aa0: 722e 6269 6e61 7279 5f70 6174 6829 04da  r.binary_path)..
+00000ab0: 0373 7263 da03 6473 74da 0773 6574 5f65  .src..dst..set_e
+00000ac0: 7865 7206 0000 0063 0400 0000 0000 0000  xer....c........
+00000ad0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00000ae0: 7330 0000 0074 00a0 017c 017c 02a1 0201  s0...t...|.|....
+00000af0: 007c 0372 2c74 027c 0283 01a0 0374 046a  .|.r,t.|.....t.j
+00000b00: 0574 046a 0642 0074 046a 0742 00a1 0101  .t.j.B.t.j.B....
+00000b10: 0064 0053 0072 2d00 0000 2908 7239 0000  .d.S.r-...).r9..
+00000b20: 00da 0863 6f70 7966 696c 6572 0200 0000  ...copyfiler....
+00000b30: da05 6368 6d6f 64da 0473 7461 74da 0753  ..chmod..stat..S
+00000b40: 5f49 5855 5352 da07 535f 4957 5553 52da  _IXUSR..S_IWUSR.
+00000b50: 0753 5f49 5255 5352 2904 7229 0000 0072  .S_IRUSR).r)...r
+00000b60: 3b00 0000 723c 0000 0072 3d00 0000 720f  ;...r<...r=...r.
+00000b70: 0000 0072 0f00 0000 7210 0000 00da 0963  ...r....r......c
+00000b80: 6f70 795f 6669 6c65 8500 0000 7306 0000  opy_file....s...
+00000b90: 0000 010c 0104 017a 1142 7569 6c64 6572  .......z.Builder
+00000ba0: 2e63 6f70 795f 6669 6c65 6304 0000 0000  .copy_filec.....
+00000bb0: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
+00000bc0: 0000 0073 6600 0000 7400 7c01 8301 7d01  ...sf...t.|...}.
+00000bd0: 7400 7c02 8301 7d02 7c02 6a01 6401 6402  t.|...}.|.j.d.d.
+00000be0: 8d01 0100 7c01 a002 6403 a101 4400 5d3a  ....|...d...D.]:
+00000bf0: 7d04 7c04 a003 a100 724a 7c00 6a04 7c04  }.|.....rJ|.j.|.
+00000c00: 7c02 7c04 6a05 1b00 7c03 6404 8d03 0100  |.|.j...|.d.....
+00000c10: 7126 7c00 6a06 7c04 7c02 7c04 6a05 1b00  q&|.j.|.|.|.j...
+00000c20: 7c03 6404 8d03 0100 7126 6400 5300 2905  |.d.....q&d.S.).
+00000c30: 4e54 2901 da08 6578 6973 745f 6f6b da01  NT)...exist_ok..
+00000c40: 2aa9 0172 3d00 0000 2907 7202 0000 0072  *..r=...).r....r
+00000c50: 2800 0000 da04 676c 6f62 7227 0000 00da  (.....globr'....
+00000c60: 0863 6f70 795f 6469 72da 046e 616d 6572  .copy_dir..namer
+00000c70: 4400 0000 2905 7229 0000 0072 3b00 0000  D...).r)...r;...
+00000c80: 723c 0000 0072 3d00 0000 da07 636f 6e74  r<...r=.....cont
+00000c90: 656e 7472 0f00 0000 720f 0000 0072 1000  entr....r....r..
+00000ca0: 0000 7249 0000 008a 0000 0073 0e00 0000  ..rI.......s....
+00000cb0: 0001 0801 0801 0c02 0e01 0801 1802 7a10  ..............z.
+00000cc0: 4275 696c 6465 722e 636f 7079 5f64 6972  Builder.copy_dir
+00000cd0: 2902 da03 7572 6c72 0600 0000 6302 0000  )...urlr....c...
+00000ce0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000cf0: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
+00000d00: 6a02 7c01 a102 6400 6b09 5300 722d 0000  j.|...d.k.S.r-..
+00000d10: 0029 03da 0272 65da 056d 6174 6368 da09  .)...re..match..
+00000d20: 7572 6c5f 7265 6765 7829 0272 2900 0000  url_regex).r)...
+00000d30: 724c 0000 0072 0f00 0000 720f 0000 0072  rL...r....r....r
+00000d40: 1000 0000 da0c 6973 5f76 616c 6964 5f75  ......is_valid_u
+00000d50: 726c 9500 0000 7302 0000 0000 017a 1442  rl....s......z.B
+00000d60: 7569 6c64 6572 2e69 735f 7661 6c69 645f  uilder.is_valid_
+00000d70: 7572 6c63 0100 0000 0000 0000 0000 0000  urlc............
+00000d80: 0100 0000 0400 0000 4300 0000 731e 0000  ........C...s...
+00000d90: 007c 006a 00a0 01a1 0072 1a74 02a0 0374  .|.j.....r.t...t
+00000da0: 047c 006a 0083 01a1 0101 0064 0053 0072  .|.j.......d.S.r
+00000db0: 2d00 0000 2905 7221 0000 0072 2700 0000  -...).r!...r'...
+00000dc0: 7239 0000 00da 0672 6d74 7265 65da 0373  r9.....rmtree..s
+00000dd0: 7472 7230 0000 0072 0f00 0000 720f 0000  trr0...r....r...
+00000de0: 0072 1000 0000 da07 636c 6561 6e75 7098  .r......cleanup.
+00000df0: 0000 0073 0400 0000 0001 0a01 7a0f 4275  ...s........z.Bu
+00000e00: 696c 6465 722e 636c 6561 6e75 7029 05da  ilder.cleanup)..
+00000e10: 0363 6d64 da05 7368 656c 6c72 2600 0000  .cmd..shellr&...
+00000e20: da03 6377 6472 0600 0000 6305 0000 0000  ..cwdr....c.....
+00000e30: 0000 0000 0000 0008 0000 000a 0000 0043  ...............C
+00000e40: 0000 0073 8000 0000 7c03 730a 7c00 6a00  ...s....|.s.|.j.
+00000e50: 7d03 7a42 7401 6a02 7c01 7401 6a03 7c03  }.zBt.j.|.t.j.|.
+00000e60: 7c04 7c02 7c00 6a04 6401 8d06 7d05 7c05  |.|.|.j.d...}.|.
+00000e70: a005 a100 6402 1900 a006 6403 a101 7d06  ....d.....d...}.
+00000e80: 7c05 6a07 6404 6b03 724a 7408 7c06 8301  |.j.d.k.rJt.|...
+00000e90: 8201 5700 6e2e 0400 7409 740a 6602 6b0a  ..W.n...t.t.f.k.
+00000ea0: 727a 0100 7d07 0100 7a0c 7408 7c07 8301  rz..}...z.t.|...
+00000eb0: 8201 5700 3500 6400 7d07 7e07 5800 5900  ..W.5.d.}.~.X.Y.
+00000ec0: 6e02 5800 6400 5300 2905 4e29 05da 0673  n.X.d.S.).N)...s
+00000ed0: 7464 6572 72da 0673 7464 6f75 7472 5600  tderr..stdoutrV.
+00000ee0: 0000 7255 0000 0072 1800 0000 7217 0000  ..rU...r....r...
+00000ef0: 007a 0575 7466 2d38 7201 0000 0029 0b72  .z.utf-8r....).r
+00000f00: 2600 0000 7224 0000 00da 0550 6f70 656e  &...r$.....Popen
+00000f10: da04 5049 5045 7218 0000 00da 0b63 6f6d  ..PIPEr......com
+00000f20: 6d75 6e69 6361 7465 da06 6465 636f 6465  municate..decode
+00000f30: da0a 7265 7475 726e 636f 6465 7212 0000  ..returncoder...
+00000f40: 00da 074f 5345 7272 6f72 7204 0000 0029  ...OSErrorr....)
+00000f50: 0872 2900 0000 7254 0000 0072 5500 0000  .r)...rT...rU...
+00000f60: 7226 0000 0072 5600 0000 da04 7072 6f63  r&...rV.....proc
+00000f70: da05 6572 726f 72da 0165 720f 0000 0072  ..error..er....r
+00000f80: 0f00 0000 7210 0000 00da 0b72 756e 5f63  ....r......run_c
+00000f90: 6f6d 6d61 6e64 9c00 0000 7320 0000 0000  ommand....s ....
+00000fa0: 0604 0106 0102 0104 0102 0104 0102 0102  ................
+00000fb0: 0102 0104 fa06 0812 010a 010c 0114 017a  ...............z
+00000fc0: 1342 7569 6c64 6572 2e72 756e 5f63 6f6d  .Builder.run_com
+00000fd0: 6d61 6e64 2902 7217 0000 0046 2901 7232  mand).r....F).r2
+00000fe0: 0000 0029 0146 2901 4629 0346 4e4e 291c  ...).F).F).FNN).
+00000ff0: 7213 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00001000: 075f 5f64 6f63 5f5f 724d 0000 00da 0763  .__doc__rM.....c
+00001010: 6f6d 7069 6c65 da0a 4947 4e4f 5245 4341  ompile..IGNORECA
+00001020: 5345 724f 0000 00da 0174 da04 4469 6374  SErO.....t..Dict
+00001030: 7252 0000 00da 0341 6e79 da08 4f70 7469  rR.....Any..Opti
+00001040: 6f6e 616c da03 696e 74da 0462 6f6f 6c72  onal..int..boolr
+00001050: 2b00 0000 da08 7072 6f70 6572 7479 7231  +.....propertyr1
+00001060: 0000 0072 3700 0000 723a 0000 00da 0555  ...r7...r:.....U
+00001070: 6e69 6f6e 7202 0000 0072 4400 0000 7249  nionr....rD...rI
+00001080: 0000 0072 5000 0000 7253 0000 00da 044c  ...rP...rS.....L
+00001090: 6973 7472 6200 0000 720f 0000 0072 0f00  istrb...r....r..
+000010a0: 0000 720f 0000 0072 1000 0000 7216 0000  ..r....r....r...
+000010b0: 0046 0000 0073 3e00 0000 0801 0402 0401  .F...s>.........
+000010c0: 0206 04f9 040c 0001 00fd 0201 0e01 0801  ................
+000010d0: 0200 02fd 0c25 0201 1003 1603 1006 2a05  .....%........*.
+000010e0: 2a0b 1003 0e06 0001 0001 00fc 0201 0801  *...............
+000010f0: 0201 0801 0e00 02fc 7216 0000 0063 0000  ........r....c..
+00001100: 0000 0000 0000 0000 0000 0000 0000 0700  ................
+00001110: 0000 0000 0000 7372 0000 0065 005a 0164  ......sr...e.Z.d
+00001120: 005a 0264 015a 0369 0064 0264 0364 0466  .Z.d.Z.i.d.d.d.f
+00001130: 0465 046a 0565 0665 046a 0766 0219 0065  .e.j.e.e.j.f...e
+00001140: 0665 046a 0865 0919 0065 0a64 0364 059c  .e.j.e...e.d.d..
+00001150: 0587 0066 0164 0664 0784 0d5a 0b65 0c65  ...f.d.d...Z.e.e
+00001160: 0a64 089c 0164 0964 0a84 0483 015a 0d64  .d...d.d.....Z.d
+00001170: 0f65 0665 0665 0664 0364 0c9c 0464 0d64  .e.e.e.d.d...d.d
+00001180: 0e84 055a 0e87 0004 005a 0f53 0029 10da  ...Z.....Z.S.)..
+00001190: 0f44 6174 6162 6173 6542 7569 6c64 6572  .DatabaseBuilder
+000011a0: 7aaf 436c 6173 7320 746f 2062 7569 6c64  z.Class to build
+000011b0: 2052 6564 6973 206f 7220 4b65 7944 4220   Redis or KeyDB 
+000011c0: 6672 6f6d 2053 6f75 7263 650a 2020 2020  from Source.    
+000011d0: 5375 7070 6f72 7465 6420 6275 696c 6420  Supported build 
+000011e0: 6d65 7468 6f64 733a 0a20 2020 2020 2d20  methods:.     - 
+000011f0: 6672 6f6d 2067 6974 0a20 2020 2053 6565  from git.    See
+00001200: 2062 7569 6c64 656e 762e 7079 2066 6f72   buildenv.py for
+00001210: 2062 7569 6c64 7469 6d65 2063 6f6e 6669   buildtime confi
+00001220: 6775 7261 7469 6f6e 206f 6620 5265 6469  guration of Redi
+00001230: 732f 4b65 7944 420a 2020 2020 7665 7273  s/KeyDB.    vers
+00001240: 696f 6e20 616e 6420 7572 6c2e 0a20 2020  ion and url..   
+00001250: 20da 046c 6962 634e 4629 05da 0962 7569   ..libcNF)...bui
+00001260: 6c64 5f65 6e76 da06 6d61 6c6c 6f63 7219  ld_env..mallocr.
+00001270: 0000 0072 1a00 0000 7206 0000 0063 0500  ...r....r....c..
+00001280: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00001290: 0000 0300 0000 731c 0000 0074 0083 006a  ......s....t...j
+000012a0: 017c 017c 037c 0464 018d 0301 007c 027c  .|.|.|.d.....|.|
+000012b0: 005f 0264 0053 0029 024e a902 7219 0000  ._.d.S.).N..r...
+000012c0: 0072 1a00 0000 2903 da05 7375 7065 7272  .r....)...superr
+000012d0: 2b00 0000 7272 0000 0029 0572 2900 0000  +...rr...).r)...
+000012e0: 7271 0000 0072 7200 0000 7219 0000 0072  rq...rr...r....r
+000012f0: 1a00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00001300: 5f72 0f00 0000 7210 0000 0072 2b00 0000  _r....r....r+...
+00001310: bc00 0000 7304 0000 0000 0512 017a 1844  ....s........z.D
+00001320: 6174 6162 6173 6542 7569 6c64 6572 2e5f  atabaseBuilder._
+00001330: 5f69 6e69 745f 5f72 2c00 0000 6301 0000  _init__r,...c...
+00001340: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00001350: 0043 0000 0073 3800 0000 6401 6402 8400  .C...s8...d.d...
+00001360: 7c00 6a00 a001 a100 4400 8301 7d01 6403  |.j.....D...}.d.
+00001370: 6404 6802 7d02 6405 6406 6802 7d03 7c02  d.h.}.d.d.h.}.|.
+00001380: a002 7c01 a101 7036 7c03 a002 7c01 a101  ..|...p6|...|...
+00001390: 5300 2907 7a20 4368 6563 6b20 6966 2052  S.).z Check if R
+000013a0: 6564 6973 206f 7220 4b65 7944 4220 6973  edis or KeyDB is
+000013b0: 2062 7569 6c74 6301 0000 0000 0000 0000   builtc.........
+000013c0: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+000013d0: 1200 0000 6800 7c00 5d0a 7d01 7c01 6a00  ....h.|.].}.|.j.
+000013e0: 9202 7104 5300 720f 0000 0029 0172 4a00  ..q.S.r....).rJ.
+000013f0: 0000 2902 da02 2e30 da04 6669 6c65 720f  ..)....0..filer.
+00001400: 0000 0072 0f00 0000 7210 0000 00da 093c  ...r....r......<
+00001410: 7365 7463 6f6d 703e c700 0000 7304 0000  setcomp>....s...
+00001420: 0006 0002 007a 2b44 6174 6162 6173 6542  .....z+DatabaseB
+00001430: 7569 6c64 6572 2e69 735f 6275 696c 742e  uilder.is_built.
+00001440: 3c6c 6f63 616c 733e 2e3c 7365 7463 6f6d  <locals>.<setcom
+00001450: 703e 7a0c 7265 6469 732d 7365 7276 6572  p>z.redis-server
+00001460: 7a09 7265 6469 732d 636c 697a 0c6b 6579  z.redis-cliz.key
+00001470: 6462 2d73 6572 7665 727a 096b 6579 6462  db-serverz.keydb
+00001480: 2d63 6c69 2903 7222 0000 00da 0769 7465  -cli).r".....ite
+00001490: 7264 6972 da08 6973 7375 6273 6574 2904  rdir..issubset).
+000014a0: 7229 0000 005a 0962 696e 5f66 696c 6573  r)...Z.bin_files
+000014b0: 5a0b 7265 6469 735f 6669 6c65 735a 0b6b  Z.redis_filesZ.k
+000014c0: 6579 6462 5f66 696c 6573 720f 0000 0072  eydb_filesr....r
+000014d0: 0f00 0000 7210 0000 0072 3100 0000 c400  ....r....r1.....
+000014e0: 0000 7308 0000 0000 0314 0108 0108 017a  ..s............z
+000014f0: 1844 6174 6162 6173 6542 7569 6c64 6572  .DatabaseBuilder
+00001500: 2e69 735f 6275 696c 7472 3200 0000 7233  .is_builtr2...r3
+00001510: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00001520: 1800 0000 0a00 0000 4300 0000 734e 0200  ........C...sN..
+00001530: 0064 017c 016b 0672 0c64 026e 0264 037d  .d.|.k.r.d.n.d.}
+00001540: 0474 007c 006a 017c 04a0 02a1 0083 027d  .t.|.j.|.......}
+00001550: 0574 007c 006a 0164 0383 027d 0674 007c  .t.|.j.d...}.t.|
+00001560: 006a 0164 0283 027d 077c 06a0 03a1 0072  .j.d...}.|.....r
+00001570: 4e74 04a0 0574 067c 0683 01a1 0101 007c  Nt...t.|.......|
+00001580: 07a0 03a1 0072 6474 04a0 0574 067c 0783  .....rdt...t.|..
+00001590: 01a1 0101 007c 00a0 077c 01a1 0173 8274  .....|...|...s.t
+000015a0: 0864 047c 049b 0064 057c 019b 009d 0483  .d.|...d.|......
+000015b0: 0182 017c 00a0 0964 06a1 0164 077c 0164  ...|...d...d.|.d
+000015c0: 087c 0264 0964 0a7c 0467 087d 087c 006a  .|.d.d.|.g.}.|.j
+000015d0: 0a7c 087c 006a 0164 0b8d 0201 007c 00a0  .|.|.j.d.....|..
+000015e0: 0964 0ca1 0164 0d74 067c 006a 0b83 0164  .d...d.t.|.j...d
+000015f0: 0e7c 006a 0c9b 009d 0267 047d 097c 006a  .|.j.....g.}.|.j
+00001600: 0a7c 0974 067c 0583 0164 0b8d 0201 007c  .|.t.|...d.....|
+00001610: 0564 0f1b 007d 0a7c 0a7c 04a0 02a1 0064  .d...}.|.|.....d
+00001620: 1017 001b 007d 0b7c 006a 0d7c 04a0 02a1  .....}.|.j.|....
+00001630: 0064 1017 001b 007d 0c7c 0a7c 04a0 02a1  .d.....}.|.|....
+00001640: 0064 1117 001b 007d 0d7c 006a 0d7c 04a0  .d.....}.|.j.|..
+00001650: 02a1 0064 1117 001b 007d 0e7c 006a 0e7c  ...d.....}.|.j.|
+00001660: 0b7c 0c64 1264 138d 0301 007c 006a 0e7c  .|.d.d.....|.j.|
+00001670: 0d7c 0e64 1264 138d 0301 0074 0074 0f6a  .|.d.d.....t.t.j
+00001680: 10a0 1174 12a1 0183 016a 136a 137d 0f74  ...t.....j.j.}.t
+00001690: 0f6a 14a0 1564 147c 0fa1 027d 1074 007c  .j...d.|...}.t.|
+000016a0: 1064 1583 02a0 16a1 007d 117a 3474 177c  .d.......}.z4t.|
+000016b0: 11a0 1864 16a1 0183 017d 1274 0074 0f6a  ...d.....}.t.t.j
+000016c0: 14a0 1564 177c 12a1 0283 01a0 16a1 007d  ...d.|.........}
+000016d0: 1374 1974 067c 1383 0183 017d 1457 006e  .t.t.|.....}.W.n
+000016e0: 3204 0074 1a74 1b66 026b 0a90 0172 e001  2..t.t.f.k...r..
+000016f0: 007d 1501 007a 0e74 0864 1883 017c 1582  .}...z.t.d...|..
+00001700: 0257 0035 0064 197d 157e 1558 0059 006e  .W.5.d.}.~.X.Y.n
+00001710: 0258 007a 3474 177c 11a0 1864 1aa1 0183  .X.z4t.|...d....
+00001720: 017d 1674 0074 0f6a 14a0 1564 1b7c 16a1  .}.t.t.j...d.|..
+00001730: 0283 01a0 16a1 007d 1774 1974 067c 1783  .......}.t.t.|..
+00001740: 0183 017d 1457 006e 3204 0074 1a74 1b66  ...}.W.n2..t.t.f
+00001750: 026b 0a90 0272 4801 007d 1501 007a 0e74  .k...rH..}...z.t
+00001760: 0864 1c83 017c 1582 0257 0035 0064 197d  .d...|...W.5.d.}
+00001770: 157e 1558 0059 006e 0258 0064 1953 0029  .~.X.Y.n.X.d.S.)
+00001780: 1d7a b542 7569 6c64 2052 6564 6973 2066  .z.Build Redis f
+00001790: 726f 6d20 6769 740a 2020 2020 2020 2020  rom git.        
+000017a0: 3a70 6172 616d 2067 6974 5f75 726c 3a20  :param git_url: 
+000017b0: 7572 6c20 6672 6f6d 2077 6869 6368 2074  url from which t
+000017c0: 6f20 7265 7472 6965 7665 2052 6564 6973  o retrieve Redis
+000017d0: 0a20 2020 2020 2020 203a 7479 7065 2067  .        :type g
+000017e0: 6974 5f75 726c 3a20 7374 720a 2020 2020  it_url: str.    
+000017f0: 2020 2020 3a70 6172 616d 2062 7261 6e63      :param branc
+00001800: 683a 2062 7261 6e63 6820 746f 2063 6865  h: branch to che
+00001810: 636b 6f75 740a 2020 2020 2020 2020 3a74  ckout.        :t
+00001820: 7970 6520 6272 616e 6368 3a20 7374 720a  ype branch: str.
+00001830: 2020 2020 2020 2020 5a05 4b65 7944 425a          Z.KeyDBZ
+00001840: 056b 6579 6462 5a05 7265 6469 737a 0a4d  .keydbZ.redisz.M
+00001850: 616c 666f 726d 6564 207a 0620 5552 4c3a  alformed z. URL:
+00001860: 20da 0367 6974 da05 636c 6f6e 65fa 082d   ..git..clone..-
+00001870: 2d62 7261 6e63 687a 072d 2d64 6570 7468  -branchz.--depth
+00001880: da01 31a9 0172 5600 0000 da04 6d61 6b65  ..1..rV.....make
+00001890: fa02 2d6a 7a07 4d41 4c4c 4f43 3d72 3b00  ..-jz.MALLOC=r;.
+000018a0: 0000 7a07 2d73 6572 7665 727a 042d 636c  ..z.-serverz.-cl
+000018b0: 6954 7247 0000 005a 1953 4d41 5254 5349  iTrG...Z.SMARTSI
+000018c0: 4d5f 4445 505f 494e 5354 414c 4c5f 5041  M_DEP_INSTALL_PA
+000018d0: 5448 721b 0000 007a 082a 2d73 6572 7665  THr....z.*-serve
+000018e0: 725a 0a52 4544 4953 5f50 4154 487a 2449  rZ.REDIS_PATHz$I
+000018f0: 6e73 7461 6c6c 6174 696f 6e20 6f66 2072  nstallation of r
+00001900: 6564 6973 2d73 6572 7665 7220 6661 696c  edis-server fail
+00001910: 6564 214e 7a05 2a2d 636c 695a 0e52 4544  ed!Nz.*-cliZ.RED
+00001920: 4953 5f43 4c49 5f50 4154 487a 2149 6e73  IS_CLI_PATHz!Ins
+00001930: 7461 6c6c 6174 696f 6e20 6f66 2072 6564  tallation of red
+00001940: 6973 2d63 6c69 2066 6169 6c65 6421 291c  is-cli failed!).
+00001950: 7202 0000 0072 2100 0000 da05 6c6f 7765  r....r!.....lowe
+00001960: 7272 2700 0000 7239 0000 0072 5100 0000  rr'...r9...rQ...
+00001970: 7252 0000 0072 5000 0000 7212 0000 0072  rR...rP...r....r
+00001980: 3a00 0000 7262 0000 0072 1900 0000 7272  :...rb...r....rr
+00001990: 0000 0072 2200 0000 7244 0000 0072 0700  ...r"...rD...r..
+000019a0: 0000 7208 0000 0072 0c00 0000 721d 0000  ..r....r....r...
+000019b0: 0072 1e00 0000 7220 0000 00da 0367 6574  .r....r .....get
+000019c0: da07 7265 736f 6c76 65da 046e 6578 7472  ..resolve..nextr
+000019d0: 4800 0000 7211 0000 0072 0d00 0000 720e  H...r....r....r.
+000019e0: 0000 0029 1872 2900 0000 7234 0000 0072  ...).r)...r4...r
+000019f0: 3500 0000 7236 0000 005a 0d64 6174 6162  5...r6...Z.datab
+00001a00: 6173 655f 6e61 6d65 5a13 6461 7461 6261  ase_nameZ.databa
+00001a10: 7365 5f62 7569 6c64 5f70 6174 685a 1072  se_build_pathZ.r
+00001a20: 6564 6973 5f62 7569 6c64 5f70 6174 685a  edis_build_pathZ
+00001a30: 106b 6579 6462 5f62 7569 6c64 5f70 6174  .keydb_build_pat
+00001a40: 68da 0963 6c6f 6e65 5f63 6d64 da09 6275  h..clone_cmd..bu
+00001a50: 696c 645f 636d 645a 1064 6174 6162 6173  ild_cmdZ.databas
+00001a60: 655f 7372 635f 6469 725a 0d73 6572 7665  e_src_dirZ.serve
+00001a70: 725f 736f 7572 6365 5a12 7365 7276 6572  r_sourceZ.server
+00001a80: 5f64 6573 7469 6e61 7469 6f6e 5a0a 636c  _destinationZ.cl
+00001a90: 695f 736f 7572 6365 5a0f 636c 695f 6465  i_sourceZ.cli_de
+00001aa0: 7374 696e 6174 696f 6e5a 0963 6f72 655f  stinationZ.core_
+00001ab0: 7061 7468 722a 0000 0072 2200 0000 5a0c  pathr*...r"...Z.
+00001ac0: 6461 7461 6261 7365 5f65 7865 5a08 6461  database_exeZ.da
+00001ad0: 7461 6261 7365 da01 5f72 6100 0000 5a0d  tabase.._ra...Z.
+00001ae0: 7265 6469 735f 636c 695f 6578 655a 0972  redis_cli_exeZ.r
+00001af0: 6564 6973 5f63 6c69 720f 0000 0072 0f00  edis_clir....r..
+00001b00: 0000 7210 0000 0072 3700 0000 cc00 0000  ..r....r7.......
+00001b10: 7360 0000 0000 0710 0110 040c 010c 0108  s`..............
+00001b20: 010e 0108 010e 030a 0114 0408 0102 0102  ................
+00001b30: 0102 0102 0102 0102 0102 f804 0a10 0408  ................
+00001b40: 0102 0108 010a fc04 0612 0308 0110 0112  ................
+00001b50: 0110 0112 0110 0110 0314 010e 010e 0102  ................
+00001b60: 010e 0116 0110 0116 011c 0302 010e 0116  ................
+00001b70: 0110 0116 017a 1e44 6174 6162 6173 6542  .....z.DatabaseB
+00001b80: 7569 6c64 6572 2e62 7569 6c64 5f66 726f  uilder.build_fro
+00001b90: 6d5f 6769 7429 0172 3200 0000 2910 7213  m_git).r2...).r.
+00001ba0: 0000 0072 1400 0000 7215 0000 0072 6300  ...r....r....rc.
+00001bb0: 0000 7266 0000 0072 6700 0000 7252 0000  ..rf...rg...rR..
+00001bc0: 0072 6800 0000 7269 0000 0072 6a00 0000  .rh...ri...rj...
+00001bd0: 726b 0000 0072 2b00 0000 726c 0000 0072  rk...r+...rl...r
+00001be0: 3100 0000 7237 0000 00da 0d5f 5f63 6c61  1...r7.....__cla
+00001bf0: 7373 6365 6c6c 5f5f 720f 0000 0072 0f00  sscell__r....r..
+00001c00: 0000 7275 0000 0072 1000 0000 726f 0000  ..ru...r....ro..
+00001c10: 00b4 0000 0073 1e00 0000 0801 0408 0201  .....s..........
+00001c20: 0201 0201 02fc 0201 0e01 0201 0801 0200  ................
+00001c30: 02fc 1008 0201 1007 726f 0000 0063 0000  ........ro...c..
+00001c40: 0000 0000 0000 0000 0000 0000 0000 0b00  ................
+00001c50: 0000 0000 0000 73d0 0000 0065 005a 0164  ......s....e.Z.d
+00001c60: 005a 0264 015a 0369 0064 0264 0264 0364  .Z.d.Z.i.d.d.d.d
+00001c70: 0364 0464 0564 0466 0865 046a 0565 0665  .d.d.d.f.e.j.e.e
+00001c80: 046a 0766 0219 0065 0665 0665 0865 0865  .j.f...e.e.e.e.e
+00001c90: 0865 046a 0965 0a19 0065 0864 0564 069c  .e.j.e...e.d.d..
+00001ca0: 0987 0066 0164 0764 0884 0d5a 0b65 0c65  ...f.d.d...Z.e.e
+00001cb0: 0d64 099c 0164 0a64 0b84 0483 015a 0e65  .d...d.d.....Z.e
+00001cc0: 0c65 0864 099c 0164 0c64 0d84 0483 015a  .e.d...d.d.....Z
+00001cd0: 0f64 0564 099c 0164 0e64 0f84 045a 1065  .d.d...d.d...Z.e
+00001ce0: 0664 0564 109c 0264 1164 1284 045a 1164  .d.d...d.d...Z.d
+00001cf0: 1b65 0665 0665 0664 0564 149c 0464 1564  .e.e.e.d.d...d.d
+00001d00: 1684 055a 1265 0664 0564 109c 0264 1764  ...Z.e.d.d...d.d
+00001d10: 1884 045a 1364 0564 099c 0164 1964 1a84  ...Z.d.d...d.d..
+00001d20: 045a 1487 0004 005a 1553 0029 1cda 0e52  .Z.....Z.S.)...R
+00001d30: 6564 6973 4149 4275 696c 6465 727a a343  edisAIBuilderz.C
+00001d40: 6c61 7373 2074 6f20 6275 696c 6420 5265  lass to build Re
+00001d50: 6469 7341 4920 6672 6f6d 2053 6f75 7263  disAI from Sourc
+00001d60: 650a 2020 2020 5375 7070 6f72 7465 6420  e.    Supported 
+00001d70: 6275 696c 6420 6d65 7468 6f64 3a0a 2020  build method:.  
+00001d80: 2020 202d 2066 726f 6d20 6769 740a 2020     - from git.  
+00001d90: 2020 5365 6520 6275 696c 6465 6e76 2e70    See buildenv.p
+00001da0: 7920 666f 7220 6275 696c 6474 696d 6520  y for buildtime 
+00001db0: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00001dc0: 2052 6564 6973 4149 0a20 2020 2076 6572   RedisAI.    ver
+00001dd0: 7369 6f6e 2061 6e64 2075 726c 2e0a 2020  sion and url..  
+00001de0: 2020 da00 5446 4e29 0972 7100 0000 da09    ..TFN).rq.....
+00001df0: 746f 7263 685f 6469 72da 096c 6962 7466  torch_dir..libtf
+00001e00: 5f64 6972 da0b 6275 696c 645f 746f 7263  _dir..build_torc
+00001e10: 68da 0862 7569 6c64 5f74 66da 0a62 7569  h..build_tf..bui
+00001e20: 6c64 5f6f 6e6e 7872 1900 0000 721a 0000  ld_onnxr....r...
+00001e30: 0072 0600 0000 6309 0000 0000 0000 0000  .r....c.........
+00001e40: 0000 0009 0000 0005 0000 0003 0000 0073  ...............s
+00001e50: 4c00 0000 7400 8300 6a01 7c01 7c07 7c08  L...t...j.|.|.|.
+00001e60: 6401 8d03 0100 7c04 721a 6402 6e02 6403  d.....|.r.d.n.d.
+00001e70: 7c00 5f02 7c05 7228 6402 6e02 6403 7c00  |._.|.r(d.n.d.|.
+00001e80: 5f03 7c06 7236 6402 6e02 6403 7c00 5f04  _.|.r6d.n.d.|._.
+00001e90: 7c03 7c00 5f05 7c02 7c00 5f06 6400 5300  |.|._.|.|._.d.S.
+00001ea0: 2904 4e72 7300 0000 7217 0000 0072 0100  ).Nrs...r....r..
+00001eb0: 0000 2907 7274 0000 0072 2b00 0000 da05  ..).rt...r+.....
+00001ec0: 746f 7263 68da 0274 66da 046f 6e6e 7872  torch..tf..onnxr
+00001ed0: 8e00 0000 728d 0000 0029 0972 2900 0000  ....r....).r)...
+00001ee0: 7271 0000 0072 8d00 0000 728e 0000 0072  rq...r....r....r
+00001ef0: 8f00 0000 7290 0000 0072 9100 0000 7219  ....r....r....r.
+00001f00: 0000 0072 1a00 0000 7275 0000 0072 0f00  ...r....ru...r..
+00001f10: 0000 7210 0000 0072 2b00 0000 1e01 0000  ..r....r+.......
+00001f20: 730c 0000 0000 0b12 030e 010e 010e 0106  s...............
+00001f30: 017a 1752 6564 6973 4149 4275 696c 6465  .z.RedisAIBuilde
+00001f40: 722e 5f5f 696e 6974 5f5f 722c 0000 0063  r.__init__r,...c
+00001f50: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001f60: 0300 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
+00001f70: 006a 0164 0183 0253 0029 024e da07 5265  .j.d...S.).N..Re
+00001f80: 6469 7341 4929 0272 0200 0000 7221 0000  disAI).r....r!..
+00001f90: 0072 3000 0000 720f 0000 0072 0f00 0000  .r0...r....r....
+00001fa0: 7210 0000 00da 0e72 6169 5f62 7569 6c64  r......rai_build
+00001fb0: 5f70 6174 6832 0100 0073 0200 0000 0002  _path2...s......
+00001fc0: 7a1d 5265 6469 7341 4942 7569 6c64 6572  z.RedisAIBuilder
+00001fd0: 2e72 6169 5f62 7569 6c64 5f70 6174 6863  .rai_build_pathc
+00001fe0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00001ff0: 0300 0000 4300 0000 7328 0000 007c 006a  ....C...s(...|.j
+00002000: 00a0 0164 01a1 01a0 02a1 007d 017c 006a  ...d.......}.|.j
+00002010: 00a0 0164 02a1 01a0 03a1 007d 027c 016f  ...d.......}.|.o
+00002020: 267c 0253 0029 034e da08 6261 636b 656e  &|.S.).N..backen
+00002030: 6473 fa0a 7265 6469 7361 692e 736f 2904  ds..redisai.so).
+00002040: 7223 0000 00da 086a 6f69 6e70 6174 6872  r#.....joinpathr
+00002050: 2700 0000 da07 6973 5f66 696c 6529 0372  '.....is_file).r
+00002060: 2900 0000 da06 7365 7276 6572 da03 636c  ).....server..cl
+00002070: 6972 0f00 0000 720f 0000 0072 1000 0000  ir....r....r....
+00002080: 7231 0000 0036 0100 0073 0600 0000 0002  r1...6...s......
+00002090: 1001 1001 7a17 5265 6469 7341 4942 7569  ....z.RedisAIBui
+000020a0: 6c64 6572 2e69 735f 6275 696c 7463 0100  lder.is_builtc..
+000020b0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+000020c0: 0000 4300 0000 733c 0000 007c 006a 0064  ..C...s<...|.j.d
+000020d0: 011b 007d 017c 01a0 01a1 0001 007c 01a0  ...}.|.......|..
+000020e0: 02a1 0072 387c 01a0 03a1 0001 007c 006a  ...r8|.......|.j
+000020f0: 047c 006a 0564 021b 007c 0164 0364 048d  .|.j.d...|.d.d..
+00002100: 0301 0064 0553 0029 067a be43 6f70 7920  ...d.S.).z.Copy 
+00002110: 7468 6520 4669 6e64 5465 6e73 6f72 466c  the FindTensorFl
+00002120: 6f77 2e63 6d61 6b65 2066 696c 6520 746f  ow.cmake file to
+00002130: 2074 6865 2062 7569 6c64 2064 6972 6563   the build direc
+00002140: 746f 7279 0a20 2020 2020 2020 2061 7320  tory.        as 
+00002150: 7468 6520 7665 7273 696f 6e20 696e 636c  the version incl
+00002160: 7564 6564 2069 6e20 5265 6469 7341 4920  uded in RedisAI 
+00002170: 6973 206f 7574 206f 6620 6461 7465 2066  is out of date f
+00002180: 6f72 2075 732e 0a20 2020 2020 2020 204e  or us..        N
+00002190: 6f74 653a 206f 7074 2f63 6d61 6b65 2f6d  ote: opt/cmake/m
+000021a0: 6f64 756c 6573 2072 656d 6f76 6564 2069  odules removed i
+000021b0: 6e20 5265 6469 7341 4920 7631 2e32 2e35  n RedisAI v1.2.5
+000021c0: 0a20 2020 2020 2020 207a 266f 7074 2f63  .        z&opt/c
+000021d0: 6d61 6b65 2f6d 6f64 756c 6573 2f46 696e  make/modules/Fin
+000021e0: 6454 656e 736f 7246 6c6f 772e 636d 616b  dTensorFlow.cmak
+000021f0: 657a 1c6d 6f64 756c 6573 2f46 696e 6454  ez.modules/FindT
+00002200: 656e 736f 7246 6c6f 772e 636d 616b 6546  ensorFlow.cmakeF
+00002210: 7247 0000 004e 2906 7296 0000 0072 8500  rG...N).r....r..
+00002220: 0000 729a 0000 00da 0675 6e6c 696e 6b72  ..r......unlinkr
+00002230: 4400 0000 7222 0000 0029 0272 2900 0000  D...r"...).r)...
+00002240: 5a08 7466 5f63 6d61 6b65 720f 0000 0072  Z.tf_cmaker....r
+00002250: 0f00 0000 7210 0000 00da 0d63 6f70 795f  ....r......copy_
+00002260: 7466 5f63 6d61 6b65 3c01 0000 7312 0000  tf_cmake<...s...
+00002270: 0000 060a 0108 0108 0108 0204 0108 0002  ................
+00002280: 0002 ff7a 1c52 6564 6973 4149 4275 696c  ...z.RedisAIBuil
+00002290: 6465 722e 636f 7079 5f74 665f 636d 616b  der.copy_tf_cmak
+000022a0: 6529 0272 3600 0000 7206 0000 0063 0200  e).r6...r....c..
+000022b0: 0000 0000 0000 0000 0000 0b00 0000 0900  ................
+000022c0: 0000 4300 0000 732e 0100 0074 007c 006a  ..C...s....t.|.j
+000022d0: 01a0 0274 036a 04a0 0564 0164 027c 019b  ...t.j...d.d.|..
+000022e0: 0064 029d 03a1 02a1 0183 017d 027c 0273  .d.........}.|.s
+000022f0: 2e74 0664 0383 0182 017c 0264 0419 0064  .t.d.....|.d...d
+00002300: 051b 007d 037c 03a0 07a1 0001 007c 03a0  ...}.|.......|..
+00002310: 08a1 0072 5474 09a0 0a7c 03a1 0101 0074  ...rTt...|.....t
+00002320: 03a0 0b7c 03a1 0101 0074 0c7c 006a 0d83  ...|.....t.|.j..
+00002330: 01a0 07a1 007d 047c 0464 061b 007d 057c  .....}.|.d...}.|
+00002340: 05a0 0ea1 0073 8a74 0664 077c 049b 009d  .....s.t.d.|....
+00002350: 0283 0182 0174 03a0 0f7c 057c 0364 061b  .....t...|.|.d..
+00002360: 00a1 0201 007c 0364 081b 007d 0674 03a0  .....|.d...}.t..
+00002370: 0b7c 06a1 0101 007c 0464 081b 007d 077c  .|.....|.d...}.|
+00002380: 07a0 08a1 0072 de74 007c 07a0 0264 02a1  .....r.t.|...d..
+00002390: 0183 017d 087c 0873 fe74 0664 097c 079b  ...}.|.s.t.d.|..
+000023a0: 009d 0283 0182 016e 2074 007c 04a0 0264  .......n t.|...d
+000023b0: 0aa1 0183 017d 087c 0873 fe74 0664 097c  .....}.|.s.t.d.|
+000023c0: 049b 009d 0283 0182 017c 0844 005d 267d  .........|.D.]&}
+000023d0: 097c 067c 096a 101b 007d 0a7c 0aa0 11a1  .|.|.j...}.|....
+000023e0: 0090 0173 0274 03a0 0f7c 097c 0aa1 0201  ...s.t...|.|....
+000023f0: 0090 0171 0264 0b53 0029 0c7a 8341 6464  ...q.d.S.).z.Add
+00002400: 2073 796d 626f 6c69 6320 6c69 6e6b 2074   symbolic link t
+00002410: 6f20 6176 6169 6c61 626c 6520 6c69 6274  o available libt
+00002420: 656e 736f 7266 6c6f 7720 696e 2052 6564  ensorflow in Red
+00002430: 6973 4149 2064 6570 732e 0a0a 2020 2020  isAI deps...    
+00002440: 2020 2020 3a70 6172 616d 2064 6576 6963      :param devic
+00002450: 653a 2063 7075 206f 7220 6770 750a 2020  e: cpu or gpu.  
+00002460: 2020 2020 2020 3a74 7970 6520 6465 7669        :type devi
+00002470: 6365 3a20 7374 720a 2020 2020 2020 2020  ce: str.        
+00002480: da04 6465 7073 7246 0000 007a 2743 6f75  ..depsrF...z'Cou
+00002490: 6c64 206e 6f74 2066 696e 6420 5265 6469  ld not find Redi
+000024a0: 7341 4920 2764 6570 7327 2064 6972 6563  sAI 'deps' direc
+000024b0: 746f 7279 7201 0000 005a 0d6c 6962 7465  toryr....Z.libte
+000024c0: 6e73 6f72 666c 6f77 da07 696e 636c 7564  nsorflow..includ
+000024d0: 657a 2443 6f75 6c64 206e 6f74 2066 696e  ez$Could not fin
+000024e0: 6420 696e 636c 7564 6520 6469 7265 6374  d include direct
+000024f0: 6f72 7920 696e 2072 1c00 0000 7a2e 436f  ory in r....z.Co
+00002500: 756c 6420 6e6f 7420 6669 6e64 206c 6962  uld not find lib
+00002510: 7465 6e73 6f72 666c 6f77 206c 6962 7261  tensorflow libra
+00002520: 7279 2066 696c 6573 2069 6e20 7a08 6c69  ry files in z.li
+00002530: 622a 2e73 6f2a 4e29 12da 0673 6f72 7465  b*.so*N)...sorte
+00002540: 6472 9600 0000 7248 0000 0072 0700 0000  dr....rH...r....
+00002550: 7208 0000 00da 046a 6f69 6e72 0e00 0000  r......joinr....
+00002560: 7285 0000 0072 2700 0000 7239 0000 0072  r....r'...r9...r
+00002570: 5100 0000 da08 6d61 6b65 6469 7273 7202  Q.....makedirsr.
+00002580: 0000 0072 8e00 0000 da06 6578 6973 7473  ...r......exists
+00002590: da07 7379 6d6c 696e 6b72 4a00 0000 729a  ..symlinkrJ...r.
+000025a0: 0000 0029 0b72 2900 0000 7236 0000 005a  ...).r)...r6...Z
+000025b0: 0d72 6169 5f64 6570 735f 7061 7468 5a0e  .rai_deps_pathZ.
+000025c0: 7261 695f 6c69 6274 665f 7061 7468 5a0a  rai_libtf_pathZ.
+000025d0: 6c69 6274 665f 7061 7468 5a10 696e 636c  libtf_pathZ.incl
+000025e0: 7564 655f 7372 635f 7061 7468 5a11 7261  ude_src_pathZ.ra
+000025f0: 695f 6c69 6274 665f 6c69 625f 6469 725a  i_libtf_lib_dirZ
+00002600: 1173 7263 5f6c 6962 7466 5f6c 6962 5f64  .src_libtf_lib_d
+00002610: 6972 5a0d 6c69 6272 6172 795f 6669 6c65  irZ.library_file
+00002620: 735a 0873 7263 5f66 696c 655a 0864 7374  sZ.src_fileZ.dst
+00002630: 5f66 696c 6572 0f00 0000 720f 0000 0072  _filer....r....r
+00002640: 1000 0000 da0d 7379 6d6c 696e 6b5f 6c69  ......symlink_li
+00002650: 6274 664b 0100 0073 4200 0000 0006 0201  btfK...sB.......
+00002660: 1cff 0403 0401 0805 0c01 0801 0801 0a02  ................
+00002670: 0a01 0e03 0801 0801 0e01 1004 0801 0a01  ................
+00002680: 0804 0801 0e01 0401 0201 08ff 0604 0e01  ................
+00002690: 0401 0201 08ff 0404 0801 0a01 0a01 7a1c  ..............z.
+000026a0: 5265 6469 7341 4942 7569 6c64 6572 2e73  RedisAIBuilder.s
+000026b0: 796d 6c69 6e6b 5f6c 6962 7466 7232 0000  ymlink_libtfr2..
+000026c0: 0072 3300 0000 6304 0000 0000 0000 0000  .r3...c.........
+000026d0: 0000 0008 0000 000a 0000 0043 0000 0073  ...........C...s
+000026e0: fa01 0000 7c00 6a00 a001 a100 7216 7402  ....|.j.....r.t.
+000026f0: a003 7c00 6a00 a101 0100 7c00 a004 7c01  ..|.j.....|...|.
+00002700: a101 732e 7405 6401 7c01 9b00 9d02 8301  ..s.t.d.|.......
+00002710: 8201 7c00 a006 6402 a101 6403 6404 6405  ..|...d...d.d.d.
+00002720: 6406 7c01 6706 7d04 6700 7d05 7407 6a08  d.|.g.}.g.}.t.j.
+00002730: 6407 6b02 7276 7c02 6408 6b02 7276 7c00  d.k.rv|.d.k.rv|.
+00002740: 6a09 7276 7c04 6409 6701 3700 7d04 6404  j.rv|.d.g.7.}.d.
+00002750: 640a 640b 6703 7d05 6e10 7c04 640c 7c02  d.d.g.}.n.|.d.|.
+00002760: 640d 6409 6704 3700 7d04 7c00 6a0a 7c04  d.d.g.7.}.|.j.|.
+00002770: 740b 6a0c 7c00 6a0d 640e 8d03 0100 7c05  t.j.|.j.d.....|.
+00002780: 72b2 7c00 6a0a 7c05 740b 6a0c 7c00 6a00  r.|.j.|.t.j.|.j.
+00002790: 640e 8d03 0100 7c00 a00e a100 0100 7c00  d.....|.......|.
+000027a0: a006 6402 a101 640f 6410 7c00 6a0f 72d6  ..d...d.d.|.j.r.
+000027b0: 7c00 6a10 73d6 6411 6e02 6412 9b00 9d02  |.j.s.d.n.d.....
+000027c0: 6413 6414 7c00 6a09 9b00 9d02 6415 7c00  d.d.|.j.....d.|.
+000027d0: a006 6416 a101 7411 7c00 6a00 6417 1b00  ..d...t.|.j.d...
+000027e0: 8301 7411 7c03 8301 6709 7d06 7c00 6a0a  ..t.|...g.}.|.j.
+000027f0: 7c06 740b 6a0c 7c00 6a00 640e 8d03 0100  |.t.j.|.j.d.....
+00002800: 7c00 6a10 9001 7234 7c03 9001 7234 7c00  |.j...r4|...r4|.
+00002810: a012 7c03 a101 0100 7c00 a006 6402 a101  ..|.....|...d...
+00002820: 6418 7c00 6a13 9b00 9d02 6410 7c00 6a0f  d.|.j.....d.|.j.
+00002830: 9b00 9d02 6413 6414 7c00 6a09 9b00 9d02  ....d.d.|.j.....
+00002840: 6419 6706 7d07 7c03 641a 6b02 9001 7278  d.g.}.|.d.k...rx
+00002850: 7c07 a014 641b a101 0100 6e0a 7c07 a014  |...d.....n.|...
+00002860: 641c a101 0100 7c00 6a15 9001 729a 7411  d.....|.j...r.t.
+00002870: 7c00 6a15 8301 7c00 6a16 641d 3c00 7c07  |.j...|.j.d.<.|.
+00002880: a017 7c00 a006 641e a101 641f 7411 7c00  ..|...d...d.t.|.
+00002890: 6a00 6420 1b00 8301 6421 7c00 6a18 9b00  j.d ....d!|.j...
+000028a0: 6422 6706 a101 0100 7c00 6a0a 7c07 7c00  d"g.....|.j.|.|.
+000028b0: 6a00 6423 8d02 0100 7c00 a019 7c03 a101  j.d#....|...|...
+000028c0: 0100 7c00 6a13 9001 72ee 7c00 a01a a100  ..|.j...r.|.....
+000028d0: 0100 7c00 a01b a100 0100 6424 5300 2925  ..|.......d$S.)%
+000028e0: 7af5 4275 696c 6420 5265 6469 7341 4920  z.Build RedisAI 
+000028f0: 6672 6f6d 2067 6974 0a20 2020 2020 2020  from git.       
+00002900: 203a 7061 7261 6d20 6769 745f 7572 6c3a   :param git_url:
+00002910: 2075 726c 2066 726f 6d20 7768 6963 6820   url from which 
+00002920: 746f 2072 6574 7269 6576 6520 5265 6469  to retrieve Redi
+00002930: 7341 490a 2020 2020 2020 2020 3a74 7970  sAI.        :typ
+00002940: 6520 6769 745f 7572 6c3a 2073 7472 0a20  e git_url: str. 
+00002950: 2020 2020 2020 203a 7061 7261 6d20 6272         :param br
+00002960: 616e 6368 3a20 6272 616e 6368 2074 6f20  anch: branch to 
+00002970: 6368 6563 6b6f 7574 0a20 2020 2020 2020  checkout.       
+00002980: 203a 7479 7065 2062 7261 6e63 683a 2073   :type branch: s
+00002990: 7472 0a20 2020 2020 2020 203a 7061 7261  tr.        :para
+000029a0: 6d20 6465 7669 6365 3a20 6370 7520 6f72  m device: cpu or
+000029b0: 2067 7075 0a20 2020 2020 2020 203a 7479   gpu.        :ty
+000029c0: 7065 2064 6576 6963 653a 2073 7472 0a20  pe device: str. 
+000029d0: 2020 2020 2020 207a 174d 616c 666f 726d         z.Malform
+000029e0: 6564 2052 6564 6973 4149 2055 524c 3a20  ed RedisAI URL: 
+000029f0: 7218 0000 007a 1547 4954 5f4c 4653 5f53  r....z.GIT_LFS_S
+00002a00: 4b49 505f 534d 5544 4745 3d31 727c 0000  KIP_SMUDGE=1r|..
+00002a10: 0072 7d00 0000 7a0b 2d2d 7265 6375 7273  .r}...z.--recurs
+00002a20: 6976 65da 0664 6172 7769 6e7a 0676 312e  ive..darwinz.v1.
+00002a30: 322e 3772 9500 0000 5a08 6368 6563 6b6f  2.7r....Z.checko
+00002a40: 7574 5a28 3633 3439 3136 6337 3232 6537  utZ(634916c722e7
+00002a50: 3138 6363 3665 6133 6661 6434 3665 3633  18cc6ea3fad46e63
+00002a60: 6637 6437 3938 6639 6164 6332 727e 0000  f7d798f9adc2r~..
+00002a70: 007a 092d 2d64 6570 7468 3d31 2902 7226  .z.--depth=1).r&
+00002a80: 0000 0072 5600 0000 7a09 5749 5448 5f50  ...rV...z.WITH_P
+00002a90: 543d 307a 0857 4954 485f 5446 3d72 1700  T=0z.WITH_TF=r..
+00002aa0: 0000 7201 0000 007a 0d57 4954 485f 5446  ..r....z.WITH_TF
+00002ab0: 4c49 5445 3d30 7a09 5749 5448 5f4f 5254  LITE=0z.WITH_ORT
+00002ac0: 3d7a 0956 4552 424f 5345 3d31 5a04 6261  =z.VERBOSE=1Z.ba
+00002ad0: 7368 7a0b 6765 745f 6465 7073 2e73 687a  shz.get_deps.shz
+00002ae0: 0857 4954 485f 5054 3d7a 1157 4954 485f  .WITH_PT=z.WITH_
+00002af0: 554e 4954 5f54 4553 5453 3d30 5a03 6770  UNIT_TESTS=0Z.gp
+00002b00: 757a 0547 5055 3d31 7a05 4750 553d 305a  uz.GPU=1z.GPU=0Z
+00002b10: 0954 6f72 6368 5f44 4952 7281 0000 007a  .Torch_DIRr....z
+00002b20: 022d 43da 036f 7074 7282 0000 00da 0562  .-C..optr......b
+00002b30: 7569 6c64 7280 0000 004e 291c 7296 0000  uildr....N).r...
+00002b40: 0072 2700 0000 7239 0000 0072 5100 0000  .r'...r9...rQ...
+00002b50: 7250 0000 0072 1200 0000 723a 0000 00da  rP...r....r:....
+00002b60: 0373 7973 da08 706c 6174 666f 726d 7294  .sys..platformr.
+00002b70: 0000 0072 6200 0000 7224 0000 0072 2500  ...rb...r$...r%.
+00002b80: 0000 7221 0000 0072 9e00 0000 7293 0000  ..r!...r....r...
+00002b90: 0072 8e00 0000 7252 0000 0072 a600 0000  .r....rR...r....
+00002ba0: 7292 0000 00da 0661 7070 656e 6472 8d00  r......appendr..
+00002bb0: 0000 7218 0000 00da 0665 7874 656e 6472  ..r......extendr
+00002bc0: 1900 0000 da11 5f69 6e73 7461 6c6c 5f62  ......_install_b
+00002bd0: 6163 6b65 6e64 73da 105f 6d6f 7665 5f74  ackends.._move_t
+00002be0: 6f72 6368 5f6c 6962 7372 5300 0000 2908  orch_libsrS...).
+00002bf0: 7229 0000 0072 3400 0000 7235 0000 0072  r)...r4...r5...r
+00002c00: 3600 0000 7287 0000 005a 1063 6865 636b  6...r....Z.check
+00002c10: 6f75 745f 6f73 785f 6669 785a 0764 6570  out_osx_fixZ.dep
+00002c20: 5f63 6d64 7288 0000 0072 0f00 0000 720f  _cmdr....r....r.
+00002c30: 0000 0072 1000 0000 7237 0000 0082 0100  ...r....r7......
+00002c40: 0073 9600 0000 000a 0a01 0c03 0a01 0e04  .s..............
+00002c50: 0801 0201 0201 0201 0201 02fa 0409 0404  ................
+00002c60: 1802 0a02 0201 0201 02fd 0607 0201 0201  ................
+00002c70: 0201 0201 02fc 0607 1401 0401 0401 0200  ................
+00002c80: 0400 04ff 0605 0804 0801 0201 1801 0201  ................
+00002c90: 0a01 0201 0801 0c01 06f7 040c 0401 0201  ................
+00002ca0: 0401 04fd 0606 0e01 0a03 0801 0a01 0a01  ................
+00002cb0: 0201 0a01 02fa 0409 0a01 0c02 0a02 0801  ................
+00002cc0: 1002 0402 0801 0201 0c01 0201 0601 02fa  ................
+00002cd0: 02ff 040a 1002 0a01 0801 0801 7a1d 5265  ............z.Re
+00002ce0: 6469 7341 4942 7569 6c64 6572 2e62 7569  disAIBuilder.bui
+00002cf0: 6c64 5f66 726f 6d5f 6769 7463 0200 0000  ld_from_gitc....
+00002d00: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+00002d10: 4300 0000 736c 0000 007c 006a 00a0 0164  C...sl...|.j...d
+00002d20: 017c 019b 009d 02a1 01a0 02a1 007c 005f  .|...........|._
+00002d30: 037c 006a 0364 021b 007d 027c 006a 0364  .|.j.d...}.|.j.d
+00002d40: 031b 007d 037c 02a0 04a1 0072 687c 03a0  ...}.|.....rh|..
+00002d50: 05a1 0072 687c 006a 067c 037c 006a 0764  ...rh|.j.|.|.j.d
+00002d60: 031b 0064 0464 058d 0301 007c 006a 087c  ...d.d.....|.j.|
+00002d70: 027c 006a 0764 021b 0064 0464 058d 0301  .|.j.d...d.d....
+00002d80: 0064 0653 0029 077a 724d 6f76 6520 6261  .d.S.).zrMove ba
+00002d90: 636b 656e 6420 6c69 6272 6172 6965 7320  ckend libraries 
+00002da0: 746f 2073 6d61 7274 7369 6d2f 5f63 6f72  to smartsim/_cor
+00002db0: 652f 6c69 622f 0a20 2020 2020 2020 203a  e/lib/.        :
+00002dc0: 7061 7261 6d20 6465 7669 6365 3a20 6370  param device: cp
+00002dd0: 7520 6f72 2063 7075 0a20 2020 2020 2020  u or cpu.       
+00002de0: 203a 7479 7065 2064 6576 6963 653a 2073   :type device: s
+00002df0: 7472 0a20 2020 2020 2020 207a 0869 6e73  tr.        z.ins
+00002e00: 7461 6c6c 2d72 9800 0000 7297 0000 0054  tall-r....r....T
+00002e10: 7247 0000 004e 2909 7296 0000 0072 9900  rG...N).r....r..
+00002e20: 0000 7285 0000 005a 1072 6169 5f69 6e73  ..r....Z.rai_ins
+00002e30: 7461 6c6c 5f70 6174 6872 9a00 0000 7227  tall_pathr....r'
+00002e40: 0000 0072 4900 0000 7223 0000 0072 4400  ...rI...r#...rD.
+00002e50: 0000 2904 7229 0000 0072 3600 0000 5a07  ..).r)...r6...Z.
+00002e60: 7261 695f 6c69 625a 0c72 6169 5f62 6163  rai_libZ.rai_bac
+00002e70: 6b65 6e64 7372 0f00 0000 720f 0000 0072  kendsr....r....r
+00002e80: 1000 0000 72ae 0000 00f3 0100 0073 1000  ....r........s..
+00002e90: 0000 0005 0601 08ff 0a03 0a01 0a02 1001  ................
+00002ea0: 1601 7a20 5265 6469 7341 4942 7569 6c64  ..z RedisAIBuild
+00002eb0: 6572 2e5f 696e 7374 616c 6c5f 6261 636b  er._install_back
+00002ec0: 656e 6473 6301 0000 0000 0000 0000 0000  endsc...........
+00002ed0: 0006 0000 0005 0000 0043 0000 0073 6800  .........C...sh.
+00002ee0: 0000 7c00 6a00 6401 1b00 6402 1b00 7d01  ..|.j.d...d...}.
+00002ef0: 7c01 6403 1b00 7d02 7401 7c00 6a02 8301  |.d...}.t.|.j...
+00002f00: 6a03 6a03 6a03 7d03 7c03 6403 1b00 7d04  j.j.j.}.|.d...}.
+00002f10: 7c00 6a04 7c04 7c02 6404 6405 8d03 0100  |.j.|.|.d.d.....
+00002f20: 7405 6a06 6406 6b02 7264 7c03 6407 1b00  t.j.d.k.rd|.d...
+00002f30: 7d05 7c00 6a04 7c05 7c01 6407 1b00 6404  }.|.j.|.|.d...d.
+00002f40: 6405 8d03 0100 6408 5300 2909 7ade 4d6f  d.....d.S.).z.Mo
+00002f50: 7665 2070 6970 2069 6e73 7461 6c6c 2074  ve pip install t
+00002f60: 6f72 6368 206c 6962 7261 7269 6573 0a20  orch libraries. 
+00002f70: 2020 2020 2020 2053 696e 6365 2077 6520         Since we 
+00002f80: 7573 6520 7069 7020 696e 7374 616c 6c65  use pip installe
+00002f90: 6420 746f 7263 6820 6c69 6272 6172 6965  d torch librarie
+00002fa0: 7320 666f 7220 6275 696c 6469 6e67 0a20  s for building. 
+00002fb0: 2020 2020 2020 2052 6564 6973 4149 2c20         RedisAI, 
+00002fc0: 7765 206e 6565 6420 746f 206d 6f76 6520  we need to move 
+00002fd0: 7468 656d 2069 6e74 6f20 7468 6520 4c44  them into the LD
+00002fe0: 5f72 756e 7061 7468 206f 6620 7265 6469  _runpath of redi
+00002ff0: 7361 692e 736f 0a20 2020 2020 2020 2069  sai.so.        i
+00003000: 6e20 7468 6520 736d 6172 7473 696d 2f5f  n the smartsim/_
+00003010: 636f 7265 2f6c 6962 2064 6972 6563 746f  core/lib directo
+00003020: 7279 2e0a 2020 2020 2020 2020 7297 0000  ry..        r...
+00003030: 005a 0d72 6564 6973 6169 5f74 6f72 6368  .Z.redisai_torch
+00003040: 721c 0000 0054 7247 0000 0072 a700 0000  r....TrG...r....
+00003050: 7a07 2e64 796c 6962 734e 2907 7223 0000  z..dylibsN).r#..
+00003060: 0072 0200 0000 728d 0000 0072 1e00 0000  .r....r....r....
+00003070: 7249 0000 0072 aa00 0000 72ab 0000 0029  rI...r....r....)
+00003080: 0672 2900 0000 5a11 7373 5f72 6169 5f74  .r)...Z.ss_rai_t
+00003090: 6f72 6368 5f70 6174 685a 1573 735f 7261  orch_pathZ.ss_ra
+000030a0: 695f 746f 7263 685f 6c69 625f 7061 7468  i_torch_lib_path
+000030b0: 5a0e 7069 705f 746f 7263 685f 7061 7468  Z.pip_torch_path
+000030c0: 5a12 7069 705f 746f 7263 685f 6c69 625f  Z.pip_torch_lib_
+000030d0: 7061 7468 5a06 6479 6c69 6273 720f 0000  pathZ.dylibsr...
+000030e0: 0072 0f00 0000 7210 0000 0072 af00 0000  .r....r....r....
+000030f0: 0202 0000 7310 0000 0000 070e 0108 0610  ....s...........
+00003100: 0108 0210 030a 0108 017a 1f52 6564 6973  .........z.Redis
+00003110: 4149 4275 696c 6465 722e 5f6d 6f76 655f  AIBuilder._move_
+00003120: 746f 7263 685f 6c69 6273 2901 7232 0000  torch_libs).r2..
+00003130: 0029 1672 1300 0000 7214 0000 0072 1500  .).r....r....r..
+00003140: 0000 7263 0000 0072 6600 0000 7267 0000  ..rc...rf...rg..
+00003150: 0072 5200 0000 7268 0000 0072 6b00 0000  .rR...rh...rk...
+00003160: 7269 0000 0072 6a00 0000 722b 0000 0072  ri...rj...r+...r
+00003170: 6c00 0000 7202 0000 0072 9600 0000 7231  l...r....r....r1
+00003180: 0000 0072 9e00 0000 72a6 0000 0072 3700  ...r....r....r7.
+00003190: 0000 72ae 0000 0072 af00 0000 728a 0000  ..r....r....r...
+000031a0: 0072 0f00 0000 720f 0000 0072 7500 0000  .r....r....ru...
+000031b0: 7210 0000 0072 8b00 0000 1601 0000 733a  r....r........s:
+000031c0: 0000 0008 0104 0902 0102 0102 0102 0102  ................
+000031d0: 0102 0102 0102 f702 020e 0102 0102 0102  ................
+000031e0: 0102 0102 0108 0102 0102 f610 1402 0110  ................
+000031f0: 0302 0110 050e 0f10 3716 7110 0f72 8b00  ........7.q..r..
+00003200: 0000 2913 7207 0000 0072 4d00 0000 7239  ..).r....rM...r9
+00003210: 0000 0072 4000 0000 7224 0000 0072 aa00  ...r@...r$...r..
+00003220: 0000 da06 7479 7069 6e67 7266 0000 00da  ....typingrf....
+00003230: 0770 6174 686c 6962 7202 0000 0072 0300  .pathlibr....r..
+00003240: 0000 7204 0000 0072 5200 0000 7211 0000  ..r....rR...r...
+00003250: 00da 0945 7863 6570 7469 6f6e 7212 0000  ...Exceptionr...
+00003260: 0072 1600 0000 726f 0000 0072 8b00 0000  .r....ro...r....
+00003270: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00003280: 1000 0000 da08 3c6d 6f64 756c 653e 1b00  ......<module>..
+00003290: 0000 731c 0000 0008 0108 0108 0108 0108  ..s.............
+000032a0: 0108 0108 010c 010c 010c 0a10 1410 040e  ................
+000032b0: 6e10 62                                  n.b
```

### Comparing `smartsim-0.4.2/smartsim/_core/_install/buildenv.py` & `smartsim-0.5.0/smartsim/_core/_install/buildenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import platform
 import site
 import subprocess
 import sys
+import typing as t
 from pathlib import Path
 from typing import Iterable
 
 import pkg_resources
-from pkg_resources import packaging
+from pkg_resources import packaging  # type: ignore
 
 Version = packaging.version.Version
 InvalidVersion = packaging.version.InvalidVersion
-
+DbEngine = t.Literal["REDIS", "KEYDB"]
 
 # NOTE: This will be imported by setup.py and hence no
 #       smartsim related items or non-standand library
 #       items should be imported here.
 
-
 class SetupError(Exception):
     """A simple exception class for errors in _install.buildenv file.
     This is primarily used to interrupt the setup.py build in case
     of a failure, and is caught frequently in the CLI which attempts
     to suppress and log the errors thrown here.
 
     One note is that this error must be imported from here to be
@@ -63,75 +63,75 @@
 
 # so as to not conflict with pkg_resources.packaging.version.Version
 class Version_(str):
     """A subclass of pkg_resources.packaging.version.Version that
     includes some helper methods for comparing versions.
     """
 
-    def _convert_to_version(self, vers):
+    def _convert_to_version(self, vers: t.Union[str, Iterable[packaging.version.Version], packaging.version.Version]) -> t.Any:
         if isinstance(vers, Version):
             return vers
         elif isinstance(vers, str):
             return Version(vers)
         elif isinstance(vers, Iterable):
             return Version(".".join((str(item) for item in vers)))
         else:
             raise InvalidVersion(vers)
 
     @property
-    def major(self):
+    def major(self) -> int:
         # Version(self).major doesn't work for all Python distributions
         # see https://github.com/lebedov/python-pdfbox/issues/28
         return int(pkg_resources.parse_version(self).base_version.split(".")[0])
 
     @property
-    def minor(self):
+    def minor(self) -> int:
         return int(pkg_resources.parse_version(self).base_version.split(".")[1])
 
     @property
-    def micro(self):
+    def micro(self) -> int:
         return int(pkg_resources.parse_version(self).base_version.split(".")[2])
 
     @property
-    def patch(self):
+    def patch(self) -> str:
         # return micro with string modifier i.e. 1.2.3+cpu -> 3+cpu
         return str(pkg_resources.parse_version(self)).split(".")[2]
 
-    def __gt__(self, cmp):
+    def __gt__(self, cmp: t.Any) -> bool:
         try:
             return Version(self).__gt__(self._convert_to_version(cmp))
         except InvalidVersion:
             return super().__gt__(cmp)
 
-    def __lt__(self, cmp):
+    def __lt__(self, cmp: t.Any) -> bool:
         try:
             return Version(self).__lt__(self._convert_to_version(cmp))
         except InvalidVersion:
             return super().__lt__(cmp)
 
-    def __eq__(self, cmp):
+    def __eq__(self, cmp: t.Any) -> bool:
         try:
             return Version(self).__eq__(self._convert_to_version(cmp))
         except InvalidVersion:
             return super().__eq__(cmp)
 
-    def __ge__(self, cmp):
+    def __ge__(self, cmp: t.Any) -> bool:
         try:
             return Version(self).__ge__(self._convert_to_version(cmp))
         except InvalidVersion:
             return super().__ge__(cmp)
 
-    def __le__(self, cmp):
+    def __le__(self, cmp: t.Any) -> bool:
         try:
             return Version(self).__le__(self._convert_to_version(cmp))
         except InvalidVersion:
             return super().__le__(cmp)
 
 
-def get_env(var, default):
+def get_env(var: str, default: str) -> str:
     return os.environ.get(var, default)
 
 
 class RedisAIVersion(Version_):
     """A subclass of Version_ that holds the dependency sets for RedisAI
 
     this class serves two purposes:
@@ -178,15 +178,15 @@
         defaults["1.2.7"].pop("skl2onnx")
         defaults["1.2.7"].pop("onnxmltools")
         defaults["1.2.7"].pop("scikit-learn")
     # Remove incompatible RAI versions for OSX
     if sys.platform == "darwin":
         defaults.pop("1.2.5", None)
 
-    def __init__(self, vers):
+    def __init__(self, vers: str) -> None:
         min_rai_version = min(Version_(ver) for ver in self.defaults)
         if min_rai_version > vers:
             raise SetupError(
                 f"RedisAI version must be greater than or equal to {min_rai_version}"
             )
         if vers not in self.defaults:
             if vers.startswith("1.2"):
@@ -196,28 +196,28 @@
             else:
                 raise SetupError(
                     f"Invalid RedisAI version {vers}. Options are {self.defaults.keys()}"
                 )
         else:
             self.version = vers
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> str:
         try:
             return self.defaults[self.version][name]
         except KeyError:
             raise AttributeError(
                 f"'{type(self).__name__}' object has no attribute '{name}'\n\n"
                 "This is likely a problem with the SmartSim build process;"
                 "if this problem persists please log a new issue at "
                 "https://github.com/CrayLabs/SmartSim/issues "
                 "or get in contact with us at "
                 "https://www.craylabs.org/docs/community.html"
             ) from None
 
-    def get_defaults(self):
+    def get_defaults(self) -> t.Dict[str, str]:
         return self.defaults[self.version].copy()
 
 
 class Versioner:
     """Versioner is responsible for managing all the versions
     within SmartSim including SmartSim itself.
 
@@ -240,16 +240,16 @@
     default versions of the machine learning libraries.
     """
 
     # compatible Python version
     PYTHON_MIN = Version_("3.8.0")
 
     # Versions
-    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.4.2"))
-    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.4.0"))
+    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.5.0"))
+    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.4.1"))
     SMARTSIM_SUFFIX = get_env("SMARTSIM_SUFFIX", "")
 
     # Redis
     REDIS = Version_(get_env("SMARTSIM_REDIS", "7.0.5"))
     REDIS_URL = get_env("SMARTSIM_REDIS_URL", "https://github.com/redis/redis.git/")
     REDIS_BRANCH = get_env("SMARTSIM_REDIS_BRANCH", REDIS)
 
@@ -273,15 +273,15 @@
     # the RedisAI package and therefore the user is free to pick other versions.
     TENSORFLOW = Version_(REDISAI.tensorflow)
     try:
         ONNX = Version_(REDISAI.onnx)
     except AttributeError:
         ONNX = None
 
-    def as_dict(self, db_name="REDIS"):
+    def as_dict(self, db_name: DbEngine = "REDIS") -> t.Dict[str, t.Any]:
         packages = [
             "SMARTSIM",
             "SMARTREDIS",
             db_name,
             "REDISAI",
             "TORCH",
             "TENSORFLOW",
@@ -296,15 +296,15 @@
         ]
         if self.ONNX:
             packages.append("ONNX")
             versions.append(self.ONNX)
         vers = {"Packages": packages, "Versions": versions}
         return vers
 
-    def ml_extras_required(self):
+    def ml_extras_required(self) -> t.List[str]:
         """Optional ML/DL dependencies we suggest for the user.
 
         The defaults are based on the RedisAI version
         """
         ml_defaults = self.REDISAI.get_defaults()
 
         # remove torch-related fields as they will be installed
@@ -319,41 +319,40 @@
             "torch_cuda_suffix",
         ]
         for field in _torch_fields:
             ml_defaults.pop(field)
 
         return [f"{lib}=={vers}" for lib, vers in ml_defaults.items()]
 
-    def get_sha(self, setup_py_dir) -> str:
+    def get_sha(self, setup_py_dir: Path) -> str:
         """Get the git sha of the current branch"""
         try:
-            sha = (
-                subprocess.check_output(["git", "rev-parse", "HEAD"], cwd=setup_py_dir)
-                .decode("ascii")
-                .strip()
-            )
+            rev_cmd = ["git", "rev-parse", "HEAD"]
+            git_rev = subprocess.check_output(rev_cmd, cwd=setup_py_dir.absolute())
+            sha = git_rev.decode("ascii").strip()
+
             return sha[:7]
         except Exception:
             # return empty string if not in git-repo
             return ""
 
-    def write_version(self, setup_py_dir):
+    def write_version(self, setup_py_dir: Path) -> str:
         """
         Write version info to version.py
 
         Use git_sha in the case where smartsim suffix is set in the environment
         """
-        version = self.SMARTSIM
+        version = str(self.SMARTSIM)
+
         if self.SMARTSIM_SUFFIX:
-            git_sha = self.get_sha(setup_py_dir)
-            if git_sha:
-                version = f"{version}+{self.SMARTSIM_SUFFIX}.{git_sha}"
-            else:
-                # wheel build (python -m build) shouldn't include git sha
-                version = f"{version}+{self.SMARTSIM_SUFFIX}"
+            version += f"+{self.SMARTSIM_SUFFIX}"
+
+            # wheel build (python -m build) won't include git sha
+            if git_sha := self.get_sha(setup_py_dir):
+                version += f".{git_sha}"
 
         version_file = setup_py_dir / "smartsim" / "version.py"
         with open(version_file, "w") as f:
             f.write("# This file is automatically generated by setup.py\n")
             f.write("# do not edit this file manually.\n\n")
 
             f.write(f"__version__ = '{version}'\n")
@@ -382,108 +381,108 @@
     CC = os.environ.get("CC", "gcc")
     CXX = os.environ.get("CXX", "g++")
     CFLAGS = os.environ.get("CFLAGS", "")
     CXXFLAGS = os.environ.get("CXXFLAGS", "")
 
     # build overrides
     MALLOC = os.environ.get("MALLOC", "libc")
-    JOBS = os.environ.get("BUILD_JOBS", 1)
+    JOBS = int(os.environ.get("BUILD_JOBS", 1))
 
     # check for CC/GCC/ETC
     CHECKS = int(os.environ.get("NO_CHECKS", 0))
     PLATFORM = sys.platform
 
-    def __init__(self, checks=True):
+    def __init__(self, checks: bool = True) -> None:
         if checks:
             self.check_dependencies()
 
-    def check_dependencies(self):
+    def check_dependencies(self) -> None:
         deps = ["git", "git-lfs", "make", "wget", "cmake", self.CC, self.CXX]
         if int(self.CHECKS) == 0:
             for dep in deps:
                 self.check_build_dependency(dep)
 
-    def __call__(self):
+    def __call__(self) -> t.Dict[str, str]:
         # return the build env for the build process
         env = os.environ.copy()
         env.update(
             {
                 "CC": self.CC,
                 "CXX": self.CXX,
                 "CFLAGS": self.CFLAGS,
                 "CXXFLAGS": self.CXXFLAGS,
             }
         )
         return env
 
-    def as_dict(self):
-        variables = [
+    def as_dict(self) -> t.Dict[str, t.List[str]]:
+        variables: t.List[str] = [
             "CC",
             "CXX",
             "CFLAGS",
             "CXXFLAGS",
             "MALLOC",
             "JOBS",
             "PYTHON_VERSION",
             "PLATFORM",
         ]
-        values = [
+        values: t.List[str] = [
             self.CC,
             self.CXX,
             self.CFLAGS,
             self.CXXFLAGS,
             self.MALLOC,
-            self.JOBS,
+            str(self.JOBS),
             self.python_version,
             self.PLATFORM,
         ]
         env = {"Environment": variables, "Values": values}
         return env
 
     @property
-    def python_version(self):
+    def python_version(self) -> str:
         return platform.python_version()
 
-    def is_compatible_python(self, python_min):
+    def is_compatible_python(self, python_min: float) -> bool:
         """Detect if system Python is too old"""
         sys_py = sys.version_info
         system_python = Version_(f"{sys_py.major}.{sys_py.minor}.{sys_py.micro}")
         return system_python > python_min
 
-    def is_windows(self):
+    def is_windows(self) -> bool:
         return self.PLATFORM in ["win32", "cygwin", "msys"]
 
-    def is_macos(self):
+    def is_macos(self) -> bool:
         return self.PLATFORM == "darwin"
 
     @property
-    def torch_cmake_path(self):
+    def torch_cmake_path(self) -> t.Optional[str]:
         """Find the path to the cmake directory within a
         pip installed pytorch package"""
 
-        def _torch_import_path():
+        def _torch_import_path() -> t.Optional[Path]:
             """Find through importing torch"""
             try:
                 import torch as t
 
                 torch_paths = [Path(p) for p in t.__path__]
                 for _path in torch_paths:
                     torch_path = _path / "share/cmake/Torch"
                     if torch_path.is_dir():
                         return torch_path
                 return None
             except ModuleNotFoundError:
                 return None
 
-        def _torch_site_path():
+        def _torch_site_path() -> t.Optional[Path]:
             """find torch through site packages"""
             site_paths = [Path(p) for p in site.getsitepackages()]
 
             # check user site (~/.local/lib)
-            if Path(site.USER_SITE).is_dir():
+            if site.USER_SITE and Path(site.USER_SITE).is_dir():
                 site_paths.append(Path(site.USER_SITE))
 
             for _path in site_paths:
                 torch_path = _path / "torch/share/cmake/Torch"
                 if torch_path.is_dir():
                     return torch_path
             return None
@@ -492,28 +491,28 @@
         if not torch_path:
             torch_path = _torch_site_path()
         if not torch_path:
             raise SetupError("Could not locate torch cmake path")
         return str(torch_path)
 
     @staticmethod
-    def get_cudnn_env():
+    def get_cudnn_env() -> t.Optional[t.Dict[str, str]]:
         """Collect the environment variables needed for Caffe (Pytorch)
         and throw an error if they are not found
 
         Specifically make sure to set at least one set of:
             - CUDNN_LIBRARY and CUDNN_INCLUDE_DIR
                 or
             - CUDNN_LIBRARY_PATH and CUDNN_INCLUDE_PATH
         """
         env = {
-            "CUDNN_LIBRARY": os.environ.get("CUDNN_LIBRARY", None),
-            "CUDNN_INCLUDE_DIR": os.environ.get("CUDNN_INCLUDE_DIR", None),
-            "CUDNN_LIBRARY_PATH": os.environ.get("CUDNN_LIBRARY_PATH", None),
-            "CUDNN_INCLUDE_PATH": os.environ.get("CUDNN_INCLUDE_PATH", None),
+            "CUDNN_LIBRARY": os.environ.get("CUDNN_LIBRARY", "env-var-not-found"),
+            "CUDNN_INCLUDE_DIR": os.environ.get("CUDNN_INCLUDE_DIR", "env-var-not-found"),
+            "CUDNN_LIBRARY_PATH": os.environ.get("CUDNN_LIBRARY_PATH", "env-var-not-found"),
+            "CUDNN_INCLUDE_PATH": os.environ.get("CUDNN_INCLUDE_PATH", "env-var-not-found"),
         }
         torch_cudnn_vars = ["CUDNN_LIBRARY", "CUDNN_INCLUDE_DIR"]
         caffe_cudnn_vars = ["CUDNN_INCLUDE_PATH", "CUDNN_LIBRARY_PATH"]
 
         torch_set = all([var in os.environ for var in torch_cudnn_vars])
         caffe_set = all([var in os.environ for var in caffe_cudnn_vars])
 
@@ -525,27 +524,27 @@
             env["CUDNN_INCLUDE_PATH"] = env["CUDNN_INCLUDE_DIR"]
             env["CUDNN_LIBRARY_PATH"] = env["CUDNN_LIBRARY"]
         elif caffe_set and not torch_set:
             env["CUDNN_INCLUDE_DIR"] = env["CUDNN_INCLUDE_PATH"]
             env["CUDNN_LIBRARY"] = env["CUDNN_LIBRARY_PATH"]
         return env
 
-    def check_build_dependency(self, command):
+    def check_build_dependency(self, command: str) -> None:
         # TODO expand this to parse and check versions.
         try:
             subprocess.check_call(
                 [command, "--version"],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
         except OSError:
             raise SetupError(f"{command} must be installed to build SmartSim") from None
 
     @staticmethod
-    def check_installed(package, version=None):
+    def check_installed(package: str, version: t.Optional[Version_] = None) -> bool:
         """Check if a package is installed. If version is provided, check if
         it's a compatible version. (major and minor the same)"""
         try:
             installed = Version_(pkg_resources.get_distribution(package).version)
             if version:
                 # detect if major or minor versions differ
                 if installed.major != version.major or installed.minor != version.minor:
```

### Comparing `smartsim-0.4.2/smartsim/_core/_install/builder.py` & `smartsim-0.5.0/smartsim/_core/_install/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,27 +26,28 @@
 
 import os
 import re
 import shutil
 import stat
 import subprocess
 import sys
+import typing as t
 from pathlib import Path
 from shutil import which
 from subprocess import SubprocessError
 
 # NOTE: This will be imported by setup.py and hence no
 #       smartsim related items should be imported into
 #       this file.
 
 # TODO:
 #   - check cmake version and use system if possible to avoid conflicts
 
 
-def expand_exe_path(exe):
+def expand_exe_path(exe: str) -> str:
     """Takes an executable and returns the full path to that executable
 
     :param exe: executable or file
     :type exe: str
     :raises TypeError: if file is not an executable
     :raises FileNotFoundError: if executable cannot be found
     """
@@ -75,16 +76,18 @@
         r"localhost|"  # localhost...
         r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"  # ...or ip
         r"(?::\d+)?"  # optional port
         r"(?:/?|[/?]\S+)$",
         re.IGNORECASE,
     )
 
-    def __init__(self, env, jobs=1, verbose=False):
-
+    def __init__(self,
+                 env: t.Dict[str, t.Any],
+                 jobs: t.Optional[int] = 1,
+                 verbose: bool = False) -> None:
         # build environment from buildenv
         self.env = env
 
         # Find _core directory and set up paths
         _core_dir = Path(os.path.abspath(__file__)).parent.parent
 
         dependency_path = _core_dir
@@ -93,15 +96,15 @@
 
         self.build_dir = _core_dir / ".third-party"
 
         self.bin_path = dependency_path / "bin"
         self.lib_path = dependency_path / "lib"
 
         # Set wether build process will output to std output
-        self.out = subprocess.DEVNULL
+        self.out: t.Optional[int] = subprocess.DEVNULL
         self.verbose = verbose
         if self.verbose:
             self.out = None
 
         # make build directory "SmartSim/smartsim/_core/.third-party"
         if not self.build_dir.is_dir():
             self.build_dir.mkdir()
@@ -111,50 +114,54 @@
             if not self.lib_path.is_dir():
                 self.lib_path.mkdir()
 
         self.jobs = jobs
 
     # implemented in base classes
     @property
-    def is_built(self):
+    def is_built(self) -> bool:
         raise NotImplementedError
 
-    def build_from_git(self):
+    def build_from_git(self, git_url: str, branch: str, device: str = "cpu") -> None:
         raise NotImplementedError
 
-    def binary_path(self, binary):
+    def binary_path(self, binary: str) -> str:
         binary_ = shutil.which(binary)
         if binary_:
             return binary_
         raise BuildError(f"{binary} not found in PATH")
 
-    def copy_file(self, src, dst, set_exe=False):
+    def copy_file(self, src: t.Union[str, Path], dst: t.Union[str, Path], set_exe: bool = False) -> None:
         shutil.copyfile(src, dst)
         if set_exe:
             Path(dst).chmod(stat.S_IXUSR | stat.S_IWUSR | stat.S_IRUSR)
 
-    def copy_dir(self, src, dst, set_exe=False):
+    def copy_dir(self, src: t.Union[str, Path], dst: t.Union[str, Path], set_exe: bool = False) -> None:
         src = Path(src)
         dst = Path(dst)
         dst.mkdir(exist_ok=True)
         # copy directory contents
         for content in src.glob("*"):
             if content.is_dir():
                 self.copy_dir(content, dst / content.name, set_exe=set_exe)
             else:
                 self.copy_file(content, dst / content.name, set_exe=set_exe)
 
-    def is_valid_url(self, url):
+    def is_valid_url(self, url: str) -> bool:
         return re.match(self.url_regex, url) is not None
 
-    def cleanup(self):
+    def cleanup(self) -> None:
         if self.build_dir.is_dir():
             shutil.rmtree(str(self.build_dir))
 
-    def run_command(self, cmd, shell=False, out=None, cwd=None):
+    def run_command(self,
+                    cmd: t.List[str],
+                    shell: bool = False,
+                    out: t.Optional[int] = None,
+                    cwd: t.Union[str, Path, None] = None) -> None:
         # option to manually disable output if necessary
         if not out:
             out = self.out
         try:
             proc = subprocess.Popen(
                 cmd,
                 stderr=subprocess.PIPE,
@@ -174,27 +181,31 @@
     """Class to build Redis or KeyDB from Source
     Supported build methods:
      - from git
     See buildenv.py for buildtime configuration of Redis/KeyDB
     version and url.
     """
 
-    def __init__(self, build_env={}, malloc="libc", jobs=None, verbose=False):
+    def __init__(self, 
+                 build_env: t.Dict[str, t.Any] = {},
+                 malloc: str = "libc",
+                 jobs: t.Optional[int] = None,
+                 verbose: bool = False) -> None:
         super().__init__(build_env, jobs=jobs, verbose=verbose)
         self.malloc = malloc
 
     @property
-    def is_built(self):
+    def is_built(self) -> bool:
         """Check if Redis or KeyDB is built"""
         bin_files = {file.name for file in self.bin_path.iterdir()}
         redis_files = {"redis-server", "redis-cli"}
         keydb_files = {"keydb-server", "keydb-cli"}
         return redis_files.issubset(bin_files) or keydb_files.issubset(bin_files)
 
-    def build_from_git(self, git_url, branch):
+    def build_from_git(self, git_url: str, branch: str, device: str = "cpu") -> None:
         """Build Redis from git
         :param git_url: url from which to retrieve Redis
         :type git_url: str
         :param branch: branch to checkout
         :type branch: str
         """
         database_name = "keydb" if "KeyDB" in git_url else "redis"
@@ -270,58 +281,58 @@
      - from git
     See buildenv.py for buildtime configuration of RedisAI
     version and url.
     """
 
     def __init__(
         self,
-        build_env={},
-        torch_dir="",
-        libtf_dir="",
-        build_torch=True,
-        build_tf=True,
-        build_onnx=False,
-        jobs=None,
-        verbose=False,
-    ):
+        build_env: t.Dict[str, t.Any]={},
+        torch_dir: str = "",
+        libtf_dir: str = "",
+        build_torch: bool = True,
+        build_tf: bool = True,
+        build_onnx: bool = False,
+        jobs: t.Optional[int ] = None,
+        verbose: bool = False,
+    ) -> None:
         super().__init__(build_env, jobs=jobs, verbose=verbose)
 
         # convert to int for RAI build script
         self.torch = 1 if build_torch else 0
         self.tf = 1 if build_tf else 0
         self.onnx = 1 if build_onnx else 0
         self.libtf_dir = libtf_dir
         self.torch_dir = torch_dir
 
     @property
-    def rai_build_path(self):
+    def rai_build_path(self) -> Path:
         return Path(self.build_dir, "RedisAI")
 
     @property
-    def is_built(self):
+    def is_built(self) -> bool:
         server = self.lib_path.joinpath("backends").is_dir()
         cli = self.lib_path.joinpath("redisai.so").is_file()
         return server and cli
 
-    def copy_tf_cmake(self):
+    def copy_tf_cmake(self) -> None:
         """Copy the FindTensorFlow.cmake file to the build directory
         as the version included in RedisAI is out of date for us.
         Note: opt/cmake/modules removed in RedisAI v1.2.5
         """
         # remove the previous version
         tf_cmake = self.rai_build_path / "opt/cmake/modules/FindTensorFlow.cmake"
         tf_cmake.resolve()
         if tf_cmake.is_file():
             tf_cmake.unlink()
             # copy ours in
             self.copy_file(
                 self.bin_path / "modules/FindTensorFlow.cmake", tf_cmake, set_exe=False
             )
 
-    def symlink_libtf(self, device):
+    def symlink_libtf(self, device: str) -> None:
         """Add symbolic link to available libtensorflow in RedisAI deps.
 
         :param device: cpu or gpu
         :type device: str
         """
         rai_deps_path = sorted(
             self.rai_build_path.glob(os.path.join("deps", f"*{device}*"))
@@ -368,15 +379,15 @@
                 )
 
         for src_file in library_files:
             dst_file = rai_libtf_lib_dir / src_file.name
             if not dst_file.is_file():
                 os.symlink(src_file, dst_file)
 
-    def build_from_git(self, git_url, branch, device):
+    def build_from_git(self, git_url: str, branch: str, device: str = "cpu") -> None:
         """Build RedisAI from git
         :param git_url: url from which to retrieve RedisAI
         :type git_url: str
         :param branch: branch to checkout
         :type branch: str
         :param device: cpu or gpu
         :type device: str
@@ -394,14 +405,17 @@
             self.binary_path("env"),
             "GIT_LFS_SKIP_SMUDGE=1",
             "git",
             "clone",
             "--recursive",
             git_url,
         ]
+        
+        checkout_osx_fix: t.List[str] = []
+
         # Circumvent a bad `get_deps.sh` script from RAI on 1.2.7 with ONNX
         # TODO: Look for a better way to do this or wait for RAI patch
         if sys.platform == "darwin" and branch == "v1.2.7" and self.onnx:
             # Clone RAI patch commit for OSX
             clone_cmd += ["RedisAI"]
             checkout_osx_fix = [
                 "git",
@@ -411,16 +425,15 @@
         else:
             # Clone RAI release commit
             clone_cmd += [
                 "--branch",
                 branch,
                 "--depth=1",
                 "RedisAI",
-            ]
-            checkout_osx_fix = []
+            ]            
 
         self.run_command(clone_cmd, out=subprocess.DEVNULL, cwd=self.build_dir)
         if checkout_osx_fix:
             self.run_command(
                 checkout_osx_fix, out=subprocess.DEVNULL, cwd=self.rai_build_path
             )
 
@@ -432,25 +445,25 @@
             self.binary_path("env"),
             f"WITH_PT=0",  # torch is always 0 because we never use the torch from RAI
             f"WITH_TF={1 if self.tf and not self.libtf_dir else 0}",
             f"WITH_TFLITE=0",  # never build with TF lite (for now)
             f"WITH_ORT={self.onnx}",
             "VERBOSE=1",
             self.binary_path("bash"),
-            self.rai_build_path / "get_deps.sh",
-            device,
+            str(self.rai_build_path / "get_deps.sh"),
+            str(device),
         ]
 
         self.run_command(
             dep_cmd,
             out=subprocess.DEVNULL,  # suppress this as it's not useful
             cwd=self.rai_build_path,
         )
 
-        if self.libtf_dir:
+        if self.libtf_dir and device:
             self.symlink_libtf(device)
 
         build_cmd = [
             self.binary_path("env"),
             f"WITH_PT={self.torch}",  # but we built it in if the user specified it
             f"WITH_TF={self.tf}",
             f"WITH_TFLITE=0",  # never build TF Lite
@@ -479,30 +492,30 @@
         self.run_command(build_cmd, cwd=self.rai_build_path)
 
         self._install_backends(device)
         if self.torch:
             self._move_torch_libs()
         self.cleanup()
 
-    def _install_backends(self, device):
+    def _install_backends(self, device: str) -> None:
         """Move backend libraries to smartsim/_core/lib/
         :param device: cpu or cpu
         :type device: str
         """
         self.rai_install_path = self.rai_build_path.joinpath(
             f"install-{device}"
         ).resolve()
         rai_lib = self.rai_install_path / "redisai.so"
         rai_backends = self.rai_install_path / "backends"
 
         if rai_lib.is_file() and rai_backends.is_dir():
             self.copy_dir(rai_backends, self.lib_path / "backends", set_exe=True)
             self.copy_file(rai_lib, self.lib_path / "redisai.so", set_exe=True)
 
-    def _move_torch_libs(self):
+    def _move_torch_libs(self) -> None:
         """Move pip install torch libraries
         Since we use pip installed torch libraries for building
         RedisAI, we need to move them into the LD_runpath of redisai.so
         in the smartsim/_core/lib directory.
         """
 
         ss_rai_torch_path = self.lib_path / "backends" / "redisai_torch"
```

### Comparing `smartsim-0.4.2/smartsim/_core/bin/modules/FindTensorFlow.cmake` & `smartsim-0.5.0/smartsim/_core/bin/modules/FindTensorFlow.cmake`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/config/__init__.py` & `smartsim-0.5.0/smartsim/_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/config/config.py` & `smartsim-0.5.0/smartsim/_core/config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,42 +21,43 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
+import psutil
+import typing as t
+
 from functools import lru_cache
 from pathlib import Path
 
-import psutil
-
 from ...error import SSConfigError
 from ..utils.helpers import expand_exe_path
 
 # Configuration Values
 #
 # These values can be set through environment variables to
 # override the default behavior of SmartSim.
 #
 # RAI_PATH
 #   - Path to the RAI shared library
 #   - Default: /smartsim/smartsim/_core/lib/redisai.so
 #
 # REDIS_CONF
 #   - Path to the redis.conf file
-#   - Default: /SmartSim/smartsim/config/redis6.conf
+#   - Default: /SmartSim/smartsim/_core/config/redis.conf
 #
 # REDIS_PATH
 #   - Path to the redis-server executable
-#   - Default: /SmartSim/smartsim/bin/redis-server
+#   - Default: /SmartSim/smartsim/_core/bin/redis-server
 #
 # REDIS_CLI_PATH
 #   - Path to the redis-cli executable
-#   - Default: /SmartSim/smartsim/bin/redis-cli
+#   - Default: /SmartSim/smartsim/_core/bin/redis-cli
 #
 # SMARTSIM_LOG_LEVEL
 #   - Log level for SmartSim
 #   - Default: info
 #
 # SMARTSIM_JM_INTERVAL
 #   - polling interval for communication with scheduler
@@ -74,29 +75,33 @@
 #  - type of launcher to use for testing
 #  - Default: Local
 #
 # SMARTSIM_TEST_DEVICE
 #  - CPU or GPU for model serving tests
 #  - Default: CPU
 #
+# SMARTSIM_TEST_NUM_GPUS
+#  - Number of GPUs on the host for testing
+#  - Defaults: 1
+#
 # SMARTSIM_TEST_ACCOUNT
 #  - Account used to run full launcher test suite on external systems
 #  - Default: None
 
 
 class Config:
-    def __init__(self):
+    def __init__(self) -> None:
         # SmartSim/smartsim/_core
         self.core_path = Path(os.path.abspath(__file__)).parent.parent
 
         dependency_path = os.environ.get("SMARTSIM_DEP_INSTALL_PATH", self.core_path)
 
         self.lib_path = Path(dependency_path, "lib").resolve()
         self.bin_path = Path(dependency_path, "bin").resolve()
-        self.conf_path = Path(dependency_path, "config", "redis6.conf")
+        self.conf_path = Path(dependency_path, "config", "redis.conf")
 
     @property
     def redisai(self) -> str:
         rai_path = self.lib_path / "redisai.so"
         redisai = Path(os.environ.get("RAI_PATH", rai_path)).resolve()
         if not redisai.is_file():
             raise SSConfigError(
@@ -139,51 +144,59 @@
 
     @property
     def log_level(self) -> str:
         return os.environ.get("SMARTSIM_LOG_LEVEL", "info")
 
     @property
     def jm_interval(self) -> int:
-        return int(os.environ.get("SMARTSIM_JM_INTERVAL", 10))
+        return int(os.environ.get("SMARTSIM_JM_INTERVAL") or 10)
 
     @property
     def wlm_trials(self) -> int:
-        return int(os.environ.get("SMARTSIM_WLM_TRIALS", 10))
+        return int(os.environ.get("SMARTSIM_WLM_TRIALS") or 10)
 
     @property
-    def test_launcher(self) -> str:
+    def test_launcher(self) -> str:  # pragma: no cover
         return os.environ.get("SMARTSIM_TEST_LAUNCHER", "local")
 
     @property
-    def test_device(self) -> str:
+    def test_device(self) -> str:  # pragma: no cover
         return os.environ.get("SMARTSIM_TEST_DEVICE", "CPU")
 
     @property
-    def test_port(self) -> int:
+    def test_num_gpus(self) -> int:  # pragma: no cover
+        return int(os.environ.get("SMARTSIM_TEST_NUM_GPUS") or 1)
+
+    @property
+    def test_port(self) -> int:  # pragma: no cover
         return int(os.environ.get("SMARTSIM_TEST_PORT", 6780))
 
     @property
-    def test_interface(self) -> str:
-        interface = os.environ.get("SMARTSIM_TEST_INTERFACE", None)
-        if not interface:
-            # try to pick a sensible one
-            net_if_addrs = psutil.net_if_addrs()
-            if "ipogif0" in net_if_addrs:
-                return "ipogif0"
-            elif "ib0" in net_if_addrs:
-                return "ib0"
-            # default to aries network
-            return "ipogif0"
-        else:
-            return interface
+    def test_interface(self) -> t.List[str]:  # pragma: no cover
+        if interfaces_cfg := os.environ.get("SMARTSIM_TEST_INTERFACE", None):
+            return interfaces_cfg.split(",")
+
+        # try to pick a sensible one
+        net_if_addrs = psutil.net_if_addrs()
+        if "ipogif0" in net_if_addrs:
+            return ["ipogif0"]
+        elif "hsn0" in net_if_addrs:
+            return [
+                net_if_addr
+                for net_if_addr in net_if_addrs
+                if net_if_addr.startswith("hsn")
+            ]
+        elif "ib0" in net_if_addrs:
+            return ["ib0"]
+        # default to aries network
+        return ["lo"]
 
     @property
-    def test_account(self) -> str:
+    def test_account(self) -> t.Optional[str]:  # pragma: no cover
         # no account by default
-        return os.environ.get("SMARTSIM_TEST_ACCOUNT", "")
+        return os.environ.get("SMARTSIM_TEST_ACCOUNT", None)
 
 
 @lru_cache(maxsize=128, typed=False)
-def get_config():
-
+def get_config() -> Config:
     # wrap into a function with a cached result
     return Config()
```

### Comparing `smartsim-0.4.2/smartsim/_core/config/keydb.conf` & `smartsim-0.5.0/smartsim/_core/config/keydb.conf`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/config/redis6.conf` & `smartsim-0.5.0/smartsim/_core/config/redis.conf`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,25 @@
 # from admin or Redis Sentinel. Since Redis always uses the last processed
 # line as value of a configuration directive, you'd better put includes
 # at the beginning of this file to avoid overwriting config change at runtime.
 #
 # If instead you are interested in using includes to override configuration
 # options, it is better to use include as the last line.
 #
+# Included paths may contain wildcards. All files matching the wildcards will
+# be included in alphabetical order.
+# Note that if an include path contains a wildcards but no files match it when
+# the server is started, the include statement will be ignored and no error will
+# be emitted.  It is safe, therefore, to include wildcard files from empty
+# directories.
+#
 # include /path/to/local.conf
 # include /path/to/other.conf
+# include /path/to/fragments/*.conf
+#
 
 ################################## MODULES #####################################
 
 # Load modules at startup. If the server is not able to load modules
 # it will abort. It is possible to use multiple loadmodule directives.
 #
 # loadmodule /path/to/my_module.so
@@ -45,51 +54,89 @@
 
 ################################## NETWORK #####################################
 
 # By default, if no "bind" configuration directive is specified, Redis listens
 # for connections from all available network interfaces on the host machine.
 # It is possible to listen to just one or multiple selected interfaces using
 # the "bind" configuration directive, followed by one or more IP addresses.
+# Each address can be prefixed by "-", which means that redis will not fail to
+# start if the address is not available. Being not available only refers to
+# addresses that does not correspond to any network interface. Addresses that
+# are already in use will always fail, and unsupported protocols will always BE
+# silently skipped.
 #
 # Examples:
 #
-# bind 192.168.1.100 10.0.0.1
-# bind 127.0.0.1 ::1
+# bind 192.168.1.100 10.0.0.1     # listens on two specific IPv4 addresses
+# bind 127.0.0.1 ::1              # listens on loopback IPv4 and IPv6
+# bind * -::*                     # like the default, all available interfaces
 #
 # ~~~ WARNING ~~~ If the computer running Redis is directly exposed to the
 # internet, binding to all the interfaces is dangerous and will expose the
 # instance to everybody on the internet. So by default we uncomment the
 # following bind directive, that will force Redis to listen only on the
-# IPv4 loopback interface address (this means Redis will only be able to
-# accept client connections from the same host that it is running on).
+# IPv4 and IPv6 (if available) loopback interface addresses (this means Redis
+# will only be able to accept client connections from the same host that it is
+# running on).
 #
 # IF YOU ARE SURE YOU WANT YOUR INSTANCE TO LISTEN TO ALL THE INTERFACES
-# JUST COMMENT OUT THE FOLLOWING LINE.
+# COMMENT OUT THE FOLLOWING LINE.
+#
+# You will also need to set a password unless you explicitly disable protected
+# mode.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-#bind 127.0.0.1
+#bind 127.0.0.1 -::1
+
+# By default, outgoing connections (from replica to master, from Sentinel to
+# instances, cluster bus, etc.) are not bound to a specific local address. In
+# most cases, this means the operating system will handle that based on routing
+# and the interface through which the connection goes out.
+#
+# Using bind-source-addr it is possible to configure a specific address to bind
+# to, which may also affect how the connection gets routed.
+#
+# Example:
+#
+# bind-source-addr 10.0.0.1
 
 # Protected mode is a layer of security protection, in order to avoid that
 # Redis instances left open on the internet are accessed and exploited.
 #
-# When protected mode is on and if:
-#
-# 1) The server is not binding explicitly to a set of addresses using the
-#    "bind" directive.
-# 2) No password is configured.
-#
-# The server only accepts connections from clients connecting from the
-# IPv4 and IPv6 loopback addresses 127.0.0.1 and ::1, and from Unix domain
-# sockets.
+# When protected mode is on and the default user has no password, the server
+# only accepts local connections from the IPv4 address (127.0.0.1), IPv6 address
+# (::1) or Unix domain sockets.
 #
 # By default protected mode is enabled. You should disable it only if
 # you are sure you want clients from other hosts to connect to Redis
-# even if no authentication is configured, nor a specific set of interfaces
-# are explicitly listed using the "bind" directive.
+# even if no authentication is configured.
 protected-mode no
 
+# Redis uses default hardened security configuration directives to reduce the
+# attack surface on innocent users. Therefore, several sensitive configuration
+# directives are immutable, and some potentially-dangerous commands are blocked.
+#
+# Configuration directives that control files that Redis writes to (e.g., 'dir'
+# and 'dbfilename') and that aren't usually modified during runtime
+# are protected by making them immutable.
+#
+# Commands that can increase the attack surface of Redis and that aren't usually
+# called by users are blocked by default.
+#
+# These can be exposed to either all connections or just local ones by setting
+# each of the configs listed below to either of these values:
+#
+# no    - Block for any connection (remain immutable)
+# yes   - Allow for any connection (no protection)
+# local - Allow only for local connections. Ones originating from the
+#         IPv4 address (127.0.0.1), IPv6 address (::1) or Unix domain sockets.
+#
+# enable-protected-configs no
+# enable-debug-command no
+# enable-module-command no
+
 # Accept connections on the specified port, default is 6379 (IANA #815344).
 # If port 0 is specified Redis will not listen on a TCP socket.
 port 6379
 
 # TCP listen() backlog.
 #
 # In high requests-per-second environments you need a high backlog in order
@@ -101,15 +148,15 @@
 
 # Unix socket.
 #
 # Specify the path for the Unix socket that will be used to listen for
 # incoming connections. There is no default, so Redis will not listen
 # on a unix socket when not specified.
 #
-# unixsocket /tmp/redis.sock
+# unixsocket /tmp/redis.socket
 # unixsocketperm 700
 
 # Close the connection after a client is idle for N seconds (0 to disable)
 timeout 0
 
 # TCP keepalive.
 #
@@ -124,14 +171,24 @@
 # Note that to close the connection the double of the time is needed.
 # On other kernels the period depends on the kernel configuration.
 #
 # A reasonable value for this option is 300 seconds, which is the new
 # Redis default starting with Redis 3.2.1.
 tcp-keepalive 300
 
+# Apply OS-specific mechanism to mark the listening socket with the specified
+# ID, to support advanced routing and filtering capabilities.
+#
+# On Linux, the ID represents a connection mark.
+# On FreeBSD, the ID represents a socket cookie ID.
+# On OpenBSD, the ID represents a route table ID.
+#
+# The default value is 0, which implies no marking is required.
+# socket-mark-id 0
+
 ################################# TLS/SSL #####################################
 
 # By default, TLS/SSL is disabled. To enable it, the "tls-port" configuration
 # directive can be used to define TLS-listening ports. To enable TLS on the
 # default port, use:
 #
 # port 0
@@ -139,16 +196,40 @@
 
 # Configure a X.509 certificate and private key to use for authenticating the
 # server to connected clients, masters or cluster peers.  These files should be
 # PEM formatted.
 #
 # tls-cert-file redis.crt
 # tls-key-file redis.key
+#
+# If the key file is encrypted using a passphrase, it can be included here
+# as well.
+#
+# tls-key-file-pass secret
+
+# Normally Redis uses the same certificate for both server functions (accepting
+# connections) and client functions (replicating from a master, establishing
+# cluster bus connections, etc.).
+#
+# Sometimes certificates are issued with attributes that designate them as
+# client-only or server-only certificates. In that case it may be desired to use
+# different certificates for incoming (server) and outgoing (client)
+# connections. To do that, use the following directives:
+#
+# tls-client-cert-file client.crt
+# tls-client-key-file client.key
+#
+# If the key file is encrypted using a passphrase, it can be included here
+# as well.
+#
+# tls-client-key-file-pass secret
 
-# Configure a DH parameters file to enable Diffie-Hellman (DH) key exchange:
+# Configure a DH parameters file to enable Diffie-Hellman (DH) key exchange,
+# required by older versions of OpenSSL (<3.0). Newer versions do not require
+# this configuration and recommend against it.
 #
 # tls-dh-params-file redis.dh
 
 # Configure a CA certificate(s) bundle or directory to authenticate TLS/SSL
 # clients and peers.  Redis requires an explicit configuration of at least one
 # of these, and will not implicitly use the system wide configuration.
 #
@@ -173,17 +254,20 @@
 # tls-replication yes
 
 # By default, the Redis Cluster bus uses a plain TCP connection. To enable
 # TLS for the bus protocol, use the following directive:
 #
 # tls-cluster yes
 
-# Explicitly specify TLS versions to support. Allowed values are case insensitive
-# and include "TLSv1", "TLSv1.1", "TLSv1.2", "TLSv1.3" (OpenSSL >= 1.1.1) or
-# any combination. To enable only TLSv1.2 and TLSv1.3, use:
+# By default, only TLSv1.2 and TLSv1.3 are enabled and it is highly recommended
+# that older formally deprecated versions are kept disabled to reduce the attack surface.
+# You can explicitly specify TLS versions to support.
+# Allowed values are case insensitive and include "TLSv1", "TLSv1.1", "TLSv1.2",
+# "TLSv1.3" (OpenSSL >= 1.1.1) or any combination.
+# To enable only TLSv1.2 and TLSv1.3, use:
 #
 # tls-protocols "TLSv1.2 TLSv1.3"
 
 # Configure allowed ciphers.  See the ciphers(1ssl) manpage for more information
 # about the syntax of this string.
 #
 # Note: this configuration applies only to <= TLSv1.2.
@@ -217,37 +301,47 @@
 #
 # tls-session-cache-timeout 60
 
 ################################# GENERAL #####################################
 
 # By default Redis does not run as a daemon. Use 'yes' if you need it.
 # Note that Redis will write a pid file in /var/run/redis.pid when daemonized.
+# When Redis is supervised by upstart or systemd, this parameter has no impact.
 daemonize no
 
 # If you run Redis from upstart or systemd, Redis can interact with your
 # supervision tree. Options:
 #   supervised no      - no supervision interaction
 #   supervised upstart - signal upstart by putting Redis into SIGSTOP mode
 #                        requires "expect stop" in your upstart job config
 #   supervised systemd - signal systemd by writing READY=1 to $NOTIFY_SOCKET
+#                        on startup, and updating Redis status on a regular
+#                        basis.
 #   supervised auto    - detect upstart or systemd method based on
 #                        UPSTART_JOB or NOTIFY_SOCKET environment variables
 # Note: these supervision methods only signal "process is ready."
 #       They do not enable continuous pings back to your supervisor.
+#
+# The default is "no". To run under upstart/systemd, you can simply uncomment
+# the line below:
+#
 supervised no
 
 # If a pid file is specified, Redis writes it where specified at startup
 # and removes it at exit.
 #
 # When the server runs non daemonized, no pid file is created if none is
 # specified in the configuration. When the server is daemonized, the pid file
 # is used even if not specified, defaulting to "/var/run/redis.pid".
 #
 # Creating a pid file is best effort: if Redis is not able to create it
 # nothing bad happens, the server will start and run normally.
+#
+# Note that on modern Linux systems "/run/redis.pid" is more conforming
+# and should be used instead.
 pidfile /var/run/redis_6379.pid
 
 # Specify the server verbosity level.
 # This can be one of:
 # debug (a lot of information, useful for development/testing)
 # verbose (many rarely useful info, but not a mess like the debug level)
 # notice (moderately verbose, what you want in production probably)
@@ -265,52 +359,83 @@
 
 # Specify the syslog identity.
 # syslog-ident redis
 
 # Specify the syslog facility. Must be USER or between LOCAL0-LOCAL7.
 # syslog-facility local0
 
+# To disable the built in crash log, which will possibly produce cleaner core
+# dumps when they are needed, uncomment the following:
+#
+# crash-log-enabled no
+
+# To disable the fast memory check that's run as part of the crash log, which
+# will possibly let redis terminate sooner, uncomment the following:
+#
+# crash-memcheck-enabled no
+
 # Set the number of databases. The default database is DB 0, you can select
 # a different one on a per-connection basis using SELECT <dbid> where
 # dbid is a number between 0 and 'databases'-1
 databases 16
 
 # By default Redis shows an ASCII art logo only when started to log to the
-# standard output and if the standard output is a TTY. Basically this means
-# that normally a logo is displayed only in interactive sessions.
+# standard output and if the standard output is a TTY and syslog logging is
+# disabled. Basically this means that normally a logo is displayed only in
+# interactive sessions.
 #
 # However it is possible to force the pre-4.0 behavior and always show a
 # ASCII art logo in startup logs by setting the following option to yes.
 always-show-logo yes
 
+# By default, Redis modifies the process title (as seen in 'top' and 'ps') to
+# provide some runtime information. It is possible to disable this and leave
+# the process name as executed by setting the following to no.
+set-proc-title yes
+
+# When changing the process title, Redis uses the following template to construct
+# the modified title.
+#
+# Template variables are specified in curly brackets. The following variables are
+# supported:
+#
+# {title}           Name of process as executed if parent, or type of child process.
+# {listen-addr}     Bind address or '*' followed by TCP or TLS port listening on, or
+#                   Unix socket if only that's available.
+# {server-mode}     Special mode, i.e. "[sentinel]" or "[cluster]".
+# {port}            TCP port listening on, or 0.
+# {tls-port}        TLS port listening on, or 0.
+# {unixsocket}      Unix domain socket listening on, or "".
+# {config-file}     Name of configuration file used.
+#
+proc-title-template "{title} {listen-addr} {server-mode}"
+
 ################################ SNAPSHOTTING  ################################
+
+# Save the DB to disk.
 #
-# Save the DB on disk:
+# save <seconds> <changes> [<seconds> <changes> ...]
 #
-#   save <seconds> <changes>
+# Redis will save the DB if the given number of seconds elapsed and it
+# surpassed the given number of write operations against the DB.
 #
-#   Will save the DB if both the given number of seconds and the given
-#   number of write operations against the DB occurred.
+# Snapshotting can be completely disabled with a single empty string argument
+# as in following example:
 #
-#   In the example below the behavior will be to save:
-#   after 900 sec (15 min) if at least 1 key changed
-#   after 300 sec (5 min) if at least 10 keys changed
-#   after 60 sec if at least 10000 keys changed
+save ""
+
 #
-#   Note: you can disable saving completely by commenting out all "save" lines.
+# Unless specified otherwise, by default Redis will save the DB:
+#   * After 3600 seconds (an hour) if at least 1 change was performed
+#   * After 300 seconds (5 minutes) if at least 100 changes were performed
+#   * After 60 seconds if at least 10000 changes were performed
 #
-#   It is also possible to remove all the previously configured save
-#   points by adding a save directive with a single empty string argument
-#   like in the following example:
+# You can set these explicitly by uncommenting the following line.
 #
-#   save ""
-
-#save 900 1
-#save 300 10
-#save 60 10000
+# save 3600 1 300 100 60 10000
 
 # By default Redis will stop accepting writes if RDB snapshots are enabled
 # (at least one save point) and the latest background save failed.
 # This will make the user aware (in a hard way) that data is not persisting
 # on disk properly, otherwise chances are that no one will notice and some
 # disaster will happen.
 #
@@ -334,14 +459,29 @@
 # hit to pay (around 10%) when saving and loading RDB files, so you can disable it
 # for maximum performances.
 #
 # RDB files created with checksum disabled have a checksum of zero that will
 # tell the loading code to skip the check.
 rdbchecksum yes
 
+# Enables or disables full sanitization checks for ziplist and listpack etc when
+# loading an RDB or RESTORE payload. This reduces the chances of a assertion or
+# crash later on while processing commands.
+# Options:
+#   no         - Never perform full sanitization
+#   yes        - Always perform full sanitization
+#   clients    - Perform full sanitization only for user connections.
+#                Excludes: RDB files, RESTORE commands received from the master
+#                connection, and client connections which have the
+#                skip-sanitize-payload ACL flag.
+# The default should be 'clients' but since it currently affects cluster
+# resharding via MIGRATE, it is temporarily set to 'no' by default.
+#
+# sanitize-dump-payload no
+
 # The filename where to dump the DB
 dbfilename dump.rdb
 
 # Remove RDB files used by replication in instances without persistence
 # enabled. By default this option is disabled, however there are environments
 # where for regulations or other security concerns, RDB files persisted on
 # disk by masters in order to feed replicas, or stored on disk by replicas
@@ -408,17 +548,18 @@
 # When a replica loses its connection with the master, or when the replication
 # is still in progress, the replica can act in two different ways:
 #
 # 1) if replica-serve-stale-data is set to 'yes' (the default) the replica will
 #    still reply to client requests, possibly with out of date data, or the
 #    data set may just be empty if this is the first synchronization.
 #
-# 2) If replica-serve-stale-data is set to 'no' the replica will reply with
-#    an error "SYNC with master in progress" to all commands except:
-#    INFO, REPLICAOF, AUTH, PING, SHUTDOWN, REPLCONF, ROLE, CONFIG, SUBSCRIBE,
+# 2) If replica-serve-stale-data is set to 'no' the replica will reply with error
+#    "MASTERDOWN Link with MASTER is down and replica-serve-stale-data is set to 'no'"
+#    to all data access commands, excluding commands such as:
+#    INFO, REPLICAOF, AUTH, SHUTDOWN, REPLCONF, ROLE, CONFIG, SUBSCRIBE,
 #    UNSUBSCRIBE, PSUBSCRIBE, PUNSUBSCRIBE, PUBLISH, PUBSUB, COMMAND, POST,
 #    HOST and LATENCY.
 #
 replica-serve-stale-data yes
 
 # You can configure a replica instance to accept writes or not. Writing against
 # a replica instance may be useful to store some ephemeral data (because data
@@ -473,41 +614,51 @@
 # new replicas arriving, that will be queued for the next RDB transfer, so the
 # server waits a delay in order to let more replicas arrive.
 #
 # The delay is specified in seconds, and by default is 5 seconds. To disable
 # it entirely just set it to 0 seconds and the transfer will start ASAP.
 repl-diskless-sync-delay 5
 
+# When diskless replication is enabled with a delay, it is possible to let
+# the replication start before the maximum delay is reached if the maximum
+# number of replicas expected have connected. Default of 0 means that the
+# maximum is not defined and Redis will wait the full delay.
+repl-diskless-sync-max-replicas 0
+
 # -----------------------------------------------------------------------------
 # WARNING: RDB diskless load is experimental. Since in this setup the replica
 # does not immediately store an RDB on disk, it may cause data loss during
 # failovers. RDB diskless load + Redis modules not handling I/O reads may also
 # cause Redis to abort in case of I/O errors during the initial synchronization
-# stage with the master. Use only if your do what you are doing.
+# stage with the master. Use only if you know what you are doing.
 # -----------------------------------------------------------------------------
 #
 # Replica can load the RDB it reads from the replication link directly from the
 # socket, or store the RDB to a file and read that file after it was completely
 # received from the master.
 #
 # In many cases the disk is slower than the network, and storing and loading
 # the RDB file may increase replication time (and even increase the master's
-# Copy on Write memory and salve buffers).
+# Copy on Write memory and replica buffers).
 # However, parsing the RDB file directly from the socket may mean that we have
 # to flush the contents of the current database before the full rdb was
 # received. For this reason we have the following options:
 #
 # "disabled"    - Don't use diskless load (store the rdb file to the disk first)
 # "on-empty-db" - Use diskless load only when it is completely safe.
-# "swapdb"      - Keep a copy of the current db contents in RAM while parsing
-#                 the data directly from the socket. note that this requires
-#                 sufficient memory, if you don't have it, you risk an OOM kill.
+# "swapdb"      - Keep current db contents in RAM while parsing the data directly
+#                 from the socket. Replicas in this mode can keep serving current
+#                 data set while replication is in progress, except for cases where
+#                 they can't recognize master as having a data set from same
+#                 replication history.
+#                 Note that this requires sufficient memory, if you don't have it,
+#                 you risk an OOM kill.
 repl-diskless-load disabled
 
-# Replicas send PINGs to server in a predefined interval. It's possible to
+# Master send PINGs to its replicas in a predefined interval. It's possible to
 # change this interval with the repl_ping_replica_period option. The default
 # value is 10 seconds.
 #
 # repl-ping-replica-period 10
 
 # The following option sets the replication timeout for:
 #
@@ -574,14 +725,51 @@
 # However a special priority of 0 marks the replica as not able to perform the
 # role of master, so a replica with priority of 0 will never be selected by
 # Redis Sentinel for promotion.
 #
 # By default the priority is 100.
 replica-priority 100
 
+# The propagation error behavior controls how Redis will behave when it is
+# unable to handle a command being processed in the replication stream from a master
+# or processed while reading from an AOF file. Errors that occur during propagation
+# are unexpected, and can cause data inconsistency. However, there are edge cases
+# in earlier versions of Redis where it was possible for the server to replicate or persist
+# commands that would fail on future versions. For this reason the default behavior
+# is to ignore such errors and continue processing commands.
+#
+# If an application wants to ensure there is no data divergence, this configuration
+# should be set to 'panic' instead. The value can also be set to 'panic-on-replicas'
+# to only panic when a replica encounters an error on the replication stream. One of
+# these two panic values will become the default value in the future once there are
+# sufficient safety mechanisms in place to prevent false positive crashes.
+#
+# propagation-error-behavior ignore
+
+# Replica ignore disk write errors controls the behavior of a replica when it is
+# unable to persist a write command received from its master to disk. By default,
+# this configuration is set to 'no' and will crash the replica in this condition.
+# It is not recommended to change this default, however in order to be compatible
+# with older versions of Redis this config can be toggled to 'yes' which will just
+# log a warning and execute the write command it got from the master.
+#
+# replica-ignore-disk-write-errors no
+
+# -----------------------------------------------------------------------------
+# By default, Redis Sentinel includes all replicas in its reports. A replica
+# can be excluded from Redis Sentinel's announcements. An unannounced replica
+# will be ignored by the 'sentinel replicas <master>' command and won't be
+# exposed to Redis Sentinel's clients.
+#
+# This option does not change the behavior of replica-priority. Even with
+# replica-announced set to 'no', the replica can be promoted to master. To
+# prevent this behavior, set replica-priority to 0.
+#
+# replica-announced yes
+
 # It is possible for a master to stop accepting writes if there are less than
 # N replicas connected, having a lag less or equal than M seconds.
 #
 # The N replicas need to be in "online" state.
 #
 # The lag in seconds, that must be <= the specified value, is calculated from
 # the last ping received from the replica, that is usually sent every second.
@@ -629,15 +817,15 @@
 # replica-announce-ip 5.5.5.5
 # replica-announce-port 1234
 
 ############################### KEYS TRACKING #################################
 
 # Redis implements server assisted support for client side caching of values.
 # This is implemented using an invalidation table that remembers, using
-# 16 millions of slots, what clients may have certain subsets of keys. In turn
+# a radix key indexed by key name, what clients have which keys. In turn
 # this is used in order to send invalidation messages to clients. Please
 # check this page to understand more about the feature:
 #
 #   https://redis.io/topics/client-side-caching
 #
 # When tracking is enabled for a client, all the read only queries are assumed
 # to be cached: this will force Redis to store information in the invalidation
@@ -693,36 +881,50 @@
 #
 # The ACL rules that describe what a user can do are the following:
 #
 #  on           Enable the user: it is possible to authenticate as this user.
 #  off          Disable the user: it's no longer possible to authenticate
 #               with this user, however the already authenticated connections
 #               will still work.
-#  +<command>   Allow the execution of that command
-#  -<command>   Disallow the execution of that command
+#  skip-sanitize-payload    RESTORE dump-payload sanitization is skipped.
+#  sanitize-payload         RESTORE dump-payload is sanitized (default).
+#  +<command>   Allow the execution of that command.
+#               May be used with `|` for allowing subcommands (e.g "+config|get")
+#  -<command>   Disallow the execution of that command.
+#               May be used with `|` for blocking subcommands (e.g "-config|set")
 #  +@<category> Allow the execution of all the commands in such category
 #               with valid categories are like @admin, @set, @sortedset, ...
 #               and so forth, see the full list in the server.c file where
 #               the Redis command table is described and defined.
 #               The special category @all means all the commands, but currently
 #               present in the server, and that will be loaded in the future
 #               via modules.
-#  +<command>|subcommand    Allow a specific subcommand of an otherwise
-#                           disabled command. Note that this form is not
-#                           allowed as negative like -DEBUG|SEGFAULT, but
-#                           only additive starting with "+".
+#  +<command>|first-arg  Allow a specific first argument of an otherwise
+#                        disabled command. It is only supported on commands with
+#                        no sub-commands, and is not allowed as negative form
+#                        like -SELECT|1, only additive starting with "+". This
+#                        feature is deprecated and may be removed in the future.
 #  allcommands  Alias for +@all. Note that it implies the ability to execute
 #               all the future commands loaded via the modules system.
 #  nocommands   Alias for -@all.
 #  ~<pattern>   Add a pattern of keys that can be mentioned as part of
 #               commands. For instance ~* allows all the keys. The pattern
 #               is a glob-style pattern like the one of KEYS.
 #               It is possible to specify multiple patterns.
+# %R~<pattern>  Add key read pattern that specifies which keys can be read
+#               from.
+# %W~<pattern>  Add key write pattern that specifies which keys can be
+#               written to.
 #  allkeys      Alias for ~*
 #  resetkeys    Flush the list of allowed keys patterns.
+#  &<pattern>   Add a glob-style pattern of Pub/Sub channels that can be
+#               accessed by the user. It is possible to specify multiple channel
+#               patterns.
+#  allchannels  Alias for &*
+#  resetchannels            Flush the list of allowed channel patterns.
 #  ><password>  Add this password to the list of valid password for the user.
 #               For example >mypass will add "mypass" to the list.
 #               This directive clears the "nopass" flag (see later).
 #  <<password>  Remove this password from the list of valid passwords.
 #  nopass       All the set passwords of the user are removed, and the user
 #               is flagged as requiring no password: it means that every
 #               password will work against this user. If this directive is
@@ -733,14 +935,22 @@
 #  resetpass    Flush the list of allowed passwords. Moreover removes the
 #               "nopass" status. After "resetpass" the user has no associated
 #               passwords and there is no way to authenticate without adding
 #               some password (or setting it as "nopass" later).
 #  reset        Performs the following actions: resetpass, resetkeys, off,
 #               -@all. The user returns to the same state it has immediately
 #               after its creation.
+# (<options>)   Create a new selector with the options specified within the
+#               parentheses and attach it to the user. Each option should be
+#               space separated. The first character must be ( and the last
+#               character must be ).
+# clearselectors            Remove all of the currently attached selectors.
+#                           Note this does not change the "root" user permissions,
+#                           which are the permissions directly applied onto the
+#                           user (outside the parentheses).
 #
 # ACL rules can be specified in any order: for instance you can start with
 # passwords, then flags, or key patterns. However note that the additive
 # and subtractive rules will CHANGE MEANING depending on the ordering.
 # For instance see the following example:
 #
 #   user alice on +@all -DEBUG ~* >somepassword
@@ -754,14 +964,48 @@
 #
 # Now DEBUG was removed when alice had yet no commands in the set of allowed
 # commands, later all the commands are added, so the user will be able to
 # execute everything.
 #
 # Basically ACL rules are processed left-to-right.
 #
+# The following is a list of command categories and their meanings:
+# * keyspace - Writing or reading from keys, databases, or their metadata
+#     in a type agnostic way. Includes DEL, RESTORE, DUMP, RENAME, EXISTS, DBSIZE,
+#     KEYS, EXPIRE, TTL, FLUSHALL, etc. Commands that may modify the keyspace,
+#     key or metadata will also have `write` category. Commands that only read
+#     the keyspace, key or metadata will have the `read` category.
+# * read - Reading from keys (values or metadata). Note that commands that don't
+#     interact with keys, will not have either `read` or `write`.
+# * write - Writing to keys (values or metadata)
+# * admin - Administrative commands. Normal applications will never need to use
+#     these. Includes REPLICAOF, CONFIG, DEBUG, SAVE, MONITOR, ACL, SHUTDOWN, etc.
+# * dangerous - Potentially dangerous (each should be considered with care for
+#     various reasons). This includes FLUSHALL, MIGRATE, RESTORE, SORT, KEYS,
+#     CLIENT, DEBUG, INFO, CONFIG, SAVE, REPLICAOF, etc.
+# * connection - Commands affecting the connection or other connections.
+#     This includes AUTH, SELECT, COMMAND, CLIENT, ECHO, PING, etc.
+# * blocking - Potentially blocking the connection until released by another
+#     command.
+# * fast - Fast O(1) commands. May loop on the number of arguments, but not the
+#     number of elements in the key.
+# * slow - All commands that are not Fast.
+# * pubsub - PUBLISH / SUBSCRIBE related
+# * transaction - WATCH / MULTI / EXEC related commands.
+# * scripting - Scripting related.
+# * set - Data type: sets related.
+# * sortedset - Data type: zsets related.
+# * list - Data type: lists related.
+# * hash - Data type: hashes related.
+# * string - Data type: strings related.
+# * bitmap - Data type: bitmaps related.
+# * hyperloglog - Data type: hyperloglog related.
+# * geo - Data type: geo related.
+# * stream - Data type: streams related.
+#
 # For more information about ACL configuration please refer to
 # the Redis web site at https://redis.io/topics/acl
 
 # ACL LOG
 #
 # The ACL Log tracks failed commands and authentication events associated
 # with ACLs. The ACL Log is useful to troubleshoot failed commands blocked
@@ -783,16 +1027,32 @@
 
 # IMPORTANT NOTE: starting with Redis 6 "requirepass" is just a compatibility
 # layer on top of the new ACL system. The option effect will be just setting
 # the password for the default user. Clients will still authenticate using
 # AUTH <password> as usually, or more explicitly with AUTH default <password>
 # if they follow the new protocol: both will work.
 #
+# The requirepass is not compatible with aclfile option and the ACL LOAD
+# command, these will cause requirepass to be ignored.
+#
 # requirepass foobared
 
+# New users are initialized with restrictive permissions by default, via the
+# equivalent of this ACL rule 'off resetkeys -@all'. Starting with Redis 6.2, it
+# is possible to manage access to Pub/Sub channels with ACL rules as well. The
+# default Pub/Sub channels permission if new users is controlled by the
+# acl-pubsub-default configuration directive, which accepts one of these values:
+#
+# allchannels: grants access to all Pub/Sub channels
+# resetchannels: revokes access to all Pub/Sub channels
+#
+# From Redis 7.0, acl-pubsub-default defaults to 'resetchannels' permission.
+#
+# acl-pubsub-default resetchannels
+
 # Command renaming (DEPRECATED).
 #
 # ------------------------------------------------------------------------
 # WARNING: avoid using this option if possible. Instead use ACLs to remove
 # commands from the default user, and put them only in some admin user you
 # create for administrative purposes.
 # ------------------------------------------------------------------------
@@ -873,22 +1133,20 @@
 #
 # LRU means Least Recently Used
 # LFU means Least Frequently Used
 #
 # Both LRU, LFU and volatile-ttl are implemented using approximated
 # randomized algorithms.
 #
-# Note: with any of the above policies, Redis will return an error on write
-#       operations, when there are no suitable keys for eviction.
-#
-#       At the date of writing these commands are: set setnx setex append
-#       incr decr rpush lpush rpushx lpushx linsert lset rpoplpush sadd
-#       sinter sinterstore sunion sunionstore sdiff sdiffstore zadd zincrby
-#       zunionstore zinterstore hset hsetnx hmset hincrby incrby decrby
-#       getset mset msetnx exec sort
+# Note: with any of the above policies, when there are no suitable keys for
+# eviction, Redis will return an error on write operations that require
+# more memory. These are usually commands that create new keys, add data or
+# modify existing keys. A few examples are: SET, INCR, HSET, LPUSH, SUNIONSTORE,
+# SORT (due to the STORE argument), and EXEC (if the transaction includes any
+# command that requires memory).
 #
 # The default is:
 #
 # maxmemory-policy noeviction
 
 # LRU, LFU and minimal TTL algorithms are not precise algorithms but approximated
 # algorithms (in order to save memory), so you can tune it for speed or
@@ -897,14 +1155,22 @@
 # configuration directive.
 #
 # The default of 5 produces good enough results. 10 Approximates very closely
 # true LRU but costs more CPU. 3 is faster but not very accurate.
 #
 # maxmemory-samples 5
 
+# Eviction processing is designed to function well with the default setting.
+# If there is an unusually large amount of write traffic, this value may need to
+# be increased.  Decreasing this value may reduce latency at the risk of
+# eviction processing effectiveness
+#   0 = minimum latency, 10 = default, 100 = process without regard to latency
+#
+# maxmemory-eviction-tenacity 10
+
 # Starting from Redis 5, by default a replica will ignore its maxmemory setting
 # (unless it is promoted to master after a failover or manually). It means
 # that the eviction of keys will be just handled by the master, sending the
 # DEL commands to the replica as keys evict in the master side.
 #
 # This behavior ensures that masters and replicas stay consistent, and is usually
 # what you want, however if your replica is writable, or you want the replica
@@ -990,14 +1256,21 @@
 # It is also possible, for the case when to replace the user code DEL calls
 # with UNLINK calls is not easy, to modify the default behavior of the DEL
 # command to act exactly like UNLINK, using the following configuration
 # directive:
 
 lazyfree-lazy-user-del no
 
+# FLUSHDB, FLUSHALL, SCRIPT FLUSH and FUNCTION FLUSH support both asynchronous and synchronous
+# deletion, which can be controlled by passing the [SYNC|ASYNC] flags into the
+# commands. When neither flag is passed, this directive will be used to determine
+# if the data should be deleted asynchronously.
+
+lazyfree-lazy-user-flush no
+
 ################################ THREADED I/O #################################
 
 # Redis is mostly single threaded, however there are certain threaded
 # operations such as UNLINK, slow I/O accesses and other things that are
 # performed on side threads.
 #
 # Now it is also possible to handle Redis clients socket reads and writes
@@ -1015,28 +1288,28 @@
 # there is no point in using this feature.
 #
 # So for instance if you have a four cores boxes, try to use 2 or 3 I/O
 # threads, if you have a 8 cores, try to use 6 threads. In order to
 # enable I/O threads use the following configuration directive:
 #
 io-threads 4
-
+#
 # Setting io-threads to 1 will just use the main thread as usual.
 # When I/O threads are enabled, we only use threads for writes, that is
 # to thread the write(2) syscall and transfer the client buffers to the
 # socket. However it is also possible to enable threading of reads and
 # protocol parsing using the following configuration directive, by setting
 # it to yes:
 #
 io-threads-do-reads yes
 #
 # Usually threading reads doesn't help much.
 #
 # NOTE 1: This configuration directive cannot be changed at runtime via
-# CONFIG SET. Aso this feature currently does not work when SSL is
+# CONFIG SET. Also, this feature currently does not work when SSL is
 # enabled.
 #
 # NOTE 2: If you want to test the Redis speedup using redis-benchmark, make
 # sure you also run the benchmark itself in threaded mode, using the
 # --threads option to match the number of Redis threads, otherwise you'll not
 # be able to notice the improvements.
 
@@ -1046,15 +1319,15 @@
 # should be killed first when out of memory.
 #
 # Enabling this feature makes Redis actively control the oom_score_adj value
 # for all its processes, depending on their role. The default scores will
 # attempt to have background child processes killed before all others, and
 # replicas killed before masters.
 #
-# Redis supports three options:
+# Redis supports these options:
 #
 # no:       Don't make changes to oom-score-adj (default).
 # yes:      Alias to "relative" see below.
 # absolute: Values in oom-score-adj-values are written as is to the kernel.
 # relative: Values are used relative to the initial value of oom_score_adj when
 #           the server starts and are then clamped to a range of -1000 to 1000.
 #           Because typically the initial value is 0, they will often match the
@@ -1067,14 +1340,27 @@
 #
 # Unprivileged processes (not root, and without CAP_SYS_RESOURCE capabilities)
 # can freely increase their value, but not decrease it below its initial
 # settings. This means that setting oom-score-adj to "relative" and setting the
 # oom-score-adj-values to positive values will always succeed.
 oom-score-adj-values 0 200 800
 
+
+#################### KERNEL transparent hugepage CONTROL ######################
+
+# Usually the kernel Transparent Huge Pages control is set to "madvise" or
+# or "never" by default (/sys/kernel/mm/transparent_hugepage/enabled), in which
+# case this config has no effect. On systems in which it is set to "always",
+# redis will attempt to disable it specifically for the redis process in order
+# to avoid latency problems specifically with fork(2) and CoW.
+# If for some reason you prefer to keep it enabled, you can set this config to
+# "no" and the kernel global to "always".
+
+disable-thp yes
+
 ############################## APPEND ONLY MODE ###############################
 
 # By default Redis asynchronously dumps the dataset on disk. This mode is
 # good enough in many applications, but an issue with the Redis process or
 # a power outage may result into a few minutes of writes lost (depending on
 # the configured save points).
 #
@@ -1085,22 +1371,51 @@
 # wrong with the Redis process itself happens, but the operating system is
 # still running correctly.
 #
 # AOF and RDB persistence can be enabled at the same time without problems.
 # If the AOF is enabled on startup Redis will load the AOF, that is the file
 # with the better durability guarantees.
 #
-# Please check http://redis.io/topics/persistence for more information.
+# Please check https://redis.io/topics/persistence for more information.
 
 appendonly no
 
-# The name of the append only file (default: "appendonly.aof")
+# The base name of the append only file.
+#
+# Redis 7 and newer use a set of append-only files to persist the dataset
+# and changes applied to it. There are two basic types of files in use:
+#
+# - Base files, which are a snapshot representing the complete state of the
+#   dataset at the time the file was created. Base files can be either in
+#   the form of RDB (binary serialized) or AOF (textual commands).
+# - Incremental files, which contain additional commands that were applied
+#   to the dataset following the previous file.
+#
+# In addition, manifest files are used to track the files and the order in
+# which they were created and should be applied.
+#
+# Append-only file names are created by Redis following a specific pattern.
+# The file name's prefix is based on the 'appendfilename' configuration
+# parameter, followed by additional information about the sequence and type.
+#
+# For example, if appendfilename is set to appendonly.aof, the following file
+# names could be derived:
+#
+# - appendonly.aof.1.base.rdb as a base file.
+# - appendonly.aof.1.incr.aof, appendonly.aof.2.incr.aof as incremental files.
+# - appendonly.aof.manifest as a manifest file.
 
 appendfilename "appendonly.aof"
 
+# For convenience, Redis stores all persistent append-only files in a dedicated
+# directory. The name of the directory is determined by the appenddirname
+# configuration parameter.
+
+appenddirname "appendonlydir"
+
 # The fsync() call tells the Operating System to actually write data on disk
 # instead of waiting for more data in the output buffer. Some OS will really flush
 # data on disk, some other OS will just try to do it ASAP.
 #
 # Redis supports three different modes:
 #
 # no: don't fsync, just let the OS flush the data when it wants. Faster.
@@ -1132,15 +1447,15 @@
 # our synchronous write(2) call.
 #
 # In order to mitigate this problem it's possible to use the following option
 # that will prevent fsync() from being called in the main process while a
 # BGSAVE or BGREWRITEAOF is in progress.
 #
 # This means that while another child is saving, the durability of Redis is
-# the same as "appendfsync none". In practical terms, this means that it is
+# the same as "appendfsync no". In practical terms, this means that it is
 # possible to lose up to 30 seconds of log in the worst scenario (with the
 # default Linux settings).
 #
 # If you have latency problems turn this to "yes". Otherwise leave it as
 # "no" that is the safest pick from the point of view of durability.
 
 no-appendfsync-on-rewrite no
@@ -1185,42 +1500,77 @@
 #
 # Note that if the AOF file will be found to be corrupted in the middle
 # the server will still exit with an error. This option only applies when
 # Redis will try to read more data from the AOF file but not enough bytes
 # will be found.
 aof-load-truncated yes
 
-# When rewriting the AOF file, Redis is able to use an RDB preamble in the
-# AOF file for faster rewrites and recoveries. When this option is turned
-# on the rewritten AOF file is composed of two different stanzas:
-#
-#   [RDB file][AOF tail]
-#
-# When loading, Redis recognizes that the AOF file starts with the "REDIS"
-# string and loads the prefixed RDB file, then continues loading the AOF
-# tail.
+# Redis can create append-only base files in either RDB or AOF formats. Using
+# the RDB format is always faster and more efficient, and disabling it is only
+# supported for backward compatibility purposes.
 aof-use-rdb-preamble yes
 
-################################ LUA SCRIPTING  ###############################
-
-# Max execution time of a Lua script in milliseconds.
-#
-# If the maximum execution time is reached Redis will log that a script is
-# still in execution after the maximum allowed time and will start to
-# reply to queries with an error.
-#
-# When a long running script exceeds the maximum execution time only the
-# SCRIPT KILL and SHUTDOWN NOSAVE commands are available. The first can be
-# used to stop a script that did not yet call any write commands. The second
-# is the only way to shut down the server in the case a write command was
-# already issued by the script but the user doesn't want to wait for the natural
-# termination of the script.
-#
-# Set it to 0 or a negative value for unlimited execution without warnings.
-lua-time-limit 5000
+# Redis supports recording timestamp annotations in the AOF to support restoring
+# the data from a specific point-in-time. However, using this capability changes
+# the AOF format in a way that may not be compatible with existing AOF parsers.
+aof-timestamp-enabled no
+
+################################ SHUTDOWN #####################################
+
+# Maximum time to wait for replicas when shutting down, in seconds.
+#
+# During shut down, a grace period allows any lagging replicas to catch up with
+# the latest replication offset before the master exists. This period can
+# prevent data loss, especially for deployments without configured disk backups.
+#
+# The 'shutdown-timeout' value is the grace period's duration in seconds. It is
+# only applicable when the instance has replicas. To disable the feature, set
+# the value to 0.
+#
+# shutdown-timeout 10
+
+# When Redis receives a SIGINT or SIGTERM, shutdown is initiated and by default
+# an RDB snapshot is written to disk in a blocking operation if save points are configured.
+# The options used on signaled shutdown can include the following values:
+# default:  Saves RDB snapshot only if save points are configured.
+#           Waits for lagging replicas to catch up.
+# save:     Forces a DB saving operation even if no save points are configured.
+# nosave:   Prevents DB saving operation even if one or more save points are configured.
+# now:      Skips waiting for lagging replicas.
+# force:    Ignores any errors that would normally prevent the server from exiting.
+#
+# Any combination of values is allowed as long as "save" and "nosave" are not set simultaneously.
+# Example: "nosave force now"
+#
+# shutdown-on-sigint default
+# shutdown-on-sigterm default
+
+################ NON-DETERMINISTIC LONG BLOCKING COMMANDS #####################
+
+# Maximum time in milliseconds for EVAL scripts, functions and in some cases
+# modules' commands before Redis can start processing or rejecting other clients.
+#
+# If the maximum execution time is reached Redis will start to reply to most
+# commands with a BUSY error.
+#
+# In this state Redis will only allow a handful of commands to be executed.
+# For instance, SCRIPT KILL, FUNCTION KILL, SHUTDOWN NOSAVE and possibly some
+# module specific 'allow-busy' commands.
+#
+# SCRIPT KILL and FUNCTION KILL will only be able to stop a script that did not
+# yet call any write commands, so SHUTDOWN NOSAVE may be the only way to stop
+# the server in the case a write command was already issued by the script when
+# the user doesn't want to wait for the natural termination of the script.
+#
+# The default is 5 seconds. It is possible to set it to 0 or a negative value
+# to disable this mechanism (uninterrupted execution). Note that in the past
+# this config had a different name, which is now an alias, so both of these do
+# the same:
+# lua-time-limit 5000
+# busy-reply-threshold 5000
 
 ################################ REDIS CLUSTER  ###############################
 
 # Normal Redis instances can't be part of a Redis Cluster; only nodes that are
 # started as cluster nodes can. In order to start a Redis instance as a
 # cluster node enable the cluster support uncommenting the following:
 #
@@ -1236,14 +1586,19 @@
 
 # Cluster node timeout is the amount of milliseconds a node must be unreachable
 # for it to be considered in failure state.
 # Most other internal time limits are a multiple of the node timeout.
 #
 # cluster-node-timeout 15000
 
+# The cluster port is the port that the cluster bus will listen for inbound connections on. When set
+# to the default value, 0, it will be bound to the command port + 10000. Setting this value requires
+# you to specify the cluster bus port when executing cluster meet.
+# cluster-port 0
+
 # A replica of a failing master will avoid to start a failover if its data
 # looks too old.
 #
 # There is no simple way for a replica to actually have an exact measure of
 # its "data age", so the following two checks are performed:
 #
 # 1) If there are multiple replicas able to failover, they exchange messages
@@ -1294,93 +1649,154 @@
 # given number of other working replicas for their old master. This number
 # is the "migration barrier". A migration barrier of 1 means that a replica
 # will migrate only if there is at least 1 other working replica for its master
 # and so forth. It usually reflects the number of replicas you want for every
 # master in your cluster.
 #
 # Default is 1 (replicas migrate only if their masters remain with at least
-# one replica). To disable migration just set it to a very large value.
+# one replica). To disable migration just set it to a very large value or
+# set cluster-allow-replica-migration to 'no'.
 # A value of 0 can be set but is useful only for debugging and dangerous
 # in production.
 #
 # cluster-migration-barrier 1
 
+# Turning off this option allows to use less automatic cluster configuration.
+# It both disables migration to orphaned masters and migration from masters
+# that became empty.
+#
+# Default is 'yes' (allow automatic migrations).
+#
+# cluster-allow-replica-migration yes
+
 # By default Redis Cluster nodes stop accepting queries if they detect there
 # is at least a hash slot uncovered (no available node is serving it).
 # This way if the cluster is partially down (for example a range of hash slots
 # are no longer covered) all the cluster becomes, eventually, unavailable.
 # It automatically returns available as soon as all the slots are covered again.
 #
 # However sometimes you want the subset of the cluster which is working,
 # to continue to accept queries for the part of the key space that is still
 # covered. In order to do so, just set the cluster-require-full-coverage
 # option to no.
 #
 cluster-require-full-coverage yes
 
 # This option, when set to yes, prevents replicas from trying to failover its
-# master during master failures. However the master can still perform a
+# master during master failures. However the replica can still perform a
 # manual failover, if forced to do so.
 #
 # This is useful in different scenarios, especially in the case of multiple
 # data center operations, where we want one side to never be promoted if not
 # in the case of a total DC failure.
 #
 # cluster-replica-no-failover no
 
 # This option, when set to yes, allows nodes to serve read traffic while the
-# the cluster is in a down state, as long as it believes it owns the slots.
+# cluster is in a down state, as long as it believes it owns the slots.
 #
 # This is useful for two cases.  The first case is for when an application
 # doesn't require consistency of data during node failures or network partitions.
 # One example of this is a cache, where as long as the node has the data it
 # should be able to serve it.
 #
 # The second use case is for configurations that don't meet the recommended
 # three shards but want to enable cluster mode and scale later. A
 # master outage in a 1 or 2 shard configuration causes a read/write outage to the
 # entire cluster without this option set, with it set there is only a write outage.
 # Without a quorum of masters, slot ownership will not change automatically.
 #
 # cluster-allow-reads-when-down no
 
+# This option, when set to yes, allows nodes to serve pubsub shard traffic while
+# the cluster is in a down state, as long as it believes it owns the slots.
+#
+# This is useful if the application would like to use the pubsub feature even when
+# the cluster global stable state is not OK. If the application wants to make sure only
+# one shard is serving a given channel, this feature should be kept as yes.
+#
+# cluster-allow-pubsubshard-when-down yes
+
+# Cluster link send buffer limit is the limit on the memory usage of an individual
+# cluster bus link's send buffer in bytes. Cluster links would be freed if they exceed
+# this limit. This is to primarily prevent send buffers from growing unbounded on links
+# toward slow peers (E.g. PubSub messages being piled up).
+# This limit is disabled by default. Enable this limit when 'mem_cluster_links' INFO field
+# and/or 'send-buffer-allocated' entries in the 'CLUSTER LINKS` command output continuously increase.
+# Minimum limit of 1gb is recommended so that cluster link buffer can fit in at least a single
+# PubSub message by default. (client-query-buffer-limit default value is 1gb)
+#
+# cluster-link-sendbuf-limit 0
+
+# Clusters can configure their announced hostname using this config. This is a common use case for
+# applications that need to use TLS Server Name Indication (SNI) or dealing with DNS based
+# routing. By default this value is only shown as additional metadata in the CLUSTER SLOTS
+# command, but can be changed using 'cluster-preferred-endpoint-type' config. This value is
+# communicated along the clusterbus to all nodes, setting it to an empty string will remove
+# the hostname and also propagate the removal.
+#
+# cluster-announce-hostname ""
+
+# Clusters can advertise how clients should connect to them using either their IP address,
+# a user defined hostname, or by declaring they have no endpoint. Which endpoint is
+# shown as the preferred endpoint is set by using the cluster-preferred-endpoint-type
+# config with values 'ip', 'hostname', or 'unknown-endpoint'. This value controls how
+# the endpoint returned for MOVED/ASKING requests as well as the first field of CLUSTER SLOTS.
+# If the preferred endpoint type is set to hostname, but no announced hostname is set, a '?'
+# will be returned instead.
+#
+# When a cluster advertises itself as having an unknown endpoint, it's indicating that
+# the server doesn't know how clients can reach the cluster. This can happen in certain
+# networking situations where there are multiple possible routes to the node, and the
+# server doesn't know which one the client took. In this case, the server is expecting
+# the client to reach out on the same endpoint it used for making the last request, but use
+# the port provided in the response.
+#
+# cluster-preferred-endpoint-type ip
+
 # In order to setup your cluster make sure to read the documentation
-# available at http://redis.io web site.
+# available at https://redis.io web site.
 
 ########################## CLUSTER DOCKER/NAT support  ########################
 
 # In certain deployments, Redis Cluster nodes address discovery fails, because
 # addresses are NAT-ted or because ports are forwarded (the typical case is
 # Docker and other containers).
 #
 # In order to make Redis Cluster working in such environments, a static
 # configuration where each node knows its public address is needed. The
-# following two options are used for this scope, and are:
+# following four options are used for this scope, and are:
 #
 # * cluster-announce-ip
 # * cluster-announce-port
+# * cluster-announce-tls-port
 # * cluster-announce-bus-port
 #
-# Each instructs the node about its address, client port, and cluster message
-# bus port. The information is then published in the header of the bus packets
-# so that other nodes will be able to correctly map the address of the node
-# publishing the information.
+# Each instructs the node about its address, client ports (for connections
+# without and with TLS) and cluster message bus port. The information is then
+# published in the header of the bus packets so that other nodes will be able to
+# correctly map the address of the node publishing the information.
+#
+# If cluster-tls is set to yes and cluster-announce-tls-port is omitted or set
+# to zero, then cluster-announce-port refers to the TLS port. Note also that
+# cluster-announce-tls-port has no effect if cluster-tls is set to no.
 #
 # If the above options are not used, the normal Redis Cluster auto-detection
 # will be used instead.
 #
 # Note that when remapped, the bus port may not be at the fixed offset of
 # clients port + 10000, so you can specify any port and bus-port depending
 # on how they get remapped. If the bus-port is not set, a fixed offset of
 # 10000 will be used as usual.
 #
 # Example:
 #
 # cluster-announce-ip 10.1.1.5
-# cluster-announce-port 6379
+# cluster-announce-tls-port 6379
+# cluster-announce-port 0
 # cluster-announce-bus-port 6380
 
 ################################## SLOW LOG ###################################
 
 # The Redis Slow Log is a system to log queries that exceeded a specified
 # execution time. The execution time does not include the I/O operations
 # like talking with the client, sending the reply and so forth,
@@ -1420,18 +1836,32 @@
 # By default latency monitoring is disabled since it is mostly not needed
 # if you don't have latency issues, and collecting data has a performance
 # impact, that while very small, can be measured under big load. Latency
 # monitoring can easily be enabled at runtime using the command
 # "CONFIG SET latency-monitor-threshold <milliseconds>" if needed.
 latency-monitor-threshold 0
 
+################################ LATENCY TRACKING ##############################
+
+# The Redis extended latency monitoring tracks the per command latencies and enables
+# exporting the percentile distribution via the INFO latencystats command,
+# and cumulative latency distributions (histograms) via the LATENCY command.
+#
+# By default, the extended latency monitoring is enabled since the overhead
+# of keeping track of the command latency is very small.
+# latency-tracking yes
+
+# By default the exported latency percentiles via the INFO latencystats command
+# are the p50, p99, and p999.
+# latency-tracking-info-percentiles 50 99 99.9
+
 ############################# EVENT NOTIFICATION ##############################
 
 # Redis can notify Pub/Sub clients about events happening in the key space.
-# This feature is documented at http://redis.io/topics/notifications
+# This feature is documented at https://redis.io/topics/notifications
 #
 # For instance if keyspace events notification is enabled, and a client
 # performs a DEL operation on key "foo" stored in the Database 0, two
 # messages will be published via Pub/Sub:
 #
 # PUBLISH __keyspace@0__:foo del
 # PUBLISH __keyevent@0__:del foo
@@ -1445,17 +1875,19 @@
 #  $     String commands
 #  l     List commands
 #  s     Set commands
 #  h     Hash commands
 #  z     Sorted set commands
 #  x     Expired events (events generated every time a key expires)
 #  e     Evicted events (events generated when a key is evicted for maxmemory)
+#  n     New key events (Note: not included in the 'A' class)
 #  t     Stream commands
+#  d     Module key type events
 #  m     Key-miss events (Note: It is not included in the 'A' class)
-#  A     Alias for g$lshzxet, so that the "AKE" string means all the events
+#  A     Alias for g$lshzxetd, so that the "AKE" string means all the events
 #        (Except key-miss events which are excluded from 'A' due to their
 #         unique nature).
 #
 #  The "notify-keyspace-events" takes as argument a string that is composed
 #  of zero or multiple characters. The empty string means that notifications
 #  are disabled.
 #
@@ -1470,94 +1902,36 @@
 #  notify-keyspace-events Ex
 #
 #  By default all notifications are disabled because most users don't need
 #  this feature and the feature has some overhead. Note that if you don't
 #  specify at least one of K or E, no events will be delivered.
 notify-keyspace-events ""
 
-############################### GOPHER SERVER #################################
-
-# Redis contains an implementation of the Gopher protocol, as specified in
-# the RFC 1436 (https://www.ietf.org/rfc/rfc1436.txt).
-#
-# The Gopher protocol was very popular in the late '90s. It is an alternative
-# to the web, and the implementation both server and client side is so simple
-# that the Redis server has just 100 lines of code in order to implement this
-# support.
-#
-# What do you do with Gopher nowadays? Well Gopher never *really* died, and
-# lately there is a movement in order for the Gopher more hierarchical content
-# composed of just plain text documents to be resurrected. Some want a simpler
-# internet, others believe that the mainstream internet became too much
-# controlled, and it's cool to create an alternative space for people that
-# want a bit of fresh air.
-#
-# Anyway for the 10nth birthday of the Redis, we gave it the Gopher protocol
-# as a gift.
-#
-# --- HOW IT WORKS? ---
-#
-# The Redis Gopher support uses the inline protocol of Redis, and specifically
-# two kind of inline requests that were anyway illegal: an empty request
-# or any request that starts with "/" (there are no Redis commands starting
-# with such a slash). Normal RESP2/RESP3 requests are completely out of the
-# path of the Gopher protocol implementation and are served as usual as well.
-#
-# If you open a connection to Redis when Gopher is enabled and send it
-# a string like "/foo", if there is a key named "/foo" it is served via the
-# Gopher protocol.
-#
-# In order to create a real Gopher "hole" (the name of a Gopher site in Gopher
-# talking), you likely need a script like the following:
-#
-#   https://github.com/antirez/gopher2redis
-#
-# --- SECURITY WARNING ---
-#
-# If you plan to put Redis on the internet in a publicly accessible address
-# to server Gopher pages MAKE SURE TO SET A PASSWORD to the instance.
-# Once a password is set:
-#
-#   1. The Gopher server (when enabled, not by default) will still serve
-#      content via Gopher.
-#   2. However other commands cannot be called before the client will
-#      authenticate.
-#
-# So use the 'requirepass' option to protect your instance.
-#
-# Note that Gopher is not currently supported when 'io-threads-do-reads'
-# is enabled.
-#
-# To enable Gopher support, uncomment the following line and set the option
-# from no (the default) to yes.
-#
-# gopher-enabled no
-
 ############################### ADVANCED CONFIG ###############################
 
 # Hashes are encoded using a memory efficient data structure when they have a
 # small number of entries, and the biggest entry does not exceed a given
 # threshold. These thresholds can be configured using the following directives.
-hash-max-ziplist-entries 512
-hash-max-ziplist-value 64
+hash-max-listpack-entries 512
+hash-max-listpack-value 64
 
 # Lists are also encoded in a special way to save a lot of space.
 # The number of entries allowed per internal list node can be specified
 # as a fixed maximum size or a maximum number of elements.
 # For a fixed maximum size, use -5 through -1, meaning:
 # -5: max size: 64 Kb  <-- not recommended for normal workloads
 # -4: max size: 32 Kb  <-- not recommended
 # -3: max size: 16 Kb  <-- probably not recommended
 # -2: max size: 8 Kb   <-- good
 # -1: max size: 4 Kb   <-- good
 # Positive numbers mean store up to _exactly_ that number of elements
 # per list node.
 # The highest performing option is usually -2 (8 Kb size) or -1 (4 Kb size),
 # but if your use case is unique, adjust the settings as necessary.
-list-max-ziplist-size -2
+list-max-listpack-size -2
 
 # Lists may also be compressed.
 # Compress depth is the number of quicklist ziplist nodes from *each* side of
 # the list to *exclude* from compression.  The head and tail of the list
 # are always uncompressed for fast push/pop operations.  Settings are:
 # 0: disable all list compression
 # 1: depth 1 means "don't start compressing until after 1 node into the list,
@@ -1577,16 +1951,16 @@
 # The following configuration setting sets the limit in the size of the
 # set in order to use this special memory saving encoding.
 set-max-intset-entries 512
 
 # Similarly to hashes and lists, sorted sets are also specially encoded in
 # order to save a lot of space. This encoding is only used when the length and
 # elements of a sorted set are below the following limits:
-zset-max-ziplist-entries 128
-zset-max-ziplist-value 64
+zset-max-listpack-entries 128
+zset-max-listpack-value 64
 
 # HyperLogLog sparse representation bytes limit. The limit includes the
 # 16 bytes header. When an HyperLogLog using the sparse representation crosses
 # this limit, it is converted into the dense representation.
 #
 # A value greater than 16000 is totally useless, since at that point the
 # dense representation is more memory efficient.
@@ -1600,15 +1974,15 @@
 
 # Streams macro node max size / items. The stream data structure is a radix
 # tree of big nodes that encode multiple items inside. Using this configuration
 # it is possible to configure how big a single node can be in bytes, and the
 # maximum number of items it may contain before switching to a new node when
 # appending new stream entries. If any of the following settings are set to
 # zero, the limit is ignored, so for instance it is possible to set just a
-# max entires limit by setting max-bytes to 0 and max-entries to the desired
+# max entries limit by setting max-bytes to 0 and max-entries to the desired
 # value.
 stream-node-max-bytes 4096
 stream-node-max-entries 100
 
 # Active rehashing uses 1 millisecond every 100 milliseconds of CPU time in
 # order to help rehashing the main Redis hash table (the one mapping top-level
 # keys to values). The hash table implementation Redis uses (see dict.c)
@@ -1633,15 +2007,15 @@
 # that are not reading data from the server fast enough for some reason (a
 # common reason is that a Pub/Sub client can't consume messages as fast as the
 # publisher can produce them).
 #
 # The limit can be set differently for the three different classes of clients:
 #
 # normal -> normal clients including MONITOR clients
-# replica  -> replica clients
+# replica -> replica clients
 # pubsub -> clients subscribed to at least one pubsub channel or pattern
 #
 # The syntax of every client-output-buffer-limit directive is the following:
 #
 # client-output-buffer-limit <class> <hard limit> <soft limit> <soft seconds>
 #
 # A client is immediately disconnected once the hard limit is reached, or if
@@ -1657,27 +2031,53 @@
 # without asking (in a push way), but just after a request, so only
 # asynchronous clients may create a scenario where data is requested faster
 # than it can read.
 #
 # Instead there is a default limit for pubsub and replica clients, since
 # subscribers and replicas receive data in a push fashion.
 #
+# Note that it doesn't make sense to set the replica clients output buffer
+# limit lower than the repl-backlog-size config (partial sync will succeed
+# and then replica will get disconnected).
+# Such a configuration is ignored (the size of repl-backlog-size will be used).
+# This doesn't have memory consumption implications since the replica client
+# will share the backlog buffers memory.
+#
 # Both the hard or the soft limit can be disabled by setting them to zero.
 client-output-buffer-limit normal 0 0 0
 client-output-buffer-limit replica 256mb 64mb 60
 client-output-buffer-limit pubsub 32mb 8mb 60
 
 # Client query buffers accumulate new commands. They are limited to a fixed
 # amount by default in order to avoid that a protocol desynchronization (for
 # instance due to a bug in the client) will lead to unbound memory usage in
 # the query buffer. However you can configure it here if you have very special
 # needs, such us huge multi/exec requests or alike.
 #
 # client-query-buffer-limit 1gb
 
+# In some scenarios client connections can hog up memory leading to OOM
+# errors or data eviction. To avoid this we can cap the accumulated memory
+# used by all client connections (all pubsub and normal clients). Once we
+# reach that limit connections will be dropped by the server freeing up
+# memory. The server will attempt to drop the connections using the most
+# memory first. We call this mechanism "client eviction".
+#
+# Client eviction is configured using the maxmemory-clients setting as follows:
+# 0 - client eviction is disabled (default)
+#
+# A memory value can be used for the client eviction threshold,
+# for example:
+# maxmemory-clients 1g
+#
+# A percentage value (between 1% and 100%) means the client eviction threshold
+# is based on a percentage of the maxmemory setting. For example to set client
+# eviction at 5% of maxmemory:
+# maxmemory-clients 5%
+
 # In the Redis protocol, bulk requests, that are, elements representing single
 # strings, are normally limited to 512 mb. However you can change this limit
 # here, but must be 1mb or greater
 #
 # proto-max-bulk-len 512mb
 
 # Redis calls an internal function to perform many background tasks, like
@@ -1710,21 +2110,21 @@
 # as a baseline, but multiples of the configured HZ value will be actually
 # used as needed once more clients are connected. In this way an idle
 # instance will use very little CPU time while a busy instance will be
 # more responsive.
 dynamic-hz yes
 
 # When a child rewrites the AOF file, if the following option is enabled
-# the file will be fsync-ed every 32 MB of data generated. This is useful
+# the file will be fsync-ed every 4 MB of data generated. This is useful
 # in order to commit the file to the disk more incrementally and avoid
 # big latency spikes.
 aof-rewrite-incremental-fsync yes
 
 # When redis saves RDB file, if the following option is enabled
-# the file will be fsync-ed every 32 MB of data generated. This is useful
+# the file will be fsync-ed every 4 MB of data generated. This is useful
 # in order to commit the file to the disk more incrementally and avoid
 # big latency spikes.
 rdb-save-incremental-fsync yes
 
 # Redis LFU eviction (see maxmemory setting) can be tuned. However it is a good
 # idea to start with the default settings and only change them after investigating
 # how to improve the performances and how the keys LFU change over time, which
@@ -1813,15 +2213,15 @@
 # 3. Once you experience fragmentation, you can enable this feature when
 #    needed with the command "CONFIG SET activedefrag yes".
 #
 # The configuration parameters are able to fine tune the behavior of the
 # defragmentation process. If you are not sure about what they mean it is
 # a good idea to leave the defaults untouched.
 
-# Enabled active defragmentation
+# Active defragmentation is disabled by default
 # activedefrag no
 
 # Minimum amount of fragmentation waste to start active defrag
 # active-defrag-ignore-bytes 100mb
 
 # Minimum percentage of fragmentation to start active defrag
 # active-defrag-threshold-lower 10
```

### Comparing `smartsim-0.4.2/smartsim/_core/control/__init__.py` & `smartsim-0.5.0/smartsim/_core/control/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/control/controller.py` & `smartsim-0.5.0/smartsim/_core/control/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,56 +20,66 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
 import os.path as osp
 import pickle
 import signal
 import threading
 import time
+import typing as t
 
 from smartredis import Client
-from smartredis.error import RedisConnectionError, RedisReplyError
 
+from ..._core.launcher.step import Step
 from ..._core.utils.redis import db_is_active, set_ml_model, set_script
 from ...database import Orchestrator
-from ...entity import DBModel, DBNode, DBObject, DBScript, EntityList, SmartSimEntity
+from ...entity import DBNode, EntityList, SmartSimEntity, Model, Ensemble
 from ...error import LauncherError, SmartSimError, SSInternalError, SSUnsupportedError
 from ...log import get_logger
 from ...status import STATUS_RUNNING, TERMINAL_STATUSES
 from ..config import CONFIG
-from ..launcher import *
+from ..launcher import SlurmLauncher, PBSLauncher, LocalLauncher, CobaltLauncher, LSFLauncher
+from ..launcher.launcher import Launcher
 from ..utils import check_cluster_status, create_cluster
 from .jobmanager import JobManager
+from .manifest import Manifest
+from .job import Job
+from ...settings.base import BatchSettings
+
 
 logger = get_logger(__name__)
 
 # job manager lock
 JM_LOCK = threading.RLock()
 
 
 class Controller:
     """The controller module provides an interface between the
     smartsim entities created in the experiment and the
     underlying workload manager or run framework.
     """
 
-    def __init__(self, launcher="local"):
+    def __init__(self, launcher: str = "local") -> None:
         """Initialize a Controller
 
         :param launcher: the type of launcher being used
         :type launcher: str
         """
         self._jobs = JobManager(JM_LOCK)
         self.init_launcher(launcher)
 
-    def start(self, manifest, block=True, kill_on_interrupt=True):
+    def start(
+        self, manifest: Manifest, block: bool = True, kill_on_interrupt: bool = True
+    ) -> None:
         """Start the passed SmartSim entities
 
         This function should not be called directly, but rather
         through the experiment interface.
 
         The controller will start the job-manager thread upon
         execution of all jobs.
@@ -86,24 +96,26 @@
         # block until all non-database jobs are complete
         if block:
             # poll handles its own keyboard interrupt as
             # it may be called seperately
             self.poll(5, True, kill_on_interrupt=kill_on_interrupt)
 
     @property
-    def orchestrator_active(self):
+    def orchestrator_active(self) -> bool:
         JM_LOCK.acquire()
         try:
             if len(self._jobs.db_jobs) > 0:
                 return True
             return False
         finally:
             JM_LOCK.release()
 
-    def poll(self, interval, verbose, kill_on_interrupt=True):
+    def poll(
+        self, interval: int, verbose: bool, kill_on_interrupt: bool = True
+    ) -> None:
         """Poll running jobs and receive logging output of job status
 
         :param interval: number of seconds to wait before polling again
         :type interval: int
         :param verbose: set verbosity
         :type verbose: bool
         :param kill_on_interrupt: flag for killing jobs when SIGINT is received
@@ -120,15 +132,15 @@
                 JM_LOCK.acquire()
                 try:
                     for job in to_monitor.values():
                         logger.info(job)
                 finally:
                     JM_LOCK.release()
 
-    def finished(self, entity):
+    def finished(self, entity: t.Union[SmartSimEntity, EntityList]) -> bool:
         """Return a boolean indicating wether a job has finished or not
 
         :param entity: object launched by SmartSim.
         :type entity: Entity | EntityList
         :returns: bool
         :raises ValueError: if entity has not been launched yet
         """
@@ -145,22 +157,22 @@
 
             return self._jobs.is_finished(entity)
         except KeyError:
             raise ValueError(
                 f"Entity {entity.name} has not been launched in this experiment"
             ) from None
 
-    def stop_entity(self, entity):
+    def stop_entity(self, entity: t.Union[SmartSimEntity, EntityList]) -> None:
         """Stop an instance of an entity
 
         This function will also update the status of the job in
         the jobmanager so that the job appears as "cancelled".
 
         :param entity: entity to be stopped
-        :type entity: SmartSimEntity
+        :type entity: Entity | EntityList
         """
         JM_LOCK.acquire()
         try:
             job = self._jobs[entity.name]
             if job.status not in TERMINAL_STATUSES:
                 logger.info(
                     " ".join(
@@ -176,53 +188,53 @@
                     error=status.error,
                     output=status.output,
                 )
                 self._jobs.move_to_completed(job)
         finally:
             JM_LOCK.release()
 
-    def stop_entity_list(self, entity_list):
+    def stop_entity_list(self, entity_list: EntityList) -> None:
         """Stop an instance of an entity list
 
         :param entity_list: entity list to be stopped
         :type entity_list: EntityList
         """
         if entity_list.batch:
             self.stop_entity(entity_list)
         else:
             for entity in entity_list.entities:
                 self.stop_entity(entity)
 
-    def get_jobs(self):
+    def get_jobs(self) -> t.Dict[str, Job]:
         """Return a dictionary of completed job data
 
         :returns: dict[str, Job]
         """
         JM_LOCK.acquire()
         try:
             return self._jobs.completed
         finally:
             JM_LOCK.release()
 
-    def get_entity_status(self, entity):
+    def get_entity_status(self, entity: t.Union[SmartSimEntity, EntityList]) -> str:
         """Get the status of an entity
 
         :param entity: entity to get status of
-        :type entity: SmartSimEntity
-        :raises TypeError: if not SmartSimEntity
+        :type entity: SmartSimEntity | EntityList
+        :raises TypeError: if not SmartSimEntity | EntityList
         :return: status of entity
         :rtype: str
         """
         if not isinstance(entity, (SmartSimEntity, EntityList)):
             raise TypeError(
                 f"Argument must be of type SmartSimEntity or EntityList, not {type(entity)}"
             )
         return self._jobs.get_status(entity)
 
-    def get_entity_list_status(self, entity_list):
+    def get_entity_list_status(self, entity_list: EntityList) -> t.List[str]:
         """Get the statuses of an entity list
 
         :param entity_list: entity list containing entities to
                             get statuses of
         :type entity_list: EntityList
         :raises TypeError: if not EntityList
         :return: list of str statuses
@@ -233,26 +245,26 @@
         if entity_list.batch:
             return [self.get_entity_status(entity_list)]
         statuses = []
         for entity in entity_list.entities:
             statuses.append(self.get_entity_status(entity))
         return statuses
 
-    def init_launcher(self, launcher):
+    def init_launcher(self, launcher: str) -> None:
         """Initialize the controller with a specific type of launcher.
         SmartSim currently supports slurm, pbs(pro), cobalt, lsf,
         and local launching
 
         :param launcher: which launcher to initialize
         :type launcher: str
         :raises SSUnsupportedError: if a string is passed that is not
                                     a supported launcher
         :raises TypeError: if no launcher argument is provided.
         """
-        launcher_map = {
+        launcher_map: t.Dict[str, t.Type[Launcher]] = {
             "slurm": SlurmLauncher,
             "pbs": PBSLauncher,
             "cobalt": CobaltLauncher,
             "lsf": LSFLauncher,
             "local": LocalLauncher,
         }
 
@@ -263,15 +275,15 @@
                 self._launcher = launcher_map[launcher]()
                 self._jobs.set_launcher(self._launcher)
             else:
                 raise SSUnsupportedError("Launcher type not supported: " + launcher)
         else:
             raise TypeError("Must provide a 'launcher' argument")
 
-    def _launch(self, manifest):
+    def _launch(self, manifest: Manifest) -> None:
         """Main launching function of the controller
 
         Orchestrators are always launched first so that the
         address of the database can be given to following entities
 
         :param manifest: Manifest of deployables to launch
         :type manifest: Manifest
@@ -290,15 +302,15 @@
                 raise SmartSimError(msg)
             self._launch_orchestrator(orchestrator)
 
         if self.orchestrator_active:
             self._set_dbobjects(manifest)
 
         # create all steps prior to launch
-        steps = []
+        steps: t.List[t.Tuple[Step, t.Union[SmartSimEntity, EntityList]]] = []
         all_entity_lists = manifest.ensembles
         for elist in all_entity_lists:
             if elist.batch:
                 batch_step = self._create_batch_job_step(elist)
                 steps.append((batch_step, elist))
             else:
                 # if ensemble is to be run as separate job steps, aka not in a batch
@@ -319,15 +331,15 @@
                 job_step = self._create_job_step(model)
                 steps.append((job_step, model))
 
         # launch steps
         for step, entity in steps:
             self._launch_step(step, entity)
 
-    def _launch_orchestrator(self, orchestrator):
+    def _launch_orchestrator(self, orchestrator: Orchestrator) -> None:
         """Launch an Orchestrator instance
 
         This function will launch the Orchestrator instance and
         if on WLM, find the nodes where it was launched and
         set them in the JobManager
 
         :param orchestrator: orchestrator to launch
@@ -338,15 +350,15 @@
         # if the orchestrator was launched as a batch workload
         if orchestrator.batch:
             orc_batch_step = self._create_batch_job_step(orchestrator)
             self._launch_step(orc_batch_step, orchestrator)
 
         # if orchestrator was run on existing allocation, locally, or in allocation
         else:
-            db_steps = [(self._create_job_step(db), db) for db in orchestrator]
+            db_steps = [(self._create_job_step(db), db) for db in orchestrator.dbnodes]
             for db_step in db_steps:
                 self._launch_step(*db_step)
 
         # wait for orchestrator to spin up
         self._orchestrator_launch_wait(orchestrator)
 
         # set the jobs in the job manager to provide SSDB variable to entities
@@ -374,15 +386,15 @@
                         time.sleep(5)
                     else:
                         # surface SSInternalError as we have no way to recover
                         raise
         self._save_orchestrator(orchestrator)
         logger.debug(f"Orchestrator launched on nodes: {orchestrator.hosts}")
 
-    def _launch_step(self, job_step, entity):
+    def _launch_step(self, job_step: Step, entity: t.Union[SmartSimEntity, EntityList]) -> None:
         """Use the launcher to launch a job stop
 
         :param job_step: a job step instance
         :type job_step: Step
         :param entity: entity instance
         :type entity: SmartSimEntity
         :raises SmartSimError: if launch fails
@@ -404,56 +416,57 @@
         if self._jobs.query_restart(entity.name):
             logger.debug(f"Restarting {entity.name}")
             self._jobs.restart_job(job_step.name, job_id, entity.name, is_task)
         else:
             logger.debug(f"Launching {entity.name}")
             self._jobs.add_job(job_step.name, job_id, entity, is_task)
 
-    def _create_batch_job_step(self, entity_list):
+    def _create_batch_job_step(self, entity_list: t.Union[Orchestrator, Ensemble, _AnonymousBatchJob]) -> Step:
         """Use launcher to create batch job step
 
         :param entity_list: EntityList to launch as batch
         :type entity_list: EntityList
         :return: job step instance
         :rtype: Step
         """
+        if not entity_list.batch_settings:
+            raise ValueError("EntityList must have batch settings to be launched as batch")
+
         batch_step = self._launcher.create_step(
             entity_list.name, entity_list.path, entity_list.batch_settings
         )
         for entity in entity_list.entities:
             # tells step creation not to look for an allocation
             entity.run_settings.in_batch = True
             step = self._create_job_step(entity)
             batch_step.add_to_batch(step)
         return batch_step
 
-    def _create_job_step(self, entity):
+    def _create_job_step(self, entity: SmartSimEntity) -> Step:
         """Create job steps for all entities with the launcher
 
-        :param entities: list of all entities to create steps for
-        :type entities: list of SmartSimEntities
-        :return: list of tuples of (launcher_step, entity)
-        :rtype: list of tuples
+        :param entity: an entity to create a step for
+        :type entity: SmartSimEntity
+        :return: the job step
+        :rtype: Step
         """
         # get SSDB, SSIN, SSOUT and add to entity run settings
-        if not isinstance(entity, DBNode):
+        if isinstance(entity, Model):
             self._prep_entity_client_env(entity)
 
         step = self._launcher.create_step(entity.name, entity.path, entity.run_settings)
         return step
 
-    def _prep_entity_client_env(self, entity):
+    def _prep_entity_client_env(self, entity: Model) -> None:
         """Retrieve all connections registered to this entity
 
         :param entity: The entity to retrieve connections from
-        :type entity:  SmartSimEntity
-        :returns: Dictionary whose keys are environment variables to be set
-        :rtype: dict
+        :type entity:  Model
         """
-        client_env = {}
+        client_env: t.Dict[str, t.Union[str, int, float, bool]] = {}
         addresses = self._jobs.get_db_host_addresses()
         if addresses:
             if len(addresses) <= 128:
                 client_env["SSDB"] = ",".join(addresses)
             else:
                 # Cap max length of SSDB
                 client_env["SSDB"] = ",".join(addresses[:128])
@@ -461,32 +474,33 @@
                 client_env["SSKEYIN"] = ",".join(
                     [in_entity.name for in_entity in entity.incoming_entities]
                 )
             if entity.query_key_prefixing():
                 client_env["SSKEYOUT"] = entity.name
 
         # Set address to local if it's a colocated model
-        if hasattr(entity, "colocated") and entity.colocated:
-            port = entity.run_settings.colocated_db_settings.get("port", None)
-            socket = entity.run_settings.colocated_db_settings.get("unix_socket", None)
-            if socket and port:
-                raise SSInternalError(
-                    "Co-located was configured for both TCP/IP and UDS"
-                )
-            if port:
-                client_env["SSDB"] = f"127.0.0.1:{str(port)}"
-            elif socket:
-                client_env["SSDB"] = f"unix://{socket}"
-            else:
-                raise SSInternalError(
-                    "Colocated database was not configured for either TCP or UDS"
-                )
+        if entity.colocated:
+            if colo_cfg := entity.run_settings.colocated_db_settings:
+                port = colo_cfg.get("port", None)
+                socket = colo_cfg.get("unix_socket", None)
+                if socket and port:
+                    raise SSInternalError(
+                        "Co-located was configured for both TCP/IP and UDS"
+                    )
+                if port:
+                    client_env["SSDB"] = f"127.0.0.1:{str(port)}"
+                elif socket:
+                    client_env["SSDB"] = f"unix://{socket}"
+                else:
+                    raise SSInternalError(
+                        "Colocated database was not configured for either TCP or UDS"
+                    )
         entity.run_settings.update_env(client_env)
 
-    def _save_orchestrator(self, orchestrator):
+    def _save_orchestrator(self, orchestrator: Orchestrator) -> None:
         """Save the orchestrator object via pickle
 
         This function saves the orchestrator information to a pickle
         file that can be imported by subsequent experiments to reconnect
         to the orchestrator.
 
         :param orchestrator: Orchestrator configuration to be saved
@@ -499,15 +513,15 @@
         steps = []
         for db_job in db_jobs.values():
             steps.append(self._launcher.step_mapping[db_job.name])
         orc_data["steps"] = steps
         with open(dat_file, "wb") as pickle_file:
             pickle.dump(orc_data, pickle_file)
 
-    def _orchestrator_launch_wait(self, orchestrator):
+    def _orchestrator_launch_wait(self, orchestrator: Orchestrator) -> None:
         """Wait for the orchestrator instances to run
 
         In the case where the orchestrator is launched as a batch
         through a WLM, we wait for the orchestrator to exit the
         queue before proceeding so new launched entities can
         be launched with SSDB address
 
@@ -538,25 +552,24 @@
                     self.stop_entity_list(orchestrator)
                     msg = "Orchestrator failed during startup"
                     msg += f" See {orchestrator.path} for details"
                     raise SmartSimError(msg)
                 else:
                     logger.debug("Waiting for orchestrator instances to spin up...")
             except KeyboardInterrupt:
-
                 logger.info("Orchestrator launch cancelled - requesting to stop")
                 self.stop_entity_list(orchestrator)
 
                 # re-raise keyboard interrupt so the job manager will display
                 # any running and un-killed jobs as this method is only called
                 # during launch and we handle all keyboard interrupts during
                 # launch explicitly
                 raise
 
-    def reload_saved_db(self, checkpoint_file):
+    def reload_saved_db(self, checkpoint_file: str) -> Orchestrator:
         JM_LOCK.acquire()
         try:
             if self.orchestrator_active:
                 raise SmartSimError("Orchestrator exists and is active")
 
             if not osp.exists(checkpoint_file):
                 raise FileNotFoundError(
@@ -605,22 +618,22 @@
             if not self._jobs.actively_monitoring:
                 self._jobs.start()
 
             return orc
         finally:
             JM_LOCK.release()
 
-    def _set_dbobjects(self, manifest):
+    def _set_dbobjects(self, manifest: Manifest) -> None:
         if not manifest.has_db_objects:
             return
 
         db_addresses = self._jobs.get_db_host_addresses()
 
         hosts = list(set([address.split(":")[0] for address in db_addresses]))
-        ports = list(set([address.split(":")[-1] for address in db_addresses]))
+        ports = list(set([int(address.split(":")[-1]) for address in db_addresses]))
 
         if not db_is_active(hosts=hosts, ports=ports, num_shards=len(db_addresses)):
             raise SSInternalError("Cannot set DB Objects, DB is not running")
 
         client = Client(address=db_addresses[0], cluster=len(db_addresses) > 1)
 
         for model in manifest.models:
@@ -631,27 +644,29 @@
                     set_script(db_script, client)
 
         for ensemble in manifest.ensembles:
             for db_model in ensemble._db_models:
                 set_ml_model(db_model, client)
             for db_script in ensemble._db_scripts:
                 set_script(db_script, client)
-            for entity in ensemble:
+            for entity in ensemble.models:
                 if not entity.colocated:
                     # Set models which could belong only
                     # to the entities and not to the ensemble
                     # but avoid duplicates
                     for db_model in entity._db_models:
                         if db_model not in ensemble._db_models:
                             set_ml_model(db_model, client)
                     for db_script in entity._db_scripts:
                         if db_script not in ensemble._db_scripts:
                             set_script(db_script, client)
 
 
 class _AnonymousBatchJob(EntityList):
-    def __init__(self, name, path, batch_settings, **kwargs):
+    def __init__(
+        self, name: str, path: str, batch_settings: BatchSettings, **kwargs: t.Any
+    ) -> None:
         super().__init__(name, path)
         self.batch_settings = batch_settings
 
-    def _initialize_entities(self, **kwargs):
+    def _initialize_entities(self, **kwargs: t.Any) -> None:
         ...
```

### Comparing `smartsim-0.4.2/smartsim/_core/control/job.py` & `smartsim-0.5.0/smartsim/_core/control/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,99 +21,118 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
+import typing as t
 
+from ...entity import SmartSimEntity, EntityList
 from ...status import STATUS_NEW
 
 
 class Job:
     """Keep track of various information for the controller.
     In doing so, continuously add various fields of information
     that is queryable by the user through interface methods in
     the controller class.
     """
 
-    def __init__(self, job_name, job_id, entity, launcher, is_task):
+    def __init__(
+        self,
+        job_name: str,
+        job_id: t.Optional[str],
+        entity: t.Union[SmartSimEntity, EntityList],
+        launcher: str,
+        is_task: bool,
+    ) -> None:
         """Initialize a Job.
 
         :param job_name: Name of the job step
         :type job_name: str
         :param job_id: The id associated with the job
         :type job_id: str
-        :param entity: The SmartSim entity associated with the job
-        :type entity: SmartSimEntity
+        :param entity: The SmartSim entity(list) associated with the job
+        :type entity: SmartSimEntity | EntityList
         :param launcher: Launcher job was started with
         :type launcher: str
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
         :type is_task: bool
         """
         self.name = job_name
         self.jid = job_id
         self.entity = entity
         self.status = STATUS_NEW
-        self.raw_status = None  # status before smartsim status mapping is applied
-        self.returncode = None
-        self.output = None  # only populated if it's system related (e.g. a command failed immediately)
-        self.error = None  # same as output
-        self.hosts = []  # currently only used for DB jobs
+        self.raw_status: t.Optional[str] = None  # status before smartsim status mapping is applied
+        self.returncode: t.Optional[int] = None
+        self.output: t.Optional[str] = None  # only populated if it's system related (e.g. a command failed immediately)
+        self.error: t.Optional[str] = None  # same as output
+        self.hosts: t.List[str] = []  # currently only used for DB jobs
         self.launched_with = launcher
         self.is_task = is_task
         self.start_time = time.time()
         self.history = History()
 
     @property
-    def ename(self):
+    def ename(self) -> str:
         """Return the name of the entity this job was created from"""
         return self.entity.name
 
-    def set_status(self, new_status, raw_status, returncode, error=None, output=None):
+    def set_status(
+        self,
+        new_status: str,
+        raw_status: str,
+        returncode: t.Optional[int],
+        error: t.Optional[str] = None,
+        output: t.Optional[str] = None,
+    ) -> None:
         """Set the status  of a job.
 
         :param new_status: The new status of the job
         :type new_status: str
         :param returncode: The return code for the job
         :type return_code: str
         """
         self.status = new_status
         self.raw_status = raw_status
         self.returncode = returncode
         self.error = error
         self.output = output
 
-    def record_history(self):
+    @property
+    def elapsed(self) -> float:
+        return time.time() - self.start_time
+
+    def record_history(self) -> None:
         """Record the launching history of a job."""
-        job_time = time.time() - self.start_time
-        self.history.record(self.jid, self.status, self.returncode, job_time)
+        self.history.record(self.jid, self.status, self.returncode, self.elapsed)
 
-    def reset(self, new_job_name, new_job_id, is_task):
+    def reset(self, new_job_name: str, new_job_id: t.Optional[str], is_task: bool) -> None:
         """Reset the job in order to be able to restart it.
 
         :param new_job_name: name of the new job step
         :type new_job_name: str
         :param new_job_id: new job id to launch under
-        :type new_job_id: str
+        :type new_job_id: int
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
         :type is_task: bool
         """
         self.name = new_job_name
         self.jid = new_job_id
         self.status = STATUS_NEW
         self.returncode = None
         self.output = None
         self.error = None
         self.hosts = []
         self.is_task = is_task
         self.start_time = time.time()
         self.history.new_run()
 
-    def error_report(self):
+    def error_report(self) -> str:
         """A descriptive error report based on job fields
 
         :return: error report for display in terminal
         :rtype: str
         """
         warning = f"{self.ename} failed. See below for details \n"
         if self.error:
@@ -125,15 +144,15 @@
             warning += f"Output: {self.output} \n"
         warning += f"Job status at failure: {self.status} \n"
         warning += f"Launcher status at failure: {self.raw_status} \n"
         warning += f"Job returncode: {self.returncode} \n"
         warning += f"Error and output file located at: {self.entity.path}"
         return warning
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return user-readable string of the Job
 
         :returns: A user-readable string of the Job
         :rtype: str
         """
         if self.jid:
             job = "{}({}): {}"
@@ -144,29 +163,29 @@
 
 
 class History:
     """History of a job instance. Holds various attributes based
     on the previous launches of a job.
     """
 
-    def __init__(self, runs=0):
+    def __init__(self, runs: int = 0) -> None:
         """Init a history object for a job
 
         :param runs: number of runs so far, defaults to 0
         :type runs: int, optional
         """
         self.runs = runs
-        self.jids = dict()
-        self.statuses = dict()
-        self.returns = dict()
-        self.job_times = dict()
+        self.jids: t.Dict[int, t.Optional[str]] = dict()
+        self.statuses: t.Dict[int, str] = dict()
+        self.returns: t.Dict[int, t.Optional[int]] = dict()
+        self.job_times: t.Dict[int, float] = dict()
 
-    def record(self, job_id, status, returncode, job_time):
+    def record(self, job_id: t.Optional[str], status: str, returncode: t.Optional[int], job_time: float) -> None:
         """record the history of a job"""
         self.jids[self.runs] = job_id
         self.statuses[self.runs] = status
         self.returns[self.runs] = returncode
         self.job_times[self.runs] = job_time
 
-    def new_run(self):
+    def new_run(self) -> None:
         """increment run total"""
         self.runs += 1
```

### Comparing `smartsim-0.4.2/smartsim/_core/control/jobmanager.py` & `smartsim-0.5.0/smartsim/_core/control/jobmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import itertools
 import time
-from threading import Thread
+import typing as t
+from threading import Thread, RLock
+from types import FrameType
 
 from ...database import Orchestrator
-from ...entity import DBNode
+from ...entity import DBNode, SmartSimEntity, EntityList
 from ...error import SmartSimError
 from ...log import get_logger
 from ...status import TERMINAL_STATUSES
 from ..config import CONFIG
-from ..launcher import LocalLauncher
+from ..launcher import LocalLauncher, Launcher
 from ..utils.network import get_ip_from_host
 from .job import Job
 
 logger = get_logger(__name__)
 
 
 class JobManager:
@@ -50,39 +52,39 @@
     to update the statuses of Jobs.
 
     The JobManager and Controller share a single instance of a launcher
     object that allows both the Controller and launcher access to the
     wlm to query information about jobs that the user requests.
     """
 
-    def __init__(self, lock, launcher=None):
+    def __init__(self, lock: RLock, launcher: t.Optional[Launcher] = None) -> None:
         """Initialize a Jobmanager
 
         :param launcher: a Launcher object to manage jobs
         :type: SmartSim.Launcher
         """
         # active jobs
-        self.jobs = {}
-        self.db_jobs = {}
+        self.jobs: t.Dict[str, Job] = {}
+        self.db_jobs: t.Dict[str, Job] = {}
 
         # completed jobs
-        self.completed = {}
+        self.completed: t.Dict[str, Job] = {}
 
         self.actively_monitoring = False  # on/off flag
         self._launcher = launcher  # reference to launcher
         self._lock = lock  # thread lock
 
         self.kill_on_interrupt = True  # flag for killing jobs on SIGINT
 
-    def start(self):
+    def start(self) -> None:
         """Start a thread for the job manager"""
         self.monitor = Thread(name="JobManager", daemon=True, target=self.run)
         self.monitor.start()
 
-    def run(self):
+    def run(self) -> None:
         """Start the JobManager thread to continually check
         the status of all jobs. Whichever launcher is selected
         by the user will be responsible for returning statuses
         that progress the state of the job.
 
         The interval of the checks is controlled by
         smartsim.constats.TM_INTERVAL and should be set to values
@@ -112,15 +114,15 @@
                         self.move_to_completed(job)
 
             # if no more jobs left to actively monitor
             if not self():
                 self.actively_monitoring = False
                 logger.debug("Sleeping, no jobs to monitor")
 
-    def move_to_completed(self, job):
+    def move_to_completed(self, job: Job) -> None:
         """Move job to completed queue so that its no longer
            actively monitored by the job manager
 
         :param job: job instance we are transitioning
         :type job: Job
         """
         self._lock.acquire()
@@ -132,15 +134,15 @@
             if job.ename in self.db_jobs.keys():
                 del self.db_jobs[job.ename]
             elif job.ename in self.jobs.keys():
                 del self.jobs[job.ename]
         finally:
             self._lock.release()
 
-    def __getitem__(self, entity_name):
+    def __getitem__(self, entity_name: str) -> Job:
         """Return the job associated with the name of the entity
         from which it was created.
 
         :param entity_name: The name of the entity of a job
         :type entity_name: str
         :returns: the Job associated with the entity_name
         :rtype: Job
@@ -153,44 +155,44 @@
                 return self.jobs[entity_name]
             if entity_name in self.completed.keys():
                 return self.completed[entity_name]
             raise KeyError
         finally:
             self._lock.release()
 
-    def __call__(self):
+    def __call__(self) -> t.Dict[str, Job]:
         """Returns dictionary all jobs for () operator
 
         :returns: Dictionary of all jobs
         :rtype: dictionary
         """
         all_jobs = {**self.jobs, **self.db_jobs}
         return all_jobs
 
-    def add_job(self, job_name, job_id, entity, is_task=True):
+    def add_job(self, job_name: str, job_id: t.Optional[str], entity: t.Union[SmartSimEntity, EntityList], is_task: bool = True) -> None:
         """Add a job to the job manager which holds specific jobs by type.
 
         :param job_name: name of the job step
         :type job_name: str
         :param job_id: job step id created by launcher
         :type job_id: str
         :param entity: entity that was launched on job step
-        :type entity: SmartSimEntity
+        :type entity: SmartSimEntity | EntityList
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
         :type is_task: bool
         """
         launcher = str(self._launcher)
         # all operations here should be atomic
         job = Job(job_name, job_id, entity, launcher, is_task)
         if isinstance(entity, (DBNode, Orchestrator)):
             self.db_jobs[entity.name] = job
         else:
             self.jobs[entity.name] = job
 
-    def is_finished(self, entity):
+    def is_finished(self, entity: SmartSimEntity) -> bool:
         """Detect if a job has completed
 
         :param entity: entity to check
         :type entity: SmartSimEntity
         :return: True if finished
         :rtype: bool
         """
@@ -200,83 +202,87 @@
             if entity.name in self.completed:
                 if job.status in TERMINAL_STATUSES:
                     return True
             return False
         finally:
             self._lock.release()
 
-    def check_jobs(self):
+    def check_jobs(self) -> None:
         """Update all jobs in jobmanager
 
         Update all jobs returncode, status, error and output
         through one call to the launcher.
 
         """
         self._lock.acquire()
         try:
             jobs = self().values()
-            job_name_map = dict([(job.name, job.ename) for job in jobs])
+            job_name_map = {job.name: job.ename for job in jobs}
 
             # returns (job step name, StepInfo) tuples
-            statuses = self._launcher.get_step_update(job_name_map.keys())
-            for job_name, status in statuses:
-                job = self[job_name_map[job_name]]
-                # uses abstract step interface
-                job.set_status(
-                    status.status,
-                    status.launcher_status,
-                    status.returncode,
-                    error=status.error,
-                    output=status.output,
-                )
+            if self._launcher:
+                step_names = list(job_name_map.keys())
+                statuses = self._launcher.get_step_update(step_names)
+                for job_name, status in statuses:
+                    job = self[job_name_map[job_name]]
+
+                    if status:
+                        # uses abstract step interface
+                        job.set_status(
+                            status.status,
+                            status.launcher_status,
+                            status.returncode,
+                            error=status.error,
+                            output=status.output,
+                        )
         finally:
             self._lock.release()
 
-    def get_status(self, entity):
+    def get_status(self, entity: t.Union[SmartSimEntity, EntityList]) -> str:
         """Return the status of a job.
 
         :param entity: SmartSimEntity or EntityList instance
         :type entity: SmartSimEntity | EntityList
         :returns: tuple of status
         """
         self._lock.acquire()
         try:
             if entity.name in self.completed:
                 return self.completed[entity.name].status
 
-            job = self[entity.name]  # locked
+            job: Job = self[entity.name]  # locked
         except KeyError:
             raise SmartSimError(
                 f"Entity {entity.name} has not been launched in this Experiment"
             ) from None
         finally:
             self._lock.release()
         return job.status
 
-    def set_launcher(self, launcher):
+    def set_launcher(self, launcher: Launcher) -> None:
         """Set the launcher of the job manager to a specific launcher instance
 
         :param launcher: child of Launcher
         :type launcher: Launcher instance
         """
         self._launcher = launcher
 
-    def query_restart(self, entity_name):
+    def query_restart(self, entity_name: str) -> bool:
         """See if the job just started should be restarted or not.
 
         :param entity_name: name of entity to check for a job for
         :type entity_name: str
         :return: if job should be restarted instead of started
         :rtype: bool
         """
         if entity_name in self.completed:
             return True
         return False
 
-    def restart_job(self, job_name, job_id, entity_name, is_task=True):
+    def restart_job(self, job_name: str, job_id: t.Optional[str], entity_name: str, is_task: bool = True) -> None:
         """Function to reset a job to record history and be
         ready to launch again.
 
         :param job_name: new job step name
         :type job_name: str
         :param job_id: new job id
         :type job_id: str
@@ -295,73 +301,76 @@
             if isinstance(job.entity, (DBNode, Orchestrator)):
                 self.db_jobs[entity_name] = job
             else:
                 self.jobs[entity_name] = job
         finally:
             self._lock.release()
 
-    def get_db_host_addresses(self):
+    def get_db_host_addresses(self) -> t.List[str]:
         """Retrieve the list of hosts for the database
 
         :return: list of host ip addresses
         :rtype: list[str]
         """
         addresses = []
         for db_job in self.db_jobs.values():
-            for combine in itertools.product(db_job.hosts, db_job.entity.ports):
-                ip_addr = get_ip_from_host(combine[0])
-                addresses.append(":".join((ip_addr, str(combine[1]))))
+            if isinstance(db_job.entity, (DBNode, Orchestrator)):
+                db_entity = db_job.entity
+
+                for combine in itertools.product(db_job.hosts, db_entity.ports):
+                    ip_addr = get_ip_from_host(combine[0])
+                    addresses.append(":".join((ip_addr, str(combine[1]))))
         return addresses
 
-    def set_db_hosts(self, orchestrator):
+    def set_db_hosts(self, orchestrator: Orchestrator) -> None:
         """Set the DB hosts in db_jobs so future entities can query this
 
         :param orchestrator: orchestrator instance
         :type orchestrator: Orchestrator
         """
         # should only be called during launch in the controller
         self._lock.acquire()
         try:
             if orchestrator.batch:
                 self.db_jobs[orchestrator.name].hosts = orchestrator.hosts
             else:
-                for dbnode in orchestrator:
+                for dbnode in orchestrator.dbnodes:
                     if not dbnode._mpmd:
                         self.db_jobs[dbnode.name].hosts = [dbnode.host]
                     else:
                         self.db_jobs[dbnode.name].hosts = dbnode.hosts
         finally:
             self._lock.release()
 
-    def signal_interrupt(self, sig, frame):
+    def signal_interrupt(self, signo: int, frame: t.Optional[FrameType]) -> None:
         """Custom handler for whenever SIGINT is received"""
         if self.actively_monitoring and len(self) > 0:
             if self.kill_on_interrupt:
                 for _, job in self().items():
-                    if job.status not in TERMINAL_STATUSES:
+                    if job.status not in TERMINAL_STATUSES and self._launcher:
                         self._launcher.stop(job.name)
             else:
                 logger.warning("SmartSim process interrupted before resource cleanup")
                 logger.warning("You may need to manually stop the following:")
 
                 for job_name, job in self().items():
                     if job.is_task:
                         # this will be the process id
                         logger.warning(f"Task {job_name} with id: {job.jid}")
                     else:
                         logger.warning(
                             f"Job {job_name} with {job.launched_with} id: {job.jid}"
                         )
 
-    def _thread_sleep(self):
+    def _thread_sleep(self) -> None:
         """Sleep the job manager for a specific constant
         set for the launcher type.
         """
         local_jm_interval = 2
         if isinstance(self._launcher, (LocalLauncher)):
             time.sleep(local_jm_interval)
         else:
             time.sleep(CONFIG.jm_interval)
 
-    def __len__(self):
+    def __len__(self) -> int:
         # number of active jobs
         return len(self.db_jobs) + len(self.jobs)
```

### Comparing `smartsim-0.4.2/smartsim/_core/control/manifest.py` & `smartsim-0.5.0/smartsim/_core/control/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,133 +20,116 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from ...database import Orchestrator
-from ...entity import EntityList, SmartSimEntity
+from ...entity import EntityList, SmartSimEntity, Model, Ensemble
 from ...error import SmartSimError
 from ..utils.helpers import fmt_dict
 
-# List of types derived from EntityList which require specific behavior
-# A corresponding property needs to exist (like db for Orchestrator),
-# otherwise they will not be accessible
-entity_list_exception_types = [Orchestrator]
-
 
 class Manifest:
     """This class is used to keep track of all deployables generated by an experiment.
     Different types of deployables (i.e. different `SmartSimEntity`-derived objects
     or `EntityList`-derived objects) can be accessed by using the corresponding accessor.
 
     Instances of ``Model``, ``Ensemble`` and ``Orchestrator``
     can all be passed as arguments
     """
 
-    def __init__(self, *args):
+    def __init__(self, *args: SmartSimEntity) -> None:
         self._deployables = list(args)
         self._check_types(self._deployables)
         self._check_names(self._deployables)
         self._check_entity_lists_nonempty()
 
     @property
-    def db(self):
+    def db(self) -> t.Optional[Orchestrator]:
         """Return Orchestrator instances in Manifest
 
         :raises SmartSimError: if user added to databases to manifest
         :return: orchestrator instances
-        :rtype: Orchestrator
+        :rtype: Orchestrator | None
         """
-        _db = None
-        for deployable in self._deployables:
-            if isinstance(deployable, Orchestrator):
-                if _db:
-                    raise SmartSimError(
-                        "User attempted to create more than one Orchestrator"
-                    )
-                _db = deployable
-        return _db
+        dbs = [item for item in self._deployables if isinstance(item, Orchestrator)]
+
+        if len(dbs) > 1:
+            raise SmartSimError("User attempted to create more than one Orchestrator")
+        
+        return dbs[0] if dbs else None
 
     @property
-    def models(self):
+    def models(self) -> t.List[Model]:
         """Return Model instances in Manifest
 
         :return: model instances
         :rtype: List[Model]
         """
-        _models = []
-        for deployable in self._deployables:
-            if isinstance(deployable, SmartSimEntity):
-                _models.append(deployable)
+        _models: t.List[Model] = [item for item in self._deployables if isinstance(item, Model)]
         return _models
 
     @property
-    def ensembles(self):
+    def ensembles(self) -> t.List[Ensemble]:
         """Return Ensemble instances in Manifest
 
         :return: list of ensembles
         :rtype: List[Ensemble]
         """
-        _ensembles = []
-        for deployable in self._deployables:
-            if isinstance(deployable, EntityList):
-                is_exceptional_type = False
-                for exceptional_type in entity_list_exception_types:
-                    if isinstance(deployable, exceptional_type):
-                        is_exceptional_type |= True
-                if not is_exceptional_type:
-                    _ensembles.append(deployable)
-
-        return _ensembles
+        return  [e for e in self._deployables if isinstance(e, Ensemble)]
 
     @property
-    def all_entity_lists(self):
+    def all_entity_lists(self) -> t.List[EntityList]:
         """All entity lists, including ensembles and
         exceptional ones like Orchestrator
 
         :return: list of entity lists
         :rtype: List[EntityList]
         """
-        _all_entity_lists = self.ensembles
+        _all_entity_lists: t.List[EntityList] = []
+        _all_entity_lists.extend(self.ensembles)
+
         db = self.db
         if db is not None:
             _all_entity_lists.append(db)
 
         return _all_entity_lists
 
-    def _check_names(self, deployables):
+    def _check_names(self, deployables: t.List[t.Any]) -> None:
         used = []
         for deployable in deployables:
             name = getattr(deployable, "name", None)
             if not name:
                 raise AttributeError(f"Entity has no name. Please set name attribute.")
             if name in used:
                 raise SmartSimError("User provided two entities with the same name")
             used.append(name)
 
-    def _check_types(self, deployables):
+    def _check_types(self, deployables: t.List[t.Any]) -> None:
         for deployable in deployables:
             if not (
                 isinstance(deployable, SmartSimEntity)
                 or isinstance(deployable, EntityList)
             ):
                 raise TypeError(
                     f"Entity has type {type(deployable)}, not SmartSimEntity or EntityList"
                 )
 
-    def _check_entity_lists_nonempty(self):
+    def _check_entity_lists_nonempty(self) -> None:
         """Check deployables for sanity before launching"""
 
         for entity_list in self.all_entity_lists:
             if len(entity_list) < 1:
                 raise ValueError(f"{entity_list.name} is empty. Nothing to launch.")
 
-    def __str__(self):
+    def __str__(self) -> str:
         s = ""
         e_header = "=== Ensembles ===\n"
         m_header = "=== Models ===\n"
         db_header = "=== Database ===\n"
         if self.ensembles:
             s += e_header
 
@@ -170,33 +153,35 @@
                     s += f"Parameters: \n{fmt_dict(model.params)}\n"
             s += "\n"
 
         if self.db:
             s += db_header
             s += f"Shards: {self.db.num_shards}\n"
             s += f"Port: {str(self.db.ports[0])}\n"
-            s += f"Network: {self.db._interface}\n"
+            s += f"Network: {self.db._interfaces}\n"
             s += f"Batch Launch: {self.db.batch}\n"
             if self.db.batch:
                 s += f"{str(self.db.batch_settings)}\n"
 
         s += "\n"
         return s
 
     @property
-    def has_db_objects(self):
+    def has_db_objects(self) -> bool:
         """Check if any entity has DBObjects to set"""
 
-        def has_db_models(entity):
+        def has_db_models(entity: t.Union[EntityList, SmartSimEntity]) -> bool:
             if hasattr(entity, "_db_models"):
                 return len(entity._db_models) > 0
+            return False
 
-        def has_db_scripts(entity):
+        def has_db_scripts(entity: t.Union[EntityList, SmartSimEntity]) -> bool:
             if hasattr(entity, "_db_scripts"):
                 return len(entity._db_scripts) > 0
+            return False
 
         has_db_objects = False
         for model in self.models:
             has_db_objects |= hasattr(model, "_db_models")
 
         # Check if any model has either a DBModel or a DBScript
         # we update has_db_objects so that as soon as one check
```

### Comparing `smartsim-0.4.2/smartsim/_core/entrypoints/__init__.py` & `smartsim-0.5.0/smartsim/_core/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/entrypoints/colocated.py` & `smartsim-0.5.0/smartsim/_core/entrypoints/colocated.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,20 @@
 
 import argparse
 import os
 import signal
 import socket
 import sys
 import tempfile
+import typing as t
+
 from pathlib import Path
 from subprocess import PIPE, STDOUT
-from typing import List
+from types import FrameType
+
 
 import filelock
 import psutil
 from smartredis import Client
 from smartredis.error import RedisConnectionError, RedisReplyError
 
 from smartsim._core.utils.network import current_ip
@@ -47,19 +50,19 @@
 
 DBPID = None
 
 # kill is not catchable
 SIGNALS = [signal.SIGINT, signal.SIGTERM, signal.SIGQUIT, signal.SIGABRT]
 
 
-def handle_signal(signo, frame):
+def handle_signal(signo: int, frame: t.Optional[FrameType]) -> None:
     cleanup()
 
 
-def launch_db_model(client: Client, db_model: List[str]):
+def launch_db_model(client: Client, db_model: t.List[str]) -> str:
     """Parse options to launch model on local cluster
 
     :param client: SmartRedis client connected to local DB
     :type client: Client
     :param db_model: List of arguments defining the model
     :type db_model: List[str]
     :return: Name of model
@@ -85,44 +88,46 @@
     outputs = None
 
     if args.inputs:
         inputs = list(args.inputs)
     if args.outputs:
         outputs = list(args.outputs)
 
-    if args.devices_per_node == 1:
+    # devices_per_node being greater than one only applies
+    # to GPU devices
+    if args.devices_per_node > 1 and args.device.lower() == "gpu":
+        client.set_model_from_file_multigpu(
+            args.name,
+            args.file,
+            args.backend,
+            0,
+            args.devices_per_node,
+            args.batch_size,
+            args.min_batch_size,
+            args.tag,
+            inputs,
+            outputs
+        )
+    else:
         client.set_model_from_file(
             args.name,
             args.file,
             args.backend,
             args.device,
             args.batch_size,
             args.min_batch_size,
             args.tag,
             inputs,
-            outputs,
+            outputs
         )
-    else:
-        for device_num in range(args.devices_per_node):
-            client.set_model_from_file(
-                args.name,
-                args.file,
-                args.backend,
-                args.device + f":{device_num}",
-                args.batch_size,
-                args.min_batch_size,
-                args.tag,
-                inputs,
-                outputs,
-            )
 
     return args.name
 
 
-def launch_db_script(client: Client, db_script: List[str]):
+def launch_db_script(client: Client, db_script: t.List[str]) -> str:
     """Parse options to launch script on local cluster
 
     :param client: SmartRedis client connected to local DB
     :type client: Client
     :param db_model: List of arguments defining the script
     :type db_model: List[str]
     :return: Name of model
@@ -132,88 +137,82 @@
     parser.add_argument("--name", type=str)
     parser.add_argument("--func", type=str)
     parser.add_argument("--file", type=str)
     parser.add_argument("--backend", type=str)
     parser.add_argument("--device", type=str)
     parser.add_argument("--devices_per_node", type=int)
     args = parser.parse_args(db_script)
+
+    if args.file and args.func:
+        raise ValueError("Both file and func cannot be provided.")
+
     if args.func:
         func = args.func.replace("\\n", "\n")
-
-        if args.devices_per_node == 1:
-            client.set_script(args.name, func, args.device)
+        if args.devices_per_node > 1 and args.device.lower() == "gpu":
+            client.set_script_multigpu(args.name, func, 0, args.devices_per_node)
         else:
-            for device_num in range(args.devices_per_node):
-                client.set_script(args.name, func, args.device + f":{device_num}")
+            client.set_script(args.name, func, args.device)
     elif args.file:
-        if args.devices_per_node == 1:
-            client.set_script_from_file(args.name, args.file, args.device)
+        if args.devices_per_node > 1 and args.device.lower() == "gpu":
+            client.set_script_from_file_multigpu(args.name, args.file, 0, args.devices_per_node)
         else:
-            for device_num in range(args.devices_per_node):
-                client.set_script_from_file(
-                    args.name, args.file, args.device + f":{device_num}"
-                )
+            client.set_script_from_file(args.name, args.file, args.device)
+    else:
+        raise ValueError("No file or func provided.")
 
     return args.name
 
 
 def main(
     network_interface: str,
     db_cpus: int,
-    command: List[str],
-    db_models: List[List[str]],
-    db_scripts: List[List[str]],
-):
+    command: t.List[str],
+    db_models: t.List[t.List[str]],
+    db_scripts: t.List[t.List[str]],
+) -> None:
     global DBPID
 
+    lo_address = current_ip("lo")
     try:
-        ip_address = None
-        if network_interface:
-            ip_address = current_ip(network_interface)
-        lo_address = current_ip("lo")
+        ip_addresses = [
+            current_ip(interface) for interface in network_interface.split(",")
+        ]
+
     except ValueError as e:
         logger.warning(e)
-        ip_address = None
+        ip_addresses = []
 
-    if lo_address == ip_address or not ip_address:
+    if all(lo_address == ip_address for ip_address in ip_addresses) or not ip_addresses:
         cmd = command + [f"--bind {lo_address}"]
     else:
         # bind to both addresses if the user specified a network
         # address that exists and is not the loopback address
-        cmd = command + [f"--bind {lo_address} {ip_address}"]
+        cmd = command + [f"--bind {lo_address} {' '.join(ip_addresses)}"]
+        # pin source address to avoid random selection by Redis
+        cmd += [f"--bind-source-addr {lo_address}"]
 
     # we generally want to catch all exceptions here as
     # if this process dies, the application will most likely fail
     try:
         p = psutil.Popen(cmd, stdout=PIPE, stderr=STDOUT)
         DBPID = p.pid
 
     except Exception as e:
         cleanup()
         logger.error(f"Failed to start database process: {str(e)}")
-        raise SSInternalError("Co-located process failed to start") from e
+        raise SSInternalError("Colocated process failed to start") from e
 
     try:
-        if sys.platform != "darwin":
-            # Set CPU affinity to the last $db_cpus CPUs
-            affinity = p.cpu_affinity()
-            cpus_to_use = affinity[-db_cpus:]
-            p.cpu_affinity(cpus_to_use)
-        else:
-            # psutil doesn't support pinning on MacOS
-            cpus_to_use = "CPU pinning disabled on MacOS"
-
         logger.debug(
-            "\n\nCo-located database information\n"
+            "\n\nColocated database information\n"
             + "\n".join(
                 (
-                    f"\tIP Address: {ip_address}",
-                    f"\t# of Database CPUs: {db_cpus}",
-                    f"\tAffinity: {cpus_to_use}",
+                    f"\tIP Address(es): {' '.join(ip_addresses + [lo_address])}",
                     f"\tCommand: {' '.join(cmd)}\n\n",
+                    f"\t# of Database CPUs: {db_cpus}",
                 )
             )
         )
 
         if db_models or db_scripts:
             try:
                 client = Client(cluster=False)
@@ -235,32 +234,32 @@
                 )
 
         for line in iter(p.stdout.readline, b""):
             print(line.decode("utf-8").rstrip(), flush=True)
 
     except Exception as e:
         cleanup()
-        logger.error(f"Co-located database process failed: {str(e)}")
-        raise SSInternalError("Co-located entrypoint raised an error") from e
+        logger.error(f"Colocated database process failed: {str(e)}")
+        raise SSInternalError("Colocated entrypoint raised an error") from e
 
 
-def cleanup():
+def cleanup() -> None:
     global DBPID
     global LOCK
     try:
-        logger.debug("Cleaning up co-located database")
+        logger.debug("Cleaning up colocated database")
         # attempt to stop the database process
         db_proc = psutil.Process(DBPID)
         db_proc.terminate()
 
     except psutil.NoSuchProcess:
         logger.warning("Couldn't find database process to kill.")
 
     except OSError as e:
-        logger.warning(f"Failed to clean up co-located database gracefully: {str(e)}")
+        logger.warning(f"Failed to clean up colocated database gracefully: {str(e)}")
     finally:
         if LOCK.is_locked:
             LOCK.release()
 
         if os.path.exists(LOCK.lock_file):
             os.remove(LOCK.lock_file)
 
@@ -296,15 +295,15 @@
         )
         args = parser.parse_args()
 
         tmp_lockfile = Path(tempfile.gettempdir()) / args.lockfile
 
         LOCK = filelock.FileLock(tmp_lockfile)
         LOCK.acquire(timeout=0.1)
-        logger.debug(f"Starting co-located database on host: {socket.gethostname()}")
+        logger.debug(f"Starting colocated database on host: {socket.gethostname()}")
 
         os.environ["PYTHONUNBUFFERED"] = "1"
 
         # make sure to register the cleanup before the start
         # the proecss so our signaller will be able to stop
         # the database process.
         for sig in SIGNALS:
```

### Comparing `smartsim-0.4.2/smartsim/_core/entrypoints/redis.py` & `smartsim-0.5.0/smartsim/_core/entrypoints/redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,47 +22,50 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import argparse
 import os
-import signal
-from subprocess import PIPE, STDOUT
-from typing import List
-
 import psutil
+import signal
+import typing as t
 
 from smartsim._core.utils.network import current_ip
 from smartsim.error import SSInternalError
 from smartsim.log import get_logger
+from subprocess import PIPE, STDOUT
+from types import FrameType
 
 logger = get_logger(__name__)
 
 """
 Redis/KeyDB entrypoint script
 """
 
 DBPID = None
 
 # kill is not catchable
 SIGNALS = [signal.SIGINT, signal.SIGQUIT, signal.SIGTERM, signal.SIGABRT]
 
 
-def handle_signal(signo, frame):
+def handle_signal(signo: int, frame: t.Optional[FrameType]) -> None:
     cleanup()
 
 
-def main(network_interface: str, command: List[str]):
+def main(network_interface: str, command: t.List[str]) -> None:
     global DBPID
 
     try:
+        ip_addresses = [current_ip(net_if) for net_if in network_interface.split(",")]
+        cmd = command + [f"--bind {' '.join(ip_addresses)}"]
 
-        ip_address = current_ip(network_interface)
-        cmd = command + [f"--bind {ip_address}"]
+        # pin source address to avoid random selection by Redis
+        ip_address = ip_addresses[0]
+        cmd += [f"--bind-source-addr {ip_address}"]
 
         print("-" * 10, "  Running  Command  ", "-" * 10, "\n", flush=True)
         print(f"COMMAND: {' '.join(cmd)}\n", flush=True)
         print(f"IPADDRESS: {ip_address}\n", flush=True)
         print(f"NETWORK: {network_interface}\n", flush=True)
         print("-" * 30, "\n\n", flush=True)
 
@@ -74,15 +77,15 @@
         for line in iter(p.stdout.readline, b""):
             print(line.decode("utf-8").rstrip(), flush=True)
     except Exception as e:
         cleanup()
         raise SSInternalError("Database process starter raised an exception") from e
 
 
-def cleanup():
+def cleanup() -> None:
     global DBPID
     try:
         logger.debug("Cleaning up database instance")
         # attempt to stop the database process
         db_proc = psutil.Process(DBPID)
         db_proc.terminate()
 
@@ -90,15 +93,14 @@
         logger.warning("Couldn't find database process to kill.")
 
     except OSError as e:
         logger.warning(f"Failed to clean up database gracefully: {str(e)}")
 
 
 if __name__ == "__main__":
-
     os.environ["PYTHONUNBUFFERED"] = "1"
 
     parser = argparse.ArgumentParser(
         prefix_chars="+", description="SmartSim Process Launcher"
     )
     parser.add_argument(
         "+ifname", type=str, help="Network Interface name", default="lo"
```

### Comparing `smartsim-0.4.2/smartsim/_core/generation/__init__.py` & `smartsim-0.5.0/smartsim/_core/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/generation/generator.py` & `smartsim-0.5.0/smartsim/_core/generation/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,38 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import pathlib
 import shutil
+import typing as t
+
 from distutils import dir_util
 from os import mkdir, path, symlink
 
-from ...entity import Model
+from ...entity import Model, TaggedFilesHierarchy
 from ...log import get_logger
 from ..control import Manifest
 from .modelwriter import ModelWriter
+from ...database import Orchestrator
+from ...entity import Ensemble
+
 
 logger = get_logger(__name__)
 logger.propagate = False
 
 
 class Generator:
     """The primary job of the generator is to create the file structure
     for a SmartSim experiment. The Generator is responsible for reading
     and writing into configuration files as well.
     """
 
-    def __init__(self, gen_path, overwrite=False):
+    def __init__(self, gen_path: str, overwrite: bool = False) -> None:
         """Initialize a generator object
 
         if overwrite is true, replace any existing
         configured models within an ensemble if there
         is a name collision. Also replace any and all directories
         for the experiment with fresh copies. Otherwise, if overwrite
         is false, raises EntityExistsError when there is a name
@@ -57,15 +62,15 @@
         :param overwrite: toggle entity replacement, defaults to False
         :type overwrite: bool, optional
         """
         self._writer = ModelWriter()
         self.gen_path = gen_path
         self.overwrite = overwrite
 
-    def generate_experiment(self, *args):
+    def generate_experiment(self, *args: t.Any) -> None:
         """Run ensemble and experiment file structure generation
 
         Generate the file structure for a SmartSim experiment. This
         includes the writing and configuring of input files for a
         model.
 
         To have files or directories present in the created entity
@@ -83,98 +88,105 @@
         """
         generator_manifest = Manifest(*args)
         self._gen_exp_dir()
         self._gen_orc_dir(generator_manifest.db)
         self._gen_entity_list_dir(generator_manifest.ensembles)
         self._gen_entity_dirs(generator_manifest.models)
 
-    def set_tag(self, tag, regex=None):
+    def set_tag(self, tag: str, regex: t.Optional[str] = None) -> None:
         """Set the tag used for tagging input files
 
         Set a tag or a regular expression for the
         generator to look for when configuring new models.
 
         For example, a tag might be ``;`` where the
         expression being replaced in the model configuration
         file would look like ``;expression;``
 
         A full regular expression might tag specific
         model configurations such that the configuration
         files don't need to be tagged manually.
 
         :param tag: A string of characters that signify
-                    an string to be changed. Defaults to ``;``
+                    the string to be changed. Defaults to ``;``
         :type tag: str
+
+        :param regex: full regex for the modelwriter to search for,
+                      defaults to None
+        :type regex: str | None
         """
         self._writer.set_tag(tag, regex)
 
-    def _gen_exp_dir(self):
+    def _gen_exp_dir(self) -> None:
         """Create the directory for an experiment if it does not
         already exist.
         """
 
         if path.isfile(self.gen_path):
             raise FileExistsError(
                 f"Experiment directory could not be created. {self.gen_path} exists"
             )
         if not path.isdir(self.gen_path):
             # keep exists ok for race conditions on NFS
             pathlib.Path(self.gen_path).mkdir(exist_ok=True)
         else:
             logger.info("Working in previously created experiment")
 
-    def _gen_orc_dir(self, orchestrator):
+    def _gen_orc_dir(self, orchestrator: t.Optional[Orchestrator]) -> None:
         """Create the directory that will hold the error, output and
            configuration files for the orchestrator.
 
         :param orchestrator: Orchestrator instance
-        :type orchestrator: Orchestrator
+        :type orchestrator: Orchestrator | None
         """
 
         if not orchestrator:
             return
 
         orc_path = path.join(self.gen_path, "database")
         orchestrator.set_path(orc_path)
 
         # Always remove orchestrator files if present.
         if path.isdir(orc_path):
             shutil.rmtree(orc_path, ignore_errors=True)
         pathlib.Path(orc_path).mkdir(exist_ok=True)
 
-    def _gen_entity_list_dir(self, entity_lists):
+    def _gen_entity_list_dir(self, entity_lists: t.List[Ensemble]) -> None:
         """Generate directories for EntityList instances
 
         :param entity_lists: list of EntityList instances
         :type entity_lists: list
         """
 
         if not entity_lists:
             return
 
         for elist in entity_lists:
-
             elist_dir = path.join(self.gen_path, elist.name)
             if path.isdir(elist_dir):
                 if self.overwrite:
                     shutil.rmtree(elist_dir)
                     mkdir(elist_dir)
             else:
                 mkdir(elist_dir)
             elist.path = elist_dir
 
-            self._gen_entity_dirs(elist.entities, entity_list=elist)
+            self._gen_entity_dirs(elist.models, entity_list=elist)
 
-    def _gen_entity_dirs(self, entities, entity_list=None):
+    def _gen_entity_dirs(
+        self,
+        entities: t.List[Model],
+        entity_list: t.Optional[Ensemble] = None,
+    ) -> None:
         """Generate directories for Entity instances
 
-        :param entities: list of Entity instances
-        :type entities: list
-        :param entity_list: EntityList instance, defaults to None
-        :type entity_list: EntityList, optional
+        :param entities: list of Model instances
+        :type entities: list[Model]
+        :param entity_list: Ensemble instance, defaults to None
+        :type entity_list: Ensemble | None
         :raises EntityExistsError: if a directory already exists for an
                                    entity by that name
         """
         if not entities:
             return
 
         for entity in entities:
@@ -190,31 +202,32 @@
                     error = (
                         f"Directory for entity {entity.name} "
                         f"already exists in path {dst}"
                     )
                     raise FileExistsError(error)
             pathlib.Path(dst).mkdir(exist_ok=True)
             entity.path = dst
+
             self._copy_entity_files(entity)
             self._link_entity_files(entity)
             self._write_tagged_entity_files(entity)
 
-    def _write_tagged_entity_files(self, entity):
+    def _write_tagged_entity_files(self, entity: Model) -> None:
         """Read, configure and write the tagged input files for
            a Model instance within an ensemble. This function
            specifically deals with the tagged files attached to
            an Ensemble.
 
-        :param entity: a SmartSimEntity, for now just Models
-        :type entity: SmartSimEntity
+        :param entity: a Model instance
+        :type entity: Model
         """
         if entity.files:
             to_write = []
 
-            def _build_tagged_files(tagged):
+            def _build_tagged_files(tagged: TaggedFilesHierarchy) -> None:
                 """Using a TaggedFileHierarchy, reproduce the tagged file
                 directory structure
 
                 :param tagged: a TaggedFileHierarchy to be built as a
                                directory structure
                 :type tagged: TaggedFilesHierarchy
                 """
@@ -223,40 +236,41 @@
                     shutil.copyfile(file, dst_path)
                     to_write.append(dst_path)
 
                 for dir in tagged.dirs:
                     mkdir(path.join(entity.path, tagged.base, path.basename(dir.base)))
                     _build_tagged_files(dir)
 
-            _build_tagged_files(entity.files.tagged_hierarchy)
+            if entity.files.tagged_hierarchy:
+                _build_tagged_files(entity.files.tagged_hierarchy)
 
             # write in changes to configurations
             if isinstance(entity, Model):
                 logger.debug(
                     f"Configuring model {entity.name} with params {entity.params}"
                 )
                 self._writer.configure_tagged_model_files(to_write, entity.params)
 
-    def _copy_entity_files(self, entity):
+    def _copy_entity_files(self, entity: Model) -> None:
         """Copy the entity files and directories attached to this entity.
 
-        :param entity: SmartSimEntity
-        :type entity: SmartSimEntity
+        :param entity: Model
+        :type entity: Model
         """
         if entity.files:
             for to_copy in entity.files.copy:
                 dst_path = path.join(entity.path, path.basename(to_copy))
                 if path.isdir(to_copy):
                     dir_util.copy_tree(to_copy, entity.path)
                 else:
                     shutil.copyfile(to_copy, dst_path)
 
-    def _link_entity_files(self, entity):
+    def _link_entity_files(self, entity: Model) -> None:
         """Symlink the entity files attached to this entity.
 
-        :param entity: SmartSimEntity
-        :type entity: SmartSimEntity
+        :param entity: Model
+        :type entity: Model
         """
         if entity.files:
             for to_link in entity.files.link:
                 dst_path = path.join(entity.path, path.basename(to_link))
                 symlink(to_link, dst_path)
```

### Comparing `smartsim-0.4.2/smartsim/_core/generation/modelwriter.py` & `smartsim-0.5.0/smartsim/_core/generation/modelwriter.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import re
+import typing as t
 
 from smartsim.error.errors import SmartSimError
 
 from ...error import ParameterWriterError
 from ...log import get_logger
 
 logger = get_logger(__name__)
 
 
 class ModelWriter:
-    def __init__(self):
+    def __init__(self) -> None:
         self.tag = ";"
         self.regex = "(;[^;]+;)"
-        self.lines = []
+        self.lines: t.List[str] = []
 
-    def set_tag(self, tag, regex=None):
+    def set_tag(self, tag: str, regex: t.Optional[str] = None) -> None:
         """Set the tag for the modelwriter to search for within
            tagged files attached to an entity.
 
         :param tag: tag for the modelwriter to search for,
                     defaults to semi-colon e.g. ";"
         :type tag: str
         :param regex: full regex for the modelwriter to search for,
@@ -54,16 +55,16 @@
         if regex:
             self.regex = regex
         else:
             self.tag = tag
             self.regex = "".join(("(", tag, ".+", tag, ")"))
 
     def configure_tagged_model_files(
-        self, tagged_files, params, make_missing_tags_fatal=False
-    ):
+        self, tagged_files: t.List[str], params: t.Dict[str, str], make_missing_tags_fatal: bool = False
+    ) -> None:
         """Read, write and configure tagged files attached to a Model
            instance.
 
         :param tagged_files: list of paths to tagged files
         :type model: list[str]
         :param params: model parameters
         :type params: dict[str, str]
@@ -71,52 +72,52 @@
         :type make_missing_tags_fatal: bool
         """
         for tagged_file in tagged_files:
             self._set_lines(tagged_file)
             self._replace_tags(params, make_missing_tags_fatal)
             self._write_changes(tagged_file)
 
-    def _set_lines(self, file_path):
+    def _set_lines(self, file_path: str) -> None:
         """Set the lines for the modelwrtter to iterate over
 
         :param file_path: path to the newly created and tagged file
         :type file_path: str
         :raises ParameterWriterError: if the newly created file cannot be read
         """
         try:
             fp = open(file_path, "r+")
             self.lines = fp.readlines()
             fp.close()
         except (IOError, OSError) as e:
             raise ParameterWriterError(file_path) from e
 
-    def _write_changes(self, file_path):
+    def _write_changes(self, file_path: str) -> None:
         """Write the ensemble-specific changes
 
         :raises ParameterWriterError: if the newly created file cannot be read
         """
         try:
             fp = open(file_path, "w+")
             for line in self.lines:
                 fp.write(line)
             fp.close()
         except (IOError, OSError) as e:
             raise ParameterWriterError(file_path, read=False) from e
 
-    def _replace_tags(self, params, make_fatal=False):
+    def _replace_tags(self, params: t.Dict[str, str], make_fatal: bool = False) -> None:
         """Replace the tagged within the tagged file attached to this
            model. The tag defaults to ";"
 
         :param model: The model instance
         :type model: Model
         :param make_fatal: (Optional) Set to True to force a fatal error if a tag is not matched
         :type make_fatal: bool
         """
         edited = []
-        unused_tags = {}
+        unused_tags: t.Dict[str, t.List[int]] = {}
         for i, line in enumerate(self.lines):
             search = re.search(self.regex, line)
             if search:
                 while search:
                     tagged_line = search.group(0)
                     previous_value = self._get_prev_value(tagged_line)
                     if self._is_ensemble_spec(tagged_line, params):
@@ -132,30 +133,30 @@
                     # put in placeholder value
                     else:
                         tag = tagged_line.split(self.tag)[1]
                         if tag not in unused_tags:
                             unused_tags[tag] = []
                         unused_tags[tag].append(i + 1)
                         edited.append(re.sub(self.regex, previous_value, line))
-                        search = False  # Move on to the next tag
+                        search = None  # Move on to the next tag
             else:
                 edited.append(line)
         for tag in unused_tags:
             missing_tag_message = (
                 f"Unused tag {tag} on line(s): {str(unused_tags[tag])}"
             )
             if make_fatal:
                 raise SmartSimError(missing_tag_message)
             else:
                 logger.warning(missing_tag_message)
         self.lines = edited
 
-    def _is_ensemble_spec(self, tagged_line, model_params):
+    def _is_ensemble_spec(self, tagged_line: str, model_params: t.Dict[str, str]) -> bool:
         split_tag = tagged_line.split(self.tag)
         prev_val = split_tag[1]
         if prev_val in model_params.keys():
             return True
         return False
 
-    def _get_prev_value(self, tagged_line):
+    def _get_prev_value(self, tagged_line: str) -> str:
         split_tag = tagged_line.split(self.tag)
         return split_tag[1]
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from .launcher import Launcher
 from .cobalt.cobaltLauncher import CobaltLauncher
 from .local.local import LocalLauncher
 from .lsf.lsfLauncher import LSFLauncher
 from .pbs.pbsLauncher import PBSLauncher
 from .slurm.slurmLauncher import SlurmLauncher
 
 __all__ = [
+    "Launcher",
     "CobaltLauncher",
     "LocalLauncher",
     "LSFLauncher",
     "PBSLauncher",
     "SlurmLauncher",
 ]
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/cobalt/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/cobalt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltCommands.py` & `smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltCommands.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltLauncher.py` & `smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltLauncher.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,33 +21,38 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
+import typing as t
 
 import psutil
 
+from smartsim._core.launcher.step import Step
+from smartsim.settings import RunSettings, SettingsBase
+
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
 from ....status import STATUS_CANCELLED, STATUS_COMPLETED
 from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..pbs.pbsCommands import qdel, qstat
 from ..step import (
+    Step,
     AprunStep,
     CobaltBatchStep,
     LocalStep,
     MpiexecStep,
     MpirunStep,
     OrterunStep,
 )
-from ..stepInfo import CobaltStepInfo
+from ..stepInfo import CobaltStepInfo, StepInfo
 from .cobaltParser import parse_cobalt_step_id, parse_cobalt_step_status, parse_qsub_out
 
 logger = get_logger(__name__)
 
 
 class CobaltLauncher(WLMLauncher):
     """This class encapsulates the functionality needed
@@ -56,29 +61,32 @@
     All WLM launchers are capable of launching managed and unmanaged
     jobs. Managed jobs are queried through interaction with with WLM,
     in this case Cobalt. Unmanaged jobs are held in the TaskManager
     and are managed through references to their launching process ID
     i.e. a psutil.Popen object
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.user = psutil.Process().username()
 
-    # RunSettings types supported by this launcher
-    supported_rs = {
-        AprunSettings: AprunStep,
-        CobaltBatchSettings: CobaltBatchStep,
-        MpirunSettings: MpirunStep,
-        MpiexecSettings: MpiexecStep,
-        OrterunSettings: OrterunStep,
-        RunSettings: LocalStep,
-    }
+    @property
+    def supported_rs(self) -> t.Dict[t.Type[SettingsBase], t.Type[Step]]:
+        # RunSettings types supported by this launcher
+        return {
+            AprunSettings: AprunStep,
+            CobaltBatchSettings: CobaltBatchStep,
+            MpirunSettings: MpirunStep,
+            MpiexecSettings: MpiexecStep,
+            OrterunSettings: OrterunStep,
+            RunSettings: LocalStep,
+        }    
+
 
-    def run(self, step):
+    def run(self, step: Step) -> t.Optional[str]:
         """Run a job step through Cobalt
 
         :param step: a job step instance
         :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
         :rtype: str
@@ -100,47 +108,52 @@
                 step_id = parse_qsub_out(out)
                 logger.debug(f"Gleaned batch job id: {step_id} for {step.name}")
         else:
             # aprun doesn't direct output for us.
             out, err = step.get_output_files()
             output = open(out, "w+")
             error = open(err, "w+")
+
             task_id = self.task_manager.start_task(
-                cmd_list, step.cwd, out=output, err=error
+                cmd_list, step.cwd, out=output.fileno(), err=error.fileno()
             )
 
         # if batch submission did not successfully retrieve job ID
         if not step_id and step.managed:
             step_id = self._get_cobalt_step_id(step)
+
         self.step_mapping.add(step.name, step_id, task_id, step.managed)
         return step_id
 
-    def stop(self, step_name):
+    def stop(self, step_name: str) -> StepInfo:
         """Step a job step
 
         :param step_name: name of the job to stop
         :type step_name: str
         :return: update for job due to cancel
         :rtype: StepInfo
         """
         stepmap = self.step_mapping[step_name]
         if stepmap.managed:
             qdel_rc, _, err = qdel([str(stepmap.step_id)])
             if qdel_rc != 0:
                 logger.warning(f"Unable to cancel job step {step_name}\n {err}")
             if stepmap.task_id:
-                self.task_manager.remove_task(stepmap.task_id)
+                self.task_manager.remove_task(str(stepmap.task_id))
         else:
-            self.task_manager.remove_task(stepmap.task_id)
+            if stepmap.task_id:
+                self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
+        if not step_info:
+            raise LauncherError(f"Could not get step_info for job step {step_name}")
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_cobalt_step_id(self, step, interval=2):
+    def _get_cobalt_step_id(self, step: Step, interval: int = 2) -> str:
         """Get the step_id of a step from qstat (rarely used)
 
         Parses cobalt qstat output by looking for the step name
         """
         step_id = None
         trials = CONFIG.wlm_trials
         while trials > 0:
@@ -151,15 +164,15 @@
             else:
                 time.sleep(interval)
                 trials -= 1
         if not step_id:
             raise LauncherError("Could not find id of launched job step")
         return step_id
 
-    def _get_managed_step_update(self, step_ids):
+    def _get_managed_step_update(self, step_ids: t.List[str]) -> t.List[StepInfo]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
         :type step_ids: list[str]
         :return: list of updates for managed jobs
         :rtype: list[StepInfo]
         """
@@ -167,19 +180,19 @@
         args.extend(step_ids)
         qstat_out, _ = qstat(args)
 
         stats = [
             parse_cobalt_step_status(qstat_out, str(step_id)) for step_id in step_ids
         ]
         # create CobaltStepInfo objects to return
-        updates = []
+        updates: t.List[StepInfo] = []
         for stat, _ in zip(stats, step_ids):
             info = CobaltStepInfo(stat, None)  # returncode not logged by Cobalt
 
             if info.status == STATUS_COMPLETED:
                 info.returncode = 0
 
             updates.append(info)
         return updates
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "Cobalt"
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltParser.py` & `smartsim-0.5.0/smartsim/_core/launcher/cobalt/cobaltParser.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,48 +20,69 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 
-def parse_cobalt_step_status(output, step_id):
+
+def parse_cobalt_step_status(output: str, step_id: str) -> str:
+    """
+    Parse and return the status of a cobalt step
+
+    :param output: output qstat
+    :type output: str
+    :param step_id: the id of the step to query
+    :type step_id: str
+    :rtype: str
+    """
     status = "NOTFOUND"
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 2:
             if fields[0] == step_id:
                 status = fields[1]
                 break
     return status
 
 
-def parse_cobalt_step_id(output, step_name):
+def parse_cobalt_step_id(output: str, step_name: str) -> str:
     """Parse and return the step id from a cobalt qstat command
 
     :param output: output qstat
     :type output: str
     :param step_name: the name of the step to query
     :type step_name: str
     :return: the step_id
     :rtype: str
     """
-    step_id = None
+    step_id = ""
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 2:
             if fields[0] == step_name:
                 step_id = fields[1]
                 break
     return step_id
 
 
-def parse_qsub_out(output):
-    step_id = None
+def parse_qsub_out(output: str) -> str:
+    """
+    Parse and return the step id from a cobalt qsub command
+
+    :param output: output qstat
+    :type output: str
+    :return: the step_id
+    :rtype: str
+    """
+    step_id = ""
     for line in output.split("\n"):
         try:
-            step_id = int(line.strip())
+            value = line.strip()
+            int(value) # if the cast works, return original string
+            step_id = value
             break
         except ValueError:
             continue
-    return str(step_id)
+    return step_id
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/colocated.py` & `smartsim-0.5.0/smartsim/_core/launcher/colocated.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import sys
+import typing as t
 
-from ...error import SSInternalError, SSUnsupportedError
+
+
+from ...error import SSInternalError
 from ..config import CONFIG
 from ..utils.helpers import create_lockfile_name
+from ...entity.dbobject import DBModel, DBScript
 
-
-def write_colocated_launch_script(file_name, db_log, colocated_settings):
+def write_colocated_launch_script(file_name: str, db_log: str, colocated_settings: t.Dict[str, t.Any]) -> None:
     """Write the colocated launch script
 
     This file will be written into the cwd of the step that
     is created for this entity.
 
     :param file_name: name of the script to write
     :type file_name: str
@@ -63,70 +66,92 @@
         # STDOUT of the job
         if colocated_settings["debug"]:
             f.write("export SMARTSIM_LOG_LEVEL=debug\n")
 
         f.write(f"{colocated_cmd}\n")
         f.write(f"DBPID=$!\n\n")
 
-        if colocated_settings["limit_app_cpus"]:
-            cpus = colocated_settings["cpus"]
-            f.write(f"taskset -c 0-$(nproc --ignore={str(cpus+1)}) $@\n\n")
-        else:
-            f.write(f"$@\n\n")
+        # Write the actual launch command for the app
+        f.write(f"$@\n\n")
 
 
 def _build_colocated_wrapper_cmd(
-    db_log,
-    cpus=1,
-    rai_args=None,
-    extra_db_args=None,
-    port=6780,
-    ifname=None,
-    **kwargs,
-):
-    """Build the command use to run a colocated db application
+    db_log: str,
+    cpus: int = 1,
+    rai_args: t.Optional[t.Dict[str, str]] = None,
+    extra_db_args: t.Optional[t.Dict[str, str]] = None,
+    port: int = 6780,
+    ifname: t.Optional[t.Union[str, t.List[str]]] = None,
+    custom_pinning: t.Optional[str] = None,
+    **kwargs: t.Any,
+) -> str:
+    """Build the command use to run a colocated DB application
 
+    :param db_log: log file for the db
+    :type db_log: str
     :param cpus: db cpus, defaults to 1
     :type cpus: int, optional
     :param rai_args: redisai args, defaults to None
     :type rai_args: dict[str, str], optional
     :param extra_db_args: extra redis args, defaults to None
     :type extra_db_args: dict[str, str], optional
+    :param port: port to bind DB to
+    :type port: int
+    :param ifname: network interface(s) to bind DB to
+    :type ifname: str | list[str], optional
+    :param db_cpu_list: The list of CPUs that the database should be limited to
+    :type db_cpu_list: str, optional
     :return: the command to run
     :rtype: str
     """
 
     # create unique lockfile name to avoid symlink vulnerability
     # this is the lockfile all the processes in the distributed
     # application will try to acquire. since we use a local tmp
     # directory on the compute node, only one process can acquire
     # the lock on the file.
     lockfile = create_lockfile_name()
 
     # create the command that will be used to launch the
     # database with the python entrypoint for starting
     # up the backgrounded db process
+
     cmd = [
-        sys.executable,
-        "-m",
-        "smartsim._core.entrypoints.colocated",
-        "+lockfile",
-        lockfile,
-        "+db_cpus",
-        str(cpus),
-    ]
+            sys.executable,
+            "-m",
+            "smartsim._core.entrypoints.colocated",
+            "+lockfile",
+            lockfile,
+            "+db_cpus",
+            str(cpus),
+        ]
     # Add in the interface if using TCP/IP
     if ifname:
-        cmd.extend(["+ifname", ifname])
+        if isinstance(ifname, str):
+            ifname = [ifname]
+        cmd.extend(["+ifname", ",".join(ifname)])
     cmd.append("+command")
     # collect DB binaries and libraries from the config
-    db_cmd = [CONFIG.database_exe, CONFIG.database_conf, "--loadmodule", CONFIG.redisai]
+
+    db_cmd = []
+    if custom_pinning:
+        db_cmd.extend([
+            'taskset', '-c', custom_pinning
+        ])
+    db_cmd.extend(
+        [
+            CONFIG.database_exe,
+            CONFIG.database_conf,
+            "--loadmodule",
+            CONFIG.redisai
+        ]
+    )
 
     # add extra redisAI configurations
-    for arg, value in rai_args.items():
+    for arg, value in (rai_args or {}).items():
         if value:
             # RAI wants arguments for inference in all caps
             # ex. THREADS_PER_QUEUE=1
             db_cmd.append(f"{arg.upper()} {str(value)}")
 
     db_cmd.extend(["--port", str(port)])
 
@@ -147,21 +172,22 @@
         raise SSInternalError(
             "`unix_socket` and `socket_permissions` must both be defined or undefined."
         )
 
     db_cmd.extend(
         ["--logfile", db_log]
     )  # usually /dev/null, unless debug was specified
-    for db_arg, value in extra_db_args.items():
-        # replace "_" with "-" in the db_arg because we use kwargs
-        # for the extra configurations and Python doesn't allow a hyphen
-        # in a variable name. All redis and KeyDB configuration options
-        # use hyphens in their names.
-        db_arg = db_arg.replace("_", "-")
-        db_cmd.extend([f"--{db_arg}", value])
+    if extra_db_args:
+        for db_arg, value in extra_db_args.items():
+            # replace "_" with "-" in the db_arg because we use kwargs
+            # for the extra configurations and Python doesn't allow a hyphen
+            # in a variable name. All redis and KeyDB configuration options
+            # use hyphens in their names.
+            db_arg = db_arg.replace("_", "-")
+            db_cmd.extend([f"--{db_arg}", value])
 
     db_models = kwargs.get("db_models", None)
     if db_models:
         db_model_cmd = _build_db_model_cmd(db_models)
         db_cmd.extend(db_model_cmd)
 
     db_scripts = kwargs.get("db_scripts", None)
@@ -172,15 +198,15 @@
     # run colocated db in the background
     db_cmd.append("&")
 
     cmd.extend(db_cmd)
     return " ".join(cmd)
 
 
-def _build_db_model_cmd(db_models):
+def _build_db_model_cmd(db_models: t.List[DBModel]) -> t.List[str]:
     cmd = []
     for db_model in db_models:
         cmd.append("+db_model")
         cmd.append(f"--name={db_model.name}")
 
         # Here db_model.file is guaranteed to exist
         # because we don't allow the user to pass a serialized DBModel
@@ -201,15 +227,15 @@
             cmd.append("--inputs=" + ",".join(db_model.inputs))
         if db_model.outputs:
             cmd.append("--outputs=" + ",".join(db_model.outputs))
 
     return cmd
 
 
-def _build_db_script_cmd(db_scripts):
+def _build_db_script_cmd(db_scripts: t.List[DBScript]) -> t.List[str]:
     cmd = []
     for db_script in db_scripts:
         cmd.append("+db_script")
         cmd.append(f"--name={db_script.name}")
         if db_script.func:
             # Notice that here db_script.func is guaranteed to be a str
             # because we don't allow the user to pass a serialized function
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/launcher.py` & `smartsim-0.5.0/smartsim/_core/launcher/launcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,68 +21,75 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import abc
+import typing as t
 
 from ...error import AllocationError, LauncherError, SSUnsupportedError
-from .stepInfo import UnmanagedStepInfo
+from .stepInfo import UnmanagedStepInfo, StepInfo
 from .stepMapping import StepMapping
 from .taskManager import TaskManager
+from .step import Step
+from ...settings import SettingsBase
 
 
 class Launcher(abc.ABC):  # pragma: no cover
     """Abstract base class of all launchers
 
     This class provides the interface between the experiment
     controller and the launcher layer. Each launcher supported
     in SmartSim should implement the methods in this class to
     be fully compatible.
     """
+    step_mapping: StepMapping
+    task_manager: TaskManager
 
-    def __init__(self):
-        pass
+    @property
+    @abc.abstractmethod
+    def supported_rs(self) -> t.Dict[t.Type[SettingsBase], t.Type[Step]]:
+        raise NotImplementedError
 
     @abc.abstractmethod
-    def create_step(self, name, cwd, step_settings):
+    def create_step(self, name: str, cwd: str, step_settings: SettingsBase) -> Step:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get_step_update(self, step_names):
+    def get_step_update(self, step_names: t.List[str]) -> t.List[t.Tuple[str, t.Union[StepInfo, None]]]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get_step_nodes(self, step_names):
+    def get_step_nodes(self, step_names: t.List[str]) -> t.List[t.List[str]]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def run(self, step):
+    def run(self, step: Step) -> t.Optional[str]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def stop(self, step_name):
+    def stop(self, step_name: str) -> StepInfo:
         raise NotImplementedError
 
 
 class WLMLauncher(Launcher):  # cov-wlm
     """The base class for any Launcher that utilizes workload
     manager specific commands. This base class is used to provide
     implemented methods that are alike across all WLM launchers.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.task_manager = TaskManager()
         self.step_mapping = StepMapping()
 
     # every launcher utilizing this interface must have a map
     # of supported RunSettings types (see slurmLauncher.py for ex)
-    def create_step(self, name, cwd, step_settings):  # cov-wlm
+    def create_step(self, name: str, cwd: str, step_settings: SettingsBase) -> Step:  # cov-wlm
         """Create a WLM job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param step_settings: batch or run settings for entity
@@ -103,61 +110,64 @@
             )
         except AllocationError as e:
             raise LauncherError("Step creation failed") from e
 
     # these methods are implemented in WLM launchers and
     # don't need to be covered here.
 
-    def get_step_nodes(self, step_names):  # pragma: no cover
+    def get_step_nodes(self, step_names: t.List[str]) -> t.List[t.List[str]]:  # pragma: no cover
         raise SSUnsupportedError("Node acquisition not supported for this launcher")
 
-    def run(self, step):  # pragma: no cover
+    def run(self, step: Step) -> t.Optional[str]:  # pragma: no cover
         raise NotImplementedError
 
-    def stop(self, step_name):  # pragma: no cover
+    def stop(self, step_name: str) -> StepInfo:  # pragma: no cover
         raise NotImplementedError
 
-    def get_step_update(self, step_names):  # cov-wlm
+    def get_step_update(self, step_names: t.List[str]) -> t.List[t.Tuple[str, t.Union[StepInfo, None]]]:  # cov-wlm
         """Get update for a list of job steps
 
         :param step_names: list of job steps to get updates for
         :type step_names: list[str]
         :return: list of name, job update tuples
         :rtype: list[(str, StepInfo)]
         """
-        updates = []
+        updates: t.List[t.Tuple[str, t.Union[StepInfo, None]]] = []
 
         # get updates of jobs managed by workload manager (PBS, Slurm, etc)
         # this is primarily batch jobs.
         s_names, step_ids = self.step_mapping.get_ids(step_names, managed=True)
         if len(step_ids) > 0:
-            s_statuses = self._get_managed_step_update(step_ids)
-            _updates = [(name, stat) for name, stat in zip(s_names, s_statuses)]
-            updates.extend(_updates)
+            _step_ids = [str(sid) for sid in step_ids]
+            s_statuses = self._get_managed_step_update(_step_ids)
+            if s_statuses:
+                _updates = [(name, stat) for name, stat in zip(s_names, s_statuses)]
+                updates.extend(_updates)
 
         # get updates of unmanaged jobs (Aprun, mpirun, etc)
         # usually jobs started and monitored through the Popen interface
         t_names, task_ids = self.step_mapping.get_ids(step_names, managed=False)
         if len(task_ids) > 0:
-            t_statuses = self._get_unmanaged_step_update(task_ids)
+            _task_ids = [str(tid) for tid in task_ids]
+            t_statuses = self._get_unmanaged_step_update(_task_ids)
             _updates = [(name, stat) for name, stat in zip(t_names, t_statuses)]
             updates.extend(_updates)
 
         return updates
 
-    def _get_unmanaged_step_update(self, task_ids):  # cov-wlm
+    def _get_unmanaged_step_update(self, task_ids: t.List[str]) -> t.List[UnmanagedStepInfo]:  # cov-wlm
         """Get step updates for Popen managed jobs
 
         :param task_ids: task id to check
         :type task_ids: list[str]
         :return: list of step updates
         :rtype: list[StepInfo]
         """
         updates = []
         for task_id in task_ids:
             stat, rc, out, err = self.task_manager.get_task_update(task_id)
             update = UnmanagedStepInfo(stat, rc, out, err)
             updates.append(update)
         return updates
 
-    def _get_managed_step_update(self, step_ids):  # pragma: no cover
-        pass
+    def _get_managed_step_update(self, step_ids: t.List[str]) -> t.Optional[t.List[StepInfo]]:  # pragma: no cover
+        return None
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/local/local.py` & `smartsim-0.5.0/smartsim/_core/launcher/local/local.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,102 +20,119 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 
+from ..launcher import Launcher
 from ....log import get_logger
-from ....settings import RunSettings
+from ....settings import RunSettings, SettingsBase
 from ..step import LocalStep
-from ..stepInfo import UnmanagedStepInfo
+from ..step import Step
+from ..stepInfo import UnmanagedStepInfo, StepInfo
 from ..stepMapping import StepMapping
 from ..taskManager import TaskManager
 
 logger = get_logger(__name__)
 
 
-class LocalLauncher:
+class LocalLauncher(Launcher):
     """Launcher used for spawning proceses on a localhost machine."""
 
-    def __init__(self):
+    @property
+    def supported_rs(self) -> t.Dict[t.Type[SettingsBase], t.Type[Step]]:
+       return {
+            RunSettings: LocalStep,
+        }    
+    
+    def __init__(self) -> None:
         self.task_manager = TaskManager()
         self.step_mapping = StepMapping()
 
-    def create_step(self, name, cwd, step_settings):
+    def create_step(self, name: str, cwd: str, step_settings: SettingsBase) -> Step:
         """Create a job step to launch an entity locally
 
         :return: Step object
         """
         if not isinstance(step_settings, RunSettings):
             raise TypeError(
                 f"Local Launcher only supports entities with RunSettings, not {type(step_settings)}"
             )
         step = LocalStep(name, cwd, step_settings)
         return step
 
-    def get_step_update(self, step_names):
+    def get_step_update(self, step_names: t.List[str]) -> t.List[t.Tuple[str, t.Optional[StepInfo]]]:
         """Get status updates of each job step name provided
 
         :param step_names: list of step_names
         :type step_names: list[str]
         :return: list of tuples for update
         :rtype: list[(str, UnmanagedStepInfo)]
         """
         # step ids are process ids of the tasks
         # as there is no WLM intermediary
-        updates = []
+        updates: t.List[t.Tuple[str, t.Optional[StepInfo]]] = []
         s_names, s_ids = self.step_mapping.get_ids(step_names, managed=False)
         for step_name, step_id in zip(s_names, s_ids):
-            status, rc, out, err = self.task_manager.get_task_update(step_id)
+            status, rc, out, err = self.task_manager.get_task_update(str(step_id))
             step_info = UnmanagedStepInfo(status, rc, out, err)
             update = (step_name, step_info)
             updates.append(update)
         return updates
 
-    def get_step_nodes(self, step_names):
+    def get_step_nodes(self, step_names: t.List[str]) -> t.List[t.List[str]]:
         """Return the address of nodes assigned to the step
 
         TODO: Use socket to find the actual Lo address?
         :return: a list containing the local host address
         """
         return [["127.0.0.1"] * len(step_names)]
 
-    def run(self, step):
+    def run(self, step: Step) -> str:
         """Run a local step created by this launcher. Utilize the shell
            library to execute the command with a Popen. Output and error
            files will be written to the entity path.
 
         :param step: LocalStep instance to run
         :type step: LocalStep
+        :return: task_id of the newly created step
+        :rtype: str
         """
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         out, err = step.get_output_files()
         output = open(out, "w+")
         error = open(err, "w+")
         cmd = step.get_launch_cmd()
+
+        env = {}
+        if isinstance(step, LocalStep):
+            env = step.env
+
         task_id = self.task_manager.start_task(
-            cmd, step.cwd, env=step.env, out=output, err=error
+            cmd, step.cwd, env=env, out=output.fileno(), err=error.fileno()
         )
         self.step_mapping.add(step.name, task_id=task_id, managed=False)
         return task_id
 
-    def stop(self, step_name):
+    def stop(self, step_name: str) -> UnmanagedStepInfo:
         """Stop a job step
 
         :param step_name: name of the step to be stopped
         :type step_name: str
         :return: a UnmanagedStepInfo instance
         :rtype: UnmanagedStepInfo
         """
         # step_id is task_id for local. Naming for consistency
         step_id = self.step_mapping[step_name].task_id
-        self.task_manager.remove_task(step_id)
-        status, rc, out, err = self.task_manager.get_task_update(step_id)
-        status = UnmanagedStepInfo("Cancelled", rc, out, err)
-        return status
+        
+        self.task_manager.remove_task(str(step_id))
+        _, rc, out, err = self.task_manager.get_task_update(str(step_id))
+        step_info = UnmanagedStepInfo("Cancelled", rc, out, err)
+        return step_info
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "Local"
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/lsf/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/lsf/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfCommands.py` & `smartsim-0.5.0/smartsim/_core/launcher/lsf/lsfCommands.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,45 +20,47 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from ..util.shell import execute_cmd
 
 
-def bjobs(args):
+def bjobs(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls LSF bjobs with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of bjobs
     """
     cmd = ["bjobs"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def bkill(args):
+def bkill(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls LSF bkill with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
     :type args: list of str
     :return: returncode, output and error
     :rtype: (int, str, str)
     """
     cmd = ["bkill"] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
 
 
-def jskill(args):
+def jskill(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls LSF jskill with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
     :type args: list of str
     :return: returncode, output and error
@@ -66,15 +68,15 @@
     """
 
     cmd = ["jskill"] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
 
 
-def jslist(args):
+def jslist(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls LSF jslist with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of jslist
     :rtype: (str, str)
     """
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfLauncher.py` & `smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsLauncher.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,174 +21,169 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
+import typing as t
 
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
+from ....settings import SettingsBase
 from ....status import STATUS_CANCELLED, STATUS_COMPLETED
 from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..step import (
-    BsubBatchStep,
-    JsrunStep,
+    Step,
+    AprunStep,
     LocalStep,
     MpiexecStep,
     MpirunStep,
     OrterunStep,
+    QsubBatchStep,
 )
-from ..stepInfo import LSFBatchStepInfo, LSFJsrunStepInfo
-from .lsfCommands import bjobs, bkill, jskill, jslist
-from .lsfParser import (
-    parse_bjobs_jobid,
-    parse_bsub,
-    parse_jslist_stepid,
-    parse_max_step_id_from_jslist,
-)
+from ..stepInfo import PBSStepInfo, StepInfo
+from .pbsCommands import qdel, qstat
+from .pbsParser import parse_qstat_jobid, parse_step_id_from_qstat
 
 logger = get_logger(__name__)
 
 
-class LSFLauncher(WLMLauncher):
+class PBSLauncher(WLMLauncher):
     """This class encapsulates the functionality needed
-    to launch jobs on systems that use LSF as a workload manager.
+    to launch jobs on systems that use PBS as a workload manager.
 
     All WLM launchers are capable of launching managed and unmanaged
     jobs. Managed jobs are queried through interaction with with WLM,
-    in this case LSF. Unmanaged jobs are held in the TaskManager
+    in this case PBS. Unmanaged jobs are held in the TaskManager
     and are managed through references to their launching process ID
     i.e. a psutil.Popen object
     """
 
     # init in WLMLauncher, launcher.py
 
-    # RunSettings types supported by this launcher
-    supported_rs = {
-        JsrunSettings: JsrunStep,
-        BsubBatchSettings: BsubBatchStep,
-        MpirunSettings: MpirunStep,
-        MpiexecSettings: MpiexecStep,
-        OrterunSettings: OrterunStep,
-        RunSettings: LocalStep,
-    }
+    @property
+    def supported_rs(self) -> t.Dict[t.Type[SettingsBase], t.Type[Step]]:
+        # RunSettings types supported by this launcher
+        return {
+            AprunSettings: AprunStep,
+            QsubBatchSettings: QsubBatchStep,
+            MpiexecSettings: MpiexecStep,
+            MpirunSettings: MpirunStep,
+            OrterunSettings: OrterunStep,
+            RunSettings: LocalStep,
+            PalsMpiexecSettings: MpiexecStep,
+        }
 
-    def run(self, step):
-        """Run a job step through LSF
+    def run(self, step: Step) -> t.Optional[str]:
+        """Run a job step through PBSPro
 
         :param step: a job step instance
         :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
         :rtype: str
         """
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         cmd_list = step.get_launch_cmd()
-        step_id = None
-        task_id = None
-        if isinstance(step, BsubBatchStep):
+        step_id: t.Optional[str] = None
+        task_id: t.Optional[str] = None
+        if isinstance(step, QsubBatchStep):
             # wait for batch step to submit successfully
             rc, out, err = self.task_manager.start_and_wait(cmd_list, step.cwd)
             if rc != 0:
-                raise LauncherError(f"Bsub batch submission failed\n {out}\n {err}")
+                raise LauncherError(f"Qsub batch submission failed\n {out}\n {err}")
             if out:
-                step_id = parse_bsub(out)
+                step_id = out.strip()
                 logger.debug(f"Gleaned batch job id: {step_id} for {step.name}")
-        elif isinstance(step, JsrunStep):
-            self.task_manager.start_task(cmd_list, step.cwd)
-            time.sleep(1)
-            step_id = self._get_lsf_step_id(step)
-            logger.debug(f"Gleaned jsrun step id: {step_id} for {step.name}")
-        else:  # isinstance(step, MpirunStep) or isinstance(step, LocalStep)
+        else:
+            # aprun doesn't direct output for us.
             out, err = step.get_output_files()
-            # mpirun and local launch don't direct output for us
             output = open(out, "w+")
             error = open(err, "w+")
             task_id = self.task_manager.start_task(
-                cmd_list, step.cwd, out=output, err=error
+                cmd_list, step.cwd, out=output.fileno(), err=error.fileno()
             )
 
+        # if batch submission did not successfully retrieve job ID
+        if not step_id and step.managed:
+            step_id = self._get_pbs_step_id(step)
+        
         self.step_mapping.add(step.name, step_id, task_id, step.managed)
+
         return step_id
 
-    def stop(self, step_name):
+    def stop(self, step_name: str) -> StepInfo:
         """Stop/cancel a job step
 
         :param step_name: name of the job to stop
         :type step_name: str
         :return: update for job due to cancel
         :rtype: StepInfo
         """
         stepmap = self.step_mapping[step_name]
         if stepmap.managed:
-            if "." in stepmap.step_id:
-                rc, _, err = jskill([stepmap.step_id.rpartition(".")[-1]])
-            else:
-                rc, _, err = bkill([str(stepmap.step_id)])
-            if rc != 0:
+            qdel_rc, _, err = qdel([str(stepmap.step_id)])
+            if qdel_rc != 0:
                 logger.warning(f"Unable to cancel job step {step_name}\n {err}")
             if stepmap.task_id:
-                self.task_manager.remove_task(stepmap.task_id)
+                self.task_manager.remove_task(str(stepmap.task_id))
         else:
-            self.task_manager.remove_task(stepmap.task_id)
+            self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
+        if not step_info:
+            raise LauncherError(f"Could not get step_info for job step {step_name}")
+
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_lsf_step_id(self, step, interval=2):
-        """Get the step_id of last launched step from jslist"""
+    def _get_pbs_step_id(self, step: Step, interval: int = 2) -> str:
+        """Get the step_id of a step from qstat (rarely used)
+
+        Parses qstat JSON output by looking for the step name
+        TODO: change this to use ``qstat -a -u user``
+        """
         time.sleep(interval)
-        step_id = "unassigned"
+        step_id: t.Optional[str] = None
         trials = CONFIG.wlm_trials
         while trials > 0:
-            output, _ = jslist([])
-            step_id = parse_max_step_id_from_jslist(output)
+            output, _ = qstat(["-f", "-F", "json"])
+            step_id = parse_step_id_from_qstat(output, step.name)
             if step_id:
                 break
             else:
                 time.sleep(interval)
                 trials -= 1
         if not step_id:
             raise LauncherError("Could not find id of launched job step")
-        return f"{step.alloc}.{step_id}"
+        return step_id
 
-    def _get_managed_step_update(self, step_ids):
+    def _get_managed_step_update(self, step_ids: t.List[str]) -> t.List[StepInfo]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
         :type step_ids: list[str]
         :return: list of updates for managed jobs
         :rtype: list[StepInfo]
         """
-        updates = []
+        updates: t.List[StepInfo] = []
 
-        for step_id in step_ids:
-
-            # Batch jobs have integer step id,
-            # Jsrun processes have {alloc}.{task_id}
-            # Include recently finished jobs
-            if "." in str(step_id):
-                jsrun_step_id = step_id.rpartition(".")[-1]
-                jslist_out, _ = jslist([])
-                stat, return_code = parse_jslist_stepid(jslist_out, jsrun_step_id)
-                info = LSFJsrunStepInfo(stat, return_code)
-            else:
-                bjobs_args = ["-a"] + step_ids
-                bjobs_out, _ = bjobs(bjobs_args)
-                stat = parse_bjobs_jobid(bjobs_out, str(step_id))
-                # create LSFBatchStepInfo objects to return
-                info = LSFBatchStepInfo(stat, None)
-                # account for case where job history is not logged by LSF
-                if info.status == STATUS_COMPLETED:
-                    info.returncode = 0
+        qstat_out, _ = qstat(step_ids)
+        stats = [parse_qstat_jobid(qstat_out, str(step_id)) for step_id in step_ids]
+        # create PBSStepInfo objects to return
+
+        for stat, _ in zip(stats, step_ids):
+            info = PBSStepInfo(stat, None)
+            # account for case where job history is not logged by PBS
+            if info.status == STATUS_COMPLETED:
+                info.returncode = 0
 
             updates.append(info)
         return updates
 
-    def __str__(self):
-        return "LSF"
+    def __str__(self) -> str:
+        return "PBS"
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfParser.py` & `smartsim-0.5.0/smartsim/_core/launcher/lsf/lsfParser.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,32 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
+import typing as t
 
 
-def parse_bsub(output):
+def parse_bsub(output: str) -> str:
     """Parse bsub output and return job id.
 
     :param output: stdout of bsub command
     :type output: str
     :returns: job id
     :rtype: str
     """
     for line in output.split("\n"):
         if line.startswith("Job"):
             return line.split()[1][1:-1]
+    return ""
 
 
-def parse_bsub_error(output):
+def parse_bsub_error(output: str) -> str:
     """Parse and return error output of a failed bsub command.
 
     :param output: stderr of qsub command
     :type output: str
     :returns: error message
     :rtype: str
     """
@@ -67,40 +69,39 @@
         return output
 
     # If output is empty, present standard error
     base_err = "LSF run error"
     return base_err
 
 
-def parse_jslist_stepid(output, step_id):
+def parse_jslist_stepid(output: str, step_id: str) -> t.Tuple[str, t.Optional[str]]:
     """Parse and return output of the jslist command run with
     options to obtain step status
 
     :param output: output of the bjobs command
     :type output: str
-    :param job_id: allocation id or job step id
-    :type job_id: str
+    :param step_id: allocation id or job step id
+    :type step_id: str
     :return: status and return code
     :rtype: (str, str)
     """
-    result = ("NOTFOUND", None)
+    result: t.Tuple[str, t.Optional[str]] = ("NOTFOUND", None)
 
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 7:
             if fields[0] == step_id:
                 stat = fields[6]
                 return_code = fields[5]
                 result = (stat, return_code)
                 break
-
     return result
 
 
-def parse_bjobs_jobid(output, job_id):
+def parse_bjobs_jobid(output: str, job_id: str) -> str:
     """Parse and return output of the bjobs command run with options
     to obtain job status.
 
     :param output: output of the bjobs command
     :type output: str
     :param job_id: allocation id or job step id
     :type job_id: str
@@ -114,15 +115,15 @@
             if fields[0] == job_id:
                 stat = fields[2]
                 result = stat
                 break
     return result
 
 
-def parse_bjobs_nodes(output):
+def parse_bjobs_nodes(output: str) -> t.List[str]:
     """Parse and return the bjobs command run with
     options to obtain node list, i.e. with `-w`.
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     :param output: output of the `bjobs -w` command
@@ -135,15 +136,15 @@
     lines = output.split("\n")
     nodes_str = lines[1].split()[5]
     nodes = nodes_str.split(":")
 
     return list(dict.fromkeys(nodes))
 
 
-def parse_max_step_id_from_jslist(output):
+def parse_max_step_id_from_jslist(output: str) -> t.Optional[str]:
     """Parse and return the maximum step id from a jslist command.
     This function must be called immedietaly after a call to jsrun,
     and before the next one, to ensure the id of the last spawned task is
     properly returned
 
     :param output: output bjobs
     :type output: str
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/pbs/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/pbs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsCommands.py` & `smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsCommands.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,42 +20,44 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from ..util.shell import execute_cmd
 
 
-def qstat(args):
+def qstat(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls PBS qstat with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of qstat
     """
     cmd = ["qstat"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def qsub(args):
+def qsub(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls PBS qsub with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of salloc
     """
     cmd = ["qsub"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def qdel(args):
+def qdel(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls PBS qdel with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
     :type args: list of str
     :return: output and error
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsParser.py` & `smartsim-0.5.0/smartsim/_core/launcher/pbs/pbsParser.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
+import typing as t
 
 
-def parse_qsub(output):
+def parse_qsub(output: str) -> str:
     """Parse qsub output and return job id. For PBS, the
     output is the job id itself.
 
     :param output: stdout of qsub command
     :type output: str
     :returns: job id
     :rtype: str
     """
     return output
 
 
-def parse_qsub_error(output):
+def parse_qsub_error(output: str) -> str:
     """Parse and return error output of a failed qsub command.
 
     :param output: stderr of qsub command
     :type output: str
     :returns: error message
     :rtype: str
     """
@@ -56,15 +57,15 @@
     for line in output.split("\n"):
         return line.strip()
     # if neither, present a base error message
     base_err = "PBS run error"
     return base_err
 
 
-def parse_qstat_jobid(output, job_id):
+def parse_qstat_jobid(output: str, job_id: str) -> str:
     """Parse and return output of the qstat command run with options
     to obtain job status.
 
     :param output: output of the qstat command
     :type output: str
     :param job_id: allocation id or job step id
     :type job_id: str
@@ -78,44 +79,44 @@
             if fields[0] == job_id:
                 stat = fields[4]
                 result = stat
                 break
     return result
 
 
-def parse_qstat_nodes(output):
+def parse_qstat_nodes(output: str) -> t.List[str]:
     """Parse and return the qstat command run with
     options to obtain node list.
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     The `output` parameter must be in JSON format.
 
     :param output: output of the qstat command in JSON format
     :type output: str
     :return: compute nodes of the allocation or job
     :rtype: list of str
     """
-    nodes = []
+    nodes: t.List[str] = []
     out_json = load_and_clean_json(output)
     if "Jobs" not in out_json:
         return nodes
     jobs = out_json["Jobs"]
     job = jobs[list(jobs.keys())[0]]
     vnodes = job["exec_vnode"]
     for vnode in vnodes.split("+"):
         vnode = vnode.strip("()")
         vnode = vnode.split(":")[0]
         nodes.append(vnode)
 
     return list(sorted(set(nodes)))
 
 
-def parse_step_id_from_qstat(output, step_name):
+def parse_step_id_from_qstat(output: str, step_name: str) -> t.Optional[str]:
     """Parse and return the step id from a qstat command
 
     :param output: output qstat
     :type output: str
     :param step_name: the name of the step to query
     :type step_name: str
     :return: the step_id
@@ -131,15 +132,15 @@
         if val["Job_Name"] == step_name:
             step_id = key
             return step_id
 
     return step_id
 
 
-def load_and_clean_json(out):
+def load_and_clean_json(out: str) -> t.Any:
     if len(out.strip()) == 0:
         return ""
     try:
         json_out = json.loads(out)
         return json_out
     except json.decoder.JSONDecodeError as e:
         out_arr = out.split("\n")
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/slurm/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmCommands.py` & `smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmCommands.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,85 +20,87 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from ....error import LauncherError
 from ...utils.helpers import expand_exe_path
 from ..util.shell import execute_cmd
 
 
-def sstat(args):
+def sstat(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls sstat with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of sstat
     """
     _sstat = _find_slurm_command("sstat")
     cmd = [_sstat] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def sacct(args):
+def sacct(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls sacct with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of sacct
     """
     _sacct = _find_slurm_command("sacct")
     cmd = [_sacct] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def salloc(args):
+def salloc(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls slurm salloc with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of salloc
     """
     _salloc = _find_slurm_command("salloc")
     cmd = [_salloc] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def sinfo(args):
+def sinfo(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls slurm sinfo with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of sinfo
     """
     _sinfo = _find_slurm_command("sinfo")
     cmd = [_sinfo] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def scontrol(args):
+def scontrol(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls slurm scontrol with args
 
     :param args: List of command arguments
     :type args: List of str
     :returns: Output and error of sinfo
     """
     _scontrol = _find_slurm_command("scontrol")
     cmd = [_scontrol] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
-def scancel(args):
+def scancel(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls slurm scancel with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
     :type args: list of str
     :return: output and error
@@ -106,15 +108,15 @@
     """
     _scancel = _find_slurm_command("scancel")
     cmd = [_scancel] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
 
 
-def _find_slurm_command(cmd):
+def _find_slurm_command(cmd: str) -> str:
     try:
         full_cmd = expand_exe_path(cmd)
         return full_cmd
     except (TypeError, FileNotFoundError) as e:
         raise LauncherError(
             f"Slurm Launcher could not find path of {cmd} command"
         ) from e
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmLauncher.py` & `smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmLauncher.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,24 +21,34 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
+import typing as t
+
 from shutil import which
 
 from ....error import LauncherError
 from ....log import get_logger
-from ....settings import *
+from ....settings import (
+    MpiexecSettings, 
+    MpirunSettings, 
+    OrterunSettings, 
+    RunSettings, 
+    SbatchSettings, 
+    SettingsBase, 
+    SrunSettings, 
+)
 from ....status import STATUS_CANCELLED
 from ...config import CONFIG
 from ..launcher import WLMLauncher
-from ..step import LocalStep, MpiexecStep, MpirunStep, OrterunStep, SbatchStep, SrunStep
-from ..stepInfo import SlurmStepInfo
+from ..step import LocalStep, MpiexecStep, MpirunStep, OrterunStep, SbatchStep, SrunStep, Step
+from ..stepInfo import SlurmStepInfo, StepInfo
 from .slurmCommands import sacct, scancel, sstat
 from .slurmParser import parse_sacct, parse_sstat_nodes, parse_step_id_from_sacct
 
 logger = get_logger(__name__)
 
 
 class SlurmLauncher(WLMLauncher):
@@ -51,24 +61,27 @@
     and are managed through references to their launching process ID
     i.e. a psutil.Popen object
     """
 
     # init in launcher.py (WLMLauncher)
 
     # RunSettings types supported by this launcher
-    supported_rs = {
-        SrunSettings: SrunStep,
-        SbatchSettings: SbatchStep,
-        MpirunSettings: MpirunStep,
-        MpiexecSettings: MpiexecStep,
-        OrterunSettings: OrterunStep,
-        RunSettings: LocalStep,
-    }
+    @property
+    def supported_rs(self) -> t.Dict[t.Type[SettingsBase], t.Type[Step]]:
+        # RunSettings types supported by this launcher
+        return {
+            SrunSettings: SrunStep,
+            SbatchSettings: SbatchStep,
+            MpirunSettings: MpirunStep,
+            MpiexecSettings: MpiexecStep,
+            OrterunSettings: OrterunStep,
+            RunSettings: LocalStep,
+        }
 
-    def get_step_nodes(self, step_names):
+    def get_step_nodes(self, step_names: t.List[str]) -> t.List[t.List[str]]:
         """Return the compute nodes of a specific job or allocation
 
         This function returns the compute nodes of a specific job or allocation
         in a list with the duplicates removed.
 
         Output gleaned from sstat e.g. the following
 
@@ -81,30 +94,30 @@
         :param step_names: list of job step names
         :type step_names: list[str]
         :raises LauncherError: if nodelist aquisition fails
         :return: list of hostnames
         :rtype: list[str]
         """
         _, step_ids = self.step_mapping.get_ids(step_names, managed=True)
-        step_str = _create_step_id_str(step_ids)
+        step_str = _create_step_id_str([val for val in step_ids if val is not None])
         output, error = sstat([step_str, "-i", "-n", "-p", "-a"])
 
         if "error:" in error.split(" "):
             raise LauncherError("Failed to retrieve nodelist from stat")
 
         # parse node list for each step
         node_lists = []
         for step_id in step_ids:
-            node_lists.append(parse_sstat_nodes(output, step_id))
+            node_lists.append(parse_sstat_nodes(output, step_id or ""))
 
         if len(node_lists) < 1:
             raise LauncherError("Failed to retrieve nodelist from stat")
         return node_lists
 
-    def run(self, step):
+    def run(self, step: Step) -> t.Optional[str]:
         """Run a job step through Slurm
 
         :param step: a job step instance
         :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
         :rtype: str
@@ -133,28 +146,29 @@
                 task_id = self.task_manager.start_task(cmd_list, step.cwd)
             else:
                 # Mpirun doesn't direct output for us like srun does
                 out, err = step.get_output_files()
                 output = open(out, "w+")
                 error = open(err, "w+")
                 task_id = self.task_manager.start_task(
-                    cmd_list, step.cwd, out=output, err=error
+                    cmd_list, step.cwd, out=output.fileno(), err=error.fileno()
                 )
 
         if not step_id and step.managed:
             step_id = self._get_slurm_step_id(step)
+        
         self.step_mapping.add(step.name, step_id, task_id, step.managed)
 
         # give slurm a rest
         # TODO make this configurable
         time.sleep(1)
 
         return step_id
 
-    def stop(self, step_name):
+    def stop(self, step_name: str) -> StepInfo:
         """Step a job step
 
         :param step_name: name of the job to stop
         :type step_name: str
         :return: update for job due to cancel
         :rtype: StepInfo
         """
@@ -166,95 +180,95 @@
             # sub-steps cannot be stopped singularly.
             if "+" in step_id:
                 step_id = step_id.split("+")[0]
             scancel_rc, _, err = scancel([step_id])
             if scancel_rc != 0:
                 logger.warning(f"Unable to cancel job step {step_name}\n {err}")
             if stepmap.task_id:
-                self.task_manager.remove_task(stepmap.task_id)
+                self.task_manager.remove_task(str(stepmap.task_id))
         else:
-            self.task_manager.remove_task(stepmap.task_id)
+            self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
+        if not step_info:
+            raise LauncherError(f"Could not get step_info for job step {step_name}")
+        
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_slurm_step_id(self, step, interval=2):
+    def _get_slurm_step_id(self, step: Step, interval: int = 2) -> str:
         """Get the step_id of a step from sacct
 
         Parses sacct output by looking for the step name
         e.g. the following
 
         SmartSim|119225|
         extern|119225.extern|
         m1-119225.0|119225.0|
         m2-119225.1|119225.1|
         """
         time.sleep(interval)
-        step_id = "unassigned"
+        step_id: t.Optional[str] = None
         trials = CONFIG.wlm_trials
         while trials > 0:
             output, _ = sacct(["--noheader", "-p", "--format=jobname,jobid"])
             step_id = parse_step_id_from_sacct(output, step.name)
             if step_id:
                 break
             else:
                 time.sleep(interval)
                 trials -= 1
         if not step_id:
             raise LauncherError("Could not find id of launched job step")
         return step_id
 
-    def _get_managed_step_update(self, step_ids):
+    def _get_managed_step_update(self, step_ids: t.List[str]) -> t.Optional[t.List[StepInfo]]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
         :type step_ids: list[str]
         :return: list of updates for managed jobs
         :rtype: list[StepInfo]
         """
         step_str = _create_step_id_str(step_ids)
         sacct_out, _ = sacct(["--noheader", "-p", "-b", "--jobs", step_str])
         # (status, returncode)
         stat_tuples = [parse_sacct(sacct_out, step_id) for step_id in step_ids]
 
         # create SlurmStepInfo objects to return
-        updates = []
+        updates: t.List[StepInfo] = []
         for stat_tuple, step_id in zip(stat_tuples, step_ids):
-            info = SlurmStepInfo(stat_tuple[0], stat_tuple[1])
+            _rc = int(stat_tuple[1]) if stat_tuple[1] else None
+            info = SlurmStepInfo(stat_tuple[0], _rc)
 
             task_id = self.step_mapping.get_task_id(step_id)
             if task_id:
                 # we still check the task manager for jobs that didn't ever
                 # become a fully managed job (e.g. error in slurm arguments)
-                _, rc, out, err = self.task_manager.get_task_update(task_id)
+                _, rc, out, err = self.task_manager.get_task_update(str(task_id))
                 if rc and rc != 0:
                     # tack on Popen error and output to status update.
                     info.output = out
                     info.error = err
 
             updates.append(info)
         return updates
 
     @staticmethod
-    def check_for_slurm():
+    def check_for_slurm() -> None:
         """Check if slurm is available
 
         This function checks for slurm commands where the experiment
         is bring run
 
         :raises LauncherError: if no access to slurm
         """
         if not which("sbatch") and not which("sacct"):
             error = "User attempted Slurm methods without access to Slurm at the call site.\n"
             raise LauncherError(error)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "Slurm"
 
 
-def _create_step_id_str(step_ids):
-    step_str = ""
-    for step_id in step_ids:
-        step_str += str(step_id) + ","
-    step_str = step_str.strip(",")
-    return step_str
+def _create_step_id_str(step_ids: t.List[str]) -> str:
+    return ",".join(step_ids)
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmParser.py` & `smartsim-0.5.0/smartsim/_core/launcher/slurm/slurmParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,28 +20,30 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 from shutil import which
 
 """
 Parsers for various slurm functions.
 """
 
 
-def parse_salloc(output):
+def parse_salloc(output: str) -> t.Optional[str]:
     for line in output.split("\n"):
         if line.startswith("salloc: Granted job allocation"):
             return line.split()[-1]
+    return None
 
 
-def parse_salloc_error(output):
+def parse_salloc_error(output: str) -> t.Optional[str]:
     """Parse and return error output of a failed salloc command
 
     :param output: stderr output of salloc command
     :type output: str
     :return: error message
     :rtype: str
     """
@@ -62,15 +64,15 @@
         if line.startswith("salloc: "):
             error = " ".join((line.split()[1:]))
             return error.strip()
     # return None if we cant find error
     return None
 
 
-def jobid_exact_match(parsed_id, job_id):
+def jobid_exact_match(parsed_id: str, job_id: str) -> bool:
     """Check that job_id is an exact match and not
     the prefix of another job_id, like 1 and 11
     or 1.1 and 1.10. Works with job id or step
     id (i.e. with or without a '.' in the id)
     :param parsed_id: the id read from the line
     :type paserd_id: str
     :param job_id: the id to check for equality
@@ -78,37 +80,37 @@
     """
     if "." in job_id:
         return parsed_id == job_id
     else:
         return parsed_id.split(".")[0] == job_id
 
 
-def parse_sacct(output, job_id):
+def parse_sacct(output: str, job_id: str) -> t.Tuple[str, t.Optional[str]]:
     """Parse and return output of the sacct command
 
     :param output: output of the sacct command
     :type output: str
     :param job_id: allocation id or job step id
     :type job_id: str
     :return: status and returncode
     :rtype: tuple
     """
-    result = ("PENDING", None)
+    result: t.Tuple[str, t.Optional[str]] = ("PENDING", None)
     for line in output.split("\n"):
-        line = line.split("|")
-        if len(line) >= 3:
-            if jobid_exact_match(line[0], job_id):
-                stat = line[1]
-                code = line[2].split(":")[0]
-                result = (stat, code)
+        parts = line.split("|")
+        if len(parts) >= 3:
+            if jobid_exact_match(parts[0], job_id):
+                stat = parts[1]
+                return_code = parts[2].split(":")[0]
+                result = (stat, return_code)
                 break
     return result
 
 
-def parse_sstat_nodes(output, job_id):
+def parse_sstat_nodes(output: str, job_id: str) -> t.List[str]:
     """Parse and return the sstat command
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     :param output: output of the sstat command
     :type output: str
@@ -123,15 +125,15 @@
         if len(sstat_string) >= 2:
             if jobid_exact_match(sstat_string[0], job_id):
                 node = sstat_string[1]
                 nodes.append(node)
     return list(set(nodes))
 
 
-def parse_step_id_from_sacct(output, step_name):
+def parse_step_id_from_sacct(output: str, step_name: str) -> t.Optional[str]:
     """Parse and return the step id from a sacct command
 
     :param output: output of sacct --noheader -p
                    --format=jobname,jobid --job <alloc>
     :type output: str
     :param step_name: the name of the step to query
     :type step_name: str
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from .step import Step
 from .alpsStep import AprunStep
 from .cobaltStep import CobaltBatchStep
 from .localStep import LocalStep
 from .lsfStep import BsubBatchStep, JsrunStep
 from .mpiStep import MpiexecStep, MpirunStep, OrterunStep
 from .pbsStep import QsubBatchStep
 from .slurmStep import SbatchStep, SrunStep
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/alpsStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/alpsStep.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,41 +22,46 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import shutil
+import typing as t
 from shlex import split as sh_split
 
 from ....error import AllocationError
 from ....log import get_logger
 from .step import Step
+from ....settings import AprunSettings
 
 logger = get_logger(__name__)
 
 
 class AprunStep(Step):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: AprunSettings) -> None:
         """Initialize a ALPS aprun job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
+        :type run_settings: AprunSettings
         """
-        super().__init__(name, cwd)
-        self.run_settings = run_settings
+        super().__init__(name, cwd, run_settings)
         self.alloc = None
         if not self.run_settings.in_batch:
             self._set_alloc()
 
-    def get_launch_cmd(self):
+    @property
+    def run_settings(self) -> AprunSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
         :rtype: list[str]
         """
         aprun = self.run_settings.run_command
         aprun_cmd = [aprun, "--wdir", self.cwd]
@@ -83,15 +88,15 @@
         # if its in a batch, redirect stdout to
         # file in the cwd.
         if self.run_settings.in_batch:
             output = self.get_step_file(ending=".out")
             aprun_cmd.extend([">", output])
         return aprun_cmd
 
-    def _set_alloc(self):
+    def _set_alloc(self) -> None:
         """Set the id of the allocation
 
         :raises AllocationError: allocation not listed or found
         """
         if "PBS_JOBID" in os.environ:
             self.alloc = os.environ["PBS_JOBID"]
             logger.debug(
@@ -103,28 +108,28 @@
                 f"Running on Cobalt allocation {self.alloc} gleaned from user environment"
             )
         else:
             raise AllocationError(
                 "No allocation specified or found and not running in batch"
             )
 
-    def _build_exe(self):
+    def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
         :rtype: list[str]
         """
         if self.run_settings.mpmd:
             return self._make_mpmd()
         else:
             exe = self.run_settings.exe
             args = self.run_settings.exe_args
             return exe + args
 
-    def _make_mpmd(self):
+    def _make_mpmd(self) -> t.List[str]:
         """Build Aprun (MPMD) executable"""
 
         exe = self.run_settings.exe
         exe_args = self.run_settings.exe_args
         cmd = exe + exe_args
 
         for mpmd in self.run_settings.mpmd:
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/cobaltStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/cobaltStep.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,57 +22,62 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import stat
+import typing as t
 
 from ....log import get_logger
+from ....settings import CobaltBatchSettings
 from .step import Step
 
 logger = get_logger(__name__)
 
 
 class CobaltBatchStep(Step):
-    def __init__(self, name, cwd, batch_settings):
+    def __init__(self, name: str, cwd: str, batch_settings: CobaltBatchSettings) -> None:
         """Initialize a Cobalt qsub step
 
         :param name: name of the entity to launch
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: BatchSettings
+        :type batch_settings: CobaltBatchSettings
         """
-        super().__init__(name, cwd)
-        self.batch_settings = batch_settings
-        self.step_cmds = []
+        super().__init__(name, cwd, batch_settings)
+        self.step_cmds: t.List[t.List[str]] = []
         self.managed = True
 
-    def get_launch_cmd(self):
+    @property
+    def batch_settings(self) -> CobaltBatchSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
         :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, script]
 
-    def add_to_batch(self, step):
+    def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
         :type step: Step
         """
         launch_cmd = step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
-    def _write_script(self):
+    def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
         :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         cobalt_debug = self.get_step_file(ending=".cobalt-debug")
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/localStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/localStep.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,49 +22,55 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import shutil
+import typing as t
 
 from .step import Step
+from ....settings.base import RunSettings
 
 
 class LocalStep(Step):
-    def __init__(self, name, cwd, run_settings):
-        super().__init__(name, cwd)
-        self.run_settings = run_settings
+    def __init__(self, name: str, cwd: str, run_settings: RunSettings):
+        super().__init__(name, cwd, run_settings)
         self.env = self._set_env()
 
-    def get_launch_cmd(self):
+    @property
+    def run_settings(self) -> RunSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         cmd = []
 
         # Add run command and args if user specified
         # default is no run command for local job steps
         if self.run_settings.run_command:
             cmd.append(self.run_settings.run_command)
             run_args = self.run_settings.format_run_args()
             cmd.extend(run_args)
 
         if self.run_settings.colocated_db_settings:
             # Replace the command with the entrypoint wrapper script
-            bash = shutil.which("bash")
+            if not (bash := shutil.which("bash")):
+                raise RuntimeError("Unable to locate bash interpreter")
 
             launch_script_path = self.get_colocated_launch_script()
             cmd.extend([bash, launch_script_path])
 
         if self.run_settings.container:
             cmd += self.run_settings.container._container_cmds(self.cwd)
 
         # build executable
         cmd.extend(self.run_settings.exe)
         if self.run_settings.exe_args:
             cmd.extend(self.run_settings.exe_args)
         return cmd
 
-    def _set_env(self):
+    def _set_env(self) -> t.Dict[str, str]:
         env = os.environ.copy()
         if self.run_settings.env_vars:
             for k, v in self.run_settings.env_vars.items():
                 env[k] = v
         return env
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/lsfStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/lsfStep.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,58 +22,64 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import shutil
+import typing as t
 
 from ....error import AllocationError
 from ....log import get_logger
 from .step import Step
+from ....settings import BsubBatchSettings
+from ....settings.base import RunSettings
 
 logger = get_logger(__name__)
 
 
 class BsubBatchStep(Step):
-    def __init__(self, name, cwd, batch_settings):
+    def __init__(self, name: str, cwd: str, batch_settings: BsubBatchSettings) -> None:
         """Initialize a LSF bsub step
 
         :param name: name of the entity to launch
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: BatchSettings
+        :type batch_settings: BsubBatchSettings
         """
-        super().__init__(name, cwd)
-        self.batch_settings = batch_settings
+        super().__init__(name, cwd, batch_settings)
         self.step_cmds = []
         self.managed = True
 
-    def get_launch_cmd(self):
+    @property
+    def batch_settings(self) -> BsubBatchSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
         :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, script]
 
-    def add_to_batch(self, step):
+    def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
         :type step: Step
         """
         launch_cmd = step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
-    def _write_script(self):
+    def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
         :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
@@ -102,32 +108,35 @@
                 if i == len(self.step_cmds) - 1:
                     f.write("\n")
                     f.write("wait\n")
         return batch_script
 
 
 class JsrunStep(Step):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: RunSettings):
         """Initialize a LSF jsrun job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
         :type run_settings: RunSettings
         """
-        super().__init__(name, cwd)
-        self.run_settings = run_settings
+        super().__init__(name, cwd, run_settings)
         self.alloc = None
         self.managed = True
         if not self.run_settings.in_batch:
             self._set_alloc()
 
-    def get_output_files(self):
+    @property
+    def run_settings(self) -> RunSettings:
+        return self.step_settings
+
+    def get_output_files(self) -> t.Tuple[str, str]:
         """Return two paths to error and output files based on cwd"""
         output = self.get_step_file(ending=".out")
         error = self.get_step_file(ending=".err")
 
         # The individual_suffix (containing %t and similar placeholders) is
         # appended to the output (and error) file name, but just before the ending.
         # So if the collective output file name would be "entity_name.out", adding
@@ -143,15 +152,15 @@
             partitioned_error = error.rpartition(".")
             error_prefix = partitioned_error[0] + self.run_settings.individual_suffix
             error_suffix = partitioned_error[-1]
             error = ".".join([error_prefix, error_suffix])
 
         return output, error
 
-    def get_launch_cmd(self):
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
         :rtype: list[str]
         """
         jsrun = self.run_settings.run_command
 
@@ -183,47 +192,47 @@
             launch_script_path = self.get_colocated_launch_script()
             jsrun_cmd.extend([bash, launch_script_path])
 
         jsrun_cmd.extend(self._build_exe())
 
         return jsrun_cmd
 
-    def _set_alloc(self):
+    def _set_alloc(self) -> None:
         """Set the id of the allocation
 
         :raises AllocationError: allocation not listed or found
         """
         if "LSB_JOBID" in os.environ:
             self.alloc = os.environ["LSB_JOBID"]
             logger.debug(
                 f"Running on LSF allocation {self.alloc} gleaned from user environment"
             )
         else:
             raise AllocationError(
                 "No allocation specified or found and not running in batch"
             )
 
-    def _build_exe(self):
+    def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
         :rtype: list[str]
         """
         exe = self.run_settings.exe
         args = self.run_settings.exe_args
         if self.run_settings.mpmd:
             erf_file = self.get_step_file(ending=".mpmd")
-            cmd = self._make_mpmd()
+            _ = self._make_mpmd()
             mp_cmd = ["--erf_input", erf_file]
             return mp_cmd
         else:
             cmd = exe + args
             return cmd
 
-    def _make_mpmd(self):
+    def _make_mpmd(self) -> None:
         """Build LSF's Explicit Resource File"""
         erf_file = self.get_step_file(ending=".mpmd")
 
         # Find launch_distribution command
         preamble_lines = self.run_settings.mpmd_preamble_lines.copy()
         distr_line = None
         for line in self.run_settings.mpmd_preamble_lines:
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/mpiStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/mpiStep.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,49 +23,54 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import shutil
 from shlex import split as sh_split
+import typing as t
 
 from ....error import AllocationError
 from ....log import get_logger
 from .step import Step
+from ....settings import MpirunSettings, MpiexecSettings, OrterunSettings
+from ....settings.base import RunSettings
 
 logger = get_logger(__name__)
 
 
 class _BaseMPIStep(Step):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: RunSettings) -> None:
         """Initialize a job step conforming to the MPI standard
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
         :type run_settings: RunSettings
         """
 
-        super().__init__(name, cwd)
-
-        self.run_settings = run_settings
+        super().__init__(name, cwd, run_settings)
 
         self.alloc = None
         if not self.run_settings.in_batch:
             self._set_alloc()
 
+    @property
+    def run_settings(self) -> RunSettings:
+        return self.step_settings
+
     _supported_launchers = ["PBS", "COBALT", "SLURM", "LSB"]
 
     @property
-    def _run_command(self):
+    def _run_command(self) -> str:
         return self.run_settings._run_command
 
-    def get_launch_cmd(self):
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
         :rtype: list[str]
         """
         mpi_cmd = [self._run_command, "--wdir", self.cwd]
         # add env vars to mpi command
@@ -89,15 +94,15 @@
         # if its in a batch, redirect stdout to
         # file in the cwd.
         if self.run_settings.in_batch:
             output = self.get_step_file(ending=".out")
             mpi_cmd += [">", output]
         return mpi_cmd
 
-    def _set_alloc(self):
+    def _set_alloc(self) -> None:
         """Set the id of the allocation
 
         :raises AllocationError: allocation not listed or found
         """
 
         environment_keys = os.environ.keys()
         for launcher in self._supported_launchers:
@@ -108,28 +113,28 @@
                 return
 
         # If this function did not return above, no allocations were found
         raise AllocationError(
             "No allocation specified or found and not running in batch"
         )
 
-    def _build_exe(self):
+    def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
         :rtype: list[str]
         """
         if self.run_settings.mpmd:
             return self._make_mpmd()
         else:
             exe = self.run_settings.exe
             args = self.run_settings.exe_args
             return exe + args
 
-    def _make_mpmd(self):
+    def _make_mpmd(self) -> t.List[str]:
         """Build mpiexec (MPMD) executable"""
         exe = self.run_settings.exe
         args = self.run_settings.exe_args
         cmd = exe + args
         for mpmd in self.run_settings.mpmd:
             cmd += [" : "]
             cmd += mpmd.format_run_args()
@@ -138,58 +143,58 @@
             cmd += mpmd.exe_args
 
         cmd = sh_split(" ".join(cmd))
         return cmd
 
 
 class MpiexecStep(_BaseMPIStep):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: MpiexecSettings) -> None:
         """Initialize an mpiexec job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
+        :type run_settings: MpiexecSettings
         :param default_run_command: The default command to launch an MPI
                                     application
         :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
 
 
 class MpirunStep(_BaseMPIStep):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: MpirunSettings) -> None:
         """Initialize an mpirun job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
+        :type run_settings: MpirunSettings
         :param default_run_command: The default command to launch an MPI
                                     application
         :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
 
 
 class OrterunStep(_BaseMPIStep):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: OrterunSettings) -> None:
         """Initialize an orterun job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
+        :type run_settings: OrterunSettings
         :param default_run_command: The default command to launch an MPI
                                     application
         :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/pbsStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/pbsStep.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,56 +20,63 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from ....log import get_logger
 from .step import Step
+from ....settings import QsubBatchSettings
+from ....settings.base import BatchSettings
 
 logger = get_logger(__name__)
 
 
 class QsubBatchStep(Step):
-    def __init__(self, name, cwd, batch_settings):
+    def __init__(self, name: str, cwd: str, batch_settings: QsubBatchSettings) -> None:
         """Initialize a PBSpro qsub step
 
         :param name: name of the entity to launch
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: BatchSettings
+        :type batch_settings: QsubBatchSettings
         """
-        super().__init__(name, cwd)
-        self.batch_settings = batch_settings
-        self.step_cmds = []
+        super().__init__(name, cwd, batch_settings)
+        self.step_cmds: t.List[t.List[str]] = []
         self.managed = True
 
-    def get_launch_cmd(self):
+    @property
+    def batch_settings(self) -> QsubBatchSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
         :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, script]
 
-    def add_to_batch(self, step):
+    def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
         :type step: Step
         """
         launch_cmd = step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
-    def _write_script(self):
+    def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
         :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/slurmStep.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/slurmStep.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,59 +23,64 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import shutil
 from shlex import split as sh_split
+import typing as t
 
 from ....error import AllocationError
 from ....log import get_logger
 from .step import Step
+from ....settings import SrunSettings, SbatchSettings
 
 logger = get_logger(__name__)
 
 
 class SbatchStep(Step):
-    def __init__(self, name, cwd, batch_settings):
+    def __init__(self, name: str, cwd: str, batch_settings: SbatchSettings) -> None:
         """Initialize a Slurm Sbatch step
 
         :param name: name of the entity to launch
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: BatchSettings
+        :type batch_settings: SbatchSettings
         """
-        super().__init__(name, cwd)
-        self.batch_settings = batch_settings
+        super().__init__(name, cwd, batch_settings)
         self.step_cmds = []
         self.managed = True
 
-    def get_launch_cmd(self):
+    @property
+    def batch_settings(self) -> SbatchSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
         :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, "--parsable", script]
 
-    def add_to_batch(self, step):
+    def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
         :type step: Step
         """
         launch_cmd = ["cd", step.cwd, ";"]
         launch_cmd += step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
-    def _write_script(self):
+    def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
         :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
@@ -98,42 +103,45 @@
                 if i == len(self.step_cmds) - 1:
                     f.write("\n")
                     f.write("wait\n")
         return batch_script
 
 
 class SrunStep(Step):
-    def __init__(self, name, cwd, run_settings):
+    def __init__(self, name: str, cwd: str, run_settings: SrunSettings) -> None:
         """Initialize a srun job step
 
         :param name: name of the entity to be launched
         :type name: str
         :param cwd: path to launch dir
         :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
+        :type run_settings: SrunSettings
         """
-        super().__init__(name, cwd)
-        self.run_settings = run_settings
+        super().__init__(name, cwd, run_settings)
         self.alloc = None
         self.managed = True
         if not self.run_settings.in_batch:
             self._set_alloc()
 
-    def get_launch_cmd(self):
+    @property
+    def run_settings(self) -> SrunSettings:
+        return self.step_settings
+
+    def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
         :rtype: list[str]
         """
         srun = self.run_settings.run_command
         output, error = self.get_output_files()
 
         srun_cmd = [srun, "--output", output, "--error", error, "--job-name", self.name]
-        compound_env = set()
+        compound_env: t.Set[str] = set()
 
         if self.alloc:
             srun_cmd += ["--jobid", str(self.alloc)]
 
         if self.run_settings.env_vars:
             (
                 env_var_str,
@@ -145,18 +153,15 @@
 
             if comma_separated_env_vars:
                 compound_env = compound_env.union(comma_separated_env_vars)
 
         srun_cmd += self.run_settings.format_run_args()
 
         if self.run_settings.colocated_db_settings:
-            # disable cpu binding as the entrypoint will set that
-            # for the application and database process now
-            srun_cmd.append("--cpu-bind=none")
-
+            
             # Replace the command with the entrypoint wrapper script
             bash = shutil.which("bash")
             launch_script_path = self.get_colocated_launch_script()
             srun_cmd += [bash, launch_script_path]
 
         if self.run_settings.container:
             srun_cmd += self.run_settings.container._container_cmds(self.cwd)
@@ -164,15 +169,15 @@
         if compound_env:
             srun_cmd = ["env"] + list(compound_env) + srun_cmd
 
         srun_cmd += self._build_exe()
 
         return srun_cmd
 
-    def _set_alloc(self):
+    def _set_alloc(self) -> None:
         """Set the id of the allocation
 
         :raises AllocationError: allocation not listed or found
         """
         if self.run_settings.alloc:
             self.alloc = str(self.run_settings.alloc)
         else:
@@ -182,28 +187,28 @@
                     f"Running on allocation {self.alloc} gleaned from user environment"
                 )
             else:
                 raise AllocationError(
                     "No allocation specified or found and not running in batch"
                 )
 
-    def _build_exe(self):
+    def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
         :rtype: list[str]
         """
         if self.run_settings.mpmd:
             return self._make_mpmd()
         else:
             exe = self.run_settings.exe
             args = self.run_settings.exe_args
             return exe + args
 
-    def _make_mpmd(self):
+    def _make_mpmd(self) -> t.List[str]:
         """Build Slurm multi-prog (MPMD) executable"""
         exe = self.run_settings.exe
         args = self.run_settings.exe_args
         cmd = exe + args
 
         compound_env_vars = []
         for mpmd in self.run_settings.mpmd:
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/step/step.py` & `smartsim-0.5.0/smartsim/_core/launcher/step/step.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,73 +20,77 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
 import os.path as osp
+import sys
 import time
+import typing as t
 
 from ....log import get_logger
 from ...utils.helpers import get_base_36_repr
 from ..colocated import write_colocated_launch_script
+from ....settings.base import SettingsBase
 
 logger = get_logger(__name__)
 
 
 class Step:
-    def __init__(self, name, cwd):
+    def __init__(self, name: str, cwd: str, step_settings: SettingsBase) -> None:
         self.name = self._create_unique_name(name)
         self.entity_name = name
         self.cwd = cwd
         self.managed = False
+        self.step_settings = step_settings
 
-    def get_launch_cmd(self):
+    def get_launch_cmd(self) -> t.List[str]:
         raise NotImplementedError
 
-    def _create_unique_name(self, entity_name):
+    def _create_unique_name(self, entity_name: str) -> str:
         step_name = entity_name + "-" + get_base_36_repr(time.time_ns())
         return step_name
 
-    def get_output_files(self):
+    def get_output_files(self) -> t.Tuple[str, str]:
         """Return two paths to error and output files based on cwd"""
         output = self.get_step_file(ending=".out")
         error = self.get_step_file(ending=".err")
         return output, error
 
-    def get_step_file(self, ending=".sh", script_name=None):
+    def get_step_file(self, ending: str = ".sh", script_name: t.Optional[str] = None) -> str:
         """Get the name for a file/script created by the step class
 
         Used for Batch scripts, mpmd scripts, etc"""
         if script_name:
             script_name = script_name if "." in script_name else script_name + ending
             return osp.join(self.cwd, script_name)
         return osp.join(self.cwd, self.entity_name + ending)
 
-    def get_colocated_launch_script(self):
+    def get_colocated_launch_script(self) -> str:
         # prep step for colocated launch if specifed in run settings
         script_path = self.get_step_file(script_name=".colocated_launcher.sh")
 
         db_settings = self.run_settings.colocated_db_settings
 
         # db log file causes write contention and kills performance so by
         # default we turn off logging unless user specified debug=True
         if db_settings.get("debug", False):
             db_log_file = self.get_step_file(ending="-db.log")
         else:
             db_log_file = "/dev/null"
 
-        # if user specified to use taskset with local launcher
-        # (not allowed b/c MacOS doesn't support it)
-        # TODO: support this only on linux
-        if (
-            self.__class__.__name__ == "LocalStep"
-            and db_settings["limit_app_cpus"] is True
-        ):  # pragma: no cover
-            logger.warning("Setting limit_app_cpus=False for local launcher")
-            db_settings["limit_app_cpus"] = False
-
         # write the colocated wrapper shell script to the directory for this
         # entity currently being prepped to launch
         write_colocated_launch_script(script_path, db_log_file, db_settings)
         return script_path
+
+    def add_to_batch(self, step: Step) -> None:
+        """Add a job step to this batch
+
+        :param step: a job step instance e.g. SrunStep
+        :type step: Step
+        """
+        raise NotImplementedError
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/stepInfo.py` & `smartsim-0.5.0/smartsim/_core/launcher/stepInfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,75 +21,97 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import psutil
+import typing as t
 
 from ...status import (
     SMARTSIM_STATUS,
     STATUS_CANCELLED,
     STATUS_COMPLETED,
     STATUS_FAILED,
     STATUS_PAUSED,
     STATUS_RUNNING,
 )
 
 
 class StepInfo:
     def __init__(
-        self, status="", launcher_status="", returncode=None, output=None, error=None
-    ):
+        self,
+        status: str = "",
+        launcher_status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         self.status = status
         self.launcher_status = launcher_status
         self.returncode = returncode
         self.output = output
         self.error = error
 
-    def __str__(self):
+    def __str__(self) -> str:
         info_str = f"Status: {self.status}"
         info_str += f" | Launcher Status {self.launcher_status}"
         info_str += f" | Returncode {str(self.returncode)}"
         return info_str
+    
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        raise NotImplementedError
+    
+    def _get_smartsim_status(self, status: str, returncode: t.Optional[int] = None) -> str:
+        """
+        Map the status of the WLM step to a smartsim-specific status
+        """
+        if status in SMARTSIM_STATUS:
+            return SMARTSIM_STATUS[status]
+        elif status in self.mapping:
+            if returncode is not None and returncode != 0:
+                return STATUS_FAILED
+            else:
+                return self.mapping[status]
+        return STATUS_FAILED
 
 
 class UnmanagedStepInfo(StepInfo):
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        # see https://github.com/giampaolo/psutil/blob/master/psutil/_pslinux.py
+        # see https://github.com/giampaolo/psutil/blob/master/psutil/_common.py
+        return {
+            psutil.STATUS_RUNNING: STATUS_RUNNING,
+            psutil.STATUS_SLEEPING: STATUS_RUNNING,  # sleeping thread is still alive
+            psutil.STATUS_WAKING: STATUS_RUNNING,
+            psutil.STATUS_DISK_SLEEP: STATUS_RUNNING,
+            psutil.STATUS_DEAD: STATUS_FAILED,
+            psutil.STATUS_TRACING_STOP: STATUS_PAUSED,
+            psutil.STATUS_WAITING: STATUS_PAUSED,
+            psutil.STATUS_STOPPED: STATUS_PAUSED,
+            psutil.STATUS_LOCKED: STATUS_PAUSED,
+            psutil.STATUS_PARKED: STATUS_PAUSED,
+            psutil.STATUS_IDLE: STATUS_PAUSED,
+            psutil.STATUS_ZOMBIE: STATUS_COMPLETED,
+        }
 
-    # see https://github.com/giampaolo/psutil/blob/master/psutil/_pslinux.py
-    # see https://github.com/giampaolo/psutil/blob/master/psutil/_common.py
-    mapping = {
-        psutil.STATUS_RUNNING: STATUS_RUNNING,
-        psutil.STATUS_SLEEPING: STATUS_RUNNING,  # sleeping thread is still alive
-        psutil.STATUS_WAKING: STATUS_RUNNING,
-        psutil.STATUS_DISK_SLEEP: STATUS_RUNNING,
-        psutil.STATUS_DEAD: STATUS_FAILED,
-        psutil.STATUS_TRACING_STOP: STATUS_PAUSED,
-        psutil.STATUS_WAITING: STATUS_PAUSED,
-        psutil.STATUS_STOPPED: STATUS_PAUSED,
-        psutil.STATUS_LOCKED: STATUS_PAUSED,
-        psutil.STATUS_PARKED: STATUS_PAUSED,
-        psutil.STATUS_IDLE: STATUS_PAUSED,
-        psutil.STATUS_ZOMBIE: STATUS_COMPLETED,
-    }
-
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         smartsim_status = self._get_smartsim_status(status)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
 
-    def _get_smartsim_status(self, status):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        if status in self.mapping:
-            return self.mapping[status]
-        # we don't know what happened so return failed to be safe
-        return STATUS_FAILED
-
 
 class SlurmStepInfo(StepInfo):  # cov-slurm
 
     # see https://slurm.schedmd.com/squeue.html#lbAG
     mapping = {
         "RUNNING": STATUS_RUNNING,
         "CONFIGURING": STATUS_RUNNING,
@@ -113,163 +135,159 @@
         "RESIZING": STATUS_PAUSED,
         "SIGNALING": STATUS_PAUSED,
         "SPECIAL_EXIT": STATUS_PAUSED,
         "STOPPED": STATUS_PAUSED,
         "SUSPENDED": STATUS_PAUSED,
     }
 
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         smartsim_status = self._get_smartsim_status(status)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
 
-    def _get_smartsim_status(self, status):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        if status in self.mapping:
-            return self.mapping[status]
-        # we don't know what happened so return failed to be safe
-        return STATUS_FAILED
-
 
 class PBSStepInfo(StepInfo):  # cov-pbs
 
-    # see http://nusc.nsu.ru/wiki/lib/exe/fetch.php/doc/pbs/PBSReferenceGuide19.2.1.pdf#M11.9.90788.PBSHeading1.81.Job.States
-    mapping = {
-        "R": STATUS_RUNNING,
-        "B": STATUS_RUNNING,
-        "H": STATUS_PAUSED,
-        "M": STATUS_PAUSED,  # Actually means that it was moved to another server, TODO: understand what this implies
-        "Q": STATUS_PAUSED,
-        "S": STATUS_PAUSED,
-        "T": STATUS_PAUSED,  # This means in transition, see above for comment
-        "U": STATUS_PAUSED,
-        "W": STATUS_PAUSED,
-        "E": STATUS_COMPLETED,
-        "F": STATUS_COMPLETED,
-        "X": STATUS_COMPLETED,
-    }
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        # see http://nusc.nsu.ru/wiki/lib/exe/fetch.php/doc/pbs/PBSReferenceGuide19.2.1.pdf#M11.9.90788.PBSHeading1.81.Job.States
+        return {
+            "R": STATUS_RUNNING,
+            "B": STATUS_RUNNING,
+            "H": STATUS_PAUSED,
+            "M": STATUS_PAUSED,  # Actually means that it was moved to another server, TODO: understand what this implies
+            "Q": STATUS_PAUSED,
+            "S": STATUS_PAUSED,
+            "T": STATUS_PAUSED,  # This means in transition, see above for comment
+            "U": STATUS_PAUSED,
+            "W": STATUS_PAUSED,
+            "E": STATUS_COMPLETED,
+            "F": STATUS_COMPLETED,
+            "X": STATUS_COMPLETED,
+        }
 
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         if status == "NOTFOUND":
             if returncode is not None:
                 smartsim_status = "Completed" if returncode == 0 else "Failed"
             else:
                 # if PBS job history isnt available, and job isnt in queue
                 smartsim_status = "Completed"
                 returncode = 0
         else:
             smartsim_status = self._get_smartsim_status(status)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
 
-    def _get_smartsim_status(self, status):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        elif status in self.mapping:
-            return self.mapping[status]
-        return STATUS_FAILED
-
 
 class CobaltStepInfo(StepInfo):  # cov-cobalt
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        return {
+            "running": STATUS_RUNNING,
+            "queued": STATUS_PAUSED,
+            "starting": STATUS_PAUSED,
+            "dep_hold": STATUS_PAUSED,
+            "user_hold": STATUS_PAUSED,
+            "admin_hold": STATUS_PAUSED,
+            "dep_fail": STATUS_FAILED,  # unsure of this one
+            "terminating": STATUS_COMPLETED,
+            "killing": STATUS_COMPLETED,
+            "exiting": STATUS_COMPLETED,
+        }
 
-    mapping = {
-        "running": STATUS_RUNNING,
-        "queued": STATUS_PAUSED,
-        "starting": STATUS_PAUSED,
-        "dep_hold": STATUS_PAUSED,
-        "user_hold": STATUS_PAUSED,
-        "admin_hold": STATUS_PAUSED,
-        "dep_fail": STATUS_FAILED,  # unsure of this one
-        "terminating": STATUS_COMPLETED,
-        "killing": STATUS_COMPLETED,
-        "exiting": STATUS_COMPLETED,
-    }
-
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         if status == "NOTFOUND":
             # returncode not logged by Cobalt
             # if job has exited the queue then we consider it "completed"
             # this should only be hit in the case when job exits abnormally fast
             smartsim_status = "Completed"
             returncode = 0
         else:
             smartsim_status = self._get_smartsim_status(status)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
 
-    def _get_smartsim_status(self, status):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        elif status in self.mapping:
-            return self.mapping[status]
-        return STATUS_FAILED
-
 
 class LSFBatchStepInfo(StepInfo):  # cov-lsf
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        # see https://www.ibm.com/docs/en/spectrum-lsf/10.1.0?topic=execution-about-job-states
+        return {
+            "RUN": STATUS_RUNNING,
+            "PSUSP": STATUS_PAUSED,
+            "USUSP": STATUS_PAUSED,
+            "SSUSP": STATUS_PAUSED,
+            "PEND": STATUS_PAUSED,
+            "DONE": STATUS_COMPLETED,
+        }
 
-    # see https://www.ibm.com/docs/en/spectrum-lsf/10.1.0?topic=execution-about-job-states
-    mapping = {
-        "RUN": STATUS_RUNNING,
-        "PSUSP": STATUS_PAUSED,
-        "USUSP": STATUS_PAUSED,
-        "SSUSP": STATUS_PAUSED,
-        "PEND": STATUS_PAUSED,
-        "DONE": STATUS_COMPLETED,
-    }
-
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         if status == "NOTFOUND":
             if returncode is not None:
                 smartsim_status = "Completed" if returncode == 0 else "Failed"
             else:
                 smartsim_status = "Completed"
                 returncode = 0
         else:
-            smartsim_status = self._get_smartsim_status(status, returncode)
+            smartsim_status = self._get_smartsim_status(status)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
 
-    def _get_smartsim_status(self, status, returncode):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        elif status in self.mapping:
-            return self.mapping[status]
-        return STATUS_FAILED
-
 
 class LSFJsrunStepInfo(StepInfo):  # cov-lsf
+    @property
+    def mapping(self) -> t.Dict[str, str]:
+        # see https://www.ibm.com/docs/en/spectrum-lsf/10.1.0?topic=execution-about-job-states
+        return {
+            "Killed": STATUS_COMPLETED,
+            "Running": STATUS_RUNNING,
+            "Queued": STATUS_PAUSED,
+            "Complete": STATUS_COMPLETED,
+        }
 
-    # see https://www.ibm.com/docs/en/spectrum-lsf/10.1.0?topic=execution-about-job-states
-    mapping = {
-        "Killed": STATUS_COMPLETED,
-        "Running": STATUS_RUNNING,
-        "Queued": STATUS_PAUSED,
-        "Complete": STATUS_COMPLETED,
-    }
-
-    def __init__(self, status="", returncode=None, output=None, error=None):
+    def __init__(
+        self,
+        status: str = "",
+        returncode: t.Optional[int] = None,
+        output: t.Optional[str] = None,
+        error: t.Optional[str] = None,
+    ) -> None:
         if status == "NOTFOUND":
             if returncode is not None:
                 smartsim_status = "Completed" if returncode == 0 else "Failed"
             else:
                 smartsim_status = "Completed"
                 returncode = 0
         else:
             smartsim_status = self._get_smartsim_status(status, returncode)
         super().__init__(
             smartsim_status, status, returncode, output=output, error=error
         )
-
-    def _get_smartsim_status(self, status, returncode):
-        if status in SMARTSIM_STATUS:
-            return SMARTSIM_STATUS[status]
-        elif status in self.mapping:
-            if returncode is not None and int(returncode) != 0:
-                return STATUS_FAILED
-            else:
-                return self.mapping[status]
-        return STATUS_FAILED
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/taskManager.py` & `smartsim-0.5.0/smartsim/_core/launcher/taskManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
+import psutil
 import time
+import typing as t
+
 from subprocess import PIPE
 from threading import RLock, Thread
 
-import psutil
-
 from ...error import LauncherError
 from ...log import get_logger
 from ..utils.helpers import check_dev_log_level
 from .util.shell import execute_async_cmd, execute_cmd
 
 logger = get_logger(__name__)
 verbose_tm = check_dev_log_level()
@@ -53,31 +56,31 @@
 
     When a launcher uses the task manager to start a task, the task
     is either managed (by a WLM) or unmanaged (meaning not managed by
     a WLM). In the latter case, the Task manager is responsible for the
     lifecycle of the process.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize a task manager thread."""
         self.actively_monitoring = False
-        self.task_history = dict()
-        self.tasks = []
+        self.task_history: t.Dict[str, t.Tuple[t.Optional[int], t.Optional[str], t.Optional[str]]] = {}
+        self.tasks: t.List[Task] = []
         self._lock = RLock()
 
-    def start(self):
+    def start(self) -> None:
         """Start the task manager thread
 
         The TaskManager is run as a daemon thread meaning
         that it will die when the main thread dies.
         """
         monitor = Thread(name="TaskManager", daemon=True, target=self.run)
         monitor.start()
 
-    def run(self):
+    def run(self) -> None:
         """Start monitoring Tasks"""
 
         global verbose_tm
         if verbose_tm:
             logger.debug("Starting Task Manager")
 
         self.actively_monitoring = True
@@ -93,15 +96,22 @@
                     self.remove_task(task.pid)
 
             if len(self) == 0:
                 self.actively_monitoring = False
                 if verbose_tm:
                     logger.debug("Sleeping, no tasks to monitor")
 
-    def start_task(self, cmd_list, cwd, env=None, out=PIPE, err=PIPE):
+    def start_task(
+        self,
+        cmd_list: t.List[str],
+        cwd: str,
+        env: t.Optional[t.Dict[str, str]] = None,
+        out: int = PIPE,
+        err: int = PIPE,
+    ) -> str:
         """Start a task managed by the TaskManager
 
         This is an "unmanaged" task, meaning it is NOT managed
         by a workload manager
 
         :param cmd_list: command to run
         :type cmd_list: list[str]
@@ -125,15 +135,21 @@
             self.tasks.append(task)
             self.task_history[task.pid] = (None, None, None)
             return task.pid
 
         finally:
             self._lock.release()
 
-    def start_and_wait(self, cmd_list, cwd, env=None, timeout=None):
+    def start_and_wait(
+        self,
+        cmd_list: t.List[str],
+        cwd: str,
+        env: t.Optional[t.Dict[str, str]] = None,
+        timeout: t.Optional[int] = None,
+    ) -> t.Tuple[int, str, str]:
         """Start a task not managed by the TaskManager
 
         This method is used by launchers to launch managed tasks
         meaning that they ARE managed by a WLM.
 
         This is primarily used for batch job launches
 
@@ -149,33 +165,33 @@
         :rtype: int, str, str
         """
         returncode, out, err = execute_cmd(cmd_list, cwd=cwd, env=env, timeout=timeout)
         if verbose_tm:
             logger.debug("Ran and waited on task")
         return returncode, out, err
 
-    def add_existing(self, task_id):
+    def add_existing(self, task_id: int) -> None:
         """Add existing task to be managed by the TaskManager
 
         :param task_id: task id of existing task
-        :type task_id: int
+        :type task_id: str
         :raises LauncherError: If task cannot be found
         """
         self._lock.acquire()
         try:
             process = psutil.Process(pid=task_id)
             task = Task(process)
             self.tasks.append(task)
             self.task_history[task.pid] = (None, None, None)
         except (psutil.NoSuchProcess, psutil.AccessDenied):
             raise LauncherError(f"Process provided {task_id} does not exist") from None
         finally:
             self._lock.release()
 
-    def remove_task(self, task_id):
+    def remove_task(self, task_id: str) -> None:
         """Remove a task from the TaskManager
 
         :param task_id: id of the task to remove
         :type task_id: str
         """
         self._lock.acquire()
         if verbose_tm:
@@ -191,15 +207,15 @@
         except psutil.NoSuchProcess:
             logger.debug("Failed to kill a task during removal")
         except KeyError:
             logger.debug("Failed to remove a task, task was already removed")
         finally:
             self._lock.release()
 
-    def get_task_update(self, task_id):
+    def get_task_update(self, task_id: str) -> t.Tuple[str, t.Optional[int], t.Optional[str], t.Optional[str]]:
         """Get the update of a task
 
         :param task_id: task id
         :type task_id: str
         :return: status, returncode, output, error
         :rtype: str, int, str, str
         """
@@ -219,114 +235,125 @@
 
             # process has completed, status set manually as we don't
             # save task statuses during runtime.
             else:
                 if rc != 0:
                     return "Failed", rc, out, err
                 return "Completed", rc, out, err
+        except KeyError:
+            logger.warning(f"Task {task_id} not found in task history dictionary")
         finally:
             self._lock.release()
 
-    def add_task_history(self, task_id, returncode, out=None, err=None):
+        return "Failed", -1, "", ""
+
+    def add_task_history(
+        self,
+        task_id: str,
+        returncode: t.Optional[int] = None,
+        out: t.Optional[str] = None,
+        err: t.Optional[str] = None,
+    ) -> None:
         """Add a task to the task history
 
         Add a task to record its future returncode, output and error
 
         :param task_id: id of the task
         :type task_id: str
         :param returncode: returncode
-        :type returncode: int
+        :type returncode: int, defaults to None
         :param out: output, defaults to None
         :type out: str, optional
         :param err: output, defaults to None
         :type err: str, optional
         """
         self.task_history[task_id] = (returncode, out, err)
 
-    def __getitem__(self, task_id):
+    def __getitem__(self, task_id: str) -> Task:
         self._lock.acquire()
         try:
             for task in self.tasks:
                 if task.pid == task_id:
                     return task
             raise KeyError
         finally:
             self._lock.release()
 
-    def __len__(self):
+    def __len__(self) -> int:
         self._lock.acquire()
         try:
             return len(self.tasks)
         finally:
             self._lock.release()
 
 
 class Task:
-    def __init__(self, process):
+    def __init__(self, process: psutil.Process) -> None:
         """Initialize a task
 
         :param process: Popen object
-        :type process: psutil.Popen
+        :type process: psutil.Process
         """
         self.process = process
         self.pid = str(self.process.pid)
 
-    def check_status(self):
+    def check_status(self) -> t.Optional[int]:
         """Ping the job and return the returncode if finished
 
         :return: returncode if finished otherwise None
         :rtype: int
         """
-        if self.owned:
+        if self.owned and isinstance(self.process, psutil.Popen):
             return self.process.poll()
         # we can't manage Processed we don't own
         # have to rely on .kill() to stop.
         return self.returncode
 
-    def get_io(self):
+    def get_io(self) -> t.Tuple[t.Optional[str], t.Optional[str]]:
         """Get the IO from the subprocess
 
         :return: output and error from the Popen
         :rtype: str, str
         """
         # Process class does not implement communicate
-        if not self.owned:
+        if not self.owned or not isinstance(self.process, psutil.Popen):
             return None, None
+
         output, error = self.process.communicate()
         if output:
             output = output.decode("utf-8")
         if error:
             error = error.decode("utf-8")
         return output, error
 
-    def kill(self, timeout=10):
+    def kill(self, timeout: int = 10) -> None:
         """Kill the subprocess and all children"""
 
-        def kill_callback(proc):
+        def kill_callback(proc: psutil.Process) -> None:
             logger.debug(f"Process terminated with kill {proc.pid}")
 
         children = self.process.children(recursive=True)
         children.append(self.process)  # add parent process to be killed
 
         for child in children:
             child.kill()
 
         _, alive = psutil.wait_procs(children, timeout=timeout, callback=kill_callback)
         if alive:
             for proc in alive:
                 logger.warning(f"Unable to kill emitted process {proc.pid}")
 
-    def terminate(self, timeout=10):
+    def terminate(self, timeout: int = 10) -> None:
         """Terminate a this process and all children.
 
         :param timeout: time to wait for task death, defaults to 10
         :type timeout: int, optional
         """
 
-        def terminate_callback(proc):
+        def terminate_callback(proc: psutil.Process) -> None:
             logger.debug(f"Cleanly terminated task {proc.pid}")
 
         children = self.process.children(recursive=True)
         children.append(self.process)  # add parent process to be killed
 
         # try SIGTERM first for clean exit
         for child in children:
@@ -339,31 +366,31 @@
             children, timeout=timeout, callback=terminate_callback
         )
 
         if alive:
             logger.debug(f"SIGTERM failed, using SIGKILL")
             self.process.kill()
 
-    def wait(self):
+    def wait(self) -> None:
         self.process.wait()
 
     @property
-    def returncode(self):
-        if self.owned:
+    def returncode(self) -> t.Optional[int]:
+        if self.owned and isinstance(self.process, psutil.Popen):
             return self.process.returncode
         if self.is_alive:
             return None
         return 0
 
     @property
-    def is_alive(self):
+    def is_alive(self) -> bool:
         return self.process.is_running()
 
     @property
-    def status(self):
+    def status(self) -> str:
         return self.process.status()
 
     @property
-    def owned(self):
+    def owned(self) -> bool:
         if isinstance(self.process, psutil.Popen):
             return True
         return False
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/util/__init__.py` & `smartsim-0.5.0/smartsim/_core/launcher/util/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/util/launcherUtil.py` & `smartsim-0.5.0/smartsim/_core/launcher/util/launcherUtil.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,32 +20,36 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 
 class ComputeNode:  # cov-slurm
     """The ComputeNode class holds resource information
     about a physical compute node
     """
 
-    def __init__(self, node_name=None, node_ppn=None):
+    def __init__(
+        self, node_name: t.Optional[str] = None, node_ppn: t.Optional[int] = None
+    ) -> None:
         """Initialize a ComputeNode
 
         :param node_name: the name of the node
         :type node_name: str
         :param node_ppn: the number of ppn
         :type node_ppn: int
         """
-        self.name = node_name
-        self.ppn = node_ppn
+        self.name: t.Optional[str] = node_name
+        self.ppn: t.Optional[int] = node_ppn
 
-    def _is_valid_node(self):
+    def _is_valid_node(self) -> bool:
         """Check if the node is complete
 
         Currently, validity is judged by name
         and ppn being not None.
 
         :returns: True if valid, false otherwise
         :rtype: bool
@@ -59,21 +63,21 @@
 
 
 class Partition:  # cov-slurm
     """The partition class holds information about
     a system partition.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize a system partition"""
-        self.name = None
-        self.min_ppn = None
-        self.nodes = set()
+        self.name: t.Optional[str] = None
+        self.min_ppn: t.Optional[int] = None
+        self.nodes: t.Set[ComputeNode] = set()
 
-    def _is_valid_partition(self):
+    def _is_valid_partition(self) -> bool:
         """Check if the partition is valid
 
         Currently, validity is judged by name
         and each ComputeNode being valid
 
         :returns: True if valid, false otherwise
         :rtype: bool
```

### Comparing `smartsim-0.4.2/smartsim/_core/launcher/util/shell.py` & `smartsim-0.5.0/smartsim/_core/launcher/util/shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,39 +20,46 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import psutil
 import time
+import typing as t
 from subprocess import PIPE, TimeoutExpired
 
-import psutil
-
 from ....error import ShellError
 from ....log import get_logger
 from ...utils.helpers import check_dev_log_level
 
 logger = get_logger(__name__)
 verbose_shell = check_dev_log_level()
 
 
-def execute_cmd(cmd_list, shell=False, cwd=None, env=None, proc_input="", timeout=None):
+def execute_cmd(
+    cmd_list: t.List[str],
+    shell: bool = False,
+    cwd: t.Optional[str] = None,
+    env: t.Optional[t.Dict[str, str]] = None,
+    proc_input: str = "",
+    timeout: t.Optional[int] = None,
+) -> t.Tuple[int, str, str]:
     """Execute a command locally
 
     :param cmd_list: list of command with arguments
     :type cmd_list: list of str
     :param shell: run in system shell, defaults to False
     :type shell: bool, optional
     :param cwd: current working directory, defaults to None
     :type cwd: str, optional
     :param env: environment to launcher process with,
                 defaults to None (current env)
-    :type env: dict, optional
+    :type env: dict[str, str], optional
     :param proc_input: input to the process, defaults to ""
     :type proc_input: str, optional
     :param timeout: timeout of the process, defaults to None
     :type timeout: int, optional
     :raises ShellError: if timeout of process was exceeded
     :raises ShellError: if child process raises an error
     :return: returncode, output, and error of the process
@@ -64,44 +71,46 @@
         logger.debug(f"Executing {source} cmd: {' '.join(cmd_list)}")
 
     # spawning the subprocess and connecting to its output
     proc = psutil.Popen(
         cmd_list, stderr=PIPE, stdout=PIPE, stdin=PIPE, cwd=cwd, shell=shell, env=env
     )
     try:
-        proc_input = proc_input.encode("utf-8")
-        out, err = proc.communicate(input=proc_input, timeout=timeout)
+        proc_bytes = proc_input.encode("utf-8")
+        out, err = proc.communicate(input=proc_bytes, timeout=timeout)
     except TimeoutExpired as e:
         proc.kill()
         _, errs = proc.communicate()
         logger.error(errs)
         raise ShellError(
-            "Failed to execute command, timeout reached", e, cmd_list
+            "Failed to execute command, timeout reached", cmd_list, details=e
         ) from None
     except OSError as e:
         raise ShellError(
-            "Exception while attempting to start a shell process", e, cmd_list
+            "Exception while attempting to start a shell process", cmd_list, details=e
         ) from None
 
     # decoding the output and err and return as a string tuple
     return proc.returncode, out.decode("utf-8"), err.decode("utf-8")
 
 
-def execute_async_cmd(cmd_list, cwd, env=None, out=PIPE, err=PIPE):
+def execute_async_cmd(
+    cmd_list: t.List[str], cwd: str, env: t.Optional[t.Dict[str, str]] = None, out: int = PIPE, err: int = PIPE
+) -> psutil.Popen:
     """Execute an asynchronous command
 
     This function executes an asynchronous command and returns a
     popen subprocess object wrapped with psutil.
 
     :param cmd_list: list of command with arguments
     :type cmd_list: list of str
     :param cwd: current working directory
     :type cwd: str
     :param env: environment variables to set
-    :type env: dict
+    :type env: dict[str, str]
     :return: the subprocess object
     :rtype: psutil.Popen
     """
     global verbose_shell
     if verbose_shell:
         logger.debug(f"Executing command: {' '.join(cmd_list)}")
 
@@ -114,11 +123,11 @@
         if not popen_obj.is_running() and popen_obj.returncode != 0:
             output, error = popen_obj.communicate()
             err_msg = ""
             if output:
                 err_msg += output.decode("utf-8") + " "
             if error:
                 err_msg += error.decode("utf-8")
-            raise ShellError("Command failed immediately", err_msg, cmd_list)
+            raise ShellError("Command failed immediately", cmd_list, details=err_msg)
     except OSError as e:
-        raise ShellError("Failed to run command", e, cmd_list) from None
+        raise ShellError("Failed to run command", cmd_list, details=e) from None
     return popen_obj
```

### Comparing `smartsim-0.4.2/smartsim/_core/utils/__init__.py` & `smartsim-0.5.0/smartsim/_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/_core/utils/helpers.py` & `smartsim-0.5.0/smartsim/_core/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,45 +25,46 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 A file of helper functions for SmartSim
 """
 import os
 import uuid
+import typing as t
 from functools import lru_cache
 from pathlib import Path
 from shutil import which
 
 
-def create_lockfile_name():
+def create_lockfile_name() -> str:
     """Generate a unique lock filename using UUID"""
     lock_suffix = str(uuid.uuid4())[:7]
     return f"smartsim-{lock_suffix}.lock"
 
 
 @lru_cache(maxsize=20, typed=False)
-def check_dev_log_level():
+def check_dev_log_level() -> bool:
     try:
         lvl = os.environ["SMARTSIM_LOG_LEVEL"]
         if lvl == "developer":
             return True
         return False
     except KeyError:
         return False
 
 
-def fmt_dict(d):
+def fmt_dict(d: t.Dict[str, t.Any]) -> str:
     fmt_str = ""
     for k, v in d.items():
         fmt_str += "\t" + str(k) + " = " + str(v)
         fmt_str += "\n" if k != list(d.keys())[-1] else ""
     return fmt_str
 
 
-def get_base_36_repr(positive_int):
+def get_base_36_repr(positive_int: int) -> str:
     """Converts a positive integer to its base 36 representation
     :param positive_int: the positive integer to convert
     :type positive_int: int
     :return: base 36 representation of the given positive int
     :rtype: str
     """
     digits = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
@@ -72,24 +73,23 @@
     while positive_int:
         next_digit = digits[positive_int % 36]
         result.append(next_digit)
         positive_int //= 36
 
     return "".join(reversed(result))
 
-
-def init_default(default, init_value, expected_type=None):
+def init_default(default: t.Any, init_value: t.Any, expected_type: t.Optional[t.Union[t.Type, t.Tuple]] = None) -> t.Any:
     if init_value is None:
         return default
     if expected_type is not None and not isinstance(init_value, expected_type):
         raise TypeError(f"Argument was of type {type(init_value)}, not {expected_type}")
     return init_value
 
 
-def expand_exe_path(exe):
+def expand_exe_path(exe: str) -> str:
     """Takes an executable and returns the full path to that executable
 
     :param exe: executable or file
     :type exe: str
     :raises TypeError: if file is not an executable
     :raises FileNotFoundError: if executable cannot be found
     """
@@ -101,36 +101,39 @@
             return os.path.abspath(exe)
         if os.path.isfile(exe) and not os.access(exe, os.X_OK):
             raise TypeError(f"File, {exe}, is not an executable")
         raise FileNotFoundError(f"Could not locate executable {exe}")
     return os.path.abspath(in_path)
 
 
-def is_valid_cmd(command):
+def is_valid_cmd(command: t.Union[str, None]) -> bool:
     try:
-        expand_exe_path(command)
-        return True
+        if command:
+            expand_exe_path(command)
+            return True
     except (TypeError, FileNotFoundError):
         return False
 
+    return False
+
 
 color2num = dict(
     gray=30,
     red=31,
     green=32,
     yellow=33,
     blue=34,
     magenta=35,
     cyan=36,
     white=37,
     crimson=38,
 )
 
 
-def colorize(string, color, bold=False, highlight=False):
+def colorize(string: str, color: str, bold: bool = False, highlight: bool = False) -> str:
     """
     Colorize a string.
     This function was originally written by John Schulman.
     And then borrowed from spinningup
     https://github.com/openai/spinningup/blob/master/spinup/utils/logx.py
     """
     attr = []
@@ -139,27 +142,27 @@
         num += 10
     attr.append(str(num))
     if bold:
         attr.append("1")
     return "\x1b[%sm%s\x1b[0m" % (";".join(attr), string)
 
 
-def delete_elements(dictionary, key_list):
+def delete_elements(dictionary: t.Dict[str, t.Any], key_list: t.List[str]) -> None:
     """Delete elements from a dictionary.
     :param dictionary: the dictionary from which the elements must be deleted.
     :type dictionary: dict
     :param key_list: the list of keys to delete from the dictionary.
     :type key: any
     """
     for key in key_list:
         if key in dictionary:
             del dictionary[key]
 
 
-def cat_arg_and_value(arg_name, value):
+def cat_arg_and_value(arg_name: str, value: str) -> str:
     """Concatenate a command line argument and its value
 
     This function returns ``arg_name`` and ``value
     concatenated in the best possible way for a command
     line execution, namely:
     - if arg_name starts with `--` (e.g. `--arg`):
       `arg_name=value` is returned (i.e. `--arg=val`)
@@ -184,15 +187,25 @@
         return " ".join((arg_name, str(value)))
     elif len(arg_name) == 1:
         return " ".join(("-" + arg_name, str(value)))
     else:
         return "=".join(("--" + arg_name, str(value)))
 
 
-def installed_redisai_backends(backends_path=None):
+def _installed(base_path: Path, backend: str) -> bool:
+    """
+    Check if a backend is available for the RedisAI module.
+    """
+    backend_key = f"redisai_{backend}"
+    backend_path = base_path / backend_key / f"{backend_key}.so"
+    backend_so = Path(os.environ.get("RAI_PATH", backend_path)).resolve()
+    
+    return backend_so.is_file()
+
+def installed_redisai_backends(backends_path: t.Optional[str] = None) -> t.List[str]:
     """Check which ML backends are available for the RedisAI module.
 
     The optional argument ``backends_path`` is needed if the backends
     have not been built as part of the SmartSim building process (i.e.
     they have not been built by invoking `smart build`). In that case
     ``backends_path`` should point to the directory containing e.g.
     the backend directories (`redisai_tensorflow`, `redisai_torch`,
@@ -202,17 +215,12 @@
     :type backends_path: str, optional
     :return: list of installed RedisAI backends
     :rtype: list[str]
     """
     # import here to avoid circular import
     from ..._core.config import CONFIG
 
-    installed = []
-    if not backends_path:
-        backends_path = CONFIG.lib_path / "backends"
-    for backend in ["tensorflow", "torch", "onnxruntime", "tflite"]:
-        backend_path = backends_path / f"redisai_{backend}" / f"redisai_{backend}.so"
-        backend_so = Path(os.environ.get("RAI_PATH", backend_path)).resolve()
-        if backend_so.is_file():
-            installed.append(backend)
+    base_path = Path(backends_path) if backends_path else CONFIG.lib_path / "backends"
+    backends = ["tensorflow", "torch", "onnxruntime", "tflite"]
 
+    installed = [backend for backend in backends if _installed(base_path, backend)]
     return installed
```

### Comparing `smartsim-0.4.2/smartsim/_core/utils/network.py` & `smartsim-0.5.0/smartsim/_core/utils/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 import psutil
 
 """
 A handful of useful functions for dealing with networks
 """
 
 
-def get_ip_from_host(host):
+def get_ip_from_host(host: str) -> str:
     """Return the IP address for the interconnect.
 
     :param host: hostname of the compute node e.g. nid00004
     :type host: str
     :returns: ip of host
     :rtype: str
     """
     ip_address = socket.gethostbyname(host)
     return ip_address
 
 
 # impossible to cover as it's only used in entrypoints
-def get_ip_from_interface(interface):  # pragma: no cover
+def get_ip_from_interface(interface: str) -> str:  # pragma: no cover
     """Get IPV4 address of a network interface
 
     :param interface: interface name
     :type interface: str
     :raises ValueError: if the interface does not exist
     :raises ValueError: if interface does not have an IPV4 address
     :return: ip address of interface
@@ -68,22 +68,22 @@
     for info in net_if_addrs[interface]:
         if info.family == socket.AF_INET:
             return info.address
     raise ValueError(f"interface {interface} doesn't have an IPv4 address")
 
 
 # impossible to cover as it's only used in entrypoints
-def get_lb_interface_name():  # pragma: no cover
+def get_lb_interface_name() -> str:  # pragma: no cover
     """Use psutil to get loopback interface name"""
     net_if_addrs = list(psutil.net_if_addrs())
     for interface in net_if_addrs:
         if interface.startswith("lo"):
             return interface
     raise OSError("Could not find loopback interface name")
 
 
-def current_ip(interface="lo"):  # pragma: no cover
+def current_ip(interface: str = "lo") -> str:  # pragma: no cover
     if interface == "lo":
         loopback = get_lb_interface_name()
         return get_ip_from_interface(loopback)
     else:
         return get_ip_from_interface(interface)
```

### Comparing `smartsim-0.4.2/smartsim/_core/utils/redis.py` & `smartsim-0.5.0/smartsim/_core/utils/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,35 +21,36 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
+import redis
 import time
+import typing as t
 
-import redis
-from rediscluster import RedisCluster
-from rediscluster.exceptions import ClusterDownError, RedisClusterException
+from itertools import product
+from redis.cluster import RedisCluster, ClusterNode
+from redis.exceptions import ClusterDownError, RedisClusterException
 from smartredis import Client
 from smartredis.error import RedisReplyError
 
-logging.getLogger("rediscluster").setLevel(logging.WARNING)
-
 from ...entity import DBModel, DBScript
 from ...error import SSInternalError
 from ...log import get_logger
 from ..config import CONFIG
 from ..launcher.util.shell import execute_cmd
 from .network import get_ip_from_host
 
+logging.getLogger("rediscluster").setLevel(logging.WARNING)
 logger = get_logger(__name__)
 
 
-def create_cluster(hosts, ports):  # cov-wlm
+def create_cluster(hosts: t.List[str], ports: t.List[int]) -> None:  # cov-wlm
     """Connect launched cluster instances.
 
     Should only be used in the case where cluster initialization
     needs to occur manually which is not often.
 
     :param hosts: List of hostnames to connect to
     :type hosts: List[str]
@@ -74,52 +75,50 @@
     if returncode != 0:
         logger.error(out)
         logger.error(err)
         raise SSInternalError("Database '--cluster create' command failed")
     logger.debug(out)
 
 
-def check_cluster_status(hosts, ports, trials=10):  # cov-wlm
+def check_cluster_status(hosts: t.List[str], ports: t.List[int], trials: int = 10) -> None:  # cov-wlm
     """Check that a Redis/KeyDB cluster is up and running
 
     :param hosts: List of hostnames to connect to
     :type hosts: List[str]
     :param ports: List of ports for each hostname
     :type ports: List[int]
     :param trials: number of attempts to verify cluster status
     :type trials: int, optional
 
     :raises SmartSimError: If cluster status cannot be verified
     """
-    host_list = []
-    for host in hosts:
-        for port in ports:
-            host_dict = dict()
-            host_dict["host"] = get_ip_from_host(host)
-            host_dict["port"] = port
-            host_list.append(host_dict)
+    cluster_nodes = [ClusterNode(get_ip_from_host(host), port)
+                     for host, port in product(hosts, ports)]
+
+    if not cluster_nodes:
+        raise SSInternalError("No cluster nodes have been set for database status check.")
 
     logger.debug("Beginning database cluster status check...")
     while trials > 0:
         # wait for cluster to spin up
         time.sleep(5)
         try:
-            redis_tester = RedisCluster(startup_nodes=host_list)
+            redis_tester: RedisCluster = RedisCluster(startup_nodes=cluster_nodes)
             redis_tester.set("__test__", "__test__")
-            redis_tester.delete("__test__")
+            redis_tester.delete("__test__")  # type: ignore
             logger.debug("Cluster status verified")
             return
         except (ClusterDownError, RedisClusterException, redis.RedisError):
             logger.debug("Cluster still spinning up...")
             trials -= 1
     if trials == 0:
         raise SSInternalError("Cluster setup could not be verified")
 
 
-def db_is_active(hosts, ports, num_shards):
+def db_is_active(hosts: t.List[str], ports: t.List[int], num_shards: int) -> bool:
     """Check if a DB is running
 
     if the DB is clustered, check cluster status, otherwise
     just ping DB.
 
     :param hosts: list of hosts
     :type hosts: list[str]
@@ -147,15 +146,15 @@
             check_cluster_status(hosts, ports, trials=1)
             return True
         # we expect this to fail if the cluster is not active
         except SSInternalError:
             return False
 
 
-def set_ml_model(db_model: DBModel, client: Client):
+def set_ml_model(db_model: DBModel, client: Client) -> None:
     logger.debug(f"Adding DBModel named {db_model.name}")
     devices = db_model._enumerate_devices()
 
     for device in devices:
         try:
             if db_model.is_file:
                 client.set_model_from_file(
@@ -182,15 +181,15 @@
                     outputs=db_model.outputs,
                 )
         except RedisReplyError as error:  # pragma: no cover
             logger.error("Error while setting model on orchestrator.")
             raise error
 
 
-def set_script(db_script: DBScript, client: Client):
+def set_script(db_script: DBScript, client: Client) -> None:
     logger.debug(f"Adding DBScript named {db_script.name}")
 
     devices = db_script._enumerate_devices()
 
     for device in devices:
         try:
             if db_script.is_file:
```

### Comparing `smartsim-0.4.2/smartsim/constants.py` & `smartsim-0.5.0/smartsim/settings/mpirunSettings.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,35 +20,20 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-# Constants for SmartSim
-
 from warnings import simplefilter, warn
 
-dep_msg = "This is a deprecated module. Please use smartsim.status instead.\n"
-dep_msg += "This module will be removed in the next release."
-
-simplefilter("once", DeprecationWarning)
-warn(dep_msg, DeprecationWarning, stacklevel=2)
+from ..log import get_logger
+from .mpiSettings import MpiexecSettings, MpirunSettings, OrterunSettings
 
+logger = get_logger(__name__)
 
-# Statuses that are applied to jobs
-STATUS_RUNNING = "Running"
-STATUS_COMPLETED = "Completed"
-STATUS_CANCELLED = "Cancelled"
-STATUS_FAILED = "Failed"
-STATUS_NEW = "New"
-STATUS_PAUSED = "Paused"
-
-# SmartSim status mapping
-SMARTSIM_STATUS = {
-    "Running": STATUS_RUNNING,
-    "Paused": STATUS_PAUSED,
-    "Completed": STATUS_COMPLETED,
-    "Cancelled": STATUS_CANCELLED,
-    "Failed": STATUS_FAILED,
-    "New": STATUS_NEW,
-}
+simplefilter("once", DeprecationWarning)
+warn(
+    "mpirunSettings will be deprecated; use mpiSettings instead.",
+    DeprecationWarning,
+    stacklevel=2,
+)
```

### Comparing `smartsim-0.4.2/smartsim/database/__init__.py` & `smartsim-0.5.0/smartsim/entity/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-# deprecated classes
-from .orchestrator import (
-    CobaltOrchestrator,
-    LSFOrchestrator,
-    Orchestrator,
-    PBSOrchestrator,
-    SlurmOrchestrator,
-)
+from .dbnode import DBNode
+from .dbobject import *
+from .ensemble import Ensemble
+from .entity import SmartSimEntity
+from .files import TaggedFilesHierarchy
+from .entityList import EntityList
+from .model import Model
```

### Comparing `smartsim-0.4.2/smartsim/database/orchestrator.py` & `smartsim-0.5.0/smartsim/database/orchestrator.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,30 +20,33 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import itertools
+import psutil
 import sys
+import typing as t
+
 from os import getcwd
 from shlex import split as sh_split
 from warnings import simplefilter, warn
 
-import psutil
 from smartredis import Client
 from smartredis.error import RedisReplyError
 
 from .._core.config import CONFIG
 from .._core.utils import db_is_active
 from .._core.utils.helpers import is_valid_cmd
 from .._core.utils.network import get_ip_from_host
 from ..entity import DBNode, EntityList
 from ..error import SmartSimError, SSConfigError, SSUnsupportedError
 from ..log import get_logger
+from ..settings.base import BatchSettings, RunSettings
 from ..settings import (
     AprunSettings,
     BsubBatchSettings,
     CobaltBatchSettings,
     JsrunSettings,
     MpiexecSettings,
     MpirunSettings,
@@ -64,33 +67,33 @@
     alongside entities in SmartSim. Data can be transferred between
     entities by using one of the Python, C, C++ or Fortran clients
     within an entity.
     """
 
     def __init__(
         self,
-        port=6379,
-        interface="lo",
-        launcher="local",
-        run_command="auto",
-        db_nodes=1,
-        batch=False,
-        hosts=None,
-        account=None,
-        time=None,
-        alloc=None,
-        single_cmd=False,
-        **kwargs,
-    ):
+        port: int = 6379,
+        interface: t.Union[str, t.List[str]] = "lo",
+        launcher: str = "local",
+        run_command: str = "auto",
+        db_nodes: int = 1,
+        batch: bool = False,
+        hosts: t.Optional[t.List[str]] = None,
+        account: t.Optional[str] = None,
+        time: t.Optional[str] = None,
+        alloc: t.Optional[str] = None,
+        single_cmd: bool = False,
+        **kwargs: t.Any,
+    ) -> None:
         """Initialize an Orchestrator reference for local launch
 
         :param port: TCP/IP port, defaults to 6379
         :type port: int, optional
-        :param interface: network interface, defaults to "lo"
-        :type interface: str, optional
+        :param interface: network interface(s), defaults to "lo"
+        :type interface: str, list[str], optional
 
         Extra configurations for RedisAI
 
         See https://oss.redislabs.com/redisai/configuration/
 
         :param threads_per_queue: threads per GPU device
         :type threads_per_queue: int, optional
@@ -99,23 +102,23 @@
         :param intra_op_threads: threads per CPU operation
         :type intra_op_threads: int, optional
         """
 
         if launcher == "auto":
             launcher = detect_launcher()
 
-        by_launcher = {
+        by_launcher: t.Dict[str, t.List[str]] = {
             "slurm": ["srun", "mpirun", "mpiexec"],
             "pbs": ["aprun", "mpirun", "mpiexec"],
             "cobalt": ["aprun", "mpirun", "mpiexec"],
             "lsf": ["jsrun"],
-            "local": [None],
+            "local": [""],
         }
 
-        def _detect_command(launcher):
+        def _detect_command(launcher: str) -> str:
             if launcher in by_launcher:
                 for cmd in by_launcher[launcher]:
                     if launcher == "local":
                         return cmd
                     if is_valid_cmd(cmd):
                         return cmd
             msg = f"Could not automatically detect a run command to use for launcher {launcher}"
@@ -129,27 +132,30 @@
             msg = f"Run command {run_command} is not supported on launcher {launcher}\n"
             msg += f"Supported run commands for the given launcher are: {by_launcher[launcher]}"
             raise SmartSimError(msg)
 
         if launcher == "local" and batch:
             msg = "Local orchestrator can not be launched with batch=True"
             raise SmartSimError(msg)
+
         if run_command == "aprun" and batch and single_cmd:
             msg = "aprun can not launch an orchestrator with batch=True and single_cmd=True. "
             msg += "Automatically switching to single_cmd=False."
             logger.info(msg)
             single_cmd = False
 
         self.launcher = launcher
         self.run_command = run_command
 
-        self.ports = []
+        self.ports: t.List[int] = []
         self.path = getcwd()
-        self._hosts = []
-        self._interface = interface
+        self._hosts: t.List[str] = []
+        if isinstance(interface, str):
+            interface = [interface]
+        self._interfaces = interface
         self._check_network_interface()
         self.queue_threads = kwargs.get("threads_per_queue", None)
         self.inter_threads = kwargs.get("inter_op_threads", None)
         self.intra_threads = kwargs.get("intra_op_threads", None)
         if self.launcher == "lsf":
             gpus_per_shard = kwargs.pop("gpus_per_shard", 0)
             cpus_per_shard = kwargs.pop("cpus_per_shard", 4)
@@ -175,102 +181,102 @@
 
         # detect if we can find at least the redis binaries. We
         # don't want to force the user to launch with RedisAI so
         # it's ok if that isn't present.
         try:
             # try to obtain redis binaries needed to launch Redis
             # will raise SSConfigError if not found
-            self._redis_exe
-            self._redis_conf
-            CONFIG.database_cli
+            self._redis_exe  # pylint: disable=W0104
+            self._redis_conf  # pylint: disable=W0104
+            CONFIG.database_cli  # pylint: disable=W0104
         except SSConfigError as e:
             msg = "SmartSim not installed with pre-built extensions (Redis)\n"
             msg += "Use the `smart` cli tool to install needed extensions\n"
             msg += "or set REDIS_PATH and REDIS_CLI_PATH in your environment\n"
             msg += "See documentation for more information"
             raise SSConfigError(msg) from e
 
         if launcher != "local":
             self.batch_settings = self._build_batch_settings(
-                db_nodes, alloc, batch, account, time, launcher=launcher, **kwargs
+                db_nodes, alloc or "", batch, account or "", time or "", launcher=launcher, **kwargs
             )
             if hosts:
                 self.set_hosts(hosts)
             elif not hosts and run_command == "mpirun":
                 raise SmartSimError(
                     "hosts argument is required when launching Orchestrator with mpirun"
                 )
-            self._reserved_run_args = {}
-            self._reserved_batch_args = {}
+            self._reserved_run_args: t.Dict[t.Type[RunSettings], t.List[str]] = {}
+            self._reserved_batch_args: t.Dict[t.Type[BatchSettings], t.List[str]] = {}
             self._fill_reserved()
 
     @property
-    def num_shards(self):
+    def num_shards(self) -> int:
         """Return the number of DB shards contained in the orchestrator.
         This might differ from the number of ``DBNode`` objects, as each
         ``DBNode`` may start more than one shard (e.g. with MPMD).
 
         :returns: num_shards
         :rtype: int
         """
         return self.db_nodes
 
     @property
-    def hosts(self):
+    def hosts(self) -> t.List[str]:
         """Return the hostnames of orchestrator instance hosts
 
         Note that this will only be populated after the orchestrator
         has been launched by SmartSim.
 
         :return: hostnames
         :rtype: list[str]
         """
         if not self._hosts:
             self._hosts = self._get_db_hosts()
         return self._hosts
 
-    def remove_stale_files(self):
+    def remove_stale_files(self) -> None:
         """Can be used to remove database files of a previous launch"""
 
-        for dbnode in self.entities:
-            dbnode.remove_stale_dbnode_files()
+        for db in self.dbnodes:
+            db.remove_stale_dbnode_files()
 
-    def get_address(self):
+    def get_address(self) -> t.List[str]:
         """Return database addresses
 
         :return: addresses
         :rtype: list[str]
 
         :raises SmartSimError: If database address cannot be found or is not active
         """
         if not self._hosts:
             raise SmartSimError("Could not find database address")
         elif not self.is_active():
             raise SmartSimError("Database is not active")
         return self._get_address()
 
-    def _get_address(self):
-        addresses = []
+    def _get_address(self) -> t.List[str]:
+        addresses: t.List[str] = []
         for ip, port in itertools.product(self._hosts, self.ports):
             addresses.append(":".join((ip, str(port))))
         return addresses
 
-    def is_active(self):
+    def is_active(self) -> bool:
         """Check if the database is active
 
         :return: True if database is active, False otherwise
         :rtype: bool
         """
         if not self._hosts:
             return False
 
         return db_is_active(self._hosts, self.ports, self.num_shards)
 
     @property
-    def _rai_module(self):
+    def _rai_module(self) -> str:
         """Get the RedisAI module from third-party installations
 
         :return: path to module or "" if not found
         :rtype: str
         """
         module = ["--loadmodule", CONFIG.redisai]
         if self.queue_threads:
@@ -278,107 +284,118 @@
         if self.inter_threads:
             module.append(f"INTER_OP_PARALLELISM {self.inter_threads}")
         if self.intra_threads:
             module.append(f"INTRA_OP_PARALLELISM {self.intra_threads}")
         return " ".join(module)
 
     @property
-    def _redis_exe(self):
+    def _redis_exe(self) -> str:
         return CONFIG.database_exe
 
     @property
-    def _redis_conf(self):
+    def _redis_conf(self) -> str:
         return CONFIG.database_conf
 
-    def set_cpus(self, num_cpus):
+    def set_cpus(self, num_cpus: int) -> None:
         """Set the number of CPUs available to each database shard
 
         This effectively will determine how many cpus can be used for
         compute threads, background threads, and network I/O.
 
         :param num_cpus: number of cpus to set
         :type num_cpus: int
         """
         if self.batch:
             if self.launcher == "pbs" or self.launcher == "cobalt":
-                self.batch_settings.set_ncpus(num_cpus)
+                if hasattr(self, 'batch_settings') and self.batch_settings:
+                    if hasattr(self.batch_settings, 'set_ncpus'):
+                        self.batch_settings.set_ncpus(num_cpus)
             if self.launcher == "slurm":
-                self.batch_settings.set_cpus_per_task(num_cpus)
-        for db in self:
+                if hasattr(self, 'batch_settings') and self.batch_settings:
+                    if hasattr(self.batch_settings, 'set_cpus_per_task'):
+                        self.batch_settings.set_cpus_per_task(num_cpus)
+
+        for db in self.dbnodes:
             db.run_settings.set_cpus_per_task(num_cpus)
-            if db._mpmd:
-                for mpmd in db.run_settings.mpmd:
-                    mpmd.set_cpus_per_task(num_cpus)
+            if db._mpmd and hasattr(db.run_settings, 'mpmd'):
+                    for mpmd in db.run_settings.mpmd:
+                        mpmd.set_cpus_per_task(num_cpus)
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the batch walltime of the orchestrator
 
         Note: This will only effect orchestrators launched as a batch
 
         :param walltime: amount of time e.g. 10 hours is 10:00:00
         :type walltime: str
         :raises SmartSimError: if orchestrator isn't launching as batch
         """
         if not self.batch:
             raise SmartSimError("Not running as batch, cannot set walltime")
-        self.batch_settings.set_walltime(walltime)
 
-    def set_hosts(self, host_list):
+        if hasattr(self, 'batch_settings') and self.batch_settings:
+            self.batch_settings.set_walltime(walltime)
+
+    def set_hosts(self, host_list: t.List[str]) -> None:
         """Specify the hosts for the ``Orchestrator`` to launch on
 
         :param host_list: list of host (compute node names)
         :type host_list: str, list[str]
         :raises TypeError: if wrong type
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         # TODO check length
         if self.batch:
-            self.batch_settings.set_hostlist(host_list)
+            if hasattr(self, 'batch_settings') and self.batch_settings:
+                self.batch_settings.set_hostlist(host_list)
 
         if self.launcher == "lsf":
-            for db in self:
+            for db in self.dbnodes:
                 db.set_hosts(host_list)
         else:
-            for host, db in zip(host_list, self.entities):
+            for host, db in zip(host_list, self.dbnodes):
                 if isinstance(db.run_settings, AprunSettings):
                     if not self.batch:
                         db.run_settings.set_hostlist([host])
                 else:
                     db.run_settings.set_hostlist([host])
-                if db._mpmd:
+
+                if db._mpmd and hasattr(db.run_settings, 'mpmd'):
                     for i, mpmd_runsettings in enumerate(db.run_settings.mpmd):
                         mpmd_runsettings.set_hostlist(host_list[i + 1])
 
-    def set_batch_arg(self, arg, value):
+    def set_batch_arg(self, arg: str, value: t.Optional[str] = None) -> None:
         """Set a batch argument the orchestrator should launch with
 
         Some commonly used arguments such as --job-name are used
         by SmartSim and will not be allowed to be set.
 
         :param arg: batch argument to set e.g. "exclusive"
         :type arg: str
         :param value: batch param - set to None if no param value
         :type value: str | None
         :raises SmartSimError: if orchestrator not launching as batch
-        """
-        if not self.batch:
+        """        
+        if not hasattr(self, 'batch_settings') or not self.batch_settings:
             raise SmartSimError("Not running as batch, cannot set batch_arg")
+
         if arg in self._reserved_batch_args[type(self.batch_settings)]:
             logger.warning(
                 f"Can not set batch argument {arg}: it is a reserved keyword in Orchestrator"
             )
         else:
-            self.batch_settings.batch_args[arg] = value
+            if hasattr(self, 'batch_settings') and self.batch_settings:
+                self.batch_settings.batch_args[arg] = value
 
-    def set_run_arg(self, arg, value):
+    def set_run_arg(self, arg: str, value: t.Optional[str] = None) -> None:
         """Set a run argument the orchestrator should launch
         each node with (it will be passed to `jrun`)
 
         Some commonly used arguments are used
         by SmartSim and will not be allowed to be set.
         For example, "n", "N", etc.
 
@@ -388,34 +405,34 @@
         :type value: str | None
         """
         if arg in self._reserved_run_args[type(self.entities[0].run_settings)]:
             logger.warning(
                 f"Can not set run argument {arg}: it is a reserved keyword in Orchestrator"
             )
         else:
-            for db in self.entities:
+            for db in self.dbnodes:
                 db.run_settings.run_args[arg] = value
-                if db._mpmd:
+                if db._mpmd and hasattr(db.run_settings, 'mpmd'):
                     for mpmd in db.run_settings.mpmd:
                         mpmd.run_args[arg] = value
 
-    def enable_checkpoints(self, frequency):
+    def enable_checkpoints(self, frequency: int) -> None:
         """Sets the database's save configuration to save the
         DB every 'frequency' seconds given that at least one
         write operation against the DB occurred in that time.
         For example, if `frequency` is 900, then the database
         will save to disk after 900 seconds if there is at least
         1 change to the dataset.
 
         :param frequency: the given number of seconds before the DB saves
         :type frequency: int
         """
         self.set_db_conf("save", str(frequency) + " 1")
 
-    def set_max_memory(self, mem):
+    def set_max_memory(self, mem: int) -> None:
         """Sets the max memory configuration. By default there is no memory limit.
         Setting max memory to zero also results in no memory limit. Once a limit is
         surpassed, keys will be removed according to the eviction strategy. The
         specified memory size is case insensitive and supports the typical forms of:
         1k => 1000 bytes
         1kb => 1024 bytes
         1m => 1000000 bytes
@@ -427,51 +444,51 @@
         :type mem: str
 
         :raises SmartSimError: If 'mem' is an invalid memory value
         :raises SmartSimError: If database is not active
         """
         self.set_db_conf("maxmemory", mem)
 
-    def set_eviction_strategy(self, strategy):
+    def set_eviction_strategy(self, strategy: str) -> None:
         """Sets how the database will select what to remove when
         'maxmemory' is reached. The default is noeviction.
 
         :param strategy: The max memory policy to use e.g. "volatile-lru", "allkeys-lru", etc.
         :type strategy: str
 
         :raises SmartSimError: If 'strategy' is an invalid maxmemory policy
         :raises SmartSimError: If database is not active
         """
         self.set_db_conf("maxmemory-policy", strategy)
 
-    def set_max_clients(self, clients=50_000):
+    def set_max_clients(self, clients: int = 50_000) -> None:
         """Sets the max number of connected clients at the same time.
         When the number of DB shards contained in the orchestrator is
         more than two, then every node will use two connections, one
         incoming and another outgoing.
 
         :param clients: the maximum number of connected clients
         :type clients: int, optional
         """
         self.set_db_conf("maxclients", str(clients))
 
-    def set_max_message_size(self, size=1_073_741_824):
+    def set_max_message_size(self, size: int = 1_073_741_824) -> None:
         """Sets the database's memory size limit for bulk requests,
         which are elements representing single strings. The default
         is 1 gigabyte. Message size must be greater than or equal to 1mb.
         The specified memory size should be an integer that represents
         the number of bytes. For example, to set the max message size
         to 1gb, use 1024*1024*1024.
 
         :param size: maximum message size in bytes
         :type size: int, optional
         """
         self.set_db_conf("proto-max-bulk-len", str(size))
 
-    def set_db_conf(self, key, value):
+    def set_db_conf(self, key: str, value: t.Union[int, str]) -> None:
         """Set any valid configuration at runtime without the need
         to restart the database. All configuration parameters
         that are set are immediately loaded by the database and
         will take effect starting with the next command executed.
 
         :param key: the configuration parameter
         :type key: str
@@ -500,28 +517,38 @@
                     "Incompatible function arguments. The key and value used for setting the database configurations must be strings."
                 ) from None
         else:
             raise SmartSimError(
                 "The SmartSim Orchestrator must be active in order to set the database's configurations."
             )
 
-    def _build_batch_settings(self, db_nodes, alloc, batch, account, time, **kwargs):
+    def _build_batch_settings(
+        self,
+        db_nodes: int,
+        alloc: str,
+        batch: bool,
+        account: str,
+        time: str,
+        **kwargs: t.Any,
+    ) -> t.Optional[BatchSettings]:
         batch_settings = None
         launcher = kwargs.pop("launcher")
 
         # enter this conditional if user has not specified an allocation to run
         # on or if user specified batch=False (alloc will be found through env)
         if not alloc and batch:
             batch_settings = create_batch_settings(
                 launcher, nodes=db_nodes, time=time, account=account, **kwargs
             )
 
         return batch_settings
 
-    def _build_run_settings(self, exe, exe_args, **kwargs):
+    def _build_run_settings(
+        self, exe: str, exe_args: t.List[t.List[str]], **kwargs: t.Any
+    ) -> RunSettings:
         run_args = kwargs.pop("run_args", {})
         db_nodes = kwargs.get("db_nodes", 1)
         single_cmd = kwargs.get("single_cmd", True)
         mpmd_nodes = single_cmd and db_nodes > 1
 
         if mpmd_nodes:
             run_settings = create_run_settings(
@@ -536,33 +563,35 @@
                     exe=exe, exe_args=exe_arg, run_args=run_args.copy(), **kwargs
                 )
                 mpmd_run_settings.set_tasks(1)
                 mpmd_run_settings.set_tasks_per_node(1)
                 run_settings.make_mpmd(mpmd_run_settings)
         else:
             run_settings = create_run_settings(
-                exe=exe, exe_args=exe_args, run_args=run_args.copy(), **kwargs
+                exe=exe, exe_args=exe_args[0], run_args=run_args.copy(), **kwargs
             )
 
             if self.launcher != "local":
                 run_settings.set_tasks(1)
 
         if self.launcher != "local":
             run_settings.set_tasks_per_node(1)
 
         # Put it back in case it is needed again
         kwargs["run_args"] = run_args
 
         return run_settings
 
-    def _build_run_settings_lsf(self, exe, exe_args, **kwargs):
+    def _build_run_settings_lsf(
+        self, exe: str, exe_args: t.List[t.List[str]], **kwargs: t.Any
+    ) -> t.Optional[JsrunSettings]:
         run_args = kwargs.pop("run_args", {})
         cpus_per_shard = kwargs.get("cpus_per_shard", None)
         gpus_per_shard = kwargs.get("gpus_per_shard", None)
-        erf_rs = None
+        erf_rs: t.Optional[JsrunSettings] = None
 
         # We always run the DB on cpus 0:cpus_per_shard-1
         # and gpus 0:gpus_per_shard-1
         for shard_id, args in enumerate(exe_args):
             host = shard_id
             run_args["launch_distribution"] = "packed"
 
@@ -581,24 +610,25 @@
             if gpus_per_shard > 1:  # pragma: no-cover
                 erf_sets["gpu"] = "{" + f"0-{gpus_per_shard-1}" + "}"
             elif gpus_per_shard > 0:
                 erf_sets["gpu"] = "{" + str(0) + "}"
 
             run_settings.set_erf_sets(erf_sets)
 
-            if erf_rs:
-                erf_rs.make_mpmd(run_settings)
-            else:
-                run_settings.make_mpmd()
+            if not erf_rs:
                 erf_rs = run_settings
+                continue
 
+            erf_rs.make_mpmd(run_settings)
+            
         kwargs["run_args"] = run_args
+
         return erf_rs
 
-    def _initialize_entities(self, **kwargs):
+    def _initialize_entities(self, **kwargs: t.Any) -> None:
         self.db_nodes = kwargs.get("db_nodes", 1)
         single_cmd = kwargs.get("single_cmd", True)
 
         if int(self.db_nodes) == 2:
             raise SSUnsupportedError("Orchestrator does not support clusters of size 2")
 
         if self.launcher == "local" and self.db_nodes > 1:
@@ -619,112 +649,127 @@
 
                 # create the exe_args list for launching multiple databases
                 # per node. also collect port range for dbnode
                 start_script_args = self._get_start_script_args(
                     db_node_name, port, cluster
                 )
 
-                exe_args = " ".join(start_script_args)
-
                 # if only launching 1 db per command, we don't need a list of exe args lists
                 run_settings = self._build_run_settings(
-                    sys.executable, exe_args, **kwargs
+                    sys.executable, [start_script_args], **kwargs
                 )
 
                 node = DBNode(
                     db_node_name,
                     self.path,
                     run_settings,
                     [port],
                     [db_node_name + ".out"],
                 )
                 self.entities.append(node)
 
             self.ports = [port]
 
-    def _initialize_entities_mpmd(self, **kwargs):
+    def _initialize_entities_mpmd(self, **kwargs: t.Any) -> None:
         port = kwargs.get("port", 6379)
         cluster = not bool(self.db_nodes < 3)
 
-        exe_args_mpmd = []
+        exe_args_mpmd: t.List[t.List[str]] = []
 
         for db_id in range(self.db_nodes):
             db_shard_name = "_".join((self.name, str(db_id)))
             # create the exe_args list for launching multiple databases
             # per node. also collect port range for dbnode
             start_script_args = self._get_start_script_args(
                 db_shard_name, port, cluster
             )
             exe_args = " ".join(start_script_args)
             exe_args_mpmd.append(sh_split(exe_args))
 
+        run_settings: t.Optional[RunSettings] = None
+        
         if self.launcher == "lsf":
             run_settings = self._build_run_settings_lsf(
                 sys.executable, exe_args_mpmd, **kwargs
             )
             output_files = [
                 "_".join((self.name, str(db_id))) + ".out"
                 for db_id in range(self.db_nodes)
             ]
         else:
             run_settings = self._build_run_settings(
                 sys.executable, exe_args_mpmd, **kwargs
             )
             output_files = [self.name + ".out"]
+            
+        if not run_settings:
+            raise ValueError(f"Could not build run settings for {self.launcher}")
+        
         node = DBNode(self.name, self.path, run_settings, [port], output_files)
         node._mpmd = True
         node._num_shards = self.db_nodes
         self.entities.append(node)
 
         self.ports = [port]
 
     @staticmethod
-    def _get_cluster_args(name, port):
+    def _get_cluster_args(name: str, port: int) -> t.List[str]:
         """Create the arguments necessary for cluster creation"""
         cluster_conf = "".join(("nodes-", name, "-", str(port), ".conf"))
         db_args = ["--cluster-enabled yes", "--cluster-config-file", cluster_conf]
         return db_args
 
-    def _get_start_script_args(self, name, port, cluster):
+    def _get_start_script_args(
+        self, name: str, port: int, cluster: bool
+    ) -> t.List[str]:
         start_script_args = [
             "-m",
             "smartsim._core.entrypoints.redis",  # entrypoint
-            f"+ifname={self._interface}",  # pass interface to start script
+            "+ifname=" + ",".join(self._interfaces),  # pass interface to start script
             "+command",  # command flag for argparser
             self._redis_exe,  # redis-server
-            self._redis_conf,  # redis6.conf file
+            self._redis_conf,  # redis.conf file
             self._rai_module,  # redisai.so
             "--port",  # redis port
             str(port),  # port number
         ]
         if cluster:
             start_script_args += self._get_cluster_args(name, port)
 
         return start_script_args
+    
+    @property
+    def dbnodes(self) -> t.List[DBNode]:
+        """
+        Helper property to cast self.entities to DBNode type for type correctness
+        """
+        dbnodes = [node for node in self.entities if isinstance(node, DBNode)]
+        return dbnodes
 
-    def _get_db_hosts(self):
+    def _get_db_hosts(self) -> t.List[str]:
         hosts = []
-        for dbnode in self.entities:
-            if not dbnode._mpmd:
-                hosts.append(dbnode.host)
+        for db in self.dbnodes:
+            if not db._mpmd:
+                hosts.append(db.host)
             else:
-                hosts.extend(dbnode.hosts)
+                hosts.extend(db.hosts)
         return hosts
 
-    def _check_network_interface(self):
+    def _check_network_interface(self) -> None:
         net_if_addrs = psutil.net_if_addrs()
-        if self._interface not in net_if_addrs and self._interface != "lo":
-            available = list(net_if_addrs.keys())
-            logger.warning(
-                f"{self._interface} is not a valid network interface on this node. \n"
-                "This could be because the head node doesn't have the same networks, if so, ignore this."
-            )
-            logger.warning(f"Found network interfaces are: {available}")
+        for interface in self._interfaces:
+            if interface not in net_if_addrs and interface != "lo":
+                available = list(net_if_addrs.keys())
+                logger.warning(
+                    f"{interface} is not a valid network interface on this node. \n"
+                    "This could be because the head node doesn't have the same networks, if so, ignore this."
+                )
+                logger.warning(f"Found network interfaces are: {available}")
 
-    def _fill_reserved(self):
+    def _fill_reserved(self) -> None:
         """Fill the reserved batch and run arguments dictionaries"""
 
         mpi_like_settings = [
             MpirunSettings,
             MpiexecSettings,
             OrterunSettings,
             PalsMpiexecSettings,
@@ -842,299 +887,7 @@
             "J",
             "o",
             "e",
             "m",
             "n",
             "nnodes",
         ]
-
-
-#
-# Deprecated Orchestrator Classes
-#
-# Same functionality incorporated into the Orchestrator base class
-#
-
-
-class CobaltOrchestrator(Orchestrator):
-    def __init__(
-        self,
-        port=6379,
-        db_nodes=1,
-        batch=True,
-        hosts=None,
-        run_command="aprun",
-        interface="ipogif0",
-        account=None,
-        queue=None,
-        time=None,
-        single_cmd=True,
-        **kwargs,
-    ):
-        """Initialize an Orchestrator reference for Cobalt based systems
-
-        The orchestrator launches as a batch by default. If batch=False,
-        at launch, the orchestrator will look for an interactive
-        allocation to launch on.
-
-        The Cobalt orchestrator does not support multiple databases per node.
-
-        :param port: TCP/IP port, defaults to 6379
-        :type port: int
-        :param db_nodes: number of database shards, defaults to 1
-        :type db_nodes: int, optional
-        :param batch: Run as a batch workload, defaults to True
-        :type batch: bool, optional
-        :param hosts: specify hosts to launch on, defaults to None. Optional if not launching with OpenMPI
-        :type hosts: list[str]
-        :param run_command: specify launch binary. Options are ``mpirun`` and ``aprun``, defaults to ``aprun``.
-        :type run_command: str, optional
-        :param interface: network interface to use, defaults to "ipogif0"
-        :type interface: str, optional
-        :param account: account to run batch on
-        :type account: str, optional
-        :param queue: queue to launch batch in
-        :type queue: str, optional
-        :param time: walltime for batch 'HH:MM:SS' format
-        :type time: str, optional
-        """
-        simplefilter("once", DeprecationWarning)
-        msg = "CobaltOrchestrator(...) is deprecated and will be removed in a future release.\n"
-        msg += "Please update your code to use Orchestrator(launcher='cobalt', ...)."
-        warn(msg, DeprecationWarning, stacklevel=2)
-        super().__init__(
-            port,
-            interface,
-            db_nodes=db_nodes,
-            batch=batch,
-            run_command=run_command,
-            single_cmd=single_cmd,
-            launcher="cobalt",
-            hosts=hosts,
-            account=account,
-            queue=queue,
-            time=time,
-            **kwargs,
-        )
-
-
-class LSFOrchestrator(Orchestrator):
-    def __init__(
-        self,
-        port=6379,
-        db_nodes=1,
-        cpus_per_shard=4,
-        gpus_per_shard=0,
-        batch=True,
-        hosts=None,
-        project=None,
-        time=None,
-        interface="ib0",
-        single_cmd=True,
-        **kwargs,
-    ):
-
-        """Initialize an Orchestrator reference for LSF based systems
-
-        The orchestrator launches as a batch by default. If
-        batch=False, at launch, the orchestrator will look for an interactive
-        allocation to launch on.
-
-        The LSFOrchestrator port provided will be incremented if multiple
-        databases per host are launched (``db_per_host>1``).
-
-        Each database shard is assigned a resource set with cpus and gpus
-        allocated contiguously on the host:
-        it is the user's responsibility to check if
-        enough resources are available on each host.
-
-        A list of hosts to launch the database on can be specified
-        these addresses must correspond to
-        those of the first ``db_nodes//db_per_host`` compute nodes
-        in the allocation: for example, for 8 ``db_nodes`` and 2 ``db_per_host``
-        the ``host_list`` must contain the addresses of hosts 1, 2, 3, and 4.
-
-        ``LSFOrchestrator`` is launched with only one ``jsrun`` command
-        as launch binary, and an Explicit Resource File (ERF) which is
-        automatically generated. The orchestrator is always launched on the
-        first ``db_nodes//db_per_host`` compute nodes in the allocation.
-
-        :param port: TCP/IP port
-        :type port: int
-        :param db_nodes: number of database shards, defaults to 1
-        :type db_nodes: int, optional
-        :param cpus_per_shard: cpus to allocate per shard, defaults to 4
-        :type cpus_per_shard: int, optional
-        :param gpus_per_shard: gpus to allocate per shard, defaults to 0
-        :type gpus_per_shard: int, optional
-        :param batch: Run as a batch workload, defaults to True
-        :type batch: bool, optional
-        :param hosts: specify hosts to launch on
-        :type hosts: list[str], optional
-        :param project: project to run batch on
-        :type project: str, optional
-        :param time: walltime for batch 'HH:MM' format
-        :type time: str, optional
-        :param interface: network interface to use
-        :type interface: str
-        """
-        simplefilter("once", DeprecationWarning)
-        msg = "LSFOrchestrator(...) is deprecated and will be removed in a future release.\n"
-        msg += "Please update your code to use Orchestrator(launcher='lsf', ...)."
-        warn(msg, DeprecationWarning, stacklevel=2)
-        if single_cmd != True:
-            raise SSUnsupportedError(
-                "LSFOrchestrator can only be run with single_cmd=True (MPMD)."
-            )
-
-        super().__init__(
-            port,
-            interface,
-            db_nodes=db_nodes,
-            batch=batch,
-            run_command="jsrun",
-            launcher="lsf",
-            project=project,
-            hosts=hosts,
-            time=time,
-            cpus_per_shard=cpus_per_shard,
-            gpus_per_shard=gpus_per_shard,
-            **kwargs,
-        )
-
-
-class SlurmOrchestrator(Orchestrator):
-    def __init__(
-        self,
-        port=6379,
-        db_nodes=1,
-        batch=True,
-        hosts=None,
-        run_command="srun",
-        account=None,
-        time=None,
-        alloc=None,
-        db_per_host=1,
-        interface="ipogif0",
-        single_cmd=False,
-        **kwargs,
-    ):
-
-        """Initialize an Orchestrator reference for Slurm based systems
-
-        The orchestrator launches as a batch by default. The Slurm orchestrator
-        can also be given an allocation to run on. If no allocation is provided,
-        and batch=False, at launch, the orchestrator will look for an interactive
-        allocation to launch on.
-
-        The SlurmOrchestrator port provided will be incremented if multiple
-        databases per node are launched.
-
-        SlurmOrchestrator supports launching with both ``srun`` and ``mpirun``
-        as launch binaries. If mpirun is used, the hosts parameter should be
-        populated with length equal to that of the ``db_nodes`` argument.
-
-        :param port: TCP/IP port
-        :type port: int
-        :param db_nodes: number of database shards, defaults to 1
-        :type db_nodes: int, optional
-        :param batch: Run as a batch workload, defaults to True
-        :type batch: bool, optional
-        :param hosts: specify hosts to launch on
-        :type hosts: list[str]
-        :param run_command: specify launch binary. Options are "mpirun" and "srun", defaults to "srun"
-        :type run_command: str, optional
-        :param account: account to run batch on
-        :type account: str, optional
-        :param time: walltime for batch 'HH:MM:SS' format
-        :type time: str, optional
-        :param alloc: allocation to launch on, defaults to None
-        :type alloc: str, optional
-        :param db_per_host: number of database shards per system host (MPMD), defaults to 1
-        :type db_per_host: int, optional
-        :param single_cmd: run all shards with one (MPMD) command, defaults to True
-        :type single_cmd: bool
-        """
-        simplefilter("once", DeprecationWarning)
-        msg = "SlurmOrchestrator(...) is deprecated and will be removed in a future release.\n"
-        msg += "Please update your code to use Orchestrator(launcher='slurm', ...)."
-        warn(msg, DeprecationWarning, stacklevel=2)
-        super().__init__(
-            port,
-            interface,
-            db_nodes=db_nodes,
-            batch=batch,
-            run_command=run_command,
-            alloc=alloc,
-            db_per_host=db_per_host,
-            single_cmd=single_cmd,
-            launcher="slurm",
-            account=account,
-            hosts=hosts,
-            time=time,
-            **kwargs,
-        )
-
-
-class PBSOrchestrator(Orchestrator):
-    def __init__(
-        self,
-        port=6379,
-        db_nodes=1,
-        batch=True,
-        hosts=None,
-        run_command="aprun",
-        interface="ipogif0",
-        account=None,
-        time=None,
-        queue=None,
-        single_cmd=True,
-        **kwargs,
-    ):
-        """Initialize an Orchestrator reference for PBSPro based systems
-
-        The ``PBSOrchestrator`` launches as a batch by default. If batch=False,
-        at launch, the ``PBSOrchestrator`` will look for an interactive
-        allocation to launch on.
-
-        The PBS orchestrator does not support multiple databases per node.
-
-        If ``mpirun`` is specifed as the ``run_command``, then the ``hosts``
-        argument is required.
-
-        :param port: TCP/IP port
-        :type port: int
-        :param db_nodes: number of compute nodes to span accross, defaults to 1
-        :type db_nodes: int, optional
-        :param batch: run as a batch workload, defaults to True
-        :type batch: bool, optional
-        :param hosts: specify hosts to launch on, defaults to None
-        :type hosts: list[str]
-        :param run_command: specify launch binary. Options are ``mpirun`` and ``aprun``, defaults to "aprun"
-        :type run_command: str, optional
-        :param interface: network interface to use, defaults to "ipogif0"
-        :type interface: str, optional
-        :param account: account to run batch on
-        :type account: str, optional
-        :param time: walltime for batch 'HH:MM:SS' format
-        :type time: str, optional
-        :param queue: queue to launch batch in
-        :type queue: str, optional
-        """
-        simplefilter("once", DeprecationWarning)
-        msg = "PBSOrchestrator(...) is deprecated and will be removed in a future release.\n"
-        msg += "Please update your code to use Orchestrator(launcher='pbs', ...)."
-        warn(msg, DeprecationWarning, stacklevel=2)
-        super().__init__(
-            port,
-            interface,
-            db_nodes=db_nodes,
-            batch=batch,
-            run_command=run_command,
-            single_cmd=single_cmd,
-            launcher="pbs",
-            hosts=hosts,
-            account=account,
-            queue=queue,
-            time=time,
-            **kwargs,
-        )
```

### Comparing `smartsim-0.4.2/smartsim/entity/__init__.py` & `smartsim-0.5.0/smartsim/ml/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,13 +20,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .dbnode import DBNode
-from .dbobject import *
-from .ensemble import Ensemble
-from .entity import SmartSimEntity
-from .entityList import EntityList
-from .model import Model
+from .data import DataDownloader, DataInfo, TrainingDataUploader, form_name
```

### Comparing `smartsim-0.4.2/smartsim/entity/dbnode.py` & `smartsim-0.5.0/smartsim/entity/dbnode.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,66 +23,70 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import os.path as osp
 import time
+import typing as t
 
 from ..error import SmartSimError
 from ..log import get_logger
 from .entity import SmartSimEntity
+from ..settings.base import RunSettings
+
 
 logger = get_logger(__name__)
 
 
 class DBNode(SmartSimEntity):
     """DBNode objects are the entities that make up the orchestrator.
     Each database node can be launched in a cluster configuration
     and take launch multiple databases per node.
 
     To configure how each instance of the database operates, look
     into the smartsimdb.conf.
     """
 
-    def __init__(self, name, path, run_settings, ports, output_files):
+    def __init__(self, name: str, path: str, run_settings: RunSettings, ports: t.List[int], output_files: t.List[str]) -> None:
         """Initialize a database node within an orchestrator."""
         self.ports = ports
-        self._host = None
+        self._host: t.Optional[str] = None
         super().__init__(name, path, run_settings)
         self._mpmd = False
-        self._num_shards = None
-        self._hosts = None
+        self._num_shards: int = 0
+        self._hosts: t.Optional[t.List[str]] = None
+
         if not output_files:
             raise ValueError("output_files cannot be empty")
         if not isinstance(output_files, list) or not all(
             [isinstance(item, str) for item in output_files]
         ):
             raise ValueError("output_files must be of type list[str]")
         self._output_files = output_files
 
     @property
-    def host(self):
+    def host(self) -> str:
         if not self._host:
             self._host = self._parse_db_host()
         return self._host
 
     @property
-    def hosts(self):
+    def hosts(self) -> t.List[str]:
         if not self._hosts:
             self._hosts = self._parse_db_hosts()
         return self._hosts
 
-    def set_host(self, host):
+    def set_host(self, host: str) -> None:
         self._host = str(host)
 
-    def set_hosts(self, hosts):
+    def set_hosts(self, hosts: t.List[str]) -> None:
         self._hosts = [str(host) for host in hosts]
 
-    def remove_stale_dbnode_files(self):
+    def remove_stale_dbnode_files(self) -> None:
         """This function removes the .conf, .err, and .out files that
         have the same names used by this dbnode that may have been
         created from a previous experiment execution.
         """
 
         for port in self.ports:
             if not self._mpmd:
@@ -107,53 +111,53 @@
                 for shard_id in range(self._num_shards):
                     file_name = osp.join(
                         self.path, self.name + "_" + str(shard_id) + file_ending
                     )
                     if osp.exists(file_name):
                         os.remove(file_name)
 
-    def _get_cluster_conf_filename(self, port):
+    def _get_cluster_conf_filename(self, port: int) -> str:
         """Returns the .conf file name for the given port number
 
         :param port: port number
         :type port: int
         :return: the dbnode configuration file name
         :rtype: str
         """
         return "".join(("nodes-", self.name, "-", str(port), ".conf"))
 
-    def _get_cluster_conf_filenames(self, port):  # cov-lsf
+    def _get_cluster_conf_filenames(self, port: int) -> t.List[str]:  # cov-lsf
         """Returns the .conf file name for the given port number
 
         This function should bu used if and only if ``_mpmd==True``
 
         :param port: port number
         :type port: int
         :return: the dbnode configuration file name
         :rtype: str
         """
         return [
             "".join(("nodes-", self.name + f"_{shard_id}", "-", str(port), ".conf"))
             for shard_id in range(self._num_shards)
         ]
 
-    def _parse_ips(self, filepath, num_ips=None):
+    def _parse_ips(self, filepath: str, num_ips: t.Optional[int] = None) -> t.List[str]:
         ips = []
         with open(filepath, "r") as f:
             lines = f.readlines()
             for line in lines:
                 content = line.split()
                 if "IPADDRESS:" in content:
                     ips.append(content[-1])
                     if num_ips and len(ips) == num_ips:
                         break
 
         return ips
 
-    def _parse_db_host(self, filepath=None):
+    def _parse_db_host(self, filepath: t.Optional[str] = None) -> str:
         """Parse the database host/IP from the output file
 
         If no file is passed as argument, then the first
         file in self._output_files is used.
 
         :param filepath: Path to file to parse
         :type filepath: str, optional
@@ -182,33 +186,33 @@
 
         if not ip:
             logger.error(f"IP address lookup strategy failed for file {filepath}.")
             raise SmartSimError("Failed to obtain database hostname")
 
         return ip
 
-    def _parse_db_hosts(self):
+    def _parse_db_hosts(self) -> t.List[str]:
         """Parse the database hosts/IPs from the output files
 
         this uses the RedisIP module that is built as a dependency
         The IP address is preferred, but if hostname is only present
         then a lookup to /etc/hosts is done through the socket library.
         This function must be called only if ``_mpmd==True``.
 
         :raises SmartSimError: if host/ip could not be found
         :return: ip addresses | hostnames
         :rtype: list[str]
         """
-        ips = []
+        ips: t.List[str] = []
 
         # Find out if all shards' output streams are piped to separate files
         if len(self._output_files) > 1:
             for output_file in self._output_files:
                 filepath = osp.join(self.path, output_file)
-                ip = self._parse_db_host(filepath)
+                _ = self._parse_db_host(filepath)
         else:
             filepath = osp.join(self.path, self._output_files[0])
             trials = 10
             ips = []
             while len(ips) < self._num_shards and trials > 0:
                 ips = []
                 try:
```

### Comparing `smartsim-0.4.2/smartsim/entity/dbobject.py` & `smartsim-0.5.0/smartsim/entity/dbobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,80 +20,89 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 
 from pathlib import Path
+from .._core.utils import init_default
 
-from .._core.utils.helpers import init_default
 
 __all__ = ["DBObject", "DBModel", "DBScript"]
 
 
 class DBObject:
     """Base class for ML objects residing on DB. Should not
     be instantiated.
     """
 
-    def __init__(self, name, func, file_path, device, devices_per_node):
+    def __init__(
+        self,
+        name: str,
+        func: t.Optional[str],
+        file_path: t.Optional[str],
+        device: str,
+        devices_per_node: int,
+    ) -> None:
         self.name = name
         self.func = func
+        self.file: t.Optional[Path] = None  # Need to have this explicitly to check on it
         if file_path:
             self.file = self._check_filepath(file_path)
-        else:
-            # Need to have this explicitly to check on it
-            self.file = None
         self.device = self._check_device(device)
         self.devices_per_node = devices_per_node
 
     @property
-    def is_file(self):
+    def is_file(self) -> bool:
         if self.func:
             return False
         return True
 
     @staticmethod
-    def _check_tensor_args(inputs, outputs):
+    def _check_tensor_args(
+        inputs: t.Union[str, t.Optional[t.List[str]]], outputs: t.Union[str, t.Optional[t.List[str]]]
+    ) -> t.Tuple[t.List[str], t.List[str]]:
         inputs = init_default([], inputs, (list, str))
         outputs = init_default([], outputs, (list, str))
+
         if isinstance(inputs, str):
             inputs = [inputs]
         if isinstance(outputs, str):
             outputs = [outputs]
-        return inputs, outputs
+        return inputs or [], outputs or []
 
     @staticmethod
-    def _check_backend(backend):
+    def _check_backend(backend: str) -> str:
         backend = backend.upper()
         all_backends = ["TF", "TORCH", "ONNX"]
         if backend in all_backends:
             return backend
         else:
             raise ValueError(
                 f"Backend type {backend} unsupported. Options are {all_backends}"
             )
 
     @staticmethod
-    def _check_filepath(file):
+    def _check_filepath(file: str) -> Path:
         file_path = Path(file).resolve()
         if not file_path.is_file():
             raise FileNotFoundError(file_path)
         return file_path
 
     @staticmethod
-    def _check_device(device):
+    def _check_device(device: str) -> str:
         device = device.upper()
         if not device.startswith("CPU") and not device.startswith("GPU"):
             raise ValueError("Device argument must start with either CPU or GPU")
         return device
 
-    def _enumerate_devices(self):
+    def _enumerate_devices(self) -> t.List[str]:
         """Enumerate devices for a DBObject
 
         :param dbobject: DBObject to enumerate
         :type dbobject: DBObject
         :return: list of device names
         :rtype: list[str]
         """
@@ -109,15 +118,20 @@
             devices = [self.device]
 
         return devices
 
 
 class DBScript(DBObject):
     def __init__(
-        self, name, script=None, script_path=None, device="CPU", devices_per_node=1
+        self,
+        name: str,
+        script: t.Optional[str] = None,
+        script_path: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
     ):
         """TorchScript code represenation
 
         Device selection is either "GPU" or "CPU". If many devices are
         present, a number can be passed for specification e.g. "GPU:1".
 
         Setting ``devices_per_node=N``, with N greater than one will result
@@ -138,18 +152,18 @@
         :type devices_per_node: int
         """
         super().__init__(name, script, script_path, device, devices_per_node)
         if not script and not script_path:
             raise ValueError("Either script or script_path must be provided")
 
     @property
-    def script(self):
+    def script(self) -> t.Optional[str]:
         return self.func
 
-    def __str__(self):
+    def __str__(self) -> str:
         desc_str = "Name: " + self.name + "\n"
         if self.func:
             desc_str += "Func: " + self.func + "\n"
         if self.file:
             desc_str += "File path: " + str(self.file) + "\n"
         devices_str = self.device + (
             "s per node\n" if self.devices_per_node > 1 else " per node\n"
@@ -157,27 +171,27 @@
         desc_str += "Devices: " + str(self.devices_per_node) + " " + devices_str
         return desc_str
 
 
 class DBModel(DBObject):
     def __init__(
         self,
-        name,
-        backend,
-        model=None,
-        model_file=None,
-        device="CPU",
-        devices_per_node=1,
-        batch_size=0,
-        min_batch_size=0,
-        min_batch_timeout=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        backend: str,
+        model: t.Optional[str] = None,
+        model_file: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        min_batch_timeout: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.List[str]] = None,
+        outputs: t.Optional[t.List[str]] = None,
+    ) -> None:
         """A TF, TF-lite, PT, or ONNX model to load into the DB at runtime
 
         One of either model (in memory representation) or model_path (file)
         must be provided
 
         :param name: key to store model under
         :type name: str
@@ -211,18 +225,18 @@
         self.batch_size = batch_size
         self.min_batch_size = min_batch_size
         self.min_batch_timeout = min_batch_timeout
         self.tag = tag
         self.inputs, self.outputs = self._check_tensor_args(inputs, outputs)
 
     @property
-    def model(self):
+    def model(self) -> t.Union[str, None]:
         return self.func
 
-    def __str__(self):
+    def __str__(self) -> str:
         desc_str = "Name: " + self.name + "\n"
         if self.model:
             desc_str += "Model stored in memory\n"
         if self.file:
             desc_str += "File path: " + str(self.file) + "\n"
         devices_str = self.device + (
             "s per node\n" if self.devices_per_node > 1 else " per node\n"
```

### Comparing `smartsim-0.4.2/smartsim/entity/ensemble.py` & `smartsim-0.5.0/smartsim/entity/ensemble.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from copy import deepcopy
 from os import getcwd
 
 from .._core.utils.helpers import init_default
 from ..error import (
     EntityExistsError,
     SmartSimError,
@@ -35,75 +37,82 @@
     UserStrategyError,
 )
 from ..log import get_logger
 from ..settings.base import BatchSettings, RunSettings
 from .dbobject import DBModel, DBScript
 from .entityList import EntityList
 from .model import Model
+from .entity import SmartSimEntity
 from .strategies import create_all_permutations, random_permutations, step_values
 
 logger = get_logger(__name__)
 
+StrategyFunction = t.Callable[[t.List[str], t.List[t.List[str]], int], t.List[t.Dict[str, str]]]
 
 class Ensemble(EntityList):
     """``Ensemble`` is a group of ``Model`` instances that can
     be treated as a reference to a single instance.
     """
 
     def __init__(
         self,
-        name,
-        params,
-        params_as_args=None,
-        batch_settings=None,
-        run_settings=None,
-        perm_strat="all_perm",
-        **kwargs,
-    ):
+        name: str,
+        params: t.Dict[str, t.Any],
+        params_as_args: t.Optional[t.List[str]] = None,
+        batch_settings: t.Optional[BatchSettings] = None,
+        run_settings: t.Optional[RunSettings] = None,
+        perm_strat: str = "all_perm",
+        **kwargs: t.Any,
+    ) -> None:
         """Initialize an Ensemble of Model instances.
 
         The kwargs argument can be used to pass custom input
         parameters to the permutation strategy.
 
         :param name: name of the ensemble
         :type name: str
         :param params: parameters to expand into ``Model`` members
         :type params: dict[str, Any]
         :param params_as_args: list of params which should be used as command line arguments
                                to the ``Model`` member executables and not written to generator
                                files
-        :type arg_params: list[str]
+        :type params_as_args: list[str]
         :param batch_settings: describes settings for ``Ensemble`` as batch workload
         :type batch_settings: BatchSettings, optional
         :param run_settings: describes how each ``Model`` should be executed
         :type run_settings: RunSettings, optional
         :param replicas: number of ``Model`` replicas to create - a keyword argument of kwargs
         :type replicas: int, optional
         :param perm_strategy: strategy for expanding ``params`` into
                              ``Model`` instances from params argument
-                             options are "all_perm", "stepped", "random"
+                             options are "all_perm", "step", "random"
                              or a callable function. Defaults to "all_perm".
         :type perm_strategy: str
         :return: ``Ensemble`` instance
         :rtype: ``Ensemble``
         """
         self.params = init_default({}, params, dict)
         self.params_as_args = init_default({}, params_as_args, (list, str))
         self._key_prefixing_enabled = True
         self.batch_settings = init_default({}, batch_settings, BatchSettings)
         self.run_settings = init_default({}, run_settings, RunSettings)
-        self._db_models = []
-        self._db_scripts = []
+        
+        self._db_models: t.List[DBModel] = []
+        self._db_scripts: t.List[DBScript] = []
         super().__init__(name, getcwd(), perm_strat=perm_strat, **kwargs)
 
     @property
-    def models(self):
-        return self.entities
+    def models(self) -> t.List[Model]:
+        """
+        Helper property to cast self.entities to Model type for type correctness
+        """
+        model_entities = [node for node in self.entities if isinstance(node, Model)]
+        return model_entities
 
-    def _initialize_entities(self, **kwargs):
+    def _initialize_entities(self, **kwargs: t.Any) -> None:
         """Initialize all the models within the ensemble based
         on the parameters passed to the ensemble and the permutation
         strategy given at init.
 
         :raises UserStrategyError: if user generation strategy fails
         """
         strategy = self._set_strategy(kwargs.pop("perm_strat"))
@@ -112,15 +121,16 @@
         # if a ensemble has parameters and run settings, create
         # the ensemble and assign run_settings to each member
         if self.params:
             if self.run_settings:
                 param_names, params = self._read_model_parameters()
 
                 # Compute all combinations of model parameters and arguments
-                all_model_params = strategy(param_names, params, **kwargs)
+                n_models = kwargs.get("n_models", 0)
+                all_model_params = strategy(param_names, params, n_models)
                 if not isinstance(all_model_params, list):
                     raise UserStrategyError(strategy)
 
                 for i, param_set in enumerate(all_model_params):
                     if not isinstance(param_set, dict):
                         raise UserStrategyError(strategy)
                     run_settings = deepcopy(self.run_settings)
@@ -168,15 +178,15 @@
             elif not self.batch_settings:
                 raise SmartSimError(
                     "Ensemble must be provided batch settings or run settings"
                 )
             else:
                 logger.info("Empty ensemble created for batch launch")
 
-    def add_model(self, model):
+    def add_model(self, model: Model) -> None:
         """Add a model to this ensemble
 
         :param model: model instance to be added
         :type model: Model
         :raises TypeError: if model is not an instance of ``Model``
         :raises EntityExistsError: if model already exists in this ensemble
         """
@@ -193,45 +203,50 @@
         if self._db_models:
             self._extend_entity_db_models(model, self._db_models)
         if self._db_scripts:
             self._extend_entity_db_scripts(model, self._db_scripts)
 
         self.entities.append(model)
 
-    def register_incoming_entity(self, incoming_entity):
+    def register_incoming_entity(self, incoming_entity: SmartSimEntity) -> None:
         """Register future communication between entities.
 
         Registers the named data sources that this entity
         has access to by storing the key_prefix associated
         with that entity
 
         Only python clients can have multiple incoming connections
 
         :param incoming_entity: The entity that data will be received from
         :type incoming_entity: SmartSimEntity
         """
-        for model in self.entities:
+        for model in self.models:
             model.register_incoming_entity(incoming_entity)
 
-    def enable_key_prefixing(self):
+    def enable_key_prefixing(self) -> None:
         """If called, all models within this ensemble will prefix their keys with its
         own model name.
         """
-        for model in self.entities:
+        for model in self.models:
             model.enable_key_prefixing()
 
-    def query_key_prefixing(self):
+    def query_key_prefixing(self) -> bool:
         """Inquire as to whether each model within the ensemble will prefix its keys
 
         :returns: True if all models have key prefixing enabled, False otherwise
         :rtype: bool
         """
-        return all([model.query_key_prefixing() for model in self.entities])
+        return all([model.query_key_prefixing() for model in self.models])
 
-    def attach_generator_files(self, to_copy=None, to_symlink=None, to_configure=None):
+    def attach_generator_files(
+        self,
+        to_copy: t.Optional[t.List[str]] = None,
+        to_symlink: t.Optional[t.List[str]] = None,
+        to_configure: t.Optional[t.List[str]] = None,
+    ) -> None:
         """Attach files to each model within the ensemble for generation
 
         Attach files needed for the entity that, upon generation,
         will be located in the path of the entity.
 
         During generation, files "to_copy" are copied into
         the path of the entity, and files "to_symlink" are
@@ -247,20 +262,22 @@
         :param to_copy: files to copy, defaults to []
         :type to_copy: list, optional
         :param to_symlink: files to symlink, defaults to []
         :type to_symlink: list, optional
         :param to_configure: input files with tagged parameters, defaults to []
         :type to_configure: list, optional
         """
-        for model in self.entities:
+        for model in self.models:
             model.attach_generator_files(
                 to_copy=to_copy, to_symlink=to_symlink, to_configure=to_configure
             )
 
-    def _set_strategy(self, strategy):
+    def _set_strategy(
+        self, strategy: str
+    ) -> StrategyFunction:
         """Set the permutation strategy for generating models within
         the ensemble
 
         :param strategy: name of the strategy or callable function
         :type strategy: str
         :raises SSUnsupportedError: if str name is not supported
         :return: strategy function
@@ -274,58 +291,59 @@
             return random_permutations
         if callable(strategy):
             return strategy
         raise SSUnsupportedError(
             f"Permutation strategy given is not supported: {strategy}"
         )
 
-    def _read_model_parameters(self):
+    def _read_model_parameters(self) -> t.Tuple[t.List[str], t.List[t.List[str]]]:
         """Take in the parameters given to the ensemble and prepare to
         create models for the ensemble
 
         :raises TypeError: if params are of the wrong type
         :return: param names and values for permutation strategy
         :rtype: tuple[list, list]
         """
 
         if not isinstance(self.params, dict):
             raise TypeError(
                 "Ensemble initialization argument 'params' must be of type dict"
             )
 
-        param_names = []
-        parameters = []
+        param_names: t.List[str] = []
+        parameters: t.List[t.List[str]] = []
         for name, val in self.params.items():
             param_names.append(name)
 
             if isinstance(val, list):
+                val = [str(v) for v in val]
                 parameters.append(val)
             elif isinstance(val, (int, str)):
-                parameters.append([val])
+                parameters.append([str(val)])
             else:
                 raise TypeError(
                     "Incorrect type for ensemble parameters\n"
                     + "Must be list, int, or string."
                 )
         return param_names, parameters
 
     def add_ml_model(
         self,
-        name,
-        backend,
-        model=None,
-        model_path=None,
-        device="CPU",
-        devices_per_node=1,
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        backend: str,
+        model: t.Optional[str] = None,
+        model_path: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.List[str]] = None,
+        outputs: t.Optional[t.List[str]] = None,
+    ) -> None:
         """A TF, TF-lite, PT, or ONNX model to load into the DB at runtime
 
         Each ML Model added will be loaded into an
         orchestrator (converged or not) prior to the execution
         of every entity belonging to this ensemble
 
         One of either model (in memory representation) or model_path (file)
@@ -362,20 +380,25 @@
             batch_size=batch_size,
             min_batch_size=min_batch_size,
             tag=tag,
             inputs=inputs,
             outputs=outputs,
         )
         self._db_models.append(db_model)
-        for entity in self:
+        for entity in self.models:
             self._extend_entity_db_models(entity, [db_model])
 
     def add_script(
-        self, name, script=None, script_path=None, device="CPU", devices_per_node=1
-    ):
+        self,
+        name: str,
+        script: t.Optional[str] = None,
+        script_path: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+    ) -> None:
         """TorchScript to launch with every entity belonging to this ensemble
 
         Each script added to the model will be loaded into an
         orchestrator (converged or not) prior to the execution
         of every entity belonging to this ensemble
 
         Device selection is either "GPU" or "CPU". If many devices are
@@ -402,18 +425,24 @@
             name=name,
             script=script,
             script_path=script_path,
             device=device,
             devices_per_node=devices_per_node,
         )
         self._db_scripts.append(db_script)
-        for entity in self:
+        for entity in self.models:
             self._extend_entity_db_scripts(entity, [db_script])
 
-    def add_function(self, name, function=None, device="CPU", devices_per_node=1):
+    def add_function(
+        self,
+        name: str,
+        function: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+    ) -> None:
         """TorchScript function to launch with every entity belonging to this ensemble
 
         Each script function to the model will be loaded into a
         non-converged orchestrator prior to the execution
         of every entity belonging to this ensemble.
 
         For converged orchestrators, the :meth:`add_script` method should be used.
@@ -422,34 +451,36 @@
         present, a number can be passed for specification e.g. "GPU:1".
 
         Setting ``devices_per_node=N``, with N greater than one will result
         in the model being stored in the first N devices of type ``device``.
 
         :param name: key to store function under
         :type name: str
-        :param script: TorchScript code
-        :type script: str, optional
-        :param script_path: path to TorchScript code
-        :type script_path: str, optional
+        :param function: TorchScript code
+        :type function: str, optional
         :param device: device for script execution, defaults to "CPU"
         :type device: str, optional
         :param devices_per_node: number of devices on each host
         :type devices_per_node: int
         """
         db_script = DBScript(
             name=name, script=function, device=device, devices_per_node=devices_per_node
         )
         self._db_scripts.append(db_script)
-        for entity in self:
+        for entity in self.models:
             self._extend_entity_db_scripts(entity, [db_script])
 
-    def _extend_entity_db_models(self, model, db_models):
+    def _extend_entity_db_models(
+        self, model: Model, db_models: t.List[DBModel]
+    ) -> None:
         entity_db_models = [db_model.name for db_model in model._db_models]
         for db_model in db_models:
             if not db_model.name in entity_db_models:
                 model._append_db_model(db_model)
 
-    def _extend_entity_db_scripts(self, model, db_scripts):
+    def _extend_entity_db_scripts(
+        self, model: Model, db_scripts: t.List[DBScript]
+    ) -> None:
         entity_db_scripts = [db_script.name for db_script in model._db_scripts]
         for db_script in db_scripts:
             if not db_script.name in entity_db_scripts:
                 model._append_db_script(db_script)
```

### Comparing `smartsim-0.4.2/smartsim/entity/entity.py` & `smartsim-0.5.0/smartsim/entity/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
+import smartsim.settings.base
 
 class SmartSimEntity:
-    def __init__(self, name, path, run_settings):
+    def __init__(self, name: str, path: str, run_settings: smartsim.settings.base.RunSettings) -> None:
         """Initialize a SmartSim entity.
 
         Each entity must have a name, path, and
         run_settings. All entities within SmartSim
         share these attributes.
 
         :param name: Name of the entity
@@ -42,18 +42,18 @@
         :type run_settings: dict
         """
         self.name = name
         self.run_settings = run_settings
         self.path = path
 
     @property
-    def type(self):
+    def type(self) -> str:
         """Return the name of the class"""
         return type(self).__name__
 
-    def set_path(self, path):
+    def set_path(self, path: str) -> None:
         if not isinstance(path, str):
             raise TypeError("path argument must be a string")
         self.path = path
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.name
```

### Comparing `smartsim-0.4.2/smartsim/entity/entityList.py` & `smartsim-0.5.0/smartsim/entity/entityList.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,52 +20,61 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
+if t.TYPE_CHECKING:
+    import smartsim
+
 
 class EntityList:
     """Abstract class for containers for SmartSimEntities"""
 
-    def __init__(self, name, path, **kwargs):
-        self.name = name
-        self.path = path
-        self.entities = []
+    def __init__(self, name: str, path: str, **kwargs: t.Any) -> None:
+        self.name: str = name
+        self.path: str = path
+        self.entities: t.List["smartsim.entity.SmartSimEntity"] = []
         self._initialize_entities(**kwargs)
 
-    def _initialize_entities(self, **kwargs):
+    def _initialize_entities(self, **kwargs: t.Any) -> None:
         """Initialize the SmartSimEntity objects in the container"""
         raise NotImplementedError
 
     @property
-    def batch(self):
+    def batch(self) -> bool:
         try:
+            if not hasattr(self, "batch_settings"):
+                return False
+
             if self.batch_settings:
                 return True
             return False
         # local orchestrator cannot launch with batches
         except AttributeError:
             return False
 
     @property
-    def type(self):
+    def type(self) -> str:
         """Return the name of the class"""
         return type(self).__name__
 
-    def set_path(self, new_path):
+    def set_path(self, new_path: str) -> None:
         self.path = new_path
         for entity in self.entities:
             entity.path = new_path
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> t.Optional["smartsim.entity.SmartSimEntity"]:
         for entity in self.entities:
             if entity.name == name:
                 return entity
+        return None
 
-    def __iter__(self):
+    def __iter__(self) -> t.Iterator["smartsim.entity.SmartSimEntity"]:
         for entity in self.entities:
             yield entity
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.entities)
```

### Comparing `smartsim-0.4.2/smartsim/entity/files.py` & `smartsim-0.5.0/smartsim/entity/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import os
+import typing as t
+
 from os import path
 
 
 class EntityFiles:
     """EntityFiles are the files a user wishes to have available to
     models and nodes within SmartSim. Each entity has a method
     `entity.attach_generator_files()` that creates one of these
@@ -43,33 +44,38 @@
     editing them for tags.
 
     Lastly, symlink can be used for big datasets or input
     files that a user just wants to have present in the directory
     without necessary having to copy the entire file.
     """
 
-    def __init__(self, tagged, copy, symlink):
+    def __init__(
+        self, 
+        tagged: t.Optional[t.List[str]] = None, 
+        copy: t.Optional[t.List[str]] = None, 
+        symlink: t.Optional[t.List[str]] = None,
+    ) -> None:
         """Initialize an EntityFiles instance
 
         :param tagged: tagged files for model configuration
         :type tagged: list of str
         :param copy: files or directories to copy into model
                      or node directories
         :type copy: list of str
         :param symlink: files to symlink into model or node
                         directories
         :type symlink: list of str
         """
-        self.tagged = tagged
-        self.copy = copy
-        self.link = symlink
+        self.tagged = tagged or []
+        self.copy = copy or []
+        self.link = symlink or []
         self.tagged_hierarchy = None
         self._check_files()
 
-    def _check_files(self):
+    def _check_files(self) -> None:
         """Ensure the files provided by the user are of the correct
            type and actually exist somewhere on the filesystem.
 
         :raises SSConfigError: If a user provides a directory within
                                the tagged files.
         """
 
@@ -83,15 +89,15 @@
         )
 
         for i in range(len(self.copy)):
             self.copy[i] = self._check_path(self.copy[i])
         for i in range(len(self.link)):
             self.link[i] = self._check_path(self.link[i])
 
-    def _type_check_files(self, file_list, file_type):
+    def _type_check_files(self, file_list: t.Union[t.List[str], None], file_type: str) -> t.List[str]:
         """Check the type of the files provided by the user.
 
         :param file_list: either tagged, copy, or symlink files
         :type file_list: list of str
         :param file_type: name of the file type e.g. "tagged"
         :type file_type: str
         :raises TypeError: if incorrect type is provided by user
@@ -103,20 +109,20 @@
                 if isinstance(file_list, str):
                     file_list = [file_list]
                 else:
                     raise TypeError(
                         f"{file_type} files given were not of type list or str"
                     )
             else:
-                if not all(isinstance(f, str) for f in file_list):
+                if not all([isinstance(f, str) for f in file_list]):
                     raise TypeError(f"Not all {file_type} files were of type str")
-        return file_list
+        return file_list or []
 
     @staticmethod
-    def _check_path(file_path):
+    def _check_path(file_path: str) -> str:
         """Given a user provided path-like str, find the actual path to
            the directory or file and create a full path.
 
         :param file_path: path to a specific file or directory
         :type file_path: str
         :raises FileNotFoundError: if file or directory does not exist
         :return: full path to file or directory
@@ -146,15 +152,15 @@
     that needs to generated
 
     By performing a depth first search over the entire
     hierarchy starting at the root directory structure, the
     tagged file directory structure can be replicated
     """
 
-    def __init__(self, parent=None, subdir_name=""):
+    def __init__(self, parent: t.Optional[t.Any] = None, subdir_name: str = "") -> None:
         """Initialize a TaggedFilesHierarchy
 
         :param parent: The parent hierarchy of the new hierarchy,
                        must be None if creating a root hierarchy,
                        must be provided if creating a subhierachy
         :type parent: TaggedFilesHierarchy | None, optional
         :param subdir_name: Name of subdirectory representd by the new hierarchy,
@@ -180,26 +186,28 @@
                 "Child TaggedFilesHierarchies subdirectory names must not contain"
                 + " path seperators or be reserved dirs '.' or '..'"
             )
 
         if parent:
             parent.dirs.add(self)
 
-        self._base = path.join(parent.base, subdir_name) if parent else ""
-        self.parent = parent
-        self.files = set()
-        self.dirs = set()
+        self._base: str = path.join(parent.base, subdir_name) if parent else ""
+        self.parent: t.Any = parent
+        self.files: t.Set[str] = set()
+        self.dirs: t.Set[TaggedFilesHierarchy] = set()
 
     @property
-    def base(self):
+    def base(self) -> str:
         """Property to ensure that self.base is read-only"""
         return self._base
 
     @classmethod
-    def from_list_paths(cls, path_list, dir_contents_to_base=False):
+    def from_list_paths(
+        cls, path_list: t.List[str], dir_contents_to_base: bool = False
+    ) -> t.Any:
         """Given a list of absolute paths to files and dirs, create and return
         a TaggedFilesHierarchy instance representing the file hierarchy of
         tagged files. All files in the path list will be placed in the base of
         the file hierarchy.
 
         :param path_list: list of absolute paths to tagged files or dirs
                           containing tagged files
@@ -221,36 +229,36 @@
                     new_paths += [os.path.join(path, file) for file in os.listdir(path)]
                 else:
                     new_paths.append(path)
             path_list = new_paths
         tagged_file_hierarchy._add_paths(path_list)
         return tagged_file_hierarchy
 
-    def _add_file(self, file):
+    def _add_file(self, file: str) -> None:
         """Add a file to the current level in the file hierarchy
 
         :param file: absoute path to a file to add to the hierarchy
         :type file: str
         """
         self.files.add(file)
 
-    def _add_dir(self, dir):
+    def _add_dir(self, dir: str) -> None:
         """Add a dir contianing tagged files by creating a new sub level in the
         tagged file hierarchy. All paths within the directroy are added to the
         the new level sub level tagged file hierarchy
 
         :param dir: absoute path to a dir to add to the hierarchy
         :type dir: str
         """
         tagged_file_hierarchy = TaggedFilesHierarchy(self, path.basename(dir))
         tagged_file_hierarchy._add_paths(
             [path.join(dir, file) for file in os.listdir(dir)]
         )
 
-    def _add_paths(self, paths):
+    def _add_paths(self, paths: t.List[str]) -> None:
         """Takes a list of paths and iterates over it, determining if each
         path is to a file or a dir and then appropriatly adding it to the
         TaggedFilesHierarchy.
 
         :param paths: list of paths to files or dirs to add to the hierarchy
         :type paths: list[str]
         :raises ValueError: if link to dir is found
```

### Comparing `smartsim-0.4.2/smartsim/entity/model.py` & `smartsim-0.5.0/smartsim/entity/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,27 +20,40 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
 
+import collections.abc
+import sys
+import typing as t
 import warnings
 
 from .._core.utils.helpers import cat_arg_and_value, init_default
 from ..error import EntityExistsError, SSUnsupportedError
 from .dbobject import DBModel, DBScript
 from .entity import SmartSimEntity
 from .files import EntityFiles
+from ..settings.base import BatchSettings, RunSettings
+from ..log import get_logger
 
+logger = get_logger(__name__)
 
 class Model(SmartSimEntity):
     def __init__(
-        self, name, params, path, run_settings, params_as_args=None, batch_settings=None
+        self,
+        name: str,
+        params: t.Dict[str, str],
+        path: str,
+        run_settings: RunSettings,
+        params_as_args: t.Optional[t.List[str]] = None,
+        batch_settings: t.Optional[BatchSettings] = None,
     ):
         """Initialize a ``Model``
 
         :param name: name of the model
         :type name: str
         :param params: model parameters for writing into configuration files or
                        to be passed as command line arguments to executable.
@@ -56,27 +69,27 @@
         :param batch_settings: Launcher settings for running the individual
                                model as a batch job, defaults to None
         :type batch_settings: BatchSettings | None
         """
         super().__init__(name, path, run_settings)
         self.params = params
         self.params_as_args = params_as_args
-        self.incoming_entities = []
+        self.incoming_entities: t.List[SmartSimEntity] = []
         self._key_prefixing_enabled = False
         self.batch_settings = batch_settings
-        self._db_models = []
-        self._db_scripts = []
-        self.files = None
+        self._db_models: t.List[DBModel] = []
+        self._db_scripts: t.List[DBScript] = []
+        self.files: t.Optional[EntityFiles] = None
 
     @property
-    def colocated(self):
+    def colocated(self) -> bool:
         """Return True if this Model will run with a colocated Orchestrator"""
         return bool(self.run_settings.colocated_db_settings)
 
-    def register_incoming_entity(self, incoming_entity):
+    def register_incoming_entity(self, incoming_entity: SmartSimEntity) -> None:
         """Register future communication between entities.
 
         Registers the named data sources that this entity
         has access to by storing the key_prefix associated
         with that entity
 
         :param incoming_entity: The entity that data will be received from
@@ -89,31 +102,38 @@
             raise EntityExistsError(
                 f"'{incoming_entity.name}' has already "
                 + "been registered as an incoming entity"
             )
 
         self.incoming_entities.append(incoming_entity)
 
-    def enable_key_prefixing(self):
+    def enable_key_prefixing(self) -> None:
         """If called, the entity will prefix its keys with its own model name"""
         self._key_prefixing_enabled = True
 
-    def disable_key_prefixing(self):
+    def disable_key_prefixing(self) -> None:
         """If called, the entity will not prefix its keys with its own model name"""
         self._key_prefixing_enabled = False
 
-    def query_key_prefixing(self):
+    def query_key_prefixing(self) -> bool:
         """Inquire as to whether this entity will prefix its keys with its name"""
         return self._key_prefixing_enabled
 
-    def attach_generator_files(self, to_copy=None, to_symlink=None, to_configure=None):
+    def attach_generator_files(
+        self,
+        to_copy: t.Optional[t.List[str]] = None,
+        to_symlink: t.Optional[t.List[str]] = None,
+        to_configure: t.Optional[t.List[str]] = None,
+    ) -> None:
         """Attach files to an entity for generation
 
         Attach files needed for the entity that, upon generation,
-        will be located in the path of the entity.
+        will be located in the path of the entity.  Invoking this method
+        after files have already been attached will overwrite
+        the previous list of entity files.
 
         During generation, files "to_copy" are copied into
         the path of the entity, and files "to_symlink" are
         symlinked into the path of the entity.
 
         Files "to_configure" are text based model input files where
         parameters for the model are set. Note that only models
@@ -130,34 +150,33 @@
         :type to_configure: list, optional
         """
         to_copy = init_default([], to_copy, (list, str))
         to_symlink = init_default([], to_symlink, (list, str))
         to_configure = init_default([], to_configure, (list, str))
         self.files = EntityFiles(to_configure, to_copy, to_symlink)
 
-    def colocate_db(self, *args, **kwargs):
+    def colocate_db(self, *args: t.Any, **kwargs: t.Any) -> None:
         """An alias for ``Model.colocate_db_tcp``"""
         warnings.warn(
             (
                 "`colocate_db` has been deprecated and will be removed in a \n"
                 "future release. Please use `colocate_db_tcp` or `colocate_db_uds`."
-            ),
-            category=DeprecationWarning,
+            ), FutureWarning
         )
         self.colocate_db_tcp(*args, **kwargs)
 
     def colocate_db_uds(
         self,
-        unix_socket="/tmp/redis.socket",
-        socket_permissions=755,
-        db_cpus=1,
-        limit_app_cpus=True,
-        debug=False,
-        **kwargs,
-    ):
+        unix_socket: str = "/tmp/redis.socket",
+        socket_permissions: int = 755,
+        db_cpus: int = 1,
+        custom_pinning: t.Optional[t.Iterable[t.Union[int, t.Iterable[int]]]] = None,
+        debug: bool = False,
+        **kwargs: t.Any,
+    ) -> None:
         """Colocate an Orchestrator instance with this Model over UDS.
 
         This method will initialize settings which add an unsharded
         database to this Model instance. Only this Model will be able to communicate
         with this colocated database by using Unix Domain sockets.
 
         Extra parameters for the db can be passed through kwargs. This includes
@@ -178,43 +197,45 @@
 
         :param unix_socket: path to where the socket file will be created
         :type unix_socket: str, optional
         :param socket_permissions: permissions for the socketfile
         :type socket_permissions: int, optional
         :param db_cpus: number of cpus to use for orchestrator, defaults to 1
         :type db_cpus: int, optional
-        :param limit_app_cpus: whether to limit the number of cpus used by the app, defaults to True
-        :type limit_app_cpus: bool, optional
-        :param debug: launch Model with extra debug information about the co-located db
+        :param custom_pinning: CPUs to pin the orchestrator to. Passing an empty iterable
+                               disables pinning
+        :type custom_pinning: iterable of ints or iterable of ints, optional
+        :param debug: launch Model with extra debug information about the colocated db
         :type debug: bool, optional
         :param kwargs: additional keyword arguments to pass to the orchestrator database
         :type kwargs: dict, optional
         """
 
         uds_options = {
             "unix_socket": unix_socket,
             "socket_permissions": socket_permissions,
             "port": 0,  # This is hardcoded to 0 as recommended by redis for UDS
         }
+
         common_options = {
             "cpus": db_cpus,
-            "limit_app_cpus": limit_app_cpus,
+            "custom_pinning": custom_pinning,
             "debug": debug,
         }
         self._set_colocated_db_settings(uds_options, common_options, **kwargs)
 
     def colocate_db_tcp(
         self,
-        port=6379,
-        ifname="lo",
-        db_cpus=1,
-        limit_app_cpus=True,
-        debug=False,
-        **kwargs,
-    ):
+        port: int = 6379,
+        ifname: t.Union[str, list[str]] = "lo",
+        db_cpus: int = 1,
+        custom_pinning: t.Optional[t.Iterable[t.Union[int, t.Iterable[int]]]] = None,
+        debug: bool = False,
+        **kwargs: t.Any,
+    ) -> None:
         """Colocate an Orchestrator instance with this Model over TCP/IP.
 
         This method will initialize settings which add an unsharded
         database to this Model instance. Only this Model will be able to communicate
         with this colocated database by using the loopback TCP interface.
 
         Extra parameters for the db can be passed through kwargs. This includes
@@ -232,49 +253,66 @@
             }
 
         Generally these don't need to be changed.
 
         :param port: port to use for orchestrator database, defaults to 6379
         :type port: int, optional
         :param ifname: interface to use for orchestrator, defaults to "lo"
-        :type ifname: str, optional
+        :type ifname: str | list[str], optional
         :param db_cpus: number of cpus to use for orchestrator, defaults to 1
         :type db_cpus: int, optional
-        :param limit_app_cpus: whether to limit the number of cpus used by the app, defaults to True
-        :type limit_app_cpus: bool, optional
-        :param debug: launch Model with extra debug information about the co-located db
+        :param custom_pinning: CPUs to pin the orchestrator to. Passing an empty iterable
+                               disables pinning
+        :type custom_pinning: iterable of ints or iterable of ints, optional
+        :param debug: launch Model with extra debug information about the colocated db
         :type debug: bool, optional
         :param kwargs: additional keyword arguments to pass to the orchestrator database
         :type kwargs: dict, optional
 
         """
 
         tcp_options = {"port": port, "ifname": ifname}
         common_options = {
             "cpus": db_cpus,
-            "limit_app_cpus": limit_app_cpus,
+            "custom_pinning": custom_pinning,
             "debug": debug,
         }
         self._set_colocated_db_settings(tcp_options, common_options, **kwargs)
 
-    def _set_colocated_db_settings(self, connection_options, common_options, **kwargs):
+    def _set_colocated_db_settings(
+        self,
+        connection_options: t.Dict[str, t.Any],
+        common_options: t.Dict[str, t.Any],
+        **kwargs: t.Any,
+    ) -> None:
         """
         Ingest the connection-specific options (UDS/TCP) and set the final settings
-        for the co-located database
+        for the colocated database
         """
 
         if hasattr(self.run_settings, "mpmd") and len(self.run_settings.mpmd) > 0:
             raise SSUnsupportedError(
-                "Models co-located with databases cannot be run as a mpmd workload"
+                "Models colocated with databases cannot be run as a mpmd workload"
             )
 
         if hasattr(self.run_settings, "_prep_colocated_db"):
             self.run_settings._prep_colocated_db(common_options["cpus"])
 
+        if "limit_app_cpus" in kwargs:
+            raise SSUnsupportedError(
+                "Pinning of app CPUs via limit_app_cpus is no supported. Modify RunSettings "
+                "instead using the correct binding option for your launcher."
+            )
+
         # TODO list which db settings can be extras
+        common_options["custom_pinning"] = self._create_pinning_string(
+            common_options["custom_pinning"],
+            common_options["cpus"]
+        )
+
         colo_db_config = {}
         colo_db_config.update(connection_options)
         colo_db_config.update(common_options)
         # redisai arguments for inference settings
         colo_db_config["rai_args"] = {
             "threads_per_queue": kwargs.get("threads_per_queue", None),
             "inter_op_parallelism": kwargs.get("inter_op_parallelism", None),
@@ -290,62 +328,122 @@
 
         self._check_db_objects_colo()
         colo_db_config["db_models"] = self._db_models
         colo_db_config["db_scripts"] = self._db_scripts
 
         self.run_settings.colocated_db_settings = colo_db_config
 
-    def params_to_args(self):
-        """Convert parameters to command line arguments and update run settings."""
-        for param in self.params_as_args:
-            if not param in self.params:
-                raise ValueError(
-                    f"Tried to convert {param} to command line argument "
-                    + f"for Model {self.name}, but its value was not found in model params"
-                )
-            if self.run_settings is None:
-                raise ValueError(
-                    f"Tried to configure command line parameter for Model {self.name}, "
-                    + "but no RunSettings are set."
+    @staticmethod
+    def _create_pinning_string(
+        pin_ids: t.Optional[t.Iterable[t.Union[int, t.Iterable[int]]]],
+        cpus: int
+        ) -> t.Optional[str]:
+        """Create a comma-separated string CPU ids. By default, None returns
+        0,1,...,cpus-1; an empty iterable will disable pinning altogether,
+        and an iterable constructs a comma separate string (e.g. 0,2,5)
+        """
+        def _stringify_id(id: int) -> str:
+            """Return the cPU id as a string if an int, otherwise raise a ValueError"""
+            if isinstance(id, int):
+                if id < 0:
+                    raise ValueError("CPU id must be a nonnegative number")
+                else:
+                    return str(id)
+            else:
+                raise TypeError(f"Argument is of type '{type(id)}' not 'int'")
+
+        _invalid_input_message = (
+            "Expected a cpu pinning specification of type iterable of ints or "
+            f"iterables of ints. Instead got type `{type(pin_ids)}`"
+        )
+
+        # Deal with MacOSX limitations first. The "None" (default) disables pinning
+        # and is equivalent to []. The only invalid option is an iterable
+        if "darwin" == sys.platform:
+            if pin_ids is None or not pin_ids:
+                return None
+            elif isinstance(pin_ids, collections.abc.Iterable):
+                warnings.warn(
+                    "CPU pinning is not supported on MacOSX. Ignoring pinning "
+                    "specification.",
+                    RuntimeWarning
                 )
-            self.run_settings.add_exe_args(cat_arg_and_value(param, self.params[param]))
+                return None
+            else:
+                raise TypeError(_invalid_input_message)
+        # Flatten the iterable into a list and check to make sure that the resulting
+        # elements are all ints
+        if pin_ids is None:
+            return ','.join(_stringify_id(i) for i in range(cpus))
+        elif not pin_ids:
+            return None
+        elif isinstance(pin_ids, collections.abc.Iterable):
+            pin_list = []
+            for pin_id in pin_ids:
+                if isinstance(pin_id, collections.abc.Iterable):
+                    pin_list.extend([_stringify_id(j) for j in pin_id])
+                else:
+                    pin_list.append(_stringify_id(pin_id))
+            return ','.join(sorted(set(pin_list)))
+        else:
+            raise TypeError(_invalid_input_message)
+
+    def params_to_args(self) -> None:
+        """Convert parameters to command line arguments and update run settings."""
+        if self.params_as_args is not None:
+            for param in self.params_as_args:
+                if not param in self.params:
+                    raise ValueError(
+                        f"Tried to convert {param} to command line argument "
+                        + f"for Model {self.name}, but its value was not found in model params"
+                    )
+                if self.run_settings is None:
+                    raise ValueError(
+                        f"Tried to configure command line parameter for Model {self.name}, "
+                        + "but no RunSettings are set."
+                    )
+                self.run_settings.add_exe_args(cat_arg_and_value(param, self.params[param]))
 
     def add_ml_model(
         self,
-        name,
-        backend,
-        model=None,
-        model_path=None,
-        device="CPU",
-        devices_per_node=1,
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        backend: str,
+        model: t.Optional[str] = None,
+        model_path: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.List[str]] = None,
+        outputs: t.Optional[t.List[str]] = None,
+    ) -> None:
         """A TF, TF-lite, PT, or ONNX model to load into the DB at runtime
 
         Each ML Model added will be loaded into an
         orchestrator (converged or not) prior to the execution
         of this Model instance
 
         One of either model (in memory representation) or model_path (file)
         must be provided
 
         :param name: key to store model under
         :type name: str
-        :param model: model in memory
+        :param backend: name of the backend (TORCH, TF, TFLITE, ONNX)
+        :type backend: str
+        :param model: A model in memory (only supported for non-colocated orchestrators)
         :type model: byte string, optional
         :param model_path: serialized model
         :type model_path: file path to model
-        :param backend: name of the backend (TORCH, TF, TFLITE, ONNX)
-        :type backend: str
         :param device: name of device for execution, defaults to "CPU"
         :type device: str, optional
+        :param devices_per_node: The number of GPU devices available on the host.
+               This parameter only applies to GPU devices and will be ignored if device
+               is specified as GPU.
+        :type devices_per_node: int
         :param batch_size: batch size for execution, defaults to 0
         :type batch_size: int, optional
         :param min_batch_size: minimum batch size for model execution, defaults to 0
         :type min_batch_size: int, optional
         :param tag: additional tag for model information, defaults to ""
         :type tag: str, optional
         :param inputs: model inputs (TF only), defaults to None
@@ -365,16 +463,21 @@
             tag=tag,
             inputs=inputs,
             outputs=outputs,
         )
         self._append_db_model(db_model)
 
     def add_script(
-        self, name, script=None, script_path=None, device="CPU", devices_per_node=1
-    ):
+        self,
+        name: str,
+        script: t.Optional[str] = None,
+        script_path: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+    ) -> None:
         """TorchScript to launch with this Model instance
 
         Each script added to the model will be loaded into an
         orchestrator (converged or not) prior to the execution
         of this Model instance
 
         Device selection is either "GPU" or "CPU". If many devices are
@@ -384,33 +487,41 @@
         in the model being stored in the first N devices of type ``device``.
 
         One of either script (in memory string representation) or script_path (file)
         must be provided
 
         :param name: key to store script under
         :type name: str
-        :param script: TorchScript code
+        :param script: TorchScript code (only supported for non-colocated orchestrators)
         :type script: str, optional
         :param script_path: path to TorchScript code
         :type script_path: str, optional
         :param device: device for script execution, defaults to "CPU"
         :type device: str, optional
-        :param devices_per_node: number of devices on each host
+        :param devices_per_node: The number of GPU devices available on the host.
+               This parameter only applies to GPU devices and will be ignored if device
+               is specified as GPU.
         :type devices_per_node: int
         """
         db_script = DBScript(
             name=name,
             script=script,
             script_path=script_path,
             device=device,
             devices_per_node=devices_per_node,
         )
         self._append_db_script(db_script)
 
-    def add_function(self, name, function=None, device="CPU", devices_per_node=1):
+    def add_function(
+        self,
+        name: str,
+        function: t.Optional[str] = None,
+        device: str = "CPU",
+        devices_per_node: int = 1,
+    ) -> None:
         """TorchScript function to launch with this Model instance
 
         Each script function to the model will be loaded into a
         non-converged orchestrator prior to the execution
         of this Model instance.
 
         For converged orchestrators, the :meth:`add_script` method should be used.
@@ -419,67 +530,69 @@
         present, a number can be passed for specification e.g. "GPU:1".
 
         Setting ``devices_per_node=N``, with N greater than one will result
         in the model being stored in the first N devices of type ``device``.
 
         :param name: key to store function under
         :type name: str
-        :param script: TorchScript code
-        :type script: str or byte string, optional
-        :param script_path: path to TorchScript code
-        :type script_path: str, optional
+        :param function: TorchScript function code
+        :type function: str, optional
         :param device: device for script execution, defaults to "CPU"
         :type device: str, optional
-        :param devices_per_node: number of devices on each host
+        :param devices_per_node: The number of GPU devices available on the host.
+               This parameter only applies to GPU devices and will be ignored if device
+               is specified as GPU.
         :type devices_per_node: int
         """
         db_script = DBScript(
             name=name, script=function, device=device, devices_per_node=devices_per_node
         )
         self._append_db_script(db_script)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Model):
+            return False
+
         if self.name == other.name:
             return True
         return False
 
-    def __str__(self):  # pragma: no cover
+    def __str__(self) -> str:  # pragma: no cover
         entity_str = "Name: " + self.name + "\n"
         entity_str += "Type: " + self.type + "\n"
         entity_str += str(self.run_settings) + "\n"
         if self._db_models:
             entity_str += "DB Models: \n" + str(len(self._db_models)) + "\n"
         if self._db_scripts:
             entity_str += "DB Scripts: \n" + str(len(self._db_scripts)) + "\n"
         return entity_str
 
-    def _append_db_model(self, db_model):
+    def _append_db_model(self, db_model: DBModel) -> None:
         if not db_model.is_file and self.colocated:
             err_msg = "ML model can not be set from memory for colocated databases.\n"
             err_msg += (
                 f"Please store the ML model named {db_model.name} in binary format "
             )
             err_msg += "and add it to the SmartSim Model as file."
             raise SSUnsupportedError(err_msg)
 
         self._db_models.append(db_model)
 
-    def _append_db_script(self, db_script):
+    def _append_db_script(self, db_script: DBScript) -> None:
         if db_script.func and self.colocated:
             if not isinstance(db_script.func, str):
                 err_msg = (
                     "Functions can not be set from memory for colocated databases.\n"
                 )
                 err_msg += f"Please convert the function named {db_script.name} to a string or store "
                 err_msg += "it as a text file and add it to the SmartSim Model with add_script."
                 raise SSUnsupportedError(err_msg)
         self._db_scripts.append(db_script)
 
-    def _check_db_objects_colo(self):
-
+    def _check_db_objects_colo(self) -> None:
         for db_model in self._db_models:
             if not db_model.is_file:
                 err_msg = (
                     "ML model can not be set from memory for colocated databases.\n"
                 )
                 err_msg += (
                     f"Please store the ML model named {db_model.name} in binary format "
```

### Comparing `smartsim-0.4.2/smartsim/entity/strategies.py` & `smartsim-0.5.0/smartsim/entity/strategies.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,50 +21,45 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # Generation Strategies
+import random
+import typing as t
 
 from itertools import product
 
 
 # create permutations of all parameters
 # single model if parameters only have one value
-def create_all_permutations(param_names, param_values):
+def create_all_permutations(
+    param_names: t.List[str], param_values: t.List[t.List[str]], _n_models: int = 0
+) -> t.List[t.Dict[str, str]]:
     perms = list(product(*param_values))
     all_permutations = []
     for p in perms:
         temp_model = dict(zip(param_names, p))
         all_permutations.append(temp_model)
     return all_permutations
 
 
-def step_values(param_names, param_values):
+def step_values(
+    param_names: t.List[str], param_values: t.List[t.List[str]], _n_models: int = 0
+) -> t.List[t.Dict[str, str]]:
     permutations = []
     for p in zip(*param_values):
         permutations.append(dict(zip(param_names, p)))
     return permutations
 
 
-def random_permutations(param_names, param_values, n_models):
-    import random
+def random_permutations(
+    param_names: t.List[str], param_values: t.List[t.List[str]], n_models: int = 0
+) -> t.List[t.Dict[str, str]]:
+    permutations = create_all_permutations(param_names, param_values)
+
+    # sample from available permutations if n_models is specified
+    if n_models and n_models < len(permutations):
+        permutations = random.sample(permutations, n_models)
 
-    # first, check if we've requested more values than possible.
-    perms = list(product(*param_values))
-    if n_models >= len(perms):
-        return create_all_permutations(param_names, param_values)
-    else:
-        permutations = []
-        permutation_strings = set()
-        while len(permutations) < n_models:
-            model_dict = dict(
-                zip(
-                    param_names,
-                    map(lambda x: x[random.randint(0, len(x) - 1)], param_values),
-                )
-            )
-            if str(model_dict) not in permutation_strings:
-                permutation_strings.add(str(model_dict))
-                permutations.append(model_dict)
-        return permutations
+    return permutations
```

### Comparing `smartsim-0.4.2/smartsim/error/__init__.py` & `smartsim-0.5.0/smartsim/error/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/error/errors.py` & `smartsim-0.5.0/smartsim/error/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 
 # Exceptions
 
 
 class SmartSimError(Exception):
     """Base SmartSim error"""
 
@@ -41,34 +42,34 @@
     an entity and either the entity/files/directories already exist"""
 
 
 class UserStrategyError(SmartSimError):
     """Raised when there is an error with model creation inside an ensemble
     that is from a user provided permutation strategy"""
 
-    def __init__(self, perm_strat):
+    def __init__(self, perm_strat: str) -> None:
         message = self.create_message(perm_strat)
         super().__init__(message)
 
-    def create_message(self, perm_strat):
+    def create_message(self, perm_strat: str) -> str:
         prefix = "User provided ensemble generation strategy"
         message = "failed to generate valid parameter names and values"
         return " ".join((prefix, str(perm_strat), message))
 
 
 class ParameterWriterError(SmartSimError):
     """Raised in the event that input parameter files for a model
     could not be written.
     """
 
-    def __init__(self, file_path, read=True):
+    def __init__(self, file_path: str, read: bool = True) -> None:
         message = self.create_message(file_path, read)
         super().__init__(message)
 
-    def create_message(self, fp, read):
+    def create_message(self, fp: str, read: bool) -> str:
         if read:
             msg = f"Failed to read configuration file to write at {fp}"
         else:
             msg = f"Failed to write configuration file to {fp}"
         return msg
 
 
@@ -76,16 +77,14 @@
 
 
 class SSInternalError(Exception):
     """
     SSInternalError is raised when an internal error is encountered.
     """
 
-    pass
-
 
 class SSConfigError(SSInternalError):
     """Raised when there is an error in the configuration of SmartSim"""
 
 
 class LauncherError(SSInternalError):
     """Raised when there is an error in the launcher"""
@@ -95,19 +94,24 @@
     """Raised when there is a problem with the user WLM allocation"""
 
 
 class ShellError(LauncherError):
     """Raised when error arises from function within launcher.shell
     Closely related to error from subprocess(Popen) commands"""
 
-    def __init__(self, message, shell_error, command_list):
-        msg = self.create_message(message, shell_error, command_list)
+    def __init__(
+        self, message: str, command_list: t.Union[str, t.List[str]], details: t.Optional[t.Union[Exception, str]] = None
+    ) -> None:
+        msg = self.create_message(message, command_list, details=details)
         super().__init__(msg)
 
-    def create_message(self, message, shell_error, command_list):
+    @staticmethod
+    def create_message(
+        message: str, command_list: t.Union[str, t.List[str]], details: t.Optional[t.Union[Exception, str]]
+    ) -> str:
         if isinstance(command_list, list):
             command_list = " ".join(command_list)
         msg = message + "\n"
         msg += f"\nCommand: {command_list}"
-        if shell_error:
-            msg += f"\nError from shell: {shell_error}"
+        if details:
+            msg += f"\nError from shell: {details}"
         return msg
```

### Comparing `smartsim-0.4.2/smartsim/experiment.py` & `smartsim-0.5.0/smartsim/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,27 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os.path as osp
 import time
+import typing as t
 from os import getcwd
 
 from tabulate import tabulate
 from tqdm import trange
 
 from ._core import Controller, Generator, Manifest
 from ._core.utils import init_default
 from .database import Orchestrator
-from .entity import Ensemble, Model
+from .entity import Ensemble, Model, SmartSimEntity
 from .error import SmartSimError
 from .log import get_logger
-from .settings import settings
+from .settings import settings, base, Container
 from .wlm import detect_launcher
 
 logger = get_logger(__name__)
 
 
 class Experiment:
     """Experiments are the Python user interface for SmartSim.
@@ -58,15 +59,17 @@
     ``Experiment.start`` or ``Experiment.stop``, accept any number of the
     instances created by the Experiment.
 
     In general, the Experiment class is designed to be initialized once
     and utilized throughout runtime.
     """
 
-    def __init__(self, name, exp_path=None, launcher="local"):
+    def __init__(
+        self, name: str, exp_path: t.Optional[str] = None, launcher: str = "local"
+    ):
         """Initialize an Experiment instance
 
         With the default settings, the Experiment will use the
         local launcher, which will start all Experiment created
         instances on the localhost.
 
         Example of initializing an Experiment with the local launcher
@@ -121,15 +124,21 @@
 
         if launcher == "auto":
             launcher = detect_launcher()
 
         self._control = Controller(launcher=launcher)
         self._launcher = launcher.lower()
 
-    def start(self, *args, block=True, summary=False, kill_on_interrupt=True):
+    def start(
+        self,
+        *args: t.Any,
+        block: bool = True,
+        summary: bool = False,
+        kill_on_interrupt: bool = True,
+    ) -> None:
         """Start passed instances using Experiment launcher
 
         Any instance ``Model``, ``Ensemble`` or ``Orchestrator``
         instance created by the Experiment can be passed as
         an argument to the start method.
 
         .. highlight:: python
@@ -185,15 +194,15 @@
                 block=block,
                 kill_on_interrupt=kill_on_interrupt,
             )
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def stop(self, *args):
+    def stop(self, *args: t.Any) -> None:
         """Stop specific instances launched by this ``Experiment``
 
         Instances of ``Model``, ``Ensemble`` and ``Orchestrator``
         can all be passed as arguments to the stop method.
 
         Whichever launcher was specified at Experiment initialization
         will be used to stop the instance. For example, which using
@@ -218,15 +227,17 @@
                 self._control.stop_entity(entity)
             for entity_list in stop_manifest.all_entity_lists:
                 self._control.stop_entity_list(entity_list)
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def generate(self, *args, tag=None, overwrite=False):
+    def generate(
+        self, *args: t.Any, tag: t.Optional[str] = None, overwrite: bool = False
+    ) -> None:
         """Generate the file structure for an ``Experiment``
 
         ``Experiment.generate`` creates directories for each instance
         passed to organize Experiments that launch many instances.
 
         If files or directories are attached to ``Model`` objects
         using ``Model.attach_generator_files()``, those files or
@@ -247,15 +258,17 @@
             if tag:
                 generator.set_tag(tag)
             generator.generate_experiment(*args)
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def poll(self, interval=10, verbose=True, kill_on_interrupt=True):
+    def poll(
+        self, interval: int = 10, verbose: bool = True, kill_on_interrupt: bool = True
+    ) -> None:
         """Monitor jobs through logging to stdout.
 
         This method should only be used if jobs were launched
         with ``Experiment.start(block=False)``
 
         The internal specified will control how often the
         logging is performed, not how often the polling occurs.
@@ -288,15 +301,15 @@
         """
         try:
             self._control.poll(interval, verbose, kill_on_interrupt=kill_on_interrupt)
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def finished(self, entity):
+    def finished(self, entity: SmartSimEntity) -> bool:
         """Query if a job has completed.
 
         An instance of ``Model`` or ``Ensemble`` can be passed
         as an argument.
 
         Passing ``Orchestrator`` will return an error as a
         database deployment is never finished until stopped
@@ -311,15 +324,15 @@
         """
         try:
             return self._control.finished(entity)
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def get_status(self, *args):
+    def get_status(self, *args: t.Any) -> t.List[str]:
         """Query the status of launched instances
 
         Return a smartsim.status string representing
         the status of the launched instance.
 
         .. highlight:: python
         .. code-block:: python
@@ -338,34 +351,34 @@
 
         :returns: status of the instances passed as arguments
         :rtype: list[str]
         :raises SmartSimError: if status retrieval fails
         """
         try:
             manifest = Manifest(*args)
-            statuses = []
+            statuses: t.List[str] = []
             for entity in manifest.models:
                 statuses.append(self._control.get_entity_status(entity))
             for entity_list in manifest.all_entity_lists:
                 statuses.extend(self._control.get_entity_list_status(entity_list))
             return statuses
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_ensemble(
         self,
-        name,
-        params=None,
-        batch_settings=None,
-        run_settings=None,
-        replicas=None,
-        perm_strategy="all_perm",
-        **kwargs,
-    ):
+        name: str,
+        params: t.Optional[t.Dict[str, t.Any]] = None,
+        batch_settings: t.Optional[base.BatchSettings] = None,
+        run_settings: t.Optional[base.RunSettings] = None,
+        replicas: t.Optional[int] = None,
+        perm_strategy: str = "all_perm",
+        **kwargs: t.Any,
+    ) -> Ensemble:
         """Create an ``Ensemble`` of ``Model`` instances
 
         Ensembles can be launched sequentially or as a batch
         if using a non-local launcher. e.g. slurm
 
         Ensembles require one of the following combinations
         of arguments
@@ -400,45 +413,45 @@
         :type batch_settings: BatchSettings
         :param run_settings: describes how each ``Model`` should be executed
         :type run_settings: RunSettings
         :param replicas: number of replicas to create
         :type replicas: int
         :param perm_strategy: strategy for expanding ``params`` into
                               ``Model`` instances from params argument
-                              options are "all_perm", "stepped", "random"
+                              options are "all_perm", "step", "random"
                               or a callable function. Default is "all_perm".
         :type perm_strategy: str, optional
         :raises SmartSimError: if initialization fails
         :return: ``Ensemble`` instance
         :rtype: Ensemble
         """
         try:
             new_ensemble = Ensemble(
                 name,
-                params,
+                params or {},
                 batch_settings=batch_settings,
                 run_settings=run_settings,
                 perm_strat=perm_strategy,
                 replicas=replicas,
                 **kwargs,
             )
             return new_ensemble
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_model(
         self,
-        name,
-        run_settings,
-        params=None,
-        path=None,
-        enable_key_prefixing=False,
-        batch_settings=None,
-    ):
+        name: str,
+        run_settings: base.RunSettings,
+        params: t.Optional[t.Dict[str, t.Any]] = None,
+        path: t.Optional[str] = None,
+        enable_key_prefixing: bool = False,
+        batch_settings: t.Optional[base.BatchSettings] = None,
+    ) -> Model:
         """Create a general purpose ``Model``
 
         The ``Model`` class is the most general encapsulation of
         executable code in SmartSim. ``Model`` instances are named
         references to pieces of a workflow that can be parameterized,
         and executed.
 
@@ -483,22 +496,22 @@
                 "epoch": 10,
                 "lr": 0.001
             }
             model = exp.create_model("pytorch_model", run_settings, params=params)
             model.attach_generator_files(to_configure="./train.cfg")
             exp.generate(model)
 
-        New in 0.4.0, ``Model`` instances can be co-located with an
+        New in 0.4.0, ``Model`` instances can be colocated with an
         Orchestrator database shard through ``Model.colocate_db``. This
         will launch a single ``Orchestrator`` instance on each compute
         host used by the (possibly distributed) application. This is
         useful for performant online inference or processing
         at runtime.
 
-        New in 0.4.2, ``Model`` instances can now be co-located with
+        New in 0.4.2, ``Model`` instances can now be colocated with
         an Orchestrator database over either TCP or UDS using the
         ``Model.colocate_db_tcp`` or ``Model.colocate_db_uds`` method
         respectively. The original ``Model.colocate_db`` method is now
         deprecated, but remains as an alias for ``Model.colocate_db_tcp``
         for backward compatibility.
 
         :param name: name of the model
@@ -518,36 +531,42 @@
                                defaults to None
         :type batch_settings: BatchSettings | None
         :raises SmartSimError: if initialization fails
         :return: the created ``Model``
         :rtype: Model
         """
         path = init_default(getcwd(), path, str)
-        params = init_default({}, params, dict)
+        
+        # mcb
+        if path is None:
+            path = getcwd()
+        if params is None:
+            params = {}
+
         try:
             new_model = Model(
                 name, params, path, run_settings, batch_settings=batch_settings
             )
             if enable_key_prefixing:
                 new_model.enable_key_prefixing()
             return new_model
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_run_settings(
         self,
-        exe,
-        exe_args=None,
-        run_command="auto",
-        run_args=None,
-        env_vars=None,
-        container=None,
-        **kwargs,
-    ):
+        exe: str,
+        exe_args: t.Optional[t.List[str]] = None,
+        run_command: str = "auto",
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        container: t.Optional[Container] = None,
+        **kwargs: t.Any,
+    ) -> settings.RunSettings:
         """Create a ``RunSettings`` instance.
 
         run_command="auto" will attempt to automatically
         match a run command on the system with a RunSettings
         class in SmartSim. If found, the class corresponding
         to that run_command will be created and returned.
 
@@ -570,20 +589,23 @@
         :param run_command: command to run the executable
         :type run_command: str
         :param exe: executable to run
         :type exe: str
         :param exe_args: arguments to pass to the executable
         :type exe_args: list[str], optional
         :param run_args: arguments to pass to the ``run_command``
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment variables to pass to the executable
         :type env_vars: dict[str, str], optional
+        :param container: if execution environment is containerized
+        :type container: Container, optional
         :return: the created ``RunSettings``
         :rtype: RunSettings
         """
+
         try:
             return settings.create_run_settings(
                 self._launcher,
                 exe,
                 exe_args=exe_args,
                 run_command=run_command,
                 run_args=run_args,
@@ -592,16 +614,22 @@
                 **kwargs,
             )
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_batch_settings(
-        self, nodes=1, time="", queue="", account="", batch_args=None, **kwargs
-    ):
+        self,
+        nodes: int = 1,
+        time: str = "",
+        queue: str = "",
+        account: str = "",
+        batch_args: t.Optional[t.Dict[str, str]] = None,
+        **kwargs: t.Any,
+    ) -> base.BatchSettings:
         """Create a ``BatchSettings`` instance
 
         Batch settings parameterize batch workloads. The result of this
         function can be passed to the ``Ensemble`` initialization.
 
         the `batch_args` parameter can be used to pass in a dictionary
         of additional batch command arguments that aren't supported through
@@ -647,26 +675,26 @@
             )
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_database(
         self,
-        port=6379,
-        db_nodes=1,
-        batch=False,
-        hosts=None,
-        run_command="auto",
-        interface="ipogif0",
-        account=None,
-        time=None,
-        queue=None,
-        single_cmd=True,
-        **kwargs,
-    ):
+        port: int = 6379,
+        db_nodes: int = 1,
+        batch: bool = False,
+        hosts: t.Optional[t.List[str]] = None,
+        run_command: str = "auto",
+        interface: str = "ipogif0",
+        account: t.Optional[str] = None,
+        time: t.Optional[str] = None,
+        queue: t.Optional[str] = None,
+        single_cmd: bool = True,
+        **kwargs: t.Any,
+    ) -> Orchestrator:
         """Initialize an Orchestrator database
 
         The ``Orchestrator`` database is a key-value store based
         on Redis that can be launched together with other Experiment
         created instances for online data storage.
 
         When launched, ``Orchestrator`` can be used to communicate
@@ -718,15 +746,15 @@
             time=time,
             queue=queue,
             single_cmd=single_cmd,
             launcher=self._launcher,
             **kwargs,
         )
 
-    def reconnect_orchestrator(self, checkpoint):
+    def reconnect_orchestrator(self, checkpoint: str) -> Orchestrator:
         """Reconnect to a running ``Orchestrator``
 
         This method can be used to connect to a ``Orchestrator`` deployment
         that was launched by a previous ``Experiment``. This can be
         helpful in the case where separate runs of an ``Experiment``
         wish to use the same ``Orchestrator`` instance currently
         running on a system.
@@ -738,15 +766,15 @@
         try:
             orc = self._control.reload_saved_db(checkpoint)
             return orc
         except SmartSimError as e:
             logger.error(e)
             raise
 
-    def summary(self, format="github"):
+    def summary(self, format: str = "github") -> str:
         """Return a summary of the ``Experiment``
 
         The summary will show each instance that has been
         launched and completed in this ``Experiment``
 
         :param format: the style in which the summary table is formatted,
                        for a full list of styles see:
@@ -785,15 +813,15 @@
                 headers,
                 showindex=True,
                 tablefmt=format,
                 missingval="None",
                 disable_numparse=True,
             )
 
-    def _launch_summary(self, manifest):
+    def _launch_summary(self, manifest: Manifest) -> None:
         """Experiment pre-launch summary of entities that will be launched
 
         :param manifest: Manifest of deployables.
         :type manifest: Manifest
         """
 
         summary = "\n\n=== Launch Summary ===\n"
@@ -810,21 +838,9 @@
         else:
             summary += f"Database Status: inactive\n"
 
         summary += f"\n{str(manifest)}"
 
         logger.info(summary)
 
-        wait, steps = 10, 100
-        prog_bar = trange(
-            steps,
-            desc="Launching in...",
-            leave=False,
-            ncols=80,
-            mininterval=0.25,
-            bar_format="{desc}: {bar}| {remaining} {elapsed}",
-        )
-        for _ in prog_bar:
-            time.sleep(wait / steps)
-
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
```

### Comparing `smartsim-0.4.2/smartsim/log.py` & `smartsim-0.5.0/smartsim/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import typing as t
 import logging
 import os
 import sys
 
 import coloredlogs
 
 # constants for logging
@@ -34,15 +35,15 @@
 coloredlogs.DEFAULT_LOG_FORMAT = (
     "%(asctime)s %(hostname)s %(name)s[%(process)d] %(levelname)s %(message)s"
 )
 # optional thread name logging for debugging
 # coloredlogs.DEFAULT_LOG_FORMAT = '%(asctime)s [%(threadName)s] %(hostname)s %(name)s[%(process)d] %(levelname)s %(message)s'
 
 
-def _get_log_level():
+def _get_log_level() -> str:
     """Get the logging level based on environment variable
        SMARTSIM_LOG_LEVEL.  If not set, default to info.
 
        Logging levels
          - quiet: Just shows errors and warnings
          - info: Show basic information and errors (default)
          - debug: Shows info, errors and user debug information
@@ -61,15 +62,17 @@
         return "debug"
     # extremely verbose logging used internally
     if log_level == "developer":
         return "debug"
     return "info"
 
 
-def get_logger(name, log_level=None, fmt=None):
+def get_logger(
+    name: str, log_level: t.Optional[str] = None, fmt: t.Optional[str] = None
+) -> logging.Logger:
     """Return a logger instance
 
     levels:
         - quiet
         - info
         - debug
         - developer
@@ -103,15 +106,15 @@
         logger.setLevel(log_level)
     else:
         log_level = user_log_level
     coloredlogs.install(level=log_level, logger=logger, fmt=fmt, stream=sys.stdout)
     return logger
 
 
-def log_to_file(filename, log_level="debug"):
+def log_to_file(filename: str, log_level: str = "debug") -> None:
     """Installs a second filestream handler to the root logger,
     allowing subsequent logging calls to be sent to filename.
 
     :param filename: the name of the desired log file.
     :type filename: str
 
     :param log_level: as defined in get_logger.  Can be specified
```

### Comparing `smartsim-0.4.2/smartsim/ml/__init__.py` & `smartsim-0.5.0/smartsim/ml/torch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .data import DataDownloader, DataInfo, TrainingDataUploader, form_name
+from .data import DataLoader, DynamicDataGenerator, StaticDataGenerator
```

### Comparing `smartsim-0.4.2/smartsim/ml/data.py` & `smartsim-0.5.0/smartsim/ml/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
+import typing as t
 from os import environ
 
 import numpy as np
 from smartredis import Client, Dataset
 from smartredis.error import RedisReplyError
 
 from ..error import SSInternalError
 from ..log import get_logger
 
 logger = get_logger(__name__)
 
 
-def form_name(*args):
+def form_name(*args: t.Any) -> str:
     return "_".join(str(arg) for arg in args if arg is not None)
 
 
 class DataInfo:
     """A class holding all relevant information to download datasets from aggregation lists
 
     This class can be passed as argument to SmartSim's ML data loaders, as it wraps the
@@ -58,23 +59,23 @@
     :param target_name: Name of tensor holding targets or labels in stored datasets.
     :type target_name: str
     :num_classes: Number of classes (for categorical data).
     :type num_classes: int | None
     """
 
     def __init__(
-        self, list_name, sample_name="samples", target_name="targets", num_classes=None
-    ):
+        self, list_name: str, sample_name: str = "samples", target_name: str = "targets", num_classes: t.Optional[int] = None
+    ) -> None:
         self.list_name = list_name
         self.sample_name = sample_name
         self.target_name = target_name
         self.num_classes = num_classes
         self._ds_name = form_name(self.list_name, "info")
 
-    def publish(self, client: Client):
+    def publish(self, client: Client) -> None:
         """Upload DataInfo information to Orchestrator
 
         The information is put on the DB as a DataSet, with strings
         stored as metastrings and integers stored as metascalars.
 
         :param client: Client to connect to Database
         :type client: SmartRedis.Client
@@ -83,15 +84,15 @@
         info_ds.add_meta_string("sample_name", self.sample_name)
         if self.target_name:
             info_ds.add_meta_string("target_name", self.target_name)
         if self.num_classes:
             info_ds.add_meta_scalar("num_classes", self.num_classes)
         client.put_dataset(info_ds)
 
-    def download(self, client: Client):
+    def download(self, client: Client) -> None:
         """Download DataInfo information from Orchestrator
 
         The information retrieved from the DB is used to populate
         this object's members. If the information is not available
         on the DB, the object members are not modified.
 
         :param client: Client to connect to Database
@@ -109,15 +110,15 @@
         self.sample_name = info_ds.get_meta_strings("sample_name")[0]
         field_names = info_ds.get_metadata_field_names()
         if "target_name" in field_names:
             self.target_name = info_ds.get_meta_strings("target_name")[0]
         if "num_classes" in field_names:
             self.num_classes = info_ds.get_meta_scalars("num_classes")[0]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         strings = ["DataInfo object"]
         strings += [f"Aggregation list name: {self.list_name}"]
         strings += [f"Sample tensor name: {self.sample_name}"]
         if self.target_name:
             strings += [f"Target tensor name: {self.target_name}"]
         if self.num_classes:
             strings += [f"Number of classes: {self.num_classes}"]
@@ -154,54 +155,54 @@
     :param verbose: If output should be logged to screen.
     :type verbose: bool
 
     """
 
     def __init__(
         self,
-        list_name="training_data",
-        sample_name="samples",
-        target_name="targets",
-        num_classes=None,
-        cluster=True,
-        address=None,
-        rank=None,
-        verbose=False,
-    ):
+        list_name: str = "training_data",
+        sample_name: str = "samples",
+        target_name: str = "targets",
+        num_classes: t.Optional[int] = None,
+        cluster: bool = True,
+        address: t.Optional[str] = None,
+        rank: t.Optional[int] = None,
+        verbose: bool = False,
+    ) -> None:
         if not list_name:
             raise ValueError("Name can not be empty")
         if not sample_name:
             raise ValueError("Sample name can not be empty")
 
         self.client = Client(address=address, cluster=cluster)
         self.verbose = verbose
         self.batch_idx = 0
         self.rank = rank
         self._info = DataInfo(list_name, sample_name, target_name, num_classes)
 
     @property
-    def list_name(self):
+    def list_name(self) -> str:
         return self._info.list_name
 
     @property
-    def sample_name(self):
+    def sample_name(self) -> str:
         return self._info.sample_name
 
     @property
-    def target_name(self):
+    def target_name(self) -> str:
         return self._info.target_name
 
     @property
-    def num_classes(self):
+    def num_classes(self) -> t.Optional[int]:
         return self._info.num_classes
 
-    def publish_info(self):
+    def publish_info(self) -> None:
         self._info.publish(self.client)
 
-    def put_batch(self, samples, targets=None):
+    def put_batch(self, samples: np.ndarray, targets: t.Optional[np.ndarray] = None) -> None:
         batch_ds_name = form_name("training_samples", self.rank, self.batch_idx)
         batch_ds = Dataset(batch_ds_name)
         batch_ds.add_tensor(self.sample_name, samples)
         if (
             targets is not None
             and self.target_name
             and (self.target_name != self.sample_name)
@@ -278,26 +279,26 @@
     :type init_samples: bool
     :param max_fetch_trials: maximum number of attempts to initialize data
     :type max_fetch_trials: int
     """
 
     def __init__(
         self,
-        data_info_or_list_name,
-        batch_size=32,
-        dynamic=True,
-        shuffle=True,
-        cluster=True,
-        address=None,
-        replica_rank=0,
-        num_replicas=1,
-        verbose=False,
-        init_samples=True,
-        max_fetch_trials=-1,
-    ):
+        data_info_or_list_name: t.Union[str, DataInfo],
+        batch_size: int = 32,
+        dynamic: bool = True,
+        shuffle: bool = True,
+        cluster: bool = True,
+        address: t.Optional[str] = None,
+        replica_rank: int = 0,
+        num_replicas: int = 1,
+        verbose: bool = False,
+        init_samples: bool = True,
+        max_fetch_trials: int = -1,
+    ) -> None:
         self.address = address
         self.cluster = cluster
         self.verbose = verbose
         self.samples = None
         self.targets = None
         self.num_samples = 0
         self.indices = np.arange(0)
@@ -308,90 +309,98 @@
             self._info = data_info_or_list_name
         elif isinstance(data_info_or_list_name, str):
             self._info = DataInfo(list_name=data_info_or_list_name)
             client = Client(self.address, self.cluster)
             self._info.download(client)
         else:
             raise TypeError("data_info_or_list_name must be either DataInfo or str")
-        self.client = None
+        self._client: t.Optional[Client] = None
         sskeyin = environ.get("SSKEYIN", "")
         self.uploader_keys = sskeyin.split(",")
 
         self.set_replica_parameters(replica_rank, num_replicas)
 
         if init_samples:
             self.init_samples(max_fetch_trials)
 
-    def log(self, message):
+    @property
+    def client(self) -> Client:
+        if self._client is None:
+            raise ValueError("Client not initialized")
+        return self._client
+
+    def log(self, message: str) -> None:
         if self.verbose:
             logger.info(message)
 
-    def set_replica_parameters(self, replica_rank, num_replicas):
+    def set_replica_parameters(self, replica_rank: int, num_replicas: int) -> None:
         self.replica_rank = replica_rank
         self.num_replicas = num_replicas
         self.next_indices = [self.replica_rank] * max(1, len(self.uploader_keys))
 
     @property
-    def autoencoding(self):
+    def autoencoding(self) -> bool:
         return self.sample_name == self.target_name
 
     @property
-    def list_name(self):
+    def list_name(self) -> str:
         return self._info.list_name
 
     @property
-    def sample_name(self):
+    def sample_name(self) -> str:
         return self._info.sample_name
 
     @property
-    def target_name(self):
+    def target_name(self) -> str:
         return self._info.target_name
 
     @property
-    def num_classes(self):
+    def num_classes(self) -> t.Optional[int]:
         return self._info.num_classes
 
     @property
-    def need_targets(self):
+    def need_targets(self) -> bool:
         """Compute if targets have to be downloaded.
 
         :return: Whether targets (or labels) should be downloaded
         :rtype: bool
         """
-        return self.target_name and not self.autoencoding
+        return bool(self.target_name) and not self.autoencoding
 
-    def __len__(self):
+    def __len__(self) -> int:
         length = int(np.floor(self.num_samples / self.batch_size))
         return length
 
-    def __iter__(self):
+    def _calc_indices(self, index: int) -> np.ndarray:
+        return self.indices[
+            index * self.batch_size : (index + 1) * self.batch_size
+        ]
+
+    def __iter__(self) -> t.Iterator[t.Tuple[np.ndarray, np.ndarray]]:
 
         self.update_data()
         # Generate data
         if len(self) < 1:
             msg = "Not enough samples in generator for one batch. "
             msg += "Please run init_samples() or initialize generator with init_samples=True"
             raise ValueError(msg)
 
-        _calc_indices = lambda index: self.indices[
-            index * self.batch_size : (index + 1) * self.batch_size
-        ]
         yield from (
-            self._data_generation(_calc_indices(idx)) for idx in range(len(self))
+            self._data_generation(self._calc_indices(idx)) for idx in range(len(self))
         )
 
-    def init_samples(self, init_trials=-1):
+    def init_samples(self, init_trials: int = -1) -> None:
         """Initialize samples (and targets, if needed).
 
         A new attempt to download samples will be made every ten seconds, for ``init_trials``
         times.
         :param init_trials: maximum number of attempts to fetch data
         :type init_trials: int
         """
-        self.client = Client(self.address, self.cluster)
+        self._client = Client(self.address, self.cluster)
 
         num_trials = 0
         max_trials = init_trials or -1
         while not len(self) and num_trials != max_trials:
             self._update_samples_and_targets()
             self.log(
                 "DataLoader could not download samples, will try again in 10 seconds"
@@ -402,61 +411,59 @@
         if not len(self):
             raise SSInternalError(
                 "Could not download samples in given number of trials"
             )
         if self.shuffle:
             np.random.shuffle(self.indices)
 
-    def _data_exists(self, batch_name, target_name):
-
+    def _data_exists(self, batch_name: str, target_name: str) -> bool:
         if self.need_targets:
             return self.client.tensor_exists(batch_name) and self.client.tensor_exists(
                 target_name
             )
         else:
             return self.client.tensor_exists(batch_name)
 
-    def _add_samples(self, indices):
+    def _add_samples(self, indices: t.List[int]) -> None:
+        datasets: t.List[Dataset] = []
 
         if self.num_replicas == 1:
-            datasets: list[Dataset] = self.client.get_dataset_list_range(
+            datasets = self.client.get_dataset_list_range(
                 self.list_name, start_index=indices[0], end_index=indices[-1]
             )
         else:
-            datasets: list[Dataset] = []
             for idx in indices:
                 datasets += self.client.get_dataset_list_range(
                     self.list_name, start_index=idx, end_index=idx
                 )
 
         if self.samples is None:
             self.samples = datasets[0].get_tensor(self.sample_name)
             if self.need_targets:
                 self.targets = datasets[0].get_tensor(self.target_name)
 
             if len(datasets) > 1:
                 datasets = datasets[1:]
 
-        for dataset in datasets:
-            self.samples = np.concatenate(
-                (self.samples, dataset.get_tensor(self.sample_name))
-            )
-            if self.need_targets:
-                self.targets = np.concatenate(
-                    (self.targets, dataset.get_tensor(self.target_name))
+        if self.samples is not None:
+            for dataset in datasets:
+                self.samples = np.concatenate(
+                    (self.samples, dataset.get_tensor(self.sample_name))
                 )
+                if self.need_targets:
+                    self.targets = np.concatenate(
+                        (self.targets, dataset.get_tensor(self.target_name))
+                    )
+
+            self.num_samples = self.samples.shape[0]
+            self.indices = np.arange(self.num_samples)
 
-        self.num_samples = self.samples.shape[0]
-        self.indices = np.arange(self.num_samples)
         self.log(f"New dataset size: {self.num_samples}, batches: {len(self)}")
 
-    def _update_samples_and_targets(self):
-        if not self.client:
-            self.client = Client(self.address, self.cluster)
-            
+    def _update_samples_and_targets(self) -> None:
         self.log(f"Rank {self.replica_rank} out of {self.num_replicas} replicas")
 
         for uploader_idx, uploader_key in enumerate(self.uploader_keys):
             if uploader_key:
                 self.client.use_list_ensemble_prefix(True)
                 self.client.set_data_source(uploader_key)
 
@@ -469,22 +476,25 @@
                     for idx in range(
                         self.next_indices[uploader_idx], list_length, self.num_replicas
                     )
                 ]
                 self._add_samples(indices)
                 self.next_indices[uploader_idx] = indices[-1] + self.num_replicas
 
-    def update_data(self):
+    def update_data(self) -> None:
         if self.dynamic:
             self._update_samples_and_targets()
         if self.shuffle:
             np.random.shuffle(self.indices)
 
-    def _data_generation(self, indices):
+    def _data_generation(self, indices: np.ndarray) -> t.Tuple[np.ndarray, np.ndarray]:
         # Initialization
+        if self.samples is None:
+            raise ValueError("Samples have not been initialized")
+
         x = self.samples[indices]
 
         if self.need_targets:
             y = self.targets[indices]
         elif self.autoencoding:
             y = x
         else:
```

### Comparing `smartsim-0.4.2/smartsim/ml/tf/__init__.py` & `smartsim-0.5.0/smartsim/ml/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.2/smartsim/ml/tf/data.py` & `smartsim-0.5.0/smartsim/ml/tf/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
+import typing as t
 from tensorflow import keras
 
 from smartsim.ml import DataDownloader
 
 
 class _TFDataGenerationCommon(DataDownloader, keras.utils.Sequence):
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> t.Tuple[np.ndarray, np.ndarray]:
         if len(self) < 1:
             msg = "Not enough samples in generator for one batch. "
             msg += "Please run init_samples() or initialize generator with init_samples=True"
             raise ValueError(msg)
         # Generate indices of the batch
         indices = self.indices[index * self.batch_size : (index + 1) * self.batch_size]
 
@@ -43,24 +44,27 @@
         x, y = self._data_generation(indices)
 
         if y is not None:
             return x, y
         else:
             return x
 
-    def on_epoch_end(self):
+    def on_epoch_end(self) -> None:
         """Callback called at the end of each training epoch
 
         If `self.shuffle` is set to `True`, data is shuffled.
         """
         if self.shuffle:
             np.random.shuffle(self.indices)
 
-    def _data_generation(self, indices):
+    def _data_generation(self, indices: np.ndarray) -> t.Tuple[np.ndarray, np.ndarray]:
         # Initialization
+        if self.samples is None:
+            raise ValueError("No samples loaded for data generation")
+            
         x = self.samples[indices]
 
         if self.need_targets:
             y = self.targets[indices]
             if self.num_classes is not None:
                 y = keras.utils.to_categorical(y, num_classes=self.num_classes)
         elif self.autoencoding:
@@ -75,15 +79,15 @@
     """A class to download a dataset from the DB.
 
     Details about parameters and features of this class can be found
     in the documentation of ``DataDownloader``, of which it is just
     a TensorFlow-specialized sub-class with dynamic=False.
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: t.Any) -> None:
         dynamic = kwargs.pop("dynamic", False)
         kwargs["dynamic"] = False
         super().__init__(**kwargs)
         if dynamic:
             self.log(
                 "Static data generator cannot be started with dynamic=True, setting it to False"
             )
@@ -93,23 +97,23 @@
     """A class to download batches from the DB.
 
     Details about parameters and features of this class can be found
     in the documentation of ``DataDownloader``, of which it is just
     a TensorFlow-specialized sub-class with dynamic=True.
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: t.Any) -> None:
         dynamic = kwargs.pop("dynamic", True)
         kwargs["dynamic"] = True
         super().__init__(**kwargs)
         if not dynamic:
             self.log(
                 "Dynamic data generator cannot be started with dynamic=False, setting it to True"
             )
 
-    def on_epoch_end(self):
+    def on_epoch_end(self) -> None:
         """Callback called at the end of each training epoch
 
         Update data (the DB is queried for new batches) and
         if `self.shuffle` is set to `True`, data is also shuffled.
         """
         self.update_data()
```

### Comparing `smartsim-0.4.2/smartsim/ml/tf/utils.py` & `smartsim-0.5.0/smartsim/ml/tf/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from pathlib import Path
 
 import tensorflow as tf
+import keras
+import typing as t
 from tensorflow.python.framework.convert_to_constants import (
     convert_variables_to_constants_v2,
 )
 
 
-def freeze_model(model, output_dir, file_name):
+def freeze_model(model: keras.Model, output_dir: str, file_name: str) -> t.Tuple[str, t.List[str], t.List[str]]:
     """Freeze a Keras or TensorFlow Graph
 
     to use a Keras or TensorFlow model in SmartSim, the model
     must be frozen and the inputs and outputs provided to the
     smartredis.client.set_model_from_file() method.
 
     This utiliy function provides everything users need to take
@@ -74,15 +76,15 @@
         name=file_name,
         as_text=False,
     )
     model_file_path = str(Path(output_dir, file_name).resolve())
     return model_file_path, input_names, output_names
 
 
-def serialize_model(model):
+def serialize_model(model: keras.Model) -> t.Tuple[str, t.List[str], t.List[str]]:
     """Serialize a Keras or TensorFlow Graph
 
     to use a Keras or TensorFlow model in SmartSim, the model
     must be frozen and the inputs and outputs provided to the
     smartredis.client.set_model() method.
 
     This utiliy function provides everything users need to take
```

### Comparing `smartsim-0.4.2/smartsim/ml/torch/__init__.py` & `smartsim-0.5.0/smartsim/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,29 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .data import DataLoader, DynamicDataGenerator, StaticDataGenerator
+
+# Statuses that are applied to jobs
+STATUS_RUNNING = "Running"
+STATUS_COMPLETED = "Completed"
+STATUS_CANCELLED = "Cancelled"
+STATUS_FAILED = "Failed"
+STATUS_NEW = "New"
+STATUS_PAUSED = "Paused"
+
+# SmartSim status mapping
+SMARTSIM_STATUS = {
+    "Running": STATUS_RUNNING,
+    "Paused": STATUS_PAUSED,
+    "Completed": STATUS_COMPLETED,
+    "Cancelled": STATUS_CANCELLED,
+    "Failed": STATUS_FAILED,
+    "New": STATUS_NEW,
+}
+
+# Status groupings
+TERMINAL_STATUSES = {STATUS_CANCELLED, STATUS_COMPLETED, STATUS_FAILED}
+LIVE_STATUSES = {STATUS_RUNNING, STATUS_PAUSED, STATUS_NEW}
```

### Comparing `smartsim-0.4.2/smartsim/ml/torch/data.py` & `smartsim-0.5.0/smartsim/ml/torch/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,41 +22,42 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
 import torch
+import typing as t
 from smartredis import Client, Dataset
 
 from smartsim.ml.data import DataDownloader
 
 
 class _TorchDataGenerationCommon(DataDownloader, torch.utils.data.IterableDataset):
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: t.Any) -> None:
         init_samples = kwargs.pop("init_samples", False)
         kwargs["init_samples"] = False
         super().__init__(**kwargs)
         if init_samples:
             self.log(
                 "PyTorch Data Generator has to be created with init_samples=False. Setting it to False automatically."
             )
 
-    def _add_samples(self, indices):
+    def _add_samples(self, indices: t.List[int]) -> None:
         if self.client is None:
             client = Client(self.address, self.cluster)
         else:
             client = self.client
 
+        datasets: t.List[Dataset] = []
         if self.num_replicas == 1:
-            datasets: list[Dataset] = client.get_dataset_list_range(
+            datasets = client.get_dataset_list_range(
                 self.list_name, start_index=indices[0], end_index=indices[-1]
             )
         else:
-            datasets: list[Dataset] = []
             for idx in indices:
                 datasets += client.get_dataset_list_range(
                     self.list_name, start_index=idx, end_index=idx
                 )
 
         if self.samples is None:
             self.samples = torch.tensor(datasets[0].get_tensor(self.sample_name))
@@ -71,15 +72,16 @@
                 (self.samples, torch.tensor(dataset.get_tensor(self.sample_name)))
             )
             if self.need_targets:
                 self.targets = torch.cat(
                     (self.targets, torch.tensor(dataset.get_tensor(self.target_name)))
                 )
 
-        self.num_samples = self.samples.shape[0]
+        if self.samples is not None:
+            self.num_samples = self.samples.shape[0]
         self.indices = np.arange(self.num_samples)
         self.log(f"New dataset size: {self.num_samples}, batches: {len(self)}")
 
 
 class StaticDataGenerator(_TorchDataGenerationCommon):
     """A class to download a dataset from the DB.
 
@@ -89,15 +91,15 @@
 
     When used in the DataLoader defined in this class, samples are initialized
     automatically before training. Other data loaders using this generator
     should implement the same behavior.
 
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: t.Any) -> None:
         dynamic = kwargs.pop("dynamic", False)
         kwargs["dynamic"] = False
         super().__init__(**kwargs)
         if dynamic:
             self.log(
                 "Static data generator cannot be started with dynamic=True, setting it to False"
             )
@@ -111,51 +113,51 @@
     a PyTorch-specialized sub-class with dynamic=True and init_samples=False.
 
     When used in the DataLoader defined in this class, samples are initialized
     automatically before training. Other data loaders using this generator
     should implement the same behavior.
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: t.Any) -> None:
         dynamic = kwargs.pop("dynamic", True)
         kwargs["dynamic"] = True
         super().__init__(**kwargs)
         if not dynamic:
             self.log(
                 "Dynamic data generator cannot be started with dynamic=False, setting it to True"
             )
 
 
+def _worker_init_fn(worker_id: int) -> None:
+    worker_info = torch.utils.data.get_worker_info()
+    dataset = worker_info.dataset  # the dataset copy in this worker process
+
+    worker_id = worker_info.id
+    num_workers = worker_info.num_workers
+
+    dataset.set_replica_parameters(
+        replica_rank=dataset.replica_rank * num_workers + worker_id,
+        num_replicas=dataset.num_replicas * num_workers,
+    )
+    dataset.log(
+        f"Worker {worker_id+1}/{num_workers}: dataset replica {dataset.replica_rank+1}/{dataset.num_replicas}"
+    )
+
+    dataset.init_samples()
+    
+
 class DataLoader(torch.utils.data.DataLoader):  # pragma: no cover
     """DataLoader to be used as a wrapper of StaticDataGenerator or DynamicDataGenerator
 
     This is just a sub-class of ``torch.utils.data.DataLoader`` which
     sets up sources of a data generator correctly. DataLoader parameters
     such as `num_workers` can be passed at initialization. `batch_size` should always
     be set to None.
     """
 
-    def __init__(self, dataset: _TorchDataGenerationCommon, **kwargs):
+    def __init__(self, dataset: _TorchDataGenerationCommon, **kwargs: t.Any) -> None:
         super().__init__(
             dataset,
-            worker_init_fn=self.worker_init_fn,
+            worker_init_fn=_worker_init_fn,
             persistent_workers=True,
             **kwargs,
         )
-
-    @staticmethod
-    def worker_init_fn(worker_id):
-        worker_info = torch.utils.data.get_worker_info()
-        dataset = worker_info.dataset  # the dataset copy in this worker process
-
-        worker_id = worker_info.id
-        num_workers = worker_info.num_workers
-
-        dataset.set_replica_parameters(
-            replica_rank=dataset.replica_rank * num_workers + worker_id,
-            num_replicas=dataset.num_replicas * num_workers,
-        )
-        dataset.log(
-            f"Worker {worker_id+1}/{num_workers}: dataset replica {dataset.replica_rank+1}/{dataset.num_replicas}"
-        )
-
-        dataset.init_samples()
```

### Comparing `smartsim-0.4.2/smartsim/settings/__init__.py` & `smartsim-0.5.0/smartsim/settings/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .alpsSettings import AprunSettings
-from .base import RunSettings
+from .base import RunSettings, SettingsBase
 from .cobaltSettings import CobaltBatchSettings
 from .containers import Container, Singularity
 from .lsfSettings import BsubBatchSettings, JsrunSettings
 from .mpiSettings import MpiexecSettings, MpirunSettings, OrterunSettings
 from .palsSettings import PalsMpiexecSettings
 from .pbsSettings import QsubBatchSettings
 from .slurmSettings import SbatchSettings, SrunSettings
@@ -40,13 +40,14 @@
     "BsubBatchSettings",
     "JsrunSettings",
     "MpirunSettings",
     "MpiexecSettings",
     "OrterunSettings",
     "QsubBatchSettings",
     "RunSettings",
+    "SettingsBase",
     "SbatchSettings",
     "SrunSettings",
     "PalsMpiexecSettings",
     "Container",
     "Singularity",
 ]
```

### Comparing `smartsim-0.4.2/smartsim/settings/alpsSettings.py` & `smartsim-0.5.0/smartsim/settings/alpsSettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,182 +20,192 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+import typing as t
+
 from ..error import SSUnsupportedError
 from .base import RunSettings
 
 
 class AprunSettings(RunSettings):
-    def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
+    def __init__(
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ):
         """Settings to run job with ``aprun`` command
 
         ``AprunSettings`` can be used for both the `pbs` and `cobalt`
         launchers.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command="aprun",
             run_args=run_args,
             env_vars=env_vars,
             **kwargs,
         )
-        self.mpmd = []
+        self.mpmd: t.List[RunSettings] = []
 
-    def make_mpmd(self, aprun_settings):
+    def make_mpmd(self, settings: RunSettings) -> None:
         """Make job an MPMD job
 
         This method combines two ``AprunSettings``
         into a single MPMD command joined with ':'
 
-        :param aprun_settings: ``AprunSettings`` instance
-        :type aprun_settings: AprunSettings
+        :param settings: ``AprunSettings`` instance
+        :type settings: AprunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
         if self.container:
             raise SSUnsupportedError(
                 "Containerized MPMD workloads are not yet supported."
             )
-        self.mpmd.append(aprun_settings)
+        self.mpmd.append(settings)
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-pe``
 
         :param cpus_per_task: number of cpus to use per task
         :type cpus_per_task: int
         """
         self.run_args["cpus-per-pe"] = int(cpus_per_task)
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--pes``
 
         :param tasks: number of tasks
         :type tasks: int
         """
         self.run_args["pes"] = int(tasks)
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--pes-per-node``
 
         :param tasks_per_node: number of tasks per node
         :type tasks_per_node: int
         """
         self.run_args["pes-per-node"] = int(tasks_per_node)
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.run_args["node-list"] = ",".join(host_list)
 
-    def set_hostlist_from_file(self, file_path):
+    def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the node list
 
         This sets ``--node-list-file``
 
         :param file_path: Path to the hostlist file
         :type file_path: str
         """
-        self.run_args["node-list-file"] = str(file_path)
+        self.run_args["node-list-file"] = file_path
 
-    def set_excluded_hosts(self, host_list):
+    def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.run_args["exclude-node-list"] = ",".join(host_list)
 
-    def set_cpu_bindings(self, bindings):
+    def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--cpu-binding``
 
         :param bindings: List of cpu numbers
         :type bindings: list[int] | int
         """
         if isinstance(bindings, int):
             bindings = [bindings]
         self.run_args["cpu-binding"] = ",".join(str(int(num)) for num in bindings)
 
-    def set_memory_per_node(self, memory_per_node):
+    def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the real memory required per node
 
         This sets ``--memory-per-pe`` in megabytes
 
         :param memory_per_node: Per PE memory limit in megabytes
         :type memory_per_node: int
         """
         self.run_args["memory-per-pe"] = int(memory_per_node)
 
-    def set_verbose_launch(self, verbose):
+    def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--debug`` arg to the highest level
 
         :param verbose: Whether the job should be run verbosely
         :type verbose: bool
         """
         if verbose:
             self.run_args["debug"] = 7
         else:
             self.run_args.pop("debug", None)
 
-    def set_quiet_launch(self, quiet):
+    def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
         :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return a list of ALPS formatted run arguments
 
         :return: list of ALPS arguments for these settings
         :rtype: list[str]
         """
         # args launcher uses
         args = []
@@ -210,27 +220,27 @@
                 else:
                     if short_arg:
                         args += [prefix + opt, str(value)]
                     else:
                         args += ["=".join((prefix + opt, str(value)))]
         return args
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for aprun
 
         :return: list of env vars
         :rtype: list[str]
         """
         formatted = []
         if self.env_vars:
             for name, value in self.env_vars.items():
                 formatted += ["-e", name + "=" + str(value)]
         return formatted
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         Walltime is given in total number of seconds
 
         :param walltime: wall time
         :type walltime: str
         """
```

### Comparing `smartsim-0.4.2/smartsim/settings/base.py` & `smartsim-0.5.0/smartsim/settings/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,32 +18,41 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from __future__ import annotations
+
+import copy
+import typing as t
+
+from smartsim.settings.containers import Container
 
 from .._core.utils.helpers import expand_exe_path, fmt_dict, init_default, is_valid_cmd
 from ..log import get_logger
 
 logger = get_logger(__name__)
 
 
-class RunSettings:
+class SettingsBase:
+    ...
+
+class RunSettings(SettingsBase):
     def __init__(
         self,
-        exe,
-        exe_args=None,
-        run_command="",
-        run_args=None,
-        env_vars=None,
-        container=None,
-        **kwargs,
-    ):
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_command: str = "",
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        container: t.Optional[Container] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Run parameters for a ``Model``
 
         The base ``RunSettings`` class should only be used with the `local`
         launcher on single node, workstations, or laptops.
 
         If no ``run_command`` is specified, the executable will be launched
         locally.
@@ -69,214 +78,234 @@
         :type run_args: dict[str, str], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         :param container: container type for workload (e.g. "singularity"), defaults to None
         :type container: Container, optional
         """
         # Do not expand executable if running within a container
-        if container:
-            self.exe = [exe]
-        else:
-            self.exe = [expand_exe_path(exe)]
-
-        self.exe_args = self._set_exe_args(exe_args)
-        self.run_args = init_default({}, run_args, dict)
-        self.env_vars = init_default({}, env_vars, dict)
+        self.exe = [exe] if container else [expand_exe_path(exe)]
+        self.exe_args = exe_args or []
+        self.run_args = run_args or {}
+        self.env_vars = env_vars or {}
         self.container = container
         self._run_command = run_command
         self.in_batch = False
-        self.colocated_db_settings = None
+        self.colocated_db_settings: t.Optional[t.Dict[str, str]] = None
+
+    @property
+    def exe_args(self) -> t.Union[str, t.List[str]]:
+        return self._exe_args
+
+    @exe_args.setter
+    def exe_args(self, value: t.Union[str, t.List[str], None]) -> None:
+        self._exe_args = self._build_exe_args(value)
 
+    @property
+    def run_args(self) -> t.Dict[str, t.Union[int, str, float, None]]:
+        return self._run_args
+    
+    @run_args.setter
+    def run_args(self, value: t.Dict[str, t.Union[int, str, float, None]]) -> None:
+        self._run_args = copy.deepcopy(value)
+
+    @property
+    def env_vars(self) -> t.Dict[str, t.Optional[str]]:
+        return self._env_vars
+    
+    @env_vars.setter
+    def env_vars(self, value: t.Dict[str, t.Optional[str]]) -> None:
+        self._env_vars = copy.deepcopy(value)
+    
     # To be overwritten by subclasses. Set of reserved args a user cannot change
     reserved_run_args = set()  # type: set[str]
 
-    def set_nodes(self, nodes):
+    def set_nodes(self, nodes: int) -> None:
         """Set the number of nodes
 
         :param nodes: number of nodes to run with
         :type nodes: int
         """
         logger.warning(
             (
                 "Node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks to launch
 
         :param tasks: number of tasks to launch
         :type tasks: int
         """
         logger.warning(
             (
                 "Task specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
         :type tasks_per_node: int
         """
         logger.warning(
             (
                 "Task per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_task_map(self, task_mapping):
+    def set_task_map(self, task_mapping: str) -> None:
         """Set a task mapping
 
         :param task_mapping: task mapping
         :type task_mapping: str
         """
         logger.warning(
             (
                 "Task mapping specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus per task
 
         :param cpus_per_task: number of cpus per task
         :type cpus_per_task: int
         """
         logger.warning(
             (
                 "CPU per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         """
         logger.warning(
             (
                 "Hostlist specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_hostlist_from_file(self, file_path):
+    def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to specify the hostlist for this job
 
         :param file_path: Path to the hostlist file
         :type file_path: str
         """
         logger.warning(
             (
                 "Hostlist from file specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_excluded_hosts(self, host_list):
+    def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
         :type host_list: str | list[str]
         """
         logger.warning(
             (
                 "Excluded host list specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_cpu_bindings(self, bindings):
+    def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Set the cores to which MPI processes are bound
 
         :param bindings: List specifing the cores to which MPI processes are bound
         :type bindings: list[int] | int
         """
         logger.warning(
             (
                 "CPU binding specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_memory_per_node(self, memory_per_node):
+    def set_memory_per_node(self, memory_per_node: int) -> None:
         """Set the amount of memory required per node in megabytes
 
         :param memory_per_node: Number of megabytes per node
         :type memory_per_node: int
         """
         logger.warning(
             (
                 "Memory per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_verbose_launch(self, verbose):
+    def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         :param verbose: Whether the job should be run verbosely
         :type verbose: bool
         """
         logger.warning(
             (
                 "Verbose specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_quiet_launch(self, quiet):
+    def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         :param quiet: Whether the job should be run quietly
         :type quiet: bool
         """
         logger.warning(
             (
                 "Quiet specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_broadcast(self, dest_path=None):
+    def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy executable file to allocated compute nodes
 
         :param dest_path: Path to copy an executable file
         :type dest_path: str | None
         """
         logger.warning(
             (
                 "Broadcast specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_time(self, hours=0, minutes=0, seconds=0):
+    def set_time(self, hours: int = 0, minutes: int = 0, seconds: int = 0) -> None:
         """Automatically format and set wall time
 
         :param hours: number of hours to run job
         :type hours: int
         :param minutes: number of minutes to run job
         :type minutes: int
         :param seconds: number of seconds to run job
         :type seconds: int
         """
         return self.set_walltime(
             self._fmt_walltime(int(hours), int(minutes), int(seconds))
         )
 
-    def _fmt_walltime(self, hours, minutes, seconds):
+    def _fmt_walltime(self, hours: int, minutes: int, seconds: int) -> str:
         """Convert hours, minutes, and seconds into valid walltime format
 
         By defualt the formatted wall time is the total number of seconds.
 
         :param hours: number of hours to run job
         :type hours: int
         :param minutes: number of minutes to run job
@@ -287,68 +316,68 @@
         :rtype: str
         """
         time_ = hours * 3600
         time_ += minutes * 60
         time_ += seconds
         return str(time_)
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the formatted walltime
 
         :param walltime: Time in format required by launcher``
         :type walltime: str
         """
         logger.warning(
             (
                 "Walltime specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_binding(self, binding):
+    def set_binding(self, binding: str) -> None:
         """Set binding
 
         :param binding: Binding
         :type binding: str
         """
         logger.warning(
             (
                 "binding specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def set_mpmd_preamble(self, preamble_lines):
+    def set_mpmd_preamble(self, preamble_lines: t.List[str]) -> None:
         """Set preamble to a file to make a job MPMD
 
         :param preamble_lines: lines to put at the beginning of a file.
         :type preamble_lines: list[str]
         """
         logger.warning(
             (
                 "MPMD preamble specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
-    def make_mpmd(self, settings):
+    def make_mpmd(self, settings: RunSettings) -> None:
         """Make job an MPMD job
 
         :param settings: ``RunSettings`` instance
-        :type aprun_settings: RunSettings
+        :type settings: RunSettings
         """
         logger.warning(
             (
                 "Make MPMD specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     @property
-    def run_command(self):
+    def run_command(self) -> t.Optional[str]:
         """Return the launch binary used to launch the executable
 
         Attempt to expand the path to the executable if possible
 
         :returns: launch binary e.g. mpiexec
         :type: str | None
         """
@@ -360,15 +389,15 @@
                 return expand_exe_path(cmd)
             # command is not valid, so return it as is
             # it may be on the compute nodes but not local machine
             return cmd
         # run without run command
         return None
 
-    def update_env(self, env_vars):
+    def update_env(self, env_vars: t.Dict[str, t.Union[str, int, float, bool]]) -> None:
         """Update the job environment variables
 
         To fully inherit the current user environment, add the
         workload-manager-specific flag to the launch command through the
         :meth:`add_exe_args` method. For example, ``--export=ALL`` for
         slurm, or ``-V`` for PBS/aprun.
 
@@ -381,31 +410,33 @@
         # Coerce env_vars values to str as a convenience to user
         for env, val in env_vars.items():
             if not isinstance(val, val_types):
                 raise TypeError(
                     f"env_vars[{env}] was of type {type(val)}, not {val_types}"
                 )
             else:
-                self.env_vars[env] = val
+                self.env_vars[env] = str(val)
 
-    def add_exe_args(self, args):
+    def add_exe_args(self, args: t.Union[str, t.List[str]]) -> None:
         """Add executable arguments to executable
 
         :param args: executable arguments
         :type args: str | list[str]
         :raises TypeError: if exe args are not strings
         """
         if isinstance(args, str):
             args = args.split()
+        
         for arg in args:
             if not isinstance(arg, str):
                 raise TypeError("Executable arguments should be a list of str")
-            self.exe_args.append(arg)
 
-    def set(self, arg, value=None, condition=True):
+        self._exe_args.extend(args)
+
+    def set(self, arg: str, value: t.Optional[str] = None, condition: bool = True) -> None:
         """Allows users to set individual run arguments.
 
         A method that allows users to set run arguments after object
         instantiation. Does basic formatting such as stripping leading dashes.
         If the argument has been set previously, this method will log warning
         but ultimately comply.
 
@@ -468,19 +499,22 @@
             )
             return
 
         if arg in self.run_args and value != self.run_args[arg]:
             logger.warning(f"Overwritting argument '{arg}' with value '{value}'")
         self.run_args[arg] = value
 
-    def _set_exe_args(self, exe_args):
+    @staticmethod
+    def _build_exe_args(exe_args: t.Optional[t.Union[str, t.List[str]]]) -> t.List[str]:
+        """Convert exe_args input to a desired collection format"""
         if exe_args:
             if isinstance(exe_args, str):
                 return exe_args.split()
             if isinstance(exe_args, list):
+                exe_args = copy.deepcopy(exe_args)
                 plain_type = all([isinstance(arg, (str)) for arg in exe_args])
                 if not plain_type:
                     nested_type = all(
                         [
                             all([isinstance(arg, (str)) for arg in exe_args_list])
                             for exe_args_list in exe_args
                         ]
@@ -492,108 +526,121 @@
                     else:
                         return exe_args
                 return exe_args
             raise TypeError("Executable arguments were not list of str or str")
         else:
             return []
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return formatted run arguments
 
         For ``RunSettings``, the run arguments are passed
         literally with no formatting.
 
         :return: list run arguments for these settings
         :rtype: list[str]
         """
         formatted = []
         for arg, value in self.run_args.items():
             formatted.append(arg)
             formatted.append(str(value))
         return formatted
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Build environment variable string
 
         :returns: formatted list of strings to export variables
         :rtype: list[str]
         """
         formatted = []
         for key, val in self.env_vars.items():
             if val is None:
                 formatted.append(f"{key}=")
             else:
                 formatted.append(f"{key}={val}")
         return formatted
 
-    def __str__(self):  # pragma: no-cover
+    def __str__(self) -> str:  # pragma: no-cover
         string = f"Executable: {self.exe[0]}\n"
         string += f"Executable Arguments: {' '.join((self.exe_args))}"
         if self.run_command:
             string += f"\nRun Command: {self._run_command}"
         if self.run_args:
             string += f"\nRun Arguments:\n{fmt_dict(self.run_args)}"
         if self.colocated_db_settings:
             string += "\nCo-located Database: True"
         return string
 
 
-class BatchSettings:
-    def __init__(self, batch_cmd, batch_args=None, **kwargs):
+class BatchSettings(SettingsBase):
+    def __init__(
+        self,
+        batch_cmd: str,
+        batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         self._batch_cmd = batch_cmd
-        self.batch_args = init_default({}, batch_args, dict)
-        self._preamble = []
+        self.batch_args = batch_args or {}
+        self._preamble: t.List[str] = []
         self.set_nodes(kwargs.get("nodes", None))
         self.set_walltime(kwargs.get("time", None))
         self.set_queue(kwargs.get("queue", None))
         self.set_account(kwargs.get("account", None))
 
     @property
-    def batch_cmd(self):
+    def batch_cmd(self) -> str:
         """Return the batch command
 
         Tests to see if we can expand the batch command
         path. If we can, then returns the expanded batch
         command. If we cannot, returns the batch command as is.
 
         :returns: batch command
         :type: str
         """
         if is_valid_cmd(self._batch_cmd):
             return expand_exe_path(self._batch_cmd)
         else:
             return self._batch_cmd
 
-    def set_nodes(self, num_nodes):
+    @property
+    def batch_args(self) -> t.Dict[str, t.Optional[str]]:
+        return self._batch_args
+    
+    @batch_args.setter
+    def batch_args(self, value: t.Dict[str, t.Optional[str]]) -> None:
+        self._batch_args = copy.deepcopy(value) if value else {}
+
+    def set_nodes(self, num_nodes: int) -> None:
         raise NotImplementedError
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         raise NotImplementedError
 
-    def set_queue(self, queue):
+    def set_queue(self, queue: str) -> None:
         raise NotImplementedError
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         raise NotImplementedError
 
-    def set_account(self, account):
+    def set_account(self, account: str) -> None:
         raise NotImplementedError
 
-    def format_batch_args(self):
+    def format_batch_args(self) -> t.List[str]:
         raise NotImplementedError
 
-    def set_batch_command(self, command):
+    def set_batch_command(self, command: str) -> None:
         """Set the command used to launch the batch e.g. ``sbatch``
 
         :param command: batch command
         :type command: str
         """
         self._batch_cmd = command
 
-    def add_preamble(self, lines):
+    def add_preamble(self, lines: t.List[str]) -> None:
         """Add lines to the batch file preamble. The lines are just
         written (unmodified) at the beginning of the batch file
         (after the WLM directives) and can be used to e.g.
         start virtual environments before running the executables.
 
         :param line: lines to add to preamble.
         :type line: str or list[str]
@@ -601,12 +648,12 @@
         if isinstance(lines, str):
             self._preamble += [lines]
         elif isinstance(lines, list):
             self._preamble += lines
         else:
             raise TypeError("Expected str or List[str] for lines argument")
 
-    def __str__(self):  # pragma: no-cover
+    def __str__(self) -> str:  # pragma: no-cover
         string = f"Batch Command: {self._batch_cmd}"
         if self.batch_args:
             string += f"\nBatch arguments:\n{fmt_dict(self.batch_args)}"
         return string
```

### Comparing `smartsim-0.4.2/smartsim/settings/cobaltSettings.py` & `smartsim-0.5.0/smartsim/settings/cobaltSettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,28 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
 from .base import BatchSettings
 
 
 class CobaltBatchSettings(BatchSettings):
     def __init__(
-        self, nodes=None, time="", queue=None, account=None, batch_args=None, **kwargs
-    ):
+        self,
+        nodes: t.Optional[int] = None,
+        time: str = "",
+        queue: t.Optional[str] = None,
+        account: t.Optional[str] = None,
+        batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Specify settings for a Cobalt ``qsub`` batch launch
 
         If the argument doesn't have a parameter, put None
         as the value. e.g. {'exclusive': None}
 
         Initialization values provided (nodes, time, account)
         will overwrite the same arguments in ``batch_args`` if present
@@ -56,15 +63,15 @@
             nodes=nodes,
             account=account,
             queue=queue,
             time=time,
             **kwargs,
         )
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         Cobalt walltime can also be specified with number
         of minutes.
 
@@ -72,25 +79,25 @@
         :type walltime: str
         """
         # TODO check for formatting errors here
         # TODO catch existing "t" in batch_args
         if walltime:
             self.batch_args["time"] = walltime
 
-    def set_nodes(self, num_nodes):
+    def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         :param num_nodes: number of nodes
         :type num_nodes: int
         """
         # TODO catch existing "n" in batch_args
         if num_nodes:
-            self.batch_args["nodecount"] = int(num_nodes)
+            self.batch_args["nodecount"] = str(int(num_nodes))
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
@@ -98,43 +105,43 @@
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         hosts = ",".join(host_list)
         self.batch_args["attrs"] = f"location={hosts}"
 
-    def set_tasks(self, num_tasks):
+    def set_tasks(self, num_tasks: int) -> None:
         """Set total number of processes to start
 
         :param num_tasks: number of processes
         :type num_tasks: int
         """
-        self.batch_args["proccount"] = int(num_tasks)
+        self.batch_args["proccount"] = str(int(num_tasks))
 
-    def set_queue(self, queue):
+    def set_queue(self, queue: str) -> None:
         """Set the queue for the batch job
 
         :param queue: queue name
         :type queue: str
         """
         # TODO catch existing "q" in batch args
         if queue:
             self.batch_args["queue"] = str(queue)
 
-    def set_account(self, account):
+    def set_account(self, account: str) -> None:
         """Set the account for this batch job
 
         :param acct: account id
         :type acct: str
         """
         # TODO catch existing "A" in batch_args
         if account:
             self.batch_args["project"] = account
 
-    def format_batch_args(self):
+    def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: list of batch arguments for Sbatch
         :rtype: list[str]
         """
         restricted = [
             "o",
```

### Comparing `smartsim-0.4.2/smartsim/settings/containers.py` & `smartsim-0.5.0/smartsim/settings/containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import shutil
+import typing as t
 
 from ..log import get_logger
 
 logger = get_logger(__name__)
 
 
 class Container:
@@ -43,15 +44,17 @@
     :type args: str | list[str], optional
     :param mount: paths to mount (bind) from host machine into image.
     :type mount: str | list[str] | dict[str, str], optional
     :param working_directory: path of the working directory within the container
     :type working_directory: str
     """
 
-    def __init__(self, image, args="", mount="", working_directory=""):
+    def __init__(
+        self, image: str, args: str = "", mount: str = "", working_directory: str = ""
+    ) -> None:
         # Validate types
         if not isinstance(image, str):
             raise TypeError("image must be a str")
         elif not isinstance(args, (str, list)):
             raise TypeError("args must be a str | list")
         elif not isinstance(mount, (str, list, dict)):
             raise TypeError("mount must be a str | list | dict")
@@ -59,15 +62,15 @@
             raise TypeError("working_directory must be a str")
 
         self.image = image
         self.args = args
         self.mount = mount
         self.working_directory = working_directory
 
-    def _containerized_run_command(self, run_command: str):
+    def _containerized_run_command(self, run_command: str) -> str:
         """Return modified run_command with container commands prepended.
 
         :param run_command: run command from a RunSettings class
         :type run_command: str
         """
         raise NotImplementedError(
             f"Containerized run command specification not implemented for this Container type: {type(self)}"
@@ -93,18 +96,18 @@
     :type image: str
     :param args: arguments to 'singularity exec' command
     :type args: str | list[str], optional
     :param mount: paths to mount (bind) from host machine into image.
     :type mount: str | list[str] | dict[str, str], optional
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
 
-    def _container_cmds(self, default_working_directory=""):
+    def _container_cmds(self, default_working_directory: str = "") -> t.List[str]:
         """Return list of container commands to be inserted before exe.
             Container members are validated during this call.
 
         :raises TypeError: if object members are invalid types
         """
         serialized_args = ""
         if self.args:
@@ -154,15 +157,15 @@
         #   so warn instead of error
         if not singularity:
             logger.warning(
                 "Unable to find singularity. Continuing in case singularity is available on compute node"
             )
 
         # Construct containerized launch command
-        cmd_list = [singularity, "exec"]
+        cmd_list = [singularity or "singularity", "exec"]
         if working_directory:
             cmd_list.extend(["--pwd", working_directory])
 
         if serialized_args:
             cmd_list.append(serialized_args)
         if serialized_mount:
             cmd_list.extend(["--bind", serialized_mount])
```

### Comparing `smartsim-0.4.2/smartsim/settings/lsfSettings.py` & `smartsim-0.5.0/smartsim/settings/lsfSettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,214 +20,222 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
+import copy
+import typing as t
 from pprint import pformat
 
 from ..error import SSUnsupportedError
 from ..log import get_logger
 from .base import BatchSettings, RunSettings
 
 logger = get_logger(__name__)
 
 
 class JsrunSettings(RunSettings):
-    def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
+    def __init__(
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to run job with ``jsrun`` command
 
         ``JsrunSettings`` should only be used on LSF-based systems.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command="jsrun",
             run_args=run_args,
             env_vars=env_vars,
         )
 
         # Parameters needed for MPMD run
         self.erf_sets = {"host": "*", "cpu": "*", "ranks": "1"}
-        self.mpmd_preamble_lines = []
-        self.mpmd = []
-        self.individual_suffix = None
+        self.mpmd_preamble_lines: t.List[str] = []
+        self.mpmd: t.List[RunSettings] = []
+        self.individual_suffix = ""
 
     reserved_run_args = {"chdir", "h"}
 
-    def set_num_rs(self, num_rs):
+    def set_num_rs(self, num_rs: t.Union[str, int]) -> None:
         """Set the number of resource sets to use
 
         This sets ``--nrs``.
 
         :param num_rs: Number of resource sets or `ALL_HOSTS`
         :type num_rs: int or str
         """
         if isinstance(num_rs, str):
             self.run_args["nrs"] = num_rs
         else:
             self.run_args["nrs"] = int(num_rs)
 
-    def set_cpus_per_rs(self, cpus_per_rs):
+    def set_cpus_per_rs(self, cpus_per_rs: int) -> None:
         """Set the number of cpus to use per resource set
 
         This sets ``--cpu_per_rs``
 
         :param cpus_per_rs: number of cpus to use per resource set or ALL_CPUS
         :type cpus_per_rs: int or str
         """
         if self.colocated_db_settings:
-            db_cpus = self.colocated_db_settings["db_cpus"]
+            db_cpus = int(self.colocated_db_settings["db_cpus"])
             if cpus_per_rs < db_cpus:
                 raise ValueError(
                     f"Cannot set cpus_per_rs ({cpus_per_rs}) to less than db_cpus ({db_cpus})"
                 )
         if isinstance(cpus_per_rs, str):
             self.run_args["cpu_per_rs"] = cpus_per_rs
         else:
             self.run_args["cpu_per_rs"] = int(cpus_per_rs)
 
-    def set_gpus_per_rs(self, gpus_per_rs):
+    def set_gpus_per_rs(self, gpus_per_rs: int) -> None:
         """Set the number of gpus to use per resource set
 
         This sets ``--gpu_per_rs``
 
         :param gpus_per_rs: number of gpus to use per resource set or ALL_GPUS
         :type gpus_per_rs: int or str
         """
         if isinstance(gpus_per_rs, str):
             self.run_args["gpu_per_rs"] = gpus_per_rs
         else:
             self.run_args["gpu_per_rs"] = int(gpus_per_rs)
 
-    def set_rs_per_host(self, rs_per_host):
+    def set_rs_per_host(self, rs_per_host: int) -> None:
         """Set the number of resource sets to use per host
 
         This sets ``--rs_per_host``
 
         :param rs_per_host: number of resource sets to use per host
         :type rs_per_host: int
         """
         self.run_args["rs_per_host"] = int(rs_per_host)
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--np``
 
         :param tasks: number of tasks
         :type tasks: int
         """
         self.run_args["np"] = int(tasks)
 
-    def set_tasks_per_rs(self, tasks_per_rs):
+    def set_tasks_per_rs(self, tasks_per_rs: int) -> None:
         """Set the number of tasks per resource set
 
         This sets ``--tasks_per_rs``
 
         :param tasks_per_rs: number of tasks per resource set
         :type tasks_per_rs: int
         """
         self.run_args["tasks_per_rs"] = int(tasks_per_rs)
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per resource set.
 
         This function is an alias for `set_tasks_per_rs`.
 
         :param tasks_per_node: number of tasks per resource set
         :type tasks_per_node: int
         """
-        self.set_tasks_per_rs(tasks_per_node)
+        self.set_tasks_per_rs(int(tasks_per_node))
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus per tasks.
 
         This function is an alias for `set_cpus_per_rs`.
 
         :param cpus_per_task: number of cpus per resource set
         :type cpus_per_task: int
         """
         self.set_cpus_per_rs(int(cpus_per_task))
 
-    def set_memory_per_rs(self, memory_per_rs):
+    def set_memory_per_rs(self, memory_per_rs: int) -> None:
         """Specify the number of megabytes of memory to assign to a resource set
 
         This sets ``--memory_per_rs``
 
         :param memory_per_rs: Number of megabytes per rs
         :type memory_per_rs: int
         """
         self.run_args["memory_per_rs"] = int(memory_per_rs)
 
-    def set_memory_per_node(self, memory_per_node):
+    def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the number of megabytes of memory to assign to a resource set
 
         Alias for `set_memory_per_rs`.
 
         :param memory_per_node: Number of megabytes per rs
         :type memory_per_node: int
         """
-        self.set_memory_per_rs(memory_per_node)
+        self.set_memory_per_rs(int(memory_per_node))
 
-    def set_binding(self, binding):
+    def set_binding(self, binding: str) -> None:
         """Set binding
 
         This sets ``--bind``
 
         :param binding: Binding, e.g. `packed:21`
         :type binding: str
         """
         self.run_args["bind"] = binding
 
-    def make_mpmd(self, jsrun_settings=None):
+    def make_mpmd(self, settings: RunSettings) -> None:
         """Make step an MPMD (or SPMD) job.
 
         This method will activate job execution through an ERF file.
 
         Optionally, this method adds an instance of ``JsrunSettings`` to
         the list of settings to be launched in the same ERF file.
 
-        :param aprun_settings: ``JsrunSettings`` instance, defaults to None
-        :type aprun_settings: JsrunSettings, optional
+        :param settings: ``JsrunSettings`` instance
+        :type settings: JsrunSettings, optional
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
 
-        if len(self.mpmd) == 0:
-            self.mpmd.append(self)
-        if jsrun_settings:
-            self.mpmd.append(jsrun_settings)
+        self.mpmd.append(settings)
 
-    def set_mpmd_preamble(self, preamble_lines):
+    def set_mpmd_preamble(self, preamble_lines: t.List[str]) -> None:
         """Set preamble used in ERF file. Typical lines include
         `oversubscribe-cpu : allow` or `overlapping-rs : allow`.
         Can be used to set `launch_distribution`. If it is not present,
         it will be inferred from the settings, or set to `packed` by
         default.
 
         :param preamble_lines: lines to put at the beginning of the ERF
                                file.
         :type preamble_lines: list[str]
         """
         self.mpmd_preamble_lines = preamble_lines
 
-    def set_erf_sets(self, erf_sets):
+    def set_erf_sets(self, erf_sets: t.Dict[str, str]) -> None:
         """Set resource sets used for ERF (SPMD or MPMD) steps.
 
         ``erf_sets`` is a dictionary used to fill the ERF
         line representing these settings, e.g.
         `{"host": "1", "cpu": "{0:21}, {21:21}", "gpu": "*"}`
         can be used to specify rank (or rank_count), hosts, cpus, gpus,
         and memory.
@@ -235,17 +243,17 @@
         `{"rank": "1, 2, 5"}`, while the key `rank_count` is used to specify
         the count only, as in `{"rank_count": "3"}`. If both are specified,
         only `rank` is used.
 
         :param hosts: dictionary of resources
         :type hosts: dict[str,str]
         """
-        self.erf_sets = erf_sets
+        self.erf_sets = copy.deepcopy(erf_sets)
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Format environment variables. Each variable needs
         to be passed with ``--env``. If a variable is set to ``None``,
         its value is propagated from the current environment.
 
         :returns: formatted list of strings to export variables
         :rtype: list[str]
         """
@@ -253,15 +261,15 @@
         for k, v in self.env_vars.items():
             if v:
                 format_str += ["-E", f"{k}={v}"]
             else:
                 format_str += ["-E", f"{k}"]
         return format_str
 
-    def set_individual_output(self, suffix=None):
+    def set_individual_output(self, suffix: t.Optional[str] = None) -> None:
         """Set individual std output.
 
         This sets ``--stdio_mode individual``
         and inserts the suffix into the output name. The resulting
         output name will be ``self.name + suffix + .out``.
 
         :param suffix: Optional suffix to add to output file names,
@@ -270,15 +278,15 @@
         :type suffix: str, optional
 
         """
         self.run_args["stdio_mode"] = "individual"
         if suffix:
             self.individual_suffix = suffix
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return a list of LSF formatted run arguments
 
         :return: list of LSF arguments for these settings
         :rtype: list[str]
         """
         # args launcher uses
         args = []
@@ -329,26 +337,26 @@
                 else:
                     if short_arg:
                         args += [prefix + opt, str(value)]
                     else:
                         args += ["=".join((prefix + opt, str(value)))]
         return args
 
-    def __str__(self):
+    def __str__(self) -> str:
         string = super().__str__()
         if self.mpmd:
             string += "\nERF settings: " + pformat(self.erf_sets)
         return string
 
-    def _prep_colocated_db(self, db_cpus):
+    def _prep_colocated_db(self, db_cpus: int) -> None:
         cpus_per_flag_set = False
         for cpu_per_rs_flag in ["cpu_per_rs", "c"]:
-            if cpu_per_rs_flag in self.run_args:
+            if run_arg_value := self.run_args.get(cpu_per_rs_flag, 0):
                 cpus_per_flag_set = True
-                cpu_per_rs = self.run_args[cpu_per_rs_flag]
+                cpu_per_rs = int(run_arg_value)
                 if cpu_per_rs < db_cpus:
                     msg = f"{cpu_per_rs_flag} flag was set to {cpu_per_rs}, "
                     msg += f"but colocated DB requires {db_cpus} CPUs per RS. Automatically setting "
                     msg += f"{cpu_per_rs_flag} flag to {db_cpus}"
                     logger.info(msg)
                     self.run_args[cpu_per_rs_flag] = db_cpus
         if not cpus_per_flag_set:
@@ -365,43 +373,43 @@
                 if rs_per_host != 1:
                     msg = f"{rs_per_host_flag} flag was set to {rs_per_host}, "
                     msg += (
                         f"but colocated DB requires running ONE resource set per host. "
                     )
                     msg += f"Automatically setting {rs_per_host_flag} flag to 1"
                     logger.info(msg)
-                    self.run_args[rs_per_host_flag] = 1
+                    self.run_args[rs_per_host_flag] = "1"
         if not rs_per_host_set:
             msg = f"Colocated DB requires one resource set per host. "
             msg += f" Automatically setting --rs_per_host==1"
             logger.info(msg)
             self.set_rs_per_host(1)
 
 
 class BsubBatchSettings(BatchSettings):
     def __init__(
         self,
-        nodes=None,
-        time=None,
-        project=None,
-        batch_args=None,
-        smts=None,
-        **kwargs,
-    ):
+        nodes: t.Optional[int] = None,
+        time: t.Optional[str] = None,
+        project: t.Optional[str] = None,
+        batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        smts: int = 0,
+        **kwargs: t.Any,
+    ) -> None:
         """Specify ``bsub`` batch parameters for a job
 
         :param nodes: number of nodes for batch, defaults to None
         :type nodes: int, optional
         :param time: walltime for batch job in format hh:mm, defaults to None
         :type time: str, optional
         :param project: project for batch launch, defaults to None
         :type project: str, optional
         :param batch_args: overrides for LSF batch arguments, defaults to None
         :type batch_args: dict[str, str], optional
-        :param smts: SMTs, defaults to None
+        :param smts: SMTs, defaults to 0
         :type smts: int, optional
         """
         if project:
             kwargs.pop("account", None)
         else:
             project = kwargs.pop("account", None)
 
@@ -410,22 +418,22 @@
             batch_args=batch_args,
             nodes=nodes,
             account=project,
             time=time,
             **kwargs,
         )
 
+        self.smts = 0
         if smts:
-            self.set_smts(smts)
-        else:
-            self.smts = None
+            self.set_smts(smts)            
+
         self.expert_mode = False
         self.easy_settings = ["ln_slots", "ln_mem", "cn_cu", "nnodes"]
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime
 
         This sets ``-W``.
 
         :param walltime: Time in hh:mm format, e.g. "10:00" for 10 hours,
                          if time is supplied in hh:mm:ss format, seconds
                          will be ignored and walltime will be set as ``hh:mm``
@@ -433,126 +441,131 @@
         """
         # For compatibility with other launchers, as explained in docstring
         if walltime:
             if len(walltime.split(":")) > 2:
                 walltime = ":".join(walltime.split(":")[:2])
         self.walltime = walltime
 
-    def set_smts(self, smts):
+    def set_smts(self, smts: int) -> None:
         """Set SMTs
 
         This sets ``-alloc_flags``. If the user sets
         SMT explicitly through ``-alloc_flags``, then that
         takes precedence.
 
         :param smts: SMT (e.g on Summit: 1, 2, or 4)
         :type smts: int
         """
-        self.smts = int(smts)
+        self.smts = smts
 
-    def set_project(self, project):
+    def set_project(self, project: str) -> None:
         """Set the project
 
         This sets ``-P``.
 
         :param time: project name
         :type time: str
         """
-        self.project = project
+        if project:
+            self.project = project
 
-    def set_account(self, account):
+    def set_account(self, account: str) -> None:
         """Set the project
 
         this function is an alias for `set_project`.
 
         :param account: project name
         :type account: str
         """
         self.set_project(account)
 
-    def set_nodes(self, num_nodes):
+    def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         This sets ``-nnodes``.
 
         :param nodes: number of nodes
         :type nodes: int
         """
         if num_nodes:
-            self.batch_args["nnodes"] = int(num_nodes)
+            self.batch_args["nnodes"] = str(int(num_nodes))
 
-    def set_expert_mode_req(self, res_req, slots):
+    def set_expert_mode_req(self, res_req: str, slots: int) -> None:
         """Set allocation for expert mode. This
         will activate expert mode (``-csm``) and
         disregard all other allocation options.
 
         This sets ``-csm -n slots -R res_req``
         """
         self.expert_mode = True
         self.batch_args["csm"] = "y"
         self.batch_args["R"] = res_req
-        self.batch_args["n"] = slots
+        self.batch_args["n"] = str(slots)
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.batch_args["m"] = '"' + " ".join(host_list) + '"'
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``-n``
 
         :param tasks: number of tasks
         :type tasks: int
         """
-        self.batch_args["n"] = int(tasks)
+        self.batch_args["n"] = str(int(tasks))
 
-    def set_queue(self, queue):
+    def set_queue(self, queue: str) -> None:
         """Set the queue for this job
 
         :param queue: The queue to submit the job on
         :type queue: str
         """
         if queue:
             self.batch_args["q"] = queue
 
-    def _format_alloc_flags(self):
+    def _format_alloc_flags(self) -> None:
         """Format ``alloc_flags`` checking if user already
         set it. Currently only adds SMT flag if missing
         and ``self.smts`` is set.
         """
 
         if self.smts:
             if not "alloc_flags" in self.batch_args.keys():
                 self.batch_args["alloc_flags"] = f"smt{self.smts}"
             else:
                 # Check if smt is in the flag, otherwise add it
-                flags = self.batch_args["alloc_flags"].strip('"').split()
+                flags: t.List[str] = []
+                if flags_arg := self.batch_args.get("alloc_flags", ""):
+                    flags = flags_arg.strip('"').split()
                 if not any([flag.startswith("smt") for flag in flags]):
                     flags.append(f"smt{self.smts}")
                     self.batch_args["alloc_flags"] = " ".join(flags)
 
         # Check if alloc_flags has to be enclosed in quotes
         if "alloc_flags" in self.batch_args.keys():
-            flags = self.batch_args["alloc_flags"].strip('"').split()
+            flags = []
+            if flags_arg := self.batch_args.get("alloc_flags", ""):
+                flags = flags_arg.strip('"').split()
             if len(flags) > 1:
                 self.batch_args["alloc_flags"] = '"' + " ".join(flags) + '"'
 
-    def format_batch_args(self):
+    def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: list of batch arguments for Qsub
         :rtype: list[str]
         """
         opts = []
```

### Comparing `smartsim-0.4.2/smartsim/settings/mpiSettings.py` & `smartsim-0.5.0/smartsim/settings/mpiSettings.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,37 +20,40 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
 import shutil
 import subprocess
+import typing as t
 
 from ..error import LauncherError, SSUnsupportedError
 from ..log import get_logger
 from .base import RunSettings
 
 logger = get_logger(__name__)
 
 
 class _BaseMPISettings(RunSettings):
     """Base class for all common arguments of MPI-standard run commands"""
 
     def __init__(
         self,
-        exe,
-        exe_args=None,
-        run_command="mpiexec",
-        run_args=None,
-        env_vars=None,
-        fail_if_missing_exec=True,
-        **kwargs,
-    ):
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_command: str = "mpiexec",
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        fail_if_missing_exec: bool = True,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to format run job with an MPI-standard binary
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
@@ -73,97 +76,97 @@
             exe,
             exe_args,
             run_command=run_command,
             run_args=run_args,
             env_vars=env_vars,
             **kwargs,
         )
-        self.mpmd = []
+        self.mpmd: t.List[RunSettings] = []
 
         if not shutil.which(self._run_command):
             msg = (
                 f"Cannot find {self._run_command}. Try passing the "
                 "full path via run_command."
             )
             if fail_if_missing_exec:
                 raise LauncherError(msg)
             else:
                 logger.warning(msg)
 
     reserved_run_args = {"wd", "wdir"}
 
-    def make_mpmd(self, mpirun_settings):
+    def make_mpmd(self, settings: RunSettings) -> None:
         """Make a mpmd workload by combining two ``mpirun`` commands
 
         This connects the two settings to be executed with a single
         Model instance
 
-        :param mpirun_settings: MpirunSettings instance
-        :type mpirun_settings: MpirunSettings
+        :param settings: MpirunSettings instance
+        :type settings: MpirunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
-        self.mpmd.append(mpirun_settings)
+        self.mpmd.append(settings)
 
-    def set_task_map(self, task_mapping):
+    def set_task_map(self, task_mapping: str) -> None:
         """Set ``mpirun`` task mapping
 
         this sets ``--map-by <mapping>``
 
         For examples, see the man page for ``mpirun``
 
         :param task_mapping: task mapping
         :type task_mapping: str
         """
-        self.run_args["map-by"] = str(task_mapping)
+        self.run_args["map-by"] = task_mapping
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--cpus-per-proc`` for MPI compliant implementations
 
         note: this option has been deprecated in openMPI 4.0+
         and will soon be replaced.
 
         :param cpus_per_task: number of tasks
         :type cpus_per_task: int
         """
         self.run_args["cpus-per-proc"] = int(cpus_per_task)
 
-    def set_cpu_binding_type(self, bind_type):
+    def set_cpu_binding_type(self, bind_type: str) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--bind-to`` for MPI compliant implementations
 
         :param bind_type: binding type
         :type bind_type: str
         """
-        self.run_args["bind-to"] = str(bind_type)
+        self.run_args["bind-to"] = bind_type
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
         :type tasks_per_node: int
         """
         self.run_args["npernode"] = int(tasks_per_node)
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``-n`` for MPI compliant implementations
 
         :param tasks: number of tasks
         :type tasks: int
         """
         self.run_args["n"] = int(tasks)
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Set the hostlist for the ``mpirun`` command
 
         This sets ``--host``
 
         :param host_list: list of host names
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
@@ -172,51 +175,51 @@
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.run_args["host"] = ",".join(host_list)
 
-    def set_hostlist_from_file(self, file_path):
+    def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the hostlist
 
         This sets ``--hostfile``
 
         :param file_path: Path to the hostlist file
         :type file_path: str
         """
-        self.run_args["hostfile"] = str(file_path)
+        self.run_args["hostfile"] = file_path
 
-    def set_verbose_launch(self, verbose):
+    def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--verbose``
 
         :param verbose: Whether the job should be run verbosely
         :type verbose: bool
         """
         if verbose:
             self.run_args["verbose"] = None
         else:
             self.run_args.pop("verbose", None)
 
-    def set_quiet_launch(self, quiet):
+    def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
         :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
-    def set_broadcast(self, dest_path=None):
+    def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy the specified executable(s) to remote machines
 
         This sets ``--preload-binary``
 
         :param dest_path: Destination path (Ignored)
         :type dest_path: str | None
         """
@@ -225,25 +228,25 @@
                 (
                     f"{type(self)} cannot set a destination path during broadcast. "
                     "Using session directory instead"
                 )
             )
         self.run_args["preload-binary"] = None
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the maximum number of seconds that a job will run
 
         This sets ``--timeout``
 
         :param walltime: number like string of seconds that a job will run in secs
         :type walltime: str
         """
-        self.run_args["timeout"] = str(walltime)
+        self.run_args["timeout"] = walltime
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return a list of MPI-standard formatted run arguments
 
         :return: list of MPI-standard arguments for these settings
         :rtype: list[str]
         """
         # args launcher uses
         args = []
@@ -254,15 +257,15 @@
                 prefix = "--"
                 if not value:
                     args += [prefix + opt]
                 else:
                     args += [prefix + opt, str(value)]
         return args
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for mpirun
 
         :return: list of env vars
         :rtype: list[str]
         """
         formatted = []
         env_string = "-x"
@@ -273,15 +276,22 @@
                     formatted += [env_string, "=".join((name, str(value)))]
                 else:
                     formatted += [env_string, name]
         return formatted
 
 
 class MpirunSettings(_BaseMPISettings):
-    def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
+    def __init__(
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to run job with ``mpirun`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
@@ -289,23 +299,30 @@
         None can be provided for arguments that do not have values.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "mpirun", run_args, env_vars, **kwargs)
 
 
 class MpiexecSettings(_BaseMPISettings):
-    def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
+    def __init__(
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to run job with ``mpiexec`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
@@ -313,15 +330,15 @@
         None can be provided for arguments that do not have values.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "mpiexec", run_args, env_vars, **kwargs)
 
         completed_process = subprocess.run(
             [self._run_command, "--help"], capture_output=True
@@ -330,15 +347,22 @@
         if "mpiexec.slurm" in help_statement:
             raise SSUnsupportedError(
                 "Slurm's wrapper for mpiexec is unsupported. Use slurmSettings instead"
             )
 
 
 class OrterunSettings(_BaseMPISettings):
-    def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
+    def __init__(
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to run job with ``orterun`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
@@ -346,12 +370,12 @@
         None can be provided for arguments that do not have values.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "orterun", run_args, env_vars, **kwargs)
```

### Comparing `smartsim-0.4.2/smartsim/settings/mpirunSettings.py` & `smartsim-0.5.0/smartsim/slurm.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,20 +20,25 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from warnings import simplefilter, warn
 
-from ..log import get_logger
-from .mpiSettings import MpiexecSettings, MpirunSettings, OrterunSettings
+from warnings import simplefilter, warn
 
-logger = get_logger(__name__)
+from .wlm.slurm import (
+    _get_alloc_cmd,
+    _get_system_partition_info,
+    get_allocation,
+    get_default_partition,
+    release_allocation,
+    validate,
+)
 
-simplefilter("once", DeprecationWarning)
-warn(
-    "mpirunSettings will be deprecated; use mpiSettings instead.",
-    DeprecationWarning,
-    stacklevel=2,
+simplefilter("once", category=DeprecationWarning)
+msg = (
+    "`smartsim.slurm` has been deprecated and will be removed in a future release.\n"
+    "Please update your code to use `smartsim.wlm.slurm`"
 )
+warn(msg, category=DeprecationWarning, stacklevel=2)
```

### Comparing `smartsim-0.4.2/smartsim/settings/palsSettings.py` & `smartsim-0.5.0/smartsim/settings/palsSettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import shutil
-import subprocess
+import typing as t
 
-from ..error import LauncherError, SSUnsupportedError
 from ..log import get_logger
 from .mpiSettings import _BaseMPISettings
 
 logger = get_logger(__name__)
 
 
 class PalsMpiexecSettings(_BaseMPISettings):
@@ -54,22 +52,22 @@
     :type run_args: dict[str, str], optional
     :param env_vars: environment vars to launch job with, defaults to None
     :type env_vars: dict[str, str], optional
     """
 
     def __init__(
         self,
-        exe,
-        exe_args=None,
-        run_command="mpiexec",
-        run_args=None,
-        env_vars=None,
-        fail_if_missing_exec=True,
-        **kwargs,
-    ):
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_command: str = "mpiexec",
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        fail_if_missing_exec: bool = True,
+        **kwargs: t.Any,
+    ) -> None:
         """Settings to format run job with an MPI-standard binary
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
@@ -77,15 +75,15 @@
         None can be provided for arguments that do not have values.
 
         :param exe: executable
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         :param fail_if_missing_exec: Throw an exception of the MPI command
                                      is missing. Otherwise, throw a warning
         :type fail_if_missing_exec: bool, optional
         """
         super().__init__(
@@ -94,77 +92,77 @@
             run_command=run_command,
             run_args=run_args,
             env_vars=env_vars,
             fail_if_missing_exec=fail_if_missing_exec,
             **kwargs,
         )
 
-    def set_task_map(self, task_mapping):
+    def set_task_map(self, task_mapping: str) -> None:
         """Set ``mpirun`` task mapping
 
         this sets ``--map-by <mapping>``
 
         For examples, see the man page for ``mpirun``
 
         :param task_mapping: task mapping
         :type task_mapping: str
         """
         logger.warning("set_task_map not supported under PALS")
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--cpus-per-proc`` for MPI compliant implementations
 
         note: this option has been deprecated in openMPI 4.0+
         and will soon be replaced.
 
         :param cpus_per_task: number of tasks
         :type cpus_per_task: int
         """
         logger.warning("set_cpus_per_task not supported under PALS")
 
-    def set_cpu_binding_type(self, bind_type):
+    def set_cpu_binding_type(self, bind_type: str) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--bind-to`` for MPI compliant implementations
 
         :param bind_type: binding type
         :type bind_type: str
         """
-        self.run_args["cpu-bind"] = str(bind_type)
+        self.run_args["cpu-bind"] = bind_type
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks
 
         :param tasks: number of total tasks to launch
         :type tasks: int
         """
         self.run_args["np"] = int(tasks)
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
         :type tasks_per_node: int
         """
         self.run_args["ppn"] = int(tasks_per_node)
 
-    def set_quiet_launch(self, quiet):
+    def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
         :type quiet: bool
         """
 
         logger.warning("set_quiet_launch not supported under PALS")
 
-    def set_broadcast(self, dest_path=None):
+    def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy the specified executable(s) to remote machines
 
         This sets ``--preload-binary``
 
         :param dest_path: Destination path (Ignored)
         :type dest_path: str | None
         """
@@ -173,23 +171,23 @@
                 (
                     f"{type(self)} cannot set a destination path during broadcast. "
                     "Using session directory instead"
                 )
             )
         self.run_args["transfer"] = None
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the maximum number of seconds that a job will run
 
         :param walltime: number like string of seconds that a job will run in secs
         :type walltime: str
         """
         logger.warning("set_walltime not supported under PALS")
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return a list of MPI-standard formatted run arguments
 
         :return: list of MPI-standard arguments for these settings
         :rtype: list[str]
         """
         # args launcher uses
         args = []
@@ -200,15 +198,15 @@
                 prefix = "--"
                 if not value:
                     args += [prefix + opt]
                 else:
                     args += [prefix + opt, str(value)]
         return args
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for mpirun
 
         :return: list of env vars
         :rtype: list[str]
         """
         formatted = []
```

### Comparing `smartsim-0.4.2/smartsim/settings/pbsSettings.py` & `smartsim-0.5.0/smartsim/settings/pbsSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,30 +20,32 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from .._core.utils import init_default
 from ..error import SmartSimError
 from .base import BatchSettings
 
 
 class QsubBatchSettings(BatchSettings):
     def __init__(
         self,
-        nodes=None,
-        ncpus=None,
-        time=None,
-        queue=None,
-        account=None,
-        resources=None,
-        batch_args=None,
-        **kwargs,
+        nodes: t.Optional[int] = None,
+        ncpus: t.Optional[int] = None,
+        time: t.Optional[str] = None,
+        queue: t.Optional[str] = None,
+        account: t.Optional[str] = None,
+        resources: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
     ):
         """Specify ``qsub`` batch parameters for a job
 
         ``nodes``, and ``ncpus`` are used to create the
         select statement for PBS if a select statement is not
         included in the ``resources``. If both are supplied
         the value for select statement supplied in ``resources``
@@ -60,134 +62,134 @@
         :param account: account for batch launch, defaults to None
         :type account: str, optional
         :param resources: overrides for resource arguments, defaults to None
         :type resources: dict[str, str], optional
         :param batch_args: overrides for PBS batch arguments, defaults to None
         :type batch_args: dict[str, str], optional
         """
-        self._time = None
-        self._nodes = None
+        self._time: t.Optional[str] = None
+        self._nodes: t.Optional[int] = None
         self._ncpus = ncpus
 
         # time, queue, nodes, and account set in parent class init
         super().__init__(
             "qsub",
             batch_args=batch_args,
             nodes=nodes,
             account=account,
             queue=queue,
             time=time,
             **kwargs,
         )
         self.resources = init_default({}, resources, dict)
-        self._hosts = None
+        self._hosts: t.List[str] = []
 
-    def set_nodes(self, num_nodes):
+    def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         If a select argument is provided in ``QsubBatchSettings.resources``
         this value will be overridden
 
         :param num_nodes: number of nodes
         :type num_nodes: int
         """
         if num_nodes:
             self._nodes = int(num_nodes)
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be a list of strings")
         self._hosts = host_list
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         If a walltime argument is provided in
         ``QsubBatchSettings.resources``, then
         this value will be overridden
 
         :param walltime: wall time
         :type walltime: str
         """
         if walltime:
             self._time = walltime
 
-    def set_queue(self, queue):
+    def set_queue(self, queue: str) -> None:
         """Set the queue for the batch job
 
         :param queue: queue name
         :type queue: str
         """
         if queue:
             self.batch_args["q"] = str(queue)
 
-    def set_ncpus(self, num_cpus):
+    def set_ncpus(self, num_cpus: t.Union[int, str]) -> None:
         """Set the number of cpus obtained in each node.
 
         If a select argument is provided in
         ``QsubBatchSettings.resources``, then
         this value will be overridden
 
         :param num_cpus: number of cpus per node in select
         :type num_cpus: int
         """
         self._ncpus = int(num_cpus)
 
-    def set_account(self, account):
+    def set_account(self, account: str) -> None:
         """Set the account for this batch job
 
         :param acct: account id
         :type acct: str
         """
         if account:
             self.batch_args["A"] = str(account)
 
-    def set_resource(self, resource_name, value):
+    def set_resource(self, resource_name: str, value: str) -> None:
         """Set a resource value for the Qsub batch
 
         If a select statement is provided, the nodes and ncpus
         arguments will be overridden. Likewise for Walltime
 
         :param resource_name: name of resource, e.g. walltime
         :type resource_name: str
         :param value: value
         :type value: str
         """
         # TODO add error checking here
         # TODO include option to overwrite place (warning for orchestrator?)
         self.resources[resource_name] = value
 
-    def format_batch_args(self):
+    def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: batch arguments for Qsub
         :rtype: list[str]
         :raises ValueError: if options are supplied without values
         """
         opts = self._create_resource_list()
         for opt, value in self.batch_args.items():
             prefix = "-"
             if not value:
                 raise ValueError("PBS options without values are not allowed")
             opts += [" ".join((prefix + opt, str(value)))]
         return opts
 
-    def _create_resource_list(self):
+    def _create_resource_list(self) -> t.List[str]:
         res = []
 
         # get select statement from resources or kwargs
         if "select" in self.resources:
             res += [f"-l select={str(self.resources['select'])}"]
         else:
             select = "-l select="
```

### Comparing `smartsim-0.4.2/smartsim/settings/settings.py` & `smartsim-0.5.0/smartsim/settings/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,23 +20,32 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import typing as t
+
 from .._core.utils.helpers import is_valid_cmd
 from ..error import SmartSimError
 from ..wlm import detect_launcher
 from . import *
+from ..settings import base
 
 
 def create_batch_settings(
-    launcher, nodes=None, time="", queue=None, account=None, batch_args=None, **kwargs
-):
+    launcher: str,
+    nodes: t.Optional[int] = None,
+    time: str = "",
+    queue: t.Optional[str] = None,
+    account: t.Optional[str] = None,
+    batch_args: t.Optional[t.Dict[str, str]] = None,
+    **kwargs: t.Any,
+) -> base.BatchSettings:
     """Create a ``BatchSettings`` instance
 
     See Experiment.create_batch_settings for details
 
     :param launcher: launcher for this experiment, if set to 'auto',
                      an attempt will be made to find an available launcher on the system
     :type launcher: str
@@ -85,23 +94,23 @@
     except KeyError:
         raise SmartSimError(
             f"User attempted to make batch settings for unsupported launcher {launcher}"
         ) from None
 
 
 def create_run_settings(
-    launcher,
-    exe,
-    exe_args=None,
-    run_command="auto",
-    run_args=None,
-    env_vars=None,
-    container=None,
-    **kwargs,
-):
+    launcher: str,
+    exe: str,
+    exe_args: t.Optional[t.List[str]] = None,
+    run_command: str = "auto",
+    run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+    env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+    container: t.Optional[Container] = None,
+    **kwargs: t.Any,
+) -> RunSettings:
     """Create a ``RunSettings`` instance.
 
     See Experiment.create_run_settings docstring for more details
 
     :param launcher: launcher to create settings for, if set to 'auto',
                      an attempt will be made to find an available launcher on the system
     :type launcher: str
@@ -111,14 +120,16 @@
     :type exe: str
     :param exe_args: arguments to pass to the executable
     :type exe_args: list[str], optional
     :param run_args: arguments to pass to the ``run_command``
     :type run_args: list[str], optional
     :param env_vars: environment variables to pass to the executable
     :type env_vars: dict[str, str], optional
+    :param container: container type for workload (e.g. "singularity"), defaults to None
+    :type container: Container, optional
     :return: the created ``RunSettings``
     :rtype: RunSettings
     :raises SmartSimError: if run_command=="auto" and detection fails
     """
     # all supported RunSettings child classes
     supported = {
         "aprun": AprunSettings,
@@ -132,39 +143,40 @@
     # run commands supported by each launcher
     # in order of suspected user preference
     by_launcher = {
         "slurm": ["srun", "mpirun", "mpiexec"],
         "pbs": ["aprun", "mpirun", "mpiexec"],
         "cobalt": ["aprun", "mpirun", "mpiexec"],
         "lsf": ["jsrun", "mpirun", "mpiexec"],
+        "local": [""],
     }
 
     if launcher == "auto":
         launcher = detect_launcher()
 
-    def _detect_command(launcher):
+    def _detect_command(launcher: str) -> str:
         if launcher in by_launcher:
+            if launcher == "local":
+                return ""
+
             for cmd in by_launcher[launcher]:
                 if is_valid_cmd(cmd):
                     return cmd
         msg = f"Could not automatically detect a run command to use for launcher {launcher}"
         msg += f"\nSearched for and could not find the following commands: {by_launcher[launcher]}"
         raise SmartSimError(msg)
 
     if run_command:
         run_command = run_command.lower()
     launcher = launcher.lower()
 
     # detect run_command automatically for all but local launcher
     if run_command == "auto":
         # no auto detection for local, revert to false
-        if launcher == "local":
-            run_command = None
-        else:
-            run_command = _detect_command(launcher)
+        run_command = _detect_command(launcher)
 
     # if user specified and supported or auto detection worked
     if run_command and run_command in supported:
         return supported[run_command](
             exe, exe_args, run_args, env_vars, container=container, **kwargs
         )
```

### Comparing `smartsim-0.4.2/smartsim/settings/slurmSettings.py` & `smartsim-0.5.0/smartsim/settings/slurmSettings.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,90 +20,98 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
 import datetime
 import os
-from typing import List, Tuple
+import typing as t
 
 from ..error import SSUnsupportedError
 from ..log import get_logger
 from .base import BatchSettings, RunSettings
 
 logger = get_logger(__name__)
 
 
 class SrunSettings(RunSettings):
     def __init__(
-        self, exe, exe_args=None, run_args=None, env_vars=None, alloc=None, **kwargs
-    ):
+        self,
+        exe: str,
+        exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
+        run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
+        env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        alloc: t.Optional[str] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Initialize run parameters for a slurm job with ``srun``
 
         ``SrunSettings`` should only be used on Slurm based systems.
 
         If an allocation is specified, the instance receiving these run
         parameters will launch on that allocation.
 
         :param exe: executable to run
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: list[str] | str, optional
         :param run_args: srun arguments without dashes, defaults to None
-        :type run_args: dict[str, str | None], optional
+        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment variables for job, defaults to None
         :type env_vars: dict[str, str], optional
         :param alloc: allocation ID if running on existing alloc, defaults to None
         :type alloc: str, optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command="srun",
             run_args=run_args,
             env_vars=env_vars,
             **kwargs,
         )
         self.alloc = alloc
-        self.mpmd = []
+        self.mpmd: t.List[RunSettings] = []
 
     reserved_run_args = {"chdir", "D"}
 
-    def set_nodes(self, nodes):
+    def set_nodes(self, nodes: int) -> None:
         """Set the number of nodes
 
         Effectively this is setting: ``srun --nodes <num_nodes>``
 
         :param nodes: number of nodes to run with
         :type nodes: int
         """
         self.run_args["nodes"] = int(nodes)
 
-    def make_mpmd(self, srun_settings):
+    def make_mpmd(self, settings: RunSettings) -> None:
         """Make a mpmd workload by combining two ``srun`` commands
 
         This connects the two settings to be executed with a single
         Model instance
 
-        :param srun_settings: SrunSettings instance
-        :type srun_settings: SrunSettings
+        :param settings: SrunSettings instance
+        :type settings: SrunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
         if self.container:
             raise SSUnsupportedError(
                 "Containerized MPMD workloads are not yet supported."
             )
-        self.mpmd.append(srun_settings)
+        self.mpmd.append(settings)
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         This sets ``--nodelist``
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
@@ -112,130 +120,130 @@
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.run_args["nodelist"] = ",".join(host_list)
 
-    def set_hostlist_from_file(self, file_path):
+    def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the node list
 
         This sets ``--nodefile``
 
         :param file_path: Path to the hostlist file
         :type file_path: str
         """
-        self.run_args["nodefile"] = str(file_path)
+        self.run_args["nodefile"] = file_path
 
-    def set_excluded_hosts(self, host_list):
+    def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
         :type host_list: list[str]
         :raises TypeError:
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.run_args["exclude"] = ",".join(host_list)
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-task``
 
         :param num_cpus: number of cpus to use per task
         :type num_cpus: int
         """
         self.run_args["cpus-per-task"] = int(cpus_per_task)
 
-    def set_tasks(self, tasks):
+    def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--ntasks``
 
         :param tasks: number of tasks
         :type tasks: int
         """
         self.run_args["ntasks"] = int(tasks)
 
-    def set_tasks_per_node(self, tasks_per_node):
+    def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--ntasks-per-node``
 
         :param tasks_per_node: number of tasks per node
         :type tasks_per_node: int
         """
         self.run_args["ntasks-per-node"] = int(tasks_per_node)
 
-    def set_cpu_bindings(self, bindings):
+    def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Bind by setting CPU masks on tasks
 
         This sets ``--cpu-bind`` using the ``map_cpu:<list>`` option
 
         :param bindings: List specifing the cores to which MPI processes are bound
         :type bindings: list[int] | int
         """
         if isinstance(bindings, int):
             bindings = [bindings]
         self.run_args["cpu_bind"] = "map_cpu:" + ",".join(
             str(int(num)) for num in bindings
         )
 
-    def set_memory_per_node(self, memory_per_node):
+    def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the real memory required per node
 
         This sets ``--mem`` in megabytes
 
         :param memory_per_node: Amount of memory per node in megabytes
         :type memory_per_node: int
         """
         self.run_args["mem"] = f"{int(memory_per_node)}M"
 
-    def set_verbose_launch(self, verbose):
+    def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--verbose``
 
         :param verbose: Whether the job should be run verbosely
         :type verbose: bool
         """
         if verbose:
             self.run_args["verbose"] = None
         else:
             self.run_args.pop("verbose", None)
 
-    def set_quiet_launch(self, quiet):
+    def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
         :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
-    def set_broadcast(self, dest_path=None):
+    def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy executable file to allocated compute nodes
 
         This sets ``--bcast``
 
         :param dest_path: Path to copy an executable file
         :type dest_path: str | None
         """
         self.run_args["bcast"] = dest_path
 
-    def _fmt_walltime(self, hours, minutes, seconds):
+    def _fmt_walltime(self, hours: int, minutes: int, seconds: int) -> str:
         """Convert hours, minutes, and seconds into valid walltime format
 
         Converts time to format HH:MM:SS
 
         :param hours: number of hours to run job
         :type hours: int
         :param minutes: number of minutes to run job
@@ -247,25 +255,25 @@
         """
         delta = datetime.timedelta(hours=hours, minutes=minutes, seconds=seconds)
         fmt_str = str(delta)
         if delta.seconds // 3600 < 10:
             fmt_str = "0" + fmt_str
         return fmt_str
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         :param walltime: wall time
         :type walltime: str
         """
         self.run_args["time"] = str(walltime)
 
-    def format_run_args(self):
+    def format_run_args(self) -> t.List[str]:
         """Return a list of slurm formatted run arguments
 
         :return: list of slurm arguments for these settings
         :rtype: list[str]
         """
         # add additional slurm arguments based on key length
         opts = []
@@ -277,15 +285,15 @@
             else:
                 if short_arg:
                     opts += [prefix + opt, str(value)]
                 else:
                     opts += ["=".join((prefix + opt, str(value)))]
         return opts
 
-    def check_env_vars(self):
+    def check_env_vars(self) -> None:
         """Warn a user trying to set a variable which is set in the environment
 
         Given Slurm's env var precedence, trying to export a variable which is already
         present in the environment will not work.
         """
         for k, v in self.env_vars.items():
             if "," not in str(v):
@@ -294,24 +302,24 @@
                 preexisting_var = os.environ.get(k, None)
                 if preexisting_var is not None:
                     msg = f"Variable {k} is set to {preexisting_var} in current environment. "
                     msg += f"If the job is running in an interactive allocation, the value {v} will not be set. "
                     msg += "Please consider removing the variable from the environment and re-run the experiment."
                     logger.warning(msg)
 
-    def format_env_vars(self):
+    def format_env_vars(self) -> t.List[str]:
         """Build bash compatible environment variable string for Slurm
 
         :returns: the formatted string of environment variables
         :rtype: list[str]
         """
         self.check_env_vars()
         return [f"{k}={v}" for k, v in self.env_vars.items() if "," not in str(v)]
 
-    def format_comma_sep_env_vars(self) -> Tuple[str, List[str]]:
+    def format_comma_sep_env_vars(self) -> t.Tuple[str, t.List[str]]:
         """Build environment variable string for Slurm
 
         Slurm takes exports in comma separated lists
         the list starts with all as to not disturb the rest of the environment
         for more information on this, see the slurm documentation for srun
 
         :returns: the formatted string of environment variables
@@ -329,23 +337,30 @@
             else:
                 exportable_env.append(kvp)
 
         # Append keys to exportable KVPs, e.g. `--export x1=v1,KO1,KO2`
         fmt_exported_env = ",".join(v for v in exportable_env + key_only)
 
         for mpmd in self.mpmd:
-            compound_mpmd_env = {k: v for k, v in mpmd.env_vars.items() if "," in v}
+            compound_mpmd_env = {k: v for k, v in mpmd.env_vars.items() if "," in str(v)}
             compound_mpmd_fmt = {f"{k}={v}" for k, v in compound_mpmd_env.items()}
             compound_env.extend(compound_mpmd_fmt)
 
         return fmt_exported_env, compound_env
 
 
 class SbatchSettings(BatchSettings):
-    def __init__(self, nodes=None, time="", account=None, batch_args=None, **kwargs):
+    def __init__(
+        self,
+        nodes: t.Optional[int] = None,
+        time: str = "",
+        account: t.Optional[str] = None,
+        batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
+        **kwargs: t.Any,
+    ) -> None:
         """Specify run parameters for a Slurm batch job
 
         Slurm `sbatch` arguments can be written into ``batch_args``
         as a dictionary. e.g. {'ntasks': 1}
 
         If the argument doesn't have a parameter, put `None`
         as the value. e.g. {'exclusive': None}
@@ -367,89 +382,89 @@
             batch_args=batch_args,
             nodes=nodes,
             account=account,
             time=time,
             **kwargs,
         )
 
-    def set_walltime(self, walltime):
+    def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         :param walltime: wall time
         :type walltime: str
         """
         # TODO check for formatting here
         if walltime:
             self.batch_args["time"] = walltime
 
-    def set_nodes(self, num_nodes):
+    def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         :param num_nodes: number of nodes
         :type num_nodes: int
         """
         if num_nodes:
-            self.batch_args["nodes"] = int(num_nodes)
+            self.batch_args["nodes"] = str(int(num_nodes))
 
-    def set_account(self, account):
+    def set_account(self, account: str) -> None:
         """Set the account for this batch job
 
         :param account: account id
         :type account: str
         """
         if account:
             self.batch_args["account"] = account
 
-    def set_partition(self, partition):
+    def set_partition(self, partition: str) -> None:
         """Set the partition for the batch job
 
         :param partition: partition name
         :type partition: str
         """
         self.batch_args["partition"] = str(partition)
 
-    def set_queue(self, queue):
+    def set_queue(self, queue: str) -> None:
         """alias for set_partition
 
         Sets the partition for the slurm batch job
 
         :param queue: the partition to run the batch job on
         :type queue: str
         """
         if queue:
             self.set_partition(queue)
 
-    def set_cpus_per_task(self, cpus_per_task):
+    def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-task``
 
         :param num_cpus: number of cpus to use per task
         :type num_cpus: int
         """
-        self.batch_args["cpus-per-task"] = int(cpus_per_task)
+        self.batch_args["cpus-per-task"] = str(int(cpus_per_task))
 
-    def set_hostlist(self, host_list):
+    def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
         :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
         self.batch_args["nodelist"] = ",".join(host_list)
 
-    def format_batch_args(self):
+    def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: batch arguments for Sbatch
         :rtype: list[str]
         """
         opts = []
         # TODO add restricted here
```

### Comparing `smartsim-0.4.2/smartsim/wlm/__init__.py` & `smartsim-0.5.0/smartsim/wlm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 from shutil import which
 from subprocess import run
+import typing as t
 
 from ..error import SSUnsupportedError
 from . import pbs as _pbs
 from . import slurm as _slurm
 
 
-def detect_launcher():
+def detect_launcher() -> str:
     """Detect available launcher."""
     # Precedence: PBS, Cobalt, LSF, Slurm, local
     if which("qsub") and which("qstat") and which("qdel"):
         qsub_version = run(
             ["qsub", "--version"], shell=False, capture_output=True, encoding="utf-8"
         )
         if "pbs" in (qsub_version.stdout).lower():
@@ -67,15 +68,15 @@
     if "COBALT_JOBID" in os.environ:
         return "cobalt"
     if "PBS_JOBID" in os.environ:
         return "pbs"
     return "local"
 
 
-def get_hosts(launcher=None):
+def get_hosts(launcher: t.Optional[str] = None) -> t.List[str]:
     """Get the name of the hosts used in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
     :type launcher: str | None
     :returns: Names of the hosts
     :rtype: list[str]
@@ -86,15 +87,15 @@
     if launcher == "pbs":
         return _pbs.get_hosts()
     if launcher == "slurm":
         return _slurm.get_hosts()
     raise SSUnsupportedError(f"SmartSim cannot get hosts for launcher `{launcher}`")
 
 
-def get_queue(launcher=None):
+def get_queue(launcher: t.Optional[str] = None) -> str:
     """Get the name of the queue used in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
     :type launcher: str | None
     :returns: Name of the queue
     :rtype: str
@@ -105,15 +106,15 @@
     if launcher == "pbs":
         return _pbs.get_queue()
     if launcher == "slurm":
         return _slurm.get_queue()
     raise SSUnsupportedError(f"SmartSim cannot get queue for launcher `{launcher}`")
 
 
-def get_tasks(launcher=None):
+def get_tasks(launcher: t.Optional[str] = None) -> int:
     """Get the number of tasks in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
     :type launcher: str | None
     :returns: Number of tasks
     :rtype: int
@@ -124,15 +125,15 @@
     if launcher == "pbs":
         return _pbs.get_tasks()
     if launcher == "slurm":
         return _slurm.get_tasks()
     raise SSUnsupportedError(f"SmartSim cannot get tasks for launcher `{launcher}`")
 
 
-def get_tasks_per_node(launcher=None):
+def get_tasks_per_node(launcher: t.Optional[str] = None) -> t.Dict[str, int]:
     """Get a map of nodes in an allocation to the number of tasks on each node.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
     :type launcher: str | None
     :returns: Map of nodes to number of processes on that node
     :rtype: dict[str, int]
```

### Comparing `smartsim-0.4.2/smartsim/wlm/pbs.py` & `smartsim-0.5.0/smartsim/wlm/pbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
 import os
+import typing as t
 from shutil import which
 
 from smartsim.error.errors import LauncherError, SmartSimError
 
 from .._core.launcher.pbs.pbsCommands import qstat
 
 
-def get_hosts():
+def get_hosts() -> t.List[str]:
     """Get the name of the hosts used in a PBS allocation.
 
     :returns: Names of the host nodes
     :rtype: list[str]
     :raises SmartSimError: ``PBS_NODEFILE`` is not set
     """
     hosts = []
@@ -50,27 +51,27 @@
         # account for repeats in PBS_NODEFILE
         return sorted(list(set(hosts)))
     raise SmartSimError(
         "Could not parse interactive allocation nodes from PBS_NODEFILE"
     )
 
 
-def get_queue():
+def get_queue() -> str:
     """Get the name of queue in a PBS allocation.
 
     :returns: The name of the queue
     :rtype: str
     :raises SmartSimError: ``PBS_QUEUE`` is not set
     """
     if "PBS_QUEUE" in os.environ:
-        return os.environ.get("PBS_QUEUE")
-    raise SmartSimError("Could not parse queue from SLURM_JOB_PARTITION")
+        return os.environ["PBS_QUEUE"]
+    raise SmartSimError("Could not parse queue from PBS_QUEUE")
 
 
-def get_tasks():
+def get_tasks() -> int:
     """Get the number of processes on each chunk in a PBS allocation.
 
     .. note::
 
         This method requires ``qstat`` be installed on the
         node from which it is run.
 
@@ -83,24 +84,25 @@
         if not which("qstat"):
             raise LauncherError(
                 (
                     "Attempted PBS function without access to "
                     "PBS(qstat) at the call site"
                 )
             )
-        job_id = os.environ.get("PBS_JOBID")
-        job_info_str, _ = qstat(["-f", "-F", "json", job_id])
-        job_info = json.loads(job_info_str)
-        return int(job_info["Jobs"][job_id]["resources_used"]["ncpus"])
+        
+        if job_id := os.environ.get("PBS_JOBID"):
+            job_info_str, _ = qstat(["-f", "-F", "json", job_id])
+            job_info = json.loads(job_info_str)
+            return int(job_info["Jobs"][job_id]["resources_used"]["ncpus"])
     raise SmartSimError(
         "Could not parse number of requested tasks without an allocation"
     )
 
 
-def get_tasks_per_node():
+def get_tasks_per_node() -> t.Dict[str, int]:
     """Get the number of processes on each chunk in a PBS allocation.
 
     .. note::
 
         This method requires ``qstat`` be installed on the
         node from which it is run.
 
@@ -113,20 +115,21 @@
         if not which("qstat"):
             raise LauncherError(
                 (
                     "Attempted PBS function without access to "
                     "PBS(qstat) at the call site"
                 )
             )
-        job_id = os.environ.get("PBS_JOBID")
-        job_info_str, _ = qstat(["-f", "-F", "json", job_id])
-        job_info = json.loads(job_info_str)
-        chunks_and_ncpus = job_info["Jobs"][job_id]["exec_vnode"]  # type: str
-
-        chunk_cpu_map = {}
-        for cunck_and_ncpu in chunks_and_ncpus.split("+"):
-            chunk, ncpu = cunck_and_ncpu.strip("()").split(":")
-            ncpu = ncpu.lstrip("ncpus=")
-            chunk_cpu_map[chunk] = int(ncpu)
 
-        return chunk_cpu_map
+        if job_id := os.environ.get("PBS_JOBID"):
+            job_info_str, _ = qstat(["-f", "-F", "json", job_id])
+            job_info = json.loads(job_info_str)
+            chunks_and_ncpus = job_info["Jobs"][job_id]["exec_vnode"]  # type: str
+
+            chunk_cpu_map = {}
+            for cunck_and_ncpu in chunks_and_ncpus.split("+"):
+                chunk, ncpu = cunck_and_ncpu.strip("()").split(":")
+                ncpu = ncpu.lstrip("ncpus=")
+                chunk_cpu_map[chunk] = int(ncpu)
+
+            return chunk_cpu_map
     raise SmartSimError("Could not parse tasks per node without an allocation")
```

### Comparing `smartsim-0.4.2/smartsim/wlm/slurm.py` & `smartsim-0.5.0/smartsim/wlm/slurm.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,27 +21,31 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
+import typing as t
 from shutil import which
 
 from .._core.launcher.slurm.slurmCommands import salloc, scancel, scontrol, sinfo
 from .._core.launcher.slurm.slurmParser import parse_salloc, parse_salloc_error
 from .._core.launcher.util.launcherUtil import ComputeNode, Partition
 from .._core.utils.helpers import init_default
 from ..error import AllocationError, LauncherError, SmartSimError
 from ..log import get_logger
 
 logger = get_logger(__name__)
 
 
-def get_allocation(nodes=1, time=None, account=None, options=None):
+def get_allocation(nodes: int = 1, 
+                   time: t.Optional[str] = None, 
+                   account: t.Optional[str] = None, 
+                   options: t.Optional[t.Dict[str, str]] = None) -> str:
     """Request an allocation
 
     This function requests an allocation with the specified arguments.
     Anything passed to the options will be processed as a Slurm
     argument and appended to the salloc command with the appropriate
     prefix (e.g. "-" or "--").
 
@@ -88,15 +92,15 @@
         if not error:
             logger.error(err)
             raise AllocationError("Error retrieving Slurm allocation")
         raise AllocationError(error)
     return str(alloc_id)
 
 
-def release_allocation(alloc_id):
+def release_allocation(alloc_id: str) -> None:
     """Free an allocation's resources
 
     :param alloc_id: allocation id
     :type alloc_id: str
     :raises LauncherError: if allocation could not be freed
     """
     if not which("scancel"):
@@ -115,15 +119,15 @@
         raise AllocationError(
             f"Unable to revoke your allocation for jobid  {str(alloc_id)}"
         )
 
     logger.info(f"Successfully freed allocation {alloc_id}")
 
 
-def validate(nodes=1, ppn=1, partition=None):
+def validate(nodes: int = 1, ppn: int = 1, partition: t.Optional[str] = None) -> bool:
     """Check that there are sufficient resources in the provided Slurm partitions.
 
     if no partition is provided, the default partition is found and used.
 
     :param nodes: Override the default node count to validate, defaults to 1
     :type nodes: int, optional
     :param ppn: Override the default processes per node to validate, defaults to 1
@@ -148,15 +152,15 @@
                 "No partition provided and default partition could not be found"
             ) from e
 
     if not p_name in sys_partitions:
         raise LauncherError(f"Partition {p_name} is not found on this system")
 
     for node in sys_partitions[p_name].nodes:
-        if node.ppn >= ppn:
+        if node.ppn is not None and node.ppn >= ppn:
             avail_nodes.add(node)
 
     n_avail_nodes = len(avail_nodes)
     logger.debug(f"Found {n_avail_nodes} nodes that match the constraints provided")
 
     if n_avail_nodes < nodes:
         logger.warning(
@@ -165,15 +169,15 @@
         )
         return False
 
     logger.info("Successfully validated Slurm with sufficient resources")
     return True
 
 
-def get_default_partition():
+def get_default_partition() -> str:
     """Returns the default partition from Slurm
 
     This default partition is assumed to be the partition with
     a star following its partition name in sinfo output
 
     :returns: the name of the default partition
     :rtype: str
@@ -186,23 +190,23 @@
             default = line.strip("*")
 
     if not default:
         raise LauncherError("Could not find default partition!")
     return default
 
 
-def _get_system_partition_info():
+def _get_system_partition_info() -> t.Dict[str, Partition]:
     """Build a dictionary of slurm partitions
     :returns: dict of Partition objects
     :rtype: dict
     """
 
     sinfo_output, _ = sinfo(["--noheader", "--format", "%R %n %c"])
 
-    partitions = {}
+    partitions: t.Dict[str, Partition] = {}
     for line in sinfo_output.split("\n"):
         line = line.strip()
         if line == "":
             continue
 
         p_info = line.split(" ")
         p_name = p_info[0]
@@ -214,15 +218,18 @@
 
         partitions[p_name].name = p_name
         partitions[p_name].nodes.add(ComputeNode(node_name=p_node, node_ppn=p_ppn))
 
     return partitions
 
 
-def _get_alloc_cmd(nodes, time, account, options=None):
+def _get_alloc_cmd(nodes: int, 
+                   time: t.Optional[str] = None, 
+                   account: t.Optional[str] = None, 
+                   options: t.Optional[t.Dict[str, str]] = None) -> t.List[str]:
     """Return the command to request an allocation from Slurm with
     the class variables as the slurm options."""
 
     salloc_args = [
         "--no-shell",
         "-N",
         str(nodes),
@@ -231,30 +238,30 @@
     ]
     # TODO check format here
     if time:
         salloc_args.extend(["-t", time])
     if account:
         salloc_args.extend(["-A", str(account)])
 
-    for opt, val in options.items():
+    for opt, val in (options or {}).items():
         if opt not in ["t", "time", "N", "nodes", "A", "account"]:
             short_arg = bool(len(str(opt)) == 1)
             prefix = "-" if short_arg else "--"
             if not val:
                 salloc_args += [prefix + opt]
             else:
                 if short_arg:
                     salloc_args += [prefix + opt, str(val)]
                 else:
                     salloc_args += ["=".join((prefix + opt, str(val)))]
 
     return salloc_args
 
 
-def get_hosts():
+def get_hosts() -> t.List[str]:
     """Get the name of the nodes used in a slurm allocation.
 
     .. note::
 
         This method requires access to ``scontrol`` from the node
         on which it is run
 
@@ -268,58 +275,58 @@
             raise LauncherError(
                 (
                     "Attempted slurm function without access to "
                     "slurm(scontrol) at the call site"
                 )
             )
         nodelist, _ = scontrol(
-            ["show", "hostnames", os.environ.get("SLURM_JOB_NODELIST")]
+            ["show", "hostnames", os.environ.get("SLURM_JOB_NODELIST", "")]
         )
         return sorted(nodelist.split())
     raise SmartSimError("Could not parse allocation nodes from SLURM_JOB_NODELIST")
 
 
-def get_queue():
+def get_queue() -> str:
     """Get the name of queue in a slurm allocation.
 
     :returns: The name of the queue
     :rtype: str
     :raises SmartSimError: ``SLURM_JOB_PARTITION`` is not set
     """
-    if "SLURM_JOB_PARTITION" in os.environ:
-        return os.environ.get("SLURM_JOB_PARTITION")
+    if job_partition := os.environ.get("SLURM_JOB_PARTITION", None):
+        return job_partition
     raise SmartSimError("Could not parse queue from SLURM_JOB_PARTITION")
 
 
-def get_tasks():
+def get_tasks() -> int:
     """Get the number of tasks in a slurm allocation.
 
     :returns: Then number of tasks in the allocation
     :rtype: int
     :raises SmartSimError: ``SLURM_NTASKS`` is not set
     """
-    if "SLURM_NTASKS" in os.environ:
-        return int(os.environ.get("SLURM_NTASKS"))
+    if ntasks_str := os.environ.get("SLURM_NTASKS", 0):
+        return int(ntasks_str)
     raise SmartSimError("Could not parse number of requested tasks from SLURM_NTASKS")
 
 
-def get_tasks_per_node():
+def get_tasks_per_node() -> t.Dict[str, int]:
     """Get the number of tasks per each node in a slurm allocation.
 
     .. note::
 
         This method requires access to ``scontrol`` from the node
         on which it is run
 
     :returns: Map of nodes to number of tasks on that node
     :rtype: dict[str, int]
     :raises SmartSimError: ``SLURM_TASKS_PER_NODE`` is not set
     """
     if "SLURM_TASKS_PER_NODE" in os.environ:
-        tasks_per_node_strs = os.environ.get("SLURM_TASKS_PER_NODE").split(",")
+        tasks_per_node_strs = os.environ.get("SLURM_TASKS_PER_NODE", "").split(",")
         tasks_per_node_list = []
         for tasks_per_node_str in tasks_per_node_strs:
             if "(" in tasks_per_node_str:
                 tasks, quantity = tasks_per_node_str.split("(")
                 quantity = quantity.rstrip(")").lstrip("x")
                 tasks_per_node_list.extend([int(tasks)] * int(quantity))
             else:
```

### Comparing `smartsim-0.4.2/smartsim.egg-info/PKG-INFO` & `smartsim-0.5.0/smartsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsim
-Version: 0.4.2
+Version: 0.5.0
 Summary: AI Workflows for Science
 Home-page: https://github.com/CrayLabs/SmartSim
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartSim
 Project-URL: Documentation, https://www.craylabs.org
@@ -105,16 +105,16 @@
         
         The documentation has a number of tutorials that make it easy to get used to SmartSim locally
         before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
         # click on link to open jupyter lab
         ```
         
         # SmartSim Infrastructure Library
         
         The Infrastructure Library (IL), the ``smartsim`` python package,
         facilitates the launch of Machine Learning and simulation
@@ -458,15 +458,15 @@
         
         Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
         docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
         ```
         Each of the following examples can be found in the
         [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
         
         ## Online Analysis
         
         Using SmartSim, HPC applications can be monitored in real time by streaming data
@@ -783,8 +783,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: mypy
 Provides-Extra: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.4.2 Summary: AI Workflows for
+Metadata-Version: 2.1 Name: smartsim Version: 0.5.0 Summary: AI Workflows for
 Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
 Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
 License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
 SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
 
@@ -56,16 +56,16 @@
 inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
 (#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
 documentation has a number of tutorials that make it easy to get used to
 SmartSim locally before using it on your system. Each tutorial is a Jupyter
 notebook that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
-ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+ghcr.io/craylabs/smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.1 # click on link to open jupyter lab ``` #
 SmartSim Infrastructure Library The Infrastructure Library (IL), the
 ``smartsim`` python package, facilitates the launch of Machine Learning and
 simulation workflows. The Python interface of the IL creates, configures,
 launches and monitors applications. ## Experiments The [Experiment](https://
 www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
 interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
 api/smartsim_api.html#experiment) users can create references to user
@@ -201,15 +201,15 @@
 smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
 workflows. The following are simple examples of how to use SmartSim and
 SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
 that can be run through the [SmartSim Tutorials docker image](https://
 github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
 lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
 ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
-craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following examples can be
 found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
 getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
 applications can be monitored in real time by streaming data from the
 application to the database. SmartRedis clients can retrieve the data, process,
 analyze it, and finally store any updated data back to the database for use by
 other clients. The following is an example of how a user could monitor and
 analyze a simulation. The example here uses the Python client; however,
@@ -339,8 +339,8 @@
 {Deep learning, Numerical simulation, Climate modeling, High performance
 computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: ml
+markdown Provides-Extra: dev Provides-Extra: mypy Provides-Extra: ml
```

### Comparing `smartsim-0.4.2/smartsim.egg-info/SOURCES.txt` & `smartsim-0.5.0/smartsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 LICENSE.md
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 smartsim/__init__.py
-smartsim/constants.py
 smartsim/experiment.py
 smartsim/log.py
 smartsim/slurm.py
 smartsim/status.py
 smartsim/version.py
 smartsim.egg-info/PKG-INFO
 smartsim.egg-info/SOURCES.txt
@@ -32,15 +30,15 @@
 smartsim/_core/_install/builder.py
 smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc
 smartsim/_core/_install/__pycache__/builder.cpython-38.pyc
 smartsim/_core/bin/modules/FindTensorFlow.cmake
 smartsim/_core/config/__init__.py
 smartsim/_core/config/config.py
 smartsim/_core/config/keydb.conf
-smartsim/_core/config/redis6.conf
+smartsim/_core/config/redis.conf
 smartsim/_core/control/__init__.py
 smartsim/_core/control/controller.py
 smartsim/_core/control/job.py
 smartsim/_core/control/jobmanager.py
 smartsim/_core/control/manifest.py
 smartsim/_core/entrypoints/__init__.py
 smartsim/_core/entrypoints/colocated.py
@@ -115,12 +113,10 @@
 smartsim/settings/lsfSettings.py
 smartsim/settings/mpiSettings.py
 smartsim/settings/mpirunSettings.py
 smartsim/settings/palsSettings.py
 smartsim/settings/pbsSettings.py
 smartsim/settings/settings.py
 smartsim/settings/slurmSettings.py
-smartsim/tf/__init__.py
-smartsim/tf/utils.py
 smartsim/wlm/__init__.py
 smartsim/wlm/pbs.py
 smartsim/wlm/slurm.py
```

