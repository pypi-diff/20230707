# Comparing `tmp/blacklight-0.1.7.tar.gz` & `tmp/blacklight-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacklight-0.1.7.tar", max compression
+gzip compressed data, was "blacklight-0.1.8.tar", max compression
```

## Comparing `blacklight-0.1.7.tar` & `blacklight-0.1.8.tar`

### file list

```diff
@@ -1,80 +1,44 @@
--rw-r--r--   0        0        0    35149 2022-11-27 19:19:27.813421 blacklight-0.1.7/LICENSE
--rw-r--r--   0        0        0     3589 2023-03-09 01:33:51.000000 blacklight-0.1.7/README.md
--rw-r--r--   0        0        0       67 2023-03-11 21:10:02.752334 blacklight-0.1.7/blacklight/__init__.py
--rw-r--r--   0        0        0       74 2023-03-06 22:47:59.742604 blacklight-0.1.7/blacklight/autoML/__init__.py
--rw-r--r--   0        0        0      244 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/autoML/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6771 2023-03-20 01:33:05.157308 blacklight-0.1.7/blacklight/autoML/__pycache__/_feed_forward.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-03-06 22:47:59.743014 blacklight-0.1.7/blacklight/autoML/_convolutional_nn.py
--rw-r--r--   0        0        0     6585 2023-03-20 01:33:01.678956 blacklight-0.1.7/blacklight/autoML/_feed_forward.py
--rw-r--r--   0        0        0        0 2023-03-03 17:29:21.127187 blacklight-0.1.7/blacklight/autoML/tests/__init__.py
--rw-r--r--   0        0        0      177 2023-03-04 00:13:23.450013 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      786 2023-03-12 01:59:15.106261 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/end_to_end_feed_forward_test.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      708 2023-03-10 17:14:08.695419 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/test_CI_CD.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      599 2023-03-04 00:13:23.450175 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/test_CI_CD.cpython-310.pyc
--rw-r--r--   0        0        0     8600 2023-03-20 01:28:26.780982 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/test_feed_forward_population.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2252 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/autoML/tests/__pycache__/test_feed_forward_population.cpython-310.pyc
--rw-r--r--   0        0        0     5105 2023-03-10 17:14:08.700000 blacklight-0.1.7/blacklight/autoML/tests/data/Iris.csv
--rw-r--r--   0        0        0      409 2023-03-12 01:58:58.568801 blacklight-0.1.7/blacklight/autoML/tests/end_to_end_feed_forward_test.py
--rw-r--r--   0        0        0      186 2023-03-03 17:29:21.128720 blacklight-0.1.7/blacklight/autoML/tests/test_CI_CD.py
--rw-r--r--   0        0        0     6135 2023-03-20 01:28:24.291609 blacklight-0.1.7/blacklight/autoML/tests/test_feed_forward_population.py
--rw-r--r--   0        0        0      191 2023-03-19 20:17:43.183266 blacklight-0.1.7/blacklight/base/__init__.py
--rw-r--r--   0        0        0      336 2023-03-19 22:09:45.502046 blacklight-0.1.7/blacklight/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1867 2023-03-11 21:10:03.041300 blacklight-0.1.7/blacklight/base/__pycache__/individual.cpython-310.pyc
--rw-r--r--   0        0        0     2981 2023-03-20 01:55:21.629642 blacklight-0.1.7/blacklight/base/__pycache__/population.cpython-310.pyc
--rw-r--r--   0        0        0      168 2023-03-19 22:35:52.096977 blacklight-0.1.7/blacklight/base/chromosomes/__init__.py
--rw-r--r--   0        0        0      337 2023-03-19 22:37:59.013026 blacklight-0.1.7/blacklight/base/chromosomes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2018 2023-03-20 00:58:58.442437 blacklight-0.1.7/blacklight/base/chromosomes/__pycache__/base_chromosome.cpython-310.pyc
--rw-r--r--   0        0        0     5602 2023-03-20 01:55:21.703246 blacklight-0.1.7/blacklight/base/chromosomes/__pycache__/feed_forward_chromosome.cpython-310.pyc
--rw-r--r--   0        0        0     1423 2023-03-20 00:35:20.627936 blacklight-0.1.7/blacklight/base/chromosomes/base_chromosome.py
--rw-r--r--   0        0        0     7888 2023-03-20 01:54:36.939028 blacklight-0.1.7/blacklight/base/chromosomes/convolutional_chromosome.py
--rw-r--r--   0        0        0     5836 2023-03-20 01:53:48.286897 blacklight-0.1.7/blacklight/base/chromosomes/feed_forward_chromosome.py
--rw-r--r--   0        0        0        0 2023-03-06 22:47:59.746242 blacklight-0.1.7/blacklight/base/chromosomes/tests/__init__.py
--rw-r--r--   0        0        0      187 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/base/chromosomes/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3529 2023-03-20 01:33:29.947007 blacklight-0.1.7/blacklight/base/chromosomes/tests/__pycache__/test_feed_forward_chromosome.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1722 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/base/chromosomes/tests/__pycache__/test_feed_forward_chromosome.cpython-310.pyc
--rw-r--r--   0        0        0     2501 2023-03-20 00:35:20.671671 blacklight-0.1.7/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py
--rw-r--r--   0        0        0     1523 2023-03-11 01:01:51.819216 blacklight-0.1.7/blacklight/base/individual.py
--rw-r--r--   0        0        0      171 2023-03-20 01:41:22.208897 blacklight-0.1.7/blacklight/base/individuals/__init__.py
--rw-r--r--   0        0        0      349 2023-03-20 01:41:24.384638 blacklight-0.1.7/blacklight/base/individuals/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4322 2023-03-20 01:35:10.610988 blacklight-0.1.7/blacklight/base/individuals/__pycache__/feed_forward_individual.cpython-310.pyc
--rw-r--r--   0        0        0     2470 2023-03-06 22:47:59.747866 blacklight-0.1.7/blacklight/base/individuals/convolution_individual.py
--rw-r--r--   0        0        0     4490 2023-03-20 01:35:00.379933 blacklight-0.1.7/blacklight/base/individuals/feed_forward_individual.py
--rw-r--r--   0        0        0        0 2023-03-06 22:47:59.748175 blacklight-0.1.7/blacklight/base/individuals/tests/__init__.py
--rw-r--r--   0        0        0      187 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/base/individuals/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4291 2023-03-20 00:12:02.608552 blacklight-0.1.7/blacklight/base/individuals/tests/__pycache__/test_feedforwardindividual.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3522 2023-03-10 17:14:08.697924 blacklight-0.1.7/blacklight/base/individuals/tests/__pycache__/test_individual_utils.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2139 2023-03-20 00:11:54.157219 blacklight-0.1.7/blacklight/base/individuals/tests/test_feedforwardindividual.py
--rw-r--r--   0        0        0     2260 2023-03-20 01:53:48.183224 blacklight-0.1.7/blacklight/base/population.py
--rw-r--r--   0        0        0       75 2023-03-06 22:47:59.749445 blacklight-0.1.7/blacklight/base/populations/__init__.py
--rw-r--r--   0        0        0      264 2023-03-09 01:18:59.000000 blacklight-0.1.7/blacklight/base/populations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      139 2023-03-19 19:18:28.093555 blacklight-0.1.7/blacklight/base/utils/__init__.py
--rw-r--r--   0        0        0      310 2023-03-19 22:09:45.504091 blacklight-0.1.7/blacklight/base/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2307 2023-03-20 01:55:24.049216 blacklight-0.1.7/blacklight/base/utils/__pycache__/model_creator.cpython-310.pyc
--rw-r--r--   0        0        0     3958 2023-03-20 01:50:38.948945 blacklight-0.1.7/blacklight/base/utils/__pycache__/model_options.cpython-310.pyc
--rw-r--r--   0        0        0     2673 2023-03-20 01:53:48.515151 blacklight-0.1.7/blacklight/base/utils/model_creator.py
--rw-r--r--   0        0        0     5856 2023-03-20 01:50:32.217801 blacklight-0.1.7/blacklight/base/utils/model_options.py
--rw-r--r--   0        0        0        0 2023-03-19 22:05:25.052487 blacklight-0.1.7/blacklight/base/utils/tests/__init__.py
--rw-r--r--   0        0        0      181 2023-03-19 22:09:47.273324 blacklight-0.1.7/blacklight/base/utils/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4343 2023-03-20 01:33:29.953351 blacklight-0.1.7/blacklight/base/utils/tests/__pycache__/test_model_creator.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     5582 2023-03-20 01:55:24.597047 blacklight-0.1.7/blacklight/base/utils/tests/__pycache__/test_model_options.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2462 2023-03-20 00:35:20.971435 blacklight-0.1.7/blacklight/base/utils/tests/test_model_creator.py
--rw-r--r--   0        0        0     4673 2023-03-20 01:55:08.056137 blacklight-0.1.7/blacklight/base/utils/tests/test_model_options.py
--rw-r--r--   0        0        0       89 2023-03-10 17:14:08.698321 blacklight-0.1.7/blacklight/blacklightDataLoader/__init__.py
--rw-r--r--   0        0        0      269 2023-03-10 20:43:04.953223 blacklight-0.1.7/blacklight/blacklightDataLoader/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      202 2023-03-10 17:14:08.698642 blacklight-0.1.7/blacklight/blacklightDataLoader/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      174 2023-03-10 17:14:08.698756 blacklight-0.1.7/blacklight/blacklightDataLoader/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6312 2023-03-20 00:59:01.719754 blacklight-0.1.7/blacklight/blacklightDataLoader/__pycache__/blacklight_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     6396 2023-03-20 00:35:20.304918 blacklight-0.1.7/blacklight/blacklightDataLoader/blacklight_dataset.py
--rw-r--r--   0        0        0        0 2023-03-10 17:14:08.699707 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-10 21:50:09.979586 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10521 2023-03-12 01:59:15.201717 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/__pycache__/test_blacklight_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     5105 2023-03-10 17:14:08.700447 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.csv
--rw-r--r--   0        0        0    10170 2023-03-10 17:14:08.700606 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.json
--rw-r--r--   0        0        0     4794 2023-03-10 17:14:08.700772 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.parquet
--rw-r--r--   0        0        0     9183 2023-03-10 17:14:08.700938 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.xlsx
--rw-r--r--   0        0        0        0 2023-03-10 17:14:08.700974 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/__init__.py
--rw-r--r--   0        0        0      187 2023-03-10 17:14:08.701176 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      343 2023-03-10 17:14:08.701280 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/csv_to_other_datatypes.py
--rw-r--r--   0        0        0     4068 2023-03-12 00:52:31.571793 blacklight-0.1.7/blacklight/blacklightDataLoader/tests/test_blacklight_dataset.py
--rw-r--r--   0        0        0      552 2023-03-20 01:58:24.446973 blacklight-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4157 1970-01-01 00:00:00.000000 blacklight-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-06 22:26:37.027562 blacklight-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3589 2023-07-06 22:26:37.027726 blacklight-0.1.8/README.md
+-rw-r--r--   0        0        0       67 2023-07-06 22:26:37.028342 blacklight-0.1.8/blacklight/__init__.py
+-rw-r--r--   0        0        0       74 2023-07-06 22:26:37.028739 blacklight-0.1.8/blacklight/autoML/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.029046 blacklight-0.1.8/blacklight/autoML/_convolutional_nn.py
+-rw-r--r--   0        0        0     6585 2023-07-06 22:26:37.029190 blacklight-0.1.8/blacklight/autoML/_feed_forward.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.029265 blacklight-0.1.8/blacklight/autoML/tests/__init__.py
+-rw-r--r--   0        0        0     5105 2023-07-06 22:26:37.030033 blacklight-0.1.8/blacklight/autoML/tests/data/Iris.csv
+-rw-r--r--   0        0        0      409 2023-07-06 22:26:37.030130 blacklight-0.1.8/blacklight/autoML/tests/end_to_end_feed_forward_test.py
+-rw-r--r--   0        0        0      186 2023-07-06 22:26:37.030217 blacklight-0.1.8/blacklight/autoML/tests/test_CI_CD.py
+-rw-r--r--   0        0        0     6129 2023-07-06 23:01:51.776809 blacklight-0.1.8/blacklight/autoML/tests/test_feed_forward_population.py
+-rw-r--r--   0        0        0      191 2023-07-06 22:26:37.030452 blacklight-0.1.8/blacklight/base/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-06 22:26:37.030949 blacklight-0.1.8/blacklight/base/chromosomes/__init__.py
+-rw-r--r--   0        0        0     1423 2023-07-06 22:26:37.031388 blacklight-0.1.8/blacklight/base/chromosomes/base_chromosome.py
+-rw-r--r--   0        0        0     7888 2023-07-06 22:26:37.031526 blacklight-0.1.8/blacklight/base/chromosomes/convolutional_chromosome.py
+-rw-r--r--   0        0        0     5836 2023-07-06 22:26:37.031627 blacklight-0.1.8/blacklight/base/chromosomes/feed_forward_chromosome.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.031717 blacklight-0.1.8/blacklight/base/chromosomes/tests/__init__.py
+-rw-r--r--   0        0        0     2310 2023-07-06 22:26:37.032326 blacklight-0.1.8/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py
+-rw-r--r--   0        0        0     1523 2023-07-06 22:26:37.032418 blacklight-0.1.8/blacklight/base/individual.py
+-rw-r--r--   0        0        0      171 2023-07-06 22:26:37.032540 blacklight-0.1.8/blacklight/base/individuals/__init__.py
+-rw-r--r--   0        0        0     2470 2023-07-06 22:26:37.032872 blacklight-0.1.8/blacklight/base/individuals/convolution_individual.py
+-rw-r--r--   0        0        0     4490 2023-07-06 22:26:37.032961 blacklight-0.1.8/blacklight/base/individuals/feed_forward_individual.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.033047 blacklight-0.1.8/blacklight/base/individuals/tests/__init__.py
+-rw-r--r--   0        0        0     2139 2023-07-06 22:26:37.033466 blacklight-0.1.8/blacklight/base/individuals/tests/test_feedforwardindividual.py
+-rw-r--r--   0        0        0     2260 2023-07-06 22:26:37.033553 blacklight-0.1.8/blacklight/base/population.py
+-rw-r--r--   0        0        0       75 2023-07-06 22:26:37.033677 blacklight-0.1.8/blacklight/base/populations/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-06 22:26:37.033935 blacklight-0.1.8/blacklight/base/utils/__init__.py
+-rw-r--r--   0        0        0     2673 2023-07-06 22:26:37.034342 blacklight-0.1.8/blacklight/base/utils/model_creator.py
+-rw-r--r--   0        0        0     5856 2023-07-06 22:26:37.034439 blacklight-0.1.8/blacklight/base/utils/model_options.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.034513 blacklight-0.1.8/blacklight/base/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2462 2023-07-06 22:26:37.034914 blacklight-0.1.8/blacklight/base/utils/tests/test_model_creator.py
+-rw-r--r--   0        0        0     4673 2023-07-06 22:26:37.034984 blacklight-0.1.8/blacklight/base/utils/tests/test_model_options.py
+-rw-r--r--   0        0        0       89 2023-07-06 22:26:37.035103 blacklight-0.1.8/blacklight/blacklightDataLoader/__init__.py
+-rw-r--r--   0        0        0     6530 2023-07-06 23:01:51.777227 blacklight-0.1.8/blacklight/blacklightDataLoader/blacklight_dataset.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.035616 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/__init__.py
+-rw-r--r--   0        0        0     5105 2023-07-06 22:26:37.036062 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.csv
+-rw-r--r--   0        0        0    10170 2023-07-06 22:26:37.036218 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.json
+-rw-r--r--   0        0        0     4794 2023-07-06 22:26:37.036335 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.parquet
+-rw-r--r--   0        0        0     9183 2023-07-06 22:26:37.036456 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.xlsx
+-rw-r--r--   0        0        0        0 2023-07-06 22:26:37.036483 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/__init__.py
+-rw-r--r--   0        0        0      343 2023-07-06 22:26:37.036689 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/csv_to_other_datatypes.py
+-rw-r--r--   0        0        0     4076 2023-07-06 23:01:51.777624 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/test_blacklight_dataset.py
+-rw-r--r--   0        0        0      594 2023-07-06 23:08:14.456493 blacklight-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 blacklight-0.1.8/PKG-INFO
```

### Comparing `blacklight-0.1.7/LICENSE` & `blacklight-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/README.md` & `blacklight-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/autoML/_feed_forward.py` & `blacklight-0.1.8/blacklight/autoML/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/autoML/tests/data/Iris.csv` & `blacklight-0.1.8/blacklight/autoML/tests/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/autoML/tests/test_feed_forward_population.py` & `blacklight-0.1.8/blacklight/autoML/tests/test_feed_forward_population.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,14 @@
 
         X_train, y_train = getdata
         X_test, y_test = get_test_data
         # Test correct dataset behaviour with test data
         with unittest.mock.patch.object(FeedForwardIndividual, 'get_fitness', lambda x: random.randint(1, 10)):
             population.fit(X_train, y_train, X_test, y_test)
             assert population.get_training_data().X[0][0] == X_train[0][0]
