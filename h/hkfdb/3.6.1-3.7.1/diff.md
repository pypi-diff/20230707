# Comparing `tmp/hkfdb-3.6.1.tar.gz` & `tmp/hkfdb-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.6.1.tar", last modified: Wed Jul  5 09:03:40 2023, max compression
+gzip compressed data, was "hkfdb-3.7.1.tar", last modified: Thu Jul  6 23:12:22 2023, max compression
```

## Comparing `hkfdb-3.6.1.tar` & `hkfdb-3.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.199053 hkfdb-3.6.1/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.6.1/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-05 09:03:40.198657 hkfdb-3.6.1/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.6.1/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.197147 hkfdb-3.6.1/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   107552 2023-07-05 09:01:07.000000 hkfdb-3.6.1/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.6.1/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.198377 hkfdb-3.6.1/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-05 09:03:40.199150 hkfdb-3.6.1/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-05 09:02:13.000000 hkfdb-3.6.1/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-06 23:12:22.956782 hkfdb-3.7.1/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.1/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-06 23:12:22.956607 hkfdb-3.7.1/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.1/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-06 23:12:22.955376 hkfdb-3.7.1/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   108180 2023-07-06 23:10:44.000000 hkfdb-3.7.1/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.1/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-06 23:12:22.956400 hkfdb-3.7.1/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-06 23:12:22.000000 hkfdb-3.7.1/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-06 23:12:22.000000 hkfdb-3.7.1/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-06 23:12:22.000000 hkfdb-3.7.1/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-06 23:12:22.000000 hkfdb-3.7.1/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-06 23:12:22.000000 hkfdb-3.7.1/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-06 23:12:22.956832 hkfdb-3.7.1/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-06 23:11:31.000000 hkfdb-3.7.1/setup.py
```

### Comparing `hkfdb-3.6.1/LICENSE` & `hkfdb-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.6.1/PKG-INFO` & `hkfdb-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.6.1
+Version: 3.7.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.6.1/README.md` & `hkfdb-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.6.1/hkfdb/Database.py` & `hkfdb-3.7.1/hkfdb/Database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 import requests
 import pandas as pd
 import json
 import ast
 import datetime
-import calendar
 from dateutil.relativedelta import relativedelta, FR
 from bs4 import BeautifulSoup
 
 
 class Database:
 
     def __init__(self,authToken):
@@ -269,15 +268,15 @@
         rolling_time = self.rolling_time
         roll_diff = self.roll_diff
         if row.current_month_expiry_date_diff == rolling_day and row.time == rolling_time:
             return roll_diff
         else:
             return 0
 
-    def get_hk_futures_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
+    def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
 
         check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
 
         self.rolling_day = rolling_day
         self.rolling_time = rolling_time
 
 
@@ -493,266 +492,266 @@
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
 
