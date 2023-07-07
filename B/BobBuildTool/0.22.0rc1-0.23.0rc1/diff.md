# Comparing `tmp/BobBuildTool-0.22.0rc1.tar.gz` & `tmp/BobBuildTool-0.23.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BobBuildTool-0.22.0rc1.tar", last modified: Wed Nov 16 16:40:00 2022, max compression
+gzip compressed data, was "BobBuildTool-0.23.0rc1.tar", last modified: Fri Jul  7 20:03:25 2023, max compression
```

## Comparing `BobBuildTool-0.22.0rc1.tar` & `BobBuildTool-0.23.0rc1.tar`

### file list

```diff
@@ -1,176 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/.github/workflows/workflow.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    35498 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      345 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/bob
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/bob.cmd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/contrib/bash-completion/
--rw-r--r--   0 runner    (1001) docker     (121)    13213 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/bash-completion/bob
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/cleanup-recipes.awk
--rwxr-xr-x   0 runner    (1001) docker     (121)     1480 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/create-release.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      551 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/notify.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/contrib/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/plugins/jenkins-cobertura.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/plugins/override.py
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/plugins/path-fmt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/contrib/sandbox.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)    52308 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/BOB_Logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    51445 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/BOB_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6750 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/_build/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/_build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)   218324 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/_static/d3.v4.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    25786 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/_static/sandbox.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (121)    67229 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/cheatsheet/bob_cheatsheet.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/cheatsheet/bob_cheatsheet.tex
--rw-r--r--   0 runner    (1001) docker     (121)    11668 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (121)   129885 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/jenkins.odg
--rw-r--r--   0 runner    (1001) docker     (121)    48173 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/jenkins.png
--rw-r--r--   0 runner    (1001) docker     (121)    10648 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/overview.odg
--rw-r--r--   0 runner    (1001) docker     (121)    17248 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/overview.png
--rw-r--r--   0 runner    (1001) docker     (121)    28093 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/recipe-flow.odg
--rw-r--r--   0 runner    (1001) docker     (121)    80846 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/recipe-flow.png
--rw-r--r--   0 runner    (1001) docker     (121)    47205 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/sandbox_graph.png
--rw-r--r--   0 runner    (1001) docker     (121)    18826 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/variant-management.odg
--rw-r--r--   0 runner    (1001) docker     (121)    19985 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/images/variant-management.png
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7807 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/manpages/
--rw-r--r--   0 runner    (1001) docker     (121)     7193 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-archive.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10832 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-build-dev.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-build.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-clean.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-dev.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-graph.rst
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-init.rst
--rw-r--r--   0 runner    (1001) docker     (121)    25086 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-jenkins.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-ls.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-project.rst
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-query-meta.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-query-path.rst
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-query-recipe.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-query-scm.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-show.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob-status.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3595 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bob.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14703 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/bobpaths.rst
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manpages/std-opt-cfg.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/manual/
--rw-r--r--   0 runner    (1001) docker     (121)     9298 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/audit-trail.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14381 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (121)   112852 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13197 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/extending.rst
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23464 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/manual/policies.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/releases/
--rw-r--r--   0 runner    (1001) docker     (121)     8403 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.13.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12628 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.14.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14335 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.15.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10360 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.16.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8909 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.17.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.18.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.19.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.20.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.21.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/0.22.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/releases/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/doc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)    14011 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/tutorial/compile.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/tutorial/create.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/tutorial/fingerprints.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21009 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/doc/tutorial/jenkins.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3721 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43494 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)    12425 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/audit.py
--rw-r--r--   0 runner    (1001) docker     (121)    82417 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18385 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17201 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    10133 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     5383 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/state.py
--rw-r--r--   0 runner    (1001) docker     (121)    12866 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/build/status.py
--rw-r--r--   0 runner    (1001) docker     (121)    18805 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/invoke.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9158 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7051 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/intermediate.py
--rw-r--r--   0 runner    (1001) docker     (121)    71466 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11195 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/cmds/show.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/develop/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/develop/make.py
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/develop/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/
--rw-r--r--   0 runner    (1001) docker     (121)    18762 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/EclipseCdtGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)    25589 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/QtCreatorGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)    17143 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/VisualStudio.py
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/VisualStudioCode.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13735 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/generators/common.py
--rw-r--r--   0 runner    (1001) docker     (121)   160778 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/input.py
--rw-r--r--   0 runner    (1001) docker     (121)    19940 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/intermediate.py
--rw-r--r--   0 runner    (1001) docker     (121)    22252 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/invoker.py
--rw-r--r--   0 runner    (1001) docker     (121)    28532 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/languages.py
--rw-r--r--   0 runner    (1001) docker     (121)    35323 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/pathspec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7383 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/cvs.py
--rw-r--r--   0 runner    (1001) docker     (121)    45739 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/imp.py
--rw-r--r--   0 runner    (1001) docker     (121)    13226 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/scm.py
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/svn.py
--rw-r--r--   0 runner    (1001) docker     (121)    17199 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scm/url.py
--rw-r--r--   0 runner    (1001) docker     (121)     9635 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)    12637 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/share.py
--rw-r--r--   0 runner    (1001) docker     (121)    26724 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/state.py
--rw-r--r--   0 runner    (1001) docker     (121)    19736 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/stringparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    16568 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/tty.py
--rw-r--r--   0 runner    (1001) docker     (121)    26498 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/pym/bob/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/pym/bob/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5958 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:40:00.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/
--rw-r--r--   0 runner    (1001) docker     (121)    23824 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/namespace-sandbox.c
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/network-tools.c
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/network-tools.h
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/process-tools.c
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-11-16 16:34:11.000000 BobBuildTool-0.22.0rc1/src/namespace-sandbox/process-tools.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/.github/workflows/workflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/bob
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/bob.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/contrib/bash-completion/
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/bash-completion/bob
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/cleanup-recipes.awk
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/create-release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/notify.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/contrib/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/plugins/jenkins-cobertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/plugins/override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/plugins/path-fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/contrib/sandbox.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.555699 BobBuildTool-0.23.0rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    52308 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/BOB_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51445 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/BOB_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.555699 BobBuildTool-0.23.0rc1/doc/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/_build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.555699 BobBuildTool-0.23.0rc1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)   218324 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/_static/d3.v4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25786 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/_static/sandbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.555699 BobBuildTool-0.23.0rc1/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.555699 BobBuildTool-0.23.0rc1/doc/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)    67229 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/cheatsheet/bob_cheatsheet.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/cheatsheet/bob_cheatsheet.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.559699 BobBuildTool-0.23.0rc1/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   129885 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/jenkins.odg
+-rw-r--r--   0 runner    (1001) docker     (123)    48173 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/jenkins.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/overview.odg
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28093 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/recipe-flow.odg
+-rw-r--r--   0 runner    (1001) docker     (123)    80846 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/recipe-flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47205 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/sandbox_graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/variant-management.odg
+-rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/images/variant-management.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.559699 BobBuildTool-0.23.0rc1/doc/manpages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-archive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-build-dev.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-clean.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-dev.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-init.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-jenkins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-ls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-query-meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-query-path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-query-recipe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-query-scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-show.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob-status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bob.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/bobpaths.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manpages/std-opt-cfg.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.563699 BobBuildTool-0.23.0rc1/doc/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/audit-trail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   113499 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/manual/policies.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.563699 BobBuildTool-0.23.0rc1/doc/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.13.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.14.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.15.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.16.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.17.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.18.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.19.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.20.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.21.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.22.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/0.23.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/releases/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.563699 BobBuildTool-0.23.0rc1/doc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/tutorial/compile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/tutorial/create.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/tutorial/fingerprints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/doc/tutorial/jenkins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/pym/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.563699 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.567699 BobBuildTool-0.23.0rc1/pym/bob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44506 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85560 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.567699 BobBuildTool-0.23.0rc1/pym/bob/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.567699 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/build/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/invoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71466 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/cmds/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/pym/bob/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/develop/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/develop/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/pym/bob/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/EclipseCdtGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25601 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/QtCreatorGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/VisualStudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/VisualStudioCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/generators/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163100 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35323 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/pathspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/pym/bob/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/cvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46137 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/svn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scm/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/stringparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/tty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26836 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/pym/bob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-07 20:03:25.000000 BobBuildTool-0.23.0rc1/pym/bob/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.551699 BobBuildTool-0.23.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:25.571699 BobBuildTool-0.23.0rc1/src/namespace-sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/src/namespace-sandbox/namespace-sandbox.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/src/namespace-sandbox/network-tools.c
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/src/namespace-sandbox/network-tools.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/src/namespace-sandbox/process-tools.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-07 20:03:11.000000 BobBuildTool-0.23.0rc1/src/namespace-sandbox/process-tools.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BobBuildTool-0.22.0rc1/.github/workflows/workflow.yaml` & `BobBuildTool-0.23.0rc1/.github/workflows/workflow.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 name: CI/CD
 
 on: [push, pull_request]
 
 jobs:
-    linux:
-        runs-on: ubuntu-latest
+    build-linux:
+        runs-on: ubuntu-20.04
         timeout-minutes: 15
         strategy:
             matrix:
-                python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
+                python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
             fail-fast: false
 
         steps:
             - name: Checkout
               uses: actions/checkout@v2
 
             - name: Set up Python ${{ matrix.python-version }}
@@ -37,40 +37,38 @@
               run: |
                 git config --global init.defaultBranch master # keep the old name
                 git config --global protocol.file.allow always # roll back CVE-2022-39253
                 eatmydata ./test/run-tests.sh -c xml
 
             - name: Build Python package
               run: |
-                python3 setup.py sdist bdist_wheel --plat-name manylinux1_x86_64
+                python3 setup.py bdist_wheel --plat-name manylinux1_x86_64
 
             - name: Upload coverage to Codecov
               # Coverage is not complete on Python <3.7 (see pym/bob/utils.py)
               if: matrix.python-version != '3.6'
               uses: codecov/codecov-action@v2
 
-            - name: Publish package
-              if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-              uses: pypa/gh-action-pypi-publish@release/v1
+            - name: Store the binary wheel
+              uses: actions/upload-artifact@v3
               with:
-                user: __token__
-                password: ${{ secrets.PYPI_API_TOKEN }}
-                skip_existing: true
+                name: python-package-distributions
+                path: dist
 
-    windows:
+    build-windows:
         runs-on: windows-latest
         timeout-minutes: 20
         steps:
             - name: Checkout
               uses: actions/checkout@v2
 
-            - name: Set up Python 3.10
+            - name: Set up Python 3.11
               uses: actions/setup-python@v2
               with:
-                python-version: "3.10"
+                python-version: "3.11"
 
             - name: Prepare MSYS2 environment
               run: |
                 C:\msys64\usr\bin\bash -l -c "pacman -Sy --needed --noconfirm parallel || true"
 
             - name: Cache Jenkins integration test
               uses: actions/cache@v3
@@ -87,20 +85,63 @@
               run: |
                 git config --global init.defaultBranch master # keep the old name
                 git config --global protocol.file.allow always # roll back CVE-2022-39253
                 $env:PATH = "$env:JAVA_HOME_11_X64\bin;$env:PATH;C:\msys64\usr\bin"
                 $env:JAVA_HOME = "$env:JAVA_HOME_11_X64"
                 bash ./test/run-tests.sh -c xml
 
+            - name: Upload coverage to Codecov
+              uses: codecov/codecov-action@v2
+
+    build-sdist:
+        runs-on: ubuntu-latest
+        timeout-minutes: 5
+        steps:
+            - name: Checkout
+              uses: actions/checkout@v2
+
+            - name: Set up Python 3.11
+              uses: actions/setup-python@v2
+              with:
+                python-version: "3.11"
+
+            - name: Install dependencies
+              run: |
+                python -m pip install --upgrade pip
+                pip install PyYAML schema python-magic pyparsing sphinx wheel
+
             - name: Build Python package
               run: |
-                python3 setup.py sdist bdist_wheel
+                python3 setup.py sdist
 
-            - name: Upload coverage to Codecov
-              uses: codecov/codecov-action@v2
+            - name: Store the source distribution
+              uses: actions/upload-artifact@v3
+              with:
+                name: python-package-distributions
+                path: dist
+
+    publish:
+        runs-on: ubuntu-latest
+        timeout-minutes: 5
+        needs:
+            # Depend on all builds even if they don't provide an artifact (e.g.
+            # windows). This makes sure we publish only if everything is ok.
+            - build-linux
+            - build-windows
+            - build-sdist
+        steps:
+            - name: Download all the dists
+              uses: actions/download-artifact@v3
+              with:
+                name: python-package-distributions
+                path: dist/
+
+            - name: List
+              run: |
+                ls dist
 
             - name: Publish package
               if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
               uses: pypa/gh-action-pypi-publish@release/v1
               with:
                 user: __token__
                 password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `BobBuildTool-0.22.0rc1/LICENSE` & `BobBuildTool-0.23.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/PKG-INFO` & `BobBuildTool-0.23.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: BobBuildTool
-Version: 0.22.0rc1
+Version: 0.23.0rc1
 Summary: Functional cross platform build-automation tool
 Home-page: https://bobbuildtool.github.io/
+Download-URL: https://github.com/BobBuildTool/bob/releases
 Author: Jan Klötzke
 Author-email: jan@kloetzke.net
 License: GPLv3+
-Download-URL: https://github.com/BobBuildTool/bob/releases
-Description: [Bob Build Tool](https://bobbuildtool.github.io/)
-        =================================================
-        
-        Bob is a build automation tool inspired by bitbake and portage. It is intended
-        for complex embedded projects and thus focuses on reproducible builds while
-        still being nice to developers in agile environments.
-        
-        [![Documentation Status](http://readthedocs.org/projects/bob-build-tool/badge/?version=latest)](http://bob-build-tool.readthedocs.io/en/latest/?badge=latest)
-        [![Build Status](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml/badge.svg)](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml)
-        [![codecov.io](https://codecov.io/github/BobBuildTool/bob/coverage.svg?branch=master)](https://codecov.io/github/BobBuildTool/bob?branch=master)
-        
-        Installation
-        ============
-        
-        To install the latest release just do a:
-        
-            $ python3 -m pip install BobBuildTool [--user]
-        
-        See the [installation instructions](https://bob-build-tool.readthedocs.io/en/latest/installation.html)
-        for more information and other methods.
-        
-        Getting started
-        ===============
-        
-        It's probably the best to head over to the
-        [documentation](http://bob-build-tool.readthedocs.io/). To get an impression
-        of how Bob is configured, have a look at the
-        [tutorials](https://github.com/BobBuildTool/bob-tutorials). A real project that
-        is built by Bob can be found [here](https://github.com/BobBuildTool/basement).
-        
-        The [Cheat Sheet](doc/cheatsheet/bob_cheatsheet.pdf) shows common used keywords
-        and commands.
-        
-        If you have a specific question you're welcome to post on the
-        [mailing list](mailto:bob-build-tool@freelists.org)
-        ([FreeLists](http://www.freelists.org/list/bob-build-tool)).
 Keywords: bob build-automation build-system
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: azure
+License-File: LICENSE
+
+[Bob Build Tool](https://bobbuildtool.github.io/)
+=================================================
+
+Bob is a build automation tool inspired by bitbake and portage. It is intended
+for complex embedded projects and thus focuses on reproducible builds while
+still being nice to developers in agile environments.
+
+[![Documentation Status](http://readthedocs.org/projects/bob-build-tool/badge/?version=latest)](http://bob-build-tool.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml/badge.svg)](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml)
+[![codecov.io](https://codecov.io/github/BobBuildTool/bob/coverage.svg?branch=master)](https://codecov.io/github/BobBuildTool/bob?branch=master)
+
+Installation
+============
+
+To install the latest release just do a:
+
+    $ python3 -m pip install BobBuildTool [--user]
+
+See the [installation instructions](https://bob-build-tool.readthedocs.io/en/latest/installation.html)
+for more information and other methods.
+
+Getting started
+===============
+
+It's probably the best to head over to the
+[documentation](http://bob-build-tool.readthedocs.io/). To get an impression
+of how Bob is configured, have a look at the
+[tutorials](https://github.com/BobBuildTool/bob-tutorials). A real project that
+is built by Bob can be found [here](https://github.com/BobBuildTool/basement).
+
+The [Cheat Sheet](doc/cheatsheet/bob_cheatsheet.pdf) shows common used keywords
+and commands.
+
+If you have a specific question you're welcome to post on the
+[mailing list](mailto:bob-build-tool@freelists.org)
+([FreeLists](http://www.freelists.org/list/bob-build-tool)).
```

