# Comparing `tmp/chiapos-2.0.0b2.tar.gz` & `tmp/chiapos-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-2.0.0b2.tar", last modified: Fri Jun 30 08:24:46 2023, max compression
+gzip compressed data, was "chiapos-2.0.0b3.tar", last modified: Fri Jul  7 21:03:02 2023, max compression
```

## Comparing `chiapos-2.0.0b2.tar` & `chiapos-2.0.0b3.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.157384 chiapos-2.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.161384 chiapos-2.0.0b2/.github/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/actions/fetch_bladebit_harvester.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.161384 chiapos-2.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/build-test-cplusplus.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/plot-k27-no-bitfield.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/plot-k27.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.161384 chiapos-2.0.0b2/chiapos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-30 08:24:46.000000 chiapos-2.0.0b2/chiapos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-30 08:24:46.000000 chiapos-2.0.0b2/chiapos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:24:46.000000 chiapos-2.0.0b2/chiapos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:24:45.000000 chiapos-2.0.0b2/chiapos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 08:24:46.000000 chiapos-2.0.0b2/chiapos.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/docker-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/docker-test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.165384 chiapos-2.0.0b2/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/bucket_graph.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/code_documentation.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.165384 chiapos-2.0.0b2/documents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/images/aesctr.png
--rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/images/beyondhellman.png
--rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/images/beyondhellman2.png
--rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/images/pointerformat.png
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/images/proofofspace.png
--rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/proof_of_space.html
--rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/documents/proof_of_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.165384 chiapos-2.0.0b2/hellman_example/
--rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/aes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/hellman.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/hellman_example/verifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lgtm.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.157384 chiapos-2.0.0b2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.157384 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.169384 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.173385 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.173385 chiapos-2.0.0b2/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/lib/include/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.173385 chiapos-2.0.0b2/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/python-bindings/chiapos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.177384 chiapos-2.0.0b2/src/
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b17phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b17phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b17phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/src/b3/
--rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3.h
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_avx512.c
--rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_portable.c
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_sse41.c
--rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/bitfield.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/bitfield_index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/chacha8.c
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/chacha8.h
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/chia_filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/entry_sizes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/phase1.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/phases.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/progress.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/quicksort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/serialize.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/sort_manager.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/threading.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/uniformsort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/src/verifier.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tests/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tests/plot-resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tests/test_python_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tools/disk.gnuplot
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/tools/parse_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:24:46.181384 chiapos-2.0.0b2/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/endianness.h
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 08:24:36.000000 chiapos-2.0.0b2/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/.github/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/actions/fetch_bladebit_harvester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/build-test-cplusplus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/plot-k27-no-bitfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/plot-k27.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/chiapos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/docker-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/docker-test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/bucket_graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/code_documentation.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/aesctr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/beyondhellman.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/pointerformat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/proofofspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/proof_of_space.html
+-rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/proof_of_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/hellman_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/aes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/hellman.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/verifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lgtm.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/include/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/python-bindings/chiapos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.785746 chiapos-2.0.0b3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/src/b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_portable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bitfield.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bitfield_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chacha8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chacha8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chia_filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/entry_sizes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase1.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/quicksort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/serialize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/sort_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/threading.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/uniformsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/verifier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/plot-resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/test_python_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tools/disk.gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tools/parse_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/endianness.h
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t_config.include
```

### Comparing `chiapos-2.0.0b2/.github/actions/fetch_bladebit_harvester.sh` & `chiapos-2.0.0b3/.github/actions/fetch_bladebit_harvester.sh`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 fi
 
 if [[ "${host_arch}" != "arm64" ]] && [[ "${host_arch}" != "x86-64" ]]; then
   echo >&2 "Unkonwn Architecture '${host_arch}'"
   exit 1
 fi
 
-# Update these when pointing to different releases
+## Change this before releasing 2.0.0
 artifact_ver="v3.0.0-alpha4"
 artifact_base_url="https://github.com/harold-b/bladebit-test/releases/download/v3-alpha4-fixes"
+## End changes
 
 linux_sha256=
 macos_sha256=
 windows_sha256=
 
 artifact_ext="tar.gz"
 sha_bin="sha256sum"
```

