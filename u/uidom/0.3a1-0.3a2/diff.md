# Comparing `tmp/uidom-0.3a1.tar.gz` & `tmp/uidom-0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.3a1.tar", max compression
+gzip compressed data, was "uidom-0.3a2.tar", max compression
```

## Comparing `uidom-0.3a1.tar` & `uidom-0.3a2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.3a1/LICENSE
--rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.3a1/README.md
--rw-r--r--   0        0        0     1274 2023-07-07 07:04:09.243677 uidom-0.3a1/pyproject.toml
--rw-r--r--   0        0        0      218 2023-07-07 07:04:13.091830 uidom-0.3a1/uidom/__init__.py
--rw-r--r--   0        0        0      142 2023-07-07 06:48:42.647563 uidom-0.3a1/uidom/alpinejs/__init__.py
--rw-r--r--   0        0        0     8850 2023-07-07 07:00:34.619955 uidom-0.3a1/uidom/alpinejs/dataset.py
--rw-r--r--   0        0        0     1091 2023-07-07 07:00:31.259852 uidom-0.3a1/uidom/alpinejs/ripple_btn.py
--rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.3a1/uidom/cli/__init__.py
--rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.3a1/uidom/cli/_cli.py
--rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.3a1/uidom/cli/cli.py
--rw-r--r--   0        0        0      517 2023-05-25 09:29:04.826275 uidom-0.3a1/uidom/dom/__init__.py
--rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.3a1/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     6150 2023-05-21 09:09:55.397380 uidom-0.3a1/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.3a1/uidom/dom/icons.py
--rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/dom/jinja.py
--rwxr-xr-x   0        0        0      372 2023-05-25 09:29:08.978350 uidom-0.3a1/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0    16619 2023-07-04 06:04:46.144307 uidom-0.3a1/uidom/dom/src/component.py
--rw-r--r--   0        0        0     3607 2023-05-18 10:26:35.330139 uidom-0.3a1/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.3a1/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    17281 2023-07-02 12:10:50.520496 uidom-0.3a1/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    31710 2023-07-06 14:42:18.425853 uidom-0.3a1/uidom/dom/src/ext.py
--rw-r--r--   0        0        0     7837 2023-05-25 06:29:16.846595 uidom-0.3a1/uidom/dom/src/html_string.py
--rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.3a1/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5072 2023-05-17 19:09:09.607096 uidom-0.3a1/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.3a1/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.3a1/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.3a1/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.3a1/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.3a1/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.3a1/uidom/dom/src/ws_rpc.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.3a1/uidom/dom/src/xmltags.py
--rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.3a1/uidom/dom/ui.py
--rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.3a1/uidom/dom/uniqueid.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.3a1/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.3a1/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.3a1/uidom/elements/__init__.py
--rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.3a1/uidom/elements/booleans.py
--rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.3a1/uidom/elements/buttons.py
--rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/chars.py
--rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/dates.py
--rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/enums.py
--rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/floats.py
--rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.3a1/uidom/elements/integers.py
--rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.3a1/uidom/examples/links.py
--rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.3a1/uidom/examples/toggle.py
--rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.3a1/uidom/reloader/__init__.py
--rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.3a1/uidom/reloader/_app.py
--rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.3a1/uidom/reloader/_models.py
--rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.3a1/uidom/reloader/_notify.py
--rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.3a1/uidom/reloader/_types.py
--rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.3a1/uidom/reloader/_watch.py
--rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.3a1/uidom/reloader/script/reloader.js
--rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.3a1/uidom/response/__init__.py
--rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.3a1/uidom/response/starlette.py
--rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.3a1/uidom/routing/__init__.py
--rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.3a1/uidom/routing/fastapi.py
--rw-r--r--   0        0        0      723 2023-05-17 09:43:23.116452 uidom-0.3a1/uidom/scripts/__init__.py
--rw-r--r--   0        0        0    12124 2023-05-26 17:51:41.362998 uidom-0.3a1/uidom/scripts/xcomponent.js
--rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.3a1/uidom/settings/__init__.py
--rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.3a1/uidom/settings/commands.py
--rw-r--r--   0        0        0     8668 2023-05-17 19:14:22.872098 uidom-0.3a1/uidom/settings/document.py
--rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.3a1/uidom/settings/paths.py
--rw-r--r--   0        0        0      255 2023-05-19 08:05:54.602186 uidom-0.3a1/uidom/slots/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.3a1/uidom/slots/custom_element_slot.py
--rw-r--r--   0        0        0     1597 2023-05-19 08:33:44.200337 uidom-0.3a1/uidom/slots/slots.py
--rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.3a1/uidom/slots/web_component_slot.py
--rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.3a1/uidom/utils/__init__.py
--rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.3a1/uidom/utils/functional.py
--rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.3a1/uidom/utils/logger.py
--rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.3a1/uidom/utils/parameters.py
--rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.3a1/uidom/web_io/__init__.py
--rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.3a1/uidom/web_io/_adapter.py
--rw-r--r--   0        0        0     7496 2023-05-17 18:36:02.616227 uidom-0.3a1/uidom/web_io/_events.py
--rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.3a1/uidom/web_io/_protocol.py
--rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.3a1/uidom/web_io/_types.py
--rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 uidom-0.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.3a2/LICENSE
+-rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.3a2/README.md
+-rw-r--r--   0        0        0     1274 2023-07-07 10:38:13.745641 uidom-0.3a2/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-07-07 10:38:08.868943 uidom-0.3a2/uidom/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-07 06:48:42.647563 uidom-0.3a2/uidom/alpinejs/__init__.py
+-rw-r--r--   0        0        0     8852 2023-07-07 10:35:51.967162 uidom-0.3a2/uidom/alpinejs/dataset.py
+-rw-r--r--   0        0        0     1091 2023-07-07 07:05:57.452135 uidom-0.3a2/uidom/alpinejs/ripple_btn.py
+-rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.3a2/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.3a2/uidom/cli/_cli.py
+-rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.3a2/uidom/cli/cli.py
+-rw-r--r--   0        0        0      517 2023-05-25 09:29:04.826275 uidom-0.3a2/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.3a2/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     6150 2023-05-21 09:09:55.397380 uidom-0.3a2/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.3a2/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.3a2/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      372 2023-05-25 09:29:08.978350 uidom-0.3a2/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    16619 2023-07-04 06:04:46.144307 uidom-0.3a2/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     3607 2023-05-18 10:26:35.330139 uidom-0.3a2/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.3a2/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    17281 2023-07-02 12:10:50.520496 uidom-0.3a2/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31710 2023-07-06 14:42:18.425853 uidom-0.3a2/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7837 2023-05-25 06:29:16.846595 uidom-0.3a2/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.3a2/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5072 2023-05-17 19:09:09.607096 uidom-0.3a2/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.3a2/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.3a2/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.3a2/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.3a2/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.3a2/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.3a2/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.3a2/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.3a2/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.3a2/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.3a2/uidom/dom/src/xmltags.py
+-rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.3a2/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.3a2/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.3a2/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.3a2/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.3a2/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.3a2/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.3a2/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.3a2/uidom/elements/chars.py
+-rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.3a2/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.3a2/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.3a2/uidom/elements/floats.py
+-rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.3a2/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.3a2/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.3a2/uidom/examples/toggle.py
+-rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.3a2/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.3a2/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.3a2/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.3a2/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.3a2/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.3a2/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.3a2/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.3a2/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.3a2/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.3a2/uidom/routing/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.3a2/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      723 2023-05-17 09:43:23.116452 uidom-0.3a2/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0    12124 2023-05-26 17:51:41.362998 uidom-0.3a2/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.3a2/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.3a2/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8668 2023-05-17 19:14:22.872098 uidom-0.3a2/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.3a2/uidom/settings/paths.py
+-rw-r--r--   0        0        0      255 2023-05-19 08:05:54.602186 uidom-0.3a2/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.3a2/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1597 2023-05-19 08:33:44.200337 uidom-0.3a2/uidom/slots/slots.py
+-rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.3a2/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.3a2/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.3a2/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.3a2/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.3a2/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.3a2/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.3a2/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7496 2023-05-17 18:36:02.616227 uidom-0.3a2/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.3a2/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.3a2/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 uidom-0.3a2/PKG-INFO
```

### Comparing `uidom-0.3a1/LICENSE` & `uidom-0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/README.md` & `uidom-0.3a2/README.md`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/pyproject.toml` & `uidom-0.3a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uidom"
-version = "0.3a1"
+version = "0.3a2"
 description = "HTML library"
 authors = ["bitplorer <bitplorer@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uidom-0.3a1/uidom/alpinejs/dataset.py` & `uidom-0.3a2/uidom/alpinejs/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "dataset_focus_visible",
     "dataset_pressed",
     "dataset_hovered",
     "dataset_checked",
     "dataset_scrolled",
     "dataset_scrollable",
     "dataset_selected",
-    "data_x_data",
+    "dataset_xdata",
     "dataset_ripple",
     "dataset_before",
     "dataset_after",
     "DataSet",
 ]
```