### Comparing `BobBuildTool-0.22.0rc1/README.md` & `BobBuildTool-0.23.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/bash-completion/bob` & `BobBuildTool-0.23.0rc1/contrib/bash-completion/bob`

 * *Files 2% similar despite different names*

```diff
@@ -420,15 +420,15 @@
                chroot+=( "${COMP_WORDS[parse_pos]}" )
                : $((parse_pos++))
             fi
             ;;
          -C?*)
             chroot+=( "${c:2}" )
             ;;
-         --query)
+         --query | --debug | --color)
             if [[ $parse_pos -lt $COMP_CWORD ]] ; then
                : $((parse_pos++))
             fi
             ;;
          -*) ;;
          *) command="$c" ; break ;;
       esac
@@ -436,21 +436,26 @@
 
    if [[ -z "$command" ]] ; then
       case "$cur" in
          -C?*)
             __bob_complete_dir "${cur:2}" "-C"
             ;;
          -*)
-            __bob_complete_words "-h --help -i --version -C --query"
+            __bob_complete_words "-h --help -i --version -C --query
+               --debug --color"
             ;;
          *)
             if [[ $prev == "-C" ]] ; then
                __bob_complete_dir "$cur"
             elif [[ $prev == "--query" ]] ; then
                __bob_complete_words "nullset nullglob nullfail"
+            elif [[ $prev == "--debug" ]] ; then
+               __bob_complete_words "pkgck ngd prof"
+            elif [[ $prev == "--color" ]] ; then
+               __bob_complete_words "never always auto"
             else
                __bob_complete_words "$1"
             fi
             ;;
       esac
    else
       local completion_func="__bob_${2-}${2+_}${command//-/_}"
```

### Comparing `BobBuildTool-0.22.0rc1/contrib/cleanup-recipes.awk` & `BobBuildTool-0.23.0rc1/contrib/cleanup-recipes.awk`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/create-release.sh` & `BobBuildTool-0.23.0rc1/contrib/create-release.sh`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/notify.sh` & `BobBuildTool-0.23.0rc1/contrib/notify.sh`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/plugins/jenkins-cobertura.py` & `BobBuildTool-0.23.0rc1/contrib/plugins/jenkins-cobertura.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/plugins/override.py` & `BobBuildTool-0.23.0rc1/contrib/plugins/override.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/plugins/path-fmt.py` & `BobBuildTool-0.23.0rc1/contrib/plugins/path-fmt.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/contrib/sandbox.rst` & `BobBuildTool-0.23.0rc1/contrib/sandbox.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/BOB_Logo.png` & `BobBuildTool-0.23.0rc1/doc/BOB_Logo.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/BOB_Logo.svg` & `BobBuildTool-0.23.0rc1/doc/BOB_Logo.svg`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/Makefile` & `BobBuildTool-0.23.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/_static/d3.v4.min.js` & `BobBuildTool-0.23.0rc1/doc/_static/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/_static/sandbox.html` & `BobBuildTool-0.23.0rc1/doc/_static/sandbox.html`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/cheatsheet/bob_cheatsheet.pdf` & `BobBuildTool-0.23.0rc1/doc/cheatsheet/bob_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/cheatsheet/bob_cheatsheet.tex` & `BobBuildTool-0.23.0rc1/doc/cheatsheet/bob_cheatsheet.tex`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/conf.py` & `BobBuildTool-0.23.0rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/glossary.rst` & `BobBuildTool-0.23.0rc1/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/jenkins.odg` & `BobBuildTool-0.23.0rc1/doc/images/jenkins.odg`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/jenkins.png` & `BobBuildTool-0.23.0rc1/doc/images/jenkins.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/overview.odg` & `BobBuildTool-0.23.0rc1/doc/images/overview.odg`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/overview.png` & `BobBuildTool-0.23.0rc1/doc/images/overview.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/recipe-flow.odg` & `BobBuildTool-0.23.0rc1/doc/images/recipe-flow.odg`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/recipe-flow.png` & `BobBuildTool-0.23.0rc1/doc/images/recipe-flow.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/sandbox_graph.png` & `BobBuildTool-0.23.0rc1/doc/images/sandbox_graph.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/variant-management.odg` & `BobBuildTool-0.23.0rc1/doc/images/variant-management.odg`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/images/variant-management.png` & `BobBuildTool-0.23.0rc1/doc/images/variant-management.png`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/index.rst` & `BobBuildTool-0.23.0rc1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/installation.rst` & `BobBuildTool-0.23.0rc1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-archive.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-archive.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-build-dev.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-build-dev.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-build.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-build.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-clean.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-clean.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-dev.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-dev.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-graph.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-graph.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-init.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-init.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-jenkins.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-jenkins.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-ls.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-ls.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-project.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-project.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-query-meta.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-query-meta.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-query-path.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-query-path.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-query-recipe.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-query-recipe.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-query-scm.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-query-scm.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-show.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-show.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob-status.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob-status.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bob.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bob.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manpages/bobpaths.rst` & `BobBuildTool-0.23.0rc1/doc/manpages/bobpaths.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/audit-trail.rst` & `BobBuildTool-0.23.0rc1/doc/manual/audit-trail.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/concepts.rst` & `BobBuildTool-0.23.0rc1/doc/manual/concepts.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/configuration.rst` & `BobBuildTool-0.23.0rc1/doc/manual/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -904,29 +904,31 @@
                                     |        ``url``: (optional, Regex-String, default: ``.*``). The matching part
                                     |           of the remote URL is replaced by
                                     |        ``repo``: (String) local storage path.
                                     |        ``optional``: (Boolean, default True). Marks the reference as
                                     |           optional if true. Otherwise a error is raised if the
                                     |           local reference repo didn't exitst.
                                     |   Note: ``references`` are not used for submodules.
+                                    | ``retries`` (\*): Number of retries before the checkout is set to failed.
                                     | ``disassociate``: (Boolean, default false). Diasassociate the reference.
 import Import directory from        | ``url``: Directory path relative to project root.
        project                      | ``prune`` (\*): Delete destination directory before importing files.
 svn    `Svn`_ repository            | ``url``: URL of SVN module
                                     | ``revision``: Optional revision number (optional)
                                     | ``sslVerify`` (\*): Whether to verify the SSL certificate when fetching (optional)
 url    While not a real SCM it      | ``url``: File that should be downloaded
        allows to download (and      | ``digestSHA1``: Expected SHA1 digest of the file (optional)
        extract) files/archives.     | ``digestSHA256``: Expected SHA256 digest of the file (optional)
                                     | ``digestSHA512``: Expected SHA512 digest of the file (optional)
                                     | ``extract`` (\*): Extract directive (optional, default: auto)
                                     | ``fileName`` (\*): Local file name (optional, default: url file name)
                                     | ``sslVerify`` (\*): Whether to verify the SSL certificate when fetching (optional)
                                     | ``stripComponents`` (\*): Number of leading components stripped from file name
-                                                                (optional, tar files only)
+                                    |                           (optional, tar files only)
+                                    | ``retries`` (\*): Number of retries before the checkout is set to failed.
 ====== ============================ =======================================================================================
 
 The following synthetic attributes exist. They are generated internally
 and cannot be set in the recipe. They are intended to be matched in queries
 or to show additional information.
 
 * ``overridden``: Boolean that is true if a :ref:`configuration-config-scmOverrides`
@@ -1174,14 +1176,15 @@
 Detailed entries must either contain a ``name`` property or a ``depends`` list.
 The following settings are supported:
 
 +-------------+-----------------+-----------------------------------------------------+
 | Name        | Type            | Description                                         |
 +=============+=================+=====================================================+
 | name        | String          | The name of the required recipe.                    |
+|             |                 | String substitution is applied to this setting.     |
 +-------------+-----------------+-----------------------------------------------------+
 | depends     | List of         | A list of dependencies inheriting the settings of   |
 |             | Dependencies    | this entry.                                         |
 +-------------+-----------------+-----------------------------------------------------+
 | use         | List of strings | List of the results that are used from the package. |
 |             |                 | The following values are allowed:                   |
 |             |                 |                                                     |
@@ -1563,15 +1566,16 @@
 
 Type: List of Patterns
 
 The ``provideDeps`` keyword receives a list of dependency names. These must be
 dependencies of the current recipe, i.e. they must appear in the ``depends``
 section. It is no error if the condition of such a dependency evaluates to
 false. In this case the entry is silently dropped. To specify multiple
-dependencies with a single entry shell globbing patterns may be used.
+dependencies with a single entry shell globbing patterns may be used. As for the
+names of the dependencies string substitution is also applied to ``provideDeps``.
 
 Provided dependencies are subsequently injected into the dependency list of the
 downstream recipe that has a dependency to this one (if ``deps`` is included in
 the ``use`` attribute of the dependency, which is the default). This works in a
 transitive fashion too, that is provided dependencies of an upstream recipe
 are forwarded to the downstream recipe too.
 
@@ -2170,14 +2174,15 @@
 
 Example::
 
    scmDefaults:
       git:
          branch: "main"
          singleBranch: True
+         retries: 3
       url:
          extract: False
 
 .. _configuration-config-scmOverrides:
 
 scmOverrides
 ~~~~~~~~~~~~
@@ -2462,14 +2467,20 @@
 
     ``always``
         Use colors in output
 
     ``auto``
         Use colors only when TTY console detected (default)
 
+parallelTUIThreshold
+    Set the threshold for switching between TUIs. Default: 16
+
+    If the number of jobs exceeds this threshold the TUI switches from one
+    status line per job to a TUI using only two status lines.
+
 queryMode
     Set the behaviour of package queries when no package is matched. Can be
     overridden on the command line by the global ``--query`` option of
     :ref:`manpage-bob`.
 
     ``nullset``
         Empty sets of packages are considered a regular result and never
```

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/extending.rst` & `BobBuildTool-0.23.0rc1/doc/manual/extending.rst`

 * *Files 4% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     }
 
 .. _extending-generators:
 
 Generators
 ----------
 
-The main purpose of a generator is to generate project files for one or more IDEs. 
+The main purpose of a generator is to generate project files for one or more IDEs.
 There are several built-in generators, e.g. for QtCreator project files.
 
 A generator is called with at least 3 arguments:
 
 * ``package``: the :class:`bob.input.Package` to build the project for.
 * ``argv``: Arguments not consumed by ``bob project``.
 * ``extra``: Extra arguments to be passed back to ``bob dev`` when called from
@@ -268,14 +268,37 @@
     manifest = {
         'apiVersion' : "0.17",
         'projectGenerators' : {
             'nullGenerator' : nullGenerator,
         }
     }
 