### Comparing `chiapos-2.0.0b2/.github/workflows/build-test-cplusplus.yml` & `chiapos-2.0.0b3/.github/workflows/build-test-cplusplus.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/.github/workflows/build-wheels.yml` & `chiapos-2.0.0b3/.github/workflows/build-wheels.yml`

 * *Files 4% similar despite different names*

```diff
@@ -129,16 +129,15 @@
 
     - name: Get Windows Bladebit Harvester Artifact
       if: runner.os == 'Windows'
       shell: bash
       run: |
         set -eo pipefail
         set -x
-
-        windows_sha256='98627bc1866aef67cb6307178caa5da15d59ad6fbddf2817ba8737619e68607f'
+        windows_sha256='febea2317b7e858e296a30344a5382161cebc1a66678975151b117f17cda5181'
         .github/actions/fetch_bladebit_harvester.sh windows x86-64
 
     - name: Build and test
       env:
         CIBW_PRERELEASE_PYTHONS: True
         CIBW_BUILD_VERBOSITY_MACOS: 1
         CIBW_BUILD_VERBOSITY_LINUX: 1
@@ -152,34 +151,34 @@
         CIBW_BEFORE_ALL_LINUX: |
           set -eo pipefail
           set -x
           # Get bladebit harvester
           set -eo pipefail
           ARCH=$(uname -m)
           if [[ $ARCH == x86_64 ]]; then
-            linux_sha256='c34f492f5cc75d8f469cda9e214d1b303fe859632af99902d8c303eab40ef817'
+            linux_sha256='ef3f8f74b9c63166a735eb1f2cb855e88b36f50ad52c9d51cf32eb3e9e25428e'
             .github/actions/fetch_bladebit_harvester.sh linux x86-64
           else
-            linux_sha256='27b96b0fe89bdf810baf553627fb3607978d4e055ab1bcd113dfb37cd92288e9'
+            linux_sha256='fcc8bf849733781c82c0b13b70bbba57aaf82abc9a0e2aee7b1ba3da6b0e58f2'
             .github/actions/fetch_bladebit_harvester.sh linux arm64
           fi
 
         CIBW_BEFORE_BUILD_LINUX: >
           python -m pip install --upgrade pip
         CIBW_ARCHS_MACOS: ${{ matrix.os.cibw-archs-macos[matrix.arch.matrix] }}
         CIBW_BEFORE_ALL_MACOS: |
           brew install gmp boost cmake
           # Get bladebit harvester
           set -eo pipefail
           ARCH=$(uname -m)
           if [[ $ARCH == x86_64 ]]; then
-            macos_sha256='797a2f481acb3aef6cb9dd3cb408127ef2d556a21240d14dd68fb7dd60023438'
+            macos_sha256='199720c9dff72e883edbd027c31cc03ed9f901e6a00e2be5a7e8ac2633ecb69c'
             .github/actions/fetch_bladebit_harvester.sh macos x86-64
           else
-            macos_sha256='c46d232689adfc2da08bfdbdb3742ac607b96298b61d0f6b69d0a1f28fd853bc'
+            macos_sha256='932d73c6a70df59bbe7baf3702cc74cc8eb483f5e6a94551b3089779b1e7b010'
             .github/actions/fetch_bladebit_harvester.sh macos arm64
           fi
 
         CIBW_BEFORE_BUILD_MACOS: >
           python -m pip install --upgrade pip
         CIBW_ENVIRONMENT_MACOS: "MACOSX_DEPLOYMENT_TARGET=10.14 CP_USE_GREEN_REAPER=1"
         CIBW_TEST_REQUIRES: pytest
```

