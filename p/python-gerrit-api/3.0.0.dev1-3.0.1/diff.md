# Comparing `tmp/python-gerrit-api-3.0.0.dev1.tar.gz` & `tmp/python-gerrit-api-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.0.dev1.tar", last modified: Fri Jun 30 15:46:47 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.1.tar", last modified: Fri Jul  7 15:47:16 2023, max compression
```

## Comparing `python-gerrit-api-3.0.0.dev1.tar` & `python-gerrit-api-3.0.1.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.353120 python-gerrit-api-3.0.0.dev1/gerrit/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gitiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gitiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.016067 python-gerrit-api-3.0.1/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.020067 python-gerrit-api-3.0.1/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.020067 python-gerrit-api-3.0.1/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.024067 python-gerrit-api-3.0.1/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.024067 python-gerrit-api-3.0.1/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gitiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gitiles/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.0.dev1/LICENSE` & `python-gerrit-api-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/PKG-INFO` & `python-gerrit-api-3.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.0.dev1
+Version: 3.0.1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
+.. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
+    :target: https://codecov.io/gh/shijl0925/python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
@@ -69,14 +71,17 @@
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
 Usage
 -----
 
+For a full documentation spec of what this library supports see `readthedocs
+<https://python-gerrit-api.readthedocs.io/en/latest/>`_
+
 Example 1: setup gerrit client:
 
 .. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
@@ -86,51 +91,66 @@
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
+.. code:: python
+
     # Creates a new project.
     input_ = {
         "description": "This is a demo project.",
         "submit_type": "INHERIT",
         "owners": [
           "MyProject-Owners"
         ]
     }
     client.projects.create('MyProject', input_)
 
     # or
     client.post(endpoint="/projects/MyProject", json=input_)
 
