# Comparing `tmp/nix-prefetch-github-6.0.1.tar.gz` & `tmp/nix-prefetch-github-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nix-prefetch-github-6.0.1.tar", last modified: Tue Mar  7 12:24:26 2023, max compression
+gzip compressed data, was "nix-prefetch-github-7.0.0.tar", last modified: Fri Jul  7 15:54:36 2023, max compression
```

## Comparing `nix-prefetch-github-6.0.1.tar` & `nix-prefetch-github-7.0.0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.260914 nix-prefetch-github-6.0.1/
--rw-r--r--   0 me        (1000) users      (100)    35149 2020-09-02 17:18:43.000000 nix-prefetch-github-6.0.1/LICENSE.txt
--rw-r--r--   0 me        (1000) users      (100)       75 2022-04-13 16:12:58.000000 nix-prefetch-github-6.0.1/MANIFEST.in
--rw-r--r--   0 me        (1000) users      (100)    10588 2023-03-07 12:24:26.260914 nix-prefetch-github-6.0.1/PKG-INFO
--rw-r--r--   0 me        (1000) users      (100)    10352 2023-03-07 12:24:09.000000 nix-prefetch-github-6.0.1/README.org
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.254913 nix-prefetch-github-6.0.1/nix_prefetch_github/
--rw-r--r--   0 me        (1000) users      (100)        5 2023-03-07 12:24:09.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/VERSION
--rw-r--r--   0 me        (1000) users      (100)        0 2021-11-29 23:39:30.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/__init__.py
--rw-r--r--   0 me        (1000) users      (100)       93 2022-04-14 17:02:09.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/__main__.py
--rw-r--r--   0 me        (1000) users      (100)      808 2022-06-30 11:03:36.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/alerter.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.255914 nix-prefetch-github-6.0.1/nix_prefetch_github/cli/
--rw-r--r--   0 me        (1000) users      (100)        0 2020-09-12 12:54:50.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/cli/__init__.py
--rw-r--r--   0 me        (1000) users      (100)      290 2022-06-13 18:03:51.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/cli/fetch_directory.py
--rw-r--r--   0 me        (1000) users      (100)      298 2022-06-13 18:09:20.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/cli/fetch_github.py
--rw-r--r--   0 me        (1000) users      (100)      295 2022-06-13 18:03:43.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/cli/fetch_latest_release.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.256914 nix-prefetch-github-6.0.1/nix_prefetch_github/command/
--rw-r--r--   0 me        (1000) users      (100)        0 2022-04-14 12:22:02.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/command/__init__.py
--rw-r--r--   0 me        (1000) users      (100)      417 2022-04-14 12:48:14.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/command/command_availability_checker.py
--rw-r--r--   0 me        (1000) users      (100)     1360 2022-07-16 06:45:42.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/command/command_runner.py
--rw-r--r--   0 me        (1000) users      (100)      802 2023-02-20 11:57:44.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/command/test_command_availability_checker.py
--rw-r--r--   0 me        (1000) users      (100)     2555 2022-07-16 06:45:35.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/command/test_command_runner.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.257914 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/
--rw-r--r--   0 me        (1000) users      (100)        0 2022-04-22 21:36:55.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/__init__.py
--rw-r--r--   0 me        (1000) users      (100)     3839 2022-09-24 08:44:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/arguments.py
--rw-r--r--   0 me        (1000) users      (100)     1774 2022-10-16 10:08:49.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_controller.py
--rw-r--r--   0 me        (1000) users      (100)     1724 2022-10-16 10:09:03.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_directory_controller.py
--rw-r--r--   0 me        (1000) users      (100)     1540 2022-10-16 10:09:11.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_latest_release_controller.py
--rw-r--r--   0 me        (1000) users      (100)     3925 2022-06-13 18:13:44.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_arguments.py
--rw-r--r--   0 me        (1000) users      (100)     6010 2022-10-16 10:08:33.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_controller.py
--rw-r--r--   0 me        (1000) users      (100)     4087 2022-10-16 10:08:00.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_directory_controller.py
--rw-r--r--   0 me        (1000) users      (100)     3139 2022-10-12 13:46:38.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_latest_release_controller.py
--rw-r--r--   0 me        (1000) users      (100)     7102 2023-03-06 23:07:08.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/dependency_injector.py
--rw-r--r--   0 me        (1000) users      (100)      245 2021-12-02 22:47:57.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/functor.py
--rw-r--r--   0 me        (1000) users      (100)      845 2023-01-09 03:49:57.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/github.py
--rw-r--r--   0 me        (1000) users      (100)      805 2023-03-05 12:14:33.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/hash.py
--rw-r--r--   0 me        (1000) users      (100)     3522 2023-03-05 14:46:15.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/interfaces.py
--rw-r--r--   0 me        (1000) users      (100)     3069 2021-11-27 14:37:22.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/list_remote.py
--rw-r--r--   0 me        (1000) users      (100)      797 2022-04-16 09:58:13.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/list_remote_factory.py
--rw-r--r--   0 me        (1000) users      (100)     1142 2022-06-30 11:01:30.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/logging.py
--rw-r--r--   0 me        (1000) users      (100)     2657 2022-04-16 10:00:12.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/prefetch.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.258914 nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/
--rw-r--r--   0 me        (1000) users      (100)     1936 2022-09-18 06:18:50.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/__init__.py
--rw-r--r--   0 me        (1000) users      (100)     2368 2022-11-26 14:28:19.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/repository_renderer.py
--rw-r--r--   0 me        (1000) users      (100)     2628 2022-10-16 09:54:07.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/test_rendering_selector_impl.py
--rw-r--r--   0 me        (1000) users      (100)     2167 2022-09-18 06:18:29.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/test_repository_renderer.py
--rw-r--r--   0 me        (1000) users      (100)       99 2022-06-13 18:02:05.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/process_environment.py
--rw-r--r--   0 me        (1000) users      (100)     1863 2023-03-06 23:07:08.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/repository_detector.py
--rw-r--r--   0 me        (1000) users      (100)      630 2022-04-16 09:57:59.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/revision_index.py
--rw-r--r--   0 me        (1000) users      (100)      773 2022-04-16 10:03:04.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/revision_index_factory.py
--rw-r--r--   0 me        (1000) users      (100)      913 2022-01-01 03:43:05.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/templates.py
--rw-r--r--   0 me        (1000) users      (100)      687 2023-01-09 03:49:57.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_github.py
--rw-r--r--   0 me        (1000) users      (100)     2648 2023-03-05 14:00:34.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_hash.py
--rw-r--r--   0 me        (1000) users      (100)     2418 2022-04-16 09:57:59.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_list_remote.py
--rw-r--r--   0 me        (1000) users      (100)     1420 2022-04-16 10:03:04.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_list_remote_factory.py
--rw-r--r--   0 me        (1000) users      (100)     2469 2022-04-22 21:43:42.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_logging.py
--rw-r--r--   0 me        (1000) users      (100)     3744 2022-10-26 08:00:46.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_prefetch.py
--rw-r--r--   0 me        (1000) users      (100)      610 2022-08-28 09:27:45.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_prefetch_options.py
--rw-r--r--   0 me        (1000) users      (100)     3220 2022-10-21 17:16:17.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_presenter.py
--rw-r--r--   0 me        (1000) users      (100)     4740 2023-03-06 23:07:08.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_repository_detector.py
--rw-r--r--   0 me        (1000) users      (100)     1804 2022-04-16 10:03:04.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_revision_index.py
--rw-r--r--   0 me        (1000) users      (100)     1566 2022-04-16 10:03:04.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/test_revision_index_factory.py
--rw-r--r--   0 me        (1000) users      (100)     2664 2023-03-05 14:46:15.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/tests.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.258914 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/
--rw-r--r--   0 me        (1000) users      (100)        0 2022-04-10 17:04:06.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/__init__.py
--rw-r--r--   0 me        (1000) users      (100)     2957 2023-03-05 14:46:15.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/nix_build.py
--rw-r--r--   0 me        (1000) users      (100)     2702 2023-03-05 14:46:15.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/nix_prefetch.py
--rw-r--r--   0 me        (1000) users      (100)     3202 2022-08-14 09:47:46.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/test_nix_prefetch_url_hasher.py
--rw-r--r--   0 me        (1000) users      (100)     4717 2023-03-05 14:31:49.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/test_url_hasher.py
--rw-r--r--   0 me        (1000) users      (100)     4605 2022-04-16 10:02:40.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/test_url_hasher_selector.py
--rw-r--r--   0 me        (1000) users      (100)     1498 2023-03-05 14:46:15.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/url_hasher_selector.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.259914 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/
--rw-r--r--   0 me        (1000) users      (100)        0 2022-04-14 15:24:18.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/__init__.py
--rw-r--r--   0 me        (1000) users      (100)     1335 2022-10-16 10:09:50.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_directory.py
--rw-r--r--   0 me        (1000) users      (100)     1121 2022-10-16 10:10:07.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_github_repository.py
--rw-r--r--   0 me        (1000) users      (100)      978 2022-10-16 10:09:45.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_latest_release.py
--rw-r--r--   0 me        (1000) users      (100)     4441 2022-10-16 10:09:34.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/test_prefetch_github_repository.py
--rw-r--r--   0 me        (1000) users      (100)      126 2020-08-06 13:21:56.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/version.py
--rw-r--r--   0 me        (1000) users      (100)      362 2022-06-29 13:09:55.000000 nix-prefetch-github-6.0.1/nix_prefetch_github/views.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.255914 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/
--rw-r--r--   0 me        (1000) users      (100)    10588 2023-03-07 12:24:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) users      (100)     3423 2023-03-07 12:24:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) users      (100)        1 2023-03-07 12:24:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) users      (100)      238 2023-03-07 12:24:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) users      (100)       26 2023-03-07 12:24:26.000000 nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/top_level.txt
--rw-r--r--   0 me        (1000) users      (100)       75 2022-01-02 18:03:00.000000 nix-prefetch-github-6.0.1/pyproject.toml
--rw-r--r--   0 me        (1000) users      (100)     1420 2023-03-07 12:24:26.260914 nix-prefetch-github-6.0.1/setup.cfg
--rw-r--r--   0 me        (1000) users      (100)       38 2022-11-13 04:18:17.000000 nix-prefetch-github-6.0.1/setup.py
-drwxr-xr-x   0 me        (1000) users      (100)        0 2023-03-07 12:24:26.259914 nix-prefetch-github-6.0.1/tests/
--rw-r--r--   0 me        (1000) users      (100)        0 2020-06-01 17:43:06.000000 nix-prefetch-github-6.0.1/tests/__init__.py
--rwxr-xr-x   0 me        (1000) users      (100)     6297 2023-03-06 23:07:08.000000 nix-prefetch-github-6.0.1/tests/test_integration.py
--rw-r--r--   0 me        (1000) users      (100)     1731 2022-04-15 14:51:42.000000 nix-prefetch-github-6.0.1/tests/test_issue_21.py
--rw-r--r--   0 me        (1000) users      (100)     1856 2022-04-15 14:51:49.000000 nix-prefetch-github-6.0.1/tests/test_issue_22.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.272716 nix-prefetch-github-7.0.0/
+-rw-r--r--   0 me        (1000) users      (100)    35149 2020-09-02 17:18:43.000000 nix-prefetch-github-7.0.0/LICENSE.txt
+-rw-r--r--   0 me        (1000) users      (100)       75 2022-04-13 16:12:58.000000 nix-prefetch-github-7.0.0/MANIFEST.in
+-rw-r--r--   0 me        (1000) users      (100)    10842 2023-07-07 15:54:36.273716 nix-prefetch-github-7.0.0/PKG-INFO
+-rw-r--r--   0 me        (1000) users      (100)    10590 2023-07-07 15:52:31.000000 nix-prefetch-github-7.0.0/README.org
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.263716 nix-prefetch-github-7.0.0/docs/
+-rw-r--r--   0 me        (1000) users      (100)    10529 2023-07-07 15:52:31.000000 nix-prefetch-github-7.0.0/docs/README.rst
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.267716 nix-prefetch-github-7.0.0/nix_prefetch_github/
+-rw-r--r--   0 me        (1000) users      (100)        5 2023-07-07 15:51:49.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/VERSION
+-rw-r--r--   0 me        (1000) users      (100)        0 2021-11-29 23:39:30.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)       93 2022-04-14 17:02:09.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/__main__.py
+-rw-r--r--   0 me        (1000) users      (100)      808 2022-06-30 11:03:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/alerter.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.268716 nix-prefetch-github-7.0.0/nix_prefetch_github/cli/
+-rw-r--r--   0 me        (1000) users      (100)        0 2020-09-12 12:54:50.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/cli/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)      290 2022-06-13 18:03:51.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/cli/fetch_directory.py
+-rw-r--r--   0 me        (1000) users      (100)      298 2022-06-13 18:09:20.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/cli/fetch_github.py
+-rw-r--r--   0 me        (1000) users      (100)      295 2022-06-13 18:03:43.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/cli/fetch_latest_release.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.269716 nix-prefetch-github-7.0.0/nix_prefetch_github/command/
+-rw-r--r--   0 me        (1000) users      (100)        0 2022-04-14 12:22:02.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/command/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)      417 2022-04-14 12:48:14.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/command/command_availability_checker.py
+-rw-r--r--   0 me        (1000) users      (100)     1360 2022-07-16 06:45:42.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/command/command_runner.py
+-rw-r--r--   0 me        (1000) users      (100)      802 2023-02-20 11:57:44.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/command/test_command_availability_checker.py
+-rw-r--r--   0 me        (1000) users      (100)     2555 2022-07-16 06:45:35.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/command/test_command_runner.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.270716 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/
+-rw-r--r--   0 me        (1000) users      (100)        0 2022-04-22 21:36:55.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)     3839 2022-09-24 08:44:26.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/arguments.py
+-rw-r--r--   0 me        (1000) users      (100)     1774 2022-10-16 10:08:49.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     1724 2022-10-16 10:09:03.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_directory_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     1540 2022-10-16 10:09:11.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_latest_release_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     3925 2022-06-13 18:13:44.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_arguments.py
+-rw-r--r--   0 me        (1000) users      (100)     6010 2022-10-16 10:08:33.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     4087 2022-10-16 10:08:00.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_directory_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     3139 2022-10-12 13:46:38.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_latest_release_controller.py
+-rw-r--r--   0 me        (1000) users      (100)     7432 2023-07-07 10:14:22.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/dependency_injector.py
+-rw-r--r--   0 me        (1000) users      (100)      245 2021-12-02 22:47:57.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/functor.py
+-rw-r--r--   0 me        (1000) users      (100)      845 2023-01-09 03:49:57.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/github.py
+-rw-r--r--   0 me        (1000) users      (100)      805 2023-03-05 12:14:33.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/hash.py
+-rw-r--r--   0 me        (1000) users      (100)      635 2023-07-07 10:14:22.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/hash_converter.py
+-rw-r--r--   0 me        (1000) users      (100)     3638 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/interfaces.py
+-rw-r--r--   0 me        (1000) users      (100)     3069 2021-11-27 14:37:22.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/list_remote.py
+-rw-r--r--   0 me        (1000) users      (100)      797 2022-04-16 09:58:13.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/list_remote_factory.py
+-rw-r--r--   0 me        (1000) users      (100)     1142 2022-06-30 11:01:30.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/logging.py
+-rw-r--r--   0 me        (1000) users      (100)     2655 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/prefetch.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.271716 nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/
+-rw-r--r--   0 me        (1000) users      (100)     1936 2022-09-18 06:18:50.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)     2372 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/repository_renderer.py
+-rw-r--r--   0 me        (1000) users      (100)     2630 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/test_rendering_selector_impl.py
+-rw-r--r--   0 me        (1000) users      (100)     2169 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/test_repository_renderer.py
+-rw-r--r--   0 me        (1000) users      (100)       99 2022-06-13 18:02:05.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/process_environment.py
+-rw-r--r--   0 me        (1000) users      (100)     1863 2023-03-06 23:07:08.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/repository_detector.py
+-rw-r--r--   0 me        (1000) users      (100)      630 2022-04-16 09:57:59.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/revision_index.py
+-rw-r--r--   0 me        (1000) users      (100)      773 2022-04-16 10:03:04.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/revision_index_factory.py
+-rw-r--r--   0 me        (1000) users      (100)      918 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/templates.py
+-rw-r--r--   0 me        (1000) users      (100)      687 2023-01-09 03:49:57.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_github.py
+-rw-r--r--   0 me        (1000) users      (100)     2648 2023-03-05 14:00:34.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_hash.py
+-rw-r--r--   0 me        (1000) users      (100)      919 2023-07-07 10:14:22.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_hash_converter.py
+-rw-r--r--   0 me        (1000) users      (100)     2418 2022-04-16 09:57:59.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_list_remote.py
+-rw-r--r--   0 me        (1000) users      (100)     1420 2022-04-16 10:03:04.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_list_remote_factory.py
+-rw-r--r--   0 me        (1000) users      (100)     2469 2022-04-22 21:43:42.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_logging.py
+-rw-r--r--   0 me        (1000) users      (100)     3742 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_prefetch.py
+-rw-r--r--   0 me        (1000) users      (100)      610 2022-08-28 09:27:45.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_prefetch_options.py
+-rw-r--r--   0 me        (1000) users      (100)     3228 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_presenter.py
+-rw-r--r--   0 me        (1000) users      (100)     4740 2023-03-06 23:07:08.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_repository_detector.py
+-rw-r--r--   0 me        (1000) users      (100)     1804 2022-04-16 10:03:04.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_revision_index.py
+-rw-r--r--   0 me        (1000) users      (100)     1566 2022-04-16 10:03:04.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/test_revision_index_factory.py
+-rw-r--r--   0 me        (1000) users      (100)     2658 2023-07-07 10:32:16.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/tests.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.271716 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/
+-rw-r--r--   0 me        (1000) users      (100)        0 2022-04-10 17:04:06.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)     3136 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/nix_build.py
+-rw-r--r--   0 me        (1000) users      (100)     2493 2023-07-07 10:32:16.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/nix_prefetch.py
+-rw-r--r--   0 me        (1000) users      (100)     3420 2023-07-07 11:15:58.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_nix_prefetch_url_hasher.py
+-rw-r--r--   0 me        (1000) users      (100)     5008 2023-07-07 10:32:16.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_url_hasher.py
+-rw-r--r--   0 me        (1000) users      (100)     4585 2023-07-07 10:32:16.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_url_hasher_selector.py
+-rw-r--r--   0 me        (1000) users      (100)     1494 2023-07-07 10:32:16.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/url_hasher_selector.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.272716 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/
+-rw-r--r--   0 me        (1000) users      (100)        0 2022-04-14 15:24:18.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/__init__.py
+-rw-r--r--   0 me        (1000) users      (100)     1335 2022-10-16 10:09:50.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_directory.py
+-rw-r--r--   0 me        (1000) users      (100)     1121 2022-10-16 10:10:07.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_github_repository.py
+-rw-r--r--   0 me        (1000) users      (100)      978 2022-10-16 10:09:45.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_latest_release.py
+-rw-r--r--   0 me        (1000) users      (100)     4443 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/test_prefetch_github_repository.py
+-rw-r--r--   0 me        (1000) users      (100)      126 2020-08-06 13:21:56.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/version.py
+-rw-r--r--   0 me        (1000) users      (100)      362 2022-06-29 13:09:55.000000 nix-prefetch-github-7.0.0/nix_prefetch_github/views.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.268716 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/
+-rw-r--r--   0 me        (1000) users      (100)    10842 2023-07-07 15:54:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) users      (100)     3520 2023-07-07 15:54:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) users      (100)        1 2023-07-07 15:54:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) users      (100)      238 2023-07-07 15:54:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) users      (100)       26 2023-07-07 15:54:36.000000 nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/top_level.txt
+-rw-r--r--   0 me        (1000) users      (100)       75 2022-01-02 18:03:00.000000 nix-prefetch-github-7.0.0/pyproject.toml
+-rw-r--r--   0 me        (1000) users      (100)     1420 2023-07-07 15:54:36.273716 nix-prefetch-github-7.0.0/setup.cfg
+-rw-r--r--   0 me        (1000) users      (100)       38 2022-11-13 04:18:17.000000 nix-prefetch-github-7.0.0/setup.py
+drwxr-xr-x   0 me        (1000) users      (100)        0 2023-07-07 15:54:36.272716 nix-prefetch-github-7.0.0/tests/
+-rw-r--r--   0 me        (1000) users      (100)        0 2020-06-01 17:43:06.000000 nix-prefetch-github-7.0.0/tests/__init__.py
+-rwxr-xr-x   0 me        (1000) users      (100)     6399 2023-07-07 10:14:22.000000 nix-prefetch-github-7.0.0/tests/test_integration.py
+-rw-r--r--   0 me        (1000) users      (100)     1731 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/tests/test_issue_21.py
+-rw-r--r--   0 me        (1000) users      (100)     1856 2023-07-07 11:03:27.000000 nix-prefetch-github-7.0.0/tests/test_issue_22.py
```

### Comparing `nix-prefetch-github-6.0.1/LICENSE.txt` & `nix-prefetch-github-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/PKG-INFO` & `nix-prefetch-github-7.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-prefetch-github
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prefetch source code from github for nix build tool
 Home-page: https://github.com/seppeljordan/nix-prefetch-github
 Author: Sebastian Jordan
 Author-email: sebastian.jordan.mail@googlemail.com
 Requires-Python: >=3.9
 License-File: LICENSE.txt
 
