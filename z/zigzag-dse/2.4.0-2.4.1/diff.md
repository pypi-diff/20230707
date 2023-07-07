# Comparing `tmp/zigzag-dse-2.4.0.tar.gz` & `tmp/zigzag-dse-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag-dse-2.4.0.tar", last modified: Fri Jun 30 16:05:54 2023, max compression
+gzip compressed data, was "zigzag-dse-2.4.1.tar", last modified: Fri Jul  7 19:18:02 2023, max compression
```

## Comparing `zigzag-dse-2.4.0.tar` & `zigzag-dse-2.4.1.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.386956 zigzag-dse-2.4.0/
--rw-r--r--   0 lmei     (17911) micas     (3600)     1522 2022-09-20 14:53:33.000000 zigzag-dse-2.4.0/LICENSE
--rw-r--r--   0 lmei     (17911) micas     (3600)       88 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/MANIFEST.in
--rw-r--r--   0 lmei     (17911) micas     (3600)     9080 2023-06-30 16:05:54.385956 zigzag-dse-2.4.0/PKG-INFO
--rw-r--r--   0 lmei     (17911) micas     (3600)     6758 2023-06-30 15:54:38.000000 zigzag-dse-2.4.0/README.md
--rw-r--r--   0 lmei     (17911) micas     (3600)     1601 2023-06-30 16:05:21.000000 zigzag-dse-2.4.0/pyproject.toml
--rw-r--r--   0 lmei     (17911) micas     (3600)       38 2023-06-30 16:05:54.386956 zigzag-dse-2.4.0/setup.cfg
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.273868 zigzag-dse-2.4.0/zigzag/
--rw-r--r--   0 lmei     (17911) micas     (3600)       22 2023-06-30 16:05:21.000000 zigzag-dse-2.4.0/zigzag/__init__.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2497 2022-11-17 18:55:03.000000 zigzag-dse-2.4.0/zigzag/__main__.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     4451 2023-06-30 15:54:55.000000 zigzag-dse-2.4.0/zigzag/api.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.287868 zigzag-dse-2.4.0/zigzag/classes/
--rw-r--r--   0 lmei     (17911) micas     (3600)        0 2022-11-17 18:55:03.000000 zigzag-dse-2.4.0/zigzag/classes/__init__.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.306869 zigzag-dse-2.4.0/zigzag/classes/cacti/
--rw-r--r--   0 lmei     (17911) micas     (3600)      291 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.343871 zigzag-dse-2.4.0/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 lmei     (17911) micas     (3600)     3494 2023-06-14 18:48:20.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.121903 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 lmei     (17911) micas     (3600)     6576 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     6555 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     6920 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     5324 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 lmei     (17911) micas     (3600)     9282 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3322 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    41184 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3607 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/Ucache.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     5116 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2771 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     2057 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2416 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     8474 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2664 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    29279 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     7364 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    11041 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 lmei     (17911) micas     (3600)    32713 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 lmei     (17911) micas     (3600)  2421320 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 lmei     (17911) micas     (3600)      173 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 lmei     (17911) micas     (3600)     1334 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 lmei     (17911) micas     (3600)    25297 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     5586 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)    27215 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     3569 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     7561 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2837 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     9565 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     5001 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     7349 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3204 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     9849 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)    62337 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     7405 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     3712 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     9750 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 lmei     (17911) micas     (3600)    17411 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)      878 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    46185 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     9068 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    23772 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3595 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 lmei     (17911) micas     (3600)   133713 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2116 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     9850 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     7217 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)      407 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 lmei     (17911) micas     (3600)    94813 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     6122 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    16630 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)      553 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    11483 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     4490 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    29014 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     5426 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    19629 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3306 2023-06-02 15:50:57.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.816932 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 lmei     (17911) micas     (3600)   134304 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   352744 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   157960 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   124352 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   156624 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   155192 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 lmei     (17911) micas     (3600)  2421320 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 lmei     (17911) micas     (3600)   175768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   159768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   160680 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   207224 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   145592 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   180464 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   178384 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   411960 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   192248 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   270320 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   569648 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   280416 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   204480 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   256824 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   313848 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   124400 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   175432 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   128080 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   144976 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   228000 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   232752 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 lmei     (17911) micas     (3600)   111980 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)    20306 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     5286 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3055 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 lmei     (17911) micas     (3600)     1886 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 lmei     (17911) micas     (3600)    10212 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     3721 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.846933 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 lmei     (17911) micas     (3600)     8781 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     8768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     8780 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)     8784 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.858934 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 lmei     (17911) micas     (3600)     9545 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 lmei     (17911) micas     (3600)      579 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 lmei     (17911) micas     (3600)     8332 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     2542 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.923936 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 lmei     (17911) micas     (3600)       25 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)    23666 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     3842 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     4575 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     4759 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     4755 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)    24571 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     4758 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)    24570 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)     4742 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 lmei     (17911) micas     (3600)    15087 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)    41317 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     4035 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     2064 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 lmei     (17911) micas     (3600)    29856 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 lmei     (17911) micas     (3600)     4375 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 lmei     (17911) micas     (3600)     6110 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.927937 zigzag-dse-2.4.0/zigzag/classes/cost_model/
--rw-r--r--   0 lmei     (17911) micas     (3600)    63132 2023-06-30 15:54:38.000000 zigzag-dse-2.4.0/zigzag/classes/cost_model/cost_model.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.201865 zigzag-dse-2.4.0/zigzag/classes/hardware/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.987939 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/
--rw-r--r--   0 lmei     (17911) micas     (3600)     1278 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     9441 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     6460 2023-06-30 15:54:38.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      918 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 lmei     (17911) micas     (3600)    11764 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3567 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 lmei     (17911) micas     (3600)    12231 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3014 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1874 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.204865 zigzag-dse-2.4.0/zigzag/classes/io/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:53.991939 zigzag-dse-2.4.0/zigzag/classes/io/accelerator/
--rw-r--r--   0 lmei     (17911) micas     (3600)     2805 2022-11-17 18:55:03.000000 zigzag-dse-2.4.0/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.039941 zigzag-dse-2.4.0/zigzag/classes/io/onnx/
--rw-r--r--   0 lmei     (17911) micas     (3600)     7087 2023-06-14 18:45:40.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      884 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     5382 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3679 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     4912 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1163 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     4089 2023-06-14 18:45:40.000000 zigzag-dse-2.4.0/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.063942 zigzag-dse-2.4.0/zigzag/classes/mapping/
--rw-r--r--   0 lmei     (17911) micas     (3600)    40951 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      637 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/loop.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     9386 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.068942 zigzag-dse-2.4.0/zigzag/classes/mapping/memory/
--rw-r--r--   0 lmei     (17911) micas     (3600)        0 2022-11-17 18:55:04.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.070942 zigzag-dse-2.4.0/zigzag/classes/mapping/spatial/
--rw-r--r--   0 lmei     (17911) micas     (3600)     7655 2023-06-14 18:45:40.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.077943 zigzag-dse-2.4.0/zigzag/classes/mapping/temporal/
--rw-r--r--   0 lmei     (17911) micas     (3600)      380 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     7412 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.215865 zigzag-dse-2.4.0/zigzag/classes/opt/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.081943 zigzag-dse-2.4.0/zigzag/classes/opt/spatial/
--rw-r--r--   0 lmei     (17911) micas     (3600)     7044 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.221866 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.096943 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 lmei     (17911) micas     (3600)    11591 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      489 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 lmei     (17911) micas     (3600)    15479 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2837 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.104944 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 lmei     (17911) micas     (3600)     8726 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3616 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.212948 zigzag-dse-2.4.0/zigzag/classes/stages/
--rw-r--r--   0 lmei     (17911) micas     (3600)     2054 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1552 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3240 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2105 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2163 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      966 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1568 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     6204 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     6260 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     6546 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     6997 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     8158 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3906 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2593 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/Stage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     4046 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1187 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2821 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.234949 zigzag-dse-2.4.0/zigzag/classes/workload/
--rw-r--r--   0 lmei     (17911) micas     (3600)     2468 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     2210 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 lmei     (17911) micas     (3600)    21102 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1542 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 lmei     (17911) micas     (3600)    14521 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.230866 zigzag-dse-2.4.0/zigzag/inputs/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.234866 zigzag-dse-2.4.0/zigzag/inputs/examples/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.254950 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/
--rw-r--r--   0 lmei     (17911) micas     (3600)     8448 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     5849 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     5746 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     7098 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     5112 2023-06-19 17:19:39.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     7287 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.293952 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/
--rw-r--r--   0 lmei     (17911) micas     (3600)      561 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/assend_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      196 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/default.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      832 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      560 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      610 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      557 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.342954 zigzag-dse-2.4.0/zigzag/inputs/examples/workload/
--rw-r--r--   0 lmei     (17911) micas     (3600)     4067 2023-01-11 10:28:45.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 lmei     (17911) micas     (3600)    71724 2023-01-11 10:28:45.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 lmei     (17911) micas     (3600)    18600 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/workload/resnet18.onnx
--rw-r--r--   0 lmei     (17911) micas     (3600)    19065 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/inputs/examples/workload/resnet18.py
--rw-r--r--   0 lmei     (17911) micas     (3600)      504 2022-11-17 18:55:04.000000 zigzag-dse-2.4.0/zigzag/utils.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:52.237866 zigzag-dse-2.4.0/zigzag/visualization/
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.349954 zigzag-dse-2.4.0/zigzag/visualization/graph/
--rw-r--r--   0 lmei     (17911) micas     (3600)     1527 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     1280 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.361955 zigzag-dse-2.4.0/zigzag/visualization/results/
--rw-r--r--   0 lmei     (17911) micas     (3600)     8773 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 lmei     (17911) micas     (3600)     3951 2023-06-02 15:50:58.000000 zigzag-dse-2.4.0/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-06-30 16:05:54.382955 zigzag-dse-2.4.0/zigzag_dse.egg-info/
--rw-r--r--   0 lmei     (17911) micas     (3600)     9080 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 lmei     (17911) micas     (3600)     9476 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 lmei     (17911) micas     (3600)        1 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 lmei     (17911) micas     (3600)       52 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 lmei     (17911) micas     (3600)      144 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 lmei     (17911) micas     (3600)       34 2023-06-30 16:05:52.000000 zigzag-dse-2.4.0/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.658456 zigzag-dse-2.4.1/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1522 2022-09-20 14:53:33.000000 zigzag-dse-2.4.1/LICENSE
+-rw-r--r--   0 lmei     (17911) micas     (3600)       88 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/MANIFEST.in
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9644 2023-07-07 19:18:02.656456 zigzag-dse-2.4.1/PKG-INFO
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7322 2023-07-07 19:14:05.000000 zigzag-dse-2.4.1/README.md
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1601 2023-07-07 19:17:50.000000 zigzag-dse-2.4.1/pyproject.toml
+-rw-r--r--   0 lmei     (17911) micas     (3600)       38 2023-07-07 19:18:02.659456 zigzag-dse-2.4.1/setup.cfg
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.471406 zigzag-dse-2.4.1/zigzag/
+-rw-r--r--   0 lmei     (17911) micas     (3600)       22 2023-07-07 19:17:50.000000 zigzag-dse-2.4.1/zigzag/__init__.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2497 2022-11-17 18:55:03.000000 zigzag-dse-2.4.1/zigzag/__main__.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4451 2023-06-30 15:54:55.000000 zigzag-dse-2.4.1/zigzag/api.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.475406 zigzag-dse-2.4.1/zigzag/classes/
+-rw-r--r--   0 lmei     (17911) micas     (3600)        0 2022-11-17 18:55:03.000000 zigzag-dse-2.4.1/zigzag/classes/__init__.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.493407 zigzag-dse-2.4.1/zigzag/classes/cacti/
+-rw-r--r--   0 lmei     (17911) micas     (3600)      291 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/README.md
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.501407 zigzag-dse-2.4.1/zigzag/classes/cacti/__pycache__/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3494 2023-06-14 18:48:20.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.907425 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6576 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6555 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6920 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5324 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/README
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9282 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/TSV.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3322 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/TSV.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    41184 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/Ucache.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3607 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/Ucache.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5116 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/arbiter.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2771 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/arbiter.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2057 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/area.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2416 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/area.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8474 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/bank.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2664 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/bank.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    29279 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/basic_circuit.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7364 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/basic_circuit.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    11041 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cache.cfg_temp
+-rw-r--r--   0 lmei     (17911) micas     (3600)    32713 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
+-rwxr-xr-x   0 lmei     (17911) micas     (3600)  2421320 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti
+-rw-r--r--   0 lmei     (17911) micas     (3600)      173 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti.i
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1334 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti.mk
+-rw-r--r--   0 lmei     (17911) micas     (3600)    25297 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5586 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_interface.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)    27215 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_interface.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3569 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7561 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/component.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2837 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/component.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9565 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/const.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5001 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/contention.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7349 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/crossbar.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3204 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/crossbar.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9849 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/ddr3.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)    62337 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/decoder.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7405 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/decoder.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3712 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/dram.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9750 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
+-rw-r--r--   0 lmei     (17911) micas     (3600)    17411 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)      878 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    46185 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio_technology.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9068 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio_technology.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    23772 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/htree2.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3595 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/htree2.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)   133713 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/io.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2116 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/io.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9850 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/lpddr.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7217 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/main.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)      407 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/makefile
+-rw-r--r--   0 lmei     (17911) micas     (3600)    94813 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/mat.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6122 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/mat.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    16630 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)      553 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    11483 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4490 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad_parameters.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    29014 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memorybus.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5426 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memorybus.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    19629 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/nuca.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3306 2023-06-02 15:50:57.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/nuca.h
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.157435 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/
+-rw-r--r--   0 lmei     (17911) micas     (3600)   134304 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   352744 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   157960 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   124352 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   156624 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   155192 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
+-rwxr-xr-x   0 lmei     (17911) micas     (3600)  2421320 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
+-rw-r--r--   0 lmei     (17911) micas     (3600)   175768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   159768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   160680 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   207224 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   145592 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   180464 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   178384 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   411960 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   192248 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   270320 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   569648 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   280416 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   204480 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   256824 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   313848 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   124400 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   175432 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   128080 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   144976 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   228000 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   232752 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
+-rw-r--r--   0 lmei     (17911) micas     (3600)   111980 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/parameter.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)    20306 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/parameter.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5286 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/powergating.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3055 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/powergating.h
+-rwxr-xr-x   0 lmei     (17911) micas     (3600)     1886 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/regression.test
+-rw-r--r--   0 lmei     (17911) micas     (3600)    10212 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/router.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3721 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/router.h
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.182436 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8781 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8768 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8780 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8784 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.187436 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/self_gen/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9545 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
+-rw-r--r--   0 lmei     (17911) micas     (3600)      579 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8332 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/subarray.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2542 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/subarray.h
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.234438 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/
+-rw-r--r--   0 lmei     (17911) micas     (3600)       25 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)    23666 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3842 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4575 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4759 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4755 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)    24571 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4758 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)    24570 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4742 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
+-rw-r--r--   0 lmei     (17911) micas     (3600)    15087 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/technology.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)    41317 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/uca.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4035 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/uca.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2064 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/version_cacti.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)    29856 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/wire.cc
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4375 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/wire.h
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6110 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_parser.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.239438 zigzag-dse-2.4.1/zigzag/classes/cost_model/
+-rw-r--r--   0 lmei     (17911) micas     (3600)    63132 2023-06-30 15:54:38.000000 zigzag-dse-2.4.1/zigzag/classes/cost_model/cost_model.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.375402 zigzag-dse-2.4.1/zigzag/classes/hardware/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.283440 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1278 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/accelerator.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9441 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/adder_hierarchy.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6460 2023-06-30 15:54:38.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/core.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      918 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/dimension.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)    11764 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_hierarchy.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3567 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_instance.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)    12231 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_level.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3014 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/operational_array.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1874 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.382403 zigzag-dse-2.4.1/zigzag/classes/io/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.287440 zigzag-dse-2.4.1/zigzag/classes/io/accelerator/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2805 2022-11-17 18:55:03.000000 zigzag-dse-2.4.1/zigzag/classes/io/accelerator/parser.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.323442 zigzag-dse-2.4.1/zigzag/classes/io/onnx/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7087 2023-06-14 18:45:40.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/conv.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      884 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/default.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5382 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/gemm.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3679 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/matmul.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4912 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/model.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1163 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/parser.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4089 2023-06-14 18:45:40.000000 zigzag-dse-2.4.1/zigzag/classes/io/onnx/utils.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.339443 zigzag-dse-2.4.1/zigzag/classes/mapping/
+-rw-r--r--   0 lmei     (17911) micas     (3600)    40951 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/combined_mapping.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      637 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/loop.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9386 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/mapping_assist_funcs.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.342443 zigzag-dse-2.4.1/zigzag/classes/mapping/memory/
+-rw-r--r--   0 lmei     (17911) micas     (3600)        0 2022-11-17 18:55:04.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/memory/data_layout.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.344443 zigzag-dse-2.4.1/zigzag/classes/mapping/spatial/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7657 2023-07-07 19:12:11.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/spatial/spatial_mapping.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.358443 zigzag-dse-2.4.1/zigzag/classes/mapping/temporal/
+-rw-r--r--   0 lmei     (17911) micas     (3600)      380 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/temporal/temporal_loop.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7412 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/mapping/temporal/temporal_mapping.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.407404 zigzag-dse-2.4.1/zigzag/classes/opt/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.361444 zigzag-dse-2.4.1/zigzag/classes/opt/spatial/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7044 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/spatial/generator.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.410404 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.375444 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/
+-rw-r--r--   0 lmei     (17911) micas     (3600)    11591 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/engine.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      489 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/loop.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)    15479 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/memory_allocator.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2837 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/multipermute.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.381444 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/salsa/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8726 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/salsa/engine.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3616 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/opt/temporal/salsa/state.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.522450 zigzag-dse-2.4.1/zigzag/classes/stages/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2054 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/CostModelStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1552 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/DumpStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3240 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2105 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/LomaStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2163 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/MainInputParserStages.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      966 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/ONNXModelParserStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1568 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6204 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/ReduceStages.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6260 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/RunOptStages.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6546 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/SalsaStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     6997 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/SaveStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8158 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3906 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2593 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/Stage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4046 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1187 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/WorkloadStage.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2821 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/stages/__init__.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.551452 zigzag-dse-2.4.1/zigzag/classes/workload/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2468 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/workload/dnn_workload.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     2210 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/workload/dummy_node.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)    21102 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/workload/layer_node.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1542 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/workload/onnx_workload.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)    14521 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/classes/workload/test_layer_node.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.416404 zigzag-dse-2.4.1/zigzag/inputs/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.420404 zigzag-dse-2.4.1/zigzag/inputs/examples/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.570452 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8448 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5849 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5746 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7098 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     5112 2023-06-19 17:19:39.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     7287 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.592453 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/
+-rw-r--r--   0 lmei     (17911) micas     (3600)      561 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/assend_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      196 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/default.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      832 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/edge_tpu_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      560 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/meta_prototype_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      610 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/tesla_npu_like.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      557 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/tpu_like.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.613454 zigzag-dse-2.4.1/zigzag/inputs/examples/workload/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     4067 2023-01-11 10:28:45.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/workload/alexnet.onnx
+-rw-r--r--   0 lmei     (17911) micas     (3600)    71724 2023-01-11 10:28:45.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/workload/mobilenetv2.onnx
+-rw-r--r--   0 lmei     (17911) micas     (3600)    18600 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/workload/resnet18.onnx
+-rw-r--r--   0 lmei     (17911) micas     (3600)    19065 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/inputs/examples/workload/resnet18.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)      504 2022-11-17 18:55:04.000000 zigzag-dse-2.4.1/zigzag/utils.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:01.425404 zigzag-dse-2.4.1/zigzag/visualization/
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.621454 zigzag-dse-2.4.1/zigzag/visualization/graph/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1527 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     1280 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.626455 zigzag-dse-2.4.1/zigzag/visualization/results/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     8773 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 lmei     (17911) micas     (3600)     3951 2023-06-02 15:50:58.000000 zigzag-dse-2.4.1/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 lmei     (17911) micas     (3600)        0 2023-07-07 19:18:02.653456 zigzag-dse-2.4.1/zigzag_dse.egg-info/
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9644 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 lmei     (17911) micas     (3600)     9476 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 lmei     (17911) micas     (3600)        1 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 lmei     (17911) micas     (3600)       52 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 lmei     (17911) micas     (3600)      144 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 lmei     (17911) micas     (3600)       34 2023-07-07 19:18:01.000000 zigzag-dse-2.4.1/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag-dse-2.4.0/LICENSE` & `zigzag-dse-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/PKG-INFO` & `zigzag-dse-2.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.4.0
+Version: 2.4.1
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
         