+Traditionally a generator handles only one package. When running the generator
+this package needs to be provided using the complete path. Starting with Bob
+0.23 a generator can specify that he can handle multiple packages as a result
+of a :ref:`package query <manpage-bobpaths>`. This is done by setting the
+optional `query` property to `True`. In this case the first argument of the
+generator are the package objects returned by
+:func:`bob.pathspec.PackageSet.queryPackagePath`.::
+
+   def nullQueryGenerator(packages, argv, extra, bob):
+       for p in packages:
+           print(p.getName())
+       return 0
+
+   manifest = {
+        'apiVersion' : "0.23",
+        'projectGenerators' : {
+            'nullQueryGenerator' : {
+               'func' : nullQueryGenerator,
+               'query' : True,
+        }
+    }
+
+
 .. _extending-settings:
 
 Plugin settings
 ---------------
 
 Sometimes plugin behaviour needs to be configurable by the user. On the other
 hand Bob expects plugins to be deterministic. To have a common interface for
```

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/introduction.rst` & `BobBuildTool-0.23.0rc1/doc/manual/introduction.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/manual/policies.rst` & `BobBuildTool-0.23.0rc1/doc/manual/policies.rst`

 * *Files 4% similar despite different names*

```diff
@@ -559,7 +559,36 @@
 
 Old behavior
    ``commit`` was checked out leaving the repo in a detached HEAD state.
 
 New behavior
    Bob checks if the ``commit`` and / or ``tag`` is on the configured ``branch`` and
    performs a checkout of the ``commit`` on a local ``branch``.
+
+.. _policies-fixImportScmVariant:
+
+fixImportScmVariant
+~~~~~~~~~~~~~~~~~~~
+
+Introduced in: 0.23
+
+Bob uses the concept of a :term:`Variant-Id` to track *how* a package is built.
+This includes the sub-directory in which a particular SCM is checked out. So if
+the ``dir`` attribute of an SCM changes, the respective Variant-Id of the
+package changes too. Bob versions before 0.23 contained a bug where the ``dir``
+attribute of an ``import`` SCM was not included in the Variant-Id calculation.
+This can cause build failures or wrongly used binary artifacts if just the
+``dir`` attribute of an ``import`` SCM is changed.
+
+Fixing the bug will affect the :term:`Variant-Id` of all packages that use an
+``import`` SCM. This implies that binary artifacts of such packages will need
+to be built again. It also transitively affects packages that depend on
+packages that utilize an ``import`` SCM.
+
+Old behavior
+   Changes to the ``dir`` attribute of an ``import`` SCM do not cause rebuilds
+   of the affected package. Wrong sharing of binary artifacts for such packages
+   may occur.
+
+New behavior
+   Changes to the ``dir`` attribute of an ``import`` SCM behave the same as for
+   any other SCM.
```

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.13.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.13.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.14.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.14.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.15.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.15.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.16.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.16.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.17.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.17.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.18.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.18.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.19.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.19.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.20.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.20.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.21.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.21.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/releases/0.22.rst` & `BobBuildTool-0.23.0rc1/doc/releases/0.22.rst`

 * *Files 3% similar despite different names*

```diff
@@ -144,7 +144,12 @@
 * Added a workaround for Bash on Windows when WSL is enabled but no
   distribution is installed. Previously Bash could not be executed even though
   the MSYS2 version was in ``%PATH%``.
 * Fixed a crash in IfExpressions where a function call and a literal were
   compared, e.g.: ``foo() == "bar"``.
 * Fixed out of tree builds of projects that use the ``import`` SCM.
   (:issue:`489`).
+* Rectified schema validation of ``set`` properties of ``scmOverride``.
+  (:issue:`497`)
+* Fixed a crash of the Visual Studio and Visual Studio Code project generators
+  with packages that have a host executable file but has no checkout step.
+  (:issue:`498`)
```

### Comparing `BobBuildTool-0.22.0rc1/doc/tutorial/compile.rst` & `BobBuildTool-0.23.0rc1/doc/tutorial/compile.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Build a demo project
 ********************
 
-Prequisites
-===========
+Prerequisites
+=============
 
 You should have Bob somewhere in your ``$PATH``. As the first step clone the
 tutorial projects::
 
     $ git clone https://github.com/BobBuildTool/bob-tutorials.git
     $ cd bob-tutorials/sandbox
```

### Comparing `BobBuildTool-0.22.0rc1/doc/tutorial/fingerprints.rst` & `BobBuildTool-0.23.0rc1/doc/tutorial/fingerprints.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/doc/tutorial/jenkins.rst` & `BobBuildTool-0.23.0rc1/doc/tutorial/jenkins.rst`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/PKG-INFO` & `BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: BobBuildTool
-Version: 0.22.0rc1
+Version: 0.23.0rc1
 Summary: Functional cross platform build-automation tool
 Home-page: https://bobbuildtool.github.io/
+Download-URL: https://github.com/BobBuildTool/bob/releases
 Author: Jan Klötzke
 Author-email: jan@kloetzke.net
 License: GPLv3+
-Download-URL: https://github.com/BobBuildTool/bob/releases
-Description: [Bob Build Tool](https://bobbuildtool.github.io/)
-        =================================================
-        
-        Bob is a build automation tool inspired by bitbake and portage. It is intended
-        for complex embedded projects and thus focuses on reproducible builds while
-        still being nice to developers in agile environments.
-        
-        [![Documentation Status](http://readthedocs.org/projects/bob-build-tool/badge/?version=latest)](http://bob-build-tool.readthedocs.io/en/latest/?badge=latest)
-        [![Build Status](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml/badge.svg)](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml)
-        [![codecov.io](https://codecov.io/github/BobBuildTool/bob/coverage.svg?branch=master)](https://codecov.io/github/BobBuildTool/bob?branch=master)
-        
-        Installation
-        ============
-        
-        To install the latest release just do a:
-        
-            $ python3 -m pip install BobBuildTool [--user]
-        
-        See the [installation instructions](https://bob-build-tool.readthedocs.io/en/latest/installation.html)
-        for more information and other methods.
-        
-        Getting started
-        ===============
-        
-        It's probably the best to head over to the
-        [documentation](http://bob-build-tool.readthedocs.io/). To get an impression
-        of how Bob is configured, have a look at the
-        [tutorials](https://github.com/BobBuildTool/bob-tutorials). A real project that
-        is built by Bob can be found [here](https://github.com/BobBuildTool/basement).
-        
-        The [Cheat Sheet](doc/cheatsheet/bob_cheatsheet.pdf) shows common used keywords
-        and commands.
-        
-        If you have a specific question you're welcome to post on the
-        [mailing list](mailto:bob-build-tool@freelists.org)
-        ([FreeLists](http://www.freelists.org/list/bob-build-tool)).
 Keywords: bob build-automation build-system
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: azure
+License-File: LICENSE
+
+[Bob Build Tool](https://bobbuildtool.github.io/)
+=================================================
+
+Bob is a build automation tool inspired by bitbake and portage. It is intended
+for complex embedded projects and thus focuses on reproducible builds while
+still being nice to developers in agile environments.
+
+[![Documentation Status](http://readthedocs.org/projects/bob-build-tool/badge/?version=latest)](http://bob-build-tool.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml/badge.svg)](https://github.com/BobBuildTool/bob/actions/workflows/workflow.yaml)
+[![codecov.io](https://codecov.io/github/BobBuildTool/bob/coverage.svg?branch=master)](https://codecov.io/github/BobBuildTool/bob?branch=master)
+
+Installation
+============
+
+To install the latest release just do a:
+
+    $ python3 -m pip install BobBuildTool [--user]
+
+See the [installation instructions](https://bob-build-tool.readthedocs.io/en/latest/installation.html)
+for more information and other methods.
+
+Getting started
+===============
+
+It's probably the best to head over to the
+[documentation](http://bob-build-tool.readthedocs.io/). To get an impression
+of how Bob is configured, have a look at the
+[tutorials](https://github.com/BobBuildTool/bob-tutorials). A real project that
+is built by Bob can be found [here](https://github.com/BobBuildTool/basement).
+
+The [Cheat Sheet](doc/cheatsheet/bob_cheatsheet.pdf) shows common used keywords
+and commands.
+
+If you have a specific question you're welcome to post on the
+[mailing list](mailto:bob-build-tool@freelists.org)
+([FreeLists](http://www.freelists.org/list/bob-build-tool)).
```

### Comparing `BobBuildTool-0.22.0rc1/pym/BobBuildTool.egg-info/SOURCES.txt` & `BobBuildTool-0.23.0rc1/pym/BobBuildTool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 doc/releases/0.16.rst
 doc/releases/0.17.rst
 doc/releases/0.18.rst
 doc/releases/0.19.rst
 doc/releases/0.20.rst
 doc/releases/0.21.rst
 doc/releases/0.22.rst
+doc/releases/0.23.rst
 doc/releases/index.rst
 doc/tutorial/compile.rst
 doc/tutorial/create.rst
 doc/tutorial/fingerprints.rst
 doc/tutorial/index.rst
 doc/tutorial/jenkins.rst
 pym/BobBuildTool.egg-info/PKG-INFO
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/__init__.py` & `BobBuildTool-0.23.0rc1/pym/bob/__init__.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/archive.py` & `BobBuildTool-0.23.0rc1/pym/bob/archive.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import asyncio
 import base64
 import concurrent.futures
 import concurrent.futures.process
 import gzip
 import hashlib
 import http.client
+import io
 import os
 import os.path
 import signal
 import ssl
 import subprocess
 import tarfile
 import textwrap
@@ -968,103 +969,132 @@
                 if ret != 0:
                     raise ArtifactUploadError("command return with status {}".format(ret))
         finally:
             os.unlink(self.name)
         return False
 
 
+class AzureStreamReadAdapter(io.RawIOBase):
+    def __init__(self, raw):
+        super().__init__()
+        self.raw = raw
+    def readable(self):
+        return True
+    def seekable(self):
+        return False
+    def writable(self):
+        return False
+    def read(self, size = -1):
+        return self.raw.read(size)
+    def readall(self):
+        return self.raw.read()
+    def readinto(self, buf):
+        data = self.raw.read(len(buf))
+        buf[0:len(data)] = data
+        return len(data)
+
 class AzureArchive(BaseArchive):
     def __init__(self, spec):
         super().__init__(spec)
         self.__container = spec['container']
         self.__account = spec['account']
-        self.__key = spec.get('key')
-        self.__sasToken = spec.get('sasToken')
+        self.__credential = spec.get('key', spec.get('sasToken'))
+
+    def __getClient(self):
         try:
-            from azure.storage.blob import BlockBlobService
+            from azure.storage.blob import ContainerClient
         except ImportError:
             raise BuildError("azure-storage-blob Python3 library not installed!")
-        self.__service = BlockBlobService(account_name=self.__account,
-            account_key=self.__key, sas_token=self.__sasToken, socket_timeout=6000)
+        return ContainerClient("https://{}.blob.core.windows.net".format(self.__account),
+            self.__container, self.__credential)
 
     @staticmethod
     def __makeBlobName(buildId, suffix):
         packageResultId = buildIdToName(buildId)
         return "/".join([packageResultId[0:2], packageResultId[2:4],
             packageResultId[4:] + suffix])
 
     def _remoteName(self, buildId, suffix):
         return "https://{}.blob.core.windows.net/{}/{}".format(self.__account,
             self.__container, self.__makeBlobName(buildId, suffix))
 
     def _openDownloadFile(self, buildId, suffix):
-        from azure.common import AzureException, AzureMissingResourceHttpError
-        (tmpFd, tmpName) = mkstemp()
+        client = self.__getClient()
+        from azure.core.exceptions import AzureError, ResourceNotFoundError
         try:
-            os.close(tmpFd)
-            self.__service.get_blob_to_path(self.__container,
-                self.__makeBlobName(buildId, suffix), tmpName)
-            ret = tmpName
-            tmpName = None
-            return AzureDownloader(ret)
-        except AzureMissingResourceHttpError:
+            stream = client.download_blob(self.__makeBlobName(buildId, suffix))
+            stream = AzureStreamReadAdapter(stream) # Make io.RawIOBase compatible
+            stream = io.BufferedReader(stream, 1048576) # 1MiB buffer. Azure read()s are synchronous.
+            ret = AzureDownloader(client, stream)
+            client = None
+            return ret
+        except ResourceNotFoundError:
             raise ArtifactNotFoundError()
-        except AzureException as e:
+        except AzureError as e:
             raise ArtifactDownloadError(str(e))
         finally:
-            if tmpName is not None: os.unlink(tmpName)
+            if client is not None: client.close()
 
     def _openUploadFile(self, buildId, suffix):
-        from azure.common import AzureException
-
+        containerClient = self.__getClient()
+        from azure.core.exceptions import AzureError
         blobName = self.__makeBlobName(buildId, suffix)
+        blobClient = None
         try:
-            if self.__service.exists(self.__container, blobName):
+            blobClient = containerClient.get_blob_client(blobName)
+            if blobClient.exists():
                 raise ArtifactExistsError()
-        except AzureException as e:
+            ret = AzureUploader(containerClient, blobClient)
+            containerClient = blobClient = None
+            return ret
+        except AzureError as e:
             raise ArtifactUploadError(str(e))
-        (tmpFd, tmpName) = mkstemp()
-        os.close(tmpFd)
-        return AzureUploader(self.__service, self.__container, tmpName, blobName)
+        finally:
+            if blobClient is not None: blobClient.close()
+            if containerClient is not None: containerClient.close()
 
 class AzureDownloader:
-    def __init__(self, name):
-        self.name = name
+    def __init__(self, client, stream):
+        self.__client = client
+        self.__stream = stream
     def __enter__(self):
-        return (self.name, None)
+        return (None, self.__stream)
     def __exit__(self, exc_type, exc_value, traceback):
-        os.unlink(self.name)
+        self.__client.close()
         return False
 
 class AzureUploader:
-    def __init__(self, service, container, name, remoteName):
-        self.__service = service
-        self.__container = container
-        self.__name = name
-        self.__remoteName = remoteName
+    def __init__(self, containerClient, blobClient):
+        self.__containerClient = containerClient
+        self.__blobClient = blobClient
 
     def __enter__(self):
-        return (self.__name, None)
+        self.__tmp = TemporaryFile()
+        return (None, self.__tmp)
 
     def __exit__(self, exc_type, exc_value, traceback):
         try:
             if exc_type is None:
                 self.__upload()
         finally:
-            os.unlink(self.__name)
+            self.__tmp.close()
+            self.__blobClient.close()
+            self.__containerClient.close()
         return False
 
     def __upload(self):
-        from azure.common import AzureException, AzureConflictHttpError
+        from azure.core.exceptions import AzureError, ResourceExistsError
         try:
-            self.__service.create_blob_from_path(self.__container,
-                self.__remoteName, self.__name, if_none_match="*")
-        except AzureConflictHttpError:
+            self.__tmp.seek(0, os.SEEK_END)
+            length = self.__tmp.tell()
+            self.__tmp.seek(0)
+            self.__blobClient.upload_blob(self.__tmp, length=length, overwrite=False)
+        except ResourceExistsError:
             raise ArtifactExistsError()
-        except AzureException as e:
+        except AzureError as e:
             raise ArtifactUploadError(str(e))
 
 
 class MultiArchive:
     def __init__(self, archives):
         self.__archives = archives
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/audit.py` & `BobBuildTool-0.23.0rc1/pym/bob/audit.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/builder.py` & `BobBuildTool-0.23.0rc1/pym/bob/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,25 +61,75 @@
     return [ t.result() for t in tasks ]
 
 def hashWorkspace(step):
     # Cache is also used by share module
     return hashDirectory(step.getStoragePath(),
         os.path.join(os.path.dirname(step.getWorkspacePath()), "cache.bin"))
 
+CHECKOUT_STATE_VARIANT_ID = None    # Key in checkout directory state for step variant-id
+CHECKOUT_STATE_BUILD_ONLY = 1       # Key for checkout state of build-only builds
+
+# Keys in checkout getDirectoryState that are not directories
+CHECKOUT_NON_DIR_KEYS = {CHECKOUT_STATE_VARIANT_ID, CHECKOUT_STATE_BUILD_ONLY}
+
 def compareDirectoryState(left, right):
     """Compare two directory states while ignoring the SCM specs.
 
     The SCM specs might change even though the digest stays the same (e.g. the
     URL changes but the commit id stays the same).  This function filters the
     spec to detect real changes.
+
+    It also compares the CHECKOUT_STATE_VARIANT_ID to detect recipe changes. In
+    contrast, the CHECKOUT_STATE_BUILD_ONLY sub-state is ignored as this is
+    only relevant for build-only builds that have their dedicated functions
+    below.
+    """
+    left  = { d : v[0] for d, v in left.items()  if d != CHECKOUT_STATE_BUILD_ONLY }
+    right = { d : v[0] for d, v in right.items() if d != CHECKOUT_STATE_BUILD_ONLY }
+    return left == right
+
+def checkoutsFromState(state):
+    """Return only the tuples related to SCMs from the checkout state."""
+    return [ (k, v) for k, v in state.items() if k not in CHECKOUT_NON_DIR_KEYS ]
+
+def checkoutBuildOnlyState(checkoutStep, inputHashes):
+    """Obtain state for build-only checkout updates.
+
+    The assumption is that we can run updates as long as all local SCMs stayed
+    the same. As this is just for build-only builds, we can assume that
+    dependencies have been setup correctly (direct deps, tools).
+
+    Because of the fixImportScmVariant bug, we include the directory too. This
+    should not have been necessary otherwise. Needs to return a tuple because
+    that's what is expected in the checkout SCM state (will be silently
+    upgraded to a tuple by BobState otherwise).
+    """
+    return ("\n".join("{} {}".format(scm.getDirectory(), scm.asDigestScript())
+                      for scm in checkoutStep.getScmList()
+                      if scm.isLocal()),
+            checkoutStep.getUpdateScriptDigest(),
+            inputHashes)
+
+def checkoutBuildOnlyStateCompatible(left, right):
+    """Returns True if it's safe to run build-only checkout updates.
+
+    Current policy is to just require that local SCMs are compatible. A
+    different step variant-id, changed update script or dependency changes do
+    *not* prohibit an in-place update.
     """
-    left  = { d : v[0] for d, v in left.items()  }
-    right = { d : v[0] for d, v in right.items() }
+    left = left.get(CHECKOUT_STATE_BUILD_ONLY, (None, None, None))[0]
+    right = right.get(CHECKOUT_STATE_BUILD_ONLY, (None, None, None))[0]
     return left == right
 
+def checkoutBuildOnlyStateChanged(left, right):
+    """Returns True if the update script has changed"""
+    left = left.get(CHECKOUT_STATE_BUILD_ONLY, None)
+    right = right.get(CHECKOUT_STATE_BUILD_ONLY, None)
+    return left != right
+
 def dissectPackageInputState(oldInputBuildId):
     """Take a package step input hashes and convert them to a common
     representation.
 
     Excluding the legacy storage, the following formats are persisted:
 
       built: [ BuildId, InputHash1, ...]
@@ -1012,50 +1062,57 @@
 
         checkoutInputHashes = [ BobState().getResultHash(i.getWorkspacePath())
             for i in checkoutStep.getAllDepSteps() if i.isValid() ]
 
         checkoutExecuted = False
         checkoutDigest = checkoutStep.getVariantId()
         checkoutState = checkoutStep.getScmDirectories().copy()
-        checkoutState[None] = (checkoutDigest, None)
+        checkoutState[CHECKOUT_STATE_VARIANT_ID] = (checkoutDigest, None)
+        checkoutState[CHECKOUT_STATE_BUILD_ONLY] = checkoutBuildOnlyState(checkoutStep, checkoutInputHashes)
         if self.__buildOnly and (BobState().getResultHash(prettySrcPath) is not None):
-            inputChanged = checkoutInputHashes != BobState().getInputHashes(prettySrcPath)
+            inputChanged = checkoutBuildOnlyStateChanged(checkoutState, oldCheckoutState)
             rehash = lambda: hashWorkspace(checkoutStep)
-            if not compareDirectoryState(checkoutState, oldCheckoutState):
+            if checkoutStep.mayUpdate(inputChanged, BobState().getResultHash(prettySrcPath), rehash):
+                if checkoutBuildOnlyStateCompatible(checkoutState, oldCheckoutState):
+                    with stepExec(checkoutStep, "UPDATE",
+                                  "{} {}".format(prettySrcPath, overridesString)) as a:
+                        await self._runShell(checkoutStep, "checkout", a, mode=InvocationMode.UPDATE)
+                    newCheckoutState = oldCheckoutState.copy()
+                    newCheckoutState[CHECKOUT_STATE_BUILD_ONLY] = checkoutState[CHECKOUT_STATE_BUILD_ONLY]
+                    BobState().setDirectoryState(prettySrcPath, newCheckoutState)
+                else:
+                    stepMessage(checkoutStep, "UPDATE", "WARNING: recipe changed - cannot update ({})"
+                        .format(prettySrcPath), WARNING)
+            elif not compareDirectoryState(checkoutState, oldCheckoutState):
                 stepMessage(checkoutStep, "CHECKOUT", "WARNING: recipe changed but skipped due to --build-only ({})"
                     .format(prettySrcPath), WARNING)
-            elif checkoutStep.mayUpdate(inputChanged, BobState().getResultHash(prettySrcPath), rehash):
-                with stepExec(checkoutStep, "UPDATE",
-                              "{} {}".format(prettySrcPath, overridesString)) as a:
-                    await self._runShell(checkoutStep, "checkout", a, mode=InvocationMode.UPDATE)
             else:
                 stepMessage(checkoutStep, "CHECKOUT", "skipped due to --build-only ({}) {}".format(prettySrcPath, overridesString),
                     SKIPPED, IMPORTANT)
         else:
             scmMap = { scm.getDirectory() : scm
                        for scm in checkoutStep.getScmList() }
 
             if self.__cleanCheckout:
                 # check state of SCMs and invalidate if the directory is dirty
-                for (scmDir, (scmDigest, scmSpec)) in oldCheckoutState.copy().items():
-                    if scmDir is None: continue
+                for (scmDir, (scmDigest, scmSpec)) in checkoutsFromState(oldCheckoutState):
                     if scmDigest != checkoutState.get(scmDir, (None, None))[0]: continue
                     if not os.path.exists(os.path.join(prettySrcPath, scmDir)): continue
                     if scmMap[scmDir].status(checkoutStep.getWorkspacePath()).dirty:
                         # Invalidate scmDigest to forcibly move it away in the loop below.
                         # Do not use None here to distinguish it from a non-existent directory.
                         oldCheckoutState[scmDir] = (False, scmSpec)
 
             if (self.__force or (not checkoutStep.isDeterministic()) or
                 (BobState().getResultHash(prettySrcPath) is None) or
                 not compareDirectoryState(checkoutState, oldCheckoutState) or
                 (checkoutInputHashes != BobState().getInputHashes(prettySrcPath))):
                 # Switch or move away old or changed source directories
-                for (scmDir, (scmDigest, scmSpec)) in oldCheckoutState.copy().items():
-                    if (scmDir is not None) and (scmDigest != checkoutState.get(scmDir, (None, None))[0]):
+                for (scmDir, (scmDigest, scmSpec)) in checkoutsFromState(oldCheckoutState):
+                    if scmDigest != checkoutState.get(scmDir, (None, None))[0]:
                         scmPath = os.path.normpath(os.path.join(prettySrcPath, scmDir))
                         canSwitch = (scmDir in scmMap) and scmDigest and \
                                      scmSpec is not None and \
                                      scmMap[scmDir].canSwitch(scmSpec) and \
                                      os.path.exists(scmPath)
                         didSwitch = False
                         if canSwitch:
@@ -1083,28 +1140,28 @@
                         del oldCheckoutState[scmDir]
                         BobState().setDirectoryState(prettySrcPath, oldCheckoutState)
 
                 # Check that new checkouts do not collide with old stuff in
                 # workspace. Do it before we store the new SCM state to
                 # check again if the step is rerun.
                 if not checkoutStep.JENKINS:
-                    for scmDir in checkoutState.keys():
-                        if scmDir is None or scmDir == ".": continue
+                    for scmDir in [ k for k,v in checkoutsFromState(checkoutState)]:
+                        if scmDir == ".": continue
                         if scmDir in oldCheckoutState: continue
                         scmPath = os.path.normpath(os.path.join(prettySrcPath, scmDir))
                         if os.path.exists(scmPath):
                             raise BuildError("New SCM checkout '{}' collides with existing file in workspace '{}'!"
                                                 .format(scmDir, prettySrcPath))
 
                 # Store new SCM checkout state. The script state is not stored
                 # so that this step will run again if it fails. OTOH we must
                 # record the SCM directories as some checkouts might already
                 # succeeded before the step ultimately fails.
                 BobState().setDirectoryState(prettySrcPath,
-                    { d:s for (d,s) in checkoutState.items() if d is not None })
+                    { d:s for (d,s) in checkoutState.items() if d != CHECKOUT_STATE_VARIANT_ID })
 
                 # Forge checkout result before we run the step again.
                 # Normally the correct result is set directly after the
                 # checkout finished. But if the step fails and the user
                 # re-runs with "build-only" the dependent steps should
                 # trigger.
                 if BobState().getResultHash(prettySrcPath) is not None:
@@ -1222,18 +1279,19 @@
         oldPackageDigest = BobState().getDirectoryState(prettyPackagePath, False)
         somethingThere = os.path.lexists(prettyPackagePath) # might be a symlink
 
         # Prune if something else was there before
         if somethingThere and packageDigest != oldPackageDigest:
             stepMessage(packageStep, "PRUNE", "{} (recipe changed)".format(prettyPackagePath),
                 WARNING)
-            if os.path.isdir(prettyPackagePath):
-                emptyDirectory(prettyPackagePath)
-            else:
+            if os.path.islink(prettyPackagePath) or os.path.isfile(prettyPackagePath):
+                # Remove symlink or file which was left by a shared package
                 os.unlink(prettyPackagePath)
+            else:
+                emptyDirectory(prettyPackagePath)
             somethingThere = False
 
         # Reset state if we start from scratch
         if not somethingThere:
             BobState().resetWorkspaceState(prettyPackagePath, packageDigest)
 
     def _useSharedPackage(self, packageStep, packageBuildId):
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/archive.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/archive.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/build.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ...archive import getArchiver
 from ...builder import LocalBuilder
 from ...errors import BuildError
 from ...input import RecipeSet
 from ...intermediate import StepIR, PackageIR, RecipeIR, ToolIR, SandboxIR, \
     RecipeSetIR
 from ...share import getShare
-from ...tty import setVerbosity, setTui
+from ...tty import setVerbosity, setTui, Warn
 from ...utils import copyTree, processDefines, EventLoopWrapper
 import argparse
 import datetime
 import re
 import os
 import subprocess
 import stat
@@ -376,19 +376,30 @@
                 + str(stats.checkouts)
                     + " checkout" + ("s" if (stats.checkouts != 1) else "")
                     + " (" + str(activeOverrides) + (" overrides" if (activeOverrides != 1) else " override") + " active), "
                 + str(stats.packagesBuilt)
                     + " package" + ("s" if (stats.packagesBuilt != 1) else "") + " built, "
                 + str(stats.packagesDownloaded) + " downloaded.")
 
-        # copy build result if requested
+        # Copy build result if requested. It's ok to overwrite files that are
+        # already at the destination. Warn if built packages overwrite
+        # themselves, though.
         ok = True
         if args.destination:
+            allFiles = set()
+            collisions = set()
             for result in results:
-                ok = copyTree(result, args.destination) and ok
+                nextFiles = set()
+                ok = copyTree(result, args.destination, nextFiles) and ok
+                collisions |= allFiles & nextFiles
+                allFiles |= nextFiles
+            if collisions:
+                shownCollisions = ", ".join(sorted(collisions)[:3])
+                if len(collisions) > 3: shownCollisions = shownCollisions + ", ..."
+                Warn("duplicate files at distination overwritten: " + shownCollisions).warn()
         if not ok:
             raise BuildError("Could not copy everything to destination. Your aggregated result is probably incomplete.")
     else:
         print("Your query matched no packages. Naptime!")
 
 def doBuild(argv, bobRoot):
     parser = argparse.ArgumentParser(prog="bob build", description='Build packages in release mode.')
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/clean.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bob build tool
 # Copyright (C) 2016-2018  TechniSat Digital GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from ...builder import LocalBuilder
+from ...builder import LocalBuilder, checkoutsFromState
 from ...input import RecipeSet
 from ...scm import getScm, ScmTaint, ScmStatus
 from ...share import getShare
 from ...state import BobState
 from ...tty import colorize, ERROR, WARNING, EXECUTED, DEFAULT, Warn
 from ...utils import removePath, processDefines
 import argparse
@@ -51,15 +51,14 @@
         for d in package.getDirectDepSteps():
             walk(d.getPackage())
 
     walk(rootPackage)
     return paths
 
 def checkSCM(workspace, scmDir, scmSpec, verbose):
-    if scmDir is None: return True
     if scmSpec is not None:
         status = getScm(scmSpec).status(workspace)
     else:
         status = UNKNOWN
 
     if verbose:
         flags = str(status)
@@ -74,15 +73,15 @@
         print(colorize("STATUS {0: <4} {1}".format(flags, workspace), color))
 
     return status.expendable
 
 def checkRegularSource(workspace, verbose):
     ret = True
     state = BobState().getDirectoryState(workspace, True)
-    for (scmDir, (scmDigest, scmSpec)) in state.items():
+    for (scmDir, (scmDigest, scmSpec)) in checkoutsFromState(state):
         if not checkSCM(workspace, scmDir, scmSpec, verbose):
             ret = False
 
     return ret
 
 def checkAtticSource(workspace, verbose):
     scmSpec = BobState().getAtticDirectoryState(workspace)
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/project.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,22 +103,25 @@
         # expand because we cannot control the argument order in the generator
         args.jobs = os.cpu_count()
     if args.jobs is not None:
         if args.jobs <= 0:
             parser.error("--jobs argument must be greater than zero!")
         extra.extend(['-j', str(args.jobs)])
 
-    package = packages.walkPackagePath(args.package)
+    if generator.get('query'):
+        package = packages.queryPackagePath(args.package)
+    else:
+        package = packages.walkPackagePath(args.package)
+        print(">>", colorize("/".join(package.getStack()), "32;1"))
 
     # execute a bob dev with the extra arguments to build all executables.
     # This makes it possible for the plugin to collect them and generate some runTargets.
     if args.execute_prebuild:
         devArgs = extra.copy()
         if args.resume: devArgs.append('--resume')
         if args.execute_buildonly: devArgs.append('-b')
         devArgs.append(args.package)
         doDevelop(devArgs, bobRoot)
 
-    print(">>", colorize("/".join(package.getStack()), "32;1"))
     print(colorize("   PROJECT   {} ({})".format(args.package, args.projectGenerator), "32"))
-    generator(package, args.args, extra, bobRoot)
+    generator.get('func')(package, args.args, extra, bobRoot)
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/query.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/query.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/state.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/state.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/build/status.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/build/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bob build tool
 # Copyright (C) 2016-2019  TechniSat Digital GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from ...builder import LocalBuilder
+from ...builder import LocalBuilder, checkoutsFromState
 from ...input import RecipeSet
 from ...scm import getScm, ScmTaint, ScmStatus
 from ...state import BobState
 from ...tty import colorize, ERROR, WARNING, EXECUTED, DEFAULT, SKIPPED, \
     IMPORTANT, NORMAL, INFO, DEBUG, TRACE, HEADLINE
 from ...utils import joinLines, processDefines
 from textwrap import indent
@@ -108,16 +108,15 @@
         checkoutState = checkoutStep.getScmDirectories()
         scms = { scm.getDirectory() : scm for scm in checkoutStep.getScmList() }
         result = {}
 
         # First scan old checkout state. This is what the user is most
         # interested in. The recipe might have changed compared to the
         # persisted state!
-        for (scmDir, (scmDigest, scmSpec)) in oldCheckoutState.items():
-            if scmDir is None: continue # checkoutScript state -> ignored
+        for (scmDir, (scmDigest, scmSpec)) in checkoutsFromState(oldCheckoutState):
             if not os.path.exists(os.path.join(workspace, scmDir)): continue
 
             if scmDigest == checkoutState.get(scmDir, (None, None))[0]:
                 # The digest still matches -> use recipe values
                 status = scms[scmDir].status(workspace)
             elif scmSpec is not None:
                 # New project that kept scm spec -> compare with that and mark
@@ -204,18 +203,18 @@
             if not isinstance(dirState, dict):
                 continue
 
             if not os.path.isdir(workspace):
                 BobState().delDirectoryState(workspace)
                 continue
 
-            # Upgrade from old format without scmSpec. Drop None dir.
+            # Upgrade from old format without scmSpec.
             dirState = sorted(
                 (dir, state) if isinstance(state, tuple) else (dir, (state, None))
-                for dir,state in dirState.items() if dir is not None)
+                for dir,state in checkoutsFromState(dirState))
             for (scmDir, (scmDigest, scmSpec)) in dirState:
                 scmDir = os.path.join(workspace, scmDir)
                 if scmSpec is not None:
                     status = getScm(scmSpec).status(workspace)
                 else:
                     status = UNKNOWN
                 pp.show(status, scmDir)
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/graph.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/graph.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/help.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/help.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/invoke.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/invoke.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/exec.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/exec.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/intermediate.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/intermediate.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/jenkins/jenkins.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/jenkins/jenkins.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/misc.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/cmds/show.py` & `BobBuildTool-0.23.0rc1/pym/bob/cmds/show.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/develop/make.py` & `BobBuildTool-0.23.0rc1/pym/bob/develop/make.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/develop/version.py` & `BobBuildTool-0.23.0rc1/pym/bob/develop/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             import sys
             print("Warning: inferred version of Bob does not match schema:",
                 version, file=sys.stderr)
             version = ""
 
     if not version:
         # Last fallback. See PEP 440 and adjust accordingly.
-        version = "0.21+unknown"
+        version = "0.23.dev999+unknown"
 
     return version
 
 try:
     BOB_VERSION = getVersion()
 except KeyboardInterrupt:
     sys.exit(1)
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/errors.py` & `BobBuildTool-0.23.0rc1/pym/bob/errors.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/generators/EclipseCdtGenerator.py` & `BobBuildTool-0.23.0rc1/pym/bob/generators/EclipseCdtGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import re
 import shutil
 import stat
 import uuid
 from os.path import expanduser
 from os.path import join
 from bob.utils import summonMagic, removePath
+from bob.errors import ParseError
 from collections import OrderedDict
 from shlex import quote
 
 # scan package recursivelely with its dependencies and build a list of checkout dirs
 def getCheckOutDirs(package, dirs):
     def collect(package, dirs, steps, processed):
         if package._getId() in processed:
@@ -229,15 +230,15 @@
                     excludePackages.append(name)
         includeDirs = []
         # find additional include dirs
         for i in args.additional_includes:
             if os.path.exists(i):
                 includeDirs.append(i)
     except re.error as e:
-        raise ParseError("Invalid regular expression '{}': {}".format(e.pattern), e)
+        raise ParseError("Invalid regular expression '{}': {}".format(e.pattern, e))
 
     with open(os.path.join(destination, ".cproject"), 'w') as cProjectFile:
         cProjectFile.write(cProjectHeader)
         addCConfig(cProjectFile, excludePackages, includeDirs, "Bob dev", id, "", buildMeFile)
         addCConfig(cProjectFile, excludePackages, includeDirs, "Bob dev (force)", id + "." + getId(), "-f", buildMeFile)
         addCConfig(cProjectFile, excludePackages, includeDirs, "Bob dev (no checkout)",id + "." + getId(), "-b", buildMeFile)
         addCConfig(cProjectFile, excludePackages, includeDirs, "Bob dev (no deps)",id + "." + getId(), "-n", buildMeFile)
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/generators/QtCreatorGenerator.py` & `BobBuildTool-0.23.0rc1/pym/bob/generators/QtCreatorGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import shutil
 import stat
 import xml.etree.ElementTree
 import shutil
 from os.path import expanduser
 from os.path import join
 from bob.utils import removePath, isWindows
-from bob.errors import BuildError
+from bob.errors import BuildError, ParseError
 from bob.utils import summonMagic, hashFile
 from collections import OrderedDict, namedtuple
 from bob.tty import colorize, WARNING
 from shlex import quote
 
 # helper to get linux or windows (MSYS2 support) cwd
 pwd = None
@@ -223,15 +223,15 @@
 
         # use default kit "Desktop" if no kit is given
         if args.kit is None:
             _kit = re.compile(r".*Desktop.*")
         else:
             _kit = re.compile(r""+args.kit)
     except re.error as e:
-        raise ParseError("Invalid regular expression '{}': {}".format(e.pattern), e)
+        raise ParseError("Invalid regular expression '{}': {}".format(e.pattern, e))
 
     getCheckOutDirs(package, excludes, dirs)
     if not projectName:
         # use package name for project name
         projectName = package.getName().replace('::', '__')
     if not destination:
         # use package name for project directory
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/generators/VisualStudio.py` & `BobBuildTool-0.23.0rc1/pym/bob/generators/VisualStudio.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/generators/VisualStudioCode.py` & `BobBuildTool-0.23.0rc1/pym/bob/generators/VisualStudioCode.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/generators/common.py` & `BobBuildTool-0.23.0rc1/pym/bob/generators/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         class PackageInfo:
             def __init__(self, recipeName, packageName):
                 self.recipeName = recipeName
                 self.packageName = packageName
                 self.checkout = False
                 self.dependencies = set()
 
-        checkouts = { False : CheckoutInfo(None, None) }
+        checkouts = { False : CheckoutInfo(BaseScanner(), None) }
         packages = {}
 
         def collect(package, rootPackage=True):
             # only once per package
             packageVid = package.getPackageStep().getVariantId()
             if packageVid in packages: return
             packages[packageVid] = packageInfo = PackageInfo(package.getRecipe().getName(), package.getName())
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/input.py` & `BobBuildTool-0.23.0rc1/pym/bob/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .errors import ParseError, BobError
 from .languages import getLanguage, ScriptLanguage, BashLanguage, PwshLanguage
 from .pathspec import PackageSet
 from .scm import CvsScm, GitScm, ImportScm, SvnScm, UrlScm, ScmOverride, \
     auditFromDir, getScm, SYNTHETIC_SCM_PROPS
 from .state import BobState
 from .stringparser import checkGlobList, Env, DEFAULT_STRING_FUNS, IfExpression
-from .tty import InfoOnce, Warn, WarnOnce, setColorMode
+from .tty import InfoOnce, Warn, WarnOnce, setColorMode, setParallelTUIThreshold
 from .utils import asHexStr, joinScripts, compareVersion, binStat, \
     updateDicRecursive, hashString, getPlatformTag, getPlatformString, \
     replacePath
 from itertools import chain
 from os.path import expanduser
 from string import Template
 from textwrap import dedent
@@ -1845,14 +1845,48 @@
     def useResultOnce(self):
         if self.usedResult:
             return False
         else:
             self.usedResult = True
             return True
 
+
+class VerbatimProvideDepsResolver:
+    def __init__(self, pattern):
+        self.pattern = pattern
+
+    def resolve(self, env, resolvedDeps):
+        pattern = self.pattern
+        return set(d for d in resolvedDeps if d == pattern)
+
+class GlobProvideDepsResolver:
+    def __init__(self, pattern):
+        self.pattern = pattern
+
+    def resolve(self, env, resolvedDeps):
+        pattern = self.pattern
+        return set(d for d in resolvedDeps if fnmatch.fnmatchcase(d, pattern))
+
+class SubstituteProvideDepsResolver:
+    def __init__(self, pattern):
+        self.pattern = pattern
+
+    def resolve(self, env, resolvedDeps):
+        pattern = self.pattern
+        pattern = env.substitute(pattern, "providedDeps::"+pattern)
+        return set(d for d in resolvedDeps if fnmatch.fnmatchcase(d, pattern))
+
+def getProvideDepsResolver(pattern):
+    if any((c in pattern) for c in '\\\"\'$'):
+        return SubstituteProvideDepsResolver(pattern)
+    elif any((c in pattern) for c in '*?['):
+        return GlobProvideDepsResolver(pattern)
+    else:
+        return VerbatimProvideDepsResolver(pattern)
+
 class Recipe(object):
     """Representation of a single recipe
 
     Multiple instaces of this class will be created if the recipe used the
     ``multiPackage`` keyword.  In this case the getName() method will return
     the name of the original recipe but the getPackageName() method will return
     it with some addition suffix. Without a ``multiPackage`` keyword there will
@@ -2216,23 +2250,16 @@
         if self.__relocatable is None:
             self.__relocatable = self.__recipeSet.getPolicy('allRelocatable') \
                 or not self.__provideTools
 
         if self.__jobServer is None:
             self.__jobServer = False
 
-        # check provided dependencies
-        availDeps = [ d.recipe for d in self.__deps ]
-        providedDeps = set()
-        for pattern in self.__provideDeps:
-            l = set(d for d in availDeps if fnmatch.fnmatchcase(d, pattern))
-            if not l:
-                raise ParseError("Unknown dependency '{}' in provideDeps".format(pattern))
-            providedDeps |= l
-        self.__provideDeps = providedDeps
+        # Optimize provideDeps
+        self.__provideDeps = [ getProvideDepsResolver(d) for d in self.__provideDeps ]
 
         # Evaluate root property
         if isinstance(self.__root, str) or isinstance(self.__root, IfExpression):
             self.__root = rootEnv.evaluate(self.__root, "root")
 
     def getRecipeSet(self):
         """Get the :class:`RecipeSet` to which the recipe belongs"""
@@ -2342,51 +2369,56 @@
         for s in states.values(): s.onEnter(env, self.__properties)
 
         # traverse dependencies
         subTreePackages = set()
         directPackages = []
         indirectPackages = []
         provideDeps = UniquePackageList(stack, self.__raiseIncompatibleProvided)
+        maybeProvideDeps = []
         checkoutDeps = []
         results = []
         depEnv = env.derive()
         depTools = tools.derive()
         depSandbox = sandbox
         depStates = { n : s.copy() for (n,s) in states.items() }
         depDiffSandbox = diffSandbox
         depDiffTools = diffTools.copy()
         thisDeps = {}
+        resolvedDeps = []
 
         for dep in self.__deps:
             env.setFunArgs({ "recipe" : self, "sandbox" : bool(sandbox) and sandboxEnabled,
                 "__tools" : tools })
 
-            if dep.condition and not all(env.evaluate(cond, "dependency "+dep.recipe)
+            recipe = env.substitute(dep.recipe, "dependency::"+dep.recipe)
+            resolvedDeps.append(recipe)
+
+            if dep.condition and not all(env.evaluate(cond, "dependency "+recipe)
                                                       for cond in dep.condition): continue
 
             if dep.toolOverride:
                 try:
                     thisDepTools = depTools.derive({
                         k : depTools[v] for k,v in dep.toolOverride.items() })
                 except KeyError as e:
                     raise ParseError("Cannot remap unkown tool '{}' for dependency '{}'!"
-                        .format(e.args[0], dep.recipe))
+                        .format(e.args[0], recipe))
                 thisDepDiffTools = depDiffTools.copy()
                 thisDepDiffTools.update({
                     k : depDiffTools.get(v, v)
                     for k, v in dep.toolOverride.items() })
             else:
                 thisDepTools = depTools
                 thisDepDiffTools = depDiffTools
 
             thisDepEnv = depEnv.derive(
-                { key : env.substitute(value, "depends["+dep.recipe+"].environment["+key+"]")
+                { key : env.substitute(value, "depends["+recipe+"].environment["+key+"]")
                   for key, value in dep.envOverride.items() })
 
-            r = self.__recipeSet.getRecipe(dep.recipe)
+            r = self.__recipeSet.getRecipe(recipe)
             try:
                 if r.__packageName in stack:
                     raise ParseError("Recipes are cyclic (1st package in cylce)")
                 depStack = stack + [r.__packageName]
                 p, s = r.prepare(thisDepEnv, sandboxEnabled, depStates,
                                  depSandbox, thisDepTools, depStack)
                 subTreePackages.add(p.getName())
@@ -2396,24 +2428,24 @@
             except ParseError as e:
                 e.pushFrame(r.getPackageName())
                 raise e
 
             # A dependency should be named only once. Hence we can
             # optimistically create the DepTracker object. If the dependency is
             # named more than one we make sure that it is the same variant.
-            depTrack = thisDeps.setdefault(dep.recipe, DepTracker(depRef))
+            depTrack = thisDeps.setdefault(recipe, DepTracker(depRef))
             if depTrack.prime():
                 directPackages.append(depRef)
             elif depCoreStep.variantId != depTrack.item.refGetDestination().variantId:
                 self.__raiseIncompatibleLocal(depCoreStep)
             elif self.__recipeSet.getPolicy('uniqueDependency'):
                 raise ParseError("Duplicate dependency '{}'. Each dependency must only be named once!"
-                                    .format(dep.recipe))
+                                    .format(recipe))
             else:
-                warnDepends.show("{} -> {}".format(self.__packageName, dep.recipe))
+                warnDepends.show("{} -> {}".format(self.__packageName, recipe))
 
             # Remember dependency diffs before changing them
             origDepDiffTools = thisDepDiffTools
             origDepDiffSandbox = depDiffSandbox
 
             # pick up various results of package
             for (n, s) in states.items():
@@ -2445,18 +2477,30 @@
                     origDepDiffSandbox)
                 if dep.provideGlobal:
                     depSandbox = sandbox
                     depDiffSandbox = diffSandbox
                 if sandboxEnabled:
                     env.update(sandbox.environment)
                     if dep.provideGlobal: depEnv.update(sandbox.environment)
