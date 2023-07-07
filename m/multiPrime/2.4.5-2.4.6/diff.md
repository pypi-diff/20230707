# Comparing `tmp/multiPrime-2.4.5.tar.gz` & `tmp/multiPrime-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.4.5.tar", last modified: Wed Jun 21 05:39:21 2023, max compression
+gzip compressed data, was "multiPrime-2.4.6.tar", last modified: Fri Jul  7 09:01:54 2023, max compression
```

## Comparing `multiPrime-2.4.5.tar` & `multiPrime-2.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.444408 multiPrime-2.4.5/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-06-21 05:39:01.000000 multiPrime-2.4.5/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-06-21 05:39:21.444408 multiPrime-2.4.5/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16831 2023-06-21 05:39:02.000000 multiPrime-2.4.5/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.443408 multiPrime-2.4.5/multiPrime/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-06-21 05:39:01.000000 multiPrime-2.4.5/multiPrime/__init__.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.443408 multiPrime-2.4.5/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-06-21 05:39:21.444408 multiPrime-2.4.5/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-06-21 05:39:02.000000 multiPrime-2.4.5/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.444408 multiPrime-2.4.5/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2467 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    86841 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    27047 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-07-07 09:01:54.360813 multiPrime-2.4.6/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-07-07 09:01:13.000000 multiPrime-2.4.6/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-07-07 09:01:54.360813 multiPrime-2.4.6/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16831 2023-07-07 09:01:14.000000 multiPrime-2.4.6/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-07-07 09:01:54.359814 multiPrime-2.4.6/multiPrime/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-07-07 09:01:14.000000 multiPrime-2.4.6/multiPrime/__init__.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-07-07 09:01:54.360813 multiPrime-2.4.6/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-07-07 09:01:53.000000 multiPrime-2.4.6/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-07-07 09:01:54.000000 multiPrime-2.4.6/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-07-07 09:01:53.000000 multiPrime-2.4.6/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-07-07 09:01:53.000000 multiPrime-2.4.6/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-07-07 09:01:53.000000 multiPrime-2.4.6/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-07-07 09:01:54.361814 multiPrime-2.4.6/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-07-07 09:01:14.000000 multiPrime-2.4.6/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-07-07 09:01:54.360813 multiPrime-2.4.6/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-07-07 09:01:14.000000 multiPrime-2.4.6/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2344 2023-07-07 09:01:14.000000 multiPrime-2.4.6/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    86708 2023-07-07 09:01:14.000000 multiPrime-2.4.6/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    23900 2023-07-07 09:01:14.000000 multiPrime-2.4.6/src/utils.py
```

### Comparing `multiPrime-2.4.5/LICENSE` & `multiPrime-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.5/PKG-INFO` & `multiPrime-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.5
+Version: 2.4.6
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.4.5/README.md` & `multiPrime-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.5/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.4.6/multiPrime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.5
+Version: 2.4.6
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.4.5/setup.py` & `multiPrime-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.5/src/src.py` & `multiPrime-2.4.6/src/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,19 +299,19 @@
         for acc_id in Input_dict.keys():
             # start_dict[acc_id] = pattern_start.search(Input_dict[acc_id]).span()[0]
             # stop_dict[acc_id] = pattern_stop.search(Input_dict[acc_id]).span()[0] - 1
             t_length = len(Input_dict[acc_id])
             start_dict[acc_id] = t_length - len(Input_dict[acc_id].lstrip("-"))
             stop_dict[acc_id] = len(Input_dict[acc_id].rstrip("-"))
             # start position should contain [coverage] sequences at least.
-        start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, method="higher")
+        start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, interpolation="higher")
         # for python 3.9.9
         # start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, method="higher")
         # stop position should contain [coverage] sequences at least.
-        stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
+        stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, interpolation="lower")
         # stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
         if stop - start < int(self.product):
             print("Error: max length of PCR product is shorter than the default min Product length with {} "
                   "coverage! Non candidate primers !!!".format(self.coverage))
             sys.exit(1)
         else:
             return [start, stop, stop - start]
@@ -401,14 +401,15 @@
                 # print("Entropy fail")
                 # This window is not a conserved region, and not proper to design primers
                 self.resQ.put(None)
             else:
                 primers_db = pd.DataFrame(primers_db)
                 # frequency matrix
                 freq_matrix = self.state_matrix(primers_db)
+                # print(freq_matrix)
                 colSum = np.sum(freq_matrix, axis=0)
                 a, b = freq_matrix.shape
                 # a < 4 means base composition of this region is less than 4 (GC bias).
                 # It's not a proper region for primer design.
                 if a < 4:
                     self.resQ.put(None)
                 elif (colSum == 0).any():
@@ -431,109 +432,98 @@
                     #     self.resQ.put(None)
                     # else:
                     #     self.resQ.put([mismatch_coverage, non_cov_primer_info, gap_seq_id_info])
 
     def degenerate_by_NN_algorithm(self, primer_start, freq_matrix, cover, non_gap_seq_id, cover_for_MM,
                                    cover_number, cBit, tBit):
         # full degenerate primer
-        full_degenerate_primer = self.full_degenerate_primer(freq_matrix)
+        # full_degenerate_primer = self.full_degenerate_primer(freq_matrix)
         # unique covered primers, which is used to calculate coverage and
         # mis-coverage in the following step.
         cover_primer_set = set(cover.keys())
         # if full_degenerate_primer is ok, then return full_degenerate_primer
         # mismatch_coverage, non_cov_primer_info = {}, {}
         F_non_cover, R_non_cover = {}, {}
         ######################################################################################################
         ############ need prone. not all primers is proper for primer-F or primer-R ##########################
         # If a primer is located in the start region, there is no need to calculate its coverage for primer-R#
         ## here is a suggestion. we can assert candidate primer as primer-F or primer-R by primer attribute ##
         ######################################################################################################