@@ -25,16 +25,16 @@
    result/bin/nix-prefetch-github seppeljordan nix-prefetch-github
 
 ::
 
    {
        "owner": "seppeljordan",
        "repo": "nix-prefetch-github",
-       "rev": "fdbb5182cac14e2dcecabcedcc1eab4e6b8405f0",
-       "sha256": "97mAbccmJzp3zxaBPCXQQkQrmFhfbKAwewYODMQVrn4="
+       "rev": "ca223cf1a727e18ad5d94ac50c4928f0a163f621",
+       "hash": "sha256-VBMKrIwg4D8/8WD2NoDPWBYb4b8uURyFzjJRpiqOt+A="
    }
 
 Available Commands
 ==================
 
 .. _nix-prefetch-github-1:
 
@@ -185,14 +185,21 @@
 ::
 
    coverage run -m nix_prefetch_github.run_tests && coverage html
 
 changes
 =======
 
+v7.0.0 (unreleased)
+-------------------
+
+-  The output format changed. In previous versions the json and nix
+   output included ``sha256`` as a field. This field was removed in
+   favour of a ``hash`` field. The value of this field is an SRI hash.
+
 v6.0.1
 ------
 
 -  Fix bug in repository detection for ``nix-prefetch-github-directory``
 
 v6.0.0
 ------