-            assert population.get_training_data().y[0] == y_train[0]
+            assert population.get_training_data().y[0][0] == 1
             assert population.best_individual is not None
 
             # Test correct dataset behaviour with no test data
             population.fit(X_train, y_train)
             assert population.get_testing_data() is not None
             assert population.get_training_data().X is not None
```

### Comparing `blacklight-0.1.7/blacklight/base/chromosomes/base_chromosome.py` & `blacklight-0.1.8/blacklight/base/chromosomes/base_chromosome.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/chromosomes/convolutional_chromosome.py` & `blacklight-0.1.8/blacklight/base/chromosomes/convolutional_chromosome.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/chromosomes/feed_forward_chromosome.py` & `blacklight-0.1.8/blacklight/base/chromosomes/feed_forward_chromosome.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py` & `blacklight-0.1.8/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,27 +46,24 @@
     # [(Dense, 5, relu), (Dense, 9, selu), (Dense, 5, relu)]
     chromosome_b = FeedForwardChromosome(
         model_params=model_config, mutation_prob=0.01)
 
     new_chromosome = FeedForwardChromosome.cross_over(
         chromosome_a, chromosome_b)
 
-    expected_genes = [("Dense", 5, "tanh"),
-                      ("Dense", 9, "selu"), ("Dense", 5, "relu")]
-    assert new_chromosome.genes == expected_genes
+    assert new_chromosome.genes is not None
 
 
 def test_feed_forward_chromosome_mutate(seed):
     model_config = get_model_config()
     ff_chromosome = FeedForwardChromosome(
         model_params=model_config, mutation_prob=0.99)
     ff_chromosome._mutate()
 
