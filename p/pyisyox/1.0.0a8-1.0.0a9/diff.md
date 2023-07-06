# Comparing `tmp/pyisyox-1.0.0a8.tar.gz` & `tmp/pyisyox-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyisyox-1.0.0a8.tar", last modified: Fri Jun 23 01:26:13 2023, max compression
+gzip compressed data, was "pyisyox-1.0.0a9.tar", last modified: Tue Jun 27 19:48:04 2023, max compression
```

## Comparing `pyisyox-1.0.0a8.tar` & `pyisyox-1.0.0a9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/postCreate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/workflows/pythonpublish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/api/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/test_cases/node_battery_only.xml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/test_cases/parsed_node_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/clock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30753 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/events/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/eventreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/tcpsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/entity_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/isy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/node_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/nodes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11942 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/folder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21160 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/node_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7857 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/nodebase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/programs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/program.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/backports.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.118466 pyisyox-1.0.0a9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.110466 pyisyox-1.0.0a9/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.devcontainer/postCreate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.110466 pyisyox-1.0.0a9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.110466 pyisyox-1.0.0a9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.github/workflows/pythonpublish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.110466 pyisyox-1.0.0a9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-27 19:48:04.118466 pyisyox-1.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.110466 pyisyox-1.0.0a9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/api/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/docs/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/test_cases/node_battery_only.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/docs/test_cases/parsed_node_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/clock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31400 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/eventreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/tcpsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/events/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/entity_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/helpers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/isy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/node_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox/nodes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11942 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/folder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21160 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/node_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7857 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/nodes/nodebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox/programs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/programs/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/programs/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.118466 pyisyox-1.0.0a9/pyisyox/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/util/backports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/util/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.118466 pyisyox-1.0.0a9/pyisyox/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyisyox/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:48:04.114466 pyisyox-1.0.0a9/pyisyox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-27 19:48:03.000000 pyisyox-1.0.0a9/pyisyox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-27 19:48:04.000000 pyisyox-1.0.0a9/pyisyox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:48:03.000000 pyisyox-1.0.0a9/pyisyox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 19:48:03.000000 pyisyox-1.0.0a9/pyisyox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 19:48:03.000000 pyisyox-1.0.0a9/pyisyox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 19:47:52.000000 pyisyox-1.0.0a9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 19:48:04.118466 pyisyox-1.0.0a9/setup.cfg
```

### Comparing `pyisyox-1.0.0a8/.devcontainer/Dockerfile` & `pyisyox-1.0.0a9/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/.devcontainer/devcontainer.json` & `pyisyox-1.0.0a9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/.github/workflows/pythonpublish.yml` & `pyisyox-1.0.0a9/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/.gitignore` & `pyisyox-1.0.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/.pre-commit-config.yaml` & `pyisyox-1.0.0a9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.274
+    rev: v0.0.275
     hooks:
       - id: ruff
         args:
           - --fix
   - hooks:
       - args: [--safe, --quiet]
         files: ^((pyisyox|examples)/.+)?[^/]+\.py$
```

### Comparing `pyisyox-1.0.0a8/.vscode/settings.json` & `pyisyox-1.0.0a9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/.yamllint` & `pyisyox-1.0.0a9/.yamllint`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/CHANGELOG.md` & `pyisyox-1.0.0a9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/LICENSE.txt` & `pyisyox-1.0.0a9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/PKG-INFO` & `pyisyox-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
 Keywords: home,automation,isy,isy994,isy-994,UDI,polisy,eisy,home-assistant
```

### Comparing `pyisyox-1.0.0a8/README.md` & `pyisyox-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/Makefile` & `pyisyox-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/conf.py` & `pyisyox-1.0.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/events.rst` & `pyisyox-1.0.0a9/docs/events.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/index.rst` & `pyisyox-1.0.0a9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/library.rst` & `pyisyox-1.0.0a9/docs/library.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/make.bat` & `pyisyox-1.0.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/quickstart.rst` & `pyisyox-1.0.0a9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/test_cases/node_battery_only.xml` & `pyisyox-1.0.0a9/docs/test_cases/node_battery_only.xml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/docs/test_cases/parsed_node_info.json` & `pyisyox-1.0.0a9/docs/test_cases/parsed_node_info.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/mypy.ini` & `pyisyox-1.0.0a9/mypy.ini`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/__init__.py` & `pyisyox-1.0.0a9/pyisyox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/__main__.py` & `pyisyox-1.0.0a9/pyisyox/__main__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/clock.py` & `pyisyox-1.0.0a9/pyisyox/clock.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/configuration.py` & `pyisyox-1.0.0a9/pyisyox/configuration.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/connection.py` & `pyisyox-1.0.0a9/pyisyox/connection.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/constants.py` & `pyisyox-1.0.0a9/pyisyox/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,14 +533,37 @@
     "113": "",  # raw 3-byte signed value
     "114": "",  # raw 4-byte signed value
     "116": "mi",
     "117": "mbar",
     "118": "hPa",
     "119": "Wh",
     "120": "in/day",