### Comparing `uidom-0.3a1/uidom/alpinejs/ripple_btn.py` & `uidom-0.3a2/uidom/alpinejs/ripple_btn.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/cli/__init__.py` & `uidom-0.3a2/uidom/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/cli/_cli.py` & `uidom-0.3a2/uidom/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/cli/cli.py` & `uidom-0.3a2/uidom/cli/cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/__init__.py` & `uidom-0.3a2/uidom/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/htmldocument.py` & `uidom-0.3a2/uidom/dom/htmldocument.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/htmlelement.py` & `uidom-0.3a2/uidom/dom/htmlelement.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/icons.py` & `uidom-0.3a2/uidom/dom/icons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/jinja.py` & `uidom-0.3a2/uidom/dom/jinja.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/component.py` & `uidom-0.3a2/uidom/dom/src/component.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/csstags.py` & `uidom-0.3a2/uidom/dom/src/csstags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/dom1core.py` & `uidom-0.3a2/uidom/dom/src/dom1core.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/dom_tag.py` & `uidom-0.3a2/uidom/dom/src/dom_tag.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/ext.py` & `uidom-0.3a2/uidom/dom/src/ext.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/html_string.py` & `uidom-0.3a2/uidom/dom/src/html_string.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/htmltags.py` & `uidom-0.3a2/uidom/dom/src/htmltags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/jinjatags.py` & `uidom-0.3a2/uidom/dom/src/jinjatags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/parse_html.py` & `uidom-0.3a2/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/pythontags.py` & `uidom-0.3a2/uidom/dom/src/pythontags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/sphinxtags.py` & `uidom-0.3a2/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/svgtags.py` & `uidom-0.3a2/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/utils/dom_util.py` & `uidom-0.3a2/uidom/dom/src/utils/dom_util.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/utils/sheets.py` & `uidom-0.3a2/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/src/ws_rpc.py` & `uidom-0.3a2/uidom/dom/src/ws_rpc.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/ui.py` & `uidom-0.3a2/uidom/dom/ui.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/dom/uniqueid.py` & `uidom-0.3a2/uidom/dom/uniqueid.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/edge_db/ql.py` & `uidom-0.3a2/uidom/edge_db/ql.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/booleans.py` & `uidom-0.3a2/uidom/elements/booleans.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/buttons.py` & `uidom-0.3a2/uidom/elements/buttons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/chars.py` & `uidom-0.3a2/uidom/elements/chars.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/dates.py` & `uidom-0.3a2/uidom/elements/dates.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/enums.py` & `uidom-0.3a2/uidom/elements/enums.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/floats.py` & `uidom-0.3a2/uidom/elements/floats.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/elements/integers.py` & `uidom-0.3a2/uidom/elements/integers.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/examples/links.py` & `uidom-0.3a2/uidom/examples/links.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/examples/toggle.py` & `uidom-0.3a2/uidom/examples/toggle.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/reloader/_app.py` & `uidom-0.3a2/uidom/reloader/_app.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/reloader/_notify.py` & `uidom-0.3a2/uidom/reloader/_notify.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/reloader/_watch.py` & `uidom-0.3a2/uidom/reloader/_watch.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/reloader/script/reloader.js` & `uidom-0.3a2/uidom/reloader/script/reloader.js`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/response/starlette.py` & `uidom-0.3a2/uidom/response/starlette.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/routing/fastapi.py` & `uidom-0.3a2/uidom/routing/fastapi.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/scripts/__init__.py` & `uidom-0.3a2/uidom/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/scripts/xcomponent.js` & `uidom-0.3a2/uidom/scripts/xcomponent.js`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/settings/commands.py` & `uidom-0.3a2/uidom/settings/commands.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/settings/document.py` & `uidom-0.3a2/uidom/settings/document.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/settings/paths.py` & `uidom-0.3a2/uidom/settings/paths.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/slots/custom_element_slot.py` & `uidom-0.3a2/uidom/slots/custom_element_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/slots/slots.py` & `uidom-0.3a2/uidom/slots/slots.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/slots/web_component_slot.py` & `uidom-0.3a2/uidom/slots/web_component_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/utils/functional.py` & `uidom-0.3a2/uidom/utils/functional.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/utils/logger.py` & `uidom-0.3a2/uidom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/utils/parameters.py` & `uidom-0.3a2/uidom/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/web_io/_adapter.py` & `uidom-0.3a2/uidom/web_io/_adapter.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/web_io/_events.py` & `uidom-0.3a2/uidom/web_io/_events.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/uidom/web_io/_protocol.py` & `uidom-0.3a2/uidom/web_io/_protocol.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a1/PKG-INFO` & `uidom-0.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uidom
-Version: 0.3a1
+Version: 0.3a2
 Summary: HTML library
 License: MIT
 Author: bitplorer
 Author-email: bitplorer@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