```

### Comparing `nix-prefetch-github-6.0.1/README.org` & `nix-prefetch-github-7.0.0/README.org`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
   #+end_src
 
   #+RESULTS:
   #+begin_example
   {
       "owner": "seppeljordan",
       "repo": "nix-prefetch-github",
-      "rev": "fdbb5182cac14e2dcecabcedcc1eab4e6b8405f0",
-      "sha256": "97mAbccmJzp3zxaBPCXQQkQrmFhfbKAwewYODMQVrn4="
+      "rev": "ca223cf1a727e18ad5d94ac50c4928f0a163f621",
+      "hash": "sha256-VBMKrIwg4D8/8WD2NoDPWBYb4b8uURyFzjJRpiqOt+A="
   }
   #+end_example
 
 * Available Commands
 ** nix-prefetch-github
    This command downloads the code from a github repository and puts
    it into the local nix store. It also prints the function arguments
@@ -178,14 +178,19 @@
   #+begin_example
     coverage run -m nix_prefetch_github.run_tests && coverage html
   #+end_example
 
   
 
 * changes
+** v7.0.0 (unreleased)
+   - The output format changed. In previous versions the json and nix
+     output included =sha256= as a field. This field was removed in
+     favour of a =hash= field. The value of this field is an SRI hash.
+
 ** v6.0.1
    - Fix bug in repository detection for
      =nix-prefetch-github-directory=
 
 ** v6.0.0
    - Drop support for python3.8
    - Drop default arguments to fetchFromGitHub from json output
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/alerter.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/alerter.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/command/command_runner.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/command/command_runner.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/command/test_command_availability_checker.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/command/test_command_availability_checker.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/command/test_command_runner.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/command/test_command_runner.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/arguments.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/arguments.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_directory_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_directory_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/nix_prefetch_github_latest_release_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/nix_prefetch_github_latest_release_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_arguments.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_arguments.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_directory_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_directory_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/controller/test_nix_prefetch_github_latest_release_controller.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/controller/test_nix_prefetch_github_latest_release_controller.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/dependency_injector.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/dependency_injector.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from nix_prefetch_github.controller.nix_prefetch_github_directory_controller import (
     PrefetchDirectoryController,
 )
 from nix_prefetch_github.controller.nix_prefetch_github_latest_release_controller import (
     PrefetchLatestReleaseController,
 )
 from nix_prefetch_github.github import GithubAPIImpl
+from nix_prefetch_github.hash_converter import HashConverterImpl
 from nix_prefetch_github.interfaces import (
     GithubAPI,
     RepositoryDetector,
     RevisionIndexFactory,
 )
 from nix_prefetch_github.list_remote_factory import ListRemoteFactoryImpl
 from nix_prefetch_github.logging import LoggerFactoryImpl
@@ -77,22 +78,29 @@
         )
 
     def get_command_availability_checker(self) -> CommandAvailabilityChecker:
         return CommandAvailabilityCheckerImpl(command_runner=self.get_command_runner())
 
     def get_nix_build_url_hasher_impl(self) -> NixBuildUrlHasherImpl:
         return NixBuildUrlHasherImpl(
-            command_runner=self.get_command_runner(), logger=self.get_logger()
+            command_runner=self.get_command_runner(),
+            logger=self.get_logger(),
+            hash_converter=self.get_hash_converter(),
         )
 
     def get_nix_prefetch_url_hasher_impl(self) -> NixPrefetchUrlHasherImpl:
         return NixPrefetchUrlHasherImpl(
-            command_runner=self.get_command_runner(), logger=self.get_logger()
+            command_runner=self.get_command_runner(),
+            logger=self.get_logger(),
+            hash_converter=self.get_hash_converter(),
         )
 
+    def get_hash_converter(self) -> HashConverterImpl:
+        return HashConverterImpl(command_runner=self.get_command_runner())
+
     def get_prefetcher(self) -> PrefetcherImpl:
         return PrefetcherImpl(
             self.get_url_hasher_selector(), self.get_revision_index_factory()
         )
 
     def get_nix_repository_renderer(self) -> NixRepositoryRenderer:
         return NixRepositoryRenderer()
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/github.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/github.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/hash.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/hash.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/interfaces.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,21 @@
     deep_clone: bool = False
     leave_dot_git: bool = False
 
     def is_safe(self) -> bool:
         return not self.deep_clone and not self.leave_dot_git
 
 
+class HashConverter(Protocol):
+    def convert_sha256_to_sri(self, original: str) -> Optional[str]:
+        ...
+
+
 class UrlHasher(Protocol):
-    def calculate_sha256_sum(
+    def calculate_hash_sum(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> Optional[str]:
         ...
 
@@ -71,27 +76,27 @@
         ...
 
 
 @dataclass(frozen=True)
 class PrefetchedRepository:
     repository: GithubRepository
     rev: str
-    sha256: str
+    hash_sum: str
     options: PrefetchOptions
 
 
 @dataclass
 class PrefetchFailure:
     class Reason(enum.Enum):
         unable_to_locate_revision = enum.auto()
-        unable_to_calculate_sha256 = enum.auto()
+        unable_to_calculate_hash_sum = enum.auto()
 
         def __str__(self) -> str:
-            if self == self.unable_to_calculate_sha256:
-                return "Unable to calculate sha256 sum"
+            if self == self.unable_to_calculate_hash_sum:
+                return "Unable to calculate hash sum"
             else:
                 return "Unable to locate revision"
 
     reason: Reason
 
 
 PrefetchResult = Union[PrefetchedRepository, PrefetchFailure]
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/list_remote.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/list_remote.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/list_remote_factory.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/list_remote_factory.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/logging.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/logging.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/prefetch.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/prefetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,24 @@
 
     def _prefetch_github(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> PrefetchResult:
-        calculated_hash = self._calculate_sha256_sum(
+        calculated_hash = self._calculate_hash_sum(
             repository, revision, prefetch_options
         )
         if calculated_hash is None:
             return PrefetchFailure(
-                reason=PrefetchFailure.Reason.unable_to_calculate_sha256
+                reason=PrefetchFailure.Reason.unable_to_calculate_hash_sum
             )
         return PrefetchedRepository(
             repository=repository,
-            sha256=calculated_hash,
+            hash_sum=calculated_hash,
             rev=revision,
             options=prefetch_options,
         )
 
     def _is_proper_revision_hash(self, revision: str) -> bool:
         return is_sha1_hash(revision)
 
@@ -69,18 +69,18 @@
             return None
         if revision is None:
             actual_rev = revision_index.get_revision_by_name("HEAD")
         else:
             actual_rev = revision_index.get_revision_by_name(revision)
         return actual_rev
 
-    def _calculate_sha256_sum(
+    def _calculate_hash_sum(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> Optional[str]:
-        return self.url_hasher.calculate_sha256_sum(
+        return self.url_hasher.calculate_hash_sum(
             repository=repository,
             revision=revision,
             prefetch_options=prefetch_options,
         )
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/__init__.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/__init__.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/repository_renderer.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/repository_renderer.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class NixRepositoryRenderer:
     def render_prefetched_repository(self, repository: PrefetchedRepository) -> str:
         return output_template(
             owner=repository.repository.owner,
             repo=repository.repository.name,
             rev=repository.rev,
-            sha256=repository.sha256,
+            hash_sum=repository.hash_sum,
             fetch_submodules=repository.options.fetch_submodules,
             leave_dot_git=repository.options.leave_dot_git,
             deep_clone=repository.options.deep_clone,
         )
 
 
 class JsonRepositoryRenderer:
@@ -31,15 +31,15 @@
     }
 
     def render_prefetched_repository(self, repository: PrefetchedRepository) -> str:
         output: Dict[str, Any] = {
             "owner": repository.repository.owner,
             "repo": repository.repository.name,
             "rev": repository.rev,
-            "sha256": repository.sha256,
+            "hash": repository.hash_sum,
         }
         if repository.options.deep_clone != self.DEFAULTS["deepClone"]:
             output["deepClone"] = repository.options.deep_clone
         if repository.options.fetch_submodules != self.DEFAULTS["fetchSubmodules"]:
             output["fetchSubmodules"] = repository.options.fetch_submodules
         if repository.options.leave_dot_git != self.DEFAULTS["leaveDotGit"]:
             output["leaveDotGit"] = repository.options.leave_dot_git
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/test_rendering_selector_impl.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/test_rendering_selector_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             self.get_repository()
         )
         self.assertEqual(output, "nix format 2")
 
     def get_repository(self) -> PrefetchedRepository:
         return PrefetchedRepository(
             repository=GithubRepository(owner="test", name="test"),
-            sha256="",
+            hash_sum="",
             options=PrefetchOptions(),
             rev="",
         )
 
 
 class RepositoryRendererImpl:
     def __init__(self, output: str) -> None:
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/presenter/test_repository_renderer.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/presenter/test_repository_renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 
     def _make_repository(
         self, leave_dot_git: bool = False, deep_clone: bool = False
     ) -> PrefetchedRepository:
         return PrefetchedRepository(
             repository=GithubRepository(owner="test", name="test"),
             rev="test",
-            sha256="test",
+            hash_sum="test",
             options=PrefetchOptions(leave_dot_git=leave_dot_git, deep_clone=deep_clone),
         )
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/repository_detector.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/repository_detector.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/revision_index.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/revision_index.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/revision_index_factory.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/revision_index_factory.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/templates.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 _OUTPUT_TEMPLATE = """let
   pkgs = import <nixpkgs> {{}};
 in
   pkgs.fetchFromGitHub {{
     owner = "{owner}";
     repo = "{repo}";
     rev = "{rev}";
-    sha256 = "{sha256}";{fetch_submodules}{leave_dot_git}{deep_clone}
+    hash = "{hash_sum}";{fetch_submodules}{leave_dot_git}{deep_clone}
   }}
 """
 
 
 def _render_line_if_enabled(line: str, condition: bool) -> str:
     return f"\n    {line};" if condition else ""
 
 
 def output_template(
     owner: str,
     repo: str,
     rev: str,
-    sha256: str,
+    hash_sum: str,
     fetch_submodules: bool,
     leave_dot_git: bool,
     deep_clone: bool,
 ) -> str:
-
     return _OUTPUT_TEMPLATE.format(
         owner=owner,
         repo=repo,
         rev=rev,
-        sha256=sha256,
+        hash_sum=hash_sum,
         fetch_submodules=_render_line_if_enabled(
             "fetchSubmodules = true", fetch_submodules
         ),
         leave_dot_git=_render_line_if_enabled("leaveDotGit = true", leave_dot_git),
         deep_clone=_render_line_if_enabled("deepClone = true", deep_clone),
     )
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_github.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_github.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_hash.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_hash.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_list_remote.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_list_remote.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_list_remote_factory.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_list_remote_factory.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_logging.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_logging.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_prefetch.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_prefetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 from nix_prefetch_github.tests import FakeRevisionIndexFactory, FakeUrlHasher
 
 
 class PrefetcherTests(TestCase):
     def test_when_url_hasher_and_revision_index_fail_then_prefetching_also_fails(
         self,
     ) -> None:
-        self.url_hasher.sha256_sum = None
+        self.url_hasher.hash_sum = None
         self.revision_index_factory.revision_index = None
         result = self.prefetch_repository()
         self.assertFailure(result)
 
     def test_return_hash_that_was_returned_by_url_hasher(self) -> None:
         result = self.prefetch_repository()
         self.assertIsInstance(result, PrefetchedRepository)
 
     def test_return_expected_hash_from_url_hasher(self) -> None:
         result = self.prefetch_repository()
-        self.assertSuccess(result, lambda r: r.sha256 == self.expected_hash)
+        self.assertSuccess(result, lambda r: r.hash_sum == self.expected_hash)
 
     def test_return_expected_revision_from_revision_index(self) -> None:
         result = self.prefetch_repository()
         self.assertSuccess(result, lambda r: r.rev == self.expected_revision)
 
     def test_cannot_prefetch_revision_that_does_not_exist(self) -> None:
         result = self.prefetch_repository(revision="does not exist")
         self.assertFailure(
             result,
             lambda f: f.reason == PrefetchFailure.Reason.unable_to_locate_revision,
         )
 
     def test_fail_with_correct_reason_when_hash_could_not_be_calculated(self) -> None:
-        self.url_hasher.sha256_sum = None
+        self.url_hasher.hash_sum = None
         self.assertFailure(
             self.prefetch_repository(),
-            lambda f: f.reason == PrefetchFailure.Reason.unable_to_calculate_sha256,
+            lambda f: f.reason == PrefetchFailure.Reason.unable_to_calculate_hash_sum,
         )
 
     def test_can_prefetch_revision_by_its_sha1_id(self) -> None:
         expected_revision = "4840fbf9ebd246d334c11335fc85747013230b05"
         self.assertSuccess(
             self.prefetch_repository(revision=expected_revision),
             lambda result: result.rev == expected_revision,
@@ -72,15 +72,15 @@
         self.assertTrue(prop(cast(PrefetchFailure, result)))
 
     def setUp(self) -> None:
         self.url_hasher = FakeUrlHasher()
         self.revision_index_factory = FakeRevisionIndexFactory()
         self.expected_hash = "test hash"
         self.expected_revision = "test ref"
-        self.url_hasher.sha256_sum = self.expected_hash
+        self.url_hasher.hash_sum = self.expected_hash
         self.revision_index_factory.revision_index = RevisionIndexImpl(
             ListRemote(
                 symrefs={"HEAD": "refs/heads/master"},
                 heads={"master": self.expected_revision},
             )
         )
         self.prefetcher = PrefetcherImpl(
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_prefetch_options.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_prefetch_options.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_presenter.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_presenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,33 @@
         self.presenter = PresenterImpl(
             view=self.view,
             repository_renderer=self.renderer,
         )
         self.repo = PrefetchedRepository(
             GithubRepository(owner="test", name="test"),
             rev="test",
-            sha256="test",
+            hash_sum="test",
             options=PrefetchOptions(),
         )
 
     def test_write_to_error_output_when_presenting_prefetch_failure(self) -> None:
         self.presenter.present(
-            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_sha256)
+            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_hash_sum)
         )
         self.assertTrue(self.read_error_output())
 
     def test_write_to_result_output_when_presenting_prefetched_repository(self) -> None:
         self.presenter.present(self.repo)
         self.assertTrue(self.read_result_output())
 
     def test_nothing_is_written_to_result_output_when_presenting_prefetch_failure(
         self,
     ) -> None:
         self.presenter.present(
-            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_sha256)
+            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_hash_sum)
         )
         self.assertFalse(self.read_result_output())
 
     def test_nothing_is_written_to_error_output_when_presenting_prefetched_respository(
         self,
     ) -> None:
         self.presenter.present(self.repo)
@@ -59,15 +59,15 @@
 
     def test_that_exit_0_is_returned_when_repository_is_rendered(self) -> None:
         self.presenter.present(self.repo)
         self.assertExitCode(0)
 
     def test_that_exit_1_is_returned_when_failure_is_rendered(self) -> None:
         self.presenter.present(
-            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_sha256)
+            PrefetchFailure(reason=PrefetchFailure.Reason.unable_to_calculate_hash_sum)
         )
         self.assertExitCode(1)
 
     def assertExitCode(self, code: int) -> None:
         self.assertEqual(
             self.view.exit_code,
             code,
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_repository_detector.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_repository_detector.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_revision_index.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_revision_index.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/test_revision_index_factory.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/test_revision_index_factory.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/tests.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 class BaseTestCase(TestCase):
     pass
 
 
 class FakeUrlHasher:
     def __init__(self) -> None:
-        self.sha256_sum: Optional[str] = None
+        self.hash_sum: Optional[str] = None
 
-    def calculate_sha256_sum(
+    def calculate_hash_sum(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> Optional[str]:
-        return self.sha256_sum
+        return self.hash_sum
 
 
 class FakeRevisionIndexFactory:
     def __init__(self) -> None:
         self.revision_index: Optional[RevisionIndexImpl] = None
 
     def get_revision_index(
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/nix_build.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/nix_build.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,52 +3,57 @@
 from logging import Logger
 from tempfile import TemporaryDirectory
 from typing import List, Optional, Tuple
 
 from nix_prefetch_github.interfaces import (
     CommandRunner,
     GithubRepository,
+    HashConverter,
     PrefetchOptions,
 )
 from nix_prefetch_github.templates import output_template
 
-trash_sha256 = ""
+trash_hash_sum = ""
 
 
 @dataclass(frozen=True)
 class NixBuildUrlHasherImpl:
     command_runner: CommandRunner
     logger: Logger
+    hash_converter: HashConverter
 
-    def calculate_sha256_sum(
+    def calculate_hash_sum(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> Optional[str]:
         status_code, output = self.run_fetch_command(
             repository,
             revision,
-            trash_sha256,
+            trash_hash_sum,
             prefetch_options,
         )
-        return detect_actual_hash_from_nix_output(output.splitlines())
+        sha256 = detect_actual_hash_from_nix_output(output.splitlines())
+        if sha256 is None:
+            return None
+        return self.hash_converter.convert_sha256_to_sri(sha256)
 
     def run_fetch_command(
         self,
         repository: GithubRepository,
         rev: str,
-        sha256: str,
+        hash_sum: str,
         prefetch_options: PrefetchOptions,
     ) -> Tuple[int, str]:
         nix_code_calculate_hash = output_template(
             owner=repository.owner,
             repo=repository.name,
             rev=rev,
-            sha256=sha256,
+            hash_sum=hash_sum,
             fetch_submodules=prefetch_options.fetch_submodules,
             leave_dot_git=prefetch_options.leave_dot_git,
             deep_clone=prefetch_options.deep_clone,
         )
         self.logger.info("Evaluating nix expression \n%s", nix_code_calculate_hash)
         with TemporaryDirectory() as temp_dir_name:
             nix_filename = temp_dir_name + "/prefetch-github.nix"
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/nix_prefetch.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_nix_prefetch_url_hasher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-import json
-from dataclasses import dataclass
-from logging import Logger
-from typing import List, Optional
-
-from nix_prefetch_github.interfaces import (
-    CommandRunner,
-    GithubRepository,
-    PrefetchOptions,
-)
-
-
-@dataclass(frozen=True)
-class NixPrefetchUrlHasherImpl:
-    command_runner: CommandRunner
-    logger: Logger
-
-    def calculate_sha256_sum(
-        self,
-        repository: GithubRepository,
-        revision: str,
-        prefetch_options: PrefetchOptions,
-    ) -> Optional[str]:
-        if self.is_default_prefetch_options(prefetch_options):
-            return self.fetch_url(repository=repository, revision=revision)
-        else:
-            return self.fetch_git(
-                repository=repository,
-                revision=revision,
-                prefetch_options=prefetch_options,
-            )
-
-    def fetch_url(self, repository: GithubRepository, revision: str) -> Optional[str]:
-        repo_url = f"https://github.com/{repository.owner}/{repository.name}/archive/{revision}.tar.gz"
-        _, output = self.command_runner.run_command(
-            ["nix-prefetch-url", "--unpack", repo_url],
-        )
-        return self.calculate_sri_representation(output.strip())
-
-    def fetch_git(
-        self,
-        repository: GithubRepository,
-        revision: str,
-        prefetch_options: PrefetchOptions,
-    ) -> Optional[str]:
-        repo_url = f"https://github.com/{repository.owner}/{repository.name}.git"
-        command = (
-            ["nix-prefetch-git"]
-            + self.prefetch_git_options(prefetch_options)
-            + [repo_url, revision]
-        )
-        _, output = self.command_runner.run_command(command)
-        return self.calculate_sri_representation(json.loads(output)["sha256"])
-
-    def calculate_sri_representation(self, sha256: str) -> str:
-        _, output = self.command_runner.run_command(
-            [
-                "nix",
-                "--extra-experimental-features",
-                "nix-command",
-                "hash",
-                "to-sri",
-                f"sha256:{sha256}",
-            ],
-        )
-        return output.strip().removeprefix("sha256-")
-
-    def is_default_prefetch_options(self, options: PrefetchOptions) -> bool:
-        return options == PrefetchOptions()
-
-    def prefetch_git_options(self, prefetch_options: PrefetchOptions) -> List[str]:
-        options: List[str] = []
-        if prefetch_options.deep_clone:
-            options.append("--deepClone")
-        if prefetch_options.leave_dot_git or prefetch_options.deep_clone:
-            options.append("--leave-dotGit")
-        if prefetch_options.fetch_submodules:
-            options.append("--fetch-submodules")
-        return options
+from logging import getLogger
+from unittest import TestCase
+
+from nix_prefetch_github.command.command_runner import CommandRunnerImpl
+from nix_prefetch_github.hash_converter import HashConverterImpl
+from nix_prefetch_github.interfaces import GithubRepository, PrefetchOptions
+from nix_prefetch_github.tests import CommandRunnerTestImpl, network, requires_nix_build
+from nix_prefetch_github.url_hasher.nix_prefetch import NixPrefetchUrlHasherImpl
+
+
+@requires_nix_build
+@network
+class UrlHasherTests(TestCase):
+    def setUp(self) -> None:
+        self.command_runner = CommandRunnerTestImpl(
+            command_runner=CommandRunnerImpl(getLogger(__name__))
+        )
+        hash_converter = HashConverterImpl(command_runner=self.command_runner)
+        self.hasher = NixPrefetchUrlHasherImpl(
+            command_runner=self.command_runner,
+            logger=getLogger(),
+            hash_converter=hash_converter,
+        )
+        self.repository = GithubRepository(
+            owner="git-up",
+            name="test-repo-submodules",
+        )
+        self.revision = "5a1dfa807759c39e3df891b6b46dfb2cf776c6ef"
+
+    def test_without_fetching_submodules(self) -> None:
+        prefetch_options = PrefetchOptions(fetch_submodules=False)
+        hash_sum = self.hasher.calculate_hash_sum(
+            repository=self.repository,
+            revision=self.revision,
+            prefetch_options=prefetch_options,
+        )
+        self.assertEqual(
+            hash_sum, "sha256-B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM="
+        )
+
+    def test_that_experimental_feature_nix_command_is_enabled(self) -> None:
+        self.hasher.calculate_hash_sum(
+            repository=self.repository,
+            revision=self.revision,
+            prefetch_options=PrefetchOptions(),
+        )
+        issued_nix_commands = list(
+            filter(lambda c: c[0] == "nix", self.command_runner.commands_issued)
+        )
+        self.assertTrue(
+            all(
+                command[1] == "--extra-experimental-features"
+                and command[2] == "nix-command"
+                for command in issued_nix_commands
+            ),
+            msg="Not all commands in  %s do include '--extra-experimental-features nix-command'"
+            % issued_nix_commands,
+        )
+
+    def test_with_fetching_submodules(self) -> None:
+        prefetch_options = PrefetchOptions(fetch_submodules=True)
+        hash_sum = self.hasher.calculate_hash_sum(
+            repository=self.repository,
+            revision=self.revision,
+            prefetch_options=prefetch_options,
+        )
+        self.assertEqual(
+            hash_sum, "sha256-wCo1YobyatxSOE85xQNSJw6jvufghFNHlZl4ToQjRHA="
+        )
+
+    def test_with_leaving_dotgit_dir(self) -> None:
+        prefetch_options = PrefetchOptions(leave_dot_git=True)
+        hash_sum = self.hasher.calculate_hash_sum(
+            repository=self.repository,
+            revision=self.revision,
+            prefetch_options=prefetch_options,
+        )
+        self.assertNotEqual(
+            hash_sum, "sha256-B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM="
+        )
+
+    def test_with_deep_clone(self) -> None:
+        prefetch_options = PrefetchOptions(deep_clone=True)
+        hash_sum = self.hasher.calculate_hash_sum(
+            repository=self.repository,
+            revision=self.revision,
+            prefetch_options=prefetch_options,
+        )
+        assert hash_sum
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/test_url_hasher.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_url_hasher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 from logging import getLogger
 from unittest import TestCase
 
 from nix_prefetch_github.command.command_runner import CommandRunnerImpl
+from nix_prefetch_github.hash_converter import HashConverterImpl
 from nix_prefetch_github.interfaces import GithubRepository
 from nix_prefetch_github.tests import network, requires_nix_build
 from nix_prefetch_github.url_hasher.nix_build import (
     NixBuildUrlHasherImpl,
     PrefetchOptions,
     detect_actual_hash_from_nix_output,
 )
 
 
 @requires_nix_build
 @network
 class UrlHasherTests(TestCase):
     def setUp(self) -> None:
+        logger = getLogger(__name__)
+        command_runner = CommandRunnerImpl(logger)
+        hash_converter = HashConverterImpl(command_runner=command_runner)
         self.hasher = NixBuildUrlHasherImpl(
-            command_runner=CommandRunnerImpl(getLogger(__name__)), logger=getLogger()
+            command_runner=command_runner, logger=logger, hash_converter=hash_converter
         )
         self.repository = GithubRepository(
             owner="git-up",
             name="test-repo-submodules",
         )
         self.revision = "5a1dfa807759c39e3df891b6b46dfb2cf776c6ef"
 
     def test_without_fetching_submodules(self) -> None:
         prefetch_options = PrefetchOptions(fetch_submodules=False)
-        hash_sum = self.hasher.calculate_sha256_sum(
+        hash_sum = self.hasher.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=prefetch_options,
         )
-        self.assertEqual(hash_sum, "B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM=")
+        self.assertEqual(
+            hash_sum, "sha256-B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM="
+        )
 
     def test_with_fetching_submodules(self) -> None:
         prefetch_options = PrefetchOptions(fetch_submodules=True)
-        hash_sum = self.hasher.calculate_sha256_sum(
+        hash_sum = self.hasher.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=prefetch_options,
         )
-        self.assertEqual(hash_sum, "wCo1YobyatxSOE85xQNSJw6jvufghFNHlZl4ToQjRHA=")
+        self.assertEqual(
+            hash_sum, "sha256-wCo1YobyatxSOE85xQNSJw6jvufghFNHlZl4ToQjRHA="
+        )
 
     def test_with_leaving_dotgit_dir(self) -> None:
         prefetch_options = PrefetchOptions(leave_dot_git=True)
-        hash_sum = self.hasher.calculate_sha256_sum(
+        hash_sum = self.hasher.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=prefetch_options,
         )
-        self.assertNotEqual(hash_sum, "B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM=")
+        self.assertNotEqual(
+            hash_sum, "sha256-B5AlNwg6kbcaqUiQEC6jslCRKVpErXLMsKC+b9aPlrM="
+        )
 
-    def test_with_deep_clone(self) -> None:
+    def test_that_with_deep_clone_option_we_at_least_get_some_hash_sum(self) -> None:
         prefetch_options = PrefetchOptions(deep_clone=True)
-        hash_sum = self.hasher.calculate_sha256_sum(
+        hash_sum = self.hasher.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=prefetch_options,
         )
-        self.assertEqual(hash_sum, "gBAtCILDbqofa6+9/bXR9drxymCGrgwf0+5mDxwF9p0=")
+        assert hash_sum
 
 
 class DetectActualHashFromNixOutputTests(TestCase):
     def setUp(self) -> None:
         self.data = (
             (
                 [
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/test_url_hasher_selector.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/test_url_hasher_selector.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,31 +14,31 @@
         self.selector = UrlHasherSelector(
             availability_checker=self.availability_checker,
             nix_build_implementation=self.nix_build_hasher,
             nix_prefetch_implementation=self.nix_prefetch_hasher,
         )
         self.availability_checker.set_as_available("nix-prefetch-url")
         self.availability_checker.set_as_available("nix-prefetch-git")
-        self.nix_build_hasher.sha256_sum = "nix build hash"
-        self.nix_prefetch_hasher.sha256_sum = "nix prefetch hash"
+        self.nix_build_hasher.hash_sum = "nix build hash"
+        self.nix_prefetch_hasher.hash_sum = "nix prefetch hash"
         self.repository = GithubRepository(owner="test", name="test")
         self.revision = "test"
 
     def test_that_prefetch_hasher_is_used(self) -> None:
-        hash_sum = self.selector.calculate_sha256_sum(
+        hash_sum = self.selector.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=PrefetchOptions(),
         )
         self.assertEqual(hash_sum, "nix prefetch hash")
 
     def test_that_nix_build_hasher_is_used_with_deep_clone_and_not_leave_dot_git(
         self,
     ) -> None:
-        hash_sum = self.selector.calculate_sha256_sum(
+        hash_sum = self.selector.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=PrefetchOptions(deep_clone=True, leave_dot_git=False),
         )
         self.assertEqual(hash_sum, "nix build hash")
 
 
@@ -50,21 +50,21 @@
         self.selector = UrlHasherSelector(
             availability_checker=self.availability_checker,
             nix_build_implementation=self.nix_build_hasher,
             nix_prefetch_implementation=self.nix_prefetch_hasher,
         )
         self.availability_checker.set_as_unavailable("nix-prefetch-url")
         self.availability_checker.set_as_unavailable("nix-prefetch-git")
-        self.nix_build_hasher.sha256_sum = "nix build hash"
-        self.nix_prefetch_hasher.sha256_sum = "nix prefetch hash"
+        self.nix_build_hasher.hash_sum = "nix build hash"
+        self.nix_prefetch_hasher.hash_sum = "nix prefetch hash"
         self.repository = GithubRepository(owner="test", name="test")
         self.revision = "test"
 
     def test_that_nix_build_hasher_is_used(self) -> None:
-        hash_sum = self.selector.calculate_sha256_sum(
+        hash_sum = self.selector.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=PrefetchOptions(),
         )
         self.assertEqual(hash_sum, "nix build hash")
 
 
@@ -76,21 +76,21 @@
         self.selector = UrlHasherSelector(
             availability_checker=self.availability_checker,
             nix_build_implementation=self.nix_build_hasher,
             nix_prefetch_implementation=self.nix_prefetch_hasher,
         )
         self.availability_checker.set_as_unavailable("nix-prefetch-url")
         self.availability_checker.set_as_available("nix-prefetch-git")
-        self.nix_build_hasher.sha256_sum = "nix build hash"
-        self.nix_prefetch_hasher.sha256_sum = "nix prefetch hash"
+        self.nix_build_hasher.hash_sum = "nix build hash"
+        self.nix_prefetch_hasher.hash_sum = "nix prefetch hash"
         self.repository = GithubRepository(owner="test", name="test")
         self.revision = "test"
 
     def test_that_nix_build_hasher_is_used(self) -> None:
-        hash_sum = self.selector.calculate_sha256_sum(
+        hash_sum = self.selector.calculate_hash_sum(
             repository=self.repository,
             revision=self.revision,
             prefetch_options=PrefetchOptions(),
         )
         self.assertEqual(hash_sum, "nix build hash")
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/url_hasher/url_hasher_selector.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/url_hasher/url_hasher_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,19 @@
         if self.availability_checker.is_command_available(
             "nix-prefetch-url"
         ) and self.availability_checker.is_command_available("nix-prefetch-git"):
             return self.nix_prefetch_implementation
         else:
             return self.nix_build_implementation
 
-    def calculate_sha256_sum(
+    def calculate_hash_sum(
         self,
         repository: GithubRepository,
         revision: str,
         prefetch_options: PrefetchOptions,
     ) -> Optional[str]:
         hasher = self._get_url_hasher(prefetch_options)
-        return hasher.calculate_sha256_sum(
+        return hasher.calculate_hash_sum(
             repository=repository,
             revision=revision,
             prefetch_options=prefetch_options,
         )
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_directory.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_directory.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_github_repository.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_github_repository.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/prefetch_latest_release.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/prefetch_latest_release.py`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github/use_cases/test_prefetch_github_repository.py` & `nix-prefetch-github-7.0.0/nix_prefetch_github/use_cases/test_prefetch_github_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         repository: GithubRepository,
         rev: Optional[str],
         prefetch_options: PrefetchOptions,
     ) -> PrefetchResult:
         return PrefetchedRepository(
             repository=repository,
             rev="",
-            sha256="",
+            hash_sum="",
             options=prefetch_options,
         )
 
 
 class FakePresenter:
     def __init__(self) -> None:
         self.results: List[PrefetchResult] = []
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/PKG-INFO` & `nix-prefetch-github-7.0.0/docs/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nix-prefetch-github
-Version: 6.0.1
-Summary: Prefetch source code from github for nix build tool
-Home-page: https://github.com/seppeljordan/nix-prefetch-github
-Author: Sebastian Jordan
-Author-email: sebastian.jordan.mail@googlemail.com
-Requires-Python: >=3.9
-License-File: LICENSE.txt
-
 Introduction
 ============
 
 This module implements a python function and a command line tool to help
 you fetch sources from github when using ``fetchFromGitHub``.
 
 This program can be distributed under the conditions of the GNU Public
