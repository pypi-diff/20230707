# Comparing `tmp/ipyforcegraph-0.3.5.tar.gz` & `tmp/ipyforcegraph-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyforcegraph-0.3.5.tar", last modified: Wed Jul  5 15:05:47 2023, max compression
+gzip compressed data, was "ipyforcegraph-0.3.6.tar", last modified: Fri Jul  7 18:06:18 2023, max compression
```

## Comparing `ipyforcegraph-0.3.5.tar` & `ipyforcegraph-0.3.6.tar`

### file list

```diff
@@ -1,305 +1,307 @@
--rw-r--r--   0        0        0      658 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.binder/environment.yml
--rw-r--r--   0        0        0      352 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.binder/jupyter_config.json
--rw-r--r--   0        0        0      145 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.binder/overrides.json
--rwxr-xr-x   0        0        0      904 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.binder/postBuild
--rw-r--r--   0        0        0      353 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/.condarc
--rw-r--r--   0        0        0     2483 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      787 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0        0        0      620 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1956 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/release.md
--rw-r--r--   0        0        0    39804 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_dev_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    13823 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_lock.conda.lock
--rw-r--r--   0        0        0    24334 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.5_py3.11.conda.lock
--rw-r--r--   0        0        0    23987 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.5_py3.8.conda.lock
--rw-r--r--   0        0        0    25224 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    24875 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.6_py3.8.conda.lock
--rw-r--r--   0        0        0    38377 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_dev_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    11993 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_lock.conda.lock
--rw-r--r--   0        0        0    23677 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.5_py3.11.conda.lock
--rw-r--r--   0        0        0    23330 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.5_py3.8.conda.lock
--rw-r--r--   0        0        0    24563 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    24214 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.6_py3.8.conda.lock
--rw-r--r--   0        0        0    36687 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_dev_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    12051 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_lock.conda.lock
--rw-r--r--   0        0        0    23677 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.5_py3.11.conda.lock
--rw-r--r--   0        0        0    23330 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.5_py3.8.conda.lock
--rw-r--r--   0        0        0    24563 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.6_py3.11.conda.lock
--rw-r--r--   0        0        0    24214 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.6_py3.8.conda.lock
--rw-r--r--   0        0        0     1031 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/pull_request_template.md
--rw-r--r--   0        0        0       36 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/requirements-build.txt
--rw-r--r--   0        0        0      258 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_atest.yml
--rw-r--r--   0        0        0      105 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_build.yml
--rw-r--r--   0        0        0       59 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_channels.yml
--rw-r--r--   0        0        0       40 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_demo.yml
--rw-r--r--   0        0        0      279 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_docs.yml
--rw-r--r--   0        0        0       59 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_doit.yml
--rw-r--r--   0        0        0      110 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_ext.yml
--rw-r--r--   0        0        0      132 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_lab/lab3.5.yml
--rw-r--r--   0        0        0       80 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_lab/lab3.6.yml
--rw-r--r--   0        0        0      222 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_lint.yml
--rw-r--r--   0        0        0       64 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_lint_unix.yml
--rw-r--r--   0        0        0       54 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_lint_win.yml
--rw-r--r--   0        0        0       48 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_nomkl.yml
--rw-r--r--   0        0        0       38 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_py/py3.11.yml
--rw-r--r--   0        0        0       50 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_py/py3.8.yml
--rw-r--r--   0        0        0       36 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_release.yml
--rw-r--r--   0        0        0      110 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_run.yml
--rw-r--r--   0        0        0       80 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_spell.yml
--rw-r--r--   0        0        0      184 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/_utest.yml
--rw-r--r--   0        0        0      240 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/binder.yml
--rw-r--r--   0        0        0      249 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/dev.yml
--rw-r--r--   0        0        0      161 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/lock.yml
--rw-r--r--   0        0        0      237 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/rtd.yml
--rw-r--r--   0        0        0      150 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/specs/test.yml
--rw-r--r--   0        0        0     1333 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/workflows/badges.yml
--rw-r--r--   0        0        0     8993 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2531 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.github/workflows/pages.yml
--rw-r--r--   0        0        0     2004 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.gitignore
--rw-r--r--   0        0        0      113 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.prettierignore
--rw-r--r--   0        0        0      349 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.readthedocs.yml
--rw-r--r--   0        0        0      193 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/.yarnrc
--rw-r--r--   0        0        0     4818 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     6635 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1367 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/COPYRIGHT.md
--rw-r--r--   0        0        0     1526 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0    11397 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/README.md
--rw-r--r--   0        0        0     2919 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/01_Behaviors.robot
--rw-r--r--   0        0        0     2635 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/02_Colors_ForceGraph.robot
--rw-r--r--   0        0        0     2647 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/02_Colors_ForceGraph3D.robot
--rw-r--r--   0        0        0     2495 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/02_Colors_GRAPH.robot.j2
--rw-r--r--   0        0        0     2493 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/03_Events.robot
--rw-r--r--   0        0        0     3501 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/04_Shapes_ForceGraph.robot
--rw-r--r--   0        0        0     3529 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/04_Shapes_ForceGraph3D.robot
--rw-r--r--   0        0        0     3130 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/04_Shapes_GRAPH.robot.j2
--rw-r--r--   0        0        0     5956 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/05_LinkShapes_ForceGraph.robot
--rw-r--r--   0        0        0     6004 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/05_LinkShapes_ForceGraph3D.robot
--rw-r--r--   0        0        0     4826 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/05_LinkShapes_GRAPH.robot.j2
--rw-r--r--   0        0        0     2581 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/06_Scales_ForceGraph.robot
--rw-r--r--   0        0        0     2589 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/06_Scales_ForceGraph3D.robot
--rw-r--r--   0        0        0     2587 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/06_Scales_GRAPH.robot.j2
--rw-r--r--   0        0        0     2925 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/07_Camera_ForceGraph.robot
--rw-r--r--   0        0        0     2929 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/07_Camera_ForceGraph3D.robot
--rw-r--r--   0        0        0     2967 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/07_Camera_GRAPH.robot.j2
--rw-r--r--   0        0        0      195 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/API/__init__.robot
--rw-r--r--   0        0        0      470 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/01_Index.robot
--rw-r--r--   0        0        0      482 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/02_Behaviors.robot
--rw-r--r--   0        0        0      469 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/03_3D.robot
--rw-r--r--   0        0        0      717 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/04_Force.robot
--rw-r--r--   0        0        0      492 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/05_WidgetSource.robot
--rw-r--r--   0        0        0      490 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/06_DodoSource.robot
--rw-r--r--   0        0        0      481 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/07_DodoApp.robot
--rw-r--r--   0        0        0      225 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Notebooks/__init__.robot
--rw-r--r--   0        0        0     1643 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Regression/103_2D_Not_Text.robot
--rw-r--r--   0        0        0      796 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Regression/90_Preserved_ID_Order.robot
--rw-r--r--   0        0        0      226 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Regression/__init__.robot
--rw-r--r--   0        0        0      242 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/Smoke.robot
--rw-r--r--   0        0        0      295 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/__init__.robot
--rw-r--r--   0        0        0      385 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_libraries/Ports.py
--rw-r--r--   0        0        0      324 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/Camera.py
--rw-r--r--   0        0        0      354 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/Colors.py
--rw-r--r--   0        0        0      387 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/Event.py
--rw-r--r--   0        0        0      585 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/GraphData.py
--rw-r--r--   0        0        0      405 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/LinkSelection.py
--rw-r--r--   0        0        0      772 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/LinkShapes.py
--rw-r--r--   0        0        0      390 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/NodeSelection.py
--rw-r--r--   0        0        0      486 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/NodeShapes.py
--rw-r--r--   0        0        0      199 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/NodeTooltip.py
--rw-r--r--   0        0        0      525 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/api/Scales.py
--rw-r--r--   0        0        0      336 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/default_setting_overrides.json
--rw-r--r--   0        0        0      151 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/jupyter_config.json
--rw-r--r--   0        0        0      847 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/regression/gh-103.py
--rw-r--r--   0        0        0     1855 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/fixtures/regression/gh-90.py
--rw-r--r--   0        0        0      959 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Browser.robot
--rw-r--r--   0        0        0      137 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/CLI.robot
--rw-r--r--   0        0        0      758 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Coverage.robot
--rw-r--r--   0        0        0     5538 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/IPyForceGraph.robot
--rw-r--r--   0        0        0     8763 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Lab.robot
--rw-r--r--   0        0        0      210 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Meta.robot
--rw-r--r--   0        0        0      947 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Regression.robot
--rw-r--r--   0        0        0      469 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Screenshots.robot
--rw-r--r--   0        0        0     4886 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/keywords/Server.robot
--rw-r--r--   0        0        0      149 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/variables/Browser.robot
--rw-r--r--   0        0        0      606 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/variables/IPyForceGraph.robot
--rw-r--r--   0        0        0     3121 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/variables/Lab.robot
--rw-r--r--   0        0        0      150 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/atest/_resources/variables/Server.robot
--rw-r--r--   0        0        0     2359 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/_static/anvil.svg
--rw-r--r--   0        0        0    20274 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/_static/logo.svg
--rw-r--r--   0        0        0      540 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/_static/theme.css
--rw-r--r--   0        0        0    29973 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/_static/wordmark.svg
--rw-r--r--   0        0        0       34 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/changelog.md
--rw-r--r--   0        0        0     2597 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/conf.py
--rw-r--r--   0        0        0       37 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/contributing.md
--rw-r--r--   0        0        0     1355 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/dictionary.txt
--rw-r--r--   0        0        0      908 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/environment.yml
--rw-r--r--   0        0        0      431 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/index.md
--rw-r--r--   0        0        0      270 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/base.md
--rw-r--r--   0        0        0      637 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/behaviors.md
--rw-r--r--   0        0        0      108 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/forces.md
--rw-r--r--   0        0        0      209 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/index.md
--rw-r--r--   0        0        0      113 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/module.md
--rw-r--r--   0        0        0      108 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/scales.md
--rw-r--r--   0        0        0      302 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/sources.md
--rw-r--r--   0        0        0       98 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/docs/reference/widgets.md
--rw-r--r--   0        0        0    26820 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/dodo.py
--rw-r--r--   0        0        0     2816 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/3D.ipynb
--rw-r--r--   0        0        0    33076 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Behaviors.ipynb
--rw-r--r--   0        0        0    14645 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Camera.ipynb
--rw-r--r--   0        0        0     1300 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/DodoApp.ipynb
--rw-r--r--   0        0        0    34979 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/DodoSource.ipynb
--rw-r--r--   0        0        0    31389 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Forces.ipynb
--rw-r--r--   0        0        0     6912 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Scales.ipynb
--rw-r--r--   0        0        0     5317 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Shapes.ipynb
--rw-r--r--   0        0        0     6429 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Test_Behaviors.ipynb
--rw-r--r--   0        0        0     2382 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Test_Forces.ipynb
--rw-r--r--   0        0        0    37961 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/Utils.ipynb
--rw-r--r--   0        0        0     5797 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/WidgetSource.ipynb
--rw-r--r--   0        0        0     5856 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/_index.ipynb
--rw-r--r--   0        0        0   342558 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/datasets/blocks.json
--rw-r--r--   0        0        0    13906 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/datasets/d3-dependencies.csv
--rw-r--r--   0        0        0     9808 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/datasets/logo.svg
--rw-r--r--   0        0        0    19506 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/datasets/miserables.json
--rw-r--r--   0        0        0  3566209 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/datasets/mplate.mtx
--rw-r--r--   0        0        0      123 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/examples/requirements.txt
--rw-r--r--   0        0        0      710 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/ignored-vulnerabilities.json
--rw-r--r--   0        0        0      244 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/index.ts
--rw-r--r--   0        0        0     1688 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/plugin.ts
--rw-r--r--   0        0        0     2926 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/template-utils.ts
--rw-r--r--   0        0        0     8968 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/tokens.ts
--rw-r--r--   0        0        0      278 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/tsconfig.cov.json
--rw-r--r--   0        0        0      225 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/tsconfig.json
--rw-r--r--   0        0        0      202 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/typings.d.ts
--rw-r--r--   0        0        0     1386 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/utils.ts
--rw-r--r--   0        0        0     7963 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/base.ts
--rw-r--r--   0        0        0     1420 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/dag.ts
--rw-r--r--   0        0        0     1081 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-center.ts
--rw-r--r--   0        0        0     3060 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-cluster.ts
--rw-r--r--   0        0        0     1100 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-collision.ts
--rw-r--r--   0        0        0     1118 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-link.ts
--rw-r--r--   0        0        0     1352 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-manybody.ts
--rw-r--r--   0        0        0     1322 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-radial.ts
--rw-r--r--   0        0        0     1025 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-x.ts
--rw-r--r--   0        0        0     1025 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-y.ts
--rw-r--r--   0        0        0     1025 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-z.ts
--rw-r--r--   0        0        0     5704 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force.ts
--rw-r--r--   0        0        0      442 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/forces/index.ts
--rw-r--r--   0        0        0     6906 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/graph-camera.ts
--rw-r--r--   0        0        0     2507 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/graph-data.ts
--rw-r--r--   0        0        0     2588 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/graph-image.ts
--rw-r--r--   0        0        0      569 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/index.ts
--rw-r--r--   0        0        0     1169 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/link-arrow.ts
--rw-r--r--   0        0        0     1333 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/link-particles.ts
--rw-r--r--   0        0        0     4340 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/link-selection.ts
--rw-r--r--   0        0        0     1276 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/link-shape.ts
--rw-r--r--   0        0        0      726 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/link-tooltip.ts
--rw-r--r--   0        0        0     3065 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/node-selection.ts
--rw-r--r--   0        0        0     2962 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/node-shape.ts
--rw-r--r--   0        0        0      726 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/node-tooltip.ts
--rw-r--r--   0        0        0     2845 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/scales.ts
--rw-r--r--   0        0        0     6165 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/base.ts
--rw-r--r--   0        0        0     1420 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/ellipse.ts
--rw-r--r--   0        0        0      198 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/index.ts
--rw-r--r--   0        0        0     1165 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/rectangle.ts
--rw-r--r--   0        0        0     3801 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/text.ts
--rw-r--r--   0        0        0    29034 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/display/2d.ts
--rw-r--r--   0        0        0     4435 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/display/3d.ts
--rw-r--r--   0        0        0      161 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/display/index.ts
--rw-r--r--   0        0        0      200 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/index.ts
--rw-r--r--   0        0        0     1361 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/serializers/dataframe.ts
--rw-r--r--   0        0        0      172 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/serializers/index.ts
--rw-r--r--   0        0        0      244 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/serializers/widget.ts
--rw-r--r--   0        0        0     7376 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/sources/dataframe.ts
--rw-r--r--   0        0        0      146 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/js/widgets/sources/index.ts
--rw-r--r--   0        0        0      135 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/lite/jupyter-lite.json
--rw-r--r--   0        0        0      196 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/lite/jupyter_lite_config.json
--rw-r--r--   0        0        0     4540 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/package.json
--rw-r--r--   0        0        0      231 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/pages-lite/jupyter_lite_config.json
--rw-r--r--   0        0        0     3329 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/__init__.py
--rw-r--r--   0        0        0     4136 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/atest.py
--rw-r--r--   0        0        0     6234 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/preflight.py
--rw-r--r--   0        0        0     9803 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/project.py
--rw-r--r--   0        0        0     1475 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/reporter.py
--rw-r--r--   0        0        0    14275 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/scripts/utils.py
--rw-r--r--   0        0        0     4682 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/package.json
--rw-r--r--   0        0        0     8813 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js
--rw-r--r--   0        0        0    42811 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js.map
--rw-r--r--   0        0        0      697 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js
--rw-r--r--   0        0        0     2332 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js.map
--rw-r--r--   0        0        0    50849 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.372aa8d5d70bf4bd091a.js
--rw-r--r--   0        0        0   183336 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.372aa8d5d70bf4bd091a.js.map
--rw-r--r--   0        0        0    28470 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js
--rw-r--r--   0        0        0   125192 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js.map
--rw-r--r--   0        0        0    48532 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js
--rw-r--r--   0        0        0   203549 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js.map
--rw-r--r--   0        0        0      329 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/228.bb390299503f7f9e929a.js
--rw-r--r--   0        0        0      356 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/228.bb390299503f7f9e929a.js.map
--rw-r--r--   0        0        0      329 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/271.512f94c488062f5c2b86.js
--rw-r--r--   0        0        0      377 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/271.512f94c488062f5c2b86.js.map
--rw-r--r--   0        0        0    96265 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js
--rw-r--r--   0        0        0       41 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.LICENSE.txt
--rw-r--r--   0        0        0   352279 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.map
--rw-r--r--   0        0        0      329 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/460.761d5a8d3129bfa049b2.js
--rw-r--r--   0        0        0      367 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/460.761d5a8d3129bfa049b2.js.map
--rw-r--r--   0        0        0    27597 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js
--rw-r--r--   0        0        0      225 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.LICENSE.txt
--rw-r--r--   0        0        0   109234 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.map
--rw-r--r--   0        0        0     1047 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js
--rw-r--r--   0        0        0     3709 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js.map
--rw-r--r--   0        0        0     7177 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js
--rw-r--r--   0        0        0    22576 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js.map
--rw-r--r--   0        0        0     7762 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js
--rw-r--r--   0        0        0    19473 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js.map
--rw-r--r--   0        0        0      327 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/65.e565d3630178010e411b.js
--rw-r--r--   0        0        0      372 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/65.e565d3630178010e411b.js.map
--rw-r--r--   0        0        0   160979 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/67fea965f2310612f9225ab29510fcff9b836e237e6f5cd8c05b266870ffd0d5.js
--rw-r--r--   0        0        0     9063 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/6eebc3e07550540f4bcb82887a5a6da943ea90aaba205486fd1b70b8db0ccfc5.js
--rw-r--r--   0        0        0    11098 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.a54f5f8e362355a77aa3.js
--rw-r--r--   0        0        0    37123 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.a54f5f8e362355a77aa3.js.map
--rw-r--r--   0        0        0     5943 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.9e3da00a7ac27d110b10.js
--rw-r--r--   0        0        0    12225 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.9e3da00a7ac27d110b10.js.map
--rw-r--r--   0        0        0    30158 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js
--rw-r--r--   0        0        0    69349 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js.map
--rw-r--r--   0        0        0   644942 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js
--rw-r--r--   0        0        0      100 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js.LICENSE.txt
--rw-r--r--   0        0        0   348579 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/998250a831af662f5f25.wasm
--rw-r--r--   0        0        0   635410 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js
--rw-r--r--   0        0        0       92 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js.LICENSE.txt
--rw-r--r--   0        0        0     9664 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.183d551b88ec5615b6f7.js
--rw-r--r--   0        0        0    43533 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.183d551b88ec5615b6f7.js.map
--rw-r--r--   0        0        0    30447 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/third-party-licenses.json
--rw-r--r--   0        0        0      536 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/__init__.py
--rw-r--r--   0        0        0      724 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/_base.py
--rw-r--r--   0        0        0      929 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/__init__.py
--rw-r--r--   0        0        0     7633 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/_base.py
--rw-r--r--   0        0        0    13199 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/forces.py
--rw-r--r--   0        0        0     1294 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/particles.py
--rw-r--r--   0        0        0     5156 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/recording.py
--rw-r--r--   0        0        0     3314 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/scales.py
--rw-r--r--   0        0        0     2778 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/selection.py
--rw-r--r--   0        0        0     5068 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/shapes.py
--rw-r--r--   0        0        0     1365 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/tooltip.py
--rw-r--r--   0        0        0      690 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/constants.py
--rw-r--r--   0        0        0     2740 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/graphs.py
--rw-r--r--   0        0        0      569 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/js.py
--rw-r--r--   0        0        0        0 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/py.typed
--rw-r--r--   0        0        0     1610 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/serializers.py
--rw-r--r--   0        0        0      287 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/sources/__init__.py
--rw-r--r--   0        0        0     2697 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/sources/dataframe.py
--rw-r--r--   0        0        0    11300 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/sources/dodo.py
--rw-r--r--   0        0        0     9476 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/sources/widget.py
--rw-r--r--   0        0        0      108 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/__init__.py
--rw-r--r--   0        0        0      436 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/conftest.py
--rw-r--r--   0        0        0      443 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_dag_widget.py
--rw-r--r--   0        0        0     1996 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_dodo_source.py
--rw-r--r--   0        0        0      578 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_meta.py
--rw-r--r--   0        0        0     1433 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_scales.py
--rw-r--r--   0        0        0     1615 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_serializers.py
--rw-r--r--   0        0        0     1725 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_widget_model_meta.py
--rw-r--r--   0        0        0     1455 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_widget_source.py
--rw-r--r--   0        0        0     1289 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/src/ipyforcegraph/trait_utils.py
--rw-r--r--   0        0        0      930 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/style/index.css
--rw-r--r--   0        0        0      186 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/tsconfig.json
--rw-r--r--   0        0        0      580 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/tsconfigbase.json
--rw-r--r--   0        0        0      493 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/webpack.config.js
--rw-r--r--   0        0        0   239298 2023-07-05 15:05:47.000000 ipyforcegraph-0.3.5/yarn.lock
--rw-r--r--   0        0        0    12930 1970-01-01 00:00:00.000000 ipyforcegraph-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      658 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.binder/environment.yml
+-rw-r--r--   0        0        0      352 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.binder/jupyter_config.json
+-rw-r--r--   0        0        0      145 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.binder/overrides.json
+-rwxr-xr-x   0        0        0      904 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.binder/postBuild
+-rw-r--r--   0        0        0      353 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/.condarc
+-rw-r--r--   0        0        0     2483 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      787 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0      620 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1956 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/release.md
+-rw-r--r--   0        0        0    39686 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_dev_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    14065 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_lock.conda.lock
+-rw-r--r--   0        0        0    24218 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.5_py3.11.conda.lock
+-rw-r--r--   0        0        0    23871 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.5_py3.8.conda.lock
+-rw-r--r--   0        0        0    25108 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    24759 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.6_py3.8.conda.lock
+-rw-r--r--   0        0        0    38259 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_dev_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    12233 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_lock.conda.lock
+-rw-r--r--   0        0        0    23561 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.5_py3.11.conda.lock
+-rw-r--r--   0        0        0    23214 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.5_py3.8.conda.lock
+-rw-r--r--   0        0        0    24447 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    24098 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.6_py3.8.conda.lock
+-rw-r--r--   0        0        0    36571 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_dev_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    12291 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_lock.conda.lock
+-rw-r--r--   0        0        0    23561 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.5_py3.11.conda.lock
+-rw-r--r--   0        0        0    23214 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.5_py3.8.conda.lock
+-rw-r--r--   0        0        0    24447 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.6_py3.11.conda.lock
+-rw-r--r--   0        0        0    24098 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.6_py3.8.conda.lock
+-rw-r--r--   0        0        0     1031 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/pull_request_template.md
+-rw-r--r--   0        0        0       36 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/requirements-build.txt
+-rw-r--r--   0        0        0      258 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_atest.yml
+-rw-r--r--   0        0        0      105 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_build.yml
+-rw-r--r--   0        0        0       59 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_channels.yml
+-rw-r--r--   0        0        0       40 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_demo.yml
+-rw-r--r--   0        0        0      279 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_docs.yml
+-rw-r--r--   0        0        0       59 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_doit.yml
+-rw-r--r--   0        0        0      110 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_ext.yml
+-rw-r--r--   0        0        0      132 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_lab/lab3.5.yml
+-rw-r--r--   0        0        0       80 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_lab/lab3.6.yml
+-rw-r--r--   0        0        0      222 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_lint.yml
+-rw-r--r--   0        0        0       64 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_lint_unix.yml
+-rw-r--r--   0        0        0       54 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_lint_win.yml
+-rw-r--r--   0        0        0       48 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_nomkl.yml
+-rw-r--r--   0        0        0       38 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_py/py3.11.yml
+-rw-r--r--   0        0        0       50 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_py/py3.8.yml
+-rw-r--r--   0        0        0       36 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_release.yml
+-rw-r--r--   0        0        0      110 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_run.yml
+-rw-r--r--   0        0        0       80 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_spell.yml
+-rw-r--r--   0        0        0      184 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/_utest.yml
+-rw-r--r--   0        0        0      240 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/binder.yml
+-rw-r--r--   0        0        0      249 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/dev.yml
+-rw-r--r--   0        0        0      161 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/lock.yml
+-rw-r--r--   0        0        0      237 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/rtd.yml
+-rw-r--r--   0        0        0      150 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/specs/test.yml
+-rw-r--r--   0        0        0     1333 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/workflows/badges.yml
+-rw-r--r--   0        0        0     9014 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2531 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.github/workflows/pages.yml
+-rw-r--r--   0        0        0     2004 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.gitignore
+-rw-r--r--   0        0        0      113 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.prettierignore
+-rw-r--r--   0        0        0      349 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.readthedocs.yml
+-rw-r--r--   0        0        0      193 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/.yarnrc
+-rw-r--r--   0        0        0     5009 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0     6635 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1367 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/COPYRIGHT.md
+-rw-r--r--   0        0        0     1526 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0    11397 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/README.md
+-rw-r--r--   0        0        0     2919 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/01_Behaviors.robot
+-rw-r--r--   0        0        0     2635 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/02_Colors_ForceGraph.robot
+-rw-r--r--   0        0        0     2647 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/02_Colors_ForceGraph3D.robot
+-rw-r--r--   0        0        0     2495 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/02_Colors_GRAPH.robot.j2
+-rw-r--r--   0        0        0     2493 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/03_Events.robot
+-rw-r--r--   0        0        0     3501 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/04_Shapes_ForceGraph.robot
+-rw-r--r--   0        0        0     3529 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/04_Shapes_ForceGraph3D.robot
+-rw-r--r--   0        0        0     3130 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/04_Shapes_GRAPH.robot.j2
+-rw-r--r--   0        0        0     5956 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/05_LinkShapes_ForceGraph.robot
+-rw-r--r--   0        0        0     6004 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/05_LinkShapes_ForceGraph3D.robot
+-rw-r--r--   0        0        0     4826 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/05_LinkShapes_GRAPH.robot.j2
+-rw-r--r--   0        0        0     2581 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/06_Scales_ForceGraph.robot
+-rw-r--r--   0        0        0     2589 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/06_Scales_ForceGraph3D.robot
+-rw-r--r--   0        0        0     2587 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/06_Scales_GRAPH.robot.j2
+-rw-r--r--   0        0        0     2925 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/07_Camera_ForceGraph.robot
+-rw-r--r--   0        0        0     2929 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/07_Camera_ForceGraph3D.robot
+-rw-r--r--   0        0        0     2967 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/07_Camera_GRAPH.robot.j2
+-rw-r--r--   0        0        0      195 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/API/__init__.robot
+-rw-r--r--   0        0        0      470 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/01_Index.robot
+-rw-r--r--   0        0        0      482 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/02_Behaviors.robot
+-rw-r--r--   0        0        0      469 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/03_3D.robot
+-rw-r--r--   0        0        0      717 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/04_Force.robot
+-rw-r--r--   0        0        0      492 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/05_WidgetSource.robot
+-rw-r--r--   0        0        0      490 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/06_DodoSource.robot
+-rw-r--r--   0        0        0      481 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/07_DodoApp.robot
+-rw-r--r--   0        0        0      225 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Notebooks/__init__.robot
+-rw-r--r--   0        0        0     1643 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Regression/103_2D_Not_Text.robot
+-rw-r--r--   0        0        0     1584 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Regression/109_Director_Padding.robot
+-rw-r--r--   0        0        0      796 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Regression/90_Preserved_ID_Order.robot
+-rw-r--r--   0        0        0      226 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Regression/__init__.robot
+-rw-r--r--   0        0        0      242 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/Smoke.robot
+-rw-r--r--   0        0        0      295 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/__init__.robot
+-rw-r--r--   0        0        0      385 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_libraries/Ports.py
+-rw-r--r--   0        0        0      324 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/Camera.py
+-rw-r--r--   0        0        0      354 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/Colors.py
+-rw-r--r--   0        0        0      387 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/Event.py
+-rw-r--r--   0        0        0      585 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/GraphData.py
+-rw-r--r--   0        0        0      405 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/LinkSelection.py
+-rw-r--r--   0        0        0      772 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/LinkShapes.py
+-rw-r--r--   0        0        0      390 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/NodeSelection.py
+-rw-r--r--   0        0        0      486 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/NodeShapes.py
+-rw-r--r--   0        0        0      199 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/NodeTooltip.py
+-rw-r--r--   0        0        0      525 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/api/Scales.py
+-rw-r--r--   0        0        0      336 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/default_setting_overrides.json
+-rw-r--r--   0        0        0      151 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/jupyter_config.json
+-rw-r--r--   0        0        0      847 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/regression/gh-103.py
+-rw-r--r--   0        0        0      912 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/regression/gh-109.py
+-rw-r--r--   0        0        0     1855 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/fixtures/regression/gh-90.py
+-rw-r--r--   0        0        0      959 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Browser.robot
+-rw-r--r--   0        0        0      137 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/CLI.robot
+-rw-r--r--   0        0        0      758 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Coverage.robot
+-rw-r--r--   0        0        0     5538 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/IPyForceGraph.robot
+-rw-r--r--   0        0        0     8763 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Lab.robot
+-rw-r--r--   0        0        0      210 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Meta.robot
+-rw-r--r--   0        0        0      947 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Regression.robot
+-rw-r--r--   0        0        0      469 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Screenshots.robot
+-rw-r--r--   0        0        0     4886 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/keywords/Server.robot
+-rw-r--r--   0        0        0      149 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/variables/Browser.robot
+-rw-r--r--   0        0        0      606 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/variables/IPyForceGraph.robot
+-rw-r--r--   0        0        0     3121 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/variables/Lab.robot
+-rw-r--r--   0        0        0      150 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/atest/_resources/variables/Server.robot
+-rw-r--r--   0        0        0     2359 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/_static/anvil.svg
+-rw-r--r--   0        0        0    20274 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/_static/logo.svg
+-rw-r--r--   0        0        0      540 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/_static/theme.css
+-rw-r--r--   0        0        0    29973 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/_static/wordmark.svg
+-rw-r--r--   0        0        0       34 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/changelog.md
+-rw-r--r--   0        0        0     2597 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/conf.py
+-rw-r--r--   0        0        0       37 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/contributing.md
+-rw-r--r--   0        0        0     1355 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/dictionary.txt
+-rw-r--r--   0        0        0      908 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/environment.yml
+-rw-r--r--   0        0        0      431 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/index.md
+-rw-r--r--   0        0        0      270 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/base.md
+-rw-r--r--   0        0        0      637 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/behaviors.md
+-rw-r--r--   0        0        0      108 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/forces.md
+-rw-r--r--   0        0        0      209 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/index.md
+-rw-r--r--   0        0        0      113 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/module.md
+-rw-r--r--   0        0        0      108 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/scales.md
+-rw-r--r--   0        0        0      302 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/sources.md
+-rw-r--r--   0        0        0       98 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/docs/reference/widgets.md
+-rw-r--r--   0        0        0    26820 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/dodo.py
+-rw-r--r--   0        0        0     2816 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/3D.ipynb
+-rw-r--r--   0        0        0    33076 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Behaviors.ipynb
+-rw-r--r--   0        0        0    14674 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Camera.ipynb
+-rw-r--r--   0        0        0     1300 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/DodoApp.ipynb
+-rw-r--r--   0        0        0    34979 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/DodoSource.ipynb
+-rw-r--r--   0        0        0    31389 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Forces.ipynb
+-rw-r--r--   0        0        0     6912 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Scales.ipynb
+-rw-r--r--   0        0        0     5317 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Shapes.ipynb
+-rw-r--r--   0        0        0     6429 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Test_Behaviors.ipynb
+-rw-r--r--   0        0        0     2382 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Test_Forces.ipynb
+-rw-r--r--   0        0        0    37961 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/Utils.ipynb
+-rw-r--r--   0        0        0     5797 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/WidgetSource.ipynb
+-rw-r--r--   0        0        0     5856 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/_index.ipynb
+-rw-r--r--   0        0        0   342558 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/datasets/blocks.json
+-rw-r--r--   0        0        0    13906 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/datasets/d3-dependencies.csv
+-rw-r--r--   0        0        0     9808 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/datasets/logo.svg
+-rw-r--r--   0        0        0    19506 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/datasets/miserables.json
+-rw-r--r--   0        0        0  3566209 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/datasets/mplate.mtx
+-rw-r--r--   0        0        0      123 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/examples/requirements.txt
+-rw-r--r--   0        0        0      710 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/ignored-vulnerabilities.json
+-rw-r--r--   0        0        0      244 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/index.ts
+-rw-r--r--   0        0        0     1688 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/plugin.ts
+-rw-r--r--   0        0        0     2926 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/template-utils.ts
+-rw-r--r--   0        0        0     8968 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/tokens.ts
+-rw-r--r--   0        0        0      278 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/tsconfig.cov.json
+-rw-r--r--   0        0        0      225 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/tsconfig.json
+-rw-r--r--   0        0        0      202 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/typings.d.ts
+-rw-r--r--   0        0        0     1386 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/utils.ts
+-rw-r--r--   0        0        0     7963 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/base.ts
+-rw-r--r--   0        0        0     1420 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/dag.ts
+-rw-r--r--   0        0        0     1081 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-center.ts
+-rw-r--r--   0        0        0     3060 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-cluster.ts
+-rw-r--r--   0        0        0     1100 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-collision.ts
+-rw-r--r--   0        0        0     1118 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-link.ts
+-rw-r--r--   0        0        0     1352 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-manybody.ts
+-rw-r--r--   0        0        0     1322 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-radial.ts
+-rw-r--r--   0        0        0     1025 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-x.ts
+-rw-r--r--   0        0        0     1025 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-y.ts
+-rw-r--r--   0        0        0     1025 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-z.ts
+-rw-r--r--   0        0        0     5704 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force.ts
+-rw-r--r--   0        0        0      442 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/forces/index.ts
+-rw-r--r--   0        0        0     6974 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/graph-camera.ts
+-rw-r--r--   0        0        0     2507 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/graph-data.ts
+-rw-r--r--   0        0        0     2588 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/graph-image.ts
+-rw-r--r--   0        0        0      569 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/index.ts
+-rw-r--r--   0        0        0     1169 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/link-arrow.ts
+-rw-r--r--   0        0        0     1333 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/link-particles.ts
+-rw-r--r--   0        0        0     4340 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/link-selection.ts
+-rw-r--r--   0        0        0     1276 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/link-shape.ts
+-rw-r--r--   0        0        0      726 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/link-tooltip.ts
+-rw-r--r--   0        0        0     3065 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/node-selection.ts
+-rw-r--r--   0        0        0     2962 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/node-shape.ts
+-rw-r--r--   0        0        0      726 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/node-tooltip.ts
+-rw-r--r--   0        0        0     2845 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/scales.ts
+-rw-r--r--   0        0        0     6165 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/base.ts
+-rw-r--r--   0        0        0     1420 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/ellipse.ts
+-rw-r--r--   0        0        0      198 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/index.ts
+-rw-r--r--   0        0        0     1165 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/rectangle.ts
+-rw-r--r--   0        0        0     3801 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/text.ts
+-rw-r--r--   0        0        0    29034 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/display/2d.ts
+-rw-r--r--   0        0        0     4435 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/display/3d.ts
+-rw-r--r--   0        0        0      161 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/display/index.ts
+-rw-r--r--   0        0        0      200 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/index.ts
+-rw-r--r--   0        0        0     1361 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/serializers/dataframe.ts
+-rw-r--r--   0        0        0      172 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/serializers/index.ts
+-rw-r--r--   0        0        0      244 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/serializers/widget.ts
+-rw-r--r--   0        0        0     7376 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/sources/dataframe.ts
+-rw-r--r--   0        0        0      146 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/js/widgets/sources/index.ts
+-rw-r--r--   0        0        0      135 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/lite/jupyter-lite.json
+-rw-r--r--   0        0        0      196 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/lite/jupyter_lite_config.json
+-rw-r--r--   0        0        0     4540 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/package.json
+-rw-r--r--   0        0        0      231 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/pages-lite/jupyter_lite_config.json
+-rw-r--r--   0        0        0     3329 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/__init__.py
+-rw-r--r--   0        0        0     4136 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/atest.py
+-rw-r--r--   0        0        0     6234 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/preflight.py
+-rw-r--r--   0        0        0     9803 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/project.py
+-rw-r--r--   0        0        0     1475 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/reporter.py
+-rw-r--r--   0        0        0    14347 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/scripts/utils.py
+-rw-r--r--   0        0        0     4682 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/package.json
+-rw-r--r--   0        0        0     8813 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js
+-rw-r--r--   0        0        0    42811 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js.map
+-rw-r--r--   0        0        0      697 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js
+-rw-r--r--   0        0        0     2332 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js.map
+-rw-r--r--   0        0        0    50872 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.6f0ddabb30857eeb84da.js
+-rw-r--r--   0        0        0   183438 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.6f0ddabb30857eeb84da.js.map
+-rw-r--r--   0        0        0    28470 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js
+-rw-r--r--   0        0        0   125192 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js.map
+-rw-r--r--   0        0        0    48532 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js
+-rw-r--r--   0        0        0   203549 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js.map
+-rw-r--r--   0        0        0      329 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/228.bb390299503f7f9e929a.js
+-rw-r--r--   0        0        0      356 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/228.bb390299503f7f9e929a.js.map
+-rw-r--r--   0        0        0      329 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/271.512f94c488062f5c2b86.js
+-rw-r--r--   0        0        0      377 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/271.512f94c488062f5c2b86.js.map
+-rw-r--r--   0        0        0    96265 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js
+-rw-r--r--   0        0        0       41 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.LICENSE.txt
+-rw-r--r--   0        0        0   352279 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.map
+-rw-r--r--   0        0        0      329 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/460.761d5a8d3129bfa049b2.js
+-rw-r--r--   0        0        0      367 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/460.761d5a8d3129bfa049b2.js.map
+-rw-r--r--   0        0        0    27597 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js
+-rw-r--r--   0        0        0      225 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.LICENSE.txt
+-rw-r--r--   0        0        0   109234 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.map
+-rw-r--r--   0        0        0     1047 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js
+-rw-r--r--   0        0        0     3709 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js.map
+-rw-r--r--   0        0        0     7177 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js
+-rw-r--r--   0        0        0    22576 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js.map
+-rw-r--r--   0        0        0     7762 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js
+-rw-r--r--   0        0        0    19473 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js.map
+-rw-r--r--   0        0        0      327 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/65.e565d3630178010e411b.js
+-rw-r--r--   0        0        0      372 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/65.e565d3630178010e411b.js.map
+-rw-r--r--   0        0        0   160979 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/67fea965f2310612f9225ab29510fcff9b836e237e6f5cd8c05b266870ffd0d5.js
+-rw-r--r--   0        0        0     9063 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/6eebc3e07550540f4bcb82887a5a6da943ea90aaba205486fd1b70b8db0ccfc5.js
+-rw-r--r--   0        0        0    11098 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.bf098c4c309569651a30.js
+-rw-r--r--   0        0        0    37123 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.bf098c4c309569651a30.js.map
+-rw-r--r--   0        0        0     5943 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.15063f9dc1ad680ce392.js
+-rw-r--r--   0        0        0    12225 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.15063f9dc1ad680ce392.js.map
+-rw-r--r--   0        0        0    30158 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js
+-rw-r--r--   0        0        0    69349 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js.map
+-rw-r--r--   0        0        0   644942 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js
+-rw-r--r--   0        0        0      100 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js.LICENSE.txt
+-rw-r--r--   0        0        0   348579 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/998250a831af662f5f25.wasm
+-rw-r--r--   0        0        0   635410 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js
+-rw-r--r--   0        0        0       92 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js.LICENSE.txt
+-rw-r--r--   0        0        0     9664 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.e4b732ee5c146d5cca18.js
+-rw-r--r--   0        0        0    43533 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.e4b732ee5c146d5cca18.js.map
+-rw-r--r--   0        0        0    30447 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/third-party-licenses.json
+-rw-r--r--   0        0        0      536 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/__init__.py
+-rw-r--r--   0        0        0      724 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/_base.py
+-rw-r--r--   0        0        0      929 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/__init__.py
+-rw-r--r--   0        0        0     7633 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/_base.py
+-rw-r--r--   0        0        0    13199 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/forces.py
+-rw-r--r--   0        0        0     1294 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/particles.py
+-rw-r--r--   0        0        0     5168 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/recording.py
+-rw-r--r--   0        0        0     3314 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/scales.py
+-rw-r--r--   0        0        0     2778 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/selection.py
+-rw-r--r--   0        0        0     5068 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/shapes.py
+-rw-r--r--   0        0        0     1365 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/tooltip.py
+-rw-r--r--   0        0        0      690 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/constants.py
+-rw-r--r--   0        0        0     2740 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/graphs.py
+-rw-r--r--   0        0        0      569 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/js.py
+-rw-r--r--   0        0        0        0 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/py.typed
+-rw-r--r--   0        0        0     1610 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/serializers.py
+-rw-r--r--   0        0        0      287 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/sources/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/sources/dataframe.py
+-rw-r--r--   0        0        0    11300 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/sources/dodo.py
+-rw-r--r--   0        0        0     9476 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/sources/widget.py
+-rw-r--r--   0        0        0      108 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/conftest.py
+-rw-r--r--   0        0        0      443 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_dag_widget.py
+-rw-r--r--   0        0        0     1996 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_dodo_source.py
+-rw-r--r--   0        0        0      578 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_meta.py
+-rw-r--r--   0        0        0     1433 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_scales.py
+-rw-r--r--   0        0        0     1615 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_serializers.py
+-rw-r--r--   0        0        0     1725 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_widget_model_meta.py
+-rw-r--r--   0        0        0     1455 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_widget_source.py
+-rw-r--r--   0        0        0     1289 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/src/ipyforcegraph/trait_utils.py
+-rw-r--r--   0        0        0      930 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/style/index.css
+-rw-r--r--   0        0        0      186 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/tsconfig.json
+-rw-r--r--   0        0        0      580 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/tsconfigbase.json
+-rw-r--r--   0        0        0      493 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/webpack.config.js
+-rw-r--r--   0        0        0   239298 2023-07-07 18:06:18.000000 ipyforcegraph-0.3.6/yarn.lock
+-rw-r--r--   0        0        0    12930 1970-01-01 00:00:00.000000 ipyforcegraph-0.3.6/PKG-INFO
```

### Comparing `ipyforcegraph-0.3.5/.binder/environment.yml` & `ipyforcegraph-0.3.6/.binder/environment.yml`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.binder/postBuild` & `ipyforcegraph-0.3.6/.binder/postBuild`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/bug_report.md` & `ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/docs.md` & `ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/docs.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/feature_request.md` & `ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/ISSUE_TEMPLATE/release.md` & `ipyforcegraph-0.3.6/.github/ISSUE_TEMPLATE/release.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_dev_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_dev_lab3.6_py3.11.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
-https://conda.anaconda.org/conda-forge/linux-64/firefox-102.12.0esr-hd3aeb46_0.conda#cce3316b58d0690f018eddff121aafd0
+https://conda.anaconda.org/conda-forge/linux-64/firefox-102.13.0esr-hd3aeb46_0.conda#680a78c6f8532670d1888f92b39254a0
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
@@ -118,15 +118,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
-https://conda.anaconda.org/conda-forge/linux-64/perl-5.32.1-2_h7f98852_perl5.tar.bz2#09ba115862623f00962e9809ea248f1a
+https://conda.anaconda.org/conda-forge/linux-64/perl-5.32.1-3_hd590300_perl5.conda#53dc30c420516340641b00ec1571dd53
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/hunspell-1.7.0-h68659b9_1001.tar.bz2#598373baf2b216b5418846df7cceeb13
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
@@ -136,15 +136,14 @@
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libxslt-1.1.37-h0054252_1.conda#f27960e8873abb5476e96ef33bdbdccd
 https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