-        if self.pre_degenerate_primer_check(full_degenerate_primer):
-            information = self.primer_pre_filter(full_degenerate_primer)
-            optimal_primer_current = full_degenerate_primer
-            F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
-                self.mis_primer_check(cover_primer_set, full_degenerate_primer, cover,
-                                      non_gap_seq_id)
-            F_non_cover.update(F_non_cover_in_cover)
-            R_non_cover.update(R_non_cover_in_cover)
-            covered_primer_set = cover_primer_set.intersection(set(self.degenerate_seq(full_degenerate_primer)))
-            optimal_coverage_init = 0
-            for seq in covered_primer_set:
-                optimal_coverage_init += cover[seq]
-            F_mis_cover = optimal_coverage_init + F_mis_cover_cover
-            R_mis_cover = optimal_coverage_init + R_mis_cover_cover
-        else:
-            NN_matrix = self.trans_matrix(cover)
-            if len(cover_for_MM) != 0:
-                optimal_primer_index_NM = self.get_optimal_primer_by_viterbi(freq_matrix, NN_matrix)
-                optimal_primer_index_MM = self.get_optimal_primer_by_MM(cover_for_MM)
-                # print(optimal_primer_index_NM.tolist()) # array
-                # print(optimal_primer_index_MM) # list
-                #  if (optimal_primer_index_NM == optimal_primer_index_MM).all():
-                if optimal_primer_index_NM.tolist() == optimal_primer_index_MM:
-                    optimal_primer_index = optimal_primer_index_NM
-                    row_names = np.array(freq_matrix.index.values).reshape(1, -1)
-                    # build a list to store init base information in each position.
-                    optimal_primer_list = row_names[:, optimal_primer_index][0].tolist()
-                    # initiation coverage (optimal primer, used as base coverage)
-                    optimal_coverage_init = cover["".join(optimal_primer_list)]
-                    optimal_primer_current, F_mis_cover, R_mis_cover, information, F_non_cover, R_non_cover = \
-                        self.coverage_stast(cover, optimal_primer_index, NN_matrix, optimal_coverage_init, cover_number,
-                                            optimal_primer_list, cover_primer_set, non_gap_seq_id, F_non_cover,
-                                            R_non_cover)
-                else:
-                    F_non_cover_NM, R_non_cover_NM, F_non_cover_MM, R_non_cover_MM = {}, {}, {}, {}
-                    row_names = np.array(freq_matrix.index.values).reshape(1, -1)
-                    # build a list to store init base information in each position.
-                    optimal_primer_list_NM = row_names[:, optimal_primer_index_NM][0].tolist()
-                    # initiation coverage (optimal primer, used as base coverage)
-                    optimal_coverage_init_NM = cover["".join(optimal_primer_list_NM)]
-                    NN_matrix_NM = NN_matrix.copy()
-                    optimal_primer_current_NM, F_mis_cover_NM, R_mis_cover_NM, information_NM, F_non_cover_NM, \
-                    R_non_cover_NM = self.coverage_stast(cover, optimal_primer_index_NM, NN_matrix_NM,
-                                                         optimal_coverage_init_NM, cover_number, optimal_primer_list_NM,
-                                                         cover_primer_set, non_gap_seq_id, F_non_cover_NM,
-                                                         R_non_cover_NM)
-                    optimal_primer_list_MM = row_names[:, optimal_primer_index_MM][0].tolist()
-                    # initiation coverage (optimal primer, used as base coverage)
-                    optimal_coverage_init_MM = cover["".join(optimal_primer_list_MM)]
-                    NN_matrix_MM = NN_matrix.copy()
-                    optimal_primer_current_MM, F_mis_cover_MM, R_mis_cover_MM, information_MM, F_non_cover_MM, \
-                    R_non_cover_MM = self.coverage_stast(cover, optimal_primer_index_MM, NN_matrix_MM,
-                                                         optimal_coverage_init_MM, cover_number,
-                                                         optimal_primer_list_MM, cover_primer_set, non_gap_seq_id,
-                                                         F_non_cover_MM, R_non_cover_MM)
-                    if (F_mis_cover_NM + R_mis_cover_NM) > (F_mis_cover_MM + R_mis_cover_MM):
-                        optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, \
-                        F_non_cover, R_non_cover, NN_matrix = optimal_primer_current_NM, F_mis_cover_NM, \
-                                                              R_mis_cover_NM, information_NM, optimal_coverage_init_NM, \
-                                                              F_non_cover_NM, R_non_cover_NM, NN_matrix_NM
-                    else:
-                        optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, \
-                        F_non_cover, R_non_cover, NN_matrix = optimal_primer_current_MM, F_mis_cover_MM, \
-                                                              R_mis_cover_MM, information_MM, optimal_coverage_init_MM, \
-                                                              F_non_cover_MM, R_non_cover_MM, NN_matrix_MM
-                    # print(F_mis_cover)
-                    # print(R_mis_cover)
+        NN_matrix = self.trans_matrix(cover)
+        if len(cover_for_MM) != 0:
+            optimal_primer_index_NM = self.get_optimal_primer_by_viterbi(freq_matrix, NN_matrix)
+            optimal_primer_index_MM = self.get_optimal_primer_by_MM(cover_for_MM)
+            # print(optimal_primer_index_NM.tolist()) # array
+            # print(optimal_primer_index_MM) # list
+            #  if (optimal_primer_index_NM == optimal_primer_index_MM).all():
+            if optimal_primer_index_NM.tolist() == optimal_primer_index_MM:
+                optimal_primer_index = optimal_primer_index_NM
+                row_names = np.array(freq_matrix.index.values).reshape(1, -1)
+                # build a list to store init base information in each position.
+                optimal_primer_list = row_names[:, optimal_primer_index][0].tolist()
+                # initiation coverage (optimal primer, used as base coverage)
+                optimal_coverage_init = cover["".join(optimal_primer_list)]
+                optimal_primer_current, F_mis_cover, R_mis_cover, information, F_non_cover, R_non_cover = \
+                    self.coverage_stast(cover, optimal_primer_index, NN_matrix, optimal_coverage_init, cover_number,
+                                        optimal_primer_list, cover_primer_set, non_gap_seq_id, F_non_cover,
+                                        R_non_cover)
+                # print(F_mis_cover)
+                # print(R_mis_cover)
             else:
-                optimal_primer_index_NM = self.get_optimal_primer_by_viterbi(freq_matrix, NN_matrix)
                 F_non_cover_NM, R_non_cover_NM, F_non_cover_MM, R_non_cover_MM = {}, {}, {}, {}
                 row_names = np.array(freq_matrix.index.values).reshape(1, -1)
                 # build a list to store init base information in each position.
                 optimal_primer_list_NM = row_names[:, optimal_primer_index_NM][0].tolist()
                 # initiation coverage (optimal primer, used as base coverage)
                 optimal_coverage_init_NM = cover["".join(optimal_primer_list_NM)]
                 NN_matrix_NM = NN_matrix.copy()
                 optimal_primer_current_NM, F_mis_cover_NM, R_mis_cover_NM, information_NM, F_non_cover_NM, \
                 R_non_cover_NM = self.coverage_stast(cover, optimal_primer_index_NM, NN_matrix_NM,
                                                      optimal_coverage_init_NM, cover_number, optimal_primer_list_NM,
-                                                     cover_primer_set, non_gap_seq_id, F_non_cover_NM, R_non_cover_NM)
-                optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, F_non_cover, \
-                R_non_cover, NN_matrix = optimal_primer_current_NM, F_mis_cover_NM, R_mis_cover_NM, information_NM, \
-                                         optimal_coverage_init_NM, F_non_cover_NM, R_non_cover_NM, NN_matrix_NM
+                                                     cover_primer_set, non_gap_seq_id, F_non_cover_NM,
+                                                     R_non_cover_NM)
+                optimal_primer_list_MM = row_names[:, optimal_primer_index_MM][0].tolist()
+                # initiation coverage (optimal primer, used as base coverage)
+                optimal_coverage_init_MM = cover["".join(optimal_primer_list_MM)]
+                NN_matrix_MM = NN_matrix.copy()
+                optimal_primer_current_MM, F_mis_cover_MM, R_mis_cover_MM, information_MM, F_non_cover_MM, \
+                R_non_cover_MM = self.coverage_stast(cover, optimal_primer_index_MM, NN_matrix_MM,
+                                                     optimal_coverage_init_MM, cover_number,
+                                                     optimal_primer_list_MM, cover_primer_set, non_gap_seq_id,
+                                                     F_non_cover_MM, R_non_cover_MM)
+                if (F_mis_cover_NM + R_mis_cover_NM) > (F_mis_cover_MM + R_mis_cover_MM):
+                    optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, \
+                    F_non_cover, R_non_cover, NN_matrix = optimal_primer_current_NM, F_mis_cover_NM, \
+                                                          R_mis_cover_NM, information_NM, optimal_coverage_init_NM, \
+                                                          F_non_cover_NM, R_non_cover_NM, NN_matrix_NM
+                else:
+                    optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, \
+                    F_non_cover, R_non_cover, NN_matrix = optimal_primer_current_MM, F_mis_cover_MM, \
+                                                          R_mis_cover_MM, information_MM, optimal_coverage_init_MM, \
+                                                          F_non_cover_MM, R_non_cover_MM, NN_matrix_MM
+                # print(F_mis_cover)
+                # print(R_mis_cover)
+        else:
+            optimal_primer_index_NM = self.get_optimal_primer_by_viterbi(freq_matrix, NN_matrix)
+            F_non_cover_NM, R_non_cover_NM, F_non_cover_MM, R_non_cover_MM = {}, {}, {}, {}
+            row_names = np.array(freq_matrix.index.values).reshape(1, -1)
+            # build a list to store init base information in each position.
+            optimal_primer_list_NM = row_names[:, optimal_primer_index_NM][0].tolist()
+            # initiation coverage (optimal primer, used as base coverage)
+            optimal_coverage_init_NM = cover["".join(optimal_primer_list_NM)]
+            NN_matrix_NM = NN_matrix.copy()
+            optimal_primer_current_NM, F_mis_cover_NM, R_mis_cover_NM, information_NM, F_non_cover_NM, \
+            R_non_cover_NM = self.coverage_stast(cover, optimal_primer_index_NM, NN_matrix_NM,
+                                                 optimal_coverage_init_NM, cover_number, optimal_primer_list_NM,
+                                                 cover_primer_set, non_gap_seq_id, F_non_cover_NM, R_non_cover_NM)
+            optimal_primer_current, F_mis_cover, R_mis_cover, information, optimal_coverage_init, F_non_cover, \
+            R_non_cover, NN_matrix = optimal_primer_current_NM, F_mis_cover_NM, R_mis_cover_NM, information_NM, \
+                                     optimal_coverage_init_NM, F_non_cover_NM, R_non_cover_NM, NN_matrix_NM
+            # print(F_mis_cover)
+            # print(R_mis_cover)
         nonsense_primer_number = len(set(self.degenerate_seq(optimal_primer_current)) - set(cover.keys()))
         primer_degenerate_number = dege_number(optimal_primer_current)
         Tm, coverage = [], []
         for seq in self.degenerate_seq(optimal_primer_current):
             Tm.append(Calc_Tm_v2(seq))
             coverage.append(cover[seq])
         Tm_average = round(mean(Tm), 2)
@@ -577,37 +567,37 @@
                                             optimal_NN_coverage, NN_matrix)
                 F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
                     self.mis_primer_check(cover_primer_set, ''.join(optimal_primer_list), cover,
                                           non_gap_seq_id)
                 # If there is no increase in NN_coverage,
                 # it suggests the presence of bugs or a mismatch in continuous positions.
                 # Is this step necessary? or shall we use DegePrime method? or shall we use machine learning?
-                if F_mis_cover_cover == R_mis_cover_cover == cover_number - optimal_coverage_init:
+                if max(F_mis_cover_cover, R_mis_cover_cover) == cover_number:
                     break
                 elif optimal_NN_coverage_update == optimal_NN_coverage:
                     break
                 # If the degeneracy exceeds the threshold, the loop will break.
                 elif 2 * degeneracy > self.score_of_dege_bases or 3 * degeneracy / 2 > self.score_of_dege_bases \
                         or number_of_degenerate == self.number_of_dege_bases:
                     break
                 else:
                     optimal_NN_coverage = optimal_NN_coverage_update
         # If the primer coverage does not increase after degeneration,
         # the process will backtrack and assess the original optimal primer.
         # print(optimal_primer_list)
         optimal_primer_current = ''.join(optimal_primer_list)
-        # print(optimal_primer_current)
         information = self.primer_pre_filter(optimal_primer_current)
         # F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
         #     self.mis_primer_check(cover_primer_set, optimal_primer_current, cover,
         #                           non_gap_seq_id)
         F_non_cover.update(F_non_cover_in_cover)
         R_non_cover.update(R_non_cover_in_cover)
         F_mis_cover = optimal_coverage_init + F_mis_cover_cover
         R_mis_cover = optimal_coverage_init + R_mis_cover_cover