@@ -25,16 +15,16 @@
    result/bin/nix-prefetch-github seppeljordan nix-prefetch-github
 
 ::
 
    {
        "owner": "seppeljordan",
        "repo": "nix-prefetch-github",
-       "rev": "fdbb5182cac14e2dcecabcedcc1eab4e6b8405f0",
-       "sha256": "97mAbccmJzp3zxaBPCXQQkQrmFhfbKAwewYODMQVrn4="
+       "rev": "ca223cf1a727e18ad5d94ac50c4928f0a163f621",
+       "hash": "sha256-VBMKrIwg4D8/8WD2NoDPWBYb4b8uURyFzjJRpiqOt+A="
    }
 
 Available Commands
 ==================
 
 .. _nix-prefetch-github-1:
 
@@ -185,14 +175,21 @@
 ::
 
    coverage run -m nix_prefetch_github.run_tests && coverage html
 
 changes
 =======
 
+v7.0.0 (unreleased)
+-------------------
+
+-  The output format changed. In previous versions the json and nix
+   output included ``sha256`` as a field. This field was removed in
+   favour of a ``hash`` field. The value of this field is an SRI hash.
+
 v6.0.1
 ------
 
 -  Fix bug in repository detection for ``nix-prefetch-github-directory``
 
 v6.0.0
 ------