### Comparing `chiapos-2.0.0b2/.github/workflows/doc-html-pdf.yml` & `chiapos-2.0.0b3/.github/workflows/doc-html-pdf.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/.github/workflows/manual-plot.yml` & `chiapos-2.0.0b3/.github/workflows/manual-plot.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/.github/workflows/plot-k27-no-bitfield.yaml` & `chiapos-2.0.0b3/.github/workflows/plot-k27-no-bitfield.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/.github/workflows/plot-k27.yaml` & `chiapos-2.0.0b3/.github/workflows/plot-k27.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/.github/workflows/stale-issue.yml` & `chiapos-2.0.0b3/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/CMakeLists.txt` & `chiapos-2.0.0b3/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   set(CP_LINK_BLADEBIT_HARVESTER ON)
 endif()
 
 if (${CP_BUILD_BLADEBIT_HARVESTER})
   FetchContent_Declare(
     bladebit
     GIT_REPOSITORY https://github.com/Chia-Network/bladebit.git
-    GIT_TAG        fix-cuda-compression-device-lost
+    GIT_TAG        cuda-compression
   )
 
   set(BB_HARVESTER_ONLY ON)
   set(BB_HARVESTER_STATIC ON)
   FetchContent_MakeAvailable(bladebit)
 endif()
```

### Comparing `chiapos-2.0.0b2/Dockerfile` & `chiapos-2.0.0b3/Dockerfile`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/LICENSE` & `chiapos-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/PKG-INFO` & `chiapos-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b2/README.md` & `chiapos-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/chiapos.egg-info/PKG-INFO` & `chiapos-2.0.0b3/chiapos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b2/chiapos.egg-info/SOURCES.txt` & `chiapos-2.0.0b3/chiapos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/bucket_graph.pdf` & `chiapos-2.0.0b3/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/code_documentation.pdf` & `chiapos-2.0.0b3/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/images/aesctr.png` & `chiapos-2.0.0b3/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/images/beyondhellman.png` & `chiapos-2.0.0b3/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/images/beyondhellman2.png` & `chiapos-2.0.0b3/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/images/pointerformat.png` & `chiapos-2.0.0b3/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/images/proofofspace.png` & `chiapos-2.0.0b3/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/proof_of_space.html` & `chiapos-2.0.0b3/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/documents/proof_of_space.md` & `chiapos-2.0.0b3/documents/proof_of_space.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/Hellman attacks.pdf` & `chiapos-2.0.0b3/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/aes.hpp` & `chiapos-2.0.0b3/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/bits.hpp` & `chiapos-2.0.0b3/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/calculate_bucket.hpp` & `chiapos-2.0.0b3/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/cli.cpp` & `chiapos-2.0.0b3/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/cxxopts.hpp` & `chiapos-2.0.0b3/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/encoding.hpp` & `chiapos-2.0.0b3/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/hellman.hpp` & `chiapos-2.0.0b3/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/picosha2.hpp` & `chiapos-2.0.0b3/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/plotter_disk.hpp` & `chiapos-2.0.0b3/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/pos_constants.hpp` & `chiapos-2.0.0b3/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/prover_disk.hpp` & `chiapos-2.0.0b3/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/sort_on_disk.hpp` & `chiapos-2.0.0b3/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/util.hpp` & `chiapos-2.0.0b3/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/hellman_example/verifier.hpp` & `chiapos-2.0.0b3/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/LICENSE` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/README.md` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/README.md` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/bitstream.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/compiler.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/debug.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/debug.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/entropy_common.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/error_private.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/error_public.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fseU16.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fseU16.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse_compress.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/hist.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/hist.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf_compress.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/lib/mem.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/COPYING` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/bench.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/bench.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/commandline.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/cpu.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fileio.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fileio.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fseDist.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fseDist.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fullbench.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzer.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/xxhash.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/xxhash.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/zlibh.c` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/FiniteStateEntropy/programs/zlibh.h` & `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/lib/include/picosha2.hpp` & `chiapos-2.0.0b3/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/python-bindings/chiapos.cpp` & `chiapos-2.0.0b3/python-bindings/chiapos.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         .def(
             "get_id",
             [](DiskProver &dp) {
                 const std::vector<uint8_t>& id = dp.GetId();
                 return py::bytes(reinterpret_cast<const char*>(id.data()), id.size());
             })
         .def("get_size", [](DiskProver &dp) { return dp.GetSize(); })