-    def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
-
-        check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
-
-        if False not in list(check_bool_dict.values()):
-
-            if freq == '1D':
-                rolling_time = 0
-                if rth_only == True:
-                    freq = freq + '_rth'
-                elif rth_only == False:
-                    freq = freq + '_all'
-
-            start_date_dt = datetime.datetime.strptime(str(start_date), '%Y%m%d').date()
-            end_date_dt = datetime.datetime.strptime(str(end_date), '%Y%m%d').date()
-
-            if start_date_dt.month > 1:
-                start_date_year = start_date_dt.year
-            else:
-                start_date_year = start_date_dt.year - 1
-                start_date_dt = start_date_dt - relativedelta(months=1)
-
-            end_date_year = end_date_dt.year if end_date_dt.month < 11 else end_date_dt.year + 1
-
-            holiday_dict = get_hk_holiday_and_expiry_date(start_date_year, end_date_year, 'datetime')
-            expiry_date_list = holiday_dict['expiry_date']
-
-            expiry_date_dict = {}
-            for expiry_date in expiry_date_list:
-                expiry_year_month_str = str(expiry_date.year - 2000) + str(expiry_date.month).zfill(2)
-                expiry_date_dict[expiry_year_month_str] = expiry_date
-
-            day_diff = (end_date_dt - start_date_dt).days
-
-            year_month_involved_list = []
-            for i in range(day_diff + 1):
-                i_date = start_date_dt + datetime.timedelta(days=i)
-                year_month = i_date.strftime('%y%m')
-                expiry_date = expiry_date_dict[year_month]
-                if i_date > expiry_date:
-                    year_month = (i_date + relativedelta(months=1)).strftime('%y%m')
-                if year_month not in year_month_involved_list:
-                    year_month_involved_list.append(year_month)
-
-            year_month_involved_list.append(
-                (datetime.datetime.strptime(year_month_involved_list[-1], '%y%m') + relativedelta(months=1)).strftime(
-                    '%y%m'))
-            year_month_involved_list_str = json.dumps(str(year_month_involved_list))
-
-            year_month_involved_list_str = year_month_involved_list_str.replace('[', '')
-            year_month_involved_list_str = year_month_involved_list_str.replace(']', '')
-            year_month_involved_list_str = year_month_involved_list_str.replace('\'', '')
-            year_month_involved_list_str = year_month_involved_list_str.replace(',', '')
-            year_month_involved_list_str = year_month_involved_list_str.replace(' ', '_')
-            year_month_involved_list_str = year_month_involved_list_str.replace('\"', '')
-
-            link_url = 'http://www.hkfdb.net/data_api?'
-            token_str = 'token=' + str(self.authToken)
-            database_str = 'database=' + 'hk_fut_ohlc'
-            index_str = 'index=' + index
-            freq_str = 'freq=' + freq
-            start_date_str = 'start_date=' + str(start_date)
-            end_date_str = 'end_date=' + str(end_date)
-            rolling_day_str = 'rolling_day=' + str(rolling_day)
-            rolling_time_str = 'rolling_time=' + str(rolling_time)
-            year_month_involved_list_str = 'year_month_involved_list=' + year_month_involved_list_str
-            link_str = link_url + index_str + '&' + freq_str + '&' + rolling_day_str + '&' + rolling_time_str + \
-                       '&' + year_month_involved_list_str + '&' \
-                       + token_str + '&' + database_str + '&' \
-                       + start_date_str + '&' + end_date_str
-
-            response = requests.get(link_str)
-            response_ok = response_check(response)
-            if response_ok == True:
-
-                result_list = json.loads(json.loads(response.content).replace("'", "\""))
-
-                df_list = []
-                date_time_list_list = []
-                date_time_intersect_list = []
-                for result in result_list:
-                    sub_df_list = []
-                    for item in result:
-                        df = pd.DataFrame(item['content'])
-                        if len(df) > 0:
-                            sub_df_list.append(df)
-
-                    if len(sub_df_list) > 0:
-                        df = pd.concat(sub_df_list)
-                        df = df.reset_index(drop=True)
-                        temp_date_list = list(df['date'].unique())
-                        temp_date_list.sort()
-
-                        date_list = []
-                        for temp_date in temp_date_list:
-                            if datetime.datetime.strptime(str(temp_date), '%Y%m%d').weekday() < 5:
-                                date_list.append(temp_date)
-
-                        front_year_month = str(date_list[0])[2:6]
-                        back_year_month = str(date_list[-1])[2:6]
-                        front_expiry_date = int(expiry_date_dict[front_year_month].strftime('%Y%m%d'))
-                        back_expiry_date = int(expiry_date_dict[back_year_month].strftime('%Y%m%d'))
-                        for i in range(len(date_list)):
-                            date_item = date_list[i]
-
-                            if i + rolling_day <= len(date_list) - 1:
-                                if date_list[i + rolling_day] == front_expiry_date:
-                                    front_cut_off_date = date_item
-                                elif date_list[i + rolling_day] == back_expiry_date:
-                                    back_cut_off_date = date_item
-                                    break
-                            else:
-                                back_cut_off_date = max(date_list)
-
-                        if df.loc[0, 'expiry_date'] == '20130530':
-                            front_cut_off_date = 20130501
-
-                        if (back_cut_off_date != end_date) or (
-                                back_cut_off_date == end_date and back_cut_off_date not in expiry_date_list):
-                            if '1D' not in freq:
-                                df_front = df[(df['date'] == front_cut_off_date) & (df['time'] == rolling_time)]
-                                df_back  = df[(df['date'] == back_cut_off_date) & (df['time'] == rolling_time)]
-
-                                df = df[(df['date'] > front_cut_off_date) | (
-                                            (df['date'] == front_cut_off_date) & (df['time'] > rolling_time))]
-                                df = df[(df['date'] < back_cut_off_date) | (
-                                            (df['date'] == back_cut_off_date) & (df['time'] < rolling_time))]
-
-                                df = pd.concat([df, df_front, df_back])
-
-                            else:
-                                df = df[(df['date'] > front_cut_off_date) | (df['date'] == front_cut_off_date)]
-                                df = df[(df['date'] < back_cut_off_date) | (df['date'] == back_cut_off_date)]
-
-                        df = df[df['date'] >= start_date]
-                        df = df[df['date'] <= end_date]
-                        df['date'] = df['date'].astype(str)
-                        if '1D' not in freq:
-                            df['time'] = df['time'].astype(str)
-                            df['time'] = df['time'].str.zfill(6)
-                            df['datetime'] = df['date'] + ' ' + df['time']
-                        else:
-                            df['datetime'] = df['date']
-
-                        df = df.reset_index(drop=True)
-                        date_time_list = df['datetime'].to_list()
-
-                        df = df.sort_values(by='datetime')
-
-                        if '1D' not in freq:
-                            # if len(date_time_list_list) > 0:
-                            #     date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
-                            #     if len(date_time_intersect) == 0:
-                            #         df_list.append(df)
-                            # else:
-                            #     df_list.append(df)
-                            df_list.append(df)
-
-                        else:
-                            date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
-                            date_time_intersect = list(date_time_intersect)
-                            if len(date_time_intersect) > 0:
-                                date_time_intersect_list.append(date_time_intersect[0])
-                            df_list.append(df)
-
-                        date_time_list_list += date_time_list
-
-                df = pd.concat(df_list)
-
-                if '1D' not in freq:
-                    cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date', 'RTH']
-
-                else:
-                    cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date']
-                    df['time'] = 0
-
-                if '1D' not in freq:
-                    df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d %H%M%S')
-                    df['RTH'] = df['RTH'].astype(bool)
-                else:
-                    df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d')
-
-                df = df[cols]
-                df['roll_diff'] = 0
-
-                if '1D' in freq:
-                    drop_index_list = []
-                    df = df.reset_index()
-                    for date_time_intersect in date_time_intersect_list:
-                        check_drop_index_row = df[df['date'] == date_time_intersect]
-                        if len(check_drop_index_row) > 1:
-                            index_0 = check_drop_index_row.index[0]
-                            index_1 = check_drop_index_row.index[1]
-                            expiry_date_0 = df.loc[index_0, 'expiry_date']
-                            expiry_date_1 = df.loc[index_1, 'expiry_date']
-                            close_price_0 = df.loc[index_0, 'close']
-                            close_price_1 = df.loc[index_1, 'close']
-                            if expiry_date_0 > expiry_date_1:
-                                drop_index_list.append(index_1)
-                                roll_diff = close_price_0 - close_price_1
-                                df.at[index_0,'roll_diff'] = roll_diff
-                            elif expiry_date_0 < expiry_date_1:
-                                drop_index_list.append(index_0)
-                                roll_diff = close_price_1 - close_price_0
-                                roll_diff = close_price_0 - close_price_1
-                                df.at[index_1,'roll_diff'] = roll_diff
-                    if len(drop_index_list) > 0:
-                        df = df.drop(drop_index_list, axis=0)
-                    df = df.drop('index', axis=1)
-
-                else:
-                    df = df.reset_index()
-
-                    duplicates = df[df.duplicated(subset=['datetime'], keep=False)]
-                    min_expiry_row_index_list = []
-
-                    for dt in duplicates['datetime'].unique():
-                        df2 = duplicates[duplicates['datetime'] == dt]
-                        min_expiry = df2['expiry_date'].min()
-                        max_expiry = df2['expiry_date'].max()
-                        min_expiry_row = df2.loc[df2['expiry_date'] == min_expiry]
-                        max_expiry_row = df2.loc[df2['expiry_date'] == max_expiry]
-                        min_expiry_row_index = min_expiry_row.index[0]
-                        max_expiry_row_index  = max_expiry_row.index[0]
-                        min_expiry_close = min_expiry_row['close'].values[0]
-                        max_expiry_close = max_expiry_row['close'].values[0]
-
-                        roll_diff = min_expiry_close - max_expiry_close
-
-                        min_expiry_row_index_list.append(min_expiry_row_index)
-                        df.at[max_expiry_row_index, 'roll_diff'] = roll_diff
-
-                    if len(min_expiry_row_index_list) > 0:
-                        df = df.drop(min_expiry_row_index_list, axis=0)
-                    df = df.drop('index', axis=1)
-
-                df = df.set_index(keys='datetime')
-                df = df.sort_index(ascending=True)
-
-                if '1D' not in freq and rth_only == True:
-                    df = df[df['RTH'] == True]
-
-                #df = df.drop_duplicates(keep='first')
-
-                return df
-
-        else:
-            err_msg = 'Error in: '
-            for error in check_bool_dict:
-                if check_bool_dict[error] == False:
-                    err_msg += error + ','
-            print(err_msg)
+    # def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
+    #
+    #     check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
+    #
+    #     if False not in list(check_bool_dict.values()):
+    #
+    #         if freq == '1D':
+    #             rolling_time = 0
+    #             if rth_only == True:
+    #                 freq = freq + '_rth'
+    #             elif rth_only == False:
+    #                 freq = freq + '_all'
+    #
+    #         start_date_dt = datetime.datetime.strptime(str(start_date), '%Y%m%d').date()
+    #         end_date_dt = datetime.datetime.strptime(str(end_date), '%Y%m%d').date()
+    #
+    #         if start_date_dt.month > 1:
+    #             start_date_year = start_date_dt.year
+    #         else:
+    #             start_date_year = start_date_dt.year - 1
+    #             start_date_dt = start_date_dt - relativedelta(months=1)
+    #
+    #         end_date_year = end_date_dt.year if end_date_dt.month < 11 else end_date_dt.year + 1
+    #
+    #         holiday_dict = get_hk_holiday_and_expiry_date(start_date_year, end_date_year, 'datetime')
+    #         expiry_date_list = holiday_dict['expiry_date']
+    #
+    #         expiry_date_dict = {}
+    #         for expiry_date in expiry_date_list:
+    #             expiry_year_month_str = str(expiry_date.year - 2000) + str(expiry_date.month).zfill(2)
+    #             expiry_date_dict[expiry_year_month_str] = expiry_date
+    #
+    #         day_diff = (end_date_dt - start_date_dt).days
+    #
+    #         year_month_involved_list = []
+    #         for i in range(day_diff + 1):
+    #             i_date = start_date_dt + datetime.timedelta(days=i)
+    #             year_month = i_date.strftime('%y%m')
+    #             expiry_date = expiry_date_dict[year_month]
+    #             if i_date > expiry_date:
+    #                 year_month = (i_date + relativedelta(months=1)).strftime('%y%m')
+    #             if year_month not in year_month_involved_list:
+    #                 year_month_involved_list.append(year_month)
+    #
+    #         year_month_involved_list.append(
+    #             (datetime.datetime.strptime(year_month_involved_list[-1], '%y%m') + relativedelta(months=1)).strftime(
+    #                 '%y%m'))
+    #         year_month_involved_list_str = json.dumps(str(year_month_involved_list))
+    #
+    #         year_month_involved_list_str = year_month_involved_list_str.replace('[', '')
+    #         year_month_involved_list_str = year_month_involved_list_str.replace(']', '')
+    #         year_month_involved_list_str = year_month_involved_list_str.replace('\'', '')
+    #         year_month_involved_list_str = year_month_involved_list_str.replace(',', '')
+    #         year_month_involved_list_str = year_month_involved_list_str.replace(' ', '_')
+    #         year_month_involved_list_str = year_month_involved_list_str.replace('\"', '')
+    #
+    #         link_url = 'http://www.hkfdb.net/data_api?'
+    #         token_str = 'token=' + str(self.authToken)
+    #         database_str = 'database=' + 'hk_fut_ohlc'
+    #         index_str = 'index=' + index
+    #         freq_str = 'freq=' + freq
+    #         start_date_str = 'start_date=' + str(start_date)
+    #         end_date_str = 'end_date=' + str(end_date)
+    #         rolling_day_str = 'rolling_day=' + str(rolling_day)
+    #         rolling_time_str = 'rolling_time=' + str(rolling_time)
+    #         year_month_involved_list_str = 'year_month_involved_list=' + year_month_involved_list_str
+    #         link_str = link_url + index_str + '&' + freq_str + '&' + rolling_day_str + '&' + rolling_time_str + \
+    #                    '&' + year_month_involved_list_str + '&' \
+    #                    + token_str + '&' + database_str + '&' \
+    #                    + start_date_str + '&' + end_date_str
+    #
+    #         response = requests.get(link_str)
+    #         response_ok = response_check(response)
+    #         if response_ok == True:
+    #
+    #             result_list = json.loads(json.loads(response.content).replace("'", "\""))
+    #
+    #             df_list = []
+    #             date_time_list_list = []
+    #             date_time_intersect_list = []
+    #             for result in result_list:
+    #                 sub_df_list = []
+    #                 for item in result:
+    #                     df = pd.DataFrame(item['content'])
+    #                     if len(df) > 0:
+    #                         sub_df_list.append(df)
+    #
+    #                 if len(sub_df_list) > 0:
+    #                     df = pd.concat(sub_df_list)
+    #                     df = df.reset_index(drop=True)
+    #                     temp_date_list = list(df['date'].unique())
+    #                     temp_date_list.sort()
+    #
+    #                     date_list = []
+    #                     for temp_date in temp_date_list:
+    #                         if datetime.datetime.strptime(str(temp_date), '%Y%m%d').weekday() < 5:
+    #                             date_list.append(temp_date)
+    #
+    #                     front_year_month = str(date_list[0])[2:6]
+    #                     back_year_month = str(date_list[-1])[2:6]
+    #                     front_expiry_date = int(expiry_date_dict[front_year_month].strftime('%Y%m%d'))
+    #                     back_expiry_date = int(expiry_date_dict[back_year_month].strftime('%Y%m%d'))
+    #                     for i in range(len(date_list)):
+    #                         date_item = date_list[i]
+    #
+    #                         if i + rolling_day <= len(date_list) - 1:
+    #                             if date_list[i + rolling_day] == front_expiry_date:
+    #                                 front_cut_off_date = date_item
+    #                             elif date_list[i + rolling_day] == back_expiry_date:
+    #                                 back_cut_off_date = date_item
+    #                                 break
+    #                         else:
+    #                             back_cut_off_date = max(date_list)
+    #
+    #                     if df.loc[0, 'expiry_date'] == '20130530':
+    #                         front_cut_off_date = 20130501
+    #
+    #                     if (back_cut_off_date != end_date) or (
+    #                             back_cut_off_date == end_date and back_cut_off_date not in expiry_date_list):
+    #                         if '1D' not in freq:
+    #                             df_front = df[(df['date'] == front_cut_off_date) & (df['time'] == rolling_time)]
+    #                             df_back  = df[(df['date'] == back_cut_off_date) & (df['time'] == rolling_time)]
+    #
+    #                             df = df[(df['date'] > front_cut_off_date) | (
+    #                                         (df['date'] == front_cut_off_date) & (df['time'] > rolling_time))]
+    #                             df = df[(df['date'] < back_cut_off_date) | (
+    #                                         (df['date'] == back_cut_off_date) & (df['time'] < rolling_time))]
+    #
+    #                             df = pd.concat([df, df_front, df_back])
+    #
+    #                         else:
+    #                             df = df[(df['date'] > front_cut_off_date) | (df['date'] == front_cut_off_date)]
+    #                             df = df[(df['date'] < back_cut_off_date) | (df['date'] == back_cut_off_date)]
+    #
+    #                     df = df[df['date'] >= start_date]
+    #                     df = df[df['date'] <= end_date]
+    #                     df['date'] = df['date'].astype(str)
+    #                     if '1D' not in freq:
+    #                         df['time'] = df['time'].astype(str)
+    #                         df['time'] = df['time'].str.zfill(6)
+    #                         df['datetime'] = df['date'] + ' ' + df['time']
+    #                     else:
+    #                         df['datetime'] = df['date']
+    #
+    #                     df = df.reset_index(drop=True)
+    #                     date_time_list = df['datetime'].to_list()
+    #
+    #                     df = df.sort_values(by='datetime')
+    #
+    #                     if '1D' not in freq:
+    #                         # if len(date_time_list_list) > 0:
+    #                         #     date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
+    #                         #     if len(date_time_intersect) == 0:
+    #                         #         df_list.append(df)
+    #                         # else:
+    #                         #     df_list.append(df)
+    #                         df_list.append(df)
+    #
+    #                     else:
+    #                         date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
+    #                         date_time_intersect = list(date_time_intersect)
+    #                         if len(date_time_intersect) > 0:
+    #                             date_time_intersect_list.append(date_time_intersect[0])
+    #                         df_list.append(df)
+    #
+    #                     date_time_list_list += date_time_list
+    #
+    #             df = pd.concat(df_list)
+    #
+    #             if '1D' not in freq:
+    #                 cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date', 'RTH']
+    #
+    #             else:
+    #                 cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date']
+    #                 df['time'] = 0
+    #
+    #             if '1D' not in freq:
+    #                 df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d %H%M%S')
+    #                 df['RTH'] = df['RTH'].astype(bool)
+    #             else:
+    #                 df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d')
+    #
+    #             df = df[cols]
+    #             df['roll_diff'] = 0
+    #
+    #             if '1D' in freq:
+    #                 drop_index_list = []
+    #                 df = df.reset_index()
+    #                 for date_time_intersect in date_time_intersect_list:
+    #                     check_drop_index_row = df[df['date'] == date_time_intersect]
+    #                     if len(check_drop_index_row) > 1:
+    #                         index_0 = check_drop_index_row.index[0]
+    #                         index_1 = check_drop_index_row.index[1]
+    #                         expiry_date_0 = df.loc[index_0, 'expiry_date']
+    #                         expiry_date_1 = df.loc[index_1, 'expiry_date']
+    #                         close_price_0 = df.loc[index_0, 'close']
+    #                         close_price_1 = df.loc[index_1, 'close']
+    #                         if expiry_date_0 > expiry_date_1:
+    #                             drop_index_list.append(index_1)
+    #                             roll_diff = close_price_0 - close_price_1
+    #                             df.at[index_0,'roll_diff'] = roll_diff
+    #                         elif expiry_date_0 < expiry_date_1:
+    #                             drop_index_list.append(index_0)
+    #                             roll_diff = close_price_1 - close_price_0
+    #                             roll_diff = close_price_0 - close_price_1
+    #                             df.at[index_1,'roll_diff'] = roll_diff
+    #                 if len(drop_index_list) > 0:
+    #                     df = df.drop(drop_index_list, axis=0)
+    #                 df = df.drop('index', axis=1)
+    #
+    #             else:
+    #                 df = df.reset_index()
+    #
+    #                 duplicates = df[df.duplicated(subset=['datetime'], keep=False)]
+    #                 min_expiry_row_index_list = []
+    #
+    #                 for dt in duplicates['datetime'].unique():
+    #                     df2 = duplicates[duplicates['datetime'] == dt]
+    #                     min_expiry = df2['expiry_date'].min()
+    #                     max_expiry = df2['expiry_date'].max()
+    #                     min_expiry_row = df2.loc[df2['expiry_date'] == min_expiry]
+    #                     max_expiry_row = df2.loc[df2['expiry_date'] == max_expiry]
+    #                     min_expiry_row_index = min_expiry_row.index[0]
+    #                     max_expiry_row_index  = max_expiry_row.index[0]
+    #                     min_expiry_close = min_expiry_row['close'].values[0]
+    #                     max_expiry_close = max_expiry_row['close'].values[0]
+    #
+    #                     roll_diff = min_expiry_close - max_expiry_close
+    #
+    #                     min_expiry_row_index_list.append(min_expiry_row_index)
+    #                     df.at[max_expiry_row_index, 'roll_diff'] = roll_diff
+    #
+    #                 if len(min_expiry_row_index_list) > 0:
+    #                     df = df.drop(min_expiry_row_index_list, axis=0)
+    #                 df = df.drop('index', axis=1)
+    #
+    #             df = df.set_index(keys='datetime')
+    #             df = df.sort_index(ascending=True)
+    #
+    #             if '1D' not in freq and rth_only == True:
+    #                 df = df[df['RTH'] == True]
+    #
+    #             #df = df.drop_duplicates(keep='first')
+    #
+    #             return df
+    #
+    #     else:
+    #         err_msg = 'Error in: '
+    #         for error in check_bool_dict:
+    #             if check_bool_dict[error] == False:
+    #                 err_msg += error + ','
+    #         print(err_msg)
 
     def get_hk_market_cap_hist_by_date(self, start_date, end_date):
 
         check_bool_dict = self.check_start_end_date(start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
```

### Comparing `hkfdb-3.6.1/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.7.1/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.6.1
+Version: 3.7.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.6.1/setup.py` & `hkfdb-3.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.6.1",
+    version="3.7.1",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

