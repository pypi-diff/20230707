# Comparing `tmp/pedal-2.5.3.tar.gz` & `tmp/pedal-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.5.3.tar", last modified: Thu Jun 29 18:03:45 2023, max compression
+gzip compressed data, was "pedal-2.5.4.tar", last modified: Thu Jul  6 22:41:56 2023, max compression
```

## Comparing `pedal-2.5.3.tar` & `pedal-2.5.4.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.967597 pedal-2.5.3/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.3/LICENSE
--rw-rw-rw-   0        0        0     2981 2023-06-29 18:03:45.967597 pedal-2.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.680593 pedal-2.5.3/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.675594 pedal-2.5.3/pedal/
--rw-rw-rw-   0        0        0      382 2023-06-28 02:39:12.000000 pedal-2.5.3/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.698594 pedal-2.5.3/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.3/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13562 2023-06-23 17:14:33.000000 pedal-2.5.3/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.3/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.3/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:54.000000 pedal-2.5.3/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.3/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3316 2023-06-23 17:04:45.000000 pedal-2.5.3/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.3/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.712595 pedal-2.5.3/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.3/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.3/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:06.000000 pedal-2.5.3/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:21.000000 pedal-2.5.3/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22520 2023-06-20 15:55:10.000000 pedal-2.5.3/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.3/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.3/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.722594 pedal-2.5.3/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7971 2023-06-14 15:23:15.000000 pedal-2.5.3/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.3/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    24755 2023-06-28 02:41:46.000000 pedal-2.5.3/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.3/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:14.000000 pedal-2.5.3/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.790594 pedal-2.5.3/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     9411 2023-06-23 17:10:49.000000 pedal-2.5.3/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/errors.py
--rw-rw-rw-   0        0        0    21541 2023-06-29 17:23:52.000000 pedal-2.5.3/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.3/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     8147 2023-06-29 16:44:20.000000 pedal-2.5.3/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.3/pedal/core/location.py
--rw-rw-rw-   0        0        0    13819 2023-06-29 17:23:24.000000 pedal-2.5.3/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.3/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.3/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.3/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.813635 pedal-2.5.3/pedal/environments/
--rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.3/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:06.000000 pedal-2.5.3/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9910 2023-06-23 17:16:42.000000 pedal-2.5.3/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.3/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.3/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.3/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:25.000000 pedal-2.5.3/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     4941 2023-06-29 17:29:51.000000 pedal-2.5.3/pedal/environments/terminal.py
--rw-rw-rw-   0        0        0     6673 2023-06-23 16:04:44.000000 pedal-2.5.3/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.820623 pedal-2.5.3/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.3/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.3/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.3/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.836627 pedal-2.5.3/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.3/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.3/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.3/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.3/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.3/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.3/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.3/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.851619 pedal-2.5.3/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.3/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.3/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:54.000000 pedal-2.5.3/pedal/resolvers/export.py
--rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:54.000000 pedal-2.5.3/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.3/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.3/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.3/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.3/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.871620 pedal-2.5.3/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.3/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    18299 2023-06-28 02:55:07.000000 pedal-2.5.3/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.3/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.3/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:28.000000 pedal-2.5.3/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.880620 pedal-2.5.3/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.3/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.3/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.3/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.3/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.3/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10132 2023-06-20 15:21:24.000000 pedal-2.5.3/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.3/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.3/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.3/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.3/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.891593 pedal-2.5.3/pedal/source/
--rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.3/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/constants.py
--rw-rw-rw-   0        0        0     6539 2023-06-29 16:45:23.000000 pedal-2.5.3/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.3/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.911599 pedal-2.5.3/pedal/tifa/
--rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.3/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-06-23 17:11:58.000000 pedal-2.5.3/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.3/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.3/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.3/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.3/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:23.000000 pedal-2.5.3/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42742 2023-06-23 17:17:45.000000 pedal-2.5.3/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.925599 pedal-2.5.3/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.3/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.3/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.938593 pedal-2.5.3/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.3/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.3/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.3/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.3/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.3/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.3/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51452 2023-06-23 17:23:01.000000 pedal-2.5.3/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    15022 2023-06-23 16:26:55.000000 pedal-2.5.3/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.3/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.965594 pedal-2.5.3/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.3/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:40.000000 pedal-2.5.3/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0    10068 2023-06-23 16:57:49.000000 pedal-2.5.3/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.3/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:07.000000 pedal-2.5.3/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.3/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.3/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-06-29 18:03:45.969594 pedal-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-06-23 16:27:25.000000 pedal-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.789507 pedal-2.5.4/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-07-06 22:41:56.789507 pedal-2.5.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.473007 pedal-2.5.4/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3759 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 22:41:56.000000 pedal-2.5.4/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.466977 pedal-2.5.4/pedal/
+-rw-rw-rw-   0        0        0      995 2023-07-04 14:03:45.000000 pedal-2.5.4/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.499979 pedal-2.5.4/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.4/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13562 2023-06-23 17:14:33.000000 pedal-2.5.4/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.4/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.4/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:54.000000 pedal-2.5.4/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.4/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3316 2023-06-23 17:04:45.000000 pedal-2.5.4/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.4/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.517978 pedal-2.5.4/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.4/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.4/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:06.000000 pedal-2.5.4/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:21.000000 pedal-2.5.4/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    23405 2023-07-06 22:36:46.000000 pedal-2.5.4/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.4/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.4/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.531983 pedal-2.5.4/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     8175 2023-06-30 18:05:29.000000 pedal-2.5.4/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.4/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24755 2023-06-28 02:41:46.000000 pedal-2.5.4/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.4/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:14.000000 pedal-2.5.4/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.567977 pedal-2.5.4/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9411 2023-06-23 17:10:49.000000 pedal-2.5.4/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    21596 2023-07-06 13:54:34.000000 pedal-2.5.4/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.4/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8147 2023-06-29 16:44:20.000000 pedal-2.5.4/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.4/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13916 2023-07-04 14:06:42.000000 pedal-2.5.4/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.4/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.4/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.4/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.589980 pedal-2.5.4/pedal/environments/
+-rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.4/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:06.000000 pedal-2.5.4/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9910 2023-06-23 17:16:42.000000 pedal-2.5.4/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.4/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.4/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.4/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:25.000000 pedal-2.5.4/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     5526 2023-06-30 15:48:08.000000 pedal-2.5.4/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6673 2023-06-23 16:04:44.000000 pedal-2.5.4/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.599977 pedal-2.5.4/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.4/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.4/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.4/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.617977 pedal-2.5.4/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.4/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.4/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.4/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.4/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.4/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.4/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.4/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.635976 pedal-2.5.4/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.4/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.4/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:54.000000 pedal-2.5.4/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:54.000000 pedal-2.5.4/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.4/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.4/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.4/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.4/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.662977 pedal-2.5.4/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.4/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    18299 2023-06-28 02:55:07.000000 pedal-2.5.4/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.4/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.4/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:28.000000 pedal-2.5.4/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.674980 pedal-2.5.4/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.4/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.4/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.4/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.4/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.4/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10132 2023-06-20 15:21:24.000000 pedal-2.5.4/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.4/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.4/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.4/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.4/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.688978 pedal-2.5.4/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.4/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     6539 2023-06-29 16:45:23.000000 pedal-2.5.4/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.4/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.713976 pedal-2.5.4/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.4/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-06-23 17:11:58.000000 pedal-2.5.4/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.4/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.4/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.4/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.4/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:23.000000 pedal-2.5.4/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42742 2023-06-23 17:17:45.000000 pedal-2.5.4/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.728980 pedal-2.5.4/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.4/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.4/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.747982 pedal-2.5.4/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.4/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.4/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.4/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.4/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.4/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.4/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51452 2023-06-23 17:23:01.000000 pedal-2.5.4/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    15022 2023-06-23 16:26:55.000000 pedal-2.5.4/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.4/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:41:56.787508 pedal-2.5.4/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.4/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:40.000000 pedal-2.5.4/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0    10068 2023-06-30 15:15:29.000000 pedal-2.5.4/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.4/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:07.000000 pedal-2.5.4/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.4/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.4/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.4/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-07-06 22:41:56.791508 pedal-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-06-30 15:53:57.000000 pedal-2.5.4/setup.py
```

### Comparing `pedal-2.5.3/LICENSE` & `pedal-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/PKG-INFO` & `pedal-2.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.3
+Version: 2.5.4
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.3/Pedal.egg-info/PKG-INFO` & `pedal-2.5.4/Pedal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.3
+Version: 2.5.4
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.3/Pedal.egg-info/SOURCES.txt` & `pedal-2.5.4/Pedal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/README.rst` & `pedal-2.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/__init__.py` & `pedal-2.5.4/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/classes.py` & `pedal-2.5.4/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/commands.py` & `pedal-2.5.4/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/feedbacks.py` & `pedal-2.5.4/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/functions.py` & `pedal-2.5.4/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/organizers.py` & `pedal-2.5.4/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/runtime.py` & `pedal-2.5.4/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/setup.py` & `pedal-2.5.4/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/static.py` & `pedal-2.5.4/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/assertions/unittest.py` & `pedal-2.5.4/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/cait/ast_helpers.py` & `pedal-2.5.4/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/cait/ast_map.py` & `pedal-2.5.4/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/cait/cait_api.py` & `pedal-2.5.4/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/cait/cait_node.py` & `pedal-2.5.4/pedal/cait/cait_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -476,21 +476,37 @@
 
         if type(node_type) is not list:
             node_type_list = [node_type]
         else:
             node_type_list = node_type
 
         for node_t in node_type_list:
-            func_name = 'visit_' + node_t
-            func_ref = main_visit
+            if node_t in ('Num', 'Str', 'Bool'):
+                func_name = 'visit_Constant'
+                func_ref = self._handle_visit_constant(node_t, main_visit)
+            else:
+                func_name = 'visit_' + node_t
+                func_ref = main_visit
             setattr(visitor, func_name, MethodType(func_ref, visitor))
 
         visitor.visit(self.astNode)
         return visitor.items
 
+    def _handle_visit_constant(self, actual_node, visitor_function):
+        def visit_Constant(self, node):
+            # TODO: Does this need to be extended for None, tuple, frozenset, anything else?
+            if actual_node == 'Bool' and isinstance(node.value, bool):
+                return visitor_function(self, node)
+            if actual_node == 'Num' and isinstance(node.value, (int, float)) and not isinstance(node.value, bool):
+                return visitor_function(self, node)
+            elif actual_node == 'Str' and isinstance(node.value, str):
+                return visitor_function(self, node)
+            return self.generic_visit(node)
+        return visit_Constant
+
     def has(self, node):
         """
         Determine if this node has the given `node`. Specifically, it checks if the ast has a given Constant or variable
         This method does NOT check for equality of two asts. Use find_matches for that functionality
         Args:
             node (): A constant (int, float, str), or Name astnode
```

### Comparing `pedal-2.5.3/pedal/cait/find_node.py` & `pedal-2.5.4/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/cait/stretchy_tree_matching.py` & `pedal-2.5.4/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/command_line/command_line.py` & `pedal-2.5.4/pedal/command_line/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,17 @@
     parser.add_argument('--cache', help='Use the given directory to hold the cache.'
                                         ' You can use "./" to use the current directory.',
                         default=False)
     # TODO: Want to allow for multiple threads too to parallel process data (faster!)
     parser.add_argument('--threaded', help='Run the instructor script in a separate thread to avoid'
                                            ' timeout crashes.',
                         default=False)
+    parser.add_argument('--log_level', help="Set the logging level for Pedal.",
+                        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+                        default="ERROR")
     '''
     parser.add_argument('--include_submissions', help='An optional REGEX filter '
                                                       'to only include certain submissions')
     parser.add_argument('--exclude_submissions', help='An optional REGEX filter '
                                                       'to remove certain submissions')
     parser.add_argument('--include_scripts', help='An optional REGEX filter to '
                                                   'only include certain scripts')
```

### Comparing `pedal-2.5.3/pedal/command_line/mocks.py` & `pedal-2.5.4/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/command_line/modes.py` & `pedal-2.5.4/pedal/command_line/modes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/command_line/report.py` & `pedal-2.5.4/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/command_line/verify.py` & `pedal-2.5.4/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/commands.py` & `pedal-2.5.4/pedal/core/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/environment.py` & `pedal-2.5.4/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/errors.py` & `pedal-2.5.4/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/feedback.py` & `pedal-2.5.4/pedal/core/feedback.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             feedback was selected. Serves as a "TL;DR" for this feedback category, useful
             for debugging why a piece of feedback appeared.
         justification_template (str): A markdown-formatted message template that will
             be used if a ``justification`` is None. Any ``fields`` will be injected
             into the template IF the ``condition`` is met.
         priority (str): An indication of how important this feedback is relative to other types
             of feedback in the same category. Might be "high/medium/low". Exactly how this
-            gets used is up to the resolver, but typicaly it helps break ties.
+            gets used is up to the resolver, but typically it helps break ties.
         valence (int): Indicates whether this is negative, positive, or neutral feedback.
             Either 1, -1, or 0.
 
         title (str, optional): A formal, student-facing title for this feedback. If None, indicates
             that the :py:attr:`~pedal.core.feedback.Feedback.label` should be used instead.
         message (str): A markdown-formatted message (aka also supporting HTML) that could be rendered
             to the user.
@@ -70,16 +70,15 @@
         correct (bool): Indicates that the entire submission should be considered correct (success) and that the
             task is now finished.
         muted (bool): Whether this piece of feedback is something that should be shown to a student. There are
             various use cases for muted feedback: they can serve as flags for later conditionals, suppressed
             default kinds of feedback, or perhaps feedback that is interesting for analysis but not pedagogically
             helpful to give to the student. They will still contribute to overall score, but not to the correctness
             of the submission.
-        unscored (bool): Whether or not this piece of feedback contributes to
-            the score/correctness.
+        unscored (bool): Whether this piece of feedback contributes to the score/correctness.
 
         else_message (str): A string to render as a message when a
             NEGATIVE valence feedback is NOT triggered, or a POSITIVE valence
             feedback IS triggered.
         else_message_template (str): Similar to the ``message_template``, but for the ``else_message``.
 
         activate (bool): Used for default feedback objects without a custom
@@ -115,15 +114,14 @@
     CATEGORIES = FeedbackCategory
     KINDS = FeedbackKind
 
     DEFAULT_FEEDBACK_MESSAGE = "No feedback message provided"
     DEFAULT_JUSTIFICATION_MESSAGE = "No justification provided"
     DEFAULT_ELSE_MESSAGE = None
 
-
     label = None
     category = None
     justification = None
     justification_template = None
     constant_fields = None
     fields = None
     field_names = None
@@ -153,15 +151,15 @@
     _stored_args: tuple
     _stored_kwargs: dict
     _override_backups = None
 
     resolved_score = None
     unused_message = None
 
-    #MAIN_REPORT
+    # MAIN_REPORT
 
     def __init__(self, *args, label=None,
                  category=None, justification=None,
                  fields=None, field_names=None,
                  kind=None, title=None,
                  message=None, message_template=None,
                  else_message=None, else_message_template=None,
@@ -198,14 +196,15 @@
             self.fields = fields
         else:
             self.fields = {}
         if self.constant_fields is not None:
             self.fields.update(self.constant_fields)
         if field_names is not None:
             self.field_names = field_names
+            # TODO: Should this be taken from `fields` if nothing is provided?
         if title is not None:
             self.title = title
         elif self.title is None:
             self.title = label
         if message is not None:
             self.message = message
         if message_template is not None:
@@ -258,15 +257,14 @@
         self._stored_kwargs = kwargs
         if delay_condition:
             self._met_condition = False
             self._status = FeedbackStatus.DELAYED
         else:
             self._handle_condition()
 
-
     def _handle_condition(self):
         """ Actually handle the condition check, updating message and report. """
         # Self-attach to a given report?
         self._exception = None
         try:
             self._met_condition = self.condition(*self._stored_args, **self._stored_kwargs)
             # Generate the message field as needed
@@ -378,15 +376,15 @@
 
     def _get_child_feedback(self, feedback, active):
         """ Callback function that Reports will call when a new piece of
         feedback is being considered. By default, does nothing. This is useful
         for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
         will just not care.
 