```

### Comparing `nix-prefetch-github-6.0.1/nix_prefetch_github.egg-info/SOURCES.txt` & `nix-prefetch-github-7.0.0/nix_prefetch_github.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 LICENSE.txt
 MANIFEST.in
 README.org
 pyproject.toml
 setup.cfg
 setup.py
+docs/README.rst
 nix_prefetch_github/VERSION
 nix_prefetch_github/__init__.py
 nix_prefetch_github/__main__.py
 nix_prefetch_github/alerter.py
 nix_prefetch_github/dependency_injector.py
 nix_prefetch_github/functor.py
 nix_prefetch_github/github.py
 nix_prefetch_github/hash.py
+nix_prefetch_github/hash_converter.py
 nix_prefetch_github/interfaces.py
 nix_prefetch_github/list_remote.py
 nix_prefetch_github/list_remote_factory.py
 nix_prefetch_github/logging.py
 nix_prefetch_github/prefetch.py
 nix_prefetch_github/process_environment.py
 nix_prefetch_github/repository_detector.py
 nix_prefetch_github/revision_index.py
 nix_prefetch_github/revision_index_factory.py
 nix_prefetch_github/templates.py
 nix_prefetch_github/test_github.py
 nix_prefetch_github/test_hash.py
+nix_prefetch_github/test_hash_converter.py
 nix_prefetch_github/test_list_remote.py
 nix_prefetch_github/test_list_remote_factory.py
 nix_prefetch_github/test_logging.py
 nix_prefetch_github/test_prefetch.py
 nix_prefetch_github/test_prefetch_options.py
 nix_prefetch_github/test_presenter.py
 nix_prefetch_github/test_repository_detector.py