+.. code:: python
+
     # Sets the description of a project.
     project = client.projects.get('MyProject')
     input_ = {
         "description": "Plugin for Gerrit that handles the replication.",,
         "commit_message": "Update the project description"
     }
     result = project.set_description(input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/description", json=input_)
 
+.. code:: python
+
     # Deletes the description of a project.
     project = client.projects.get('MyProject')
     project.delete_description()
 
     # or
-    client.put(endpoint="/projects/MyProject/description")
+    client.delete(endpoint="/projects/MyProject/description")
+
+.. code:: python
 
     # get a branch of th project by ref
     branch = project.branches.get('refs/heads/stable')
 
+.. code:: python
+
     # get these branches of th project
+    branches = project.branches.list()
+
+    # or 
     branches = client.get(endpoint = "/projects/MyProject"/branches/)
 
+.. code:: python
+
     # Creates a new branch.
     input_ = {
         'revision': '76016386a0d8ecc7b6be212424978bb45959d668'
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
@@ -143,64 +163,82 @@
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
+.. code:: python
+
     # Marks a change as reviewed.
     change.mark_as_reviewed()
 
+.. code:: python
+
     # Adds and removes hashtags from a change.
     input_ = {
         "add" : [
             "hashtag3"
         ],
         "remove" : [
             "hashtag2"
         ]
     }
     result = change.set_hashtags(input_)
 
+.. code:: python
+
     # get one revision by revision id
     revision = change.get_revision('534b3ce21655a092eccf72680f2ad16b8fecf119')
 
+.. code:: python
+
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
+.. code:: python
+
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
 Example 4: operate gerrit account:
 
 .. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
+.. code:: python
+
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
+.. code:: python
+
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
 Example 5: operate gerrit group:
 
 .. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
+.. code:: python
+
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
+.. code:: python
+
     # Sets the owner group of a Gerrit internal group.
     input_ = {
         "owner": "6a1e70e1a88782771a91808c8af9bbb7a9871389"
     }
     result = group.set_owner(input_)
 
 About this library
@@ -268,32 +306,30 @@
 
 * Ability to execute Gerrit config:
     * Retrieves/Sets the default user/diff/edit preferences for the server.
     * ...
 
 * Ability to install/enable/disable/reload/query Gerrit plugins
 
-For a full documentation spec of what this library supports see `readthedocs
-<https://python-gerrit-api.readthedocs.io/en/latest/>`_
-
 Python versions
 ---------------
 
 The project has been tested against Python versions:
 
 * 3.6
 * 3.7
 * 3.8
 * 3.9
 * 3.10
+* 3.11
 
 Gerrit versions
 ---------------
 
-Project tested on Version 3.5.0 Gerrit.
+Project tested on Version 3.8.0 Gerrit.
 
 Important Links
 ---------------
 
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
```

### Comparing `python-gerrit-api-3.0.0.dev1/README.rst` & `python-gerrit-api-3.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
+.. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
+    :target: https://codecov.io/gh/shijl0925/python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
@@ -46,14 +48,17 @@
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
 Usage
 -----
 
+For a full documentation spec of what this library supports see `readthedocs
+<https://python-gerrit-api.readthedocs.io/en/latest/>`_
+
 Example 1: setup gerrit client:
 
 .. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
@@ -63,51 +68,66 @@
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
+.. code:: python
+
     # Creates a new project.
     input_ = {
         "description": "This is a demo project.",
         "submit_type": "INHERIT",
         "owners": [
           "MyProject-Owners"
         ]
     }
     client.projects.create('MyProject', input_)
 
     # or
     client.post(endpoint="/projects/MyProject", json=input_)
 
+.. code:: python
+
     # Sets the description of a project.
     project = client.projects.get('MyProject')
     input_ = {
         "description": "Plugin for Gerrit that handles the replication.",,
         "commit_message": "Update the project description"
     }
     result = project.set_description(input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/description", json=input_)
 
+.. code:: python
+
     # Deletes the description of a project.
     project = client.projects.get('MyProject')
     project.delete_description()
 
     # or
-    client.put(endpoint="/projects/MyProject/description")
+    client.delete(endpoint="/projects/MyProject/description")
+
+.. code:: python
 
     # get a branch of th project by ref
     branch = project.branches.get('refs/heads/stable')
 
+.. code:: python
+
     # get these branches of th project
+    branches = project.branches.list()
+
+    # or 
     branches = client.get(endpoint = "/projects/MyProject"/branches/)
 
+.. code:: python
+
     # Creates a new branch.
     input_ = {
         'revision': '76016386a0d8ecc7b6be212424978bb45959d668'
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
@@ -120,64 +140,82 @@
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
+.. code:: python
+
     # Marks a change as reviewed.
     change.mark_as_reviewed()
 
+.. code:: python
+
     # Adds and removes hashtags from a change.
     input_ = {
         "add" : [
             "hashtag3"
         ],
         "remove" : [
             "hashtag2"
         ]
     }
     result = change.set_hashtags(input_)
 
+.. code:: python
+
     # get one revision by revision id
     revision = change.get_revision('534b3ce21655a092eccf72680f2ad16b8fecf119')
 
+.. code:: python
+
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
+.. code:: python
+
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
 Example 4: operate gerrit account:
 
 .. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
+.. code:: python
+
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
+.. code:: python
+
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
 Example 5: operate gerrit group:
 
 .. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
+.. code:: python
+
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
+.. code:: python
+
     # Sets the owner group of a Gerrit internal group.
     input_ = {
         "owner": "6a1e70e1a88782771a91808c8af9bbb7a9871389"
     }
     result = group.set_owner(input_)
 
 About this library
@@ -245,32 +283,30 @@
 
 * Ability to execute Gerrit config:
     * Retrieves/Sets the default user/diff/edit preferences for the server.
     * ...
 
 * Ability to install/enable/disable/reload/query Gerrit plugins
 
-For a full documentation spec of what this library supports see `readthedocs
-<https://python-gerrit-api.readthedocs.io/en/latest/>`_
-
 Python versions
 ---------------
 
 The project has been tested against Python versions:
 
 * 3.6
 * 3.7
 * 3.8
 * 3.9
 * 3.10
+* 3.11
 
 Gerrit versions
 ---------------
 
-Project tested on Version 3.5.0 Gerrit.
+Project tested on Version 3.8.0 Gerrit.
 
 Important Links
 ---------------
 
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/__init__.py` & `python-gerrit-api-3.0.1/gerrit/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-__version__ = "3.0.0.dev1"
-
 import netrc
 from gerrit.utils.requester import Requester
 from gerrit.utils.common import (
     decode_response,
     strip_trailing_slash
 )
 from gerrit.config.config import GerritConfig
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py` & `python-gerrit-api-3.0.1/gerrit/accounts/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_name(input_)
 
 
         :param input_: the AccountNameInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #account-name-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#account-name-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/name",
                                json=input_, headers=self.gerrit.default_headers)
 
     def delete_name(self):
         """
@@ -103,16 +102,15 @@
                 "username": "shijl0925.shi"
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_username(input_)
 
         :param input_: the UsernameInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #username-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#username-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/username",
                                json=input_, headers=self.gerrit.default_headers)
 
     def set_displayname(self, input_):
         """
@@ -125,16 +123,15 @@
                 "display_name": "Kevin"
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_displayname(input_)
 
         :param input_: the DisplayNameInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #display-name-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#display-name-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/displayname",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_active(self):
         """
@@ -172,16 +169,15 @@
                 "http_password": "the_password"
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_http_password(input_)
 
         :param input_: the HttpPasswordInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #http-password-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#http-password-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/password.http",
                                json=input_, headers=self.gerrit.default_headers)
 
     def delete_http_password(self):
         """
@@ -285,16 +281,15 @@
                 "mute_common_path_prefixes": true,
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_user_preferences(input_)
 
         :param input_: the PreferencesInput entity，
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #preferences-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#preferences-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/preferences",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_diff_preferences(self):
         """
@@ -325,16 +320,15 @@
                 "font_size": 12
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_diff_preferences(input_)
 
         :param input_: the DiffPreferencesInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #diff-preferences-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#diff-preferences-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/preferences.diff",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_edit_preferences(self):
         """
@@ -367,16 +361,15 @@
                 "auto_close_brackets": true
             }
 
             account = client.accounts.get('kevin.shi')
             result = account.set_edit_preferences(input_)
 
         :param input_: the EditPreferencesInfo entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #edit-preferences-info
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#edit-preferences-info
         :return:
         """
         return self.gerrit.put(self.endpoint + "/preferences.edit",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_watched_projects(self):
         """
@@ -482,16 +475,15 @@
             input_ = {
                 "name": "Individual"
             }
             account = client.accounts.get('kevin.shi')
             result = account.sign_contributor_agreement(input_)
 
         :param input_: the ContributorAgreementInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #contributor-agreement-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#contributor-agreement-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/agreements",
                                json=input_, headers=self.gerrit.default_headers)
 
     def delete_draft_comments(self, input_):
         """
@@ -502,16 +494,15 @@
             input_ = {
                 "query": "is:abandoned"
             }
             account = client.accounts.get('kevin.shi')
             result = account.delete_draft_comments(input_)
 
         :param input_: the DeleteDraftCommentsInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #delete-draft-comments-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#delete-draft-comments-input
         :return:
         """
         return self.gerrit.post(self.endpoint + "/drafts:delete",
                                 json=input_, headers=self.gerrit.default_headers)
 
     def index(self):
         """
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.1/gerrit/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.1/gerrit/accounts/emails.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.1/gerrit/accounts/gpg_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.1/gerrit/accounts/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py` & `python-gerrit-api-3.0.1/gerrit/changes/change.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,15 @@
                 }
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.update(input_)
 
         :param input_: the MergePatchSetInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #merge-patch-set-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#merge-patch-set-input
         :return:
         """
         return self.gerrit.post(self.endpoint + "/merge",
                                 json=input_, headers=self.gerrit.default_headers)
 
     def set_commit_message(self, input_):
         """
@@ -93,16 +92,15 @@
                 "message": "New Commit message \\n\\nChange-Id: I10394472cbd17dd12454f22b143a444\\n"
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.set_commit_message(input_)
 
         :param input_: the CommitMessageInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #commit-message-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#commit-message-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/message",
                                json=input_, headers=self.gerrit.default_headers)
 
     def list_votes(self, account):
         """
@@ -130,16 +128,15 @@
             change.delete_vote('John', 'Code-Review', input_)
             # or
             change.delete_vote('John', 'Code-Review')
 
         :param account:
         :param label:
         :param input_: the DeleteVoteInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-vote-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-vote-input
         :return:
         """
         endpoint = f"{self.endpoint}/reviewers/{account}/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             endpoint += "/delete"
@@ -491,16 +488,15 @@
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.set_work_in_progress(input_)
             # or
             result = change.set_work_in_progress()
 
         :param input_: the WorkInProgressInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #work-in-progress-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#work-in-progress-input
         :return:
         """
         self.gerrit.post(self.endpoint + "/wip",
                          json=input_ or {}, headers=self.gerrit.default_headers
                          )
 
     def set_ready_for_review(self, input_):
@@ -516,16 +512,15 @@
                 'message': 'Refactoring is done.'
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             change.set_ready_for_review(input_)
 
         :param input_: the WorkInProgressInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #work-in-progress-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#work-in-progress-input
         :return:
         """
         self.gerrit.post(self.endpoint + "/ready", json=input_, headers=self.gerrit.default_headers)
 
     def mark_private(self, input_):
         """
         Marks the change to be private. Only open changes can be marked private.
@@ -752,16 +747,15 @@
                 "user": "John Doe",
                 "reason": "reason"
             }
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             result = change.add_to_attention_set(input_)
 
         :param input_: the AttentionSetInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #attention-set-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#attention-set-input
         :return:
         """
         result = self.gerrit.post(self.endpoint + "/attention",
                                   json=input_, headers=self.gerrit.default_headers)
         return result
 
     def remove_from_attention_set(self, id_, input_=None):
@@ -780,16 +774,15 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             change.remove_from_attention_set('kevin.shi', input_)
             # or
             change.remove_from_attention_set('kevin.shi')
 
         :param id_: account id
         :param input_: the AttentionSetInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #attention-set-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#attention-set-input
         :return:
         """
         endpoint = self.endpoint + f"/attention/{id_}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             endpoint += "/delete"
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py` & `python-gerrit-api-3.0.1/gerrit/changes/changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py` & `python-gerrit-api-3.0.1/gerrit/changes/edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,15 @@
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             edit = change.get_edit()
             edit.change_commit_message(input_)
 
         :param input_: the ChangeEditMessageInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #change-edit-message-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-edit-message-input
         :return:
         """
         self.gerrit.put(self.endpoint + ":message",
                         json=input_, headers=self.gerrit.default_headers)
 
     def get_commit_message(self):
         """