-            if dep.recipe in self.__provideDeps:
+
+            maybeProvideDeps.append((recipe, depRef, p.getName(), origDepDiffTools, origDepDiffSandbox))
+
+        # check provided dependencies
+        providedDeps = set()
+        for pattern in self.__provideDeps:
+            l = pattern.resolve(env, resolvedDeps)
+            if not l:
+                raise ParseError("Unknown dependency '{}' in provideDeps".format(pattern.pattern))
+            providedDeps |= l
+
+        for (recipe, depRef, name, origDepDiffTools, origDepDiffSandbox) in maybeProvideDeps:
+            if recipe in providedDeps:
                 provideDeps.append(depRef)
-                provideDeps.extend(CoreRef(d, [p.getName()], origDepDiffTools, origDepDiffSandbox)
-                    for d in depCoreStep.providedDeps)
+                provideDeps.extend([CoreRef(d, [name], origDepDiffTools, origDepDiffSandbox)
+                    for d in depRef.refGetDestination().providedDeps])
 
         # Filter indirect packages and add to result list if necessary. Most
         # likely there are many duplicates that are dropped.
         tmp = indirectPackages
         indirectPackages = []
         for depRef in tmp:
             depCoreStep = depRef.refGetDestination()
@@ -2888,14 +2932,15 @@
 
     It holds global information about the project.
     """
 
     BUILD_DEV_SCHEMA = schema.Schema(
         {
             schema.Optional('always_checkout') : [str],
+            schema.Optional('attic') : bool,
             schema.Optional('audit') : bool,
             schema.Optional('build_mode') : schema.Or("build-only","normal", "checkout-only"),
             schema.Optional('clean') : bool,
             schema.Optional('clean_checkout') : bool,
             schema.Optional('destination') : str,
             schema.Optional('download') : schema.Or("yes", "no", "deps",
                 "forced", "forced-deps", "forced-fallback",
@@ -2936,14 +2981,15 @@
                 schema.Optional('secureSSL') : bool,
                 schema.Optional('sandboxFingerprints') : bool,
                 schema.Optional('fingerprintVars') : bool,
                 schema.Optional('noUndefinedTools') : bool,
                 schema.Optional('scmIgnoreUser') : bool,
                 schema.Optional('pruneImportScm') : bool,
                 schema.Optional('gitCommitOnBranch') : bool,
+                schema.Optional('fixImportScmVariant') : bool,
             },
             error="Invalid policy specified! Maybe your Bob is too old?"
         ),
         schema.Optional('layers') : [str],
         schema.Optional('scriptLanguage',
                         default=ScriptLanguage.BASH) : schema.And(schema.Or("bash", "PowerShell"),
                                                                   schema.Use(ScriptLanguage)),
@@ -3063,14 +3109,19 @@
                     help="See http://bob-build-tool.readthedocs.io/en/latest/manual/policies.html#pruneimportscm for more information.")
             ),
             'gitCommitOnBranch' : (
                 "0.21.0.dev5",
                 InfoOnce("gitCommitOnBranch policy not set. Will not check if commit / tag is on configured branch.",
                     help="See http://bob-build-tool.readthedocs.io/en/latest/manual/policies.html#gitcommitonbranch for more information.")
             ),
+            'fixImportScmVariant' : (
+                "0.22.1.dev34",
+                InfoOnce("fixImportScmVariant policy not set. Recipe variant calculation w/ import SCM is boguous.",
+                    help="See http://bob-build-tool.readthedocs.io/en/latest/manual/policies.html#fiximportscmvariant for more information.")
+            ),
         }
         self.__buildHooks = {}
         self.__sandboxOpts = {}
         self.__scmDefaults = {}
         def updateArchive(x): self.__archive = x
 
         def updateWhiteList(x):
@@ -3135,15 +3186,15 @@
                 lambda x: updateDicRecursive(self.__scmDefaults, x)
             ),
             "scmOverrides" : BuiltinSetting(
                 schema.Schema([{
                     schema.Optional('if') : schema.Or(str, IfExpression),
                     schema.Optional('match') : schema.Schema({ str: object }),
                     schema.Optional('del') : [str],
-                    schema.Optional('set') : object,
+                    schema.Optional('set') : schema.Schema({ str: object }),
                     schema.Optional('replace') : schema.Schema({
                         str : schema.Schema({
                             'pattern' : str,
                             'replacement' : str
                         })
                     })
                 }]),
@@ -3157,14 +3208,15 @@
                     schema.Optional('autoClean') : bool,
                 }),
                 lambda x: updateDicRecursive(self.__shareConfig, x),
             ),
             "ui" : BuiltinSetting(
                 schema.Schema({
                     schema.Optional('color') : schema.Or('never', 'always', 'auto'),
+                    schema.Optional('parallelTUIThreshold') : int,
                     schema.Optional('queryMode') : schema.Or('nullset', 'nullglob', 'nullfail'),
                 }),
                 lambda x: updateDicRecursive(self.__uiConfig, x)
             ),
             "whitelist" : BuiltinSetting(
                 schema.Schema([ schema.Regex(r'^[^=]*$') ]),
                 updateWhiteList
@@ -3237,14 +3289,18 @@
         if projectGenerators:
             if compareVersion(apiVersion, "0.16.1.dev33") < 0:
                 # cut off extra argument for old generators
                 projectGenerators = {
                     name : lambda package, args, extra, bobRoot: generator(package, args, extra)
                     for name, generator in projectGenerators.items()
                 }
+            projectGenerators = {
+                name : generator if isinstance(generator, dict) else {'func' :  generator, 'query' : False }
+                for name, generator in projectGenerators.items()
+            }
             self.__projectGenerators.update(projectGenerators)
 
         properties = manifest.get('properties', {})
         if not isinstance(properties, dict):
             raise ParseError("Plugin '"+fileName+"': 'properties' has wrong type!")
         if properties:
             self.__pluginPropDeps += pluginStat
@@ -3534,14 +3590,15 @@
         if layer and not self.getPolicy("relativeIncludes"):
             raise ParseError("Layers require the relativeIncludes policy to be set to the new behaviour!")
         self.__parseUserConfig(os.path.join(rootDir, "default.yaml"))
 
         # color mode provided in cmd line takes precedence
         # (if no color mode provided by user, default one will be used)
         setColorMode(self._colorModeConfig or self.__uiConfig.get('color', 'auto'))
+        setParallelTUIThreshold(self.__uiConfig.get('parallelTUIThreshold', 16))
 
         # finally parse recipes
         classesDir = os.path.join(rootDir, 'classes')
         for root, dirnames, filenames in os.walk(classesDir):
             for path in fnmatch.filter(filenames, "[!.]*.yaml"):
                 try:
                     [r] = Recipe.loadFromFile(self, layer, classesDir,
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/intermediate.py` & `BobBuildTool-0.23.0rc1/pym/bob/intermediate.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         return { d : (bytes.fromhex(h), p) for (d, (h, p)) in self.__data['scmDirectories'].items() }
 
     def mayUpdate(self, inputChanged, oldHash, rehash):
         if any((s.isLocal() and not s.isDeterministic()) for s in self.getScmList()):
             return True
         if not self.getUpdateScript():
             return False
-        if not self.isUpdateDeterministic():
+        if not self.isUpdateDeterministic() or inputChanged:
             return True
         return rehash() != oldHash
 
     def _getSandboxVariantId(self):
         return bytes.fromhex(self.__data['sandboxVariantId'])
 
     async def getDigestCoro(self, calculate, forceSandbox=False, hasher=DigestHasher,
@@ -385,14 +385,29 @@
         h.update(self._getSandboxVariantId())
         for s in self.getScmList():
             liveBId = s.calcLiveBuildId(workspacePath)
             if liveBId is None: return None
             h.update(liveBId)
         return h.digest()
 
+    def getUpdateScriptDigest(self):
+        """Return a digest that tracks relevant changes to the update script behaviour"""
+        h = hashlib.sha1()
+        script = self.getUpdateScript()
+        if script:
+            h.update(struct.pack("<I", len(script)))
+            h.update(script.encode("utf8"))
+        else:
+            h.update(b'\x00\x00\x00\x00')
+        h.update(struct.pack("<I", len(self.__data['digestEnv'])))
+        for (key, val) in sorted(self.__data['digestEnv'].items()):
+            h.update(struct.pack("<II", len(key), len(val)))
+            h.update((key+val).encode('utf8'))
+        return h.digest()
+
 
 class PackageIR(AbstractIR):
 
     @classmethod
     def fromPackage(cls, package, graph, partial=False):
         self = cls()
         self.__data = {}
@@ -545,14 +560,15 @@
             'allRelocatable' : recipeSet.getPolicy('allRelocatable'),
             'pruneImportScm' : recipeSet.getPolicy('pruneImportScm'),
             'scmIgnoreUser' : recipeSet.getPolicy('scmIgnoreUser'),
             'secureSSL' : recipeSet.getPolicy('secureSSL'),
             'tidyUrlScm' : recipeSet.getPolicy('tidyUrlScm'),
             'sandboxFingerprints' : recipeSet.getPolicy('sandboxFingerprints'),
             'gitCommitOnBranch' : recipeSet.getPolicy('gitCommitOnBranch'),
+            'fixImportScmVariant' : recipeSet.getPolicy('fixImportScmVariant'),
         }
         self.__data['archiveSpec'] = recipeSet.archiveSpec()
         self.__data['envWhiteList'] = sorted(recipeSet.envWhiteList())
         self.__data['projectRoot'] = recipeSet.getProjectRoot()
         return self
 
     @classmethod
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/invoker.py` & `BobBuildTool-0.23.0rc1/pym/bob/invoker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .errors import BuildError
 from .input import CheckoutAssert
 from .scm import getScm
 from .stringparser import Env
 from .tty import Unbuffered
 from .utils import removePath, emptyDirectory, isWindows
 from enum import Enum
-from pipes import quote
+from shlex import quote
 import asyncio
 import concurrent.futures
 import datetime
 import io
 import locale
 import os
 import re
@@ -505,22 +505,34 @@
         return ret
 
     async def runCommand(self, args, cwd=None, **kwargs):
         cwd = os.path.join(self.__cwd, cwd) if cwd else self.__cwd
         ret = await self.__runCommand(args, cwd, **kwargs)
         return ret
 
-    async def callCommand(self, args, cwd=None, **kwargs):
+    async def callCommand(self, args, cwd=None, retries=0, success=0, **kwargs):
         cwd = os.path.join(self.__cwd, cwd) if cwd else self.__cwd
-        ret = await self.__runCommand(args, cwd, **kwargs)
+        while True:
+            ret = await self.__runCommand(args, cwd, **kwargs)
+            if (ret == success) or (retries == 0):
+                break
+            await asyncio.sleep(3)
+            retries -= 1
         return ret.returncode
 
-    async def checkCommand(self, args, cwd=None, **kwargs):
+    async def checkCommand(self, args, cwd=None, retries=0, **kwargs):
         cwd = os.path.join(self.__cwd, cwd) if cwd else self.__cwd
-        await self.__runCommand(args, cwd, check=True, **kwargs)
+        while retries != 0:
+            ret = await self.__runCommand(args, cwd, **kwargs)
+            if ret.returncode == 0:
+                return
+            await asyncio.sleep(3)
+            retries -= 1
+        if retries == 0:
+            await self.__runCommand(args, cwd, check=True, **kwargs)
 
     async def checkOutputCommand(self, args, cwd=None, **kwargs):
         cwd = os.path.join(self.__cwd, cwd) if cwd else self.__cwd
         ret = await self.__runCommand(args, cwd, stdout=True, check=True, **kwargs)
         return ret.stdout.rstrip()
 
     def __print(self, *args, file=DEVNULL, **kwargs):
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/languages.py` & `BobBuildTool-0.23.0rc1/pym/bob/languages.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/pathspec.py` & `BobBuildTool-0.23.0rc1/pym/bob/pathspec.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/__init__.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     if scm == "git":
         return GitScm(spec, overrides, recipeSet and recipeSet.getPolicy('secureSSL'),
             recipeSet and recipeSet.getPolicy('scmIgnoreUser'),
             recipeSet and recipeSet.getPolicy('gitCommitOnBranch'))
     elif scm == "import":
         return ImportScm(spec, overrides,
             recipeSet and recipeSet.getPolicy('pruneImportScm'),
+            recipeSet and recipeSet.getPolicy('fixImportScmVariant'),
             recipeSet and recipeSet.getProjectRoot())
     elif scm == "svn":
         return SvnScm(spec, overrides)
     elif scm == "cvs":
         return CvsScm(spec, overrides)
     elif scm == "url":
         return UrlScm(spec, overrides, recipeSet and recipeSet.getPolicy('tidyUrlScm'),
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/cvs.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/cvs.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/git.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         schema.Optional('references') :
             schema.Schema([schema.Or(str, {
                 schema.Optional('url') : str,
                 'repo'    : str,
                 schema.Optional('optional') : bool,
             })]),
         schema.Optional('dissociate') : bool,
+        schema.Optional('retries') : schema.And(int, lambda n: n >= 0, error="Invalid retries attribute"),
     }
 
     __SCHEMA = {
         'scm' : 'git',
         'url' : str,
         schema.Optional('if') : schema.Or(str, IfExpression),
         schema.Optional('tag') : str,
@@ -109,14 +110,15 @@
         self.__recurseSubmodules = spec.get('recurseSubmodules', False)
         self.__shallowSubmodules = spec.get('shallowSubmodules', True)
         self.__stripUser = stripUser
         self.__references = spec.get('references')
         self.__dissociate = spec.get('dissociate', False)
         self.__resolvedReferences = []
         self.__useBranchAndCommit = spec.get('useBranchAndCommit', useBranchAndCommit)
+        self.__retries = spec.get('retries', 0)
 
         def __resolveReferences(self, alt):
             # if the reference is a string it's used as optional reference
             if isinstance(alt, str):
                 return (alt, True)
             else:
                 try:
@@ -140,14 +142,15 @@
             'tag' : self.__tag,
             'commit' : self.__commit,
             'dir' : self.__dir,
             'rev' : ( self.__commit if self.__commit else
                 (("refs/tags/" + self.__tag) if self.__tag else
                     ("refs/heads/" + self.__branch))
             ),
+            'retries' : self.__retries,
             'sslVerify' : self.__sslVerify,
             'singleBranch' : self.__singleBranch,
             'shallow' : self.__shallow,
             'submodules' : self.__submodules,
             'recurseSubmodules' : self.__recurseSubmodules,
             'shallowSubmodules' : self.__shallowSubmodules,
             'references' : self.__references,
@@ -248,15 +251,15 @@
             "-q", "HEAD"], stdout=False, cwd=self.__dir)) == 0
         if headValid and not switch:
             return
 
         # There is no point in doing the extra dance of fetching commits
         # explicitly like in __checkoutTag on shallow clones. We must make sure
         # that the commit is on the selected branch and need the full history!
-        await invoker.checkCommand(fetchCmd, cwd=self.__dir)
+        await invoker.checkCommand(fetchCmd, retries=self.__retries, cwd=self.__dir)
 
         # Verify that commit/tag is on requested branch
         commit = self.__commit if self.__commit else "tags/"+self.__tag
         if await invoker.callCommand(["git", "merge-base", "--is-ancestor",
                                      commit, "remotes/origin/"+self.__branch],
                                      cwd=self.__dir):
             invoker.fail("Branch '{}' does not contain '{}'".format(self.__branch, commit))
@@ -290,38 +293,38 @@
             await self.__updateSubmodulesPost(invoker, preUpdate)
 
     async def __checkoutTag(self, invoker, fetchCmd, switch):
         # checkout only if HEAD is invalid
         head = await invoker.callCommand(["git", "rev-parse", "--verify", "-q", "HEAD"],
             stdout=False, cwd=self.__dir)
         if head or switch:
-            await invoker.checkCommand(fetchCmd, cwd=self.__dir)
+            await invoker.checkCommand(fetchCmd, retries=self.__retries, cwd=self.__dir)
             if self.__commit and (self.__shallow is not None):
                 # Shallow clones might not fetch the requested commit if the
                 # depth is too small. The problem is that we cannot blindly
                 # always request the commit explicitly because this is rejected
                 # by git-upload-pack by default. Instead check here that we got
                 # the commit and only if this is not the case we fetch a 2nd
                 # time with the explicit commit.
                 haveCommit = await invoker.callCommand(["git", "cat-file", "-e",
                     self.__commit], cwd=self.__dir) == 0
                 if not haveCommit:
                     ok = await invoker.callCommand(fetchCmd + [self.__commit],
-                        cwd=self.__dir)
+                        retries = self.__retries, cwd=self.__dir)
                     if ok != 0:
                         invoker.fail("Plain git-fetch in", self.__dir,
                             "did not download the requested commit and the explicit fetch failed!",
                             returncode=ok)
             await invoker.checkCommand(["git", "checkout", "-q", "--no-recurse-submodules",
                 self.__commit if self.__commit else "tags/"+self.__tag], cwd=self.__dir)
             # FIXME: will not be called again if interrupted!
             await self.__checkoutSubmodules(invoker)
 
     async def __checkoutBranch(self, invoker, fetchCmd, switch):
-        await invoker.checkCommand(fetchCmd, cwd=self.__dir)
+        await invoker.checkCommand(fetchCmd, retries=self.__retries, cwd=self.__dir)
         if await invoker.callCommand(["git", "rev-parse", "--verify", "-q", "HEAD"],
                        stdout=False, cwd=self.__dir):
             # checkout only if HEAD is invalid
             await invoker.checkCommand(["git", "checkout", "--no-recurse-submodules", "-b", self.__branch,
                 "remotes/origin/"+self.__branch], cwd=self.__dir)
             await self.__checkoutSubmodules(invoker)
         elif switch:
@@ -471,15 +474,16 @@
                 await self.__updateSubmodulesPost(invoker, subMods[p],
                                                   os.path.join(base, p))
 
     def canSwitch(self, oldSpec):
         diff = self._diffSpec(oldSpec)
 
         # Filter irrelevant properties
-        diff -= {"sslVerify", 'singleBranch', 'shallow', 'shallowSubmodules'}
+        diff -= {"sslVerify", 'singleBranch', 'shallow',
+                'shallowSubmodules', "useBranchAndCommit"}
         diff = set(prop for prop in diff if not prop.startswith("remote-"))
 
         # Enabling "submodules" and/or "recurseSubmodules" is ok. The
         # additional content will be checked out in invoke().
         if not oldSpec.get("submodules", False) and self.__submodules:
             diff.discard("submodules")
         if not oldSpec.get("recursiveSubmodules", False) and self.__recurseSubmodules:
@@ -687,26 +691,23 @@
 
             if self.__commit:
                 output = self.callGit(workspacePath, 'rev-parse', 'HEAD')
                 if output != self.__commit:
                     status.add(ScmTaint.switched,
                         "> commit: configured: '{}', actual: '{}'".format(self.__commit, output))
             elif self.__tag:
-                output = self.callGit(workspacePath, 'tag', '--points-at', 'HEAD').splitlines()
-                if self.__tag not in output:
+                currentCommit = self.callGit(workspacePath, 'rev-parse', 'HEAD')
+                tagCommit = self.callGit(workspacePath, 'rev-parse',
+                                         'refs/tags/'+self.__tag+'^{commit}',
+                                         check=False)
+                if (not currentCommit) or (currentCommit != tagCommit):
+                    output = self.callGit(workspacePath, 'tag', '--points-at', 'HEAD').splitlines()
                     actual = ("'" + ", ".join(output) + "'") if output else "not on any tag"
                     status.add(ScmTaint.switched,
                         "> tag: configured: '{}', actual: {}".format(self.__tag, actual))
-
-                # Need to check if the tag still exists. Otherwise the "git
-                # log" command at the end will trip.
-                try:
-                    self.callGit(workspacePath, 'rev-parse', 'tags/'+self.__tag)
-                except BuildError:
-                    pass
             elif self.__branch:
                 output = self.callGit(workspacePath, 'rev-parse', '--abbrev-ref', 'HEAD')
                 if output != self.__branch:
                     status.add(ScmTaint.switched,
                         "> branch: configured: '{}', actual: '{}'".format(self.__branch, output))
                 else:
                     output = self.callGit(workspacePath, 'log', '--oneline',
@@ -845,14 +846,15 @@
                 # Annotated tags are objects themselves. We need the commit object!
                 refs = ["refs/tags/" + self.__tag + '^{}', "refs/tags/" + self.__tag]
             else:
                 refs = ["refs/heads/" + self.__branch]
             cmdLine = ['git', 'ls-remote', self.__url] + refs
             try:
                 stdout = await check_output(cmdLine, stderr=subprocess.DEVNULL,
+                    retries = self.__retries,
                     universal_newlines=True, errors='replace')
                 output = stdout.strip()
             except subprocess.CalledProcessError as e:
                 a.fail("exit {}".format(e.returncode), WARNING)
                 return None
             except OSError as e:
                 a.fail("error ({})".format(e))
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/imp.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/imp.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,21 +123,22 @@
         'scm' : 'import',
         'url' : str,
         schema.Optional('if') : schema.Or(str, IfExpression),
     }
 
     SCHEMA = schema.Schema({**__SCHEMA, **DEFAULTS})
 
-    def __init__(self, spec, overrides=[], pruneDefault=None, projectRoot=""):
+    def __init__(self, spec, overrides=[], pruneDefault=None, fixDigestBug=False, projectRoot=""):
         super().__init__(spec, overrides)
         self.__url = spec["url"]
         self.__dir = spec.get("dir", ".")
         self.__prune = spec.get("prune", pruneDefault or False)
         self.__data = spec.get("__data")
         self.__projectRoot = spec.get("__projectRoot", projectRoot)
+        self.__fixDigestBug = fixDigestBug
 
     def getProperties(self, isJenkins):
         ret = super().getProperties(isJenkins)
         ret.update({
             'scm' : 'import',
             'url' : self.__url,
             'dir' : self.__dir,
@@ -158,15 +159,18 @@
             if not os.path.isdir(src):
                 invoker.fail("Cannot import '{}': not a directory!".format(src))
             copyTree(src, dest, invoker)
         else:
             unpackTree(self.__data, dest)
 
     def asDigestScript(self):
-        return self.__url
+        if self.__fixDigestBug:
+            return self.__url + " " + self.__dir
+        else:
+            return self.__url
 
     def getDirectory(self):
         return self.__dir
 
     def isDeterministic(self):
         return False
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/scm.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/scm.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/svn.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/svn.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scm/url.py` & `BobBuildTool-0.23.0rc1/pym/bob/scm/url.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,21 +113,24 @@
     else:
         raise ValueError("URL must be a fully qualified path name")
 
     # looks legit
     return urllib.parse.ParseResult(url.scheme, url.netloc,path, '', '', '')
 
 
+isWin32 = sys.platform == "win32"
+
 class UrlScm(Scm):
 
     DEFAULTS = {
         schema.Optional('extract') : schema.Or(bool, str),
         schema.Optional('fileName') : str,
         schema.Optional('stripComponents') : int,
         schema.Optional('sslVerify') : bool,
+        schema.Optional('retries') : schema.And(int, lambda n: n >= 0, error="Invalid retries attribute"),
     }
 
     __SCHEMA = {
         'scm' : 'url',
         'url' : str,
         schema.Optional('dir') : str,
         schema.Optional('if') : schema.Or(str, IfExpression),
@@ -148,31 +151,34 @@
         (".tar",       "tar"),
         (".gz",        "gzip"),
         (".xz",        "xz"),
         (".7z",        "7z"),
         (".zip",       "zip"),
     ]
 
+    # Use the Python tar/zip extraction only on Windows. They are slower and in
+    # case of tarfile broken in certain ways (e.g. tarfile will result in
+    # different file modes!). But it shouldn't make a difference on Windows.
     EXTRACTORS = {
         "tar"  : [
-            ("tar", ["-x", "--no-same-owner", "--no-same-permissions", "-f", "{}"], "--strip-components={}"),
-            ("python", ["-m", "tarfile", "-e", "{}"], None),
+            (isWin32, "python", ["-m", "tarfile", "-e", "{}"], None),
+            (True, "tar", ["-x", "--no-same-owner", "--no-same-permissions", "-f", "{}"], "--strip-components={}"),
         ],
         "gzip" : [
-            ("gunzip", ["-kf", "{}"], None),
+            (True, "gunzip", ["-kf", "{}"], None),
         ],
         "xz" : [
-            ("unxz", ["-kf", "{}"], None),
+            (True, "unxz", ["-kf", "{}"], None),
         ],
         "7z" : [
-            ("7z", ["x", "-y", "{}"], None),
+            (True, "7z", ["x", "-y", "{}"], None),
         ],
         "zip" : [
-            ("unzip", ["-o", "{}"], None),
-            ("python", ["-m", "zipfile", "-e", "{}", "."], None),
+            (isWin32, "python", ["-m", "zipfile", "-e", "{}", "."], None),
+            (True, "unzip", ["-o", "{}"], None),
         ],
     }
 
     def __init__(self, spec, overrides=[], tidy=None, stripUser=None):
         super().__init__(spec, overrides)
         self.__url = spec["url"]
         self.__digestSha1 = spec.get("digestSHA1")
@@ -200,28 +206,30 @@
                 url = url.replace('\\', '/')
             self.__fn = url.split("/")[-1]
         self.__extract = spec.get("extract", "auto")
         self.__tidy = tidy
         self.__strip = spec.get("stripComponents", 0)
         self.__sslVerify = spec.get('sslVerify', True)
         self.__stripUser = stripUser
+        self.__retries = spec.get("retries", 0)
 
     def getProperties(self, isJenkins):
         ret = super().getProperties(isJenkins)
         ret.update({
             'scm' : 'url',
             'url' : self.__url,
             'digestSHA1' : self.__digestSha1,
             'digestSHA256' : self.__digestSha256,
             'digestSHA512' : self.__digestSha512,
             'dir' : self.__dir,
             'fileName' : self.__fn,
             'extract' : self.__extract,
             'stripComponents' : self.__strip,
             'sslVerify' : self.__sslVerify,
+            'retries' : self.__retries,
         })
         return ret
 
     def _download(self, destination):
         headers = {}
         headers["User-Agent"] = "BobBuildTool/{}".format(BOB_VERSION)
         context = None if self.__sslVerify else sslNoVerifyContext()
@@ -306,21 +314,30 @@
                 # Local files: copy only if newer (u), target never is a directory (T)
                 if isYounger(url.path, destination):
                     if os.path.isdir(destination):
                         invoker.fail("Destination", destination, "is an existing directory!")
                     invoker.trace("<cp>", url.path, workspaceFile)
                     shutil.copy(url.path, destination)
             elif url.scheme in ["http", "https", "ftp"]:
-                invoker.trace("<wget>", self.__url, ">", workspaceFile)
-                try:
-                    err = await invoker.runInExecutor(UrlScm._download, self, destination)
-                    if err:
-                        invoker.fail(err)
-                except (concurrent.futures.CancelledError, concurrent.futures.process.BrokenProcessPool):
-                    invoker.fail("Download interrupted!")
+                retries = self.__retries
+                while True:
+                    invoker.trace("<wget>", self.__url, ">",
+                            workspaceFile, "retires:", retries)
+                    try:
+                        err = await invoker.runInExecutor(UrlScm._download, self, destination)
+                        if err:
+                            if retries == 0:
+                                invoker.fail(err)
+                        else:
+                            break
+                    except (concurrent.futures.CancelledError,
+                            concurrent.futures.process.BrokenProcessPool):
+                        invoker.fail("Download interrupted!")
+                    retries -= 1
+                    await asyncio.sleep(3)
             else:
                 invoker.fail("Unsupported URL scheme: " + url.scheme)
 
 
         # Always verify file hashes
         if self.__digestSha1:
             invoker.trace("<sha1sum>", workspaceFile)
@@ -360,15 +377,15 @@
         Otherwise it is "url dir extract". A "s#" is appended if leading paths
         are stripped where # is the number of stripped elements.
         """
         if self.__stripUser:
             filt = removeUserFromUrl
         else:
             filt = lambda x: x