```

### Comparing `nix-prefetch-github-6.0.1/setup.cfg` & `nix-prefetch-github-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nix-prefetch-github-6.0.1/tests/test_integration.py` & `nix-prefetch-github-7.0.0/tests/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
 @network
 @requires_nix_build
 class VersionFlagTests(TestCase):
     def setUp(self) -> None:
         self.directory = tempfile.mkdtemp()
         self.output = path.join(self.directory, "result")
-        subprocess.run(["nix", "build", "--out-link", self.output], capture_output=True)
+        subprocess.run(
+            ["nix", "build", "--out-link", self.output], capture_output=True, check=True
+        )
 
     def test_can_specify_version_flag(self) -> None:
         commands = [
             "nix-prefetch-github",
             "nix-prefetch-github-directory",
             "nix-prefetch-github-latest-release",
         ]
@@ -80,15 +82,17 @@
 
 @network
 @requires_nix_build
 class NixEvaluationTests(TestCase):
     def setUp(self) -> None:
         self.directory = tempfile.mkdtemp()
         self.output = path.join(self.directory, "result")
-        subprocess.run(["nix", "build", "--out-link", self.output], capture_output=True)
+        subprocess.run(
+            ["nix", "build", "--out-link", self.output], capture_output=True, check=True
+        )
 
     def test_can_build_nix_expressions(self) -> None:
         expressions = [
             [
                 f"{self.output}/bin/nix-prefetch-github",
                 "seppeljordan",
                 "nix-prefetch-github",
@@ -119,15 +123,17 @@
 
 @network
 @requires_nix_build
 class JsonIntegrityTests(TestCase):
     def setUp(self) -> None:
         self.directory = tempfile.mkdtemp()
         self.output = path.join(self.directory, "result")
-        subprocess.run(["nix", "build", "--out-link", self.output], capture_output=True)
+        subprocess.run(
+            ["nix", "build", "--out-link", self.output], capture_output=True, check=True
+        )
 
     def tearDown(self) -> None:
         shutil.rmtree(self.directory)
 
     def test_can_load_json_output_as_json(self) -> None:
         expressions = [
             [
```

### Comparing `nix-prefetch-github-6.0.1/tests/test_issue_21.py` & `nix-prefetch-github-7.0.0/tests/test_issue_21.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,19 @@
             owner="sensu",
             name="sensu-go",
         )
         self.revision_index_factory = FakeRevisionIndexFactory()
         self.prefetcher = PrefetcherImpl(self.url_hasher, self.revision_index_factory)
 
     def test_prefetch_sensu_go_5_11(self) -> None:
-        self.url_hasher.sha256_sum = "TEST_HASH_SUM"
+        self.url_hasher.hash_sum = "TEST_HASH_SUM"
         self.revision_index_factory.revision_index = RevisionIndexImpl(
             self.sensu_go_ls_remote_output
         )
         result = self.prefetcher.prefetch_github(
             repository=self.repository,
             rev="5.11.0",
             prefetch_options=PrefetchOptions(),
         )
         assert isinstance(result, PrefetchedRepository)
         assert result.rev == "dd8f160a9033ecb5ad0384baf6a9965fa7bd3c17"
-        assert result.sha256 == "TEST_HASH_SUM"
+        assert result.hash_sum == "TEST_HASH_SUM"
```

### Comparing `nix-prefetch-github-6.0.1/tests/test_issue_22.py` & `nix-prefetch-github-7.0.0/tests/test_issue_22.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         )
         self.prefetcher = PrefetcherImpl(
             self.url_hasher,
             self.revision_index_factory,
         )
 
     def test_issue_22(self) -> None:
-        self.url_hasher.sha256_sum = "TEST_HASH_SUM"
+        self.url_hasher.hash_sum = "TEST_HASH_SUM"
         result = self.prefetcher.prefetch_github(
             repository=self.repository,
             rev="jrg/mvp",
             prefetch_options=PrefetchOptions(),
         )
         assert isinstance(result, PrefetchedRepository)
         assert result.rev == "ad1a1d1d25870cc70cd7e708a73c874322064d96"
-        assert result.sha256 == "TEST_HASH_SUM"
+        assert result.hash_sum == "TEST_HASH_SUM"
```