+        # print(F_mis_cover)
         return optimal_primer_current, F_mis_cover, R_mis_cover, information, F_non_cover, R_non_cover
 
     def refine_by_NN_array(self, optimal_primer_list, optimal_coverage_init, cover,
                            optimal_NN_index, optimal_NN_coverage, NN_array):
         # use minimum index of optimal_NN_coverage as the position to refine
         refine_index = np.where(optimal_NN_coverage == np.min(optimal_NN_coverage))[0]  # np.where[0] is a list
         # build dict to record coverage and NN array
@@ -781,38 +771,43 @@
             y_index = int(y.strip())
             if y_index > 0:
                 Y_strict.append(y_index)
                 Y_strict_R.append(self.primer_length - y_index)
             else:
                 Y_strict.append(self.primer_length + y_index + 1)
                 Y_strict_R.append(-y_index + 1)
-        return Y_strict, Y_strict_R
+        return set(Y_strict), set(Y_strict_R)
 
     def mis_primer_check(self, all_primers, optimal_primer, cover, non_gap_seq_id):
         # uncoverage sequence in cover dict
         optimal_primer_set = set(self.degenerate_seq(optimal_primer))
         uncover_primer_set = all_primers - optimal_primer_set
         F_non_cover, R_non_cover = {}, {}
         F_mis_cover, R_mis_cover = 0, 0
         for uncover_primer in uncover_primer_set:
             Y_dist = Y_distance(optimal_primer, uncover_primer)
+            # print(uncover_primer)
+            # print(Y_dist)
+            # print(set(Y_dist))
             if len(Y_dist) > self.variation:
                 # record sequence and acc_ID which will never mis-coverage. too many mismatch!
                 F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 R_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
             # if len(Y_dist) <= self.variation:
             else:
                 if len(set(Y_dist).intersection(self.Y_strict)) > 0:
                     F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 else:
                     F_mis_cover += cover[uncover_primer]
                 if len(set(Y_dist).intersection(self.Y_strict_R)) > 0:
                     R_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 else:
                     R_mis_cover += cover[uncover_primer]
+        # print(optimal_primer)
+        # print(F_mis_cover)
         return F_mis_cover, F_non_cover, R_mis_cover, R_non_cover
 
     ################# get_primers #####################
     def run(self):
         p = ProcessPoolExecutor(self.nproc)  #
         sequence_dict = self.seq_dict
         start_primer = self.start_position
@@ -858,14 +853,15 @@
                 json.dump(dict(gap_seq_id_out), fg, indent=4)
             fg.close()
             # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
             # but slow.
         p.shutdown()
 
 
+
 class Primers_filter(object):
     def __init__(self, ref_file, primer_file, adaptor, rep_seq_number=500, distance=4, outfile="", diff_Tm=5,
                  size="300,700", position=9, GC="0.4,0.6", nproc=10, fraction=0.6):
         self.nproc = nproc
         self.primer_file = primer_file
         self.adaptor = adaptor
         self.size = size
@@ -933,33 +929,23 @@
             seq.append([cs])
         return ("".join(i) for i in product(*seq))
 
     ################# Hairpin #####################
     def hairpin_check(self, primer):
         n = 0
         distance = self.distance
-        check = "FALSE"
         while n <= len(primer) - 5 - 5 - distance:
             kmer = self.degenerate_seq(primer[n:n + 5])
             left = self.degenerate_seq(primer[n + 5 + distance:])
             for k in kmer:
                 for l in left:
                     if re.search(RC(k), l):
-                        check = "TRUE"
-                        break
-                if check == "TRUE":
-                    break
-            if check == "TRUE":
-                break
+                        return True
             n += 1
-
-        if check == "TRUE":
-            return True
-        else:
-            return False
+        return False
 
     ################# current_end #####################
     def current_end(self, primer, adaptor="", num=5, length=14):
         primer_extend = adaptor + primer
         end_seq = []
         for i in range(num, (num + length)):
             s = primer_extend[-i:]
@@ -987,40 +973,30 @@
             Delta_G_list.append(Delta_G)
         return round(max(Delta_G_list), 2)
 
     ################# Dimer #####################
     def dimer_check(self, primer_F, primer_R):
         current_end_set = set(self.current_end(primer_F)).union(set(self.current_end(primer_R)))
         primer_pairs = [primer_F, primer_R]
-        dimer = False
         for pp in primer_pairs:
             for end in current_end_set:
                 for p in self.degenerate_seq(pp):
                     idx = p.find(RC(end))
                     if idx >= 0:
                         end_length = len(end)
                         end_GC = end.count("G") + end.count("C")
                         end_d1 = 0
                         end_d2 = len(p) - len(end) - idx
                         Loss = Penalty_points(
                             end_length, end_GC, end_d1, end_d2)
                         delta_G = self.deltaG(end)
                         # threshold = 3 or 3.6 or 3.96
                         if Loss > 3.6 or (delta_G < -5 and (end_d1 == end_d2)):
-                            dimer = True
-                            if dimer:
-                                break
-                if dimer:
-                    break
-            if dimer:
-                break
-        if dimer:
-            return True
-        else:
-            return False
+                            return True
+        return False
 
     ################# position of degenerate base #####################
     def dege_filter_in_term_N_bp(self, sequence):
         term = self.position
         if term == 0:
             term_base = ["A"]
         else:
@@ -1038,43 +1014,29 @@
         for seq in sequence_expand:
             GC_list.append(round((list(seq).count("G") + list(seq).count("C")) / len(list(seq)), 3))
         GC_average = mean(GC_list)
         return GC_average
 
     ################# di_nucleotide #####################
     def di_nucleotide(self, primer):
-        Check = "False"
         primers = self.degenerate_seq(primer)
         for m in primers:
             for n in di_nucleotides:
                 if re.search(n, m):
-                    Check = "True"
-                    break
-                else:
-                    pass
-            if Check == "True":
-                break
-        if Check == "True":
-            return True
-        else:
-            return False
+                    return True
+        return False
 
     ################# di_nucleotide #####################
     def GC_clamp(self, primer, num=4, length=13):
-        check = False
         for i in range(num, (num + length)):
             s = primer[-i:]
             gc_fraction = self.GC_fraction(s)
             if gc_fraction > 0.6:
-                check = True
-                break
-        if check:
-            return True
-        else:
-            return False
+                return True
+        return False
 
     def pre_filter(self):
         limits = self.GC.split(",")
         min = float(limits[0])
         max = float(limits[1])
         # min_cov = self.fraction
         candidate_primers_position = []
@@ -1199,18 +1161,24 @@
         max_len = int(size_list[1])
         candidate_position = self.pre_filter_primers
         adaptor = self.adaptor.split(",")
         primer_pairs = Manager().list()
         # print(candidate_position)
         coverage_threshold = 1 - self.fraction
         if int(candidate_position[-1]) - int(candidate_position[0]) < min_len:
-            # print("min len!")
-            pass
+            print("Max PCR product legnth < min len!")
+            ID = str(self.outfile)
+            with open(self.outfile, "w") as fo:
+                # headers = ["Primer_F_seq", "Primer_R_seq", "Product length:Tm:coverage_percentage",
+                # "Target number", "Primer_start_end"]
+                # fo.write(ID + "\t" + "\t".join(headers) + "\t")
+                fo.write(ID + "\n")
         else:
             for start in range(len(candidate_position)):
+                print(start)
                 p.submit(self.primer_pairs(start, adaptor, min_len, max_len, candidate_position, primer_pairs,
                                            coverage_threshold))
                 # This will submit all tasks to one place without blocking, and then each
                 # thread in the thread pool will fetch tasks.
             p.shutdown()
             # After I run the main, I don't care whether the sub thread is alive or dead. With this parameter,
             # after all the sub threads are executed, the main function is executed get results after shutdown.
@@ -1232,16 +1200,18 @@
                 # fo.write(ID + "\t" + "\t".join(headers) + "\t")
                 with open(self.outfile + ".fa", "w") as fa:
                     fo.write(ID + "\t")
                     primer_pairs_sort = sorted(primer_pairs, key=lambda k: k[3], reverse=True)
                     for i in primer_pairs_sort:
                         fo.write("\t".join(map(str, i)) + "\t")
                         start_stop = i[4].split(":")
-                        fa.write(">" + primer_ID + "_" + start_stop[0] + "F\n" + i[0] + "\n>" + primer_ID + "_" +
-                            start_stop[1]+ "R\n" + i[1] + "\n")
+                        fa.write(
+                            ">" + primer_ID + "_" + start_stop[0] + "F\n" + i[0] + "\n>" + primer_ID + "_" + start_stop[
+                                1]
+                            + "R\n" + i[1] + "\n")
                     # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
                     # but slow.
                     fo.write("\n")
                     fo.close()
                     fa.close()
 
 
@@ -1388,15 +1358,16 @@
                 "Coveraged number of sequence:\t{}\n"
                 "Rate of coverage:\t> {}\n".format(seq_number, len(Product_seq_id),
                                                    round(float(len(Product_seq_id)) / seq_number, 2)))
         c.close()
 
 
 class Errors(object):
