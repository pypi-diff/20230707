# Comparing `tmp/TabularDataInvestigation-0.0.7.tar.gz` & `tmp/TabularDataInvestigation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TabularDataInvestigation-0.0.7.tar", last modified: Sat Jun 17 08:02:02 2023, max compression
+gzip compressed data, was "TabularDataInvestigation-0.0.8.tar", last modified: Fri Jul  7 09:19:50 2023, max compression
```

## Comparing `TabularDataInvestigation-0.0.7.tar` & `TabularDataInvestigation-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.712310 TabularDataInvestigation-0.0.7/
--rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0    14894 2023-06-17 08:02:02.713310 TabularDataInvestigation-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    13979 2023-06-17 08:01:56.000000 TabularDataInvestigation-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.682311 TabularDataInvestigation-0.0.7/TabularDataInvestigation/
--rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation/__init__.py
--rw-rw-rw-   0        0        0     5794 2023-06-17 07:59:46.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation/tdi.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.711316 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/
--rw-rw-rw-   0        0        0    14894 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-17 08:02:02.715311 TabularDataInvestigation-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-06-17 07:59:30.000000 TabularDataInvestigation-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:19:50.025811 TabularDataInvestigation-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-06-16 12:54:49.000000 TabularDataInvestigation-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    15855 2023-07-07 09:19:50.025811 TabularDataInvestigation-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    14917 2023-07-07 09:15:13.000000 TabularDataInvestigation-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 09:19:49.944809 TabularDataInvestigation-0.0.8/TabularDataInvestigation/
+-rw-rw-rw-   0        0        0     6299 2023-06-16 18:26:40.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/TabularDataInvestigation.py
+-rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:19:50.023811 TabularDataInvestigation-0.0.8/TabularDataInvestigation/__pycache__/
+-rw-rw-rw-   0        0        0     4235 2023-06-16 19:00:42.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/__pycache__/TabularDataInvestigation.cpython-310.pyc
+-rw-rw-rw-   0        0        0      165 2023-06-16 18:57:13.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3784 2023-06-17 05:09:53.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/__pycache__/tdi.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5794 2023-06-17 07:59:46.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation/tdi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:19:49.989811 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/
+-rw-rw-rw-   0        0        0    15855 2023-07-07 09:19:49.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-07-07 09:19:49.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:19:49.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 09:19:49.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-07 09:19:49.000000 TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-07 09:19:50.027814 TabularDataInvestigation-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-07 09:17:57.000000 TabularDataInvestigation-0.0.8/setup.py
```

### Comparing `TabularDataInvestigation-0.0.7/LICENSE.txt` & `TabularDataInvestigation-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TabularDataInvestigation-0.0.7/PKG-INFO` & `TabularDataInvestigation-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-Metadata-Version: 2.1
-Name: TabularDataInvestigation
-Version: 0.0.7
-Summary: This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed 
-Home-page: https://github.com/Tanvir223/TabularDataInvestigation
-Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.7.tar.gz
-Author: Tanvir Islam
-Author-email: islamtanvir659@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/Tanvir223/TabularDataInvestigation/issues
-Keywords: pypi,TabularDataInvestigation,TabularData,Data-Manupulation,Data-Preprocessing,Data Cleaning,Machine Learning,Artificial Intelligence,Industry Data,Data Science
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <div class="cell markdown" id="lJNrv9lwHw7t">
 
-**This package provide a fast tabular data investigation and it will
-eligible for ML model building and also helps to developers in their
-projects when needed. Most of the functions return a dataframe or json
-as output**
+## This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed. Most of the functions return a dataframe or json as output
 
 </div>
 
 <div class="cell code" id="HRSU2lZ5Ht9v">
 
 ``` python
 pip install TabularDataInvestigation
 ```
 
 </div>
 
-<div class="cell code" execution_count="43" id="VzC1_y2hTSlb">
+<div class="cell code" id="VzC1_y2hTSlb">
 
 ``` python
 from TabularDataInvestigation import tdi
 ```
 
 </div>
 
 <div class="cell markdown" id="5o29-lUSKmIy">
 