-        return ( self.__digestSha512 or self.__digestSha256 or 
+        return ( self.__digestSha512 or self.__digestSha256 or
                  self.__digestSha1 or filt(self.__url)
                ) + " " + posixpath.join(self.__dir, self.__fn) + " " + str(self.__extract) + \
                ( " s{}".format(self.__strip) if self.__strip > 0 else "" )
 
     def getDirectory(self):
         return self.__dir if self.__tidy else os.path.join(self.__dir, self.__fn)
 
@@ -412,21 +429,22 @@
             raise ParseError("Invalid extract mode: " + self.__extract)
 
         if extractors is None:
             return []
 
         ret = []
         for extractor in extractors:
+            if not extractor[0]: continue
             if self.__strip > 0:
-                if extractor[2] is None:
+                if extractor[3] is None:
                     continue
-                strip = [extractor[2].format(self.__strip)]
+                strip = [extractor[3].format(self.__strip)]
             else:
                 strip = []
-            ret.append([extractor[0]] + [a.format(self.__fn) for a in extractor[1]] + strip)
+            ret.append([extractor[1]] + [a.format(self.__fn) for a in extractor[2]] + strip)
 
         if not ret:
             raise ParseError("Extractor does not support 'stripComponents'!")
 
         return ret
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/scripts.py` & `BobBuildTool-0.23.0rc1/pym/bob/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
     def cmd():
         parser = argparse.ArgumentParser(prog="bob",
                                          description="Bob build tool\n" + describeCommands(),
                                          formatter_class=argparse.RawDescriptionHelpFormatter)
         parser.add_argument('-C', '--directory', dest='directory', action='append', help="Change to DIRECTORY before doing anything", metavar="DIRECTORY")
         parser.add_argument('--version', dest='version', action='store_true', help="Show version")
-        parser.add_argument('--debug',   dest='debug', help="Enable debug modes (pkgck,ngd)")
+        parser.add_argument('--debug',   dest='debug', help="Enable debug modes (pkgck,ngd,prof)")
         parser.add_argument('-i', dest='ignore_commandCfg', default=False, action='store_true',
                 help="Use bob's default argument settings and do not use commands section of the userconfig.")
         parser.add_argument('--color', dest='color_mode',
                 help="Color mode of console output (default: auto)",
                 choices=['never', 'always', 'auto'])
         parser.add_argument("--query", dest='query_mode', metavar="MODE",
                 choices=['nullset', 'nullglob', 'nullfail'],
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/share.py` & `BobBuildTool-0.23.0rc1/pym/bob/share.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/state.py` & `BobBuildTool-0.23.0rc1/pym/bob/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,16 +285,17 @@
     # Version history:
     #  2 -> 3: byNameDirs: values are tuples (directory, isSourceDir)
     #  3 -> 4: jenkins job names are lower case
     #  4 -> 5: build state stores step kind (checkout-step vs. others)
     #  5 -> 6: build state stores predicted live-build-ids too
     #  6 -> 7: amended directory state for source steps, store attic directories
     #  7 -> 8: normalize attic directories
+    #  8 -> 9: checkout directory state tracks import scm / update script state
     MIN_VERSION = 2
-    CUR_VERSION = 8
+    CUR_VERSION = 9
 
     VERSION_SINCE_ATTIC_TRACKED = 7
 
     instance = None
     def __init__(self):
         self.__path = ".bob-state.pickle"
         self.__uncommittedPath = self.__path + ".new"
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/stringparser.py` & `BobBuildTool-0.23.0rc1/pym/bob/stringparser.py`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/tty.py` & `BobBuildTool-0.23.0rc1/pym/bob/tty.py`

 * *Files 18% similar despite different names*

```diff
@@ -270,27 +270,29 @@
         print("\r" + "\x1b[2K", line, "\x1b[K", sep="")
 
     def __putLine(self, line):
         self.__putLineCont(line)
         self.__putFooter()
 
     def __putFooter(self):
+        # CR, disable line wrap, erase line, ...
         print("\r\x1b[?7l\x1b[2K====== {}/{} jobs running, {}% ({}/{} tasks) done "
                 .format(len(self.__jobs), self.__maxJobs,
                         self.__tasksDone*100//self.__tasksNum,
                         self.__tasksDone, self.__tasksNum),
               end="")
         i = 0
         while i < self.__maxJobs:
             num = self.__slots[i]
             if num is not None:
                 print("\n\x1b[2K {:>4}  {}".format(num, self.__jobs[num]), end='')
             else:
                 print("\n\x1b[2K ****  <idle>", end='')
             i += 1
+        # Move up <i> lines, enable line wrap
         print("\x1b[{}A".format(i), "\x1b[?7h\r", sep='', end='')
 
     def _putResult(self, slot, msg):
         job = self.__slots[slot]
         self.__slots[slot] = None
         del self.__jobs[job]
         if msg:
@@ -377,20 +379,15 @@
             else:
                 kind = self.err_kind
                 status = self.err_message
             msg += status
         elif exc_type is not None and self.err_message:
             kind = self.err_kind
             stderr = self.err_message
-        self.__tui._print(self.__job, msg, kind, "End")
-        if stderr:
-            # Print error messages on stderr when being on a dumb output. It is
-            # probably redirected by some other script or an analyzed IDE (thin
-            # "bob project").
-            print(stderr, file=sys.stderr)
+        self.__tui._printResult(self.__job, msg, stderr, kind)
         return False
 
 class ParallelDumbUI(BaseTUI):
     def __init__(self, verbosity):
         super().__init__(verbosity)
         self.__index = 1
 
@@ -399,14 +396,110 @@
         self.__index += 1
         return ret
 
     def _print(self, job, msg, kind, stage=""):
         level = COLORS2TEXT[kind & 7]
         print("[{:<5} {:>4}] {}: {}".format(stage, job, level, colorize(msg, kind)))
 
+    def _printResult(self, job, msg, stderr, kind):
+        self._print(job, msg, kind, "End")
+        if stderr:
+            # Print error messages on stderr when being on a dumb output. It is
+            # probably redirected by some other script or an analyzed IDE (think
+            # "bob project").
+            print(stderr, file=sys.stderr)
+
+    def log(self, message, kind, severity):
+        if not self._isVisible(severity): return
+        self._print("****", message, kind, "*****")
+
+    def stepMessage(self, step, action, message, kind, severity):
+        if not self._isVisible(severity): return
+        self._print("", "{:10}{} - {}".format(action,
+            step.getPackage().getName(), message), kind)
+
+    def stepAction(self, step, action, message, severity, details):
+        return self.__action(step, action, message, severity, details, True)
+
+    def stepExec(self, step, action, message, severity, details):
+        return self.__action(step, action, message, severity, details, False)
+
+    def __action(self, step, action, message, severity, details, ellipsis):
+        if not self._isVisible(severity): return DummyTUIAction()
+        showDetails = self._isVisible(INFO)
+        if showDetails and details:
+            details = " " + details
+        else:
+            details = ""
+        if ellipsis:
+            details += ": "
+
+        job = self.__nextJob()
+        name = step.getPackage().getName()
+        self._print(job, "{:10}{} - {}".format(action, name, message), EXECUTED, "Start")
+        msg = "{:10}{} - {}{}".format(action, name, message, details)
+        return ParallelDumbUIAction(self, job, name, msg, ellipsis, showDetails)
+
+class MassiveParallelTtyUI(BaseTUI):
+    def __init__(self, verbosity, maxJobs):
+        super().__init__(verbosity)
+        self.__index = 1
+        self.__maxJobs = maxJobs
+        self.__jobs = {}
+        self.__tasksDone = 0
+        self.__tasksNum = 1
+
+        # disable cursor
+        print("\x1b[?25l")
+
+        # disable echo
+        try:
+            import termios
+            fd = sys.stdin.fileno()
+            self.__oldTcAttr = termios.tcgetattr(fd)
+            new = termios.tcgetattr(fd)
+            new[3] = new[3] & ~termios.ECHO
+            termios.tcsetattr(fd, termios.TCSADRAIN, new)
+        except ImportError:
+            pass
+
+    def __nextJob(self):
+        ret = self.__index
+        self.__index += 1
+        return ret
+
+    def __putLineCont(self, line):
+        print("\r" + "\x1b[2K", line, "\x1b[K", sep="")
+
+    def __putLine(self, line):
+        self.__putLineCont(line)
+        self.__putFooter()
+
+    def __putFooter(self):
+        # CR, disable line wrap, erase line, ...
+        print("\r\x1b[?7l\x1b[2K====== {}/{} jobs running, {}% ({}/{} tasks) done "
+                .format(len(self.__jobs), self.__maxJobs,
+                        self.__tasksDone*100//self.__tasksNum,
+                        self.__tasksDone, self.__tasksNum))
+        for i, name in sorted(self.__jobs.items()):
+            print("[{} {}]".format(i, name), end="")
+        # Move up one lines, enable line wrap
+        print("\x1b[A\x1b[?7h\r", end='')
+
+    def _print(self, job, msg, kind, stage=""):
+        self.__putLine("[{:<5} {:>4}] {}".format(stage, job, colorize(msg, kind)))
+
+    def _printResult(self, job, msg, stderr, kind):
+        del self.__jobs[job]
+        self._print(job, msg, kind, "End")
+        if stderr:
+            for l in stderr.splitlines():
+                self.__putLineCont("[{:<5} {:>4}] {}".format("ERR", job, l))
+            self.__putFooter()
+
     def log(self, message, kind, severity):
         if not self._isVisible(severity): return
         self._print("****", message, kind, "*****")
 
     def stepMessage(self, step, action, message, kind, severity):
         if not self._isVisible(severity): return
         self._print("", "{:10}{} - {}".format(action,
@@ -426,18 +519,33 @@
         else:
             details = ""
         if ellipsis:
             details += ": "
 
         job = self.__nextJob()
         name = step.getPackage().getName()
+        self.__jobs[job] = name
         self._print(job, "{:10}{} - {}".format(action, name, message), EXECUTED, "Start")
         msg = "{:10}{} - {}{}".format(action, name, message, details)
         return ParallelDumbUIAction(self, job, name, msg, ellipsis, showDetails)
 
+    def cleanup(self):
+        self.__putFooter()
+        print()
+        print("\x1b[?25h")
+        try:
+            import termios
+            termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, self.__oldTcAttr)
+        except ImportError:
+            pass
+
+    def setProgress(self, done, num):
+        self.__tasksDone = done
+        self.__tasksNum = num
+
 def log(message, kind, severity=-2):
     __tui.log(message, kind, severity)
 
 def stepMessage(step, action, message, kind, severity=-2):
     __tui.stepMessage(step, action, message, kind, severity)
 
 def stepAction(step, action, message, severity=-2, details=""):
@@ -455,15 +563,18 @@
 
 def setTui(maxJobs):
     global __tui
     __tui.cleanup()
     if maxJobs <= 1:
         __tui = SingleTUI(__tui.getVerbosity())
     elif __onTTY:
-        __tui = ParallelTtyUI(__tui.getVerbosity(), maxJobs)
+        if maxJobs <= __parallelTUIThreshold:
+            __tui = ParallelTtyUI(__tui.getVerbosity(), maxJobs)
+        else:
+            __tui = MassiveParallelTtyUI(__tui.getVerbosity(), maxJobs)
     else:
         __tui = ParallelDumbUI(__tui.getVerbosity())
 
 def cleanup():
     __tui.cleanup()
     if __onTTY and sys.platform == "win32":
         kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), __origMode.value)
@@ -479,14 +590,15 @@
         kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), __origMode.value | 4)
 
 # module initialization
 
 __onTTY = (sys.stdout.isatty() and sys.stderr.isatty())
 __useColor = False
 __tui = SingleTUI(NORMAL)
+__parallelTUIThreshold = 16
 
 if __onTTY and sys.platform == "win32":
     # Try to set ENABLE_VIRTUAL_TERMINAL_PROCESSING flag. Enables vt100 color
     # codes on Windows 10 console. If this fails we inhibit color code usage
     # because it will clutter the output.
     import ctypes
     import ctypes.wintypes
@@ -501,9 +613,13 @@
     if mode == 'never':
         __useColor = False
     elif mode == 'always':
         __useColor = True
     elif mode == 'auto':
         __useColor = __onTTY
 
+def setParallelTUIThreshold(num):
+    global __parallelTUIThreshold
+    __parallelTUIThreshold = num
+
 # auto is the default
 setColorMode('auto')
```

### Comparing `BobBuildTool-0.22.0rc1/pym/bob/utils.py` & `BobBuildTool-0.23.0rc1/pym/bob/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,19 @@
                 return self.magic.file(name)
         return WrapMagic()
     else:
         raise NotImplementedError("I do not understand your magic")
 
 ### directory copy ###
 
-def copyTree(src, dst):
+class __BlackHoleSet:
+    def add(self, item):
+        pass
+
+def copyTree(src, dst, fileSet = __BlackHoleSet()):
     try:
         names = os.listdir(src)
         os.makedirs(dst, exist_ok=True)
     except OSError as e:
         logging.getLogger(__name__).error("Copy '%s' to '%s' failed: %s", src,
                                           dst, str(e))
         return False
@@ -622,14 +626,15 @@
                     logging.getLogger(__name__).error(
                         "Cannon overwrite non-directory '%s' with directory '%s'",
                         dstname, srcname)
                     ret = False
                 else:
                     ret = copyTree(srcname, dstname) and ret
             else:
+                fileSet.add(dstname)
                 if os.path.lexists(dstname):
                     os.unlink(dstname)
                 if os.path.islink(srcname):
                     linkto = os.readlink(srcname)
                     os.symlink(linkto, dstname)
                 else:
                     shutil.copy(srcname, dstname)
@@ -732,31 +737,41 @@
     def __exit__(self, exc_type, exc_value, traceback):
         import asyncio
         self.__executor.shutdown()
         self.__loop.close()
         asyncio.set_event_loop(None)
 
 
-async def run(args, universal_newlines=False, errors=None, check=False, shell=False, **kwargs):
+async def run(args, universal_newlines=False, errors=None, check=False,
+        shell=False, retries=0, **kwargs):
     """Provide the subprocess.run() function as asyncio corouting.
 
     This takes care of the missing 'universal_newlines' and 'check' options.
     Everything else is passed through. Will also raise the same exceptions as
     subprocess.run() to act as a drop-in replacement.
     """
     import asyncio
     import io
     import locale
     import subprocess
 
-    if shell:
-        proc = await asyncio.create_subprocess_shell(args, **kwargs)
-    else:
-        proc = await asyncio.create_subprocess_exec(*args, **kwargs)
-    stdout, stderr = await proc.communicate()
+    stdout = ""
+    stderr = ""
+
+    while True:
+        if shell:
+            proc = await asyncio.create_subprocess_shell(args, **kwargs)
+        else:
+            proc = await asyncio.create_subprocess_exec(*args, **kwargs)
+        stdout, stderr = await proc.communicate()
+
+        if (proc.returncode == 0) or (retries == 0):
+            break
+        retries -= 1
+        await asyncio.sleep(1)
 
     if universal_newlines and (stdout is not None):
         stdout = io.TextIOWrapper(io.BytesIO(stdout), errors=errors).read()
     if universal_newlines and (stderr is not None):
         stderr = io.TextIOWrapper(io.BytesIO(stderr), errors=errors).read()
 
     if check and (proc.returncode != 0):
```

### Comparing `BobBuildTool-0.22.0rc1/setup.py` & `BobBuildTool-0.23.0rc1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,56 +37,48 @@
             "src/namespace-sandbox/namespace-sandbox.c",
             "src/namespace-sandbox/network-tools.c",
             "src/namespace-sandbox/process-tools.c",
             "-std=c99", "-Os", "-static", "-lm",
             "-ffunction-sections", "-fdata-sections", "-Wl,--gc-sections"])
         self.spawn(["strip", "bin/bob-namespace-sandbox"])
 