@@ -91,7 +91,9 @@
 S. Colleman, P. Zhu, W. Sun and M. Verhelst, "Optimizing Accelerator Configurability for Mobile Transformer Networks," 2022 IEEE 4th International Conference on Artificial Intelligence Circuits and Systems (AICAS), Incheon, Korea, Republic of, 2022, pp. 142-145, doi: 10.1109/AICAS54282.2022.9869945. [paper](https://ieeexplore.ieee.org/document/9869945), [slides](https://docs.google.com/presentation/d/1tp11akyAVGg3Y20Aupp2wlTRSgg9nKAQ/edit?usp=sharing&ouid=117150865143314519834&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1tglc-BCGVclrWT-kNhWy02Vms5sjk1zt/view?usp=sharing)
 
 #### Extend ZigZag to support cross-layer depth-first scheduling
 L. Mei, K. Goetschalckx, A. Symons and M. Verhelst, " DeFiNES: Enabling Fast Exploration of the Depth-first Scheduling Space for DNN Accelerators through Analytical Modeling," 2023 IEEE International Symposium on High-Performance Computer Architecture (HPCA), 2023 [paper](https://arxiv.org/abs/2212.05344), [slides](https://drive.google.com/file/d/1u_PG9ZhjUZVrH2wnMLDe-PYJeO0RUGLd/view?usp=sharing), [github](https://github.com/ZigZag-Project/DeFiNES)
 
 #### Extend ZigZag to support multi-core layer-fused scheduling
 A. Symons, L. Mei, S. Colleman, P. Houshmand, S. Karl and M. Verhelst, “Towards Heterogeneous Multi-core Accelerators Exploiting Fine-grained Scheduling of Layer-Fused Deep Neural Networks”, <i>arXiv e-prints</i>, 2022. doi:10.48550/arXiv.2212.10612. [paper](https://arxiv.org/abs/2212.10612), [github](https://github.com/ZigZag-Project/stream)
+
+S. Karl, A. Symons, N. Fasfous and M. Verhelst, "Genetic Algorithm-based Framework for Layer-Fused Scheduling of Multiple DNNs on Multi-core Systems," 2023 Design, Automation & Test in Europe Conference & Exhibition (DATE), Antwerp, Belgium, 2023, pp. 1-6, doi: 10.23919/DATE56975.2023.10137070. [paper](https://ieeexplore.ieee.org/document/10137070), [slides](https://www.dropbox.com/s/rv8qiko59h4pp0s/Genetic%20Algorithm-based%20Framework%20for.pptx?dl=0), [video](https://www.dropbox.com/s/12v94stvevj9xns/Genetic%20Algorithm-based%20Framework%20for.mp4?dl=0)
```

### Comparing `zigzag-dse-2.4.0/README.md` & `zigzag-dse-2.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,7 +47,9 @@
 S. Colleman, P. Zhu, W. Sun and M. Verhelst, "Optimizing Accelerator Configurability for Mobile Transformer Networks," 2022 IEEE 4th International Conference on Artificial Intelligence Circuits and Systems (AICAS), Incheon, Korea, Republic of, 2022, pp. 142-145, doi: 10.1109/AICAS54282.2022.9869945. [paper](https://ieeexplore.ieee.org/document/9869945), [slides](https://docs.google.com/presentation/d/1tp11akyAVGg3Y20Aupp2wlTRSgg9nKAQ/edit?usp=sharing&ouid=117150865143314519834&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1tglc-BCGVclrWT-kNhWy02Vms5sjk1zt/view?usp=sharing)
 
 #### Extend ZigZag to support cross-layer depth-first scheduling
 L. Mei, K. Goetschalckx, A. Symons and M. Verhelst, " DeFiNES: Enabling Fast Exploration of the Depth-first Scheduling Space for DNN Accelerators through Analytical Modeling," 2023 IEEE International Symposium on High-Performance Computer Architecture (HPCA), 2023 [paper](https://arxiv.org/abs/2212.05344), [slides](https://drive.google.com/file/d/1u_PG9ZhjUZVrH2wnMLDe-PYJeO0RUGLd/view?usp=sharing), [github](https://github.com/ZigZag-Project/DeFiNES)
 
 #### Extend ZigZag to support multi-core layer-fused scheduling
 A. Symons, L. Mei, S. Colleman, P. Houshmand, S. Karl and M. Verhelst, “Towards Heterogeneous Multi-core Accelerators Exploiting Fine-grained Scheduling of Layer-Fused Deep Neural Networks”, <i>arXiv e-prints</i>, 2022. doi:10.48550/arXiv.2212.10612. [paper](https://arxiv.org/abs/2212.10612), [github](https://github.com/ZigZag-Project/stream)
+
+S. Karl, A. Symons, N. Fasfous and M. Verhelst, "Genetic Algorithm-based Framework for Layer-Fused Scheduling of Multiple DNNs on Multi-core Systems," 2023 Design, Automation & Test in Europe Conference & Exhibition (DATE), Antwerp, Belgium, 2023, pp. 1-6, doi: 10.23919/DATE56975.2023.10137070. [paper](https://ieeexplore.ieee.org/document/10137070), [slides](https://www.dropbox.com/s/rv8qiko59h4pp0s/Genetic%20Algorithm-based%20Framework%20for.pptx?dl=0), [video](https://www.dropbox.com/s/12v94stvevj9xns/Genetic%20Algorithm-based%20Framework%20for.mp4?dl=0)
```

### Comparing `zigzag-dse-2.4.0/pyproject.toml` & `zigzag-dse-2.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "2.4.0"
+version = "2.4.1"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "2.4.0"
+current_version = "2.4.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag-dse-2.4.0/zigzag/__main__.py` & `zigzag-dse-2.4.1/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/api.py` & `zigzag-dse-2.4.1/zigzag/api.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/README` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/README`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/TSV.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/TSV.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/TSV.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/TSV.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/Ucache.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/Ucache.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/Ucache.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/Ucache.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/arbiter.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/arbiter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/arbiter.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/arbiter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/area.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/area.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/area.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/area.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/bank.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/bank.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/bank.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/bank.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/basic_circuit.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/basic_circuit.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/basic_circuit.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cache.cfg_temp`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cache_old.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti.mk` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti.mk`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_interface.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_interface.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_interface.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/component.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/component.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/component.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/component.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/const.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/const.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/contention.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/contention.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/crossbar.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/crossbar.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/crossbar.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/crossbar.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/ddr3.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/ddr3.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/decoder.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/decoder.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/decoder.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/decoder.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/dram.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/dram.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio_technology.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio_technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/extio_technology.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/extio_technology.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/htree2.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/htree2.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/htree2.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/htree2.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/io.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/io.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/io.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/io.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/lpddr.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/lpddr.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/main.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/main.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/mat.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/mat.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/mat.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/mat.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad_parameters.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memcad_parameters.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memorybus.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memorybus.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/memorybus.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/memorybus.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/nuca.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/nuca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/nuca.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/nuca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/area.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/component.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/io.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/main.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/router.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/parameter.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/parameter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/parameter.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/parameter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/powergating.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/powergating.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/powergating.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/powergating.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/regression.test` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/regression.test`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/router.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/router.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/router.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/router.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/subarray.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/subarray.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/subarray.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/subarray.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/technology.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/uca.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/uca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/uca.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/uca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/version_cacti.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/version_cacti.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/wire.cc` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/wire.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_master/wire.h` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_master/wire.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cacti/cacti_parser.py` & `zigzag-dse-2.4.1/zigzag/classes/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/cost_model/cost_model.py` & `zigzag-dse-2.4.1/zigzag/classes/cost_model/cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/accelerator.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/accelerator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/adder_hierarchy.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/adder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/core.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/core.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/dimension.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/dimension.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_hierarchy.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_instance.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/memory_level.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/memory_level.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/operational_array.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag-dse-2.4.1/zigzag/classes/hardware/architecture/operational_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/accelerator/parser.py` & `zigzag-dse-2.4.1/zigzag/classes/io/accelerator/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/conv.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/conv.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/default.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/default.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/gemm.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/gemm.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/matmul.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/matmul.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/model.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/parser.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/io/onnx/utils.py` & `zigzag-dse-2.4.1/zigzag/classes/io/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/mapping/combined_mapping.py` & `zigzag-dse-2.4.1/zigzag/classes/mapping/combined_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/mapping/loop.py` & `zigzag-dse-2.4.1/zigzag/classes/mapping/loop.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag-dse-2.4.1/zigzag/classes/mapping/mapping_assist_funcs.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag-dse-2.4.1/zigzag/classes/mapping/spatial/spatial_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         Calculate memory bandwidth incremental factor between architectural levels.
 
         NOTE: mem_bw_boost doesn't include MAC level, thus is one level less than other spatial mapping attributes.
         """
         """ mem_bw_boost can calculated by either dividing unit_unique at current level by unit_count at one level above. """
         mem_bw_boost = {
             op: [
-                int(self.unit_unique[op][lv] / self.unit_unique[op][lv + 1])
+                round(self.unit_unique[op][lv] / self.unit_unique[op][lv + 1])
                 for lv in range(self.arch_level[op] - 1)
             ]
             for op in self.operand_list
         }
 
         self.mem_bw_boost = mem_bw_boost
```

### Comparing `zigzag-dse-2.4.0/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag-dse-2.4.1/zigzag/classes/mapping/temporal/temporal_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/spatial/generator.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/spatial/generator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/temporal/loma/multipermute.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/temporal/loma/multipermute.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/temporal/salsa/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag-dse-2.4.1/zigzag/classes/opt/temporal/salsa/state.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/CostModelStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/CostModelStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/DumpStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/DumpStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/GeneralParameterIteratorStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/GeneralParameterIteratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/LomaStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/LomaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/MainInputParserStages.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/MainInputParserStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/ONNXModelParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/PlotTemporalMappingsStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/ReduceStages.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/ReduceStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/RunOptStages.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/RunOptStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/SalsaStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/SalsaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/SaveStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/SaveStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/SpatialMappingConversionStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/SpatialMappingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/SpatialMappingGeneratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/Stage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/Stage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/TemporalOrderingConversionStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/TemporalOrderingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/WorkloadStage.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/WorkloadStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/stages/__init__.py` & `zigzag-dse-2.4.1/zigzag/classes/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/workload/dnn_workload.py` & `zigzag-dse-2.4.1/zigzag/classes/workload/dnn_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/workload/dummy_node.py` & `zigzag-dse-2.4.1/zigzag/classes/workload/dummy_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/workload/layer_node.py` & `zigzag-dse-2.4.1/zigzag/classes/workload/layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/workload/onnx_workload.py` & `zigzag-dse-2.4.1/zigzag/classes/workload/onnx_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/classes/workload/test_layer_node.py` & `zigzag-dse-2.4.1/zigzag/classes/workload/test_layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Ascend_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Eyeriss_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Meta_prototype.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Meta_prototype.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/TPU_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/assend_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/assend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/edge_tpu_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/meta_prototype_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/tesla_npu_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/mapping/tpu_like.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/mapping/tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/workload/alexnet.onnx` & `zigzag-dse-2.4.1/zigzag/inputs/examples/workload/alexnet.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/workload/mobilenetv2.onnx` & `zigzag-dse-2.4.1/zigzag/inputs/examples/workload/mobilenetv2.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/workload/resnet18.onnx` & `zigzag-dse-2.4.1/zigzag/inputs/examples/workload/resnet18.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/inputs/examples/workload/resnet18.py` & `zigzag-dse-2.4.1/zigzag/inputs/examples/workload/resnet18.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag-dse-2.4.1/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/visualization/graph/workload.py` & `zigzag-dse-2.4.1/zigzag/visualization/graph/workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/visualization/results/plot_cme.py` & `zigzag-dse-2.4.1/zigzag/visualization/results/plot_cme.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag/visualization/results/print_mapping.py` & `zigzag-dse-2.4.1/zigzag/visualization/results/print_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.4.0/zigzag_dse.egg-info/PKG-INFO` & `zigzag-dse-2.4.1/zigzag_dse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.4.0
+Version: 2.4.1
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
         
@@ -91,7 +91,9 @@
 S. Colleman, P. Zhu, W. Sun and M. Verhelst, "Optimizing Accelerator Configurability for Mobile Transformer Networks," 2022 IEEE 4th International Conference on Artificial Intelligence Circuits and Systems (AICAS), Incheon, Korea, Republic of, 2022, pp. 142-145, doi: 10.1109/AICAS54282.2022.9869945. [paper](https://ieeexplore.ieee.org/document/9869945), [slides](https://docs.google.com/presentation/d/1tp11akyAVGg3Y20Aupp2wlTRSgg9nKAQ/edit?usp=sharing&ouid=117150865143314519834&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1tglc-BCGVclrWT-kNhWy02Vms5sjk1zt/view?usp=sharing)
 
 #### Extend ZigZag to support cross-layer depth-first scheduling
 L. Mei, K. Goetschalckx, A. Symons and M. Verhelst, " DeFiNES: Enabling Fast Exploration of the Depth-first Scheduling Space for DNN Accelerators through Analytical Modeling," 2023 IEEE International Symposium on High-Performance Computer Architecture (HPCA), 2023 [paper](https://arxiv.org/abs/2212.05344), [slides](https://drive.google.com/file/d/1u_PG9ZhjUZVrH2wnMLDe-PYJeO0RUGLd/view?usp=sharing), [github](https://github.com/ZigZag-Project/DeFiNES)
 
 #### Extend ZigZag to support multi-core layer-fused scheduling
 A. Symons, L. Mei, S. Colleman, P. Houshmand, S. Karl and M. Verhelst, “Towards Heterogeneous Multi-core Accelerators Exploiting Fine-grained Scheduling of Layer-Fused Deep Neural Networks”, <i>arXiv e-prints</i>, 2022. doi:10.48550/arXiv.2212.10612. [paper](https://arxiv.org/abs/2212.10612), [github](https://github.com/ZigZag-Project/stream)
+
+S. Karl, A. Symons, N. Fasfous and M. Verhelst, "Genetic Algorithm-based Framework for Layer-Fused Scheduling of Multiple DNNs on Multi-core Systems," 2023 Design, Automation & Test in Europe Conference & Exhibition (DATE), Antwerp, Belgium, 2023, pp. 1-6, doi: 10.23919/DATE56975.2023.10137070. [paper](https://ieeexplore.ieee.org/document/10137070), [slides](https://www.dropbox.com/s/rv8qiko59h4pp0s/Genetic%20Algorithm-based%20Framework%20for.pptx?dl=0), [video](https://www.dropbox.com/s/12v94stvevj9xns/Genetic%20Algorithm-based%20Framework%20for.mp4?dl=0)
```

### Comparing `zigzag-dse-2.4.0/zigzag_dse.egg-info/SOURCES.txt` & `zigzag-dse-2.4.1/zigzag_dse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