-        .def("get_compresion_level", [](DiskProver &dp) { return dp.GetCompressionLevel(); })
+        .def("get_compression_level", [](DiskProver &dp) { return dp.GetCompressionLevel(); })
         .def("get_filename", [](DiskProver &dp) { return dp.GetFilename(); })
         .def(
             "get_qualities_for_challenge",
             [](DiskProver &dp, const py::bytes &challenge) {
                 if (len(challenge) != 32) {
                     throw std::invalid_argument("Challenge must be exactly 32 bytes");
                 }
```

### Comparing `chiapos-2.0.0b2/setup.py` & `chiapos-2.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b17phase2.hpp` & `chiapos-2.0.0b3/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b17phase3.hpp` & `chiapos-2.0.0b3/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b17phase4.hpp` & `chiapos-2.0.0b3/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b17sort_manager.hpp` & `chiapos-2.0.0b3/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3.c` & `chiapos-2.0.0b3/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3.h` & `chiapos-2.0.0b3/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_avx2.c` & `chiapos-2.0.0b3/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_avx2_x86-64_unix.S` & `chiapos-2.0.0b3/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_avx512.c` & `chiapos-2.0.0b3/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_avx512_x86-64_unix.S` & `chiapos-2.0.0b3/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_dispatch.c` & `chiapos-2.0.0b3/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_impl.h` & `chiapos-2.0.0b3/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_portable.c` & `chiapos-2.0.0b3/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_sse41.c` & `chiapos-2.0.0b3/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/b3/blake3_sse41_x86-64_unix.S` & `chiapos-2.0.0b3/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/bitfield.hpp` & `chiapos-2.0.0b3/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/bitfield_index.hpp` & `chiapos-2.0.0b3/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/bits.hpp` & `chiapos-2.0.0b3/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/calculate_bucket.hpp` & `chiapos-2.0.0b3/src/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/chacha8.c` & `chiapos-2.0.0b3/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/chia_filesystem.hpp` & `chiapos-2.0.0b3/src/chia_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/cli.cpp` & `chiapos-2.0.0b3/src/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/disk.hpp` & `chiapos-2.0.0b3/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/encoding.hpp` & `chiapos-2.0.0b3/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/entry_sizes.hpp` & `chiapos-2.0.0b3/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/exceptions.hpp` & `chiapos-2.0.0b3/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/phase1.hpp` & `chiapos-2.0.0b3/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/phase2.hpp` & `chiapos-2.0.0b3/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/phase3.hpp` & `chiapos-2.0.0b3/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/phase4.hpp` & `chiapos-2.0.0b3/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/phases.hpp` & `chiapos-2.0.0b3/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/plotter_disk.hpp` & `chiapos-2.0.0b3/src/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/pos_constants.hpp` & `chiapos-2.0.0b3/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/prover_disk.hpp` & `chiapos-2.0.0b3/src/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/quicksort.hpp` & `chiapos-2.0.0b3/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/serialize.hpp` & `chiapos-2.0.0b3/src/serialize.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/sort_manager.hpp` & `chiapos-2.0.0b3/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/threading.hpp` & `chiapos-2.0.0b3/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/uniformsort.hpp` & `chiapos-2.0.0b3/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/util.hpp` & `chiapos-2.0.0b3/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/src/verifier.hpp` & `chiapos-2.0.0b3/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/tests/plot-resources.py` & `chiapos-2.0.0b3/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/tests/test.cpp` & `chiapos-2.0.0b3/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/tests/test_python_bindings.py` & `chiapos-2.0.0b3/tests/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/tools/disk.gnuplot` & `chiapos-2.0.0b3/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/tools/parse_disk.py` & `chiapos-2.0.0b3/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/LICENSE` & `chiapos-2.0.0b3/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/README.md` & `chiapos-2.0.0b3/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/endianness.h` & `chiapos-2.0.0b3/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/uint128_t.cpp` & `chiapos-2.0.0b3/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/uint128_t.include` & `chiapos-2.0.0b3/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b2/uint128_t/uint128_t_config.include` & `chiapos-2.0.0b3/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