@@ -153,33 +152,33 @@
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py311h38be061_1.tar.bz2#599159b0740e9b82e7eef0e8471be3c2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/future-0.18.3-pyhd8ed1ab_0.conda#fec8329fc739090f26a7d7803db254f1
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py311hb755f60_1.conda#82f9885f18cc7ba9bca6687ac97f1d65
 https://conda.anaconda.org/conda-forge/noarch/hunspell-en-2023.01.01-hd8ed1ab_0.conda#ee22bd6d6a07b0ad4981c79bbbde52a8
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/itsdangerous-2.1.2-pyhd8ed1ab_0.tar.bz2#3c3de74912f11d2b590184f03c7cd09b
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
-https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.2-py311h1a07684_1.conda#22b4fb083a8262c0b4e135c86a2c0c99
+https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.3-py311h1a07684_0.conda#59a580306d62ef144c9dd592b5120f36
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py311ha3edf6b_0.conda#7415f24f8c44e44152623d93c5015000
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
@@ -214,15 +213,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.0.275-py311h7145743_0.conda#23187227d6a05fbc2139499107faeebb
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.0.276-py311h7145743_0.conda#1f5f6036a09d54863f8547d76079176e
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
@@ -241,21 +240,21 @@
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/noarch/types-docutils-0.20.0.1-pyhd8ed1ab_0.conda#113839f783e42733ec5cb243989ef9f1
 https://conda.anaconda.org/conda-forge/noarch/types-pyyaml-5.4.12-pyhd8ed1ab_0.tar.bz2#efd73a6664edb11d09c52fb05356f0bf
 https://conda.anaconda.org/conda-forge/noarch/types-urllib3-1.26.25.13-pyhd8ed1ab_0.conda#9a73576dfe2f764c431347b9dc35a3fc
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/ujson-5.7.0-py311hcafe171_0.conda#ec3960b6d13bb60aad9c67f42a801720
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py311hfe55011_0.conda#216fb67bd1016b05fe33672bd71937a8
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/linux-64/ansi2html-1.8.0-py311h38be061_1.tar.bz2#5ce42a68e90f54266ad06ac13b773ef1
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/autopep8-2.0.2-pyhd8ed1ab_0.conda#e21ecb8bff82ba3bb589904ca97582b6
@@ -285,30 +284,30 @@
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pip-requirements-parser-32.0.1-pyhd8ed1ab_0.conda#a0efd67d53ab8c20c6020aa40e55bc15
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pyfiglet-0.8.post1-py_0.tar.bz2#e22d3c090f24856764e9d70e76fa3a5f
-https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.12.1-pyhd8ed1ab_0.conda#7abe4ac9f532e2ed024cd08ff69edde1
+https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.13.0-pyhd8ed1ab_0.conda#30bf5ee7d6bf0a7a7eb79685b456ad1c
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
 https://conda.anaconda.org/conda-forge/noarch/types-requests-2.31.0.1-pyhd8ed1ab_0.conda#d4edae6cf0af5332243c2d995f5e8745