-        The ``active`` parameter controls whether or not the condition for the
+        The ``active`` parameter controls whether the condition for the
         feedback was met. """
 
     def __xor__(self, other):
         """
         Allows you to have two mutually exclusive conditions. Only one condition will be activated.
 
         Args:
@@ -499,25 +497,27 @@
 
     Args:
         functions (callable): A list of callable functions.
 
     Returns:
         callable: The decorated function.
     """
+
     def CompositeFeedbackFunction_with_attrs(function):
         """
 
         Args:
             function:
 
         Returns:
 
         """
         CompositeFeedbackFunction_with_attrs.functions = functions
         return function
+
     return CompositeFeedbackFunction_with_attrs
 
 
 class FeedbackGroup(Feedback):
     """
     An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
     to indicate that this class will start a new Group context within the report
```

### Comparing `pedal-2.5.3/pedal/core/feedback_category.py` & `pedal-2.5.4/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/final_feedback.py` & `pedal-2.5.4/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/formatting.py` & `pedal-2.5.4/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/location.py` & `pedal-2.5.4/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/report.py` & `pedal-2.5.4/pedal/core/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 File that holds the the Report class and the global MAIN_REPORT.
 
 Note that you can make other Reports, but that doesn't actually seem to be
 useful very often. Usually you want to just rely on the global MAIN_REPORT.
 """
 
 __all__ = ['Report', 'MAIN_REPORT']
+import logging
 
 from pedal.core.errors import PedalToolNotRegistered, PedalToolAlreadyRegistered
 from pedal.core.feedback_category import FeedbackCategory
 
 
 # TODO: Mechanism for checking whether a piece of feedback is in the report
 from pedal.core.formatting import Formatter
 from pedal.core.tool import ToolRegistration
 
+log = logging.getLogger(__name__)
+
 
 class Report:
     """
     A class for storing Feedback generated by Tools, along with any auxiliary
     data that the Tool might want to provide for other tools.
 
     Attributes:
@@ -74,14 +77,15 @@
         self.hooks = {}
         self.class_hooks = {}
         self.submission = None
         self.format = Formatter()
         self.result = None
         self.resolves = []
         self.overridden_feedbacks = set()
+        log.debug("New Pedal Report created.")
 
     def clear(self):
         """
         Resets the entire report back to its starting form,
         including deleting any attached submissions, tool data, and feedbacks.
         It will also reset any overridden fields of feedback classes.
         However, it will not affect class hooks.
```

### Comparing `pedal-2.5.3/pedal/core/resolver.py` & `pedal-2.5.4/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/scoring.py` & `pedal-2.5.4/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/submission.py` & `pedal-2.5.4/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/core/tool.py` & `pedal-2.5.4/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/__init__.py` & `pedal-2.5.4/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/blockpy.py` & `pedal-2.5.4/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/gradescope.py` & `pedal-2.5.4/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/jupyter.py` & `pedal-2.5.4/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/nbgrader.py` & `pedal-2.5.4/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/sandbox.py` & `pedal-2.5.4/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/standard.py` & `pedal-2.5.4/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/environments/terminal.py` & `pedal-2.5.4/pedal/environments/terminal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,83 @@
 import sys
+import os
 
 from pedal import verify, allow_real_io, block_real_io, get_python_errors
 from pedal.core.environment import Environment
 from pedal.core.report import MAIN_REPORT
-from pedal.core.feedback_category import FeedbackCategory
 from pedal.core.commands import set_correct as set_correct_feedback
 from pedal.resolvers.core import make_resolver
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.sandbox.feedbacks import runtime_error
 from pedal.source.feedbacks import syntax_error
 from pedal.tifa import tifa_analysis
 from pedal.resolvers.simple import resolve
 from pedal.core.formatting import Formatter
 
+RESET = "\033[0;0m"
+REVERSE = "\033[;7m"
+UNDERLINE = "\033[4m"
+# \033[1m\033[96m
+BOLD_BRIGHT_COLOR = "\033[1;96m"
+BOLD_RED = "\033[1;91m"
+BOLD_GREEN = "\033[1;92m"
+CHECKMARK = "\u2713"
+CROSSMARK = "\u2717"
+
 
 class TerminalFormatter(Formatter):
+    def __init__(self, report=MAIN_REPORT, path_mask=None, **kwargs):
+        super().__init__(report, **kwargs)
+        self.path_mask = path_mask
+
     def name(self, name):
-        return f"\033[1m\033[96m{name}\033[0m"
+        return f"{BOLD_BRIGHT_COLOR}{name}{RESET}"
 
     def line(self, line_number):
-        return f"\033[4m{line_number}\033[0m"
+        return f"{UNDERLINE}{line_number}{RESET}"
 
-
-RESET = "\033[0;0m"
-REVERSE = "\033[;7m"
+    def filename(self, filename):
+        if self.path_mask:
+            filename = filename.replace(self.path_mask, '')
+        else:
+            filename = os.path.basename(filename)
+        return f"{UNDERLINE}{filename}{RESET}"
 
 
 @make_resolver
 def resolve_on_terminal(report=MAIN_REPORT, file=sys.stdout):
     # print("\033[47m", "-" * 35, "FEEDBACK", "-" * 35, "\033[0m", file=file)
     feedback = resolve(report)
     print("", file=file)
     print(f"{REVERSE}FEEDBACK{RESET} Based on your code, here are some tips and recommendations:\n", file=file)
     if feedback.correct:
-        print(f"✔️  Your code ran successfully.", file=file)
+        print(f"{BOLD_GREEN}{CHECKMARK}{RESET}️  Your code ran successfully.", file=file)
         print(f"{feedback.message}", file=file)
     else:
-        print(f"❌  {feedback.title}\n", file=file)
+        print(f"{BOLD_RED}{CROSSMARK}{RESET}  {feedback.title}\n", file=file)
         print(f"{feedback.message}", file=file)
     print("", file=file)
 
     # if feedback.category not in (FeedbackCategory.SYNTAX, FeedbackCategory.RUNTIME):
-        # Print out the first runtime/syntax error that we encounter
+    # Print out the first runtime/syntax error that we encounter
     for python_error in get_python_errors(report):
         if python_error:
             print(f"{REVERSE}TERMINAL OUTPUT{RESET} For reference, here is the original Python error:", file=file)
             print(to_native_message(python_error), file=file)
         break
     return feedback
 
 
 def to_native_message(error):
     return f"\n{error.fields['traceback_message']}\n{error.fields['exception_name']}: {error.fields['exception_message'].strip()}"
 
 
-def enhance_native_errors(report=MAIN_REPORT):
-    syntax_error.override(message_template = "Bad syntax on line {lineno:line}.\n{suggestion_message}")
-    runtime_error.override(message_template = (
+def enhance_native_errors():
+    syntax_error.override(message_template="Bad syntax on line {lineno:line}.\n{suggestion_message}")
+    runtime_error.override(message_template=(
         "{context_message}\n"
         "{exception_name_proper} occurred:\n\n"
         "{exception_message}\n\n"
         "{suggestion_message}"
     ))
 
 
@@ -75,24 +92,24 @@
             given, then `main_file` will be used to select a `files` from that dictionary (defaults to `answer.py`).
     """
 
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
                  instructor_file='on_run.py', skip_tifa=False, skip_run=False,
                  inputs=None, set_correct=True, set_success=None,