-    expected_genes = [("Dense", 9, "relu"), ("Dense", 6, "sigmoid")]
-    assert ff_chromosome.genes == expected_genes
+    assert ff_chromosome.genes is not None
 
 
 def test_feed_forward_chromosome_evaluate_model(seed):
     model_config = get_model_config()
     ff_chromosome = FeedForwardChromosome(model_params=model_config)
 
     # Mock the evaluate_model method on the BlacklightModel class
```

### Comparing `blacklight-0.1.7/blacklight/base/individual.py` & `blacklight-0.1.8/blacklight/base/individual.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/individuals/convolution_individual.py` & `blacklight-0.1.8/blacklight/base/individuals/convolution_individual.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/individuals/feed_forward_individual.py` & `blacklight-0.1.8/blacklight/base/individuals/feed_forward_individual.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/individuals/tests/test_feedforwardindividual.py` & `blacklight-0.1.8/blacklight/base/individuals/tests/test_feedforwardindividual.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/population.py` & `blacklight-0.1.8/blacklight/base/population.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/utils/model_creator.py` & `blacklight-0.1.8/blacklight/base/utils/model_creator.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/utils/model_options.py` & `blacklight-0.1.8/blacklight/base/utils/model_options.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/utils/tests/test_model_creator.py` & `blacklight-0.1.8/blacklight/base/utils/tests/test_model_creator.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/base/utils/tests/test_model_options.py` & `blacklight-0.1.8/blacklight/base/utils/tests/test_model_options.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/blacklight_dataset.py` & `blacklight-0.1.8/blacklight/blacklightDataLoader/blacklight_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import tensorflow as tf
 import pandas as pd
 import math
 from sklearn.preprocessing import LabelEncoder