-https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.0-pyhd8ed1ab_0.conda#fb341d4f1631592d3ab7360e2e9201c3
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.1-pyhd8ed1ab_0.conda#a44efd4003609542c549f8737b97fa9a
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/url-normalize-1.4.3-pyhd8ed1ab_0.tar.bz2#7c4076e494f0efe76705154ac9302ba6
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
 https://conda.anaconda.org/conda-forge/linux-64/cmarkgfm-0.8.0-py311hd4cff14_2.tar.bz2#ed1a2dba3b53fcd450f2fe867af0ba3f
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py311h63ff55d_0.conda#69ad01f66b8efff535d341ba5b283c2c
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-python-lib-3.1.5-pyhd8ed1ab_0.conda#c979eaff5759cb6c8c91369b0ada1abc
@@ -326,65 +325,65 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-10.16.2-pyhd8ed1ab_0.tar.bz2#06b0afa55cd119e243aea39b037c94ce
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.17-py311h459d7ec_0.conda#40840325f6415f6072b93c5750c8e527
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.1-py311h38be061_0.conda#a3b7b73e6929e60a3cd85c6640fcbeaa
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/linux-64/black-23.3.0-py311h38be061_1.conda#b0d621848bfba5aacbdfc43dfdeabfec
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-bom-3.11.0-pyhd8ed1ab_0.conda#fa8a12276f6186783d375a4dff5160a2
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/noarch/ossindex-lib-1.1.1-pyhd8ed1ab_0.tar.bz2#11718ae7e5d0bd9987636caf9a58b968
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
-https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.0.1-pyhd8ed1ab_0.conda#43ec7b3627237e5fe23413e314e8ba4c
+https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.1.0-pyhd8ed1ab_0.conda#57b89064c125bb9d0e533e018c3eb17a
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py311h38be061_1.tar.bz2#ec745aaae03cc47120c1f11ac7b7bcf5
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/autodoc-traits-1.1.0-pyhd8ed1ab_0.conda#66907045fcff46748e485201304cea80
 https://conda.anaconda.org/conda-forge/noarch/jake-3.0.1-pyhd8ed1ab_0.conda#f719c7a0825a40e8032d071d2a47d9aa
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/jupyterlite-core-0.1.0-pyhd8ed1ab_0.conda#c848221f9bd434fb89fa992214e5e64a
 https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py311h38be061_0.conda#b8eedb6181eff2dfeb34182330db1240
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autodoc-typehints-1.21.8-pyhd8ed1ab_0.conda#21e2e0ea045848dcb0053b6cc67a7f7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/jupyterlite-core-with-libarchive-0.1.0-pyhd8ed1ab_0.conda#3f852a733a6553ff1ad52e82be0c2a95
 https://conda.anaconda.org/conda-forge/noarch/jupyterlite-pyodide-kernel-0.0.8-pyhd8ed1ab_0.conda#69de51ba70120084be1f6991020fa297
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/noarch/nbstripout-0.6.1-pyhd8ed1ab_0.tar.bz2#53913d98739527409e0f3227ed7eef7d
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/twine-3.8.0-pyhd8ed1ab_0.tar.bz2#5d3c0f63166e57c20516b6fc2c1d1115
 https://conda.anaconda.org/conda-forge/noarch/black-jupyter-23.3.0-hd8ed1ab_1.conda#62cc29ee11300ae8a587ff6396e78b62
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/nbqa-1.7.0-pyhd8ed1ab_1.conda#65da1779c33b7fa51a0aba5c30758c5e
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_lock.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_lock.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -85,45 +85,47 @@
 https://conda.anaconda.org/conda-forge/linux-64/ruamel_yaml-0.15.80-py311hd4cff14_1008.tar.bz2#cfc7aa9d4e13c267fb6531d4788f2ede
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.4.5-h658169a_0.conda#30f234e9bb2cc1b549b508af79299129
+https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.4.6-h658169a_0.conda#a1a020a8c1a487bbf774fb8e7f1dc047
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py311h459d7ec_0.conda#628868dc17f9bd39a2eb77846e35980c
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py311hd4cff14_1005.tar.bz2#9bdac7084ecfc08338bae1b976535724
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py311h63ff55d_0.conda#69ad01f66b8efff535d341ba5b283c2c
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
-https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.4.5-py311h527f279_0.conda#be887339ca5be1b148578ed1a9e21316
+https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.4.6-py311h527f279_0.conda#febaca29e4186f0d0a1456dbd8c0e1fa
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.9-py311h459d7ec_0.conda#1d8d643ba4e4fcf3e95ce787261798da
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.0.2-py311h46250e7_0.conda#560d9cba6cd30c12baca52f873ca869d
 https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py311haa97af0_2.conda#10b11630d87e0a1d4abce705bc4e0b55
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-2.0.1-py311h459d7ec_2.conda#00875831566ce1cd5d101057ae646d5e
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py311h38be061_1.tar.bz2#ec745aaae03cc47120c1f11ac7b7bcf5
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
 https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py311h38be061_0.conda#b8eedb6181eff2dfeb34182330db1240
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/linux-64/conda-22.9.0-py311h38be061_2.tar.bz2#d083486f8b405adad834ba22b9cd7340
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
-https://conda.anaconda.org/conda-forge/linux-64/mamba-1.4.5-py311h3072747_0.conda#af2bc0b6f7d9f1dc1712f8cdef59147b
+https://conda.anaconda.org/conda-forge/linux-64/mamba-1.4.6-py311h3072747_0.conda#837d044a4d01f0964d1531555eda876f
 https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.5_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.5_py3.11.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-102.12.0esr-hd3aeb46_0.conda#cce3316b58d0690f018eddff121aafd0
+https://conda.anaconda.org/conda-forge/linux-64/firefox-102.13.0esr-hd3aeb46_0.conda#680a78c6f8532670d1888f92b39254a0
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
@@ -74,40 +74,39 @@
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libxslt-1.1.37-h0054252_1.conda#f27960e8873abb5476e96ef33bdbdccd
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
-https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.2-py311h1a07684_1.conda#22b4fb083a8262c0b4e135c86a2c0c99
+https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.3-py311h1a07684_0.conda#59a580306d62ef144c9dd592b5120f36
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py311ha3edf6b_0.conda#7415f24f8c44e44152623d93c5015000
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
@@ -142,20 +141,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
@@ -182,15 +181,15 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/linux-64/pandas-2.0.3-py311h320fe9a_0.conda#c9308b00067b8aa10893cb020bc39627
@@ -200,29 +199,29 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.1-py311h38be061_0.conda#a3b7b73e6929e60a3cd85c6640fcbeaa
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.3-pyh210e3f2_0.conda#8c1f6bf32a6ca81232c4853d4165ca67
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.5_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.6_py3.8.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # channels:
 #   - conda-forge
 #   - nodefaults
 # dependencies:
-#   - comm <0.1.3
 #   - conda-forge/label/robotframework_jupyterlibrary_alpha::robotframework-jupyterlibrary
 #     >=0.5.0a0
 #   - doit-with-toml
 #   - firefox =102
 #   - geckodriver
 #   - importnb
 #   - ipydatagrid
-#   - ipykernel <6.22.0
 #   - ipylab >=0.7.0
-#   - ipywidgets <8.0.5
 #   - ipywidgets >=8.0.0
-#   - jupyterlab >=3.5.2,<3.6
-#   - jupyterlab_widgets <3.0.6
+#   - jupyter_server >=2.2.1
+#   - jupyterlab >=3.6.4,<3.7
 #   - lxml
 #   - networkx
 #   - numcodecs
+#   - orjson
 #   - pandas
 #   - pandas <2
 #   - pip
 #   - pytest-asyncio
 #   - pytest-cov
 #   - pytest-html
 #   - pytest-json-report
@@ -46,15 +44,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-102.12.0esr-hd3aeb46_0.conda#cce3316b58d0690f018eddff121aafd0
+https://conda.anaconda.org/conda-forge/linux-64/firefox-102.13.0esr-hd3aeb46_0.conda#680a78c6f8532670d1888f92b39254a0
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
@@ -73,48 +71,49 @@
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libxslt-1.1.37-h0054252_1.conda#f27960e8873abb5476e96ef33bdbdccd
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
-https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.2-py38h0ef1326_1.conda#240c6945ec3b4d4144d1c01c9a968926
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
+https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.3-py38h0ef1326_0.conda#f9b8c58aade85e2f76ae31c832dbcb9c
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
+https://conda.anaconda.org/conda-forge/linux-64/orjson-3.9.1-py38h0488081_0.conda#22bfe5916c3e3077d928a54e65757ca6
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
@@ -140,29 +139,30 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py38h9fda977_0.conda#18517ed6c99222252a7409b9e128015c
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.2-pyhd8ed1ab_0.conda#3c78af4752bb1600ebe5e83ef4588eaa
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
@@ -180,16 +180,17 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
@@ -198,42 +199,46 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py38h578d9bd_1.tar.bz2#111c35cf763a092d1f7f6a4db462de69
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.1-py38h578d9bd_0.conda#9c8b384dc98e143a8a751ff8d5191c11
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyh41d4057_0.conda#acebfd89278ecac2a67b60b657e00d5c
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.3-pyh210e3f2_0.conda#8c1f6bf32a6ca81232c4853d4165ca67
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.4-pyhd8ed1ab_0.conda#9dea5ab3cc33084f7a3680a98859731e
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/ipydatagrid-1.1.16-pyhd8ed1ab_0.conda#0fbc366d2693efe3d34c76b484064549
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.5_py3.8.conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # channels:
 #   - conda-forge
 #   - nodefaults
 # dependencies:
+#   - comm <0.1.3
 #   - conda-forge/label/robotframework_jupyterlibrary_alpha::robotframework-jupyterlibrary
 #     >=0.5.0a0
 #   - doit-with-toml
 #   - firefox =102
 #   - geckodriver
 #   - importnb
 #   - ipydatagrid
+#   - ipykernel <6.22.0
 #   - ipylab >=0.7.0
+#   - ipywidgets <8.0.5
 #   - ipywidgets >=8.0.0
-#   - jupyter_server >=2.2.1
-#   - jupyterlab >=3.6.4,<3.7
+#   - jupyterlab >=3.5.2,<3.6
+#   - jupyterlab_widgets <3.0.6
 #   - lxml
 #   - networkx
 #   - numcodecs
-#   - orjson
 #   - pandas
+#   - pandas <2
 #   - pip
 #   - pytest-asyncio
 #   - pytest-cov
 #   - pytest-html
 #   - pytest-json-report
 #   - pytest-xdist
-#   - python >=3.11,<3.12
 #   - python >=3.8,<3.12
+#   - python >=3.8,<3.9
 #   - python-dotenv
 #   - robotframework-pabot
 #   - robotframework-robocop
 #   - robotframework-tidy >=3.4.0
 #   - scour
 #   - selenium <4.10.0
 #   - tomli
@@ -37,26 +40,24 @@
 
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.1.0-h15d22d2_0.conda#afb656a334c409dd9805508af1c89c7a
 https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-102.12.0esr-hd3aeb46_0.conda#cce3316b58d0690f018eddff121aafd0
+https://conda.anaconda.org/conda-forge/linux-64/firefox-102.13.0esr-hd3aeb46_0.conda#680a78c6f8532670d1888f92b39254a0
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
@@ -71,111 +72,106 @@
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libxslt-1.1.37-h0054252_1.conda#f27960e8873abb5476e96ef33bdbdccd
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
-https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
-https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.2-py311h1a07684_1.conda#22b4fb083a8262c0b4e135c86a2c0c99
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
+https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.3-py38h0ef1326_0.conda#f9b8c58aade85e2f76ae31c832dbcb9c
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py311ha3edf6b_0.conda#7415f24f8c44e44152623d93c5015000
+https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py311h64a7726_0.conda#4df60430eca64502eb01e02df92246bf
-https://conda.anaconda.org/conda-forge/linux-64/orjson-3.9.1-py311h34b1e23_0.conda#1ddc29665d5dbcc5b3e9dbb13e9a8097
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
-https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
-https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py311hfe55011_0.conda#216fb67bd1016b05fe33672bd71937a8
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py311h459d7ec_0.conda#3c2c65575c28b23afc5e4ff721a2fc9f
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.2-pyhd8ed1ab_0.conda#3c78af4752bb1600ebe5e83ef4588eaa
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/linux-64/numcodecs-0.11.0-py311hcafe171_1.conda#ecdaf0772e524ed51218f6d52ef74424
+https://conda.anaconda.org/conda-forge/linux-64/numcodecs-0.11.0-py38h8dc9893_1.conda#3258076e23cb8c8760e0546bcf2a4605
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
@@ -183,65 +179,60 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
-https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.0.3-py311h320fe9a_0.conda#c9308b00067b8aa10893cb020bc39627
+https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.0-pyhd8ed1ab_0.conda#87d7a2fa554e3ccdfb2eb69b460aa3a5
 https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.1-py38h578d9bd_0.conda#9c8b384dc98e143a8a751ff8d5191c11
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyh41d4057_0.conda#acebfd89278ecac2a67b60b657e00d5c
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.3-pyh210e3f2_0.conda#8c1f6bf32a6ca81232c4853d4165ca67
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.4-pyhd8ed1ab_0.conda#9dea5ab3cc33084f7a3680a98859731e
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/ipydatagrid-1.1.16-pyhd8ed1ab_0.conda#0fbc366d2693efe3d34c76b484064549
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/linux-64_test_lab3.6_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/linux-64_test_lab3.6_py3.11.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 #   - jupyter_server >=2.2.1
 #   - jupyterlab >=3.6.4,<3.7
 #   - lxml
 #   - networkx
 #   - numcodecs
 #   - orjson
 #   - pandas
-#   - pandas <2
 #   - pip
 #   - pytest-asyncio
 #   - pytest-cov
 #   - pytest-html
 #   - pytest-json-report
 #   - pytest-xdist
+#   - python >=3.11,<3.12
 #   - python >=3.8,<3.12
-#   - python >=3.8,<3.9
 #   - python-dotenv
 #   - robotframework-pabot
 #   - robotframework-robocop
 #   - robotframework-tidy >=3.4.0
 #   - scour
 #   - selenium <4.10.0
 #   - tomli
@@ -38,24 +37,26 @@
 
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.1.0-h15d22d2_0.conda#afb656a334c409dd9805508af1c89c7a
 https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-102.12.0esr-hd3aeb46_0.conda#cce3316b58d0690f018eddff121aafd0
+https://conda.anaconda.org/conda-forge/linux-64/firefox-102.13.0esr-hd3aeb46_0.conda#680a78c6f8532670d1888f92b39254a0
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
@@ -70,110 +71,110 @@
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libxslt-1.1.37-h0054252_1.conda#f27960e8873abb5476e96ef33bdbdccd
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
-https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.2-py38h0ef1326_1.conda#240c6945ec3b4d4144d1c01c9a968926
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
+https://conda.anaconda.org/conda-forge/linux-64/lxml-4.9.3-py311h1a07684_0.conda#59a580306d62ef144c9dd592b5120f36
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
+https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py311ha3edf6b_0.conda#7415f24f8c44e44152623d93c5015000
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
-https://conda.anaconda.org/conda-forge/linux-64/orjson-3.9.1-py38h0488081_0.conda#22bfe5916c3e3077d928a54e65757ca6
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py311h64a7726_0.conda#4df60430eca64502eb01e02df92246bf
+https://conda.anaconda.org/conda-forge/linux-64/orjson-3.9.1-py311h34b1e23_0.conda#1ddc29665d5dbcc5b3e9dbb13e9a8097
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
-https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py38h9fda977_0.conda#18517ed6c99222252a7409b9e128015c
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py311hfe55011_0.conda#216fb67bd1016b05fe33672bd71937a8
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py311h459d7ec_0.conda#3c2c65575c28b23afc5e4ff721a2fc9f
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/linux-64/numcodecs-0.11.0-py38h8dc9893_1.conda#3258076e23cb8c8760e0546bcf2a4605
+https://conda.anaconda.org/conda-forge/linux-64/numcodecs-0.11.0-py311hcafe171_1.conda#ecdaf0772e524ed51218f6d52ef74424
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
@@ -181,59 +182,59 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.0.3-py311h320fe9a_0.conda#c9308b00067b8aa10893cb020bc39627
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.0-pyhd8ed1ab_0.conda#87d7a2fa554e3ccdfb2eb69b460aa3a5
 https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.1.0-pyhd8ed1ab_0.conda#06eb685a3a0b146347a58dda979485da
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py38h578d9bd_1.tar.bz2#111c35cf763a092d1f7f6a4db462de69
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.1-py311h38be061_0.conda#a3b7b73e6929e60a3cd85c6640fcbeaa
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyh41d4057_0.conda#acebfd89278ecac2a67b60b657e00d5c
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_dev_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_dev_lab3.6_py3.11.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,20 @@
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/lzo-2.10-haf1e3a3_1000.tar.bz2#0b6bca372a95d6c602c7a922e928ce79
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
-https://conda.anaconda.org/conda-forge/osx-64/perl-5.32.1-2_h0d85af4_perl5.tar.bz2#dd13a8c2fac0cd8e102fcdc7bca1f077
+https://conda.anaconda.org/conda-forge/osx-64/perl-5.32.1-3_h0dc2134_perl5.conda#2859377d4bf9b56ee085c77233814e44
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-102.12.0esr-he965462_0.conda#84e8cfb7df60142d05ef4662ba3f9973
+https://conda.anaconda.org/conda-forge/osx-64/firefox-102.13.0esr-he965462_0.conda#f6854bcb5fd99ce1b8e70f987e23e7c0
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
 https://conda.anaconda.org/conda-forge/osx-64/gettext-0.21.1-h8a4c099_0.tar.bz2#1e3aff29ce703d421c43f371ad676cc5
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
@@ -123,15 +123,14 @@
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libxslt-1.1.37-h20bfa82_1.conda#177817e2ba32a7d5ffdfbcb876fd4f10
 https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
 https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
@@ -139,33 +138,33 @@
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py311h6eed73b_1.tar.bz2#268664c5447607a94cd67a0be91f83cd
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/future-0.18.3-pyhd8ed1ab_0.conda#fec8329fc739090f26a7d7803db254f1
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py311hdf8f085_1.conda#58ebad2ba8dc2225237ebd7d7c3111d2
 https://conda.anaconda.org/conda-forge/noarch/hunspell-en-2023.01.01-hd8ed1ab_0.conda#ee22bd6d6a07b0ad4981c79bbbde52a8
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/itsdangerous-2.1.2-pyhd8ed1ab_0.tar.bz2#3c3de74912f11d2b590184f03c7cd09b
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.2-py311h19a211c_1.conda#3e040f6919f0ea959045fae0a718cade
+https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.3-py311h19a211c_0.conda#35de207a04d98dad952b1c7c9d7a8a9c
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py311hd2070f0_0.conda#d3a60c5422b7d61b2740c7c5df508c86
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
@@ -199,15 +198,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/osx-64/ruff-0.0.275-py311hbf57787_0.conda#cfef93230647f6ae38389edbd9ef1663
+https://conda.anaconda.org/conda-forge/osx-64/ruff-0.0.276-py311hbf57787_0.conda#dcff0b8769fee9267786e2dc3fb21609
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
@@ -225,21 +224,21 @@
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/noarch/types-docutils-0.20.0.1-pyhd8ed1ab_0.conda#113839f783e42733ec5cb243989ef9f1
 https://conda.anaconda.org/conda-forge/noarch/types-pyyaml-5.4.12-pyhd8ed1ab_0.tar.bz2#efd73a6664edb11d09c52fb05356f0bf
 https://conda.anaconda.org/conda-forge/noarch/types-urllib3-1.26.25.13-pyhd8ed1ab_0.conda#9a73576dfe2f764c431347b9dc35a3fc
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/ujson-5.7.0-py311h814d153_0.conda#85ba096ace69a6474493ec4d4d2c15c8
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py311h890d03e_0.conda#d333683779e7145d5fe8bb18e08a7623
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/osx-64/ansi2html-1.8.0-py311h6eed73b_1.tar.bz2#f38cdc0af433fdbe1765af0fefcbb187
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/autopep8-2.0.2-pyhd8ed1ab_0.conda#e21ecb8bff82ba3bb589904ca97582b6
@@ -270,30 +269,30 @@
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pip-requirements-parser-32.0.1-pyhd8ed1ab_0.conda#a0efd67d53ab8c20c6020aa40e55bc15
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pyfiglet-0.8.post1-py_0.tar.bz2#e22d3c090f24856764e9d70e76fa3a5f
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py311hf110eff_0.conda#460e6d2c254ec4aa4299cd9bffa3b7f8
-https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.12.1-pyhd8ed1ab_0.conda#7abe4ac9f532e2ed024cd08ff69edde1
+https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.13.0-pyhd8ed1ab_0.conda#30bf5ee7d6bf0a7a7eb79685b456ad1c
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
 https://conda.anaconda.org/conda-forge/noarch/types-requests-2.31.0.1-pyhd8ed1ab_0.conda#d4edae6cf0af5332243c2d995f5e8745
-https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.0-pyhd8ed1ab_0.conda#fb341d4f1631592d3ab7360e2e9201c3
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.1-pyhd8ed1ab_0.conda#a44efd4003609542c549f8737b97fa9a
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/url-normalize-1.4.3-pyhd8ed1ab_0.tar.bz2#7c4076e494f0efe76705154ac9302ba6
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
 https://conda.anaconda.org/conda-forge/osx-64/cmarkgfm-0.8.0-py311h5547dcb_2.tar.bz2#69cd422f24f98fb4f8a9a896798bff06
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-python-lib-3.1.5-pyhd8ed1ab_0.conda#c979eaff5759cb6c8c91369b0ada1abc
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
@@ -312,48 +311,48 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-10.16.2-pyhd8ed1ab_0.tar.bz2#06b0afa55cd119e243aea39b037c94ce
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.17-py311h2725bcf_0.conda#39426e541ffaa328cd89feb4e1cc6837
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.1-py311h6eed73b_0.conda#106669bc77d8ab47dbc08178acd3d904
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/osx-64/black-23.3.0-py311h6eed73b_1.conda#2783c68e84c0573fece0880488c7c001
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-bom-3.11.0-pyhd8ed1ab_0.conda#fa8a12276f6186783d375a4dff5160a2
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py311h6eed73b_0.conda#8ba03d96e54958cd02110dc032d0bda2
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py311hc44ba51_0.conda#11037145324619832869a29d0b21f66f
 https://conda.anaconda.org/conda-forge/noarch/ossindex-lib-1.1.1-pyhd8ed1ab_0.tar.bz2#11718ae7e5d0bd9987636caf9a58b968
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
-https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.0.1-pyhd8ed1ab_0.conda#43ec7b3627237e5fe23413e314e8ba4c
+https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.1.0-pyhd8ed1ab_0.conda#57b89064c125bb9d0e533e018c3eb17a
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/autodoc-traits-1.1.0-pyhd8ed1ab_0.conda#66907045fcff46748e485201304cea80
 https://conda.anaconda.org/conda-forge/noarch/jake-3.0.1-pyhd8ed1ab_0.conda#f719c7a0825a40e8032d071d2a47d9aa
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/jupyterlite-core-0.1.0-pyhd8ed1ab_0.conda#c848221f9bd434fb89fa992214e5e64a
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/numcodecs-0.11.0-py311h814d153_1.conda#21f2ae35161c19b8c4ad0791d12ef2a3
 https://conda.anaconda.org/conda-forge/osx-64/pandas-2.0.3-py311hab14417_0.conda#f9dddf66591e316635e4a8541a4ed385
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autodoc-typehints-1.21.8-pyhd8ed1ab_0.conda#21e2e0ea045848dcb0053b6cc67a7f7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/twine-3.8.0-pyhd8ed1ab_0.tar.bz2#5d3c0f63166e57c20516b6fc2c1d1115
@@ -365,15 +364,15 @@
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/black-jupyter-23.3.0-hd8ed1ab_1.conda#62cc29ee11300ae8a587ff6396e78b62
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/nbqa-1.7.0-pyhd8ed1ab_1.conda#65da1779c33b7fa51a0aba5c30758c5e
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_lock.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_lock.conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -71,44 +71,46 @@
 https://conda.anaconda.org/conda-forge/osx-64/ruamel_yaml-0.15.80-py311h5547dcb_1008.tar.bz2#42c63993b1aaba9dc3c69a36e368d11c
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.4.5-hc2ec11d_0.conda#358888c03c6b8e5011e7a8a64b6a7dba
+https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.4.6-hc2ec11d_0.conda#6e2b1fefb504393436ec7d3be220e0d2
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py311h2725bcf_0.conda#c5c5f7cf4ca556cfdb605e05cfbc8bec
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py311h5547dcb_1005.tar.bz2#5f97ac938a90d06eebea42c321abe0d7
 https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py311h892b619_0.conda#d1e57a1ae104a8d97fd68c4d61c26323
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
-https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.4.5-py311h266e549_0.conda#b4720520ef4cf48254ed79177252fac5
+https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.4.6-py311h266e549_0.conda#4383ae4b27cac8bd235603c8442bf83c
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.9-py311h2725bcf_0.conda#c6e744d388e4de3c75aa3b00b102503c
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.0.2-py311h299eb51_0.conda#e93eef8c040d5f0dedce073e48260b76
 https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py311h26cfcfc_2.conda#864dbcdc4f7a00fee5a84d4655bc4799
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py311h6eed73b_0.conda#8ba03d96e54958cd02110dc032d0bda2
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-2.0.1-py311h2725bcf_2.conda#cda3e5a4f7d6cb5a305e2596304ab136
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/osx-64/conda-22.9.0-py311h6eed73b_2.tar.bz2#d18ef2c39925384887a22371e00b1160
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
-https://conda.anaconda.org/conda-forge/osx-64/mamba-1.4.5-py311h8082e30_0.conda#f64d7a16fd4584df5f38fa786dc29e19
+https://conda.anaconda.org/conda-forge/osx-64/mamba-1.4.6-py311h8082e30_0.conda#ff7a66b24a0c3f1b3c84dd622c823d5e
 https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.5_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.6_py3.11.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # channels:
 #   - conda-forge
 #   - nodefaults
 # dependencies:
-#   - comm <0.1.3
 #   - conda-forge/label/robotframework_jupyterlibrary_alpha::robotframework-jupyterlibrary
 #     >=0.5.0a0
 #   - doit-with-toml
 #   - firefox =102
 #   - geckodriver
 #   - importnb
 #   - ipydatagrid
-#   - ipykernel <6.22.0
 #   - ipylab >=0.7.0
-#   - ipywidgets <8.0.5
 #   - ipywidgets >=8.0.0
-#   - jupyterlab >=3.5.2,<3.6
-#   - jupyterlab_widgets <3.0.6
+#   - jupyter_server >=2.2.1
+#   - jupyterlab >=3.6.4,<3.7
 #   - lxml
 #   - networkx
 #   - numcodecs
+#   - orjson
 #   - pandas
 #   - pip
 #   - pytest-asyncio
 #   - pytest-cov
 #   - pytest-html
 #   - pytest-json-report
 #   - pytest-xdist
@@ -49,62 +47,63 @@
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-102.12.0esr-he965462_0.conda#84e8cfb7df60142d05ef4662ba3f9973
+https://conda.anaconda.org/conda-forge/osx-64/firefox-102.13.0esr-he965462_0.conda#f6854bcb5fd99ce1b8e70f987e23e7c0
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libxslt-1.1.37-h20bfa82_1.conda#177817e2ba32a7d5ffdfbcb876fd4f10
 https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.2-py311h19a211c_1.conda#3e040f6919f0ea959045fae0a718cade
+https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.3-py311h19a211c_0.conda#35de207a04d98dad952b1c7c9d7a8a9c
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py311hd2070f0_0.conda#d3a60c5422b7d61b2740c7c5df508c86
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
+https://conda.anaconda.org/conda-forge/osx-64/orjson-3.9.1-py311h52ff4d3_0.conda#09614329aa9f9d770954332c1e106b3b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
@@ -130,29 +129,30 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py311h890d03e_0.conda#d333683779e7145d5fe8bb18e08a7623
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.2-pyhd8ed1ab_0.conda#3c78af4752bb1600ebe5e83ef4588eaa
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
@@ -171,16 +171,17 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
@@ -191,46 +192,50 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.1-py311h6eed73b_0.conda#106669bc77d8ab47dbc08178acd3d904
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py311hc44ba51_0.conda#11037145324619832869a29d0b21f66f
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/numcodecs-0.11.0-py311h814d153_1.conda#21f2ae35161c19b8c4ad0791d12ef2a3
 https://conda.anaconda.org/conda-forge/osx-64/pandas-2.0.3-py311hab14417_0.conda#f9dddf66591e316635e4a8541a4ed385
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.2-pyh736e0ef_0.conda#aa43ffb10a39d9eb2538761a3f838a87
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.4-pyhd8ed1ab_0.conda#9dea5ab3cc33084f7a3680a98859731e
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/ipydatagrid-1.1.16-pyhd8ed1ab_0.conda#0fbc366d2693efe3d34c76b484064549
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.5_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.5_py3.8.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -48,55 +48,54 @@
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-102.12.0esr-he965462_0.conda#84e8cfb7df60142d05ef4662ba3f9973
+https://conda.anaconda.org/conda-forge/osx-64/firefox-102.13.0esr-he965462_0.conda#f6854bcb5fd99ce1b8e70f987e23e7c0
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libxslt-1.1.37-h20bfa82_1.conda#177817e2ba32a7d5ffdfbcb876fd4f10
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.2-py38h2d3ed51_1.conda#a7d62467d0bb0dae259d6a9a1f122c3a
+https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.3-py38h2d3ed51_0.conda#69ae6108e1c1eff9182225eddb9d8bf4
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py38h98b9b1b_0.conda#c8dc8bd685921ea63ba672f4ae018f06
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
@@ -128,20 +127,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
@@ -169,15 +168,15 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
@@ -189,33 +188,33 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py38h50d1736_1.tar.bz2#10df625ea09ec9693735cd0385a52a27
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.1-py38h50d1736_0.conda#c1c83c14b527740467a4376c27a561ef
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/numcodecs-0.11.0-py38h4cd09af_1.conda#6fc938c31040ef364277ad4d52e54302
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyhd1c38e8_0.conda#acc618532cbc899f5721cc96407b16cc
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.2-pyh736e0ef_0.conda#aa43ffb10a39d9eb2538761a3f838a87
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.5_py3.11.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # channels:
 #   - conda-forge
 #   - nodefaults
 # dependencies:
+#   - comm <0.1.3
 #   - conda-forge/label/robotframework_jupyterlibrary_alpha::robotframework-jupyterlibrary
 #     >=0.5.0a0
 #   - doit-with-toml
 #   - firefox =102
 #   - geckodriver
 #   - importnb
 #   - ipydatagrid
+#   - ipykernel <6.22.0
 #   - ipylab >=0.7.0
+#   - ipywidgets <8.0.5
 #   - ipywidgets >=8.0.0
-#   - jupyter_server >=2.2.1
-#   - jupyterlab >=3.6.4,<3.7
+#   - jupyterlab >=3.5.2,<3.6
+#   - jupyterlab_widgets <3.0.6
 #   - lxml
 #   - networkx
 #   - numcodecs
-#   - orjson
 #   - pandas
 #   - pip
 #   - pytest-asyncio
 #   - pytest-cov
 #   - pytest-html
 #   - pytest-json-report
 #   - pytest-xdist
@@ -47,64 +49,61 @@
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-102.12.0esr-he965462_0.conda#84e8cfb7df60142d05ef4662ba3f9973
+https://conda.anaconda.org/conda-forge/osx-64/firefox-102.13.0esr-he965462_0.conda#f6854bcb5fd99ce1b8e70f987e23e7c0
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libxslt-1.1.37-h20bfa82_1.conda#177817e2ba32a7d5ffdfbcb876fd4f10
 https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
-https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.2-py311h19a211c_1.conda#3e040f6919f0ea959045fae0a718cade
+https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.3-py311h19a211c_0.conda#35de207a04d98dad952b1c7c9d7a8a9c
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py311hd2070f0_0.conda#d3a60c5422b7d61b2740c7c5df508c86
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
-https://conda.anaconda.org/conda-forge/osx-64/orjson-3.9.1-py311h52ff4d3_0.conda#09614329aa9f9d770954332c1e106b3b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
@@ -130,30 +129,29 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
-https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py311h890d03e_0.conda#d333683779e7145d5fe8bb18e08a7623
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.2-pyhd8ed1ab_0.conda#3c78af4752bb1600ebe5e83ef4588eaa
 https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
@@ -172,17 +170,16 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
-https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
@@ -193,50 +190,46 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.1-py311h6eed73b_0.conda#106669bc77d8ab47dbc08178acd3d904
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py311hc44ba51_0.conda#11037145324619832869a29d0b21f66f
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/numcodecs-0.11.0-py311h814d153_1.conda#21f2ae35161c19b8c4ad0791d12ef2a3
 https://conda.anaconda.org/conda-forge/osx-64/pandas-2.0.3-py311hab14417_0.conda#f9dddf66591e316635e4a8541a4ed385
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.2-pyh736e0ef_0.conda#aa43ffb10a39d9eb2538761a3f838a87
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.4-pyhd8ed1ab_0.conda#9dea5ab3cc33084f7a3680a98859731e
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/ipydatagrid-1.1.16-pyhd8ed1ab_0.conda#0fbc366d2693efe3d34c76b484064549
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/osx-64_test_lab3.6_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/osx-64_test_lab3.6_py3.8.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -46,56 +46,55 @@
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-102.12.0esr-he965462_0.conda#84e8cfb7df60142d05ef4662ba3f9973
+https://conda.anaconda.org/conda-forge/osx-64/firefox-102.13.0esr-he965462_0.conda#f6854bcb5fd99ce1b8e70f987e23e7c0
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libxslt-1.1.37-h20bfa82_1.conda#177817e2ba32a7d5ffdfbcb876fd4f10
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.2-py38h2d3ed51_1.conda#a7d62467d0bb0dae259d6a9a1f122c3a
+https://conda.anaconda.org/conda-forge/osx-64/lxml-4.9.3-py38h2d3ed51_0.conda#69ae6108e1c1eff9182225eddb9d8bf4
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py38h98b9b1b_0.conda#c8dc8bd685921ea63ba672f4ae018f06
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
@@ -128,20 +127,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py38he94b92c_0.conda#433e9f376d8b2295c16dcc9e97e0fea3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
@@ -170,15 +169,15 @@
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
@@ -191,44 +190,44 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py38h50d1736_1.tar.bz2#10df625ea09ec9693735cd0385a52a27
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.1-py38h50d1736_0.conda#c1c83c14b527740467a4376c27a561ef
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/numcodecs-0.11.0-py38h4cd09af_1.conda#6fc938c31040ef364277ad4d52e54302
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyhd1c38e8_0.conda#acc618532cbc899f5721cc96407b16cc
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_dev_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_dev_lab3.6_py3.11.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/m2-msys2-runtime-2.5.0.17080.65c939c-3.tar.bz2#ce25c58bc90071bf71f3d472cb8dfbce
 https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/m2-gcc-libs-5.3.0-4.tar.bz2#51f9bee002e596f14e31c4f528f1fe6c
 https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-102.12.0esr-h63175ca_0.conda#88cc5a7779722782ce0a5b2658188153
+https://conda.anaconda.org/conda-forge/win-64/firefox-102.13.0esr-h63175ca_0.conda#a1baad1ee4cfd8e3dbb70ad8ecff4d7a
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
@@ -106,44 +106,43 @@
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/m2-libintl-0.19.7-4.tar.bz2#bfe5803477f36865cd307b1285bd4209
 https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_6.conda#62826565682d013b3e2346aaf7bded0e
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py311h1ea47a8_1.tar.bz2#52b2142036004451e1881d97e9d01e8a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/future-0.18.3-pyhd8ed1ab_0.conda#fec8329fc739090f26a7d7803db254f1
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py311h12c1d0e_1.conda#07ff18c128d8f3cea2d077a431658456
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/itsdangerous-2.1.2-pyhd8ed1ab_0.tar.bz2#3c3de74912f11d2b590184f03c7cd09b
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/libarchive-3.6.2-h6f8411a_1.conda#314124476882f64abc20b76148d2909b
 https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.1-nocuda_h15da153_6.conda#95b1bd8df3033d08ae5125ed69d71194
 https://conda.anaconda.org/conda-forge/win-64/libxslt-1.1.37-h6070c61_1.conda#b9ed82b82e2f292f75f1af56f35f8c9f
 https://conda.anaconda.org/conda-forge/win-64/m2-dos2unix-7.3.3-2.tar.bz2#978a12148b0ec1954a8bec9259c32b0d
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
@@ -181,15 +180,15 @@
 https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py311h1ea47a8_0.conda#93204e67d63d9ea4ef2b878172222b74
 https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py311h12c1d0e_0.conda#4d7e034dc93f50757cf039a2e3183343
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
 https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/win-64/ruff-0.0.275-py311hc14472d_0.conda#144d6e17af0dcd33390a1a71a621ea68
+https://conda.anaconda.org/conda-forge/win-64/ruff-0.0.276-py311hc14472d_0.conda#34a24ae4788fc4bc4ff24d17cac3f19b
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
@@ -207,21 +206,21 @@
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/noarch/types-docutils-0.20.0.1-pyhd8ed1ab_0.conda#113839f783e42733ec5cb243989ef9f1
 https://conda.anaconda.org/conda-forge/noarch/types-pyyaml-5.4.12-pyhd8ed1ab_0.tar.bz2#efd73a6664edb11d09c52fb05356f0bf
 https://conda.anaconda.org/conda-forge/noarch/types-urllib3-1.26.25.13-pyhd8ed1ab_0.conda#9a73576dfe2f764c431347b9dc35a3fc
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/win-64/ujson-5.7.0-py311h12c1d0e_0.conda#fd194cb1a5c8a838987032a370ba92d8
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py311hc37eb10_0.conda#c16da06cd2c39bba7391076fd64024d8
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/win-64/ansi2html-1.8.0-py311h1ea47a8_1.tar.bz2#37eaf0b4baf7aa03a7d38339c31db411
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
@@ -241,25 +240,25 @@
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
-https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.2-py311h750ae06_1.conda#6c849bdb564c51961a61696c9a376d35
+https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.3-py311h750ae06_0.conda#109154a2e2b00c17f1c6e1680a0f6564
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/win-64/mypy-1.4.1-py311ha68e1ae_0.conda#6d8c5eed03be56e4ceedee017d5edb83
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pip-requirements-parser-32.0.1-pyhd8ed1ab_0.conda#a0efd67d53ab8c20c6020aa40e55bc15
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pyfiglet-0.8.post1-py_0.tar.bz2#e22d3c090f24856764e9d70e76fa3a5f
-https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.12.1-pyhd8ed1ab_0.conda#7abe4ac9f532e2ed024cd08ff69edde1
+https://conda.anaconda.org/conda-forge/noarch/pyproject-fmt-0.13.0-pyhd8ed1ab_0.conda#30bf5ee7d6bf0a7a7eb79685b456ad1c
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/win-64/python-libarchive-c-4.0-py311h1ea47a8_2.tar.bz2#587f3af8e6a1d545a1b3b5a2617435f7
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
@@ -268,16 +267,16 @@
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
 https://conda.anaconda.org/conda-forge/win-64/tbb-2021.9.0-h91493d7_0.conda#6aa3f1becefeaa00a4d2a79b2a478aee
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
 https://conda.anaconda.org/conda-forge/noarch/types-requests-2.31.0.1-pyhd8ed1ab_0.conda#d4edae6cf0af5332243c2d995f5e8745
-https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.0-pyhd8ed1ab_0.conda#fb341d4f1631592d3ab7360e2e9201c3
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/types-setuptools-68.0.0.1-pyhd8ed1ab_0.conda#a44efd4003609542c549f8737b97fa9a
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/url-normalize-1.4.3-pyhd8ed1ab_0.tar.bz2#7c4076e494f0efe76705154ac9302ba6
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
 https://conda.anaconda.org/conda-forge/win-64/cmarkgfm-0.8.0-py311ha68e1ae_2.tar.bz2#206cb594ef199270b7e0d3d17aa87cbe
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-python-lib-3.1.5-pyhd8ed1ab_0.conda#c979eaff5759cb6c8c91369b0ada1abc
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
@@ -292,44 +291,44 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rich-10.16.2-pyhd8ed1ab_0.tar.bz2#06b0afa55cd119e243aea39b037c94ce
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.17-py311ha68e1ae_0.conda#d214a52eb64ec52386ffbc153269d0df
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.1-py311h1ea47a8_0.conda#b82a7bedda179443d95328896b9239e8
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/win-64/black-23.3.0-py311h1ea47a8_1.conda#cff72d53d4ea05005adc2f478447a0a1
 https://conda.anaconda.org/conda-forge/noarch/cyclonedx-bom-3.11.0-pyhd8ed1ab_0.conda#fa8a12276f6186783d375a4dff5160a2
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/win-64/keyring-24.2.0-py311h1ea47a8_0.conda#6a5239529cb5af3437bdd24c1082c2eb
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_mkl.conda#9e42ac6b256b96bfaa19f829c25940e8
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/jupyterlite-core-0.1.0-pyhd8ed1ab_0.conda#c848221f9bd434fb89fa992214e5e64a
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_mkl.conda#768b2c3be666ecf9e62f939ea919f819
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_mkl.conda#278121fe8f0d65d496998aa290f36322
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/noarch/ossindex-lib-1.1.1-pyhd8ed1ab_0.tar.bz2#11718ae7e5d0bd9987636caf9a58b968
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
-https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.0.1-pyhd8ed1ab_0.conda#43ec7b3627237e5fe23413e314e8ba4c
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/requests-cache-1.1.0-pyhd8ed1ab_0.conda#57b89064c125bb9d0e533e018c3eb17a
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
 https://conda.anaconda.org/conda-forge/noarch/autodoc-traits-1.1.0-pyhd8ed1ab_0.conda#66907045fcff46748e485201304cea80
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
 https://conda.anaconda.org/conda-forge/noarch/jake-3.0.1-pyhd8ed1ab_0.conda#f719c7a0825a40e8032d071d2a47d9aa
@@ -342,22 +341,22 @@
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autodoc-typehints-1.21.8-pyhd8ed1ab_0.conda#21e2e0ea045848dcb0053b6cc67a7f7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/twine-3.8.0-pyhd8ed1ab_0.tar.bz2#5d3c0f63166e57c20516b6fc2c1d1115
 https://conda.anaconda.org/conda-forge/noarch/black-jupyter-23.3.0-hd8ed1ab_1.conda#62cc29ee11300ae8a587ff6396e78b62
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/nbqa-1.7.0-pyhd8ed1ab_1.conda#65da1779c33b7fa51a0aba5c30758c5e
 https://conda.anaconda.org/conda-forge/win-64/numcodecs-0.11.0-py311h12c1d0e_1.conda#9b66ec550742f950ba5fdc1fe650ce26
 https://conda.anaconda.org/conda-forge/win-64/pandas-2.0.3-py311hf63dbb6_0.conda#dfbb4b8168065ca0e028907676173f89
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_lock.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_lock.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -68,47 +68,49 @@
 https://conda.anaconda.org/conda-forge/win-64/ruamel_yaml-0.15.80-py311ha68e1ae_1008.tar.bz2#c1c3cca1078977cfa12d36f32eb58fbe
 https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/win-64/libmamba-1.4.5-ha24f096_0.conda#d0e97dcea91a1364f57e65fcd477ef55
+https://conda.anaconda.org/conda-forge/win-64/libmamba-1.4.6-ha24f096_0.conda#a54d92a1a8fbd4261826f1fdebca750b
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py311ha68e1ae_0.conda#1a51f29331338bfde51127db204d7757
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py311ha68e1ae_1005.tar.bz2#dd9604ece454103e7210110c6d343e37
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.1-py311h28e9c30_0.conda#d2b52be40a519bd255397a884bd3fb1c
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
-https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.4.5-py311h29ee5fe_0.conda#4eea49d0269aa4944a663f236def835d
+https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.4.6-py311h29ee5fe_0.conda#c88dc18013b3a79d4b89ced52e3b9064
 https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
-https://conda.anaconda.org/conda-forge/win-64/pydantic-1.10.9-py311ha68e1ae_0.conda#b086521bbe799f96dcc8006869496d1a
+https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.0.2-py311hc37eb10_0.conda#95b86813b262bbcc8413373a6e2e9139
 https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py311he5d195f_2.conda#7ef609e9bfd58d18962d7b7c0c529638
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/keyring-24.2.0-py311h1ea47a8_0.conda#6a5239529cb5af3437bdd24c1082c2eb
+https://conda.anaconda.org/conda-forge/win-64/pydantic-2.0.1-py311ha68e1ae_2.conda#f395df96f5e2eb2f02c0a817dda5a8b2
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/win-64/conda-22.9.0-py311h1ea47a8_2.tar.bz2#b10f47d78cb51f295ee9e6f3a611fa17
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
-https://conda.anaconda.org/conda-forge/win-64/mamba-1.4.5-py311h8cb466b_0.conda#42ec8e65aab0d0505dffab593b721968
+https://conda.anaconda.org/conda-forge/win-64/mamba-1.4.6-py311h8cb466b_0.conda#8365e5d3940063719e29dfa9cca7cbde
 https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.5_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.5_py3.11.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-102.12.0esr-h63175ca_0.conda#88cc5a7779722782ce0a5b2658188153
