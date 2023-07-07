# Comparing `tmp/iricore-1.4.6.tar.gz` & `tmp/iricore-1.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iricore-1.4.6.tar", max compression
+gzip compressed data, was "iricore-1.5.0.dev0.tar", max compression
```

## Comparing `iricore-1.4.6.tar` & `iricore-1.5.0.dev0.tar`

### file list

```diff
@@ -1,141 +1,139 @@
--rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.4.6/LICENSE
--rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.4.6/README.md
--rwxr-xr-x   0        0        0      463 2022-11-10 03:07:50.807105 iricore-1.4.6/build.py
--rwxr-xr-x   0        0        0      641 2023-06-16 02:20:34.377596 iricore-1.4.6/pyproject.toml
--rwxr-xr-x   0        0        0      431 2023-06-16 02:04:11.203309 iricore-1.4.6/src/iricore/CMakeLists.txt
--rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.4.6/src/iricore/__init__.py
--rw-r--r--   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.4.6/src/iricore/config.py
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020s.dat
--rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.4.6/src/iricore/data/data16/index/apf107.dat
--rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.4.6/src/iricore/data/data16/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi22.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2015-02-11 20:37:48.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020s.dat
--rw-r--r--   0        0        0  1324624 2022-10-07 03:31:18.000000 iricore-1.4.6/src/iricore/data/data20/index/apf107.dat
--rw-r--r--   0        0        0     9823 2022-10-07 03:33:30.000000 iricore-1.4.6/src/iricore/data/data20/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi22.asc
--rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/data_update.py
--rwxr-xr-x   0        0        0     9332 2023-06-16 02:19:12.764327 iricore-1.4.6/src/iricore/iri.py
--rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/iri2016/cira.for
--rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/iri2016/igrf.for
--rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.4.6/src/iricore/iri2016/iridreg.for
--rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.4.6/src/iricore/iri2016/iriflip.for
--rwxr-xr-x   0        0        0   485167 2023-06-12 18:38:06.344577 iricore-1.4.6/src/iricore/iri2016/irifun.for
--rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.4.6/src/iricore/iri2016/irirtam.for
--rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.4.6/src/iricore/iri2016/irisub.for
--rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.4.6/src/iricore/iri2016/iritec.for
--rw-r--r--   0        0        0   112771 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/cira.for
--rw-r--r--   0        0        0   161131 2023-06-12 18:46:31.728823 iricore-1.4.6/src/iricore/iri2020/igrf.for
--rw-r--r--   0        0        0  1315925 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/iridreg.for
--rw-r--r--   0        0        0    87909 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/iriflip.for
--rw-r--r--   0        0        0   580220 2023-06-12 18:49:14.319628 iricore-1.4.6/src/iricore/iri2020/irifun.for
--rw-r--r--   0        0        0     6147 2023-06-12 18:52:43.590118 iricore-1.4.6/src/iricore/iri2020/irirtam.for
--rw-r--r--   0        0        0    88920 2023-06-12 18:52:43.622117 iricore-1.4.6/src/iricore/iri2020/irisub.for
--rw-r--r--   0        0        0   623932 2023-03-19 02:54:42.000000 iricore-1.4.6/src/iricore/iri2020/rocdrift.for
--rw-r--r--   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.4.6/src/iricore/modules.py
--rwxr-xr-x   0        0        0     1317 2023-06-16 02:18:13.523470 iricore-1.4.6/src/iricore/python_interface.f90
--rw-r--r--   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.4.6/src/iricore/python_stec.f90
--rw-r--r--   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.4.6/src/iricore/read_iri_data.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 iricore-1.4.6/setup.py
--rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 iricore-1.4.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.5.0.dev0/LICENSE
+-rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.5.0.dev0/README.md
+-rwxr-xr-x   0        0        0     1631 2023-07-07 20:47:14.897104 iricore-1.5.0.dev0/build.py
+-rw-r--r--   0        0        0     1085 2023-07-07 20:35:26.791475 iricore-1.5.0.dev0/pyproject.toml
+-rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.5.0.dev0/src/iricore/__init__.py
+-rwxr-xr-x   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.5.0.dev0/src/iricore/config.py
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir11.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir12.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir13.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir14.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir15.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir16.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir17.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir18.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir19.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir20.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir21.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir22.asc
+-rwxr-xr-x   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1945.dat
+-rwxr-xr-x   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1950.dat
+-rwxr-xr-x   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1955.dat
+-rwxr-xr-x   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1960.dat
+-rwxr-xr-x   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1965.dat
+-rwxr-xr-x   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1970.dat
+-rwxr-xr-x   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1975.dat
+-rwxr-xr-x   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1980.dat
+-rwxr-xr-x   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1985.dat
+-rwxr-xr-x   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1990.dat
+-rwxr-xr-x   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf1995.dat
+-rwxr-xr-x   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2000.dat
+-rwxr-xr-x   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2005.dat
+-rwxr-xr-x   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2010.dat
+-rwxr-xr-x   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2015.dat
+-rwxr-xr-x   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/igrf2020.dat
+-rwxr-xr-x   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.5.0.dev0/src/iricore/data/data16/igrf/igrf2020s.dat
+-rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.5.0.dev0/src/iricore/data/data16/index/apf107.dat
+-rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.5.0.dev0/src/iricore/data/data16/index/ig_rz.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat11.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat12.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat13.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat14.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat15.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat16.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat17.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat18.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat19.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat20.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat21.dat
+-rwxr-xr-x   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat22.dat
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi11.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi12.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi13.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi14.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi15.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi16.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi17.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi18.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi19.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi20.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi21.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi22.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir11.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir12.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir13.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir14.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir15.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir16.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir17.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir18.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir19.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir20.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir21.asc
+-rwxr-xr-x   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir22.asc
+-rwxr-xr-x   0        0        0      443 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1945.dat
+-rwxr-xr-x   0        0        0      445 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1950.dat
+-rwxr-xr-x   0        0        0      437 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1955.dat
+-rwxr-xr-x   0        0        0      431 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1960.dat
+-rwxr-xr-x   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1965.dat
+-rwxr-xr-x   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1970.dat
+-rwxr-xr-x   0        0        0      439 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1975.dat
+-rwxr-xr-x   0        0        0      436 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1980.dat
+-rwxr-xr-x   0        0        0      433 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1985.dat
+-rwxr-xr-x   0        0        0      434 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1990.dat
+-rwxr-xr-x   0        0        0      438 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf1995.dat
+-rwxr-xr-x   0        0        0     1015 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2000.dat
+-rwxr-xr-x   0        0        0     1219 2011-12-16 23:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2005.dat
+-rwxr-xr-x   0        0        0     1218 2015-02-11 20:37:48.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2010.dat
+-rwxr-xr-x   0        0        0     1188 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2015.dat
+-rwxr-xr-x   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/igrf2020.dat
+-rwxr-xr-x   0        0        0      598 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/igrf/igrf2020s.dat
+-rwxr-xr-x   0        0        0  1324624 2022-10-07 03:31:18.000000 iricore-1.5.0.dev0/src/iricore/data/data20/index/apf107.dat
+-rwxr-xr-x   0        0        0     9823 2022-10-07 03:33:30.000000 iricore-1.5.0.dev0/src/iricore/data/data20/index/ig_rz.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat11.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat12.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat13.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat14.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat15.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat16.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat17.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat18.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat19.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat20.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat21.dat
+-rwxr-xr-x   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat22.dat
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi11.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi12.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi13.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi14.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi15.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi16.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi17.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi18.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi19.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi20.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi21.asc
+-rwxr-xr-x   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi22.asc
+-rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.5.0.dev0/src/iricore/data_update.py
+-rwxr-xr-x   0        0        0     9332 2023-06-16 02:19:12.764327 iricore-1.5.0.dev0/src/iricore/iri.py
+-rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.5.0.dev0/src/iricore/iri2016/cira.for
+-rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.5.0.dev0/src/iricore/iri2016/igrf.for
+-rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.5.0.dev0/src/iricore/iri2016/iridreg.for
+-rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.5.0.dev0/src/iricore/iri2016/iriflip.for
+-rwxr-xr-x   0        0        0   485167 2023-06-12 18:38:06.344577 iricore-1.5.0.dev0/src/iricore/iri2016/irifun.for
+-rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.5.0.dev0/src/iricore/iri2016/irirtam.for
+-rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.5.0.dev0/src/iricore/iri2016/irisub.for
+-rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.5.0.dev0/src/iricore/iri2016/iritec.for
+-rwxr-xr-x   0        0        0   112771 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/iri2020/cira.for
+-rwxr-xr-x   0        0        0   161131 2023-06-12 18:46:31.728823 iricore-1.5.0.dev0/src/iricore/iri2020/igrf.for
+-rwxr-xr-x   0        0        0  1315925 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/iri2020/iridreg.for
+-rwxr-xr-x   0        0        0    87909 2022-09-06 07:12:00.000000 iricore-1.5.0.dev0/src/iricore/iri2020/iriflip.for
+-rwxr-xr-x   0        0        0   580220 2023-06-12 18:49:14.319628 iricore-1.5.0.dev0/src/iricore/iri2020/irifun.for
+-rwxr-xr-x   0        0        0     6147 2023-06-12 18:52:43.590118 iricore-1.5.0.dev0/src/iricore/iri2020/irirtam.for
+-rwxr-xr-x   0        0        0    88920 2023-06-12 18:52:43.622117 iricore-1.5.0.dev0/src/iricore/iri2020/irisub.for
+-rwxr-xr-x   0        0        0   623932 2023-03-19 02:54:42.000000 iricore-1.5.0.dev0/src/iricore/iri2020/rocdrift.for
+-rwxr-xr-x   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.5.0.dev0/src/iricore/modules.py
+-rwxr-xr-x   0        0        0     1317 2023-06-16 02:18:13.523470 iricore-1.5.0.dev0/src/iricore/python_interface.f90
+-rwxr-xr-x   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.5.0.dev0/src/iricore/python_stec.f90
+-rwxr-xr-x   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.5.0.dev0/src/iricore/read_iri_data.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 iricore-1.5.0.dev0/PKG-INFO
```

### Comparing `iricore-1.4.6/LICENSE` & `iricore-1.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/README.md` & `iricore-1.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir11.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir12.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir13.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir14.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir15.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir16.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir17.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir18.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir19.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir20.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir21.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ccir/ccir22.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2000.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2005.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2010.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2015.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020s.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/index/apf107.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/index/ig_rz.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat11.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat12.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat13.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat14.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat15.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat16.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat17.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat18.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat19.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat20.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat21.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat22.dat` & `iricore-1.5.0.dev0/src/iricore/data/data16/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi11.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi12.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi13.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi14.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi15.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi16.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi17.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi18.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi19.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi20.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi21.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data16/ursi/ursi22.asc` & `iricore-1.5.0.dev0/src/iricore/data/data16/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir11.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir12.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir13.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir14.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir15.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir16.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir17.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir18.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir19.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir20.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir21.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ccir/ccir22.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2000.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2005.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2010.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2015.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020s.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/index/apf107.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/index/ig_rz.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat11.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat12.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat13.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat14.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat15.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat16.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat17.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat18.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat19.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat20.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat21.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat22.dat` & `iricore-1.5.0.dev0/src/iricore/data/data20/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi11.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi12.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi13.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi14.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi15.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi16.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi17.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi18.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi19.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi20.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi21.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data/data20/ursi/ursi22.asc` & `iricore-1.5.0.dev0/src/iricore/data/data20/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/data_update.py` & `iricore-1.5.0.dev0/src/iricore/data_update.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri.py` & `iricore-1.5.0.dev0/src/iricore/iri.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/cira.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/igrf.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/iridreg.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/iriflip.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/irifun.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/irirtam.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/irisub.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2016/iritec.for` & `iricore-1.5.0.dev0/src/iricore/iri2016/iritec.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/cira.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/igrf.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/iridreg.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/iriflip.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/irifun.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/irirtam.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/irisub.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/iri2020/rocdrift.for` & `iricore-1.5.0.dev0/src/iricore/iri2020/rocdrift.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/modules.py` & `iricore-1.5.0.dev0/src/iricore/modules.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/python_interface.f90` & `iricore-1.5.0.dev0/src/iricore/python_interface.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/python_stec.f90` & `iricore-1.5.0.dev0/src/iricore/python_stec.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/src/iricore/read_iri_data.py` & `iricore-1.5.0.dev0/src/iricore/read_iri_data.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.6/PKG-INFO` & `iricore-1.5.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: iricore
-Version: 1.4.6
-Summary: 
+Version: 1.5.0.dev0
+Summary: A Python wraper to the Inernational Ionosphere Model
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fortranformat (>=1.2.2,<2.0.0)
-Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: fortranformat (>=2.0.0,<3.0.0)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pymap3d (>=3.0.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # iricore
 A Python interface to IRI-2016 and IRI-2020 using `ctypes` communication.
 
 **Important!** Because this package is mainly used for the [MIST experiment](http://www.physics.mcgill.ca/mist/),
```