+    "122": "μg/m³",  # Microgram per cubic meter
+    "123": "bq/m³",  # Becquerel per cubic meter
+    "124": "pCi/L",  # Picocuries per liter
+    "125": "pH",
+    "126": "bpm",  # Beats per Minute
+    "127": "mmHg",
+    "128": "J",
+    "129": "BMI",  # Body Mass Index
+    "130": "L/h",
+    "131": "dBm",
+    "132": "bpm",  # Breaths per minute
+    "133": "kHz",
+    "134": "m/²",
+    "135": "VA",  # Volt-Amp
+    "136": "var",  # VAR = Volt-Amp Reactive
+    "137": "",  # NTP DateTime - Number of seconds since 1900
+    "138": "psi",
+    "139": "°",
+    "140": "mg/L",
+    "141": "N",
+    "142": "gal/s",
+    "143": "gpm",
+    "144": "gph",
 }
 
 UOM_TO_STATES: dict[str, dict[str, str]] = {
     "11": {  # Deadbolt Status
         "0": "unlocked",
         "100": "locked",
         "101": "unknown",
```

### Comparing `pyisyox-1.0.0a8/pyisyox/events/eventreader.py` & `pyisyox-1.0.0a9/pyisyox/events/eventreader.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/events/router.py` & `pyisyox-1.0.0a9/pyisyox/events/router.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/events/strings.py` & `pyisyox-1.0.0a9/pyisyox/events/strings.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/events/tcpsocket.py` & `pyisyox-1.0.0a9/pyisyox/events/tcpsocket.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/events/websocket.py` & `pyisyox-1.0.0a9/pyisyox/events/websocket.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/exceptions.py` & `pyisyox-1.0.0a9/pyisyox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/__init__.py` & `pyisyox-1.0.0a9/pyisyox/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/entity.py` & `pyisyox-1.0.0a9/pyisyox/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/entity_platform.py` & `pyisyox-1.0.0a9/pyisyox/helpers/entity_platform.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/events.py` & `pyisyox-1.0.0a9/pyisyox/helpers/events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/models.py` & `pyisyox-1.0.0a9/pyisyox/helpers/models.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/session.py` & `pyisyox-1.0.0a9/pyisyox/helpers/session.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/timeit.py` & `pyisyox-1.0.0a9/pyisyox/helpers/timeit.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/helpers/xml.py` & `pyisyox-1.0.0a9/pyisyox/helpers/xml.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/isy.py` & `pyisyox-1.0.0a9/pyisyox/isy.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/logging.py` & `pyisyox-1.0.0a9/pyisyox/logging.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/networking.py` & `pyisyox-1.0.0a9/pyisyox/networking.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/node_servers.py` & `pyisyox-1.0.0a9/pyisyox/node_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,16 @@
             ]
             if nls_list:
                 try:
                     nls_lookup = dict(re.split(r"\s+=\s+", line) for line in nls_list)
                     self._node_server_nls[slot] = nls_lookup
                 except ValueError:
                     _LOGGER.error(
-                        "Error parsing language file for node server slot %s, invalid format"
+                        "Error parsing language file for node server slot %s, invalid format",
+                        slot,
                     )
 
             if self.isy.args and self.isy.args.file:
                 filename = "-".join(path.split("/")[-2:]).replace(".txt", ".yaml")
                 await self.isy.loop.run_in_executor(
                     None,
                     write_to_file,
```

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/__init__.py` & `pyisyox-1.0.0a9/pyisyox/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/folder.py` & `pyisyox-1.0.0a9/pyisyox/nodes/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/group.py` & `pyisyox-1.0.0a9/pyisyox/nodes/group.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/node.py` & `pyisyox-1.0.0a9/pyisyox/nodes/node.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/node_events.py` & `pyisyox-1.0.0a9/pyisyox/nodes/node_events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/nodes/nodebase.py` & `pyisyox-1.0.0a9/pyisyox/nodes/nodebase.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/programs/__init__.py` & `pyisyox-1.0.0a9/pyisyox/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/programs/folder.py` & `pyisyox-1.0.0a9/pyisyox/programs/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/programs/program.py` & `pyisyox-1.0.0a9/pyisyox/programs/program.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/util/backports.py` & `pyisyox-1.0.0a9/pyisyox/util/backports.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/util/output.py` & `pyisyox-1.0.0a9/pyisyox/util/output.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/variables/__init__.py` & `pyisyox-1.0.0a9/pyisyox/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox/variables/variable.py` & `pyisyox-1.0.0a9/pyisyox/variables/variable.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyisyox.egg-info/PKG-INFO` & `pyisyox-1.0.0a9/pyisyox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
 Keywords: home,automation,isy,isy994,isy-994,UDI,polisy,eisy,home-assistant
```

### Comparing `pyisyox-1.0.0a8/pyisyox.egg-info/SOURCES.txt` & `pyisyox-1.0.0a9/pyisyox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a8/pyproject.toml` & `pyisyox-1.0.0a9/pyproject.toml`

 * *Files identical despite different names*