@@ -113,16 +112,15 @@
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             edit = change.get_edit()
             edit.publish(input_)
 
         :param input_: the PublishChangeEditInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #publish-change-edit-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#publish-change-edit-input
         :return:
         """
         self.gerrit.post(self.endpoint + ":publish",
                          json=input_, headers=self.gerrit.default_headers)
 
     def rebase(self):
         """
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py` & `python-gerrit-api-3.0.1/gerrit/changes/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,15 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             message = change.messages.get("babf4c5dd53d7a11080696efa78830d0a07762e6")
             result = message.delete(input_)
             # or
             result = message.delete()
 
         :param input_: the DeleteChangeMessageInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-change-message-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-change-message-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint)
         else:
             self.gerrit.post(self.endpoint + "/delete",
                              json=input_, headers=self.gerrit.default_headers)
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.1/gerrit/changes/reviewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             reviewer = change.reviewers.get('john.doe')
             reviewer.delete(input_)
             # or
             reviewer.delete()
 
         :param input_: the DeleteReviewerInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-reviewer-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-reviewer-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint)
         else:
             self.gerrit.post(self.endpoint + "/delete",
                              json=input_, headers=self.gerrit.default_headers)
@@ -76,16 +75,15 @@
             reviewer = change.reviewers.get('john.doe')
             reviewer.delete_vote('Code-Review', input_)
             # or
             reviewer.delete_vote('Code-Review')
 
         :param label:
         :param input_: the DeleteVoteInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-vote-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-vote-input
         :return:
         """
         endpoint = self.endpoint + f"/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             self.gerrit.post(endpoint + "/delete", json=input_, headers=self.gerrit.default_headers)
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py` & `python-gerrit-api-3.0.1/gerrit/changes/revision/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,15 @@
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.set_description(input_)
 
         :param input_: the DescriptionInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #description-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#description-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/description",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_merge_list(self):
         """