-    def __init__(self, primer_file, term_length=18, reference_file="", mismatch_num=1, term_threshold=4, bowtie="",
+    def __init__(self, primer_file, term_length=int, reference_file=str, mismatch_num=1, term_threshold=4,
+                 bowtie="",
                  PCR_product_size="150,2000", outfile="", nproc=10, targets="None"):
         #  If an attribute in a Python class does not want to be accessed externally,
         #  we can start with a double underscore (__) when naming the attribute,
         #  Then the attribute cannot be accessed with the original variable name, making it private.
         #  If an attribute is marked with "__xxxx_" Is defined, then it can be accessed externally.
         self.bowtie = bowtie
         self.term_threshold = term_threshold
@@ -1614,7 +1585,34 @@
                 total_dict = pickle.load(raw_total_seq_dict)
                 print(len(set(total_dict.keys())), len(target_seq))
                 unmatched_seq_set = set(total_dict.keys()) - target_seq
                 with open(self.outfile + ".total.acc.num", "a+") as fo3:
                     fo3.write("total target number is: {}\n".format(len(total_dict.keys())))
                 for unmatch in unmatched_seq_set:
                     out.write(total_dict[unmatch])
+
+def Bowtie_index(Input, method):
+    Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
+    Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
+    bowtie_cmd = method + "-build"
+    if re.search("bowtie2", method):
+        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.bt2")
+        Bowtie_index = Path(Input).parent.joinpath(Path(Input).name).with_suffix(".1.bt2")
+    elif re.search("bowtie", method):
+        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.ebwt")
+        Bowtie_index = Path(Input).parent.joinpath(Path(Input).name).with_suffix(".1.ebwt")
+    else:
+        print("bowtie1 or bowtie2 must be specified !!!")
+        sys.exit(1)
+    if ref_index.exists():
+        return Bowtie_prefix
+    else:
+        if Bowtie_index.exists():
+            return Input
+        else:
+            if Bowtie_file.exists():
+                print("No Bowtie index found, start building ...")
+            else:
+                os.mkdir(Bowtie_file)
+            os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
+            return Bowtie_prefix
+
```

### Comparing `multiPrime-2.4.5/src/utils.py` & `multiPrime-2.4.6/src/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import argparse
 import os
 import re
 from optparse import OptionParser
 from pathlib import Path
 
 import numpy as np
 import sys
@@ -13,211 +14,97 @@
 from bisect import bisect_left
 
 
 # Melting temperature between 55-80◦C reduces the occurrence of hairpins
 # Runs of three or more Cs or Gs at the 3'-ends of primers may promote mispriming at G or C-rich sequences
 # (because of stability of annealing), and should be avoided.
 def DPrime_argsParse():
-    parser = OptionParser('Usage: %prog DPrime -i input -o output -p 10\n \
-                Options: { -l [18] -n [4] -d [10] -v [1] -g [0.2,0.7] -f [0.8] -c [4] -p [10] -a [4] }')
-    parser.add_option('-i', '--input',
-                      dest='input',
-                      help='Input file: multi-alignment output (muscle or others).')
-
-    parser.add_option('-l', '--plen',
-                      dest='plen',
-                      default=18,
-                      type="int",
-                      help='Length of primer. Default: 18.')
-
-    parser.add_option('-n', '--dnum',
-                      dest='dnum',
-                      default=4,
-                      type="int",
-                      help='Number of degenerate. Default: 4.')
-
-    parser.add_option('-d', '--degeneracy',
-                      dest='degeneracy',
-                      default=10,
-                      type="int",
-                      help='degeneracy of primer. Default: 10.')
-
-    parser.add_option('-v', '--variation',
-                      dest='variation',
-                      default=1,
-                      type="int",
-                      help='Max mismatch number of primer. Default: 1.')
-
-    parser.add_option('-e', '--entropy',
-                      dest='entropy',
-                      default=3.6,
-                      type="float",
-                      help='Entropy is actually a measure of disorder. This parameter is used to judge whether the '
-                           'window is conservation. Entropy of primer-length window. Default: 3.6.')
-
-    parser.add_option('-g', '--gc',
-                      dest='gc',
-                      default="0.2,0.7",
-                      help="Filter primers by GC content. Default [0.2,0.7].")
-
-    parser.add_option('-s', '--size',
-                      dest='size',
-                      default="100",
-                      type="int",
-                      help="Filter primers by mini PRODUCT size. Default 100.")
-
-    parser.add_option('-f', '--fraction',
-                      dest='fraction',
-                      default="0.8",
-                      type="float",
-                      help="Filter primers by match fraction. If you set -s lower than 0.8, make sure that "
-                           "--entropy greater than 3.6, because disorder region (entropy > 3.6) will not be processed "
-                           "in multiPrime. Even these regions can design coverage with error greater than your "
-                           "threshold, it wont be processed. Default: 0.8.")
-
-    parser.add_option('-c', '--coordinate',
-                      dest='coordinate',
-                      default="2,-1",
-                      type="str",
-                      help="Mismatch index is not allowed to locate in your specific positions."
-                           "otherwise, it won't be regard as the mis-coverage. "
-                           "With this param, you can control the index of Y-distance (number=variation and position "
-                           "of mismatch). "
-                           "when calculate coverage with error. coordinate>0: 5\'==>3\'; coordinate<0: 3\'==>5\'."
-                           "You can set this param to any value that you prefer. Default: 1,-1. "
-                           "1:  I dont want mismatch at the 2nd position, start from 0."
-                           "-1: I dont want mismatch at the -1st position, start from -1.")
-
-    parser.add_option('-p', '--proc',
-                      dest='proc',
-                      default="20",
-                      type="int",
-                      help="Number of process to launch. Default: 20.")
-
-    parser.add_option('-a', '--away',
-                      dest='away',
-                      default=4,
-                      type="int",
-                      help='Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. '
-                           'Example:(number of X) AGCT[XXXX]AGCT. '
-                           'Primers should not have complementary sequences (no consecutive 4 bp complementarities),'
-                           'otherwise the primers themselves will fold into hairpin structure.')
-
-    parser.add_option('-o', '--out',
-                      dest='out',
-                      help='Output file: candidate primers. e.g. [*].candidate.primers.txt.')
-    (options, args) = parser.parse_args()
-    if len(sys.argv) == 2:
-        parser.print_help()
-        sys.exit(1)
-    elif options.input is None:
-        parser.print_help()
-        print("Input file must be specified !!!")
-        sys.exit(1)
-    elif options.out is None:
-        parser.print_help()
-        print("No output file provided !!!")
-        sys.exit(1)
+    parser = argparse.ArgumentParser(description="For degenerate primer design")
+    parser.add_argument("-i", "--input", type=str, required=True,
+                        help="Input file: multi-alignment output (muscle or others).", metavar="<file>")
+    parser.add_argument("-l", "--plen", type=int, default=18,
+                        help='Length of primer. Default: 18.', metavar="<int>")
+    parser.add_argument("-n", "--dnum", type=int, default=4,
+                        help='Max number of degenerate. Default: 4.', metavar="<int>")
+    parser.add_argument("-d", "--degeneracy", type=int, default=10,
+                        help='Max degeneracy of primer. Default: 10.', metavar="<int>")
+    parser.add_argument("-v", "--variation", type=int, default=1,
+                        help='Max mismatch number of primer. Default: 1', metavar="<int>")
+    parser.add_argument("-e", "--entropy", type=float, default=3.6,
+                        help='Entropy is actually a measure of disorder. This parameter is used to judge whether the '
+                             'window is conservation. Entropy of primer-length window. Default: 3.6.',
+                        metavar="<float>")
+    parser.add_argument("-g", "--gc", type=str, default="0.2,0.7",
+                        help='Filter primers by GC content. Default [0.2,0.7].', metavar="<str>")
+    parser.add_argument("-s", "--size", type=int, default=100,
+                        help='Filter primers by mini PRODUCT size. Default 100.', metavar="<int>")
+    parser.add_argument("-f", "--fraction", type=float, default=0.8,
+                        help='Filter primers by match fraction. If you set -s lower than 0.8, make sure that'
+                             '--entropy greater than 3.6, because disorder region (entropy > 3.6) will not be processed'
+                             'in multiPrime. Even these regions can design coverage with error greater than your '
+                             'threshold, it wont be processed. Default: 0.8.', metavar="<float>")
+    parser.add_argument("-c", "--coordinate", type=str, default="1,2,-1",
+                        help='Mismatch index is not allowed to locate in your specific positions.'
+                             'otherwise, it wont be regard as the mis-coverage. With this param, '
+                             'you can control the index of Y-distance (number=variation and position of mismatch)'
+                             'when calculate coverage with error. coordinate>0: 5\'==>3\'; coordinate<0: 3\'==>5\'.'
+                             'You can set this param to any value that you prefer. Default: 1,-1. '
+                             '1:  I dont want mismatch at the 2nd position, start from 0.'
+                             '-1: I dont want mismatch at the -1st position, start fro -1.', metavar="<str>")
+    parser.add_argument("-p", "--proc", type=int, default=20,
+                        help='Number of process to launch. Default: 20.', metavar="<int>")
+    parser.add_argument("-a", "--away", type=int, default=4,
+                        help='Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. '
+                             'Example:(number of X) AGCT[XXXX]AGCT. '
+                             'Primers should not have complementary sequences (no consecutive 4 bp complementarities),'
+                             'otherwise the primers themselves will fold into hairpin structure.', metavar="<int>")
+    parser.add_argument("-o", "--out", type=str, required=True,
+                        help='output file', metavar="<file>")
     return parser.parse_args()
 
-
-
 def Ppair_argsParse():
-    parser = OptionParser('Usage: %prog Ppair -i [input] -r [sequence.fa] -o [output] \n \
-                Options: {-f [0.6] -m [500] -n [200] -e [4] -p [9] -s [250,500] -g [0.4,0.6] -d [4] -a ","}.')
-    parser.add_option('-i', '--input',
-                      dest='input',
-                      help='Input file: multiPrime out.')
-
-    parser.add_option('-r', '--ref',
-                      dest='ref',
-                      help='Reference sequence file: all the sequence in 1 fasta, for example: (Cluster_96_171.tfa).')
-
-    parser.add_option('-g', '--gc',
-                      dest='gc',
-                      default="0.2,0.7",
-                      help="Filter primers by GC content. Default [0.2,0.7].")
-
-    parser.add_option('-f', '--fraction',
-                      dest='fraction',
-                      default="0.6",
-                      type="float",
-                      help="Filter primers by match fraction. Default: 0.6. \n"
-                           "Sometimes you need a small fraction to get output.")
-
-    parser.add_option('-e', '--end',
-                      dest='end',
-                      default="4",
-                      type="int",
-                      help="Filter primers by degenerate base position. e.g. [-e 4] means I dont want degenerate base "
-                           "appear at the end four bases when primer pre-filter. Default: 4.")
-
-    parser.add_option('-p', '--proc',
-                      dest='proc',
-                      default="10",
-                      type="int",
-                      help="Number of process to launch.  default: 10.")
-
-    parser.add_option('-s', '--size',
-                      dest='size',
-                      default="250,500",
-                      help="Filter primers by PRODUCT size. Default [250,500].")
-
-    parser.add_option('-d', '--dist',
-                      dest='dist',
-                      default=4,
-                      type="int",
-                      help='Filter param of hairpin, which means distance of the minimal paired bases. Default: 4. '
-                           'Example:(number of X) AGCT[XXXX]AGCT.')
-
-    parser.add_option('-t', '--tm',
-                      dest='Tm',
-                      default=5,
-                      type="int",
-                      help='Difference of Tm between primer-F and primer-R. Default: 5. ')
-
-    parser.add_option('-a', '--adaptor',
-                      dest='adaptor',
-                      default="TCTTTCCCTACACGACGCTCTTCCGATCT,TCTTTCCCTACACGACGCTCTTCCGATCT",
-                      type="str",
-                      help='Adaptor sequence, which is used for NGS next. Hairpin or dimer detection for [adaptor--primer].'
-                           '\n \ For example: TCTTTCCCTACACGACGCTCTTCCGATCT,TCTTTCCCTACACGACGCTCTTCCGATCT (Default). ''If '
-                           'you dont want adaptor, use [","] ')
-
-    parser.add_option('-m', '--maxseq',
-                      dest='maxseq',
-                      default=0,
-                      type="int",
-                      help='Limit of sequence number. Default: 0. If 0, then all sequence will take into account.\n'
-                           'This param should consistent with [max_seq] in multi-alignment [muscle].')
-
-    parser.add_option('-o', '--out',
-                      dest='out',
-                      help='Output file: candidate primer pairs. e.g. [*].candidate.primers.txt.'
-                           'Header of output: Primer_F_seq, Primer_R_seq, Product length:Tm:coverage_percentage, '
-                           'coverage_number, Primer_start_end')
-    (options, args) = parser.parse_args()
-    if len(sys.argv) == 2:
-        parser.print_help()
-        sys.exit(1)
-    elif options.input is None:
-        parser.print_help()
-        print("Input file must be specified !!!")
-        sys.exit(1)
-    elif options.ref is None:
-        parser.print_help()
-        print("Reference file must be specified !!!")
-        sys.exit(1)
-    elif options.out is None:
-        parser.print_help()
-        print("No output file provided !!!")
-        sys.exit(1)
+    parser = argparse.ArgumentParser(description="For degenerate primer design")
+    parser.add_argument("-i", "--input", type=str, required=True,
+                        help="Input file: multiPrime out.", metavar="<file>")
+    parser.add_argument("-r", "--ref", type=str, required=True,
+                        help='Reference sequence file: all the sequence in 1 fasta, for example: (Cluster_96_171.tfa).',
+                        metavar="<str>")
+    parser.add_argument("-g", "--gc", type=str, default="0.2,0.7",
+                        help='Filter primers by GC content. Default [0.2,0.7].', metavar="<str>")
+    parser.add_argument("-f", "--fraction", type=float, default=0.6,
+                        help='Filter primers by match fraction.Sometimes you need a small fraction to get output.'
+                             'Default: 0.6.', metavar="<float>")
+    parser.add_argument("-e", "--end", type=int, default=4,
+                        help='Filter primers by degenerate base position. e.g. [-t 4] means I dont want degenerate base'
+                             'appear at the end four bases when primer pre-filter. Default: 4.', metavar="<int>")
+    parser.add_argument("-p", "--proc", type=int, default=20,
+                        help='Number of process to launch. Default: 20.', metavar="<int>")
+    parser.add_argument("-s", "--size", type=str, default="250,500",
+                        help='Filter primers by PRODUCT size. Default [250,500].', metavar="<str>")
+    parser.add_argument("-d", "--dist", type=int, default=4,
+                        help='Filter param of hairpin, which means distance of the minimal paired bases. Default: 4.'
+                             'Example:(number of X) AGCT[XXXX]AGCT.', metavar="<int>")
+    parser.add_argument("-t", "--Tm", type=int, default=4,
+                        help='Difference of Tm between primer-F and primer-R. Default: 4.', metavar="<int>")
+    parser.add_argument("-a", "--adaptor", type=str, default="TCTTTCCCTACACGACGCTCTTCCGATCT,"
+                                                             "TCTTTCCCTACACGACGCTCTTCCGATCT",
+                        help='Adaptor sequence, which is used for NGS next. Hairpin or dimer detection for ['
+                             'adaptor--primer]. For example: TCTTTCCCTACACGACGCTCTTCCGATCT,'
+                             'TCTTTCCCTACACGACGCTCTTCCGATCT (Default). If you dont want adaptor, use [","]',
+                        metavar="<str>")
+    parser.add_argument("-m", "--maxseq", type=int, default=0,
+                        help='Limit of sequence number. Default: 0. If 0, then all sequence will take into account.\n'
+                             'This param should consistent with [max_seq] in multi-alignment [muscle].',
+                        metavar="<int>")
+    parser.add_argument("-o", "--out", type=str, required=True,
+                        help='Output file: candidate primers. e.g. [*].candidate.primers.txt.'
+                             'Header of output: Primer_F_seq, Primer_R_seq, Product length:Tm:coverage_percentage,'
+                             'coverage_number, Primer_start_end', metavar="<file>")
     return parser.parse_args()
 
-
 def Perfect_argsParse():
     parser = OptionParser('Usage: %prog Perfect -r [reference] -i [input] -p [10] -f [format] -o [output] '
                           '-s [Coverage.xls]', version="%prog 0.0.2")
     parser.add_option('-r', '--ref',
                       dest='ref',
                       help='reference file: all the input sequences in 1 fasta.')
 
@@ -266,101 +153,52 @@
         sys.exit(1)
     elif options.out is None:
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
-
 def Errors_argsParse():
-    parser = OptionParser('Usage: %prog -i [input] -r [reference fasta] -l [150,2000] -p [10]-o [output]',
-                          version="%prog 0.0.8")
-
-    parser.add_option('-i', '--input',
-                      dest='input_file',
-                      help='input file: primer.fa.')
-
-    parser.add_option('-r', '--ref',
-                      dest='ref',
-                      help='Reference file.The program will first search for Bowtie index files using the parameter '
-                           'you provided as the prefix.'
-                           'If the files are not found, it will build an index using the prefix you provided. '
-                           'else, the program will use the Bowtie index prefix you provided.')
-
-    parser.add_option('-l', '--len',
-                      dest='len',
-                      default=0,
-                      type="int",
-                      help='Length of primer, which is used for mapping. '
-                           'If the length of the primer used for mapping is set to 0, '
-                           'the entire length of the primer will be utilized. '
-                           'Default: 0')
-
-    parser.add_option('-t', '--term',
-                      dest='term',
-                      default=4,
-                      type="int",
-                      help='Position of mismatch is not allowed in the 3 term of primer. Default: 4')
-
-    parser.add_option('-s', '--s',
-                      dest='size',
-                      default="100,1500",
-                      type="str",
-                      help='Length of PCR product, default: 100,1500.')
-
-    parser.add_option('-p', '--proc',
-                      dest='proc',
-                      default="20",
-                      type="int",
-                      help='Number of process. Default: 20')
-
-    parser.add_option('-b', '--bowtie',
-                      dest='bowtie',
-                      default="bowtie2",
-                      type="string",
-                      help='bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. '
-                           'Default: bowtie2')
-
-    parser.add_option('-m', '--seedmms',
-                      dest='seedmms',
-                      default="1",
-                      type="int",
-                      help='Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).'
-                           'Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).')
-
-    parser.add_option('-d', '--dict',
-                      dest='dict',
-                      default="None",
-                      help='Dictionary of targets sequences, binary format. '
-                           'It can be obtained from prepare_fa_pickle.py (https://github.com/joybio/multiPrime).')
-
-    parser.add_option('-o', '--out',
-                      dest='out',
-                      help='Prodcut of PCR product with primers.')
-
-    (options, args) = parser.parse_args()
-    if len(sys.argv) == 1:
-        parser.print_help()
-        sys.exit(1)
-    elif options.input_file is None:
-        parser.print_help()
-        print("Input file must be specified !!!")
-        sys.exit(1)
-    elif options.ref is None:
-        parser.print_help()
-        print("reference (fasta) must be specified !!!")
-        sys.exit(1)
-    elif options.out is None:
-        parser.print_help()
-        print("No output file provided !!!")
-        sys.exit(1)
+    parser = argparse.ArgumentParser(description="For mismatch coverage stastic.")
+    parser.add_argument("-i", "--input", type=str, required=True,
+                        help="input file: primer.fa.", metavar="<file>")
+    parser.add_argument("-r", "--ref", type=str, required=True,
+                        help='Reference sequence file: Reference file. The program will first search for Bowtie index '
+                             'files using the parameter you provided as the prefix. If the files are not found, '
+                             'it will build an index using the prefix you provided. Otherwise, '
+                             'the program will use the Bowtie index prefix you provided.',
+                        metavar="<str>")
+    parser.add_argument("-l", "--len", type=int, default=0,
+                        help='Length of primer, which is used for mapping. If the length of the primer used for '
+                             'mapping is set to 0, the entire length of the primer will be utilized. Default: 0',
+                        metavar="<int>")
+    parser.add_argument("-t", "--term", type=int, default=4,
+                        help='Position of mismatch is not allowed in the 3 term of primer. Default: 4', metavar="<int>")
+    parser.add_argument("-s", "--size", type=str, default="100,1500",
+                        help='Length of PCR product, default: 100,1500.', metavar="<str>")
+    parser.add_argument("-p", "--proc", type=int, default=20,
+                        help='Number of process to launch. Default: 20.', metavar="<int>")
+
+    parser.add_argument("-b", "--bowtie", type=str, default="bowtie2",
+                        help='bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. '
+                             'Default: bowtie2', metavar="<str>")
+    parser.add_argument("-m", "--seedmms", type=int, default=1,
+                        help='Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).'
+                             'Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1)',
+                        metavar="<int>")
+    parser.add_argument("-d", "--dict", type=str, default="None",
+                        help='Dictionary of targets sequences, binary format. '
+                             'It can be obtained from prepare_fa_pickle.py.', metavar="<str>")
+    parser.add_argument("-o", "--out", type=str, required=True,
+                        help='Output file: Prodcut of PCR product with primers.', metavar="<file>")
     return parser.parse_args()
 
+
 def main_Usage():
-    print('Usage (version 2.4.5): \n'
+    print('Usage (version 2.4.6): \n'
           'multiPrime DPrime:  Degenerate primer design through MD-DPD or MD-EDPD.\n'
           'multiPrime Ppair:   Primer pair selection from the result of multiPrime DPrime.\n'
           'multiPrime Perfect: Extract primer-contained sequences with non-mismatches.\n'
           'multiPrime Errors:  Extract primer-contained sequences with errors.\n')
 
 
 degenerate_base = {"-": ["-"], "A": ["A"], "G": ["G"], "C": ["C"], "T": ["T"], "R": ["A", "G"], "Y": ["C", "T"],
```