+https://conda.anaconda.org/conda-forge/win-64/firefox-102.13.0esr-h63175ca_0.conda#a1baad1ee4cfd8e3dbb70ad8ecff4d7a
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/openmp-5.0.0-vc14_1.tar.bz2#8284c925330fa53668ade00db3c9e787
@@ -64,37 +64,36 @@
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/libflang-5.0.0-h6538335_20180525.tar.bz2#9f473a344e18668e99a93f7e21a54b69
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
 https://conda.anaconda.org/conda-forge/win-64/libopenblas-0.3.23-pthreads_hc140b1d_0.conda#dd6ee99b05a7db5b202b8b81cda2812f
 https://conda.anaconda.org/conda-forge/win-64/libxslt-1.1.37-h6070c61_1.conda#b9ed82b82e2f292f75f1af56f35f8c9f
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py311h005e61a_0.conda#01a252f384a5d1ad338cff1184d9a9c0
@@ -130,20 +129,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
@@ -155,15 +154,15 @@
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_openblas.conda#51d270addd38d5dbf21127975992c4f7
-https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.2-py311h750ae06_1.conda#6c849bdb564c51961a61696c9a376d35
+https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.3-py311h750ae06_0.conda#109154a2e2b00c17f1c6e1680a0f6564
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
@@ -173,15 +172,15 @@
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_openblas.conda#be74d3e9999b4ca23bc544d600ec40eb
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_openblas.conda#4073c29a64a9dd59ac31719c9851900d
@@ -191,34 +190,34 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.1-py311h1ea47a8_0.conda#b82a7bedda179443d95328896b9239e8
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.0-py311h0b4df5a_0.conda#71e3f022337531e4109c2ae97f409e1d
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/win-64/numcodecs-0.11.0-py311h12c1d0e_1.conda#9b66ec550742f950ba5fdc1fe650ce26
 https://conda.anaconda.org/conda-forge/win-64/pandas-2.0.3-py311hf63dbb6_0.conda#dfbb4b8168065ca0e028907676173f89
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.3-pyh025b116_0.conda#d33b22490fee39bf6462424a3ea34aba
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.5_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.5_py3.8.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-102.12.0esr-h63175ca_0.conda#88cc5a7779722782ce0a5b2658188153
+https://conda.anaconda.org/conda-forge/win-64/firefox-102.13.0esr-h63175ca_0.conda#a1baad1ee4cfd8e3dbb70ad8ecff4d7a
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/openmp-5.0.0-vc14_1.tar.bz2#8284c925330fa53668ade00db3c9e787
@@ -63,37 +63,36 @@
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/libflang-5.0.0-h6538335_20180525.tar.bz2#9f473a344e18668e99a93f7e21a54b69
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/python-3.8.17-h4de0772_0_cpython.conda#be2296eaf70eeb1cb83c4e95136e694a
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py38hd3f51b4_9.conda#b451fb48b1337ceb34b7b39de0bc09c8
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.5-pyhd8ed1ab_0.conda#953a312b272f37d39fe9d09f46734622
 https://conda.anaconda.org/conda-forge/win-64/libopenblas-0.3.23-pthreads_hc140b1d_0.conda#dd6ee99b05a7db5b202b8b81cda2812f
 https://conda.anaconda.org/conda-forge/win-64/libxslt-1.1.37-h6070c61_1.conda#b9ed82b82e2f292f75f1af56f35f8c9f
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py38h91455d4_0.conda#a674b0be89418013ffa8f92c89d08640
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py38hb1fd069_0.conda#766477345ea8870d47d2dd2988f5c1f8
@@ -128,20 +127,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
@@ -153,15 +152,15 @@
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_openblas.conda#51d270addd38d5dbf21127975992c4f7
-https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.2-py38h5a3a0f9_1.conda#d565096783f7613b6355c824778c0c25
+https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.3-py38h5a3a0f9_0.conda#12ba9693683674c1acb79c309c4dc40c
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
@@ -171,15 +170,15 @@
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_openblas.conda#be74d3e9999b4ca23bc544d600ec40eb
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_openblas.conda#4073c29a64a9dd59ac31719c9851900d
@@ -189,34 +188,34 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py38haa244fe_1.tar.bz2#a67c458650b93acbb664fc359c23cef2
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.1-py38haa244fe_0.conda#53b71f6003217b5ea3662ed2b60fef48
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py38haa244fe_0.conda#15542a4c949a848b768a9e3b8ce3dd30
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.24.4-py38h1d91fd2_0.conda#bb13551a7913ff4de74df687f03ba14e
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/win-64/numcodecs-0.11.0-py38hd3f51b4_1.conda#5acbc1656f223965aab612e43e960b13
 https://conda.anaconda.org/conda-forge/win-64/pandas-1.5.3-py38h5846ac1_1.conda#3a7a1e5c4431a1020b6b7769edf1ccdc
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyh08f2357_0.conda#f289f9dc26526b8bd9f5845486f53a4d
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.21.3-pyh025b116_0.conda#d33b22490fee39bf6462424a3ea34aba
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.6_py3.11.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.6_py3.11.conda.lock`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-102.12.0esr-h63175ca_0.conda#88cc5a7779722782ce0a5b2658188153
+https://conda.anaconda.org/conda-forge/win-64/firefox-102.13.0esr-h63175ca_0.conda#a1baad1ee4cfd8e3dbb70ad8ecff4d7a
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/openmp-5.0.0-vc14_1.tar.bz2#8284c925330fa53668ade00db3c9e787
@@ -63,38 +63,37 @@
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/libflang-5.0.0-h6538335_20180525.tar.bz2#9f473a344e18668e99a93f7e21a54b69
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/libopenblas-0.3.23-pthreads_hc140b1d_0.conda#dd6ee99b05a7db5b202b8b81cda2812f
 https://conda.anaconda.org/conda-forge/win-64/libxslt-1.1.37-h6070c61_1.conda#b9ed82b82e2f292f75f1af56f35f8c9f
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py311h005e61a_0.conda#01a252f384a5d1ad338cff1184d9a9c0
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
@@ -130,20 +129,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py311hc37eb10_0.conda#c16da06cd2c39bba7391076fd64024d8
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
@@ -156,15 +155,15 @@
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_openblas.conda#51d270addd38d5dbf21127975992c4f7
-https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.2-py311h750ae06_1.conda#6c849bdb564c51961a61696c9a376d35
+https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.3-py311h750ae06_0.conda#109154a2e2b00c17f1c6e1680a0f6564
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
@@ -174,15 +173,15 @@
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_openblas.conda#be74d3e9999b4ca23bc544d600ec40eb
@@ -193,45 +192,45 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.1-py311h1ea47a8_0.conda#b82a7bedda179443d95328896b9239e8
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.0-py311h0b4df5a_0.conda#71e3f022337531e4109c2ae97f409e1d
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/win-64/numcodecs-0.11.0-py311h12c1d0e_1.conda#9b66ec550742f950ba5fdc1fe650ce26
 https://conda.anaconda.org/conda-forge/win-64/pandas-2.0.3-py311hf63dbb6_0.conda#dfbb4b8168065ca0e028907676173f89
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
```

### Comparing `ipyforcegraph-0.3.5/.github/locks/win-64_test_lab3.6_py3.8.conda.lock` & `ipyforcegraph-0.3.6/.github/locks/win-64_test_lab3.6_py3.8.conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
 https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-102.12.0esr-h63175ca_0.conda#88cc5a7779722782ce0a5b2658188153
+https://conda.anaconda.org/conda-forge/win-64/firefox-102.13.0esr-h63175ca_0.conda#a1baad1ee4cfd8e3dbb70ad8ecff4d7a
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/openmp-5.0.0-vc14_1.tar.bz2#8284c925330fa53668ade00db3c9e787
@@ -62,38 +62,37 @@
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/libflang-5.0.0-h6538335_20180525.tar.bz2#9f473a344e18668e99a93f7e21a54b69
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/python-3.8.17-h4de0772_0_cpython.conda#be2296eaf70eeb1cb83c4e95136e694a
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py38hd3f51b4_9.conda#b451fb48b1337ceb34b7b39de0bc09c8
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/execnet-1.9.0-pyhd8ed1ab_0.tar.bz2#0e521f7a5e60d508b121d38b04874fb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/gast-0.4.0-pyh9f0ad1d_0.tar.bz2#42323c77b73462199fca93bc8ac9279d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/importnb-2023.1.7-pyhd8ed1ab_0.conda#4ff1d5888b17056732615d7975c254dd
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/libopenblas-0.3.23-pthreads_hc140b1d_0.conda#dd6ee99b05a7db5b202b8b81cda2812f
 https://conda.anaconda.org/conda-forge/win-64/libxslt-1.1.37-h6070c61_1.conda#b9ed82b82e2f292f75f1af56f35f8c9f
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py38h91455d4_0.conda#a674b0be89418013ffa8f92c89d08640
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py38hb1fd069_0.conda#766477345ea8870d47d2dd2988f5c1f8
 https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
@@ -128,20 +127,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py38h4900a04_0.conda#4ba79cbf620ff0cd934fee88bb9c7713
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
@@ -154,15 +153,15 @@
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_openblas.conda#51d270addd38d5dbf21127975992c4f7
-https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.2-py38h5a3a0f9_1.conda#d565096783f7613b6355c824778c0c25
+https://conda.anaconda.org/conda-forge/win-64/lxml-4.9.3-py38h5a3a0f9_0.conda#12ba9693683674c1acb79c309c4dc40c
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/py2vega-0.6.1-pyhd8ed1ab_0.tar.bz2#07594783f950301f5943e6d080ffb4eb
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
@@ -172,15 +171,15 @@
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/scour-0.38.2-pyhd8ed1ab_0.tar.bz2#59d6742bdfe7b3d54c01c0d999e939f0
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/traittypes-0.2.1-pyh9f0ad1d_2.tar.bz2#7d32ccb5334a6822c28af3e864550618
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_openblas.conda#be74d3e9999b4ca23bc544d600ec40eb
@@ -191,45 +190,45 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.3.1-pyhd8ed1ab_0.conda#816073bb54ef59f33f0f26c14f88311b
 https://conda.anaconda.org/conda-forge/noarch/python-dotenv-1.0.0-pyhd8ed1ab_0.conda#a94065a7cbac6b5630fb7e4801366b40
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
 https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.2.1-pyhd8ed1ab_0.conda#cfc3018a9b4411c1cb3efe1e8b5c435b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py38haa244fe_1.tar.bz2#a67c458650b93acbb664fc359c23cef2
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.1-py38haa244fe_0.conda#53b71f6003217b5ea3662ed2b60fef48
 https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py38haa244fe_0.conda#15542a4c949a848b768a9e3b8ce3dd30
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.24.4-py38h1d91fd2_0.conda#bb13551a7913ff4de74df687f03ba14e
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/noarch/pytest-html-3.2.0-pyhd8ed1ab_1.tar.bz2#d5c7a941dfbceaab4b172a56d7918eb0
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
 https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/win-64/numcodecs-0.11.0-py38hd3f51b4_1.conda#5acbc1656f223965aab612e43e960b13
 https://conda.anaconda.org/conda-forge/win-64/pandas-1.5.3-py38h5846ac1_1.conda#3a7a1e5c4431a1020b6b7769edf1ccdc
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.2-pyh08f2357_0.conda#f289f9dc26526b8bd9f5845486f53a4d
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/label/robotframework_jupyterlibrary_alpha/noarch/robotframework-jupyterlibrary-0.5.0a0-pyhbd01f6c_0.conda#ddf6944afacd8f2e8a87d0c6aa141f93
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/bqplot-0.12.39-pyhd8ed1ab_0.conda#f7455264455f8b225034af96269ca78d
 https://conda.anaconda.org/conda-forge/noarch/ipylab-0.7.1-pyhd8ed1ab_1.conda#fd19f67b01ac2ed4d6354c8ae732f889
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
```

### Comparing `ipyforcegraph-0.3.5/.github/pull_request_template.md` & `ipyforcegraph-0.3.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/workflows/badges.yml` & `ipyforcegraph-0.3.6/.github/workflows/badges.yml`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/.github/workflows/ci.yml` & `ipyforcegraph-0.3.6/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   PYTHONIOENCODING: utf-8
   PYTHONUNBUFFERED: '1'
   PIP_DISABLE_PIP_VERSION_CHECK: 'True'
   # until have mamabforge...
   CONDA_EXE: mamba
   # our stuff
   SKIP_CONDA_PREFLIGHT: 1
-  CACHE_EPOCH: 12
+  CACHE_EPOCH: 13
   ATEST_RETRIES: 2
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}-latest
     env:
       BUILDING_IN_CI: 1
@@ -199,15 +199,15 @@
         shell: bash -l {0}
         run: |
           xvfb-run --auto-servernum doit -n4 test || xvfb-run --auto-servernum doit test || exit 1
 
       - name: report (coverage)
         shell: bash -l {0}
         run: |
-          doit -n8 coverage
+          doit -n8 coverage && doit -n8 coverage
 
       - name: upload (coverage)
         if: always()
         uses: actions/upload-artifact@v3
         with:
           name: ipyforcegraph-${{ github.run_number }}-coverage
           path: |
```

### Comparing `ipyforcegraph-0.3.5/.github/workflows/pages.yml` & `ipyforcegraph-0.3.6/.github/workflows/pages.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   PYTHONIOENCODING: utf-8
   PYTHONUNBUFFERED: '1'
   PIP_DISABLE_PIP_VERSION_CHECK: 'True'
   # until have mamabforge...
   CONDA_EXE: mamba
   # our stuff
   SKIP_CONDA_PREFLIGHT: 1
-  CACHE_EPOCH: 12
+  CACHE_EPOCH: 13
   ATEST_RETRIES: 2
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}-latest
     env:
       TOTAL_COVERAGE: 1
```

### Comparing `ipyforcegraph-0.3.5/.gitignore` & `ipyforcegraph-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/CHANGELOG.md` & `ipyforcegraph-0.3.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## `0.3.6`
+
+### `ipyforcegraph 0.3.6`
+
+- rename `GraphDirector.padding` to `.fit_padding`
+
+### `@jupyrdf/jupyter-forcegraph 0.3.6`
+
+- normalize `GraphDirectorModel.padding` to `fit_padding`
+
 ## `0.3.5`
 
 ### `ipyforcegraph 0.3.5`
 
 ### `@jupyrdf/jupyter-forcegraph 0.3.5`
 
 - 2D node text can now be provided by non-text values (by constant or `Column`)
```

### Comparing `ipyforcegraph-0.3.5/CONTRIBUTING.md` & `ipyforcegraph-0.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/COPYRIGHT.md` & `ipyforcegraph-0.3.6/COPYRIGHT.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/LICENSE.txt` & `ipyforcegraph-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/README.md` & `ipyforcegraph-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/01_Behaviors.robot` & `ipyforcegraph-0.3.6/atest/API/01_Behaviors.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/02_Colors_ForceGraph.robot` & `ipyforcegraph-0.3.6/atest/API/02_Colors_ForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/02_Colors_ForceGraph3D.robot` & `ipyforcegraph-0.3.6/atest/API/02_Colors_ForceGraph3D.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/02_Colors_GRAPH.robot.j2` & `ipyforcegraph-0.3.6/atest/API/02_Colors_GRAPH.robot.j2`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/03_Events.robot` & `ipyforcegraph-0.3.6/atest/API/03_Events.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/04_Shapes_ForceGraph.robot` & `ipyforcegraph-0.3.6/atest/API/04_Shapes_ForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/04_Shapes_ForceGraph3D.robot` & `ipyforcegraph-0.3.6/atest/API/04_Shapes_ForceGraph3D.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/04_Shapes_GRAPH.robot.j2` & `ipyforcegraph-0.3.6/atest/API/04_Shapes_GRAPH.robot.j2`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/05_LinkShapes_ForceGraph.robot` & `ipyforcegraph-0.3.6/atest/API/05_LinkShapes_ForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/05_LinkShapes_ForceGraph3D.robot` & `ipyforcegraph-0.3.6/atest/API/05_LinkShapes_ForceGraph3D.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/05_LinkShapes_GRAPH.robot.j2` & `ipyforcegraph-0.3.6/atest/API/05_LinkShapes_GRAPH.robot.j2`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/06_Scales_ForceGraph.robot` & `ipyforcegraph-0.3.6/atest/API/06_Scales_ForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/06_Scales_ForceGraph3D.robot` & `ipyforcegraph-0.3.6/atest/API/06_Scales_ForceGraph3D.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/06_Scales_GRAPH.robot.j2` & `ipyforcegraph-0.3.6/atest/API/06_Scales_GRAPH.robot.j2`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/07_Camera_ForceGraph.robot` & `ipyforcegraph-0.3.6/atest/API/07_Camera_ForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/07_Camera_ForceGraph3D.robot` & `ipyforcegraph-0.3.6/atest/API/07_Camera_ForceGraph3D.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/API/07_Camera_GRAPH.robot.j2` & `ipyforcegraph-0.3.6/atest/API/07_Camera_GRAPH.robot.j2`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/Notebooks/04_Force.robot` & `ipyforcegraph-0.3.6/atest/Notebooks/04_Force.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/Regression/103_2D_Not_Text.robot` & `ipyforcegraph-0.3.6/atest/Regression/103_2D_Not_Text.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/Regression/90_Preserved_ID_Order.robot` & `ipyforcegraph-0.3.6/atest/Regression/90_Preserved_ID_Order.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/fixtures/api/GraphData.py` & `ipyforcegraph-0.3.6/atest/_resources/fixtures/api/GraphData.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/fixtures/api/LinkShapes.py` & `ipyforcegraph-0.3.6/atest/_resources/fixtures/api/LinkShapes.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/fixtures/api/Scales.py` & `ipyforcegraph-0.3.6/atest/_resources/fixtures/api/Scales.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/fixtures/regression/gh-103.py` & `ipyforcegraph-0.3.6/atest/_resources/fixtures/regression/gh-103.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/fixtures/regression/gh-90.py` & `ipyforcegraph-0.3.6/atest/_resources/fixtures/regression/gh-90.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/Browser.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/Browser.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/Coverage.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/Coverage.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/IPyForceGraph.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/IPyForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/Lab.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/Lab.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/Regression.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/Regression.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/keywords/Server.robot` & `ipyforcegraph-0.3.6/atest/_resources/keywords/Server.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/variables/IPyForceGraph.robot` & `ipyforcegraph-0.3.6/atest/_resources/variables/IPyForceGraph.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/atest/_resources/variables/Lab.robot` & `ipyforcegraph-0.3.6/atest/_resources/variables/Lab.robot`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/_static/anvil.svg` & `ipyforcegraph-0.3.6/docs/_static/anvil.svg`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/_static/logo.svg` & `ipyforcegraph-0.3.6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/_static/theme.css` & `ipyforcegraph-0.3.6/docs/_static/theme.css`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/_static/wordmark.svg` & `ipyforcegraph-0.3.6/docs/_static/wordmark.svg`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/conf.py` & `ipyforcegraph-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/dictionary.txt` & `ipyforcegraph-0.3.6/docs/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/environment.yml` & `ipyforcegraph-0.3.6/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/docs/reference/behaviors.md` & `ipyforcegraph-0.3.6/docs/reference/behaviors.md`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/dodo.py` & `ipyforcegraph-0.3.6/dodo.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/3D.ipynb` & `ipyforcegraph-0.3.6/examples/3D.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Behaviors.ipynb` & `ipyforcegraph-0.3.6/examples/Behaviors.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Camera.ipynb` & `ipyforcegraph-0.3.6/examples/Camera.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975904569003528%*

 * *Differences: {"'cells'": '{19: {\'source\': {insert: [(4, \'fit_pad = W.IntSlider(description="fit padding", '*

 * *            "min=0, max=200)\\n')], delete: [4]}}, 27: {'source': {insert: [(19, 'T.link((d2, "*

 * *            '"fit_padding"), (fit_pad, "value"))\\n\'), (20, \'T.link((d3, "fit_padding"), '*

 * *            '(fit_pad, "value"))\\n\'), (22, \'btn_tmpl.observe(on_tmpl, "value")\\n\'), (23, '*

 * *            "'on_tmpl()')], delete: [22, 20, 19]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.4'}}"}*

```diff
@@ -246,15 +246,15 @@
             },
             "outputs": [],
             "source": [
                 "users = {d[\"user\"] for d in data[\"nodes\"] if \"user\" in d}\n",
                 "sel_user = W.Dropdown(description=\"by user\", options=sorted(users))\n",
                 "tmpl_txt = W.Textarea(description=\"template\")\n",
                 "tmpl_nj = B.Nunjucks(\"\")\n",
-                "fit_pad = W.FloatSlider(description=\"padding\", min=0, max=200)\n",
+                "fit_pad = W.IntSlider(description=\"fit padding\", min=0, max=200)\n",
                 "btn_tmpl = W.ToggleButton(description=\"use template\", icon=\"filter\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "11a85001-cec4-4427-a935-636f8ed1cee7",
             "metadata": {},
@@ -396,18 +396,19 @@
                 "        d3.visible = tmpl_nj\n",
                 "\n",
                 "\n",
                 "graph_toggle.observe(on_tmpl, \"value\")\n",
                 "T.dlink(\n",
                 "    (sel_user, \"value\"), (tmpl_txt, \"value\"), lambda x: \"{{ node.user == '%s' }}\" % x\n",
                 ")\n",
-                "T.link((d2, \"padding\"), (fit_pad, \"value\"))\n",
-                "T.link((d3, \"padding\"), (fit_pad, \"value\"))\n",
+                "T.link((d2, \"fit_padding\"), (fit_pad, \"value\"))\n",
+                "T.link((d3, \"fit_padding\"), (fit_pad, \"value\"))\n",
                 "T.dlink((tmpl_txt, \"value\"), (tmpl_nj, \"value\"))\n",
-                "btn_tmpl.observe(on_tmpl, \"value\")"
+                "btn_tmpl.observe(on_tmpl, \"value\")\n",
+                "on_tmpl()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6b99fdc8-3fe5-4064-8b8d-2c335e92db3a",
             "metadata": {},
             "source": [
@@ -494,13 +495,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.11.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ipyforcegraph-0.3.5/examples/DodoApp.ipynb` & `ipyforcegraph-0.3.6/examples/DodoApp.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/DodoSource.ipynb` & `ipyforcegraph-0.3.6/examples/DodoSource.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Forces.ipynb` & `ipyforcegraph-0.3.6/examples/Forces.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Scales.ipynb` & `ipyforcegraph-0.3.6/examples/Scales.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Shapes.ipynb` & `ipyforcegraph-0.3.6/examples/Shapes.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Test_Behaviors.ipynb` & `ipyforcegraph-0.3.6/examples/Test_Behaviors.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Test_Forces.ipynb` & `ipyforcegraph-0.3.6/examples/Test_Forces.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/Utils.ipynb` & `ipyforcegraph-0.3.6/examples/Utils.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/WidgetSource.ipynb` & `ipyforcegraph-0.3.6/examples/WidgetSource.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/_index.ipynb` & `ipyforcegraph-0.3.6/examples/_index.ipynb`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/datasets/blocks.json` & `ipyforcegraph-0.3.6/examples/datasets/blocks.json`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/datasets/d3-dependencies.csv` & `ipyforcegraph-0.3.6/examples/datasets/d3-dependencies.csv`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/datasets/logo.svg` & `ipyforcegraph-0.3.6/examples/datasets/logo.svg`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/datasets/miserables.json` & `ipyforcegraph-0.3.6/examples/datasets/miserables.json`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/examples/datasets/mplate.mtx` & `ipyforcegraph-0.3.6/examples/datasets/mplate.mtx`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/ignored-vulnerabilities.json` & `ipyforcegraph-0.3.6/ignored-vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/plugin.ts` & `ipyforcegraph-0.3.6/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/template-utils.ts` & `ipyforcegraph-0.3.6/js/template-utils.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/tokens.ts` & `ipyforcegraph-0.3.6/js/tokens.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/utils.ts` & `ipyforcegraph-0.3.6/js/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/base.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/base.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/dag.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/dag.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-center.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-center.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-cluster.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-cluster.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-collision.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-collision.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-link.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-link.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-manybody.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-manybody.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-radial.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-radial.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-x.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-x.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-y.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-y.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force-z.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force-z.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/forces/force.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/forces/force.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/graph-camera.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/graph-camera.ts`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,19 @@
     this.center = [zoom.x, zoom.y, ...z];
     this.zoom = k;
     this.lookAt = zoom.lookAt != null ? [lookAt.x, lookAt.y, lookAt.z] : null;
     if (this.captureVisible) {
       this.visible = is3d ? this.getVisible3d(zoom) : this.getVisible2d(zoom);
     }
 
-    this.save();
+    try {
+      this.save();
+    } catch {
+      // nothing to do here
+    }
   }
 
   protected getVisible3d(zoom: IZoomData): number[] {
     const graph = zoom.graph as any as ForceGraph3DInstance;
     const visible = [];
     let i = 0;
 
@@ -156,27 +160,27 @@
   defaults() {
     return {
       ...super.defaults(),
       ...WIDGET_DEFAULTS,
       _model_name: GraphCameraModel.model_name,
       zoom: null,
       visible: null,
-      padding: null,
+      fit_padding: null,
       center: null,
       zoom_first: false,
       zoom_duration: 0.2,
       pan_duration: 0.2,
       fit_duration: 0.2,
     };
   }
 
   initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {
     super.initialize(attributes, options);
     this.on(
-      'change:zoom change:center change:visible change:padding',
+      'change:zoom change:center change:visible change:fit_padding',
       this.onZoomChanged,
       this
     );
     this.updateRequested.connect(this.onZoomChanged, this);
     this.onZoomChanged();
   }
```

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/graph-data.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/graph-data.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/graph-image.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/graph-image.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/index.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/index.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/link-arrow.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/link-arrow.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/link-particles.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/link-particles.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/link-selection.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/link-selection.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/link-shape.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/link-shape.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/link-tooltip.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/link-tooltip.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/node-selection.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/node-selection.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/node-shape.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/node-shape.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/node-tooltip.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/node-tooltip.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/scales.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/scales.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/base.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/base.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/ellipse.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/ellipse.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/rectangle.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/rectangle.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/behaviors/shapes/text.ts` & `ipyforcegraph-0.3.6/js/widgets/behaviors/shapes/text.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/display/2d.ts` & `ipyforcegraph-0.3.6/js/widgets/display/2d.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/display/3d.ts` & `ipyforcegraph-0.3.6/js/widgets/display/3d.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/serializers/dataframe.ts` & `ipyforcegraph-0.3.6/js/widgets/serializers/dataframe.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/js/widgets/sources/dataframe.ts` & `ipyforcegraph-0.3.6/js/widgets/sources/dataframe.ts`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/package.json` & `ipyforcegraph-0.3.6/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -151,9 +151,9 @@
         "watch:lib": "jlpm build:ts --watch --preserveWatchOutput"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.3.5"
+    "version": "0.3.6"
 }