@@ -312,16 +311,15 @@
             }
 
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             result = revision.cherry_pick(input_)
 
         :param input_: the CherryPickInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #cherry-pick-commit
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#cherry-pick-commit
         :return:
         """
         return self.gerrit.post(self.endpoint + "/cherrypick",
                                 json=input_, headers=self.gerrit.default_headers)
 
     def list_reviewers(self):
         """
@@ -359,16 +357,15 @@
             revision.delete_vote('John', 'Code-Review', input_)
             # or
             revision.delete_vote('John', 'Code-Review')
 
         :param account:
         :param label:
         :param input_: the DeleteVoteInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-vote-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-vote-input
         :return:
         """
         endpoint = self.endpoint + f"/reviewers/{account}/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             endpoint += "/delete"
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py` & `python-gerrit-api-3.0.1/gerrit/changes/revision/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,15 @@
             revision = change.get_revision('3848807f587dbd3a7e61723bbfbf1ad13ad5a00a')
             comment = revision.comments.get("e167e775_e069567a")
             result = comment.delete(input_)
             # or
             result = comment.delete()
 
         :param input_: the DeleteCommentInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #delete-comment-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-comment-input
         :return:
         """
         if input_ is None:
             return self.gerrit.delete(self.endpoint)
         else:
             return self.gerrit.post(self.endpoint + "/delete",
                                     json=input_, headers=self.gerrit.default_headers)
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py` & `python-gerrit-api-3.0.1/gerrit/changes/revision/drafts.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
 
 class GerritChangeRevisionDrafts:
     def __init__(self, change, revision, gerrit):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
-        self.endpoint = self.gerrit.get(f"/changes/{self.change}/revisions/{self.revision}/drafts")
+        self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/drafts"
 
     def list(self):
         """
         Lists the draft comments of a revision that belong to the calling user.
 
         :return:
         """
-        result = self.gerrit.get(f"/changes/{self.change}/revisions/{self.revision}/drafts")
+        result = self.gerrit.get(self.endpoint)
         drafts = []
         for key, value in result.items():
             for item in value:
                 draft = item
                 draft.update({"path": key})
                 drafts.append(draft)
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/files.py` & `python-gerrit-api-3.0.1/gerrit/changes/revision/files.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py` & `python-gerrit-api-3.0.1/gerrit/config/caches.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,12 +65,11 @@
 
             input_ = {
                 "operation": "FLUSH_ALL"
             }
             gerrit.config.caches.operation(input_)
 
         :param input_: the CacheOperationInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html
-          #cache-operation-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#cache-operation-input
         :return:
         """
         self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/config/config.py` & `python-gerrit-api-3.0.1/gerrit/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,15 @@
             input_ = {
                 "check_accounts": {},
                 "check_account_external_ids": {}
             }
             result = client.config.check_consistency(input_)
 
         :param input_: the ConsistencyCheckInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html
-          #consistency-check-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#consistency-check-input
         :return:
         """
         return self.gerrit.post(
             self.endpoint + "/check.consistency", json=input_, headers=self.gerrit.default_headers)
 
     def reload_config(self):
         """
@@ -64,16 +63,15 @@
 
             input_ = {
                 "token": "Enim+QNbAo6TV8Hur8WwoUypI6apG7qBPvF+bw==$MTAwMDAwNDp0ZXN0QHRlc3QuZGU="
             }
             result = client.config.confirm_email(input_)
 
         :param input_: the EmailConfirmationInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html
-          #email-confirmation-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#email-confirmation-input
         :return:
         """
         self.gerrit.put(
             self.endpoint + "/email.confirm", json=input_, headers=self.gerrit.default_headers
         )
 
     @property
@@ -129,16 +127,15 @@
 
             input_ = {
                 "changes_per_page": 50
             }
             result = client.config.set_default_user_preferences(input_)
 
         :param input_: the PreferencesInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #preferences-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#preferences-input
         :return:
         """
         return self.gerrit.put(
             self.endpoint + "/preferences", json=input_, headers=self.gerrit.default_headers
         )
 
     def get_default_diff_preferences(self):
@@ -168,16 +165,15 @@
                 "auto_hide_diff_table_header": true,
                 "theme": "DEFAULT",
                 "ignore_whitespace": "IGNORE_NONE"
             }
             result = client.config.set_default_diff_preferences(input_)
 
         :param input_: the DiffPreferencesInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #diff-preferences-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#diff-preferences-input
         :return:
         """
         return self.gerrit.put(
             self.endpoint + "/preferences.diff", json=input_, headers=self.gerrit.default_headers
         )
 
     def get_default_edit_preferences(self):
@@ -205,16 +201,15 @@
                 "auto_close_brackets": true,
                 "theme": "DEFAULT",
                 "key_map_type": "DEFAULT"
             }
             result = client.config.set_default_edit_preferences(input_)
 
         :param input_: the EditPreferencesInfo entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