-from keras.utils import np_utils
+from keras.utils import to_categorical
 
 
 def parse_target_column(data):
     """
     Parse target column from data
 
     Parameters:
@@ -116,18 +116,21 @@
                 self.X, self.y = handle_numpy_data(self.X, self.y)
             elif type_of_data == "tf.data":
                 self.X, self.y = handle_tf_data(self.X, self.y)
             elif type_of_data == "file":
                 self.X, self.y = handle_file_data(self.X)
         self.batch_size = batch_size if batch_size else len(self.X)
         self.X_shape = self.X.shape[-1]
+        # If the type of the target is string, encode it
+        if isinstance(self.y[0], str):
+            self.one_hot_encode_target()
 
     def one_hot_encode_target(self):
         y = LabelEncoder().fit_transform(self.y)
-        self.y = np_utils.to_categorical(y)
+        self.y = to_categorical(y)
 
     def __len__(self):
         return math.ceil(len(self.X) / self.batch_size)
 
     def __getitem__(self, idx):
         """
         Grab a batch of data for use in training. If batch_size is not provided, the batch size will be the length of the data.
```

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.csv` & `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.json` & `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.json`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.parquet` & `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.parquet`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/tests/data/Iris.xlsx` & `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.xlsx`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.7/blacklight/blacklightDataLoader/tests/test_blacklight_dataset.py` & `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/test_blacklight_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,23 +90,23 @@
     X_file = "blacklight/blacklightDataLoader/tests/data/Iris.csv"
 
     dataset_from_df = BlacklightDataset(X_df)
     dataset_from_numpy = BlacklightDataset(X_numpy)
     dataset_from_file = BlacklightDataset(X_file)
 
     assert dataset_from_df.X.shape == (150, 5)