```

### Comparing `ipyforcegraph-0.3.5/pyproject.toml` & `ipyforcegraph-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = [
   "flit_core<4,>=3.9",
 ]
 
 [project]
 name = "ipyforcegraph"
-version = "0.3.5"
+version = "0.3.6"
 description = "2D and 3D force-directed graph widgets for Jupyter"
 readme = "README.md"
 authors = [
     {name = "ipyforcegraph contributors", email = "jupyrdf@users.noreply.github.com"},
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ipyforcegraph-0.3.5/scripts/atest.py` & `ipyforcegraph-0.3.6/scripts/atest.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/scripts/preflight.py` & `ipyforcegraph-0.3.6/scripts/preflight.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/scripts/project.py` & `ipyforcegraph-0.3.6/scripts/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,16 +283,16 @@
 ATEST_COV_PY_INDEX = ATEST_COV_PY / "index.html"
 ALL_COV_PY = REPORTS / "cov_ALL"
 ALL_COV_PY_INDEX = ALL_COV_PY / "index.html"
 PYTEST_COV_THRESHOLD = 90 if (WIN and PY_MAJOR == "3.8") else 91
 PYTEST_HTML = REPORTS / "pytest.html"
 PYTEST_XUNIT = REPORTS / "pytest.xunit.xml"
 PYTEST_JSON = REPORTS / f"report-{PY_MAJOR}-{PLATFORM}.json"
-JS_COV_LINE_THRESHOLD = 83
-JS_COV_BRANCH_THRESHOLD = 63
+JS_COV_LINE_THRESHOLD = 80
+JS_COV_BRANCH_THRESHOLD = 59
 ATEST_PY_COV_THRESHOLD = 88
 ALL_PY_COV_THRESHOLD = 98
 
 # derived info
 PY_VERSION = PY_PROJ_DATA["project"]["version"]
 
 # built artifacts
```

### Comparing `ipyforcegraph-0.3.5/scripts/reporter.py` & `ipyforcegraph-0.3.6/scripts/reporter.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/scripts/utils.py` & `ipyforcegraph-0.3.6/scripts/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,26 +393,27 @@
     if not all_js_cov:
         print("No JS coverage from atest")
         return False
 
     with tempfile.TemporaryDirectory() as td:
         for js_cov in all_js_cov:
             shutil.copy2(js_cov, Path(td) / js_cov.name)
-        subprocess.call(
+        rc = subprocess.call(
             [
                 "jlpm",
                 "nyc",
                 "report",
                 f"--report-dir={P.ATEST_COV_JS}",
                 f"--temp-dir={td}",
                 "--check-coverage",
                 f"--lines={P.JS_COV_LINE_THRESHOLD}",
                 f"--branches={P.JS_COV_BRANCH_THRESHOLD}",
             ]
         )
+    return rc == 0
 
 
 def atest_cov_py():
     all_py_cov = sorted(P.ATEST_OUT.glob("*/pabot_results/*/pycov/.coverage*"))
 
     if not all_py_cov:
         print("No Python coverage from atest")
@@ -427,26 +428,27 @@
                 "--show-contexts",
                 "--omit",
                 "*/tests/*",
                 f"--directory={P.ATEST_COV_PY}",
             ],
             cwd=td,
         )
-        subprocess.call(
+        rc = subprocess.call(
             [
                 "coverage",
                 "report",
                 "--omit",
                 "*/tests/*",
                 "--show-missing",
                 "--skip-covered",
                 f"--fail-under={P.ATEST_PY_COV_THRESHOLD}",
             ],
             cwd=td,
         )
+    return rc == 0
 
 
 def all_cov():
     all_py_cov = [
         P.UTEST_COV_DATA,
         *sorted(P.ATEST_OUT.glob("*/pabot_results/*/pycov/.coverage*")),
     ]
@@ -458,24 +460,25 @@
                 "html",
                 "--title=ALL",
                 "--show-contexts",
                 f"--directory={P.ALL_COV_PY}",
             ],
             cwd=td,
         )
-        subprocess.call(
+        rc = subprocess.call(
             [
                 "coverage",
                 "report",
                 "--show-missing",
                 "--skip-covered",
                 f"--fail-under={P.ALL_PY_COV_THRESHOLD}",
             ],
             cwd=td,
         )
+    return rc == 0
 
 
 def hash_files(
     hash_file: Path,
     hash_deps: List[Path],
     quiet: Optional[bool] = False,
     root: Optional[Path] = None,
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/package.json` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757936507936508%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e4b732ee5c146d5cca18.js'}}",*

 * * "'version'": "'0.3.6'"}*

```diff
@@ -49,15 +49,15 @@
         "third-party/**/*",
         "{lib,style}/**/*.{.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,css}"
     ],
     "homepage": "https://github.com/jupyrdf/ipyforcegraph",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.183d551b88ec5615b6f7.js",
+            "load": "static/remoteEntry.e4b732ee5c146d5cca18.js",
             "style": "./style"
         },
         "extension": "lib/plugin",
         "outputDir": "./src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -156,9 +156,9 @@
         "watch:lib": "jlpm build:ts --watch --preserveWatchOutput"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.3.5"
+    "version": "0.3.6"
 }
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/125.cbe545e870b647d5ab9b.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/132.4eb7dabd414d9d5f9b76.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.372aa8d5d70bf4bd091a.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.6f0ddabb30857eeb84da.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -736,15 +736,18 @@
                 }
                 onZoom(e) {
                     const {
                         graph: t,
                         k: s,
                         lookAt: n
                     } = e, i = this.is3d(t), r = null == e.z ? [] : [e.z];
-                    this.center = [e.x, e.y, ...r], this.zoom = s, this.lookAt = null != e.lookAt ? [n.x, n.y, n.z] : null, this.captureVisible && (this.visible = i ? this.getVisible3d(e) : this.getVisible2d(e)), this.save()
+                    this.center = [e.x, e.y, ...r], this.zoom = s, this.lookAt = null != e.lookAt ? [n.x, n.y, n.z] : null, this.captureVisible && (this.visible = i ? this.getVisible3d(e) : this.getVisible2d(e));
+                    try {
+                        this.save()
+                    } catch (e) {}
                 }
                 getVisible3d(e) {
                     const t = e.graph,
                         s = [];
                     let n = 0;
                     const {
                         THREE: i
@@ -782,24 +785,24 @@
                 defaults() {
                     return {
                         ...super.defaults(),
                         ...a.sB,
                         _model_name: j.model_name,
                         zoom: null,
                         visible: null,
-                        padding: null,
+                        fit_padding: null,
                         center: null,
                         zoom_first: !1,
                         zoom_duration: .2,
                         pan_duration: .2,
                         fit_duration: .2
                     }
                 }
                 initialize(e, t) {
-                    super.initialize(e, t), this.on("change:zoom change:center change:visible change:padding", this.onZoomChanged, this), this.updateRequested.connect(this.onZoomChanged, this), this.onZoomChanged()
+                    super.initialize(e, t), this.on("change:zoom change:center change:visible change:fit_padding", this.onZoomChanged, this), this.updateRequested.connect(this.onZoomChanged, this), this.onZoomChanged()
                 }
                 get zoomFirst() {
                     return this.get("zoom_first")
                 }
                 set zoomFirst(e) {
                     this.set("zoom_first", e)
                 }
@@ -2316,8 +2319,8 @@
             });
             const n = {
                 deserialize: s(647).unpack_models
             }
         }
     }
 ]);