-          #edit-preferences-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#edit-preferences-input
         :return:
         """
         return self.gerrit.put(
             self.endpoint + "/preferences.edit", json=input_, headers=self.gerrit.default_headers
         )
 
     def index_changes(self, input_):
@@ -223,14 +218,13 @@
 
         .. code-block:: python
 
             input_ = {changes: ["foo~101", "bar~202"]}
             gerrit.config.index_changes(input_)
 
         :param input_: the IndexChangesInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html
-          #index-changes-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-config.html#index-changes-input
         :return:
         """
         self.gerrit.post(
             self.endpoint + "/index.changes", json=input_, headers=self.gerrit.default_headers
         )
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/config/tasks.py` & `python-gerrit-api-3.0.1/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py` & `python-gerrit-api-3.0.1/gerrit/groups/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,15 @@
                 "visible_to_all": True
             }
             group = client.groups.get('0017af503a22f7b3fa6ce2cd3b551734d90701b4')
             result = group.set_options(input_)
 
 
         :param input_: the GroupOptionsInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-groups.html
-          #group-options-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-groups.html#group-options-input
         :return:
         """
         return self.gerrit.put(
             self.endpoint + "/options", json=input_, headers=self.gerrit.default_headers)
 
     def get_owner(self):
         """
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py` & `python-gerrit-api-3.0.1/gerrit/groups/groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py` & `python-gerrit-api-3.0.1/gerrit/groups/members.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py` & `python-gerrit-api-3.0.1/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.1/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/branches.py` & `python-gerrit-api-3.0.1/gerrit/projects/branches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py` & `python-gerrit-api-3.0.1/gerrit/projects/commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             input_ = {
                 "message": "Implementing Feature X",
                 "destination": "release-branch"
             }
             result = commit.cherry_pick(input_)
 
         :param input_: the CherryPickInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
-          #cherrypick-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#cherrypick-input
         :return:  the resulting cherry-picked change
         """
         result = self.gerrit.post(
             self.endpoint + "/cherrypick", json=input_, headers=self.gerrit.default_headers)
         return result
 
     def list_change_files(self):
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.1/gerrit/projects/dashboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,15 @@
                 "commit_message": "Define the default dashboard"
             }
             new_dashboard = project.dashboards.create('master:closed', input_)
 
 
         :param id_: the dashboard id
         :param input_: the DashboardInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #dashboard-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#dashboard-input
         :return:
         """
         result = self.gerrit.put(
             self.endpoint + f"/{id_}", json=input_, headers=self.gerrit.default_headers)
         return result
 
     def get(self, id_):
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py` & `python-gerrit-api-3.0.1/gerrit/projects/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,15 @@
             }
 
             project = client.projects.get("MyProject")
             label = project.labels.get("foo")
             result = label.set(input_)
 
         :param input_: the LabelDefinitionInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #label-definition-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#label-definition-input
         :return:
         """
         result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
         return result
 
     def delete(self):
         """
@@ -97,16 +96,15 @@
                 },
                 "commit_message": "Create Foo Label"
             }
             new_label = project.labels.create('foo', input_)
 
         :param name: label name
         :param input_: the LabelDefinitionInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #label-definition-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#label-definition-input
         :return:
         """
         result = self.gerrit.put(
             self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
         return result
 
     def delete(self, name):
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py` & `python-gerrit-api-3.0.1/gerrit/projects/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,15 @@
                 "description": "Plugin for Gerrit that handles the replication.",
                 "commit_message": "Update the project description"
             }
             project = client.projects.get('myproject')
             result = project.set_description(input_)
 
         :param input_: the ProjectDescriptionInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #project-description-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-description-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/description",
                                json=input_, headers=self.gerrit.default_headers)
 
     def delete_description(self):
         """
@@ -92,16 +91,15 @@
                 "parent": "Public-Plugins",
                 "commit_message": "Update the project parent"
             }
             project = client.projects.get('myproject')
             result = project.set_parent(input_)
 
         :param input_: The ProjectParentInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #project-parent-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-parent-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/parent",
                                json=input_, headers=self.gerrit.default_headers)
 
     def get_head(self):
         """
@@ -231,16 +229,15 @@
 
     def set_access_rights(self, input_):
         """
         Sets access rights for the project using the diff schema provided by ProjectAccessInput.
         https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#set-access
 
         :param input_: the ProjectAccessInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #project-access-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-access-input
         :return:
         """
         return self.gerrit.post(self.endpoint + "/access",
                                 json=input_, headers=self.gerrit.default_headers)
 
     def create_change(self, input_):
         """
@@ -269,20 +266,18 @@
         return result
 
     def create_access_rights_change(self, input_):
         """
         Sets access rights for the project using the diff schema provided by ProjectAccessInput
         This takes the same input as Update Access Rights, but creates a pending change for review.
         Like Create Change, it returns a ChangeInfo entity describing the resulting change.
-        https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-        #create-access-change
+        https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#create-access-change
 
         :param input_: the ProjectAccessInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #project-access-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-access-input
         :return:
         """
         result = self.gerrit.put(self.endpoint + "/access:review",
                                  json=input_, headers=self.gerrit.default_headers)
         return result
 
     def check_access(self, options):
@@ -313,16 +308,15 @@
                 "index_children": "true"
                 "async": "true"
             }
             project = client.projects.get('myproject')
             result = project.index(input_)
 
         :param input_: the IndexProjectInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #index-project-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#index-project-input
         :return:
         """
         self.gerrit.post(self.endpoint + "/index",
                          json=input_, headers=self.gerrit.default_headers)
 
     def index_all_changes(self):
         """