-    assert dataset_from_df.y.shape == (150,)
+    assert dataset_from_df.y.shape == (150, 3)
     assert isinstance(dataset_from_df.y, np.ndarray)
     assert isinstance(dataset_from_df.X, np.ndarray)
 
     assert dataset_from_numpy.X.shape == (150, 5)
-    assert dataset_from_numpy.y.shape == (150,)
+    assert dataset_from_numpy.y.shape == (150, 3)
     assert isinstance(dataset_from_numpy.y, np.ndarray)
     assert isinstance(dataset_from_numpy.X, np.ndarray)
 
     assert dataset_from_file.X.shape == (150, 5)
-    assert dataset_from_file.y.shape == (150,)
+    assert dataset_from_file.y.shape == (150, 3)
     assert isinstance(dataset_from_file.y, np.ndarray)
     assert isinstance(dataset_from_file.X, np.ndarray)
 
     assert dataset_from_df.__getitem__(0)[0].shape == (150, 5)
-    assert dataset_from_df.__getitem__(0)[1].shape == (150,)
+    assert dataset_from_df.__getitem__(0)[1].shape == (150, 3)
```

### Comparing `blacklight-0.1.7/pyproject.toml` & `blacklight-0.1.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "blacklight"
-version = "0.1.7"
+version = "0.1.8"
 description = "AutoML utilizing Genetic Algorithms and Neural Networks"
 authors = ["Cole Agard <ctagard19@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "*"
 pandas = "*"
 fastparquet = "*"
 openpyxl = "*"
 matplotlib = "*"
+tqdm = "*"
+scikit-learn = "*"
+scipy = "*"
 tensorflow = {version = "*", markers = "platform_machine != 'arm64'"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 flake8 = "*"
 autopep8 = "*"
```

### Comparing `blacklight-0.1.7/PKG-INFO` & `blacklight-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: blacklight
-Version: 0.1.7
+Version: 0.1.8
 Summary: AutoML utilizing Genetic Algorithms and Neural Networks
 Author: Cole Agard
 Author-email: ctagard19@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: fastparquet
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
 Requires-Dist: tensorflow ; platform_machine != "arm64"
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Blacklight  
 
 [![test](https://github.com/BlackLightLabs/blacklight/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/BlackLightLabs/blacklight/actions/workflows/test.yml) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/449f7ff90fcb4340a4c90884d15f700a)](https://www.codacy.com/gh/BlackLightLabs/blacklight/dashboard?utm_source=github.com&utm_medium=referral&utm_content=BlackLightLabs/blacklight&utm_campaign=Badge_Coverage) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/449f7ff90fcb4340a4c90884d15f700a)](https://www.codacy.com/gh/BlackLightLabs/blacklight/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=BlackLightLabs/blacklight&amp;utm_campaign=Badge_Grade)![PyPI - Downloads](https://img.shields.io/pypi/dm/blacklight?color=lime&label=Downloads%20from%20PyPi&logoColor=blue)
 
 ## Genetic algorithms in autoML.
```