-//# sourceMappingURL=137.372aa8d5d70bf4bd091a.js.map?v=372aa8d5d70bf4bd091a
+//# sourceMappingURL=137.6f0ddabb30857eeb84da.js.map?v=6f0ddabb30857eeb84da
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.372aa8d5d70bf4bd091a.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/137.6f0ddabb30857eeb84da.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8528834541062802%*

 * *Differences: {"'file'": "'137.6f0ddabb30857eeb84da.js?v=6f0ddabb30857eeb84da'",*

 * * "'mappings'": "'yNAQO,MAAMA,EAAa,CACxBC,EAAGC,KAAKD,EACRE,KAAMD,KAAKC,KACXC,IAAKF,KAAKE,IACVC,OAAQH,KAAKG,OACbC,MAAOJ,KAAKI,MACZC,GAAIL,KAAKK,GACTC,QAASN,KAAKM,QACdC,MAAOP,KAAKO,OAGDC,EAAa,CACxBR,KAAKS,KACLT,KAAKU,MACLV,KAAKW,KACLX,KAAKY,MACLZ,KAAKa,KACLb,KAAKc,MACLd,KAAKe,KACLf,KAAKgB,KACLhB,KAAKiB,IACLjB,KAAKkB,KACLlB,KAAKmB,IACLnB,KAAKoB,MACLpB,KAAKqB,MACLrB,KAAKsB,OACLtB,KAAKuB,IACLvB,KAAKwB,MACLxB,KAAKyB,MACLzB,KAAK0B,KACL1B,KAAK2B,KAC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "137.372aa8d5d70bf4bd091a.js?v=372aa8d5d70bf4bd091a",
-    "mappings": "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",
+    "file": "137.6f0ddabb30857eeb84da.js?v=6f0ddabb30857eeb84da",
+    "mappings": "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",
     "names": [
         "MATH_CONST",
         "E",
         "Math",
         "LN10",
         "LN2",
         "LOG10E",
@@ -305,15 +305,15 @@
         "halfH",
         "height",
         "bx",
         "by",
         "GraphDirectorModel",
         "_resetting",
         "_doneResetting",
-        "padding",
+        "fit_padding",
         "zoom_first",
         "zoom_duration",
         "pan_duration",
         "fit_duration",
         "onZoomChanged",
         "zoomFirst",
         "zoomDuration",
@@ -458,14 +458,15 @@
         "fill",
         "scale_on_zoom",
         "stroke",
         "stroke_width",
         "RECTANGLE_DEFAULTS",
         "TEXT_DEFAULTS",
         "font",
+        "padding",
         "text",
         "ShapeBaseModel",
         "_resolveFacets",
         "markType",
         "draw",
         "facets",
         "GeometryShapeModel",
@@ -786,15 +787,15 @@
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\n// import type d3Force from 'd3-force';\nimport { forceLink as d3ForceLink } from 'd3-force-3d';\n\nimport { IBehave, IForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class LinkForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'LinkForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    strength: widget_serialization,\n    distance: widget_serialization,\n  };\n\n  _force: d3ForceLink;\n\n  protected get _modelClass(): typeof LinkForceModel {\n    return LinkForceModel;\n  }\n\n  forceFactory(): d3ForceLink {\n    return d3ForceLink();\n  }\n\n  get force(): d3ForceLink {\n    const { strength, distance } = this._linkFacets;\n\n    let force = this._force;\n    force = strength == null ? force : force.strength(this.wrapForLink(strength));\n    force = distance == null ? force : force.distance(this.wrapForLink(distance));\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { forceManyBody as d3ForceManyBody } from 'd3-force-3d';\n\nimport { IBehave, IForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class ManyBodyForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'ManyBodyForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    strength: widget_serialization,\n    theta: widget_serialization,\n    distance_max: widget_serialization,\n    distance_min: widget_serialization,\n  };\n\n  _force: d3ForceManyBody;\n\n  forceFactory(): d3ForceManyBody {\n    return d3ForceManyBody();\n  }\n\n  protected get _modelClass(): typeof ManyBodyForceModel {\n    return ManyBodyForceModel;\n  }\n\n  get force(): d3ForceManyBody {\n    const { strength, theta, distance_max, distance_min } = this._nodeFacets;\n\n    let force = this._force;\n    force = strength == null ? force : force.strength(this.wrapForNode(strength));\n\n    force = theta == null ? force : force.theta(theta());\n    force = distance_max == null ? force : force.distanceMax(distance_max());\n    force = distance_min == null ? force : force.distanceMin(distance_min());\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { forceRadial as d3ForceRadial } from 'd3-force-3d';\n\nimport { IBehave, IForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class RadialForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'RadialForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    x: widget_serialization,\n    y: widget_serialization,\n    z: widget_serialization,\n    radius: widget_serialization,\n    strength: widget_serialization,\n  };\n\n  _force: d3ForceRadial;\n\n  protected get _modelClass(): typeof RadialForceModel {\n    return RadialForceModel;\n  }\n\n  forceFactory(): d3ForceRadial {\n    return d3ForceRadial();\n  }\n\n  get force(): d3ForceRadial {\n    const { strength, radius, x, y, z } = this._nodeFacets;\n\n    let force = this._force;\n    force = strength == null ? force : force.strength(this.wrapForNode(strength));\n    force = radius == null ? force : force.radius(this.wrapForNode(radius));\n    force = x == null ? force : force.x(x());\n    force = y == null ? force : force.y(y());\n    force = z == null ? force : force.z(z());\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { forceX as d3XForce } from 'd3-force-3d';\n\nimport { IBehave, IForce, TAnyForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class XForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'XForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    x: widget_serialization,\n    strength: widget_serialization,\n  };\n\n  _force: d3XForce;\n\n  protected get _modelClass(): typeof XForceModel {\n    return XForceModel;\n  }\n\n  forceFactory(): d3XForce {\n    return d3XForce();\n  }\n\n  get force(): TAnyForce {\n    const { x, strength } = this._nodeFacets;\n\n    let force = this._force;\n    force = x == null ? force : force.x(this.wrapForNode(x));\n    force = strength == null ? force : force.strength(this.wrapForNode(strength));\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { forceY as d3YForce } from 'd3-force-3d';\n\nimport { IBehave, IForce, TAnyForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class YForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'YForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    y: widget_serialization,\n    strength: widget_serialization,\n  };\n\n  _force: d3YForce;\n\n  protected get _modelClass(): typeof YForceModel {\n    return YForceModel;\n  }\n\n  forceFactory(): d3YForce {\n    return d3YForce();\n  }\n\n  get force(): TAnyForce {\n    const { y, strength } = this._nodeFacets;\n\n    let force = this._force;\n    force = y == null ? force : force.y(this.wrapForNode(y));\n    force = strength == null ? force : force.strength(this.wrapForNode(strength));\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { forceZ as d3ZForce } from 'd3-force-3d';\n\nimport { IBehave, IForce, TAnyForce } from '../../../tokens';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class ZForceModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'ZForceModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    z: widget_serialization,\n    strength: widget_serialization,\n  };\n\n  _force: d3ZForce;\n\n  protected get _modelClass(): typeof ZForceModel {\n    return ZForceModel;\n  }\n\n  forceFactory(): d3ZForce {\n    return d3ZForce();\n  }\n\n  get force(): TAnyForce {\n    const { z, strength } = this._nodeFacets;\n\n    let force = this._force;\n    force = z == null ? force : force.z(this.wrapForNode(z));\n    force = strength == null ? force : force.strength(this.wrapForNode(strength));\n    return force;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { ForceGraphInstance } from 'force-graph/dist/force-graph';\n\nimport { IBehave, IForce } from '../../../tokens';\nimport { yes } from '../../../utils';\nimport { widget_serialization } from '../../serializers/widget';\n\nimport { FacetedForceModel } from './force';\n\nexport class DAGBehaviorModel extends FacetedForceModel implements IBehave, IForce {\n  static model_name = 'DAGBehaviorModel';\n\n  static serializers = {\n    ...FacetedForceModel.serializers,\n    mode: widget_serialization,\n    level_distance: widget_serialization,\n    // node template\n    node_filter: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof DAGBehaviorModel {\n    return DAGBehaviorModel;\n  }\n\n  forceFactory(): void {\n    // raises an error otherwise\n  }\n\n  refreshBehavior(graph: ForceGraphInstance) {\n    const { mode, level_distance, node_filter } = this._nodeFacets;\n\n    const activeMode = this.active && mode ? mode() : null;\n    if (activeMode) {\n      graph.dagMode(activeMode);\n      graph.dagLevelDistance(level_distance ? level_distance() : null);\n\n      const nodeFilter = node_filter ? (this.wrapForNode(node_filter) as any) : yes;\n\n      graph.dagNodeFilter(nodeFilter);\n    } else {\n      graph.dagMode(null);\n      graph.dagLevelDistance(null);\n      graph.dagNodeFilter(yes);\n    }\n  }\n}\n",
-        "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { ForceGraph3DInstance } from '3d-force-graph';\nimport { ForceGraphInstance } from 'force-graph';\n\nimport { IBackboneModelOptions } from '@jupyter-widgets/base';\n\nimport {\n  IBehave,\n  IUpdateGraphCameraOptions,\n  IZoomData,\n  WIDGET_DEFAULTS,\n} from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nclass ZoomBase extends FacetedModel implements IBehave {\n  get zoom(): number | null {\n    return this.get('zoom');\n  }\n\n  set zoom(zoom: number | null) {\n    this.set('zoom', zoom);\n  }\n\n  get lookAt() {\n    return this.get('look_at');\n  }\n\n  set lookAt(lookAt: number[]) {\n    this.set('look_at', lookAt && lookAt.length ? lookAt : null);\n  }\n\n  get center(): number[] {\n    return this.get('center');\n  }\n\n  set center(center: number[]) {\n    this.set('center', center);\n  }\n\n  is3d(graph: ForceGraphInstance | ForceGraph3DInstance) {\n    return graph.hasOwnProperty('nodeThreeObject');\n  }\n}\n\nexport class GraphCameraModel extends ZoomBase implements IBehave {\n  static model_name = 'GraphCameraModel';\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphCameraModel.model_name,\n      zoom: 0,\n      center: [0, 0],\n      visible: [],\n      capturing: false,\n    };\n  }\n\n  get visible(): number[] {\n    return this.get('visible') || [];\n  }\n\n  set visible(visible: number[]) {\n    this.set('visible', visible);\n  }\n\n  get captureVisible(): boolean {\n    return this.get('capturing');\n  }\n\n  set captureVisible(captureVisible: boolean) {\n    this.set('capturing', captureVisible);\n  }\n\n  onZoom(zoom: IZoomData): void {\n    const { graph, k, lookAt } = zoom;\n    const is3d = this.is3d(graph);\n    const z = zoom.z == null ? [] : [zoom.z];\n    this.center = [zoom.x, zoom.y, ...z];\n    this.zoom = k;\n    this.lookAt = zoom.lookAt != null ? [lookAt.x, lookAt.y, lookAt.z] : null;\n    if (this.captureVisible) {\n      this.visible = is3d ? this.getVisible3d(zoom) : this.getVisible2d(zoom);\n    }\n\n    this.save();\n  }\n\n  protected getVisible3d(zoom: IZoomData): number[] {\n    const graph = zoom.graph as any as ForceGraph3DInstance;\n    const visible = [];\n    let i = 0;\n\n    const { THREE } = zoom.iframeClasses;\n    const camera = graph.camera();\n\n    const frustum: THREE.Frustum = new THREE.Frustum().setFromProjectionMatrix(\n      new THREE.Matrix4().multiplyMatrices(\n        camera.projectionMatrix,\n        camera.matrixWorldInverse\n      )\n    );\n\n    for (let node of graph.graphData().nodes) {\n      let __threeObj: THREE.Object3D = (node as any).__threeObj;\n      if (\n        frustum.containsPoint(__threeObj.position) ||\n        frustum.intersectsObject(__threeObj)\n      ) {\n        visible.push(i);\n      }\n      i++;\n    }\n\n    return visible;\n  }\n\n  protected getVisible2d(zoom: IZoomData): number[] {\n    const { graph, k } = zoom;\n    const halfW = graph.width() / 2 / k;\n    const halfH = graph.height() / 2 / k;\n    const bx = [zoom.x - halfW, zoom.x + halfW];\n    const by = [zoom.y - halfH, zoom.y + halfH];\n    const visible = [];\n    let i = 0;\n    for (let { x, y } of graph.graphData().nodes) {\n      if (x >= bx[0] && x <= bx[1] && y >= by[0] && y <= by[1]) {\n        visible.push(i);\n      }\n      i++;\n    }\n    return visible;\n  }\n}\n\nexport class GraphDirectorModel extends ZoomBase implements IBehave {\n  static model_name = 'GraphDirectorModel';\n\n  private _resetting = false;\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    visible: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof GraphDirectorModel {\n    return GraphDirectorModel;\n  }\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphCameraModel.model_name,\n      zoom: null,\n      visible: null,\n      padding: null,\n      center: null,\n      zoom_first: false,\n      zoom_duration: 0.2,\n      pan_duration: 0.2,\n      fit_duration: 0.2,\n    };\n  }\n\n  initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {\n    super.initialize(attributes, options);\n    this.on(\n      'change:zoom change:center change:visible change:padding',\n      this.onZoomChanged,\n      this\n    );\n    this.updateRequested.connect(this.onZoomChanged, this);\n    this.onZoomChanged();\n  }\n\n  get zoomFirst(): boolean {\n    return this.get('zoom_first');\n  }\n\n  set zoomFirst(zoomFirst: boolean) {\n    this.set('zoom_first', zoomFirst);\n  }\n\n  get zoomDuration(): number {\n    return (this.get('zoom_duration') || 0) * 1000;\n  }\n\n  set zoomDuration(zoomDuration: number) {\n    this.set('zoom_duration', zoomDuration);\n  }\n\n  get panDuration(): number {\n    return (this.get('pan_duration') || 0) * 1000;\n  }\n\n  set panDuration(panDuration: number) {\n    this.set('pan_duration', panDuration);\n  }\n\n  get fitDuration(): number {\n    return (this.get('fit_duration') || 0) * 1000;\n  }\n\n  set fitDuration(fitDuration: number) {\n    this.set('fit_duration', fitDuration);\n  }\n\n  get fitPadding(): number {\n    return this.get('fit_padding');\n  }\n\n  set fitPadding(fitPadding: number) {\n    this.set('fit_padding', fitPadding);\n  }\n\n  onZoomChanged() {\n    if (!this._resetting) {\n      this._graphCameraUpdateRequested.emit();\n    }\n  }\n\n  async updateGraphCamera(options: IUpdateGraphCameraOptions): Promise<void> {\n    const { graph } = options;\n    const is3d = this.is3d(graph);\n\n    let visible = null;\n\n    if (this.get('visible')) {\n      await this.ensureFacets();\n      visible = this._nodeFacets['visible'];\n    }\n\n    if (visible) {\n      const wrappedFit = this.wrapForNode(visible) as any;\n      graph.zoomToFit(this.fitDuration, this.fitPadding, wrappedFit);\n    } else {\n      if (is3d) {\n        const { lookAt, center } = this;\n        if (!lookAt || !center) {\n          return;\n        }\n        let graph3 = graph as any as ForceGraph3DInstance;\n        const { Vector3 } = options.iframeClasses.THREE;\n        const vLookAt: THREE.Vector3 = new Vector3(...lookAt);\n        const [x, y, z] = center;\n        graph3.cameraPosition({ x, y, z }, vLookAt, this.zoomDuration);\n      } else {\n        const k = this.zoom;\n        const [x, y] = this.center || [];\n        if (this.zoomFirst) {\n          k == null ? null : graph.zoom(k, this.zoomDuration);\n          x == null && y == null ? null : graph.centerAt(x, y, this.panDuration);\n        } else {\n          x == null && y == null ? null : graph.centerAt(x, y, this.panDuration);\n          k == null ? null : graph.zoom(k, this.zoomDuration);\n        }\n      }\n      this._resetting = true;\n      this.save({ zoom: null, center: null, look_at: null });\n      setTimeout(this._doneResetting, this.panDuration + this.zoomDuration);\n    }\n  }\n\n  private _doneResetting = () => {\n    this._resetting = false;\n  };\n}\n",
+        "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { ForceGraph3DInstance } from '3d-force-graph';\nimport { ForceGraphInstance } from 'force-graph';\n\nimport { IBackboneModelOptions } from '@jupyter-widgets/base';\n\nimport {\n  IBehave,\n  IUpdateGraphCameraOptions,\n  IZoomData,\n  WIDGET_DEFAULTS,\n} from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nclass ZoomBase extends FacetedModel implements IBehave {\n  get zoom(): number | null {\n    return this.get('zoom');\n  }\n\n  set zoom(zoom: number | null) {\n    this.set('zoom', zoom);\n  }\n\n  get lookAt() {\n    return this.get('look_at');\n  }\n\n  set lookAt(lookAt: number[]) {\n    this.set('look_at', lookAt && lookAt.length ? lookAt : null);\n  }\n\n  get center(): number[] {\n    return this.get('center');\n  }\n\n  set center(center: number[]) {\n    this.set('center', center);\n  }\n\n  is3d(graph: ForceGraphInstance | ForceGraph3DInstance) {\n    return graph.hasOwnProperty('nodeThreeObject');\n  }\n}\n\nexport class GraphCameraModel extends ZoomBase implements IBehave {\n  static model_name = 'GraphCameraModel';\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphCameraModel.model_name,\n      zoom: 0,\n      center: [0, 0],\n      visible: [],\n      capturing: false,\n    };\n  }\n\n  get visible(): number[] {\n    return this.get('visible') || [];\n  }\n\n  set visible(visible: number[]) {\n    this.set('visible', visible);\n  }\n\n  get captureVisible(): boolean {\n    return this.get('capturing');\n  }\n\n  set captureVisible(captureVisible: boolean) {\n    this.set('capturing', captureVisible);\n  }\n\n  onZoom(zoom: IZoomData): void {\n    const { graph, k, lookAt } = zoom;\n    const is3d = this.is3d(graph);\n    const z = zoom.z == null ? [] : [zoom.z];\n    this.center = [zoom.x, zoom.y, ...z];\n    this.zoom = k;\n    this.lookAt = zoom.lookAt != null ? [lookAt.x, lookAt.y, lookAt.z] : null;\n    if (this.captureVisible) {\n      this.visible = is3d ? this.getVisible3d(zoom) : this.getVisible2d(zoom);\n    }\n\n    try {\n      this.save();\n    } catch {\n      // nothing to do here\n    }\n  }\n\n  protected getVisible3d(zoom: IZoomData): number[] {\n    const graph = zoom.graph as any as ForceGraph3DInstance;\n    const visible = [];\n    let i = 0;\n\n    const { THREE } = zoom.iframeClasses;\n    const camera = graph.camera();\n\n    const frustum: THREE.Frustum = new THREE.Frustum().setFromProjectionMatrix(\n      new THREE.Matrix4().multiplyMatrices(\n        camera.projectionMatrix,\n        camera.matrixWorldInverse\n      )\n    );\n\n    for (let node of graph.graphData().nodes) {\n      let __threeObj: THREE.Object3D = (node as any).__threeObj;\n      if (\n        frustum.containsPoint(__threeObj.position) ||\n        frustum.intersectsObject(__threeObj)\n      ) {\n        visible.push(i);\n      }\n      i++;\n    }\n\n    return visible;\n  }\n\n  protected getVisible2d(zoom: IZoomData): number[] {\n    const { graph, k } = zoom;\n    const halfW = graph.width() / 2 / k;\n    const halfH = graph.height() / 2 / k;\n    const bx = [zoom.x - halfW, zoom.x + halfW];\n    const by = [zoom.y - halfH, zoom.y + halfH];\n    const visible = [];\n    let i = 0;\n    for (let { x, y } of graph.graphData().nodes) {\n      if (x >= bx[0] && x <= bx[1] && y >= by[0] && y <= by[1]) {\n        visible.push(i);\n      }\n      i++;\n    }\n    return visible;\n  }\n}\n\nexport class GraphDirectorModel extends ZoomBase implements IBehave {\n  static model_name = 'GraphDirectorModel';\n\n  private _resetting = false;\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    visible: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof GraphDirectorModel {\n    return GraphDirectorModel;\n  }\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphCameraModel.model_name,\n      zoom: null,\n      visible: null,\n      fit_padding: null,\n      center: null,\n      zoom_first: false,\n      zoom_duration: 0.2,\n      pan_duration: 0.2,\n      fit_duration: 0.2,\n    };\n  }\n\n  initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {\n    super.initialize(attributes, options);\n    this.on(\n      'change:zoom change:center change:visible change:fit_padding',\n      this.onZoomChanged,\n      this\n    );\n    this.updateRequested.connect(this.onZoomChanged, this);\n    this.onZoomChanged();\n  }\n\n  get zoomFirst(): boolean {\n    return this.get('zoom_first');\n  }\n\n  set zoomFirst(zoomFirst: boolean) {\n    this.set('zoom_first', zoomFirst);\n  }\n\n  get zoomDuration(): number {\n    return (this.get('zoom_duration') || 0) * 1000;\n  }\n\n  set zoomDuration(zoomDuration: number) {\n    this.set('zoom_duration', zoomDuration);\n  }\n\n  get panDuration(): number {\n    return (this.get('pan_duration') || 0) * 1000;\n  }\n\n  set panDuration(panDuration: number) {\n    this.set('pan_duration', panDuration);\n  }\n\n  get fitDuration(): number {\n    return (this.get('fit_duration') || 0) * 1000;\n  }\n\n  set fitDuration(fitDuration: number) {\n    this.set('fit_duration', fitDuration);\n  }\n\n  get fitPadding(): number {\n    return this.get('fit_padding');\n  }\n\n  set fitPadding(fitPadding: number) {\n    this.set('fit_padding', fitPadding);\n  }\n\n  onZoomChanged() {\n    if (!this._resetting) {\n      this._graphCameraUpdateRequested.emit();\n    }\n  }\n\n  async updateGraphCamera(options: IUpdateGraphCameraOptions): Promise<void> {\n    const { graph } = options;\n    const is3d = this.is3d(graph);\n\n    let visible = null;\n\n    if (this.get('visible')) {\n      await this.ensureFacets();\n      visible = this._nodeFacets['visible'];\n    }\n\n    if (visible) {\n      const wrappedFit = this.wrapForNode(visible) as any;\n      graph.zoomToFit(this.fitDuration, this.fitPadding, wrappedFit);\n    } else {\n      if (is3d) {\n        const { lookAt, center } = this;\n        if (!lookAt || !center) {\n          return;\n        }\n        let graph3 = graph as any as ForceGraph3DInstance;\n        const { Vector3 } = options.iframeClasses.THREE;\n        const vLookAt: THREE.Vector3 = new Vector3(...lookAt);\n        const [x, y, z] = center;\n        graph3.cameraPosition({ x, y, z }, vLookAt, this.zoomDuration);\n      } else {\n        const k = this.zoom;\n        const [x, y] = this.center || [];\n        if (this.zoomFirst) {\n          k == null ? null : graph.zoom(k, this.zoomDuration);\n          x == null && y == null ? null : graph.centerAt(x, y, this.panDuration);\n        } else {\n          x == null && y == null ? null : graph.centerAt(x, y, this.panDuration);\n          k == null ? null : graph.zoom(k, this.zoomDuration);\n        }\n      }\n      this._resetting = true;\n      this.save({ zoom: null, center: null, look_at: null });\n      setTimeout(this._doneResetting, this.panDuration + this.zoomDuration);\n    }\n  }\n\n  private _doneResetting = () => {\n    this._resetting = false;\n  };\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBackboneModelOptions, WidgetModel } from '@jupyter-widgets/base';\n\nimport {\n  EUpdate,\n  IBehave,\n  IExtraColumns,\n  IRenderOptions,\n  WIDGET_DEFAULTS,\n} from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\nimport { DataFrameSourceModel } from '../sources';\n\nimport { BehaviorModel } from './base';\n\nexport class GraphDataModel extends BehaviorModel implements IBehave {\n  static model_name = 'GraphDataModel';\n  static serializers = {\n    ...WidgetModel.serializers,\n    sources: widget_serialization,\n  };\n\n  protected _sourcesToCapture = 0;\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphDataModel.model_name,\n      capturing: false,\n      source_count: 1,\n      sources: [],\n    };\n  }\n\n  get sourceCount(): number {\n    return this.get('source_count');\n  }\n\n  get capturing(): boolean {\n    return this.get('capturing');\n  }\n\n  get sources(): DataFrameSourceModel[] {\n    return this.get('sources');\n  }\n\n  initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {\n    super.initialize(attributes, options);\n    this.on('change:capturing', this.onCapturingChanged, this);\n    this.onCapturingChanged();\n  }\n\n  protected onCapturingChanged(e?: any): void {\n    this._sourcesToCapture = this.capturing ? this.sourceCount : 0;\n    if (this._sourcesToCapture) {\n      this._updateRequested.emit(EUpdate.Render);\n    }\n  }\n\n  getExtraColumns(behaviors: IBehave[]): IExtraColumns {\n    const nodes = [];\n    const links = [];\n    for (const behavior of behaviors) {\n      const { extraColumns } = behavior;\n      if (!extraColumns) {\n        continue;\n      }\n      nodes.push(...extraColumns.nodes);\n      links.push(...extraColumns.links);\n    }\n    return { nodes, links };\n  }\n\n  onRender(options: IRenderOptions): void {\n    const { _sourcesToCapture } = this;\n\n    if (!_sourcesToCapture) {\n      return;\n    }\n\n    const { sourceCount, sources } = this;\n\n    const index = sourceCount - _sourcesToCapture;\n\n    this._sourcesToCapture -= 1;\n\n    let source = sources[index];\n\n    source.setFromGraphData(\n      options.graphData,\n      this.getExtraColumns(options.view.model.behaviors)\n    );\n\n    if (this._sourcesToCapture) {\n      return;\n    }\n\n    for (source of sources) {\n      source.save();\n    }\n    this.set({ capturing: false });\n    this.save();\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBackboneModelOptions, WidgetModel } from '@jupyter-widgets/base';\nimport { ImageModel } from '@jupyter-widgets/controls';\n\nimport { EMOJI, EUpdate, IBehave, IRenderOptions, WIDGET_DEFAULTS } from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { BehaviorModel } from './base';\n\nexport class GraphImageModel extends BehaviorModel implements IBehave {\n  static model_name = 'GraphImageModel';\n  static serializers = {\n    ...WidgetModel.serializers,\n    frames: widget_serialization,\n  };\n\n  protected _framesToCapture = 0;\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: GraphImageModel.model_name,\n      enabled: false,\n      frame_count: 1,\n      frames: [],\n    };\n  }\n\n  get frameCount(): number {\n    return this.get('frame_count');\n  }\n\n  get capturing(): boolean {\n    return this.get('capturing');\n  }\n\n  get frames(): ImageModel[] {\n    return this.get('frames');\n  }\n\n  initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {\n    super.initialize(attributes, options);\n    this.on('change:capturing', this.onCapturingChanged, this);\n    this.onCapturingChanged();\n  }\n\n  protected onCapturingChanged(e?: any): void {\n    this._framesToCapture = this.capturing ? this.frameCount : 0;\n    if (this._framesToCapture) {\n      this._updateRequested.emit(EUpdate.Render);\n    }\n  }\n\n  onRender(options: IRenderOptions): void {\n    const { _framesToCapture } = this;\n\n    if (!_framesToCapture) {\n      return;\n    }\n\n    const { frameCount } = this;\n\n    const index = frameCount - _framesToCapture;\n\n    this._framesToCapture -= 1;\n\n    const { context2d, renderer3d } = options;\n\n    let canvas: HTMLCanvasElement | null = null;\n\n    if (context2d) {\n      canvas = context2d.canvas;\n    } else if (renderer3d) {\n      canvas = renderer3d.domElement;\n    }\n\n    if (canvas == null) {\n      console.warn(`${EMOJI} couldn't handle post render of`, options);\n      return;\n    }\n\n    canvas.toBlob(this.onBlob.bind(this, index, this._framesToCapture === 0));\n  }\n\n  protected onBlob = async (\n    index: number,\n    save: boolean,\n    blob: Blob\n  ): Promise<void> => {\n    let frame = this.frames[index];\n    const value = new DataView(await blob.arrayBuffer());\n    frame.set({ value });\n    if (!save) {\n      return;\n    }\n    for (frame of this.frames) {\n      frame.save();\n    }\n    this.set({ capturing: false });\n    this.save();\n  };\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBehave, ILinkBehaveOptions } from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nexport class LinkArrowModel extends FacetedModel implements IBehave {\n  static model_name = 'LinkArrowModel';\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    length: widget_serialization,\n    color: widget_serialization,\n    relative_position: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof LinkArrowModel {\n    return LinkArrowModel;\n  }\n\n  getLinkDirectionalArrowColor(options: ILinkBehaveOptions): string | null {\n    return this._linkFacets.color ? this._linkFacets.color(options) : null;\n  }\n\n  getLinkDirectionalArrowLength(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.length ? this._linkFacets.length(options) : null;\n  }\n\n  getLinkDirectionalArrowRelPos(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.relative_position\n      ? this._linkFacets.relative_position(options)\n      : null;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBehave, ILinkBehaveOptions } from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nexport class LinkParticleModel extends FacetedModel implements IBehave {\n  static model_name = 'LinkParticleModel';\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    color: widget_serialization,\n    density: widget_serialization,\n    speed: widget_serialization,\n    width: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof LinkParticleModel {\n    return LinkParticleModel;\n  }\n\n  getLinkDirectionalParticleColor(options: ILinkBehaveOptions): string | null {\n    return this._linkFacets.color ? this._linkFacets.color(options) : null;\n  }\n\n  getLinkDirectionalParticleSpeed(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.speed ? this._linkFacets.speed(options) : null;\n  }\n\n  getLinkDirectionalParticles(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.density ? this._linkFacets.density(options) : null;\n  }\n\n  getLinkDirectionalParticleWidth(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.width ? this._linkFacets.width(options) : null;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { GraphData } from 'force-graph';\n\nimport { IBackboneModelOptions } from '@jupyter-widgets/base';\n\nimport {\n  DEFAULT_COLORS,\n  DEFAULT_CURVATURES,\n  DEFAULT_LINE_DASHES,\n  DEFAULT_WIDTHS,\n  EUpdate,\n  IBehave,\n  IExtraColumns,\n  ILinkBehaveOptions,\n  ILinkEventBehaveOptions,\n  TSelectedSet,\n  WIDGET_DEFAULTS,\n} from '../../tokens';\n\nimport { BehaviorModel } from './base';\n\nexport class LinkSelectionModel extends BehaviorModel implements IBehave {\n  static model_name = 'LinkSelectionModel';\n\n  defaults() {\n    return {\n      ...super.defaults(),\n      ...WIDGET_DEFAULTS,\n      _model_name: LinkSelectionModel.model_name,\n      selected: [],\n      selected_color: DEFAULT_COLORS.selected,\n      selected_curvature: DEFAULT_CURVATURES.selected,\n      selected_line_dash: DEFAULT_LINE_DASHES.selected,\n      selected_width: DEFAULT_WIDTHS.selected,\n      multiple: true,\n    };\n  }\n\n  initialize(attributes: Backbone.ObjectHash, options: IBackboneModelOptions) {\n    super.initialize(attributes, options);\n    this.on('change:selected change:column_name', this.onValueChange, this);\n    this.onValueChange();\n  }\n\n  get extraColumns(): IExtraColumns {\n    return { links: this.columnName ? [this.columnName] : [], nodes: [] };\n  }\n\n  onValueChange(change?: any) {\n    this._updateRequested.emit(EUpdate.Render);\n    if (this.columnName) {\n      this._graphDataUpdateRequested.emit(void 0);\n    }\n  }\n\n  async updateGraphData(graphData: GraphData): Promise<void> {\n    const { selected, columnName } = this;\n    if (!columnName) {\n      return;\n    }\n    const { links } = graphData;\n    const linkCount = links.length;\n    for (let i = 0; i < linkCount; i++) {\n      links[i][columnName] = selected.has(i);\n    }\n  }\n\n  get selected(): TSelectedSet {\n    return new Set([...(this.get('selected') || [])]);\n  }\n\n  set selected(selected: TSelectedSet) {\n    this.set({ selected: [...selected] });\n    this.save_changes();\n  }\n\n  get selectedColor(): string {\n    return this.get('selected_color') || DEFAULT_COLORS.selected;\n  }\n\n  get selectedCurvature(): string {\n    return this.get('selected_curvature') || DEFAULT_CURVATURES.selected;\n  }\n\n  get selectedLineDash(): string {\n    return this.get('selected_line_dash') || DEFAULT_LINE_DASHES.selected;\n  }\n\n  get selectedWidth(): string {\n    return this.get('selected_width') || DEFAULT_WIDTHS.selected;\n  }\n\n  get columnName(): string | null {\n    return this.get('column_name') || null;\n  }\n\n  get multiple(): boolean {\n    return this.get('multiple');\n  }\n\n  getLinkColor({ index }: ILinkBehaveOptions): string | null {\n    const color = this.selected.has(index) ? this.selectedColor : null;\n    return color;\n  }\n\n  getLinkCurvature({ index }: ILinkBehaveOptions): number | null {\n    const curvature = this.selected.has(index) ? this.selectedCurvature : null;\n    if (curvature != null) {\n      return parseFloat(curvature);\n    }\n    return null;\n  }\n\n  getLinkLineDash({ index }: ILinkBehaveOptions): number[] | null {\n    const line_dash = this.selected.has(index) ? this.selectedLineDash : null;\n    if (line_dash != null) {\n      if (typeof line_dash === 'string') {\n        return JSON.parse(line_dash);\n      }\n      return line_dash;\n    }\n    return null;\n  }\n\n  getLinkWidth({ index }: ILinkBehaveOptions): number | null {\n    const width = this.selected.has(index) ? this.selectedWidth : null;\n    if (width != null) {\n      return parseFloat(width);\n    }\n    return null;\n  }\n\n  onLinkClick = ({\n    link,\n    index,\n    event,\n    graphData,\n  }: ILinkEventBehaveOptions): boolean => {\n    let { selected, columnName, multiple } = this;\n    const indexWasSelected = selected.has(index);\n    if (multiple && (event.ctrlKey || event.shiftKey || event.altKey)) {\n      indexWasSelected ? selected.delete(index) : selected.add(index);\n    } else {\n      if (columnName) {\n        for (const oldIndex of selected) {\n          const oldLink = graphData.links[oldIndex];\n          oldLink && (oldLink[columnName] = false);\n        }\n      }\n      selected.clear();\n      !indexWasSelected && selected.add(index);\n    }\n\n    if (columnName) {\n      link[columnName] = !indexWasSelected;\n    }\n\n    this.selected = selected;\n\n    return true;\n  };\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBehave, ILinkBehaveOptions } from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nexport class LinkShapeModel extends FacetedModel implements IBehave {\n  static model_name = 'LinkShapeModel';\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    color: widget_serialization,\n    curvature: widget_serialization,\n    line_dash: widget_serialization,\n    width: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof LinkShapeModel {\n    return LinkShapeModel;\n  }\n\n  getLinkColor(options: ILinkBehaveOptions): string | null {\n    return this._linkFacets.color ? this._linkFacets.color(options) : null;\n  }\n\n  getLinkCurvature(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.curvature ? this._linkFacets.curvature(options) : null;\n  }\n\n  getLinkLineDash(options: ILinkBehaveOptions): number[] | null {\n    return this._linkFacets.line_dash ? this._linkFacets.line_dash(options) : null;\n  }\n\n  getLinkWidth(options: ILinkBehaveOptions): number | null {\n    return this._linkFacets.width ? this._linkFacets.width(options) : null;\n  }\n}\n",
         "/*\n * Copyright (c) 2023 ipyforcegraph contributors.\n * Distributed under the terms of the Modified BSD License.\n */\nimport { IBehave, ILinkBehaveOptions } from '../../tokens';\nimport { widget_serialization } from '../serializers/widget';\n\nimport { FacetedModel } from './base';\n\nexport class LinkTooltipModel extends FacetedModel implements IBehave {\n  static model_name = 'LinkTooltipModel';\n\n  static serializers = {\n    ...FacetedModel.serializers,\n    label: widget_serialization,\n  };\n\n  protected get _modelClass(): typeof LinkTooltipModel {\n    return LinkTooltipModel;\n  }\n\n  getLinkLabel(options: ILinkBehaveOptions): string | null {\n    return this._linkFacets.label ? this._linkFacets.label(options) : null;\n  }\n}\n",
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/202.69ccd391259ee24eeacf.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/226.726d942c72e811f593f4.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/440.5e8fcb46c2bee136fa6d.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/486.2faa11708efbdc0ccfb7.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/505.6d254900e1dbad3f5cc3.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/549.5a0498a5bdcead199546.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/562.928857973c775977676d.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/67fea965f2310612f9225ab29510fcff9b836e237e6f5cd8c05b266870ffd0d5.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/67fea965f2310612f9225ab29510fcff9b836e237e6f5cd8c05b266870ffd0d5.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/6eebc3e07550540f4bcb82887a5a6da943ea90aaba205486fd1b70b8db0ccfc5.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/6eebc3e07550540f4bcb82887a5a6da943ea90aaba205486fd1b70b8db0ccfc5.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.a54f5f8e362355a77aa3.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.bf098c4c309569651a30.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -77,15 +77,15 @@
                 A1: () => o,
                 BU: () => N,
                 q4: () => i,
                 sB: () => A,
                 ow: () => w,
                 EC: () => D
             });
-            const t = JSON.parse('{"u2":"@jupyrdf/jupyter-forcegraph","i8":"0.3.5"}'),
+            const t = JSON.parse('{"u2":"@jupyrdf/jupyter-forcegraph","i8":"0.3.6"}'),
                 o = t.u2,
                 i = t.i8,
                 a = "🕸️",
                 c = window.location.href.includes("FORCEGRAPH_DEBUG"),
                 l = {
                     widget: "jp-ForceGraph"
                 },
@@ -400,8 +400,8 @@
                         r = l
                     }
                 }
             }
         }
     }
 ]);
-//# sourceMappingURL=709.a54f5f8e362355a77aa3.js.map?v=a54f5f8e362355a77aa3
+//# sourceMappingURL=709.bf098c4c309569651a30.js.map?v=bf098c4c309569651a30
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.a54f5f8e362355a77aa3.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/709.bf098c4c309569651a30.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'709.bf098c4c309569651a30.js?v=bf098c4c309569651a30'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "709.a54f5f8e362355a77aa3.js?v=a54f5f8e362355a77aa3",
+    "file": "709.bf098c4c309569651a30.js?v=bf098c4c309569651a30",
     "mappings": "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",
     "names": [
         "___CSS_LOADER_EXPORT___",
         "push",
         "module",
         "id",
         "requires",
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.9e3da00a7ac27d110b10.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.15063f9dc1ad680ce392.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -112,15 +112,15 @@
                 A1: () => l,
                 BU: () => m,
                 q4: () => t,
                 sB: () => D,
                 ow: () => S,
                 EC: () => T
             });
-            const r = JSON.parse('{"u2":"@jupyrdf/jupyter-forcegraph","i8":"0.3.5"}'),
+            const r = JSON.parse('{"u2":"@jupyrdf/jupyter-forcegraph","i8":"0.3.6"}'),
                 l = r.u2,
                 t = r.i8,
                 n = "🕸️",
                 a = window.location.href.includes("FORCEGRAPH_DEBUG"),
                 d = {
                     widget: "jp-ForceGraph"
                 },