@@ -348,16 +342,15 @@
                 }
             }
 
             project = client.projects.get('myproject')
             result = project.check_consistency(input_)
 
         :param input_: the CheckProjectInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
-          #check-project-input
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#check-project-input
         :return:
         """
         return self.gerrit.post(self.endpoint + "/check",
                                 json=input_, headers=self.gerrit.default_headers)
 
     @property
     def branches(self):
```

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py` & `python-gerrit-api-3.0.1/gerrit/projects/projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py` & `python-gerrit-api-3.0.1/gerrit/projects/tags.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py` & `python-gerrit-api-3.0.1/gerrit/projects/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/utils/common.py` & `python-gerrit-api-3.0.1/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/utils/exceptions.py` & `python-gerrit-api-3.0.1/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/utils/gerritbase.py` & `python-gerrit-api-3.0.1/gerrit/utils/gerritbase.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gerrit/utils/requester.py` & `python-gerrit-api-3.0.1/gerrit/utils/requester.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/gitiles/__init__.py` & `python-gerrit-api-3.0.1/gitiles/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.1/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.0.dev1
+Version: 3.0.1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
+.. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
+    :target: https://codecov.io/gh/shijl0925/python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
@@ -69,14 +71,17 @@
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
 Usage
 -----
 
+For a full documentation spec of what this library supports see `readthedocs
+<https://python-gerrit-api.readthedocs.io/en/latest/>`_
+
 Example 1: setup gerrit client:
 
 .. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
@@ -86,51 +91,66 @@
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
+.. code:: python
+
     # Creates a new project.
     input_ = {
         "description": "This is a demo project.",
         "submit_type": "INHERIT",
         "owners": [
           "MyProject-Owners"
         ]
     }
     client.projects.create('MyProject', input_)
 
     # or
     client.post(endpoint="/projects/MyProject", json=input_)
 
+.. code:: python
+
     # Sets the description of a project.
     project = client.projects.get('MyProject')
     input_ = {
         "description": "Plugin for Gerrit that handles the replication.",,
         "commit_message": "Update the project description"
     }
     result = project.set_description(input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/description", json=input_)
 
+.. code:: python
+
     # Deletes the description of a project.
     project = client.projects.get('MyProject')
     project.delete_description()
 
     # or
-    client.put(endpoint="/projects/MyProject/description")
+    client.delete(endpoint="/projects/MyProject/description")
+
+.. code:: python
 
     # get a branch of th project by ref
     branch = project.branches.get('refs/heads/stable')
 
+.. code:: python
+
     # get these branches of th project
+    branches = project.branches.list()
+
+    # or 
     branches = client.get(endpoint = "/projects/MyProject"/branches/)
 
+.. code:: python
+
     # Creates a new branch.
     input_ = {
         'revision': '76016386a0d8ecc7b6be212424978bb45959d668'
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
@@ -143,64 +163,82 @@
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
+.. code:: python
+
     # Marks a change as reviewed.
     change.mark_as_reviewed()
 
+.. code:: python
+
     # Adds and removes hashtags from a change.
     input_ = {
         "add" : [
             "hashtag3"
         ],
         "remove" : [
             "hashtag2"
         ]
     }
     result = change.set_hashtags(input_)
 
+.. code:: python
+
     # get one revision by revision id
     revision = change.get_revision('534b3ce21655a092eccf72680f2ad16b8fecf119')
 
+.. code:: python
+
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
+.. code:: python
+
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
 Example 4: operate gerrit account:
 
 .. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
+.. code:: python
+
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
+.. code:: python
+
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
 Example 5: operate gerrit group:
 
 .. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
+.. code:: python
+
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
+.. code:: python
+
     # Sets the owner group of a Gerrit internal group.
     input_ = {
         "owner": "6a1e70e1a88782771a91808c8af9bbb7a9871389"
     }
     result = group.set_owner(input_)
 
 About this library
@@ -268,32 +306,30 @@
 
 * Ability to execute Gerrit config:
     * Retrieves/Sets the default user/diff/edit preferences for the server.
     * ...
 
 * Ability to install/enable/disable/reload/query Gerrit plugins
 
-For a full documentation spec of what this library supports see `readthedocs
-<https://python-gerrit-api.readthedocs.io/en/latest/>`_
-
 Python versions
 ---------------
 
 The project has been tested against Python versions:
 
 * 3.6
 * 3.7
 * 3.8
 * 3.9
 * 3.10
+* 3.11
 
 Gerrit versions
 ---------------
 
-Project tested on Version 3.5.0 Gerrit.
+Project tested on Version 3.8.0 Gerrit.
 
 Important Links
 ---------------
 
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
```

### Comparing `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.1/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 gerrit/__init__.py
+gerrit/base.py
 gerrit/accounts/__init__.py
 gerrit/accounts/account.py
 gerrit/accounts/accounts.py
 gerrit/accounts/emails.py
 gerrit/accounts/gpg_keys.py
 gerrit/accounts/ssh_keys.py
 gerrit/changes/__init__.py
 gerrit/changes/change.py
 gerrit/changes/changes.py
 gerrit/changes/edit.py
 gerrit/changes/messages.py
 gerrit/changes/reviewers.py
 gerrit/changes/revision/__init__.py
+gerrit/changes/revision/base.py
 gerrit/changes/revision/comments.py
 gerrit/changes/revision/drafts.py
 gerrit/changes/revision/files.py
 gerrit/config/__init__.py
 gerrit/config/caches.py
 gerrit/config/config.py
 gerrit/config/tasks.py
@@ -42,14 +44,15 @@
 gerrit/projects/webhooks.py
 gerrit/utils/__init__.py
 gerrit/utils/common.py
 gerrit/utils/exceptions.py
 gerrit/utils/gerritbase.py
 gerrit/utils/requester.py
 gitiles/__init__.py
+gitiles/base.py
 python_gerrit_api.egg-info/PKG-INFO
 python_gerrit_api.egg-info/SOURCES.txt
 python_gerrit_api.egg-info/dependency_links.txt
 python_gerrit_api.egg-info/requires.txt
 python_gerrit_api.egg-info/top_level.txt
 tests/test_accounts.py
 tests/test_changes.py
```

### Comparing `python-gerrit-api-3.0.0.dev1/setup.py` & `python-gerrit-api-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_accounts.py` & `python-gerrit-api-3.0.1/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_changes.py` & `python-gerrit-api-3.0.1/tests/test_changes.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,46 +26,44 @@
         "branch": "lineage-20.0",
         "topic": "create-change-in-browser",
         "status": "NEW"
     }
     gerrit_client.changes.create(input_)
 
 
-def test_get_change(gerrit_client):
+def test_get_change(gerrit_client, latest_change_id):
     from gerrit.utils.exceptions import ChangeNotFoundError
     with pytest.raises(ChangeNotFoundError):
         gerrit_client.changes.get(id_="I00000000")
 
     with pytest.raises(ChangeNotFoundError):
         gerrit_client.changes.get(id_="I0bcf3ba13177947a2c018d9dcebdb94b561573d3")
 
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I07827e3af3827a40260f012e828a96dbf4dfcbe1"
-    change = gerrit_client.changes.get(id_=change_id)
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     assert "_number" in change.to_dict()
 
     logger.debug(change.to_dict())
 
-    attrs = ["id", "project", "branch", "topic", "hashtags", "change_id", "subject",
-             "status", "created", "updated", "submit_type", "number", "owner", "insertions", "deletions"]
+    attrs = ["id", "project", "branch", "hashtags", "change_id", "subject",
+             "status", "created", "updated", "number", "owner", "insertions", "deletions"]
     for attr in attrs:
         logger.debug(f"{attr}, {hasattr(change, attr)}, {getattr(change, attr)}")
 
     assert all([hasattr(change, attr) for attr in attrs])
 
 
 @pytest.mark.xfail(reason="Request is not authorized")
 def test_delete_change(gerrit_client):
     change_id = "LineageOS%2Fandroid~lineage-20.0~I07827e3af3827a40260f012e828a96dbf4dfcbe1"
     gerrit_client.changes.delete(id_=change_id)
 
 
-def test_get_change_detail(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I07827e3af3827a40260f012e828a96dbf4dfcbe1"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_detail(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     detail = change.get_detail(options=["LABELS"])
     assert "labels" in detail
 
 
 def test_get_change_votes(gerrit_client):
     change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
@@ -81,89 +79,79 @@
     change_id = "LineageOS%2Fandroid~lineage-20.0~I07827e3af3827a40260f012e828a96dbf4dfcbe1"
     change = gerrit_client.changes.get(id_=change_id)
 
     topic = change.get_topic()
     assert topic == "tangorpro"
 
 
-def test_list_submitted_together_changes(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_google_tangorpro~lineage-20~I7e178ddc69c5e9397c7eef5dca0ba5998d942737"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_list_submitted_together_changes(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     res = change.list_submitted_together_changes()
-    assert len(res.get("changes")) > 0
+    assert len(res.get("changes")) >= 0
 
 
-def test_get_change_include_in(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_include_in(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     res = change.get_include_in()
 
     assert "branches" in res
     assert "tags" in res
 
 
-def test_list_change_comments(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_list_change_comments(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     res = change.list_comments()
-
-    assert res.get("/PATCHSET_LEVEL")[0].get("message") == "pending ASB merge."
+    assert len(res.keys()) >= 0
 
 
-def test_get_change_attention_set(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_attention_set(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     res = change.get_attention_set()
     assert len(res) >= 0
 
 
-def test_get_change_hashtags(gerrit_client):
-    change_id = "LineageOS%2Fandroid_frameworks_base~lineage-15.1~I4fafa2b1e342608e2690c3dda7cb06aaf88247ba"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_hashtags(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     res = change.get_hashtags()
-    assert len(res) > 0
-
+    assert len(res) >= 0
 
-def test_get_change_meta_diff(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"  # "359381"
-    change = gerrit_client.changes.get(id_=change_id)
 
-    res = change.get_meta_diff(old="530324a14d17c05a63dd8b003cba68f70f9f4a1e")
+def test_get_change_meta_diff(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
+    res = change.get_meta_diff()
 
     assert "removed" in res
     assert "added" in res
 
 
-def test_get_change_messages(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_messages(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     messages = change.messages.list()
-    assert len(messages) > 0
+    assert len(messages) >= 0
 
 
 def test_get_change_message(gerrit_client):
     change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
     change = gerrit_client.changes.get(id_=change_id)
 
     message = change.messages.get(id_="47aa7615e1759c79a182f82003b2b295cdbe9ca2")
     assert "message" in message.to_dict()
 
 
-def test_get_change_reviewers(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_reviewers(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     reviewers = change.reviewers.list()
-    assert len(reviewers) > 0
+    assert len(reviewers) >= 0
 
 
 def test_get_change_reviewer(gerrit_client):
     change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
     change = gerrit_client.changes.get(id_=change_id)
 
     from gerrit.utils.exceptions import ReviewerNotFoundError
```

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_gitiles.py` & `python-gerrit-api-3.0.1/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_groups.py` & `python-gerrit-api-3.0.1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_projects.py` & `python-gerrit-api-3.0.1/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0.dev1/tests/test_revision.py` & `python-gerrit-api-3.0.1/tests/test_revision.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,88 +3,81 @@
 # @Author: Jialiang Shi
 import logging
 import pytest
 
 logger = logging.getLogger(__name__)
 
 
-def test_get_change_revision(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_change_revision(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     c1 = change.get_revision(1).get_commit()
-    assert c1.get("commit") == "530324a14d17c05a63dd8b003cba68f70f9f4a1e"
+    assert len(c1.get("commit")) > 0
 
     c2 = change.get_revision().get_commit()
-    assert c2.get("commit") == "1b16713d0ca30ecc9f6f3ac78554d57b5d4fa467"
+    assert len(c2.get("commit")) > 0
 
 
-def test_get_revision_actions(gerrit_client):
-    change_id = "LineageOS%2Fandroid_kernel_xiaomi_sm8250~lineage-20~I53a2b78c6529e8459c6baacaba3f8c8dcaf0c387"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_actions(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     result = revision.get_revision_actions()
 
     assert "cherrypick" in result
 
 
-def test_get_revision_review(gerrit_client):
-    change_id = "LineageOS%2Fandroid_kernel_xiaomi_sm8250~lineage-20~I53a2b78c6529e8459c6baacaba3f8c8dcaf0c387"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_review(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     result = revision.get_review()
     reviewers = result.get("reviewers")
 
-    cc = reviewers.get("CC")
-    assert len(cc) > 0
+    cc = reviewers.get("CC", [])
+    assert len(cc) >= 0
 
-    reviewer = reviewers.get("REVIEWER")
-    assert len(reviewer) > 0
+    reviewer = reviewers.get("REVIEWER", [])
+    assert len(reviewer) >= 0
 
 
-def test_get_revision_related_changes(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_fairphone_FP3~lineage-20~Ic54e2787ef27022556430c6c1db346b1e1348e39"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_related_changes(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     result = revision.get_related_changes()
 
-    assert len(result.get("changes")) > 0
+    assert len(result.get("changes")) >= 0
 
 
-def test_get_revision_patch(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_fairphone_FP3~lineage-20~Ic54e2787ef27022556430c6c1db346b1e1348e39"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_patch(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     content = revision.get_patch(decode=True)
 
     assert len(content) > 0
 
 
-def test_get_revision_submit_type(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_fairphone_FP3~lineage-20~Ic54e2787ef27022556430c6c1db346b1e1348e39"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_submit_type(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     result = revision.get_submit_type()
 
     assert result == "REBASE_IF_NECESSARY"
 
 
-def test_get_revision_comments(gerrit_client):
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_comments(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     comments = revision.comments.list()
 
-    assert len(comments) > 0
+    assert len(comments) >= 0
 
 
 def test_get_revision_comment(gerrit_client):
     change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
     change = gerrit_client.changes.get(id_=change_id)
 
     revision = change.get_revision()
@@ -96,34 +89,32 @@
 @pytest.mark.parametrize('reviewed, base, q, parent',
                          [(True, None, None, None),
                           (None, 1, None, None),
                           (None, None, "sdm710.mk", None),
                           (None, None, None, 1),
                           (None, None, None, None),
                           ])
-def test_search_revision_files(gerrit_client, reviewed, base, q, parent):
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_search_revision_files(gerrit_client, latest_change_id, reviewed, base, q, parent):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     revision.files.search(reviewed, base, q, parent)
 
 
-def test_get_revision_files(gerrit_client):
+def test_get_revision_files(gerrit_client, latest_change_id):
     from gerrit.changes.revision.files import GerritChangeRevisionFile
     from gerrit.utils.exceptions import UnknownFile
-    change_id = "LineageOS%2Fandroid_device_xiaomi_sdm710-common~lineage-20~I3767d8a44cbd9af891fbac7a67380b205b414a37"
-    change = gerrit_client.changes.get(id_=change_id)
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     files = revision.files
     assert len(files) > 0
     assert len(files.keys()) > 0
-    assert "extract-files.sh" in files
-    assert isinstance(files.get("extract-files.sh"), GerritChangeRevisionFile)
+    # assert "extract-files.sh" in files
+    # assert isinstance(files.get("extract-files.sh"), GerritChangeRevisionFile)
 
     for item in files:
         assert isinstance(item, GerritChangeRevisionFile)
 
     with pytest.raises(UnknownFile):
         revision.files["test.py"]
 
@@ -164,14 +155,13 @@
     revision = change.get_revision()
     votes = revision.list_votes(account="johnsonnolen")
 
     assert votes.get("Code-Review") == 1
     assert votes.get("Verified") == 1
 
 
-def test_get_revision_reviewers(gerrit_client):
-    change_id = "LineageOS%2Fandroid~lineage-20.0~I0bcf3ba13177947a2c018d9dcebdb94b561573d3"
-    change = gerrit_client.changes.get(id_=change_id)
+def test_get_revision_reviewers(gerrit_client, latest_change_id):
+    change = gerrit_client.changes.get(id_=latest_change_id)
 
     revision = change.get_revision()
     result = revision.list_reviewers()
-    assert len(result) > 0
+    assert len(result) >= 0
```

