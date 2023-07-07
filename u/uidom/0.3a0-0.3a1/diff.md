# Comparing `tmp/uidom-0.3a0.tar.gz` & `tmp/uidom-0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.3a0.tar", max compression
+gzip compressed data, was "uidom-0.3a1.tar", max compression
```

## Comparing `uidom-0.3a0.tar` & `uidom-0.3a1.tar`

### file list

```diff
@@ -1,76 +1,79 @@
--rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.3a0/LICENSE
--rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.3a0/README.md
--rw-r--r--   0        0        0     1274 2023-05-21 09:02:27.519438 uidom-0.3a0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-21 09:02:16.247389 uidom-0.3a0/uidom/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.3a0/uidom/cli/__init__.py
--rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.3a0/uidom/cli/_cli.py
--rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.3a0/uidom/cli/cli.py
--rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.3a0/uidom/dom/__init__.py
--rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.3a0/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     6150 2023-05-21 09:09:55.397380 uidom-0.3a0/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.3a0/uidom/dom/icons.py
--rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.3a0/uidom/dom/jinja.py
--rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.3a0/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0    14679 2023-05-18 10:23:20.607511 uidom-0.3a0/uidom/dom/src/component.py
--rw-r--r--   0        0        0     3607 2023-05-18 10:26:35.330139 uidom-0.3a0/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.3a0/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    16799 2023-05-21 06:39:43.281172 uidom-0.3a0/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    31315 2023-05-17 18:54:56.506273 uidom-0.3a0/uidom/dom/src/ext.py
--rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.3a0/uidom/dom/src/html_string.py
--rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.3a0/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5072 2023-05-17 19:09:09.607096 uidom-0.3a0/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.3a0/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.3a0/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.3a0/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.3a0/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.3a0/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.3a0/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.3a0/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.3a0/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.3a0/uidom/dom/src/ws_rpc.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.3a0/uidom/dom/src/xmltags.py
--rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.3a0/uidom/dom/ui.py
--rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.3a0/uidom/dom/uniqueid.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.3a0/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.3a0/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.3a0/uidom/elements/__init__.py
--rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.3a0/uidom/elements/booleans.py
--rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.3a0/uidom/elements/buttons.py
--rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.3a0/uidom/elements/chars.py
--rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.3a0/uidom/elements/dates.py
--rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.3a0/uidom/elements/enums.py
--rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.3a0/uidom/elements/floats.py
--rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.3a0/uidom/elements/integers.py
--rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.3a0/uidom/examples/links.py
--rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.3a0/uidom/examples/toggle.py
--rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.3a0/uidom/reloader/__init__.py
--rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.3a0/uidom/reloader/_app.py
--rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.3a0/uidom/reloader/_models.py
--rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.3a0/uidom/reloader/_notify.py
--rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.3a0/uidom/reloader/_types.py
--rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.3a0/uidom/reloader/_watch.py
--rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.3a0/uidom/reloader/script/reloader.js
--rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.3a0/uidom/response/__init__.py
--rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.3a0/uidom/response/starlette.py
--rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.3a0/uidom/routing/__init__.py
--rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.3a0/uidom/routing/fastapi.py
--rw-r--r--   0        0        0      723 2023-05-17 09:43:23.116452 uidom-0.3a0/uidom/scripts/__init__.py
--rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.3a0/uidom/scripts/xcomponent.js
--rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.3a0/uidom/settings/__init__.py
--rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.3a0/uidom/settings/commands.py
--rw-r--r--   0        0        0     8668 2023-05-17 19:14:22.872098 uidom-0.3a0/uidom/settings/document.py
--rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.3a0/uidom/settings/paths.py
--rw-r--r--   0        0        0      255 2023-05-19 08:05:54.602186 uidom-0.3a0/uidom/slots/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.3a0/uidom/slots/custom_element_slot.py
--rw-r--r--   0        0        0     1597 2023-05-19 08:33:44.200337 uidom-0.3a0/uidom/slots/slots.py
--rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.3a0/uidom/slots/web_component_slot.py
--rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.3a0/uidom/utils/__init__.py
--rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.3a0/uidom/utils/functional.py
--rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.3a0/uidom/utils/logger.py
--rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.3a0/uidom/utils/parameters.py
--rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.3a0/uidom/web_io/__init__.py
--rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.3a0/uidom/web_io/_adapter.py
--rw-r--r--   0        0        0     7496 2023-05-17 18:36:02.616227 uidom-0.3a0/uidom/web_io/_events.py
--rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.3a0/uidom/web_io/_protocol.py
--rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.3a0/uidom/web_io/_types.py
--rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 uidom-0.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.3a1/LICENSE
+-rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.3a1/README.md
+-rw-r--r--   0        0        0     1274 2023-07-07 07:04:09.243677 uidom-0.3a1/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-07-07 07:04:13.091830 uidom-0.3a1/uidom/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-07 06:48:42.647563 uidom-0.3a1/uidom/alpinejs/__init__.py
+-rw-r--r--   0        0        0     8850 2023-07-07 07:00:34.619955 uidom-0.3a1/uidom/alpinejs/dataset.py
+-rw-r--r--   0        0        0     1091 2023-07-07 07:00:31.259852 uidom-0.3a1/uidom/alpinejs/ripple_btn.py
+-rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.3a1/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.3a1/uidom/cli/_cli.py
+-rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.3a1/uidom/cli/cli.py
+-rw-r--r--   0        0        0      517 2023-05-25 09:29:04.826275 uidom-0.3a1/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.3a1/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     6150 2023-05-21 09:09:55.397380 uidom-0.3a1/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.3a1/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      372 2023-05-25 09:29:08.978350 uidom-0.3a1/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    16619 2023-07-04 06:04:46.144307 uidom-0.3a1/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     3607 2023-05-18 10:26:35.330139 uidom-0.3a1/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.3a1/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    17281 2023-07-02 12:10:50.520496 uidom-0.3a1/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31710 2023-07-06 14:42:18.425853 uidom-0.3a1/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7837 2023-05-25 06:29:16.846595 uidom-0.3a1/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.3a1/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5072 2023-05-17 19:09:09.607096 uidom-0.3a1/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.3a1/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.3a1/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.3a1/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.3a1/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.3a1/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.3a1/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.3a1/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.3a1/uidom/dom/src/xmltags.py
+-rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.3a1/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.3a1/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.3a1/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.3a1/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.3a1/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.3a1/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.3a1/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/chars.py
+-rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.3a1/uidom/elements/floats.py
+-rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.3a1/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.3a1/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.3a1/uidom/examples/toggle.py
+-rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.3a1/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.3a1/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.3a1/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.3a1/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.3a1/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.3a1/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.3a1/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.3a1/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.3a1/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.3a1/uidom/routing/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.3a1/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      723 2023-05-17 09:43:23.116452 uidom-0.3a1/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0    12124 2023-05-26 17:51:41.362998 uidom-0.3a1/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.3a1/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.3a1/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8668 2023-05-17 19:14:22.872098 uidom-0.3a1/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.3a1/uidom/settings/paths.py
+-rw-r--r--   0        0        0      255 2023-05-19 08:05:54.602186 uidom-0.3a1/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.3a1/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1597 2023-05-19 08:33:44.200337 uidom-0.3a1/uidom/slots/slots.py
+-rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.3a1/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.3a1/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.3a1/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.3a1/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.3a1/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.3a1/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.3a1/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7496 2023-05-17 18:36:02.616227 uidom-0.3a1/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.3a1/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.3a1/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 uidom-0.3a1/PKG-INFO
```

### Comparing `uidom-0.3a0/LICENSE` & `uidom-0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/README.md` & `uidom-0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/pyproject.toml` & `uidom-0.3a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uidom"
-version = "0.3a0"
+version = "0.3a1"
 description = "HTML library"
 authors = ["bitplorer <bitplorer@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uidom-0.3a0/uidom/cli/__init__.py` & `uidom-0.3a1/uidom/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/cli/_cli.py` & `uidom-0.3a1/uidom/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/cli/cli.py` & `uidom-0.3a1/uidom/cli/cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/__init__.py` & `uidom-0.3a1/uidom/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/htmldocument.py` & `uidom-0.3a1/uidom/dom/htmldocument.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/htmlelement.py` & `uidom-0.3a1/uidom/dom/htmlelement.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/icons.py` & `uidom-0.3a1/uidom/dom/icons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/jinja.py` & `uidom-0.3a1/uidom/dom/jinja.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/component.py` & `uidom-0.3a1/uidom/dom/src/component.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from uidom.dom.src import csstags, htmltags, jinjatags, svgtags
 from uidom.dom.src.dom_tag import dom_tag
 from uidom.dom.src.html_string import string_to_element
 from uidom.dom.src.main import extension
 from uidom.utils.parameters import Parameters
 
-__all__ = ["Component", "ReactiveComponent"]
+__all__ = ["Component", "ReactiveComponent", "Fragment", "MergeClassAttribute"]
 
 
 @dataclass
 class Component(extension.Tags):
     left_delimiter = "<"
     right_delimiter = ">"
     css_tags = csstags
@@ -38,14 +38,16 @@
     parent: Union[html_tags.dom_tag, None] = field(init=False, default=None)
     document: Union[html_tags.dom_tag, None] = field(init=False, default=None)
     files_directory: Union[str, Path, None] = field(init=False, default=None)
     escape_string: bool = field(init=False, default=True)
     string_is_markdown: bool = field(init=False, default=False)
 
     def __init__(self, *args, **kwargs):
+        super(Component, self).__init__()
+
         global markdown
         markdown = kwargs.pop("markdown", None) or markdown
         markdown = getattr(markdown, "convert", markdown)
         # first we get the child from the render method and sanitize it.
         child = self.render(*args, **kwargs)
 
         if isinstance(child, str):
@@ -62,16 +64,17 @@
                 child = (
                     markdown(child) if self.escape_string else unescape(markdown(child))
                 )
             child = string_to_element(child, escape=self.escape_string)
 
         if isinstance(child, (list, tuple)) and len(child) == 1:
             child = child[0]
-
-        super(Component, self).__init__()
+        # commented and shifted __init__ below to the first line because then Fragment can
+        # add *args and **kwargs on initialization inside render method
+        # super(Component, self).__init__()
 
         if child is not self:
             self.add(child)
 
         self._entry = self if isinstance(child, (list, tuple)) else child
 
         # we perform checks on the _entry "after" the dom initialization because .get method
@@ -256,14 +259,75 @@
 
         raise NotImplemented(f"method: {self.call.__qualname__} not implemented")
 
     def __dir__(self) -> Iterable[str]:
         return sorted(iter(self.__dict__), key=lambda k: k)
 
 
+class Fragment(Component):
+    """Its just a placeholder which renders all its childrens
+        but not itself and passes all it attributes to its childrens.
+
+    Args:
+        None
+
+    Returns:
+        Fragment: it returns fragment which renders all its childrens
+    """
+
+    render_tag = False
+
+    def _add_attrs_to_child(self, child):
+        child.safe_attributes.update(self.safe_attributes)
+        child.add(self.attributes)
+
+    def add(self, *args):
+        for arg in args:
+            if isinstance(arg, (extension.Tags, dom_tag)):
+                self._add_attrs_to_child(arg)
+        super().add(*args)
+
+    def render(self, *args, **kwargs):
+        self.add(kwargs)
+        self.add(args)
+
+        # for this component to behave as a fragment we must simply return self
+        # Component class will take care of all the things itself.
+        return self
+
+
+class MergeClassAttribute(Fragment):
+    """Merging the attributes with subcontexts via uidom.dom.src.dom_tag.attr
+
+    Args:
+        None:
+    Usage:
+        with MergeClassAttribute():
+            attr(className=...)
+            attr(className=...)
+            div()
+            ### this div receives all the attributes set via attr methods contexts
+            ### but all the className kwargs are merged..
+
+    """
+
+    def _merge_class_attr(self, key, value):
+        if key == "class" and self.attributes.get(key, None):
+            value = " ".join([self.attributes[key], value])
+        return key, value
+
+    def set_attribute(self, key, value):
+        if key == "class":
+            key, value = self._merge_class_attr(key, value)
+
+        super().set_attribute(key, value)
+
+    __setitem__ = set_attribute
+
+
 @dataclass(eq=False)
 class ReactiveComponent(Component):
     def __init__(self, *args, **kwargs):
         super(ReactiveComponent, self).__init__(*args, **kwargs)
         self.__states: dict = kwargs
 
     def __post_init__(self, *args, **kwargs):
```

### Comparing `uidom-0.3a0/uidom/dom/src/csstags.py` & `uidom-0.3a1/uidom/dom/src/csstags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/dom1core.py` & `uidom-0.3a1/uidom/dom/src/dom1core.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/dom_tag.py` & `uidom-0.3a1/uidom/dom/src/dom_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 def _get_thread_context():
     context = [threading.current_thread()]
     if greenlet:
         context.append(greenlet.getcurrent())
     return hash(tuple(context))
 
 
+class dom_string(basestring):
+    pass
+
+
 class dom_tag(object):
     is_single = False  # Tag does not require matching end tag (ex. <hr/>)
     is_pretty = True  # Text inside the tag should be left as-is (ex. <pre>)
     # otherwise, text will be escaped() and whitespace may be
     # modified
     is_inline = False
     escape_string = True
@@ -77,26 +81,26 @@
         There is a non-rendering attribute which controls how the tag renders:
 
         * `__inline` - Boolean value. If True renders all children tags on the same
                        line.
         """
 
         self.attributes = {}
-        self.children = []
+        self.children: typing.List[typing.Union[str, dom_tag]] = []
         self.parent = None
         self.document = None
 
         # Does not insert newlines on all children if True (recursive attribute)
         self.is_inline = kwargs.pop("__inline", self.is_inline)
         self.is_pretty = kwargs.pop("__pretty", self.is_pretty)
         self.escape_string = kwargs.pop("__escape_string", self.escape_string)
 
         # Add child elements
         if args:
-            self.add(args)
+            self.add(*args)
 
         for attr, value in kwargs.items():
             self.set_attribute(*type(self).clean_pair(attr, value))
 
         # this is where the this class instance is added to the parent context via _add_to_context
         self._ctx: typing.Optional[dom_tag.frame] = None
         self._add_to_ctx()
@@ -206,14 +210,22 @@
                 # we are going to add the support for escaping only those strings whoes parents
                 # have explicit variable "escape_string" set to True
                 if hasattr(self, "escape_string"):
                     if self.escape_string:
                         obj = escape(obj)
                 else:
                     obj = escape(obj)
+
+                # we are wrapping str into dom_string because when we use .get method we may
+                # for some reason want to get the parent of the string values in children,
+                # natively its not possible so we wrap str in dom_string and set self as parent
+
+                obj = dom_string(obj) if not isinstance(obj, dom_string) else obj
+                obj.parent = self
+
                 self.children.append(obj)
 
             elif isinstance(obj, dom_tag):
                 stack = dom_tag._with_contexts.get(_get_thread_context(), [])
                 for s in stack:
                     s.used.add(obj)
```

### Comparing `uidom-0.3a0/uidom/dom/src/ext.py` & `uidom-0.3a1/uidom/dom/src/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     SELF_DEDENT = "self_dedent"
     CHILD_DEDENT = "child_dedent"
     OPEN_TAG = "open_tag"
     CLOSE_TAG = "close_tag"
     RENDER_TAG = "render_tag"
     file_extension = ".html"
     attribute_prefix_map: dict = {}
+    safe_attributes: dict = {}
 
     def __init__(self, *args, **kwargs):
         # if any(args):
         # msg = f"can only pass {dom_tag!r} or {str!r} types in arguments, got {args!r} instead"
         # if not all(map(lambda x: isinstance(x, (dom_tag, str)), args)):
         #     raise TypeError(msg)
         super(Tags, self).__init__(*args, **kwargs)
@@ -59,38 +60,52 @@
     ):
         if open_tag:
             sb.append("%s" % open_tag)
         else:
             # open tag is absent
             sb.append(self.left_delimiter)
             sb.append(name)
-            sb = self._render_attribute(sb)
+            sb = self._render_attribute(sb, indent_level, indent_str, pretty)
             sb.append(
                 "".join(["/", self.right_delimiter])
                 if self.is_single and xhtml
                 else self.right_delimiter
             )
         return sb
 
-    def _render_attribute(self, sb):
+    def _wrap_attr_value(self, value, indent_level, indent_str, pretty):
+        # adding support to write multiline tailwindcss classes
+        multiline_string = textwrap.dedent(value)
+        wrapped_string = textwrap.fill(
+            multiline_string,
+            break_long_words=False,
+            break_on_hyphens=False,
+        )
+        value = re.sub(r"\s+", " ", wrapped_string.strip())
+
+        return value
+
+    def _render_attribute(self, sb, indent_level, indent_str, pretty):
         for attribute, value in sorted(self.attributes.items()):
             if value is not False and value not in [
                 None
             ]:  # False values must be omitted completely
                 if attribute == "class":
-                    # adding support to write multiline tailwindcss classes
-                    multiline_string = textwrap.dedent(value)
-                    wrapped_string = textwrap.fill(
-                        multiline_string, break_long_words=False, break_on_hyphens=False
+                    value = self._wrap_attr_value(
+                        value, indent_level, indent_str, pretty
                     )
-                    value = re.sub(r"\s+", " ", wrapped_string.strip())
                 if not isinstance(
                     value, (typing.MutableMapping, typing.MutableSequence)
                 ):
-                    sb.append(' %s="%s"' % (attribute, escape(unicode(value), True)))
+                    if self.safe_attributes.get(attribute, True):
+                        sb.append(
+                            ' %s="%s"' % (attribute, escape(unicode(value), True))
+                        )
+                    else:
+                        sb.append(' %s="%s"' % (attribute, unicode(value)))
                 else:
                     value = htmlsafe_json_dumps(value)
                     sb.append(
                         " %s='%s'" % (attribute, escape(unicode(value), quote=False))
                     )
             if value in [None]:  # minified xhtml attributes are added
                 sb.append(" %s" % attribute)
@@ -101,15 +116,14 @@
             sb.append("%s" % close_tag)
         else:
             sb.append("".join([self.left_delimiter, "/"]))
             sb.append(name)
             sb.append(self.right_delimiter)
         return sb
 
-    # @staticmethod
     def _new_line_and_inline_handler(
         self, sb, indent_level, indent_str, pretty, is_inline
     ):
         if pretty and not is_inline:
             is_inline = False
             sb.append(self.new_line)
             sb.append(indent_str * indent_level)
@@ -139,15 +153,15 @@
         }.get(attribute, attribute)
 
         # Workaround for Python's reserved words
         if len(attribute) >= 2:
             if attribute[0] == "_" and attribute[1] != "_":
                 attribute = attribute[1:]
 
-        # Workaround for dash plus support for VueJS, HTMX, Unpoly and AngularJS
+        # Workaround for dash plus support for VueJS, HTMX, AlpineJS, Unpoly and AngularJS
         special_prefix = any(
             [
                 attribute.startswith(x)
                 for x in (
                     "data_",  # for data-type="value" support
                     "aria_",  # for aria support
                     "x_",  # for AlpineJS and x-component support
@@ -165,18 +179,16 @@
         if attribute in {"http_equiv"} or special_prefix:
             attribute = attribute.replace("_", "-")
             attribute = attribute.replace("--", ":")
             attribute = attribute.replace("v-bind-", ":")
             attribute = attribute.replace("v-bind", "")
             attribute = attribute.replace("x-bind-", ":")
             attribute = attribute.replace("x-bind", "")
-            attribute = attribute.replace("x-transition-enter", "x-transition:enter")
-            attribute = attribute.replace("x-transition-leave", "x-transition:leave")
-            attribute = attribute.replace("x-intersect-enter", "x-intersect:enter")
-            attribute = attribute.replace("x-intersect-leave", "x-intersect:leave")
+            attribute = attribute.replace("-enter", ":enter")
+            attribute = attribute.replace("-leave", ":leave")
             attribute = attribute.replace("v-on:", "@")
             attribute = attribute.replace("v-on-", "@")
             attribute = attribute.replace("x-on:", "@")
             attribute = attribute.replace("x-on-", "@")
             attribute = attribute.replace("-dot-", ".")
             if attribute in cls.attribute_prefix_map:
                 attribute = attribute.replace(
@@ -469,14 +481,17 @@
     def __and__(self, other: dom_tag) -> "Tags":
         return (
             PlaceholderTag(__inline=self.is_inline, __pretty=self.is_pretty)
             & self
             & other
         )
 
+    def __iter__(self) -> typing.List[typing.Union[str, dom_tag, "Tags"]]:
+        return super().__iter__()
+
     def save(
         self,
         file_name: typing.Union[str, Path, None] = None,
         folder_name: typing.Union[str, Path, None] = None,
         current_dir: bool = False,
         file_or_dir: typing.Union[str, Path, None] = None,
     ):
```

### Comparing `uidom-0.3a0/uidom/dom/src/html_string.py` & `uidom-0.3a1/uidom/dom/src/html_string.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/htmltags.py` & `uidom-0.3a1/uidom/dom/src/htmltags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/jinjatags.py` & `uidom-0.3a1/uidom/dom/src/jinjatags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/parse_html.py` & `uidom-0.3a1/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/pythontags.py` & `uidom-0.3a1/uidom/dom/src/pythontags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/sphinxtags.py` & `uidom-0.3a1/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/svgtags.py` & `uidom-0.3a1/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/utils/dom_util.py` & `uidom-0.3a1/uidom/dom/src/utils/dom_util.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/utils/sheets.py` & `uidom-0.3a1/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/src/ws_rpc.py` & `uidom-0.3a1/uidom/dom/src/ws_rpc.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/ui.py` & `uidom-0.3a1/uidom/dom/ui.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/dom/uniqueid.py` & `uidom-0.3a1/uidom/dom/uniqueid.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/edge_db/ql.py` & `uidom-0.3a1/uidom/edge_db/ql.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/booleans.py` & `uidom-0.3a1/uidom/elements/booleans.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/buttons.py` & `uidom-0.3a1/uidom/elements/buttons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/chars.py` & `uidom-0.3a1/uidom/elements/chars.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/dates.py` & `uidom-0.3a1/uidom/elements/dates.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/enums.py` & `uidom-0.3a1/uidom/elements/enums.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/floats.py` & `uidom-0.3a1/uidom/elements/floats.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/elements/integers.py` & `uidom-0.3a1/uidom/elements/integers.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/examples/links.py` & `uidom-0.3a1/uidom/examples/links.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/examples/toggle.py` & `uidom-0.3a1/uidom/examples/toggle.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/reloader/_app.py` & `uidom-0.3a1/uidom/reloader/_app.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/reloader/_notify.py` & `uidom-0.3a1/uidom/reloader/_notify.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/reloader/_watch.py` & `uidom-0.3a1/uidom/reloader/_watch.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/reloader/script/reloader.js` & `uidom-0.3a1/uidom/reloader/script/reloader.js`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/response/starlette.py` & `uidom-0.3a1/uidom/response/starlette.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/routing/fastapi.py` & `uidom-0.3a1/uidom/routing/fastapi.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/scripts/__init__.py` & `uidom-0.3a1/uidom/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/scripts/xcomponent.js` & `uidom-0.3a1/uidom/scripts/xcomponent.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -153,15 +153,20 @@
                 }
                 this.shadow = shadow;
                 this.checkOrCreateId();
                 document.addEventListener('alpine:initialized', () => {
                     Alpine.initTree(this.shadow);
                 });
             } else {
-                this.append(component.content.cloneNode(true));
+                if (!!template) {
+                    this.append(component.content.cloneNode(true));
+                } else {
+                    this.append(component.cloneNode(true));
+                }
+
                 this.checkOrCreateId();
                 document.addEventListener('alpine:initialized', () => {
                     Alpine.initTree(this);
                 });
             }
```

### Comparing `uidom-0.3a0/uidom/settings/commands.py` & `uidom-0.3a1/uidom/settings/commands.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/settings/document.py` & `uidom-0.3a1/uidom/settings/document.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/settings/paths.py` & `uidom-0.3a1/uidom/settings/paths.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/slots/custom_element_slot.py` & `uidom-0.3a1/uidom/slots/custom_element_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/slots/slots.py` & `uidom-0.3a1/uidom/slots/slots.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/slots/web_component_slot.py` & `uidom-0.3a1/uidom/slots/web_component_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/utils/functional.py` & `uidom-0.3a1/uidom/utils/functional.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/utils/logger.py` & `uidom-0.3a1/uidom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/utils/parameters.py` & `uidom-0.3a1/uidom/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/web_io/_adapter.py` & `uidom-0.3a1/uidom/web_io/_adapter.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/web_io/_events.py` & `uidom-0.3a1/uidom/web_io/_events.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/uidom/web_io/_protocol.py` & `uidom-0.3a1/uidom/web_io/_protocol.py`

 * *Files identical despite different names*

### Comparing `uidom-0.3a0/PKG-INFO` & `uidom-0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uidom
-Version: 0.3a0
+Version: 0.3a1
 Summary: HTML library
 License: MIT
 Author: bitplorer
 Author-email: bitplorer@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