@@ -217,8 +217,8 @@
             const m = {
                 limit: 200,
                 edge: "trailing"
             }
         }
     }
 ]);
-//# sourceMappingURL=717.9e3da00a7ac27d110b10.js.map?v=9e3da00a7ac27d110b10
+//# sourceMappingURL=717.15063f9dc1ad680ce392.js.map?v=15063f9dc1ad680ce392
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.9e3da00a7ac27d110b10.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/717.15063f9dc1ad680ce392.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'717.15063f9dc1ad680ce392.js?v=15063f9dc1ad680ce392'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "717.9e3da00a7ac27d110b10.js?v=9e3da00a7ac27d110b10",
+    "file": "717.15063f9dc1ad680ce392.js?v=15063f9dc1ad680ce392",
     "mappings": "24FAsBaA,EAAO,KACPC,EAAU,KACVC,EAAQ,MACRC,EAAQC,OAAOC,SAASC,KAAKC,SAAS,oBAEtCC,EAAM,CACjBC,OAAQ,iBAGGC,EAA8BC,OAAOC,OAAO,CACvDC,MAAO,GACPC,MAAO,KAGIC,EAAkB,CAC7BC,GAAI,KACJC,OAAQ,SACRC,OAAQ,UAGGC,EAAwB,IAExBC,EAAiB,CAC5BC,SAAU,2BACVC,KAAM,0BACNC,KAAM,wBACNC,WAAY,sBAGDC,EAAiB,CAC5BF,KAAM,EACNF,SAAU,EACVC,KAAM,GAGKI,EAAqB,CAChCH,KAAM,EACNF,SAAU,MAGCM,EAAsB,CACjCJ,KAAM,GACNF,SAAU,MAGCO,EAAkB,CAC7BC,cAAe7B,EACf8B,sBAAuB7B,EACvB8B,aAAc/B,EACdgC,qBAAsB/B,GAIxB,IAAYgC,EAoDAC,GApDZ,SAAYD,GACV,yBACA,uBACA,2BACA,uBACA,0BACD,CAND,CAAYA,IAAAA,EAAO,KAoDnB,SAAYC,GACV,mCACA,mCACA,2CACA,yCACA,mCACA,mEACA,qEACA,qEACA,yEACA,yEACA,0EACA,kEACA,iCACD,CAdD,CAAYA,IAAAA,EAAiB,KAgBtB,MAAMC,EAAmB,CAC9BC,aAAcF,EAAkBE,aAChCC,aAAcH,EAAkBG,aAChCC,iBAAkBJ,EAAkBI,iBACpCC,gBAAiBL,EAAkBK,gBACnCC,aAAcN,EAAkBM,aAChCC,6BAA8BP,EAAkBO,6BAChDC,8BAA+BR,EAAkBQ,8BACjDC,8BAA+BT,EAAkBS,8BACjDC,gCAAiCV,EAAkBU,gCACnDC,gCAAiCX,EAAkBW,gCACnDC,gCAAiCZ,EAAkBY,gCACnDC,4BAA6Bb,EAAkBa,4BAC/CC,YAAad,EAAkBc,aAIjC,IAAYC,GAAZ,SAAYA,GACV,mCACA,mCACA,iCACA,iDACA,+CACA,gCACD,CAPD,CAAYA,IAAAA,EAAiB,KAStB,MAAMC,EAAmB,CAC9BC,aAAcF,EAAkBE,aAChCC,aAAcH,EAAkBG,aAChCC,YAAaJ,EAAkBI,YAC/BC,oBAAqBL,EAAkBK,oBACvCC,mBAAoBN,EAAkBM,mBACtCC,YAAaP,EAAkBO,aAIjC,IAAYC,GAAZ,SAAYA,GACV,2BACA,sBACD,CAHD,CAAYA,IAAAA,EAAkB,KAIvB,MAAMC,EAAoB,CAC/BC,SAAUF,EAAmBE,SAC7BC,OAAQH,EAAmBG,QAuFhBC,EAAalD,OAAOC,OAAO,IAC3BkD,EAAwBnD,OAAOC,OAAO,CACjDE,MAAO+C,EACPhD,MAAOgD,IAgBIE,EAASpD,OAAOC,OAAO,CAClC,GACA,KACA,KACA,KACA,MACA,IACA,QACA,MACA,OACA,SAGF,IAAYoD,EAaAC,GAbZ,SAAYD,GACV,gBACA,oBACA,kBACD,CAJD,CAAYA,IAAAA,EAAO,KAanB,SAAYC,GACV,cACA,aACD,CAHD,CAAYA,IAAAA,EAAK,KAeV,MAAMC,EAAoC,CAAEC,MAAO,IAAKC,KAAM,W",
     "names": [
         "NAME",
         "VERSION",
         "EMOJI",
         "DEBUG",
         "window",
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/829.adbfb126b45c34270ce4.js.map`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/86faec196a5ee5ecc1fc282e34a970be4a18e88d065531f8ea3d174343d67d50.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/998250a831af662f5f25.wasm` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/998250a831af662f5f25.wasm`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/f3725cfa8da49e80941eba5a2eca1192609a5999d6f05b27f5a9f57b0aaf7c67.js`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.183d551b88ec5615b6f7.js` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.e4b732ee5c146d5cca18.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -59,55 +59,55 @@
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         65: "e565d3630178010e411b",
         125: "cbe545e870b647d5ab9b",
         132: "4eb7dabd414d9d5f9b76",
-        137: "372aa8d5d70bf4bd091a",
+        137: "6f0ddabb30857eeb84da",
         202: "69ccd391259ee24eeacf",
         226: "726d942c72e811f593f4",
         228: "bb390299503f7f9e929a",
         236: "8d62e83e35f5e65f00c4",
         253: "84ac30eded183c4db1b9",
         271: "512f94c488062f5c2b86",
         303: "879af8043e11297982af",
         410: "8ea2bb5c049210dcd4a3",
         440: "5e8fcb46c2bee136fa6d",
         460: "761d5a8d3129bfa049b2",
         486: "2faa11708efbdc0ccfb7",
         505: "6d254900e1dbad3f5cc3",
         549: "5a0498a5bdcead199546",
         562: "928857973c775977676d",
-        709: "a54f5f8e362355a77aa3",
+        709: "bf098c4c309569651a30",
         716: "8cff0bdfdf56e5c75152",
-        717: "9e3da00a7ac27d110b10",
+        717: "15063f9dc1ad680ce392",
         829: "adbfb126b45c34270ce4"
     } [e] + ".js?v=" + {
         65: "e565d3630178010e411b",
         125: "cbe545e870b647d5ab9b",
         132: "4eb7dabd414d9d5f9b76",
-        137: "372aa8d5d70bf4bd091a",
+        137: "6f0ddabb30857eeb84da",
         202: "69ccd391259ee24eeacf",
         226: "726d942c72e811f593f4",
         228: "bb390299503f7f9e929a",
         236: "8d62e83e35f5e65f00c4",
         253: "84ac30eded183c4db1b9",
         271: "512f94c488062f5c2b86",
         303: "879af8043e11297982af",
         410: "8ea2bb5c049210dcd4a3",
         440: "5e8fcb46c2bee136fa6d",
         460: "761d5a8d3129bfa049b2",
         486: "2faa11708efbdc0ccfb7",
         505: "6d254900e1dbad3f5cc3",
         549: "5a0498a5bdcead199546",
         562: "928857973c775977676d",
-        709: "a54f5f8e362355a77aa3",
+        709: "bf098c4c309569651a30",
         716: "8cff0bdfdf56e5c75152",
-        717: "9e3da00a7ac27d110b10",
+        717: "15063f9dc1ad680ce392",
         829: "adbfb126b45c34270ce4"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -160,15 +160,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : f > d.from)) && (n[r] = {
                             get: t,
                             from: f,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (d("@bokuweb/zstd-wasm", "0.0.20", (() => P.e(562).then((() => () => P(2562))))), d("@jupyrdf/jupyter-forcegraph", "0.3.5", (() => Promise.all([P.e(125), P.e(236), P.e(137), P.e(716), P.e(717)]).then((() => () => P(2516))))), d("buffer", "6.0.3", (() => P.e(486).then((() => () => P(2486))))), d("d3-force-3d", "3.0.5", (() => P.e(202).then((() => () => P(8202))))), d("d3-force-cluster-3d", "1.1.1", (() => P.e(505).then((() => () => P(4505))))), d("d3-scale-chromatic", "3.0.0", (() => P.e(829).then((() => () => P(5829))))), d("d3-scale", "4.0.2", (() => P.e(226).then((() => () => P(4226))))), d("nunjucks", "3.2.4", (() => P.e(440).then((() => () => P(9440)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@bokuweb/zstd-wasm", "0.0.20", (() => P.e(562).then((() => () => P(2562))))), d("@jupyrdf/jupyter-forcegraph", "0.3.6", (() => Promise.all([P.e(125), P.e(236), P.e(137), P.e(716), P.e(717)]).then((() => () => P(2516))))), d("buffer", "6.0.3", (() => P.e(486).then((() => () => P(2486))))), d("d3-force-3d", "3.0.5", (() => P.e(202).then((() => () => P(8202))))), d("d3-force-cluster-3d", "1.1.1", (() => P.e(505).then((() => () => P(4505))))), d("d3-scale-chromatic", "3.0.0", (() => P.e(829).then((() => () => P(5829))))), d("d3-scale", "4.0.2", (() => P.e(226).then((() => () => P(4226))))), d("nunjucks", "3.2.4", (() => P.e(440).then((() => () => P(9440)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -343,8 +343,8 @@
             },
             t = self.webpackChunk_jupyrdf_jupyter_forcegraph = self.webpackChunk_jupyrdf_jupyter_forcegraph || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var S = P(9076);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyrdf/jupyter-forcegraph"] = S
 })();
-//# sourceMappingURL=remoteEntry.183d551b88ec5615b6f7.js.map
+//# sourceMappingURL=remoteEntry.e4b732ee5c146d5cca18.js.map
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.183d551b88ec5615b6f7.js.map` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/remoteEntry.e4b732ee5c146d5cca18.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9135338345864661%*

 * *Differences: {"'file'": "'remoteEntry.e4b732ee5c146d5cca18.js'",*

 * * "'sourcesContent'": "{insert: [(8, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"65":"e565d3630178010e411b","125":"cbe545e870b647d5ab9b","132":"4eb7dabd414d9d5f9b76","137":"6f0ddabb30857eeb84da","202":"69ccd391259ee24eeacf","226":"726d942c72e811f593f4","22 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.183d551b88ec5615b6f7.js",
+    "file": "remoteEntry.e4b732ee5c146d5cca18.js",
     "mappings": "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",
     "names": [
         "leafPrototypes",
         "getProto",
         "inProgress",
         "dataWebpackPrefix",
         "parseVersion",
@@ -208,19 +208,19 @@
         "var inProgress = {};\nvar dataWebpackPrefix = \"@jupyrdf/jupyter-forcegraph:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t2739: () => (loadStrictVersionCheckFallback(\"default\", \"@bokuweb/zstd-wasm\", [2,0,0,20], () => (__webpack_require__.e(562).then(() => (() => (__webpack_require__(2562))))))),\n\t6042: () => (loadStrictVersionCheckFallback(\"default\", \"buffer\", [1,6,0,3], () => (__webpack_require__.e(486).then(() => (() => (__webpack_require__(2486))))))),\n\t1840: () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t2874: () => (loadStrictVersionCheckFallback(\"default\", \"d3-force-3d\", [2,3,0,5], () => (__webpack_require__.e(202).then(() => (() => (__webpack_require__(8202))))))),\n\t7967: () => (loadStrictVersionCheckFallback(\"default\", \"d3-force-cluster-3d\", [2,1,1,1], () => (__webpack_require__.e(505).then(() => (() => (__webpack_require__(4505))))))),\n\t647: () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [1,6,0,2])),\n\t1526: () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t410: () => (loadStrictVersionCheckFallback(\"default\", \"nunjucks\", [1,3,2,4], () => (__webpack_require__.e(440).then(() => (() => (__webpack_require__(9440))))))),\n\t2303: () => (loadStrictVersionCheckFallback(\"default\", \"d3-scale-chromatic\", [1,3,0,0], () => (__webpack_require__.e(829).then(() => (() => (__webpack_require__(5829))))))),\n\t4253: () => (loadStrictVersionCheckFallback(\"default\", \"d3-scale\", [1,4,0,2], () => (__webpack_require__.e(226).then(() => (() => (__webpack_require__(4226)))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"137\": [\n\t\t1840,\n\t\t2874,\n\t\t7967\n\t],\n\t\"236\": [\n\t\t2739,\n\t\t6042\n\t],\n\t\"253\": [\n\t\t4253\n\t],\n\t\"303\": [\n\t\t2303\n\t],\n\t\"410\": [\n\t\t410\n\t],\n\t\"716\": [\n\t\t647,\n\t\t1526\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(125), __webpack_require__.e(236), __webpack_require__.e(137), __webpack_require__.e(716), __webpack_require__.e(717)]).then(() => (() => ((__webpack_require__(2516)))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(716), __webpack_require__.e(709)]).then(() => (() => ((__webpack_require__(8709)))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(549).then(() => (() => ((__webpack_require__(7549)))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"65\":\"e565d3630178010e411b\",\"125\":\"cbe545e870b647d5ab9b\",\"132\":\"4eb7dabd414d9d5f9b76\",\"137\":\"372aa8d5d70bf4bd091a\",\"202\":\"69ccd391259ee24eeacf\",\"226\":\"726d942c72e811f593f4\",\"228\":\"bb390299503f7f9e929a\",\"236\":\"8d62e83e35f5e65f00c4\",\"253\":\"84ac30eded183c4db1b9\",\"271\":\"512f94c488062f5c2b86\",\"303\":\"879af8043e11297982af\",\"410\":\"8ea2bb5c049210dcd4a3\",\"440\":\"5e8fcb46c2bee136fa6d\",\"460\":\"761d5a8d3129bfa049b2\",\"486\":\"2faa11708efbdc0ccfb7\",\"505\":\"6d254900e1dbad3f5cc3\",\"549\":\"5a0498a5bdcead199546\",\"562\":\"928857973c775977676d\",\"709\":\"a54f5f8e362355a77aa3\",\"716\":\"8cff0bdfdf56e5c75152\",\"717\":\"9e3da00a7ac27d110b10\",\"829\":\"adbfb126b45c34270ce4\"}[chunkId] + \".js?v=\" + {\"65\":\"e565d3630178010e411b\",\"125\":\"cbe545e870b647d5ab9b\",\"132\":\"4eb7dabd414d9d5f9b76\",\"137\":\"372aa8d5d70bf4bd091a\",\"202\":\"69ccd391259ee24eeacf\",\"226\":\"726d942c72e811f593f4\",\"228\":\"bb390299503f7f9e929a\",\"236\":\"8d62e83e35f5e65f00c4\",\"253\":\"84ac30eded183c4db1b9\",\"271\":\"512f94c488062f5c2b86\",\"303\":\"879af8043e11297982af\",\"410\":\"8ea2bb5c049210dcd4a3\",\"440\":\"5e8fcb46c2bee136fa6d\",\"460\":\"761d5a8d3129bfa049b2\",\"486\":\"2faa11708efbdc0ccfb7\",\"505\":\"6d254900e1dbad3f5cc3\",\"549\":\"5a0498a5bdcead199546\",\"562\":\"928857973c775977676d\",\"709\":\"a54f5f8e362355a77aa3\",\"716\":\"8cff0bdfdf56e5c75152\",\"717\":\"9e3da00a7ac27d110b10\",\"829\":\"adbfb126b45c34270ce4\"}[chunkId] + \"\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"65\":\"e565d3630178010e411b\",\"125\":\"cbe545e870b647d5ab9b\",\"132\":\"4eb7dabd414d9d5f9b76\",\"137\":\"6f0ddabb30857eeb84da\",\"202\":\"69ccd391259ee24eeacf\",\"226\":\"726d942c72e811f593f4\",\"228\":\"bb390299503f7f9e929a\",\"236\":\"8d62e83e35f5e65f00c4\",\"253\":\"84ac30eded183c4db1b9\",\"271\":\"512f94c488062f5c2b86\",\"303\":\"879af8043e11297982af\",\"410\":\"8ea2bb5c049210dcd4a3\",\"440\":\"5e8fcb46c2bee136fa6d\",\"460\":\"761d5a8d3129bfa049b2\",\"486\":\"2faa11708efbdc0ccfb7\",\"505\":\"6d254900e1dbad3f5cc3\",\"549\":\"5a0498a5bdcead199546\",\"562\":\"928857973c775977676d\",\"709\":\"bf098c4c309569651a30\",\"716\":\"8cff0bdfdf56e5c75152\",\"717\":\"15063f9dc1ad680ce392\",\"829\":\"adbfb126b45c34270ce4\"}[chunkId] + \".js?v=\" + {\"65\":\"e565d3630178010e411b\",\"125\":\"cbe545e870b647d5ab9b\",\"132\":\"4eb7dabd414d9d5f9b76\",\"137\":\"6f0ddabb30857eeb84da\",\"202\":\"69ccd391259ee24eeacf\",\"226\":\"726d942c72e811f593f4\",\"228\":\"bb390299503f7f9e929a\",\"236\":\"8d62e83e35f5e65f00c4\",\"253\":\"84ac30eded183c4db1b9\",\"271\":\"512f94c488062f5c2b86\",\"303\":\"879af8043e11297982af\",\"410\":\"8ea2bb5c049210dcd4a3\",\"440\":\"5e8fcb46c2bee136fa6d\",\"460\":\"761d5a8d3129bfa049b2\",\"486\":\"2faa11708efbdc0ccfb7\",\"505\":\"6d254900e1dbad3f5cc3\",\"549\":\"5a0498a5bdcead199546\",\"562\":\"928857973c775977676d\",\"709\":\"bf098c4c309569651a30\",\"716\":\"8cff0bdfdf56e5c75152\",\"717\":\"15063f9dc1ad680ce392\",\"829\":\"adbfb126b45c34270ce4\"}[chunkId] + \"\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@jupyrdf/jupyter-forcegraph\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@bokuweb/zstd-wasm\", \"0.0.20\", () => (__webpack_require__.e(562).then(() => (() => (__webpack_require__(2562))))));\n\t\t\tregister(\"@jupyrdf/jupyter-forcegraph\", \"0.3.5\", () => (Promise.all([__webpack_require__.e(125), __webpack_require__.e(236), __webpack_require__.e(137), __webpack_require__.e(716), __webpack_require__.e(717)]).then(() => (() => (__webpack_require__(2516))))));\n\t\t\tregister(\"buffer\", \"6.0.3\", () => (__webpack_require__.e(486).then(() => (() => (__webpack_require__(2486))))));\n\t\t\tregister(\"d3-force-3d\", \"3.0.5\", () => (__webpack_require__.e(202).then(() => (() => (__webpack_require__(8202))))));\n\t\t\tregister(\"d3-force-cluster-3d\", \"1.1.1\", () => (__webpack_require__.e(505).then(() => (() => (__webpack_require__(4505))))));\n\t\t\tregister(\"d3-scale-chromatic\", \"3.0.0\", () => (__webpack_require__.e(829).then(() => (() => (__webpack_require__(5829))))));\n\t\t\tregister(\"d3-scale\", \"4.0.2\", () => (__webpack_require__.e(226).then(() => (() => (__webpack_require__(4226))))));\n\t\t\tregister(\"nunjucks\", \"3.2.4\", () => (__webpack_require__.e(440).then(() => (() => (__webpack_require__(9440))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@jupyrdf/jupyter-forcegraph\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@bokuweb/zstd-wasm\", \"0.0.20\", () => (__webpack_require__.e(562).then(() => (() => (__webpack_require__(2562))))));\n\t\t\tregister(\"@jupyrdf/jupyter-forcegraph\", \"0.3.6\", () => (Promise.all([__webpack_require__.e(125), __webpack_require__.e(236), __webpack_require__.e(137), __webpack_require__.e(716), __webpack_require__.e(717)]).then(() => (() => (__webpack_require__(2516))))));\n\t\t\tregister(\"buffer\", \"6.0.3\", () => (__webpack_require__.e(486).then(() => (() => (__webpack_require__(2486))))));\n\t\t\tregister(\"d3-force-3d\", \"3.0.5\", () => (__webpack_require__.e(202).then(() => (() => (__webpack_require__(8202))))));\n\t\t\tregister(\"d3-force-cluster-3d\", \"1.1.1\", () => (__webpack_require__.e(505).then(() => (() => (__webpack_require__(4505))))));\n\t\t\tregister(\"d3-scale-chromatic\", \"3.0.0\", () => (__webpack_require__.e(829).then(() => (() => (__webpack_require__(5829))))));\n\t\t\tregister(\"d3-scale\", \"4.0.2\", () => (__webpack_require__.e(226).then(() => (() => (__webpack_require__(4226))))));\n\t\t\tregister(\"nunjucks\", \"3.2.4\", () => (__webpack_require__.e(440).then(() => (() => (__webpack_require__(9440))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t426: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^(236|253|303|410|716)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_jupyrdf_jupyter_forcegraph\"] = self[\"webpackChunk_jupyrdf_jupyter_forcegraph\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(9076);\n"
     ],
     "version": 3
 }
```

### Comparing `ipyforcegraph-0.3.5/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/third-party-licenses.json` & `ipyforcegraph-0.3.6/src/_d/share/jupyter/labextensions/@jupyrdf/jupyter-forcegraph/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/__init__.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/_base.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/_base.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/__init__.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/_base.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/_base.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/forces.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/forces.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/particles.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/particles.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/recording.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,20 +140,20 @@
 
     visible: TFeature = _make_trait(
         "fit nodes in viewport for which this column/template is truthy",
         by_template=True,
         by_column=True,
     )
 
-    padding: float = T.Float(
-        10, help="pixels of padding between nodes and viewport"
-    ).tag(sync=True)
-
     zoom_duration: float = T.Float(0.2, help="seconds to animate a zoom").tag(sync=True)
 
     pan_duration: float = T.Float(0.2, help="seconds to animate a pan").tag(sync=True)
 
     fit_duration: float = T.Float(0.2, help="seconds to animate a fit").tag(sync=True)
 
+    fit_padding: float = T.Float(
+        10, help="pixels of padding between visible nodes and viewport"
+    ).tag(sync=True)
+
     @T.validate("visible")
     def _validate_scale_bools(self, proposal: T.Bunch) -> Any:
         return coerce(proposal, JSON_TYPES.boolean)
```

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/scales.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/scales.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/selection.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/selection.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/shapes.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/shapes.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/behaviors/tooltip.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/behaviors/tooltip.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/constants.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/constants.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/graphs.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/graphs.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/js.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/js.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/serializers.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/serializers.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/sources/dataframe.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/sources/dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/sources/dodo.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/sources/dodo.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/sources/widget.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/sources/widget.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_dodo_source.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_dodo_source.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_meta.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_scales.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_serializers.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_widget_model_meta.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_widget_model_meta.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/tests/test_widget_source.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/tests/test_widget_source.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/src/ipyforcegraph/trait_utils.py` & `ipyforcegraph-0.3.6/src/ipyforcegraph/trait_utils.py`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/style/index.css` & `ipyforcegraph-0.3.6/style/index.css`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/tsconfigbase.json` & `ipyforcegraph-0.3.6/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/yarn.lock` & `ipyforcegraph-0.3.6/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipyforcegraph-0.3.5/PKG-INFO` & `ipyforcegraph-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyforcegraph
-Version: 0.3.5
+Version: 0.3.6
 Summary: 2D and 3D force-directed graph widgets for Jupyter
 Author-email: ipyforcegraph contributors <jupyrdf@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
```