+# Additional command to build manpages on POSIX systems
+class BuildManpages(Command):
+    description = "Build manpages"
+    user_options = []
+
+    def enabled(self):
+        return sys.platform != "win32"
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        self.spawn(["sphinx-build", "-b", "man", "doc", "doc/_build/man"])
+
 # Wrapper around build command to force automatic execution of the
 # documentation and applet builds.
 class build(build_orig):
     sub_commands = [
-        ('build_apps', BuildApps.enabled )
+        ('build_apps', BuildApps.enabled ),
+        ('build_man', BuildManpages.enabled ),
     ] + build_orig.sub_commands
 
 cmdclass = {
     'build' : build,
     'build_apps': BuildApps,
+    'build_man' : BuildManpages,
 }
 data_files = []
 
-# Installation time dependencies only needed by setup.py
-setup_requires = [
-    'setuptools_scm<7',   # automatically get package version
-                          # TODO: remove constraint when Python 3.7 is required
-]
-
-# Stub class that acts as a proxy for the real sphinx.setup_command.BuildDoc
-# class. We want to defer the import until it is really needed to give the
-# setuptools a chance to fetch the build depencency first.
-class BuildDocStub:
-    def __getattr__(self, attr):
-        from sphinx.setup_command import BuildDoc
-        return getattr(BuildDoc, attr)
-
-    def __setattr__(self, attr, value):
-        from sphinx.setup_command import BuildDoc
-        setattr(BuildDoc, attr, value)
-
-    def __call__(self, *args, **kwargs):
-        from sphinx.setup_command import BuildDoc
-        return BuildDoc(*args, **kwargs)
-
 # Sphinx manpages and bash completion do not work on Windows
 if sys.platform != 'win32':