-                 report=MAIN_REPORT, trace=True, threaded=False, real_io=True):
+                 report=MAIN_REPORT, trace=True, threaded=False, real_io=True, path_mask=None):
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
                          report=report)
-        enhance_native_errors(report=report)
-        report.set_formatter(TerminalFormatter(report))
-        set_correct_feedback.override(message_template = ("Great work! Based on your code submitted, there are no other "
-                                                 "recommendations available. You can proceed to the next page by "
-                                                 "using the “Next” button in your lesson."))
+        enhance_native_errors()
+        report.set_formatter(TerminalFormatter(report, path_mask=path_mask))
+        set_correct_feedback.override(message_template=("Great work! Based on your code submitted, there are no other "
+                                                        "recommendations available. You can proceed to the next page "
+                                                        "by using the “Next” button in your lesson."))
         verify(report=self.report)
         if not skip_tifa:
             tifa_analysis(report=self.report)
         if inputs:
             set_input(inputs)
         if skip_run:
             student = get_sandbox(report=report)
```

### Comparing `pedal-2.5.3/pedal/environments/vpl.py` & `pedal-2.5.4/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/extensions/microbit.py` & `pedal-2.5.4/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/extensions/plotting.py` & `pedal-2.5.4/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/__init__.py` & `pedal-2.5.4/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/feedbacks.py` & `pedal-2.5.4/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/graders.py` & `pedal-2.5.4/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/loader.py` & `pedal-2.5.4/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/pool.py` & `pedal-2.5.4/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/questions.py` & `pedal-2.5.4/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/questions/setup.py` & `pedal-2.5.4/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/__init__.py` & `pedal-2.5.4/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/core.py` & `pedal-2.5.4/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/export.py` & `pedal-2.5.4/pedal/resolvers/export.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/full.py` & `pedal-2.5.4/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/sectional.py` & `pedal-2.5.4/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/simple.py` & `pedal-2.5.4/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/resolvers/statistics.py` & `pedal-2.5.4/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/__init__.py` & `pedal-2.5.4/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/commands.py` & `pedal-2.5.4/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/data.py` & `pedal-2.5.4/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/exceptions.py` & `pedal-2.5.4/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/feedbacks.py` & `pedal-2.5.4/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/library/designer.py` & `pedal-2.5.4/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/library/matplotlib.py` & `pedal-2.5.4/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/library/microbit.py` & `pedal-2.5.4/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/library/turtles.py` & `pedal-2.5.4/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/mocked.py` & `pedal-2.5.4/pedal/sandbox/mocked.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/result.py` & `pedal-2.5.4/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/sandbox.py` & `pedal-2.5.4/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/timeout.py` & `pedal-2.5.4/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/sandbox/tracer.py` & `pedal-2.5.4/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/source/__init__.py` & `pedal-2.5.4/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/source/feedbacks.py` & `pedal-2.5.4/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/source/sections.py` & `pedal-2.5.4/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/source/source.py` & `pedal-2.5.4/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/__init__.py` & `pedal-2.5.4/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/commands.py` & `pedal-2.5.4/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/contexts.py` & `pedal-2.5.4/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/feedbacks.py` & `pedal-2.5.4/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/identifier.py` & `pedal-2.5.4/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/settings.py` & `pedal-2.5.4/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/state.py` & `pedal-2.5.4/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/tifa_core.py` & `pedal-2.5.4/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/tifa/tifa_visitor.py` & `pedal-2.5.4/pedal/tifa/tifa_visitor.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/builtin.py` & `pedal-2.5.4/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/library/cs1_curriculum.py` & `pedal-2.5.4/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/library/designer.py` & `pedal-2.5.4/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/library/matplotlib.py` & `pedal-2.5.4/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/library/microbit.py` & `pedal-2.5.4/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/new_types.py` & `pedal-2.5.4/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/normalize.py` & `pedal-2.5.4/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/types/operations.py` & `pedal-2.5.4/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/__init__.py` & `pedal-2.5.4/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/ast_tools.py` & `pedal-2.5.4/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/comparisons.py` & `pedal-2.5.4/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/dictionaries.py` & `pedal-2.5.4/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/exceptions.py` & `pedal-2.5.4/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/files.py` & `pedal-2.5.4/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/operators.py` & `pedal-2.5.4/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/progsnap.py` & `pedal-2.5.4/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/sorting.py` & `pedal-2.5.4/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/text.py` & `pedal-2.5.4/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/pedal/utilities/types.py` & `pedal-2.5.4/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.3/setup.py` & `pedal-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.5.3',
+    version='2.5.4',
     python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