-**tdi.find_index_for_null_values(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe'**
+# tdi.find_index_for_null_values(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe'
+
+</div>
+
+<div class="cell markdown" id="ZxDbq_gbf3fM">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="vYvrNlAvIDQd">
 
-Some we need to delete or fill the null values each cell specifically
-with different methods. some data has meaning and some are unnecceesary.
-so using this function we can get all the missing column indexes that we
-can use in our project.
+Sometimes, we need to drop or fill the null values according to
+individual cell specifically with different methods. Some data contains
+meaning and some are unnecceesary.So, using this function we can get all
+the missing cell indexes that we can use in our project.
 
 </div>
 
-<div class="cell code" execution_count="19"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="TGS5k7JWIqz8" outputId="3663fd25-23cb-4558-a175-5ede1691661d">
 
 ``` python
 df = pd.DataFrame({'A': [1, None, 3], 'B': ['!', 5, '?'], 'C': ['a', 'b', None]})
 df
 ```
@@ -73,15 +62,15 @@
     1  NaN  5     b
     2  3.0  ?  None
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="20"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="HLVms92Zn4qW" outputId="669872b8-bce7-456b-afae-37dca420cc49">
 
 ``` python
 tdi.find_index_for_null_values(df)
 ```
 
@@ -90,15 +79,15 @@
          A    C
     0  [1]  [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="21"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="8_NmdR_UKRWy" outputId="b650a6f9-2f2b-49f8-a3e0-e575a1d74df0">
 
 ``` python
 tdi.find_index_for_null_values(df, return_type='json')
 ```
 
@@ -110,36 +99,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="d9uRAKLzKYDy">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. From the output we understand that column "A" Index "1" has a
+null value.
 
 </div>
 
 <div class="cell markdown" id="OSAs6sHgLVf3">
 
-**tdi.check_error_data_types(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe')**
+# tdi.check_error_data_types(df, return_type='dataframe')
+
+**Parameters(Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe')
+
+</div>
+
+<div class="cell markdown" id="jTm7bE7mgP1k">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="OpKOTMPmLl5w">
 
-We usually face some unusual behave in the dataframe. Sometimes we are
-seeing there is a numeric type column but after checking it shows object
-or string type column. So this function will find the cuase.
+We usually face some unusual behave in the dataframe for data type
+issue. Sometimes we are seeing there is a numeric type column but after
+checking it shows object or string type column for error in the data. So
+this function will find the cuase in the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="25"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WQAv7nOpLktf" outputId="599eb053-4f53-4857-a2a0-52c1c68fc8d3">
 
 ``` python
 df = pd.DataFrame({'A': [1, 'a', 3], 'B': [1, 5, 2], 'C': [1.3, 3.9,'2,0']})
 df
 ```
@@ -151,15 +151,15 @@
     1  a  5  3.9
     2  3  2  2,0
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="26"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:112}"
 id="S8gaMAASbZc4" outputId="0325075a-93e6-4347-bbfc-823e74021772">
 
 ``` python
 tdi.check_error_data_types(df)
 ```
 
@@ -169,15 +169,15 @@
     0       A        [a]         [1]
     1       C      [2,0]         [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="27"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="RcCmVNZAMgkH" outputId="4c6315d7-6fd3-4a87-9ef2-4116f47b4401">
 
 ``` python
 tdi.check_error_data_types(df, return_type='json')
 ```
 
@@ -189,31 +189,41 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="NSjujMp0Mqv1">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column `"A"` have error data value
+`"a"` and which index is `"1"`
 
 </div>
 
 <div class="cell markdown" id="IwI-sfT4MsLG">
 
-**tdi.check_num_of_min_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;minimum_threshold : this define the minimum count of a
-category(Default=3)\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_num_of_min_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   minimum_threshold : this define the minimum count of a
+    category(Default=3)
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="nQZU9yJAhqOg">
+
+**Output : DataFrame**
 
 </div>
 
-<div class="cell code" execution_count="28"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="eM1XHOiOM1Fd" outputId="4b9d38f4-fe36-4b69-e47c-971529b56d69">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'y','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -226,15 +236,15 @@
     2  b  y  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="29"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="EwgrDhQ4C0fj" outputId="7adb6b4a-e039-46f5-9273-93e4299faf54">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1)
 ```
 
@@ -243,15 +253,15 @@
       columns category index
     0       B      [y]   [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="30"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="zNg1D-hZNwhF" outputId="c4f3bef9-1796-499d-927c-ab572ab08c51">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1, return_type='json')
 ```
 
@@ -263,37 +273,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="FpWRMlBINw0M">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" have fewer categories
+because we set the minimum threshold is "1" and which index is "2"
 
 </div>
 
 <div class="cell markdown" id="gXIXp6XBN7NM">
 
-**tdi.check_col_with_one_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_col_with_one_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="5yE89DndjHNl">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="YO1-JmApOFDz">
 
 Sometimes we got such categorical column which data have no variation
 that means all column's data are same. So this function will findout
 those column(s)
 
 </div>
 
-<div class="cell code" execution_count="31"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="GOO1rwMHN6c0" outputId="288a9482-0ac7-437b-f248-67f5021c8753">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'x','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -306,15 +326,15 @@
     2  b  x  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="32"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="R_dXOEClEBKg" outputId="c10cbf14-cb6c-49fc-82a6-e37fdd3c4787">
 
 ``` python
 tdi.check_col_with_one_category(df)
 ```
 
@@ -323,15 +343,15 @@
       columns category_name
     0       B           [x]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="33"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="m2Fz5iqlO9nM" outputId="1cbbf8e0-c640-47bc-ae60-1a16ef866c60">
 
 ``` python
 tdi.check_col_with_one_category(df,return_type='json')
 ```
 
@@ -343,36 +363,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="uR3g6QQIPFRh">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" has one category only
+which category value is "x"
 
 </div>
 
 <div class="cell markdown" id="zal9tBcxPH5B">
 
-**tdi.find_special_char_index(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.find_special_char_index(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="IzRE_G_3jwN1">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="BujDuVwXPRrg">
 
-This function will find out for us those indexes which holding the
+This function will find out for us those indexes which contain the
 double spaces and special characters into the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="34"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WzJTJwX3O9vR" outputId="3f85f568-b4ad-4a2c-a3d2-8fa68a9099e2">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1.2, 2.6, '3,2']})
 df
 ```
@@ -384,15 +414,15 @@
     1  2  5  2.6
     2  3  ?  3,2
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="35"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="OhApZcUnENOd" outputId="934cef2f-027e-44b0-f5e8-574664df530a">
 
 ``` python
 tdi.find_special_char_index(df)
 ```
 
@@ -403,15 +433,15 @@
     1       B              [0, 2]
     2       C                 [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="36"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
 id="BpYx5OUJP6TR" outputId="a4ba4445-0265-4826-a059-b7103b62b763">
 
 ``` python
 tdi.find_special_char_index(df, return_type='json')
 ```
 
@@ -423,34 +453,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="CBfT0D9sP6ho">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output dataframe defines that column "B" have special
+characters which indexes are \[0,2\] and column "C" has also special
+character which index is \[2\]
 
 </div>
 
 <div class="cell markdown" id="78DYtKBjQFDA">
 
-**tdi.duplicate_columns(df)\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe**
+# tdi.duplicate_columns(df)
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+
+</div>
+
+<div class="cell markdown" id="qMMBY5Kuk73j">
+
+**Output : List**
 
 </div>
 
 <div class="cell markdown" id="rKojcLDDQXC4">
 
-This function return a list of column names those containg the same
-value column name may different but data is same
+This function returns a list of column names those containing the same
+value. Also, handle the case that the column name may different but data
+is same
 
 </div>
 
-<div class="cell code" execution_count="37"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="h3KeKIY6Q1Hn" outputId="e6dd6b1d-eade-4120-ce55-ae9a5bc92896">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1, 2, 3]})
 df
 ```
@@ -462,15 +504,15 @@
     1  2  5  2
     2  3  ?  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="38"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
 id="oLt8h-ksEQCf" outputId="93387b3e-d8d1-4df3-8071-4884039a9575">
 
 ``` python
 l = tdi.duplicate_columns(df)
 l
 ```
@@ -487,30 +529,38 @@
 
 So here 'A' and 'C' columns contain the same data
 
 </div>
 
 <div class="cell markdown" id="_tH4YAE-SIKl">
 
-**tdi.correlated_columns(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.correlated_columns(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="HjHMEZB6lNoC">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="9QYFkYRQSQb-">
 
 This function will return a dataframe or json which will define that
-different column but the data is more than 90% correlated
+different column but the data is more than 90% correlated.
 
 </div>
 
-<div class="cell code" execution_count="40"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="qTs0jpchFPHD" outputId="e49b0c80-9db3-478d-d2f0-301cb27b9c75">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['a', 5, 'b'], 'C': [1, 2, 3]})
 df
 ```
@@ -522,15 +572,15 @@
     1  2  5  2
     2  3  b  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="41"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:167}"
 id="zwpXXkFPFAFH" outputId="34fe3c23-24ed-41ea-b0b6-888c1449cd73">
 
 ``` python
 tdi.correlated_columns(df, return_type='dataframe')
 ```
 
@@ -547,15 +597,15 @@
     0       A                [C]       [1.0]
     1       C                [A]       [1.0]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="42"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:107}"
 id="1_5JXsFgFIdg" outputId="cf45f62e-cd6e-4fed-9803-d2a30b4f4f95">
 
 ``` python
 tdi.correlated_columns(df, return_type='json')
 ```
 
@@ -574,12 +624,19 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="AMpvo2RYS92c">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column A is correlated with column
+C and also shows the correlation value
 
 </div>
 
+<div class="cell code" id="6uyQ5pVcS5VG">
 
+``` python
+```
+
+</div>
```

### Comparing `TabularDataInvestigation-0.0.7/README.md` & `TabularDataInvestigation-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,73 @@
+Metadata-Version: 2.1
+Name: TabularDataInvestigation
+Version: 0.0.8
+Summary: This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed 
+Home-page: https://github.com/Tanvir223/TabularDataInvestigation
+Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.8.tar.gz
+Author: Tanvir Islam
+Author-email: islamtanvir659@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/Tanvir223/TabularDataInvestigation/issues
+Keywords: pypi,TabularDataInvestigation,TabularData,Data-Manupulation,Data-Preprocessing,Data Cleaning,Machine Learning,Artificial Intelligence,Industry Data,Data Science
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
+
 <div class="cell markdown" id="lJNrv9lwHw7t">
 
-**This package provide a fast tabular data investigation and it will
-eligible for ML model building and also helps to developers in their
-projects when needed. Most of the functions return a dataframe or json
-as output**
+## This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed. Most of the functions return a dataframe or json as output
 
 </div>
 
 <div class="cell code" id="HRSU2lZ5Ht9v">
 
 ``` python
 pip install TabularDataInvestigation
 ```
 
 </div>
 
-<div class="cell code" execution_count="43" id="VzC1_y2hTSlb">
+<div class="cell code" id="VzC1_y2hTSlb">
 
 ``` python
 from TabularDataInvestigation import tdi
 ```
 
 </div>
 
 <div class="cell markdown" id="5o29-lUSKmIy">
 
-**tdi.find_index_for_null_values(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe'**
+# tdi.find_index_for_null_values(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe'
+
+</div>
+
+<div class="cell markdown" id="ZxDbq_gbf3fM">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="vYvrNlAvIDQd">
 
-Some we need to delete or fill the null values each cell specifically
-with different methods. some data has meaning and some are unnecceesary.
-so using this function we can get all the missing column indexes that we
-can use in our project.
+Sometimes, we need to drop or fill the null values according to
+individual cell specifically with different methods. Some data contains
+meaning and some are unnecceesary.So, using this function we can get all
+the missing cell indexes that we can use in our project.
 
 </div>
 
-<div class="cell code" execution_count="19"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="TGS5k7JWIqz8" outputId="3663fd25-23cb-4558-a175-5ede1691661d">
 
 ``` python
 df = pd.DataFrame({'A': [1, None, 3], 'B': ['!', 5, '?'], 'C': ['a', 'b', None]})
 df
 ```
@@ -57,15 +79,15 @@
     1  NaN  5     b
     2  3.0  ?  None
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="20"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="HLVms92Zn4qW" outputId="669872b8-bce7-456b-afae-37dca420cc49">
 
 ``` python
 tdi.find_index_for_null_values(df)
 ```
 
@@ -74,15 +96,15 @@
          A    C
     0  [1]  [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="21"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="8_NmdR_UKRWy" outputId="b650a6f9-2f2b-49f8-a3e0-e575a1d74df0">
 
 ``` python
 tdi.find_index_for_null_values(df, return_type='json')
 ```
 
@@ -94,36 +116,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="d9uRAKLzKYDy">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. From the output we understand that column "A" Index "1" has a
+null value.
 
 </div>
 
 <div class="cell markdown" id="OSAs6sHgLVf3">
 
-**tdi.check_error_data_types(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe')**
+# tdi.check_error_data_types(df, return_type='dataframe')
+
+**Parameters(Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe')
+
+</div>
+
+<div class="cell markdown" id="jTm7bE7mgP1k">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="OpKOTMPmLl5w">
 
-We usually face some unusual behave in the dataframe. Sometimes we are
-seeing there is a numeric type column but after checking it shows object
-or string type column. So this function will find the cuase.
+We usually face some unusual behave in the dataframe for data type
+issue. Sometimes we are seeing there is a numeric type column but after
+checking it shows object or string type column for error in the data. So
+this function will find the cuase in the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="25"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WQAv7nOpLktf" outputId="599eb053-4f53-4857-a2a0-52c1c68fc8d3">
 
 ``` python
 df = pd.DataFrame({'A': [1, 'a', 3], 'B': [1, 5, 2], 'C': [1.3, 3.9,'2,0']})
 df
 ```
@@ -135,15 +168,15 @@
     1  a  5  3.9
     2  3  2  2,0
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="26"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:112}"
 id="S8gaMAASbZc4" outputId="0325075a-93e6-4347-bbfc-823e74021772">
 
 ``` python
 tdi.check_error_data_types(df)
 ```
 
@@ -153,15 +186,15 @@
     0       A        [a]         [1]
     1       C      [2,0]         [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="27"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="RcCmVNZAMgkH" outputId="4c6315d7-6fd3-4a87-9ef2-4116f47b4401">
 
 ``` python
 tdi.check_error_data_types(df, return_type='json')
 ```
 
@@ -173,31 +206,41 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="NSjujMp0Mqv1">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column `"A"` have error data value
+`"a"` and which index is `"1"`
 
 </div>
 
 <div class="cell markdown" id="IwI-sfT4MsLG">
 
-**tdi.check_num_of_min_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;minimum_threshold : this define the minimum count of a
-category(Default=3)\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_num_of_min_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   minimum_threshold : this define the minimum count of a
+    category(Default=3)
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="nQZU9yJAhqOg">
+
+**Output : DataFrame**
 
 </div>
 
-<div class="cell code" execution_count="28"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="eM1XHOiOM1Fd" outputId="4b9d38f4-fe36-4b69-e47c-971529b56d69">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'y','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -210,15 +253,15 @@
     2  b  y  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="29"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="EwgrDhQ4C0fj" outputId="7adb6b4a-e039-46f5-9273-93e4299faf54">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1)
 ```
 
@@ -227,15 +270,15 @@
       columns category index
     0       B      [y]   [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="30"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="zNg1D-hZNwhF" outputId="c4f3bef9-1796-499d-927c-ab572ab08c51">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1, return_type='json')
 ```
 
@@ -247,37 +290,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="FpWRMlBINw0M">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" have fewer categories
+because we set the minimum threshold is "1" and which index is "2"
 
 </div>
 
 <div class="cell markdown" id="gXIXp6XBN7NM">
 
-**tdi.check_col_with_one_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_col_with_one_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="5yE89DndjHNl">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="YO1-JmApOFDz">
 
 Sometimes we got such categorical column which data have no variation
 that means all column's data are same. So this function will findout
 those column(s)
 
 </div>
 
-<div class="cell code" execution_count="31"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="GOO1rwMHN6c0" outputId="288a9482-0ac7-437b-f248-67f5021c8753">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'x','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -290,15 +343,15 @@
     2  b  x  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="32"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="R_dXOEClEBKg" outputId="c10cbf14-cb6c-49fc-82a6-e37fdd3c4787">
 
 ``` python
 tdi.check_col_with_one_category(df)
 ```
 
@@ -307,15 +360,15 @@
       columns category_name
     0       B           [x]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="33"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="m2Fz5iqlO9nM" outputId="1cbbf8e0-c640-47bc-ae60-1a16ef866c60">
 
 ``` python
 tdi.check_col_with_one_category(df,return_type='json')
 ```
 
@@ -327,36 +380,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="uR3g6QQIPFRh">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" has one category only
+which category value is "x"
 
 </div>
 
 <div class="cell markdown" id="zal9tBcxPH5B">
 
-**tdi.find_special_char_index(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.find_special_char_index(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="IzRE_G_3jwN1">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="BujDuVwXPRrg">
 
-This function will find out for us those indexes which holding the
+This function will find out for us those indexes which contain the
 double spaces and special characters into the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="34"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WzJTJwX3O9vR" outputId="3f85f568-b4ad-4a2c-a3d2-8fa68a9099e2">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1.2, 2.6, '3,2']})
 df
 ```
@@ -368,15 +431,15 @@
     1  2  5  2.6
     2  3  ?  3,2
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="35"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="OhApZcUnENOd" outputId="934cef2f-027e-44b0-f5e8-574664df530a">
 
 ``` python
 tdi.find_special_char_index(df)
 ```
 
@@ -387,15 +450,15 @@
     1       B              [0, 2]
     2       C                 [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="36"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
 id="BpYx5OUJP6TR" outputId="a4ba4445-0265-4826-a059-b7103b62b763">
 
 ``` python
 tdi.find_special_char_index(df, return_type='json')
 ```
 
@@ -407,34 +470,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="CBfT0D9sP6ho">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output dataframe defines that column "B" have special
+characters which indexes are \[0,2\] and column "C" has also special
+character which index is \[2\]
 
 </div>
 
 <div class="cell markdown" id="78DYtKBjQFDA">
 
-**tdi.duplicate_columns(df)\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe**
+# tdi.duplicate_columns(df)
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+
+</div>
+
+<div class="cell markdown" id="qMMBY5Kuk73j">
+
+**Output : List**
 
 </div>
 
 <div class="cell markdown" id="rKojcLDDQXC4">
 
-This function return a list of column names those containg the same
-value column name may different but data is same
+This function returns a list of column names those containing the same
+value. Also, handle the case that the column name may different but data
+is same
 
 </div>
 
-<div class="cell code" execution_count="37"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="h3KeKIY6Q1Hn" outputId="e6dd6b1d-eade-4120-ce55-ae9a5bc92896">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1, 2, 3]})
 df
 ```
@@ -446,15 +521,15 @@
     1  2  5  2
     2  3  ?  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="38"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
 id="oLt8h-ksEQCf" outputId="93387b3e-d8d1-4df3-8071-4884039a9575">
 
 ``` python
 l = tdi.duplicate_columns(df)
 l
 ```
@@ -471,30 +546,38 @@
 
 So here 'A' and 'C' columns contain the same data
 
 </div>
 
 <div class="cell markdown" id="_tH4YAE-SIKl">
 
-**tdi.correlated_columns(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.correlated_columns(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="HjHMEZB6lNoC">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="9QYFkYRQSQb-">
 
 This function will return a dataframe or json which will define that
-different column but the data is more than 90% correlated
+different column but the data is more than 90% correlated.
 
 </div>
 
-<div class="cell code" execution_count="40"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="qTs0jpchFPHD" outputId="e49b0c80-9db3-478d-d2f0-301cb27b9c75">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['a', 5, 'b'], 'C': [1, 2, 3]})
 df
 ```
@@ -506,15 +589,15 @@
     1  2  5  2
     2  3  b  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="41"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:167}"
 id="zwpXXkFPFAFH" outputId="34fe3c23-24ed-41ea-b0b6-888c1449cd73">
 
 ``` python
 tdi.correlated_columns(df, return_type='dataframe')
 ```
 
@@ -531,15 +614,15 @@
     0       A                [C]       [1.0]
     1       C                [A]       [1.0]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="42"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:107}"
 id="1_5JXsFgFIdg" outputId="cf45f62e-cd6e-4fed-9803-d2a30b4f4f95">
 
 ``` python
 tdi.correlated_columns(df, return_type='json')
 ```
 
@@ -558,12 +641,19 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="AMpvo2RYS92c">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column A is correlated with column
+C and also shows the correlation value
 
 </div>
 
+<div class="cell code" id="6uyQ5pVcS5VG">
 
+``` python
+```
+
+</div>
```

### Comparing `TabularDataInvestigation-0.0.7/TabularDataInvestigation/tdi.py` & `TabularDataInvestigation-0.0.8/TabularDataInvestigation/tdi.py`

 * *Files identical despite different names*

### Comparing `TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/PKG-INFO` & `TabularDataInvestigation-0.0.8/TabularDataInvestigation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 Metadata-Version: 2.1
 Name: TabularDataInvestigation
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed 
 Home-page: https://github.com/Tanvir223/TabularDataInvestigation
-Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.8.tar.gz
 Author: Tanvir Islam
 Author-email: islamtanvir659@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Tanvir223/TabularDataInvestigation/issues
 Keywords: pypi,TabularDataInvestigation,TabularData,Data-Manupulation,Data-Preprocessing,Data Cleaning,Machine Learning,Artificial Intelligence,Industry Data,Data Science
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 License-File: LICENSE.txt
 
 <div class="cell markdown" id="lJNrv9lwHw7t">
 
-**This package provide a fast tabular data investigation and it will
-eligible for ML model building and also helps to developers in their
-projects when needed. Most of the functions return a dataframe or json
-as output**
+## This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed. Most of the functions return a dataframe or json as output
 
 </div>
 
 <div class="cell code" id="HRSU2lZ5Ht9v">
 
 ``` python
 pip install TabularDataInvestigation
 ```
 
 </div>
 
-<div class="cell code" execution_count="43" id="VzC1_y2hTSlb">
+<div class="cell code" id="VzC1_y2hTSlb">
 
 ``` python
 from TabularDataInvestigation import tdi
 ```
 
 </div>
 
 <div class="cell markdown" id="5o29-lUSKmIy">
 
-**tdi.find_index_for_null_values(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe'**
+# tdi.find_index_for_null_values(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe'
+
+</div>
+
+<div class="cell markdown" id="ZxDbq_gbf3fM">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="vYvrNlAvIDQd">
 
-Some we need to delete or fill the null values each cell specifically
-with different methods. some data has meaning and some are unnecceesary.
-so using this function we can get all the missing column indexes that we
-can use in our project.
+Sometimes, we need to drop or fill the null values according to
+individual cell specifically with different methods. Some data contains
+meaning and some are unnecceesary.So, using this function we can get all
+the missing cell indexes that we can use in our project.
 
 </div>
 
-<div class="cell code" execution_count="19"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="TGS5k7JWIqz8" outputId="3663fd25-23cb-4558-a175-5ede1691661d">
 
 ``` python
 df = pd.DataFrame({'A': [1, None, 3], 'B': ['!', 5, '?'], 'C': ['a', 'b', None]})
 df
 ```
@@ -73,15 +79,15 @@
     1  NaN  5     b
     2  3.0  ?  None
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="20"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="HLVms92Zn4qW" outputId="669872b8-bce7-456b-afae-37dca420cc49">
 
 ``` python
 tdi.find_index_for_null_values(df)
 ```
 
@@ -90,15 +96,15 @@
          A    C
     0  [1]  [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="21"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="8_NmdR_UKRWy" outputId="b650a6f9-2f2b-49f8-a3e0-e575a1d74df0">
 
 ``` python
 tdi.find_index_for_null_values(df, return_type='json')
 ```
 
@@ -110,36 +116,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="d9uRAKLzKYDy">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. From the output we understand that column "A" Index "1" has a
+null value.
 
 </div>
 
 <div class="cell markdown" id="OSAs6sHgLVf3">
 
-**tdi.check_error_data_types(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional): Default = 'dataframe')**
+# tdi.check_error_data_types(df, return_type='dataframe')
+
+**Parameters(Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional): Default = 'dataframe')
+
+</div>
+
+<div class="cell markdown" id="jTm7bE7mgP1k">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="OpKOTMPmLl5w">
 
-We usually face some unusual behave in the dataframe. Sometimes we are
-seeing there is a numeric type column but after checking it shows object
-or string type column. So this function will find the cuase.
+We usually face some unusual behave in the dataframe for data type
+issue. Sometimes we are seeing there is a numeric type column but after
+checking it shows object or string type column for error in the data. So
+this function will find the cuase in the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="25"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WQAv7nOpLktf" outputId="599eb053-4f53-4857-a2a0-52c1c68fc8d3">
 
 ``` python
 df = pd.DataFrame({'A': [1, 'a', 3], 'B': [1, 5, 2], 'C': [1.3, 3.9,'2,0']})
 df
 ```
@@ -151,15 +168,15 @@
     1  a  5  3.9
     2  3  2  2,0
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="26"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:112}"
 id="S8gaMAASbZc4" outputId="0325075a-93e6-4347-bbfc-823e74021772">
 
 ``` python
 tdi.check_error_data_types(df)
 ```
 
@@ -169,15 +186,15 @@
     0       A        [a]         [1]
     1       C      [2,0]         [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="27"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="RcCmVNZAMgkH" outputId="4c6315d7-6fd3-4a87-9ef2-4116f47b4401">
 
 ``` python
 tdi.check_error_data_types(df, return_type='json')
 ```
 
@@ -189,31 +206,41 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="NSjujMp0Mqv1">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column `"A"` have error data value
+`"a"` and which index is `"1"`
 
 </div>
 
 <div class="cell markdown" id="IwI-sfT4MsLG">
 
-**tdi.check_num_of_min_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;minimum_threshold : this define the minimum count of a
-category(Default=3)\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_num_of_min_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   minimum_threshold : this define the minimum count of a
+    category(Default=3)
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="nQZU9yJAhqOg">
+
+**Output : DataFrame**
 
 </div>
 
-<div class="cell code" execution_count="28"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="eM1XHOiOM1Fd" outputId="4b9d38f4-fe36-4b69-e47c-971529b56d69">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'y','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -226,15 +253,15 @@
     2  b  y  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="29"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="EwgrDhQ4C0fj" outputId="7adb6b4a-e039-46f5-9273-93e4299faf54">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1)
 ```
 
@@ -243,15 +270,15 @@
       columns category index
     0       B      [y]   [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="30"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="zNg1D-hZNwhF" outputId="c4f3bef9-1796-499d-927c-ab572ab08c51">
 
 ``` python
 tdi.check_num_of_min_category(df, minimum_threshold=1, return_type='json')
 ```
 
@@ -263,37 +290,47 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="FpWRMlBINw0M">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" have fewer categories
+because we set the minimum threshold is "1" and which index is "2"
 
 </div>
 
 <div class="cell markdown" id="gXIXp6XBN7NM">
 
-**tdi.check_col_with_one_category(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.check_col_with_one_category(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="5yE89DndjHNl">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="YO1-JmApOFDz">
 
 Sometimes we got such categorical column which data have no variation
 that means all column's data are same. So this function will findout
 those column(s)
 
 </div>
 
-<div class="cell code" execution_count="31"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:175}"
 id="GOO1rwMHN6c0" outputId="288a9482-0ac7-437b-f248-67f5021c8753">
 
 ``` python
 df = pd.DataFrame({'A': ['b', 'a', 'b','a'], 'B': ['x', 'x', 'x','x'], 'C': ['p', 'p', 'q','q']})
 df
 ```
@@ -306,15 +343,15 @@
     2  b  x  q
     3  a  x  q
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="32"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:81}"
 id="R_dXOEClEBKg" outputId="c10cbf14-cb6c-49fc-82a6-e37fdd3c4787">
 
 ``` python
 tdi.check_col_with_one_category(df)
 ```
 
@@ -323,15 +360,15 @@
       columns category_name
     0       B           [x]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="33"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:35}"
 id="m2Fz5iqlO9nM" outputId="1cbbf8e0-c640-47bc-ae60-1a16ef866c60">
 
 ``` python
 tdi.check_col_with_one_category(df,return_type='json')
 ```
 
@@ -343,36 +380,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="uR3g6QQIPFRh">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column "B" has one category only
+which category value is "x"
 
 </div>
 
 <div class="cell markdown" id="zal9tBcxPH5B">
 
-**tdi.find_special_char_index(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.find_special_char_index(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="IzRE_G_3jwN1">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="BujDuVwXPRrg">
 
-This function will find out for us those indexes which holding the
+This function will find out for us those indexes which contain the
 double spaces and special characters into the dataframe.
 
 </div>
 
-<div class="cell code" execution_count="34"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="WzJTJwX3O9vR" outputId="3f85f568-b4ad-4a2c-a3d2-8fa68a9099e2">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1.2, 2.6, '3,2']})
 df
 ```
@@ -384,15 +431,15 @@
     1  2  5  2.6
     2  3  ?  3,2
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="35"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="OhApZcUnENOd" outputId="934cef2f-027e-44b0-f5e8-574664df530a">
 
 ``` python
 tdi.find_special_char_index(df)
 ```
 
@@ -403,15 +450,15 @@
     1       B              [0, 2]
     2       C                 [2]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="36"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
 id="BpYx5OUJP6TR" outputId="a4ba4445-0265-4826-a059-b7103b62b763">
 
 ``` python
 tdi.find_special_char_index(df, return_type='json')
 ```
 
@@ -423,34 +470,46 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="CBfT0D9sP6ho">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output dataframe defines that column "B" have special
+characters which indexes are \[0,2\] and column "C" has also special
+character which index is \[2\]
 
 </div>
 
 <div class="cell markdown" id="78DYtKBjQFDA">
 
-**tdi.duplicate_columns(df)\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe**
+# tdi.duplicate_columns(df)
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+
+</div>
+
+<div class="cell markdown" id="qMMBY5Kuk73j">
+
+**Output : List**
 
 </div>
 
 <div class="cell markdown" id="rKojcLDDQXC4">
 
-This function return a list of column names those containg the same
-value column name may different but data is same
+This function returns a list of column names those containing the same
+value. Also, handle the case that the column name may different but data
+is same
 
 </div>
 
-<div class="cell code" execution_count="37"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="h3KeKIY6Q1Hn" outputId="e6dd6b1d-eade-4120-ce55-ae9a5bc92896">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['!', 5, '?'], 'C': [1, 2, 3]})
 df
 ```
@@ -462,15 +521,15 @@
     1  2  5  2
     2  3  ?  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="38"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
 id="oLt8h-ksEQCf" outputId="93387b3e-d8d1-4df3-8071-4884039a9575">
 
 ``` python
 l = tdi.duplicate_columns(df)
 l
 ```
@@ -487,30 +546,38 @@
 
 So here 'A' and 'C' columns contain the same data
 
 </div>
 
 <div class="cell markdown" id="_tH4YAE-SIKl">
 
-**tdi.correlated_columns(df, return_type='dataframe')\
-&nbsp;Parameters:\
-&nbsp;&nbsp;df: pandas Dataframe\
-&nbsp;&nbsp;return_type(optional):how want to get the output (Default =
-'dataframe')**
+# tdi.correlated_columns(df, return_type='dataframe')
+
+**Parameters (Input):**
+
+-   df: pandas Dataframe
+-   return_type(optional):how want to get the output (Default =
+    'dataframe')
+
+</div>
+
+<div class="cell markdown" id="HjHMEZB6lNoC">
+
+**Output : DataFrame**
 
 </div>
 
 <div class="cell markdown" id="9QYFkYRQSQb-">
 
 This function will return a dataframe or json which will define that
-different column but the data is more than 90% correlated
+different column but the data is more than 90% correlated.
 
 </div>
 
-<div class="cell code" execution_count="40"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
 id="qTs0jpchFPHD" outputId="e49b0c80-9db3-478d-d2f0-301cb27b9c75">
 
 ``` python
 df = pd.DataFrame({'A': [1, 2, 3], 'B': ['a', 5, 'b'], 'C': [1, 2, 3]})
 df
 ```
@@ -522,15 +589,15 @@
     1  2  5  2
     2  3  b  3
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="41"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:167}"
 id="zwpXXkFPFAFH" outputId="34fe3c23-24ed-41ea-b0b6-888c1449cd73">
 
 ``` python
 tdi.correlated_columns(df, return_type='dataframe')
 ```
 
@@ -547,15 +614,15 @@
     0       A                [C]       [1.0]
     1       C                [A]       [1.0]
 
 </div>
 
 </div>
 
-<div class="cell code" execution_count="42"
+<div class="cell code"
 colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:107}"
 id="1_5JXsFgFIdg" outputId="cf45f62e-cd6e-4fed-9803-d2a30b4f4f95">
 
 ``` python
 tdi.correlated_columns(df, return_type='json')
 ```
 
@@ -574,12 +641,19 @@
 
 </div>
 
 </div>
 
 <div class="cell markdown" id="AMpvo2RYS92c">
 
-Here return type is optional ('dataframe' or 'json'). Default: dataframe
+Here return type is optional ('dataframe' or 'json'). Default:
+dataframe. Above output defines that column A is correlated with column
+C and also shows the correlation value
 
 </div>
 
+<div class="cell code" id="6uyQ5pVcS5VG">
 
+``` python
+```
+
+</div>
```

### Comparing `TabularDataInvestigation-0.0.7/setup.py` & `TabularDataInvestigation-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='TabularDataInvestigation',
     packages=['TabularDataInvestigation'],
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     description='This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tanvir Islam',
     author_email='islamtanvir659@gmail.com',
     url='https://github.com/Tanvir223/TabularDataInvestigation',
     project_urls = {
         "Bug Tracker": "https://github.com/Tanvir223/TabularDataInvestigation/issues"
     },
     install_requires=['requests'],
 
-    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.7.tar.gz",
+    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.8.tar.gz",
     keywords=["pypi", "TabularDataInvestigation", "TabularData", "Data-Manupulation", "Data-Preprocessing", "Data Cleaning","Machine Learning", "Artificial Intelligence", "Industry Data" , "Data Science"],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10'
     ]
 )
```