-    cmdclass['build_sphinx'] = BuildDocStub()
-    build.sub_commands.append(('build_sphinx', None))
-    setup_requires.extend([
-        'sphinx',
-    ])
     data_files.extend([
         ('share/man/man1', [
             'doc/_build/man/bob-archive.1',
             'doc/_build/man/bob-build.1',
             'doc/_build/man/bob-clean.1',
             'doc/_build/man/bob-dev.1',
             'doc/_build/man/bob-graph.1',
@@ -147,15 +139,18 @@
 
     # Optional dependencies that are not needed by default
     extras_require = {
         'azure' : [ 'azure-storage-blob' ],
     },
 
     # Installation time dependencies only needed by setup.py
-    setup_requires = setup_requires,
+    setup_requires = [
+        'setuptools_scm<7',   # automatically get package version
+                              # TODO: remove constraint when Python 3.7 is required
+    ],
 
     # Provide executables
     entry_points = {
         'console_scripts' : [
             'bob = bob.scripts:bob',
         ]
     },
```

### Comparing `BobBuildTool-0.22.0rc1/src/namespace-sandbox/namespace-sandbox.c` & `BobBuildTool-0.23.0rc1/src/namespace-sandbox/namespace-sandbox.c`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/src/namespace-sandbox/network-tools.c` & `BobBuildTool-0.23.0rc1/src/namespace-sandbox/network-tools.c`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/src/namespace-sandbox/network-tools.h` & `BobBuildTool-0.23.0rc1/src/namespace-sandbox/network-tools.h`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/src/namespace-sandbox/process-tools.c` & `BobBuildTool-0.23.0rc1/src/namespace-sandbox/process-tools.c`

 * *Files identical despite different names*

### Comparing `BobBuildTool-0.22.0rc1/src/namespace-sandbox/process-tools.h` & `BobBuildTool-0.23.0rc1/src/namespace-sandbox/process-tools.h`

 * *Files identical despite different names*

