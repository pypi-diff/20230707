# Comparing `tmp/yplib-2.3.1.tar.gz` & `tmp/yplib-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.1.tar", last modified: Thu Jul  6 08:50:01 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.2.tar", last modified: Fri Jul  7 00:45:15 2023, max compression
```

## Comparing `yplib-2.3.1.tar` & `yplib-2.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.930331 yplib-2.3.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-06 08:50:01.929465 yplib-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 08:50:01.930331 yplib-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-06 08:49:53.000000 yplib-2.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.925604 yplib-2.3.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.3.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.3.1/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    33596 2023-07-06 08:49:32.000000 yplib-2.3.1/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.928963 yplib-2.3.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.080333 yplib-2.3.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-07 00:45:15.079560 yplib-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 00:45:15.080333 yplib-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-07 00:45:04.000000 yplib-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.074144 yplib-2.3.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    30470 2023-07-07 00:24:58.000000 yplib-2.3.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.078433 yplib-2.3.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.1/LICENSE` & `yplib-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/setup.py` & `yplib-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.1",
+  version="2.3.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.1/yplib/__init__.py` & `yplib-2.3.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/chart.py` & `yplib-2.3.2/yplib/chart.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,16 +29,14 @@
                 html_line = html_line.replace(one_p, str(one_data))
         h_r.append(html_line)
     to_txt(data_list=h_r,
            file_name=str(name),
            file_path='html',
            fixed_name=False,
            suffix='.html')
-    # current_path = os.path.abspath(__file__)
-    # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
 
 
 # 将数据整理成折线图
 # 情况1:
 # x轴数据 : x_list = [
 #       ['x轴的数据', 'line1', 'line2', 'line3'],
 #       ['2020-01-01', 120, 132, 101],
@@ -127,38 +125,34 @@
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     # [120, 132, 101, 134, 90, 230, 210],
     series = []
     for y_index in range(len(y_list)):
         y_o = {}
         y_one = y_list[y_index]
-        y_o['name'] = y_one['name'] if 'name' in y_one else name_list[y_index]
-        y_o['smooth'] = 1 if 'smooth' in y_one and y_one['smooth'] else 0
+        y_o['name'] = name_list[y_index]
         y_o['data'] = y_one['data'] if 'data' in y_one else y_one
         y_o['type'] = 'line'
         y_o['stack'] = 'Total'
+        if 'smooth' in y_one and y_one['smooth']:
+            y_o['smooth'] = 1
         # 只有一条线,就不显示 name 了
-        if len(y_list) == 1 and 'name' in y_o:
+        if len(y_list) == 1:
             del y_o['name']
         series.append(y_o)
 
     if not name_raw:
         name = 'line_stack' if name is None else name + '_line_stack'
     insert_data_to_chart(html_data=line_stack_html(),
                          name=name,
                          x_list=x_list,
                          legend=legend,
                          series=series)
 
 
-# print(str([1, 2, 3]))
-# print(str(['a', 'b', 'c']))
-# print(str(map(['a', 'b', 'c'])))
-# print(str(list(map(lambda x: {str(x): 0}, [1, 2, 3, 4]))))
-
 # 将数据整理成折线图
 # 一条折线
 # 数据 : data_list = [
 #             ['2020-01-01', 132],
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
@@ -291,76 +285,7 @@
             y = one_data[value_key]
         x_list.append(x)
         y_list.append(y)
     insert_data_to_chart(html_data=bar_html(),
                          name=name,
                          x_list=x_list,
                          y_list=y_list)
-
-# test_list = []
-# # for i in range(10):
-# #     data.append([uuid_random(), int(random.uniform(0, 1000))])
-# for i in range(10):
-#     one = {}
-#     one['name'] = random_uuid()
-#     one['value'] = int(random.uniform(0, 1000))
-#     test_list.append(one)
-#
-# to_chart_bar(test_list)
-
-#
-#
-# test_list = []
-# for i in range(10):
-#     test_list.append([random_uuid(), int(random.uniform(0, 1000))])
-#
-# to_chart_pie(test_list)
-# to_chart_pie(data, 'yp')
-
-# x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-# y_list = json.loads(
-#     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
-#
-
-# # # 将 list 转化成 图表的例子
-# x_list = []
-# y_list = []
-# # # x 轴有 100 个
-# # # 100 个横坐标
-# for i in range(1000):
-#     x_list.append(i)
-# #
-# # 有 10 条线
-# for i in range(10):  # 0 1 2 3 4 55
-#     n = {}
-#     n['name'] = str(int(random.uniform(0, 1000)))
-#     data = []
-#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
-#     for i in range(100):
-#         data.append(int(random.uniform(0, 1000)))
-#     n['data'] = data
-#     # n['hide'] = '1'
-#     y_list.append(n)
-# #
-# to_chart(x_list, y_list)
-#
-#
-# test_list = []
-# for i in range(50):
-#     test_list.append([i, int(random_int(4))])
-#     test_list.append({'name': i, 'value': int(random_int(4))})
-#
-# to_chart_one(test_list, name='yp')
-# to_chart_one(test_list, name='yp', smooth=True)
-# to_chart_one(test_list, name='yp', is_area=True)
-# to_chart_one(test_list, name='yp', is_area=True, smooth=True)
-#
-# data_list =
-#
-# to_chart(data_list)
-
-# to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls'))
-
-# to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls', column_date=1), name='yp')
-
-#
-# print('end')
```

### Comparing `yplib-2.3.1/yplib/chart_html.py` & `yplib-2.3.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/db.py` & `yplib-2.3.2/yplib/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 
 # 执行 sql 语句
 def exec_sql(db_conn, sql='', commit=True):
     db_cursor = db_conn.cursor()
     if isinstance(sql, list) or isinstance(sql, set):
         for s in sql:
+            to_log_file(s)
             db_cursor.execute(s)
     else:
+        to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
 # print('end')
```

### Comparing `yplib-2.3.1/yplib/file.py` & `yplib-2.3.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/http_util.py` & `yplib-2.3.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/index.py` & `yplib-2.3.2/yplib/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -255,27 +255,27 @@
 
 
 # 将字符串 s 转化成 datetime, 然后再次转化成 str
 def to_datetime_str(s=None):
     return to_datetime(s, r_str=True)
 
 
-# 时间加几天
+# 时间加减
 def to_datetime_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return to_datetime(s) + timedelta(days=days, seconds=seconds, microseconds=microseconds,
                                       milliseconds=milliseconds, minutes=minutes, hours=hours,
                                       weeks=weeks)
 
 
 # 将字符串 s 转化成 date 例如: 2021-02-03
 def to_date(s=None):
     return str(to_datetime(s))[0:10]
 
 
-# 时间加几天
+# 时间加减
 def to_date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return str(to_datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds,
                                milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # data_list   : 数组数据, 也可以不是数组
@@ -494,42 +494,64 @@
                         row_data.append(cell_data)
                         if list_only_one:
                             row_data = cell_data
         data_list.append(row_data)
     return data_list
 
 
-# 将一个文件中以空行作为分隔符, 组成一个 list(list) 数据
+# 将一个文件中以空行作为分隔符,
+# 组成一个 list(list) 数据
+# 多行空行,自动合并到一行空行
 def to_list_from_txt_with_blank_row(file_name='a.txt'):
     return to_list_from_txt(file_name, sep_line='')
 
 
+# 将一个文件中的数据按照行来区分,
+# 会自动过滤掉空格行,
+# 组成一个 list(json) 数据
+def to_list_json_from_txt(file_name='a.txt',
+                          start_index=None,
+                          start_line=None,
+                          end_index=None,
+                          end_line=None,
+                          count=None):
+    return to_list_from_txt(file_name,
+                            start_index=start_index,
+                            start_line=start_line,
+                            end_index=end_index,
+                            end_line=end_line,
+                            count=count,
+                            line_json=True)
+
+
 # 将 txt 文件转化成 list 的方法
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
-# sep               : 是否对每一行进行分割,如果存在这个字段,就分割
-# sep_line          : 这一行是一个分隔符, 返回的是一个 list(list)
-# sep_line_contain  : 这一行是一个分隔符,包含这个行分隔符的做分割, 返回的是一个 list(list)
-# sep_line_prefix   : 这一行是一个分隔符,以这个分隔符作为前缀的, 返回的是一个 list(list)
-# sep_line_suffix   : 这一行是一个分隔符,以这个分隔符作为后缀的, 返回的是一个 list(list)
-# sep_all           : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
-# join              : 针对 list(list) 转化成 list(str) 类型的数据
+# sep               : 对每一行进行分割,将 list(str) 转化为 list(list(str)), 或者将 list(list(str)) 转化为 list(list(list(str)))
+# sep_line          : 这一行是一个分隔符, 分隔符与这行一样, 将 list(str) 转化为 list(list(str))
+# sep_line_contain  : 这一行是一个分隔符,包含这个行分隔符的做分割, 将 list(str) 转化为 list(list(str))
+# sep_line_prefix   : 这一行是一个分隔符,以这个分隔符作为前缀的, 将 list(str) 转化为 list(list(str))
+# sep_line_suffix   : 这一行是一个分隔符,以这个分隔符作为后缀的, 将 list(str) 转化为 list(list(str))
+# sep_all           : 将文件转化成一个字符串,然后对这个字符串,再次总体分割 将 list(str) 转化为 str , 然后再次转化成 list(str)
+# line_join         : 将 list(list(str)) 转化成 list(str) 类型的数据
+# line_json         : 将 list(str) 转化成 list(json) 类型的数据, 会自动过滤掉空格行
 # start_index       : 从这个地方开始读取,从1开始标号 , 包含这一行
 # start_line        : 从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
 # end_index         : 读取到这个地方结束,从1开始标号 , 不包含这一行
 # end_line          : 读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
 # count             : 读取指定的行数
 def to_list_from_txt(file_name='a.txt',
                      sep=None,
                      sep_line=None,
                      sep_line_contain=None,
                      sep_line_prefix=None,
                      sep_line_suffix=None,
                      sep_all=None,
-                     join=None,
+                     line_join=None,
+                     line_json=None,
                      start_index=None,
                      start_line=None,
                      end_index=None,
                      end_line=None,
                      count=None):
     if file_is_empty(file_name=file_name):
         return []
@@ -612,16 +634,24 @@
             # list(list) 情况
             elif isinstance(line, list):
                 a_list = []
                 for o_line in line:
                     a_list.append(o_line.split(str(sep)))
                 r_list.append(a_list)
         data_list = r_list
-    if join is not None:
-        data_list = list(map(lambda x: str(join).join(x), data_list))
+    # data_list 中的每一个元素都转化成 str
+    if line_join is not None:
+        data_list = list(map(lambda x: str(line_join).join(x), data_list))
+    # data_list 中的每一个元素都转化成 先转化成str, 然后再转化成json
+    if line_json is not None and line_json:
+        data_list = list(map(lambda x:
+                             json.loads(str('' if line_join is None else line_join).join(x)),
+                             list(filter(lambda x: x is not None and len(str(x)), data_list))
+                             )
+                         )
     return data_list
 
 
 # 读取文件中的数据,返回一个 str
 def to_str_from_file(file_name='a.txt',
                      str_join='',
                      start_index=None,
@@ -720,166 +750,7 @@
             else:
                 s = str(one_data)
             sh.write(m, n, s)  # 写入A3，数值等于1
         m += 1
     # 5. 保存
     # myWorkbook.save('5002200.xls')
     w_b.save(file_path + '/' + get_file_name(file_name, '.xls'))
-
-# print('start')
-# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt')
-# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\abc\d\e\f')
-# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\p.t')
-# to_txt([1, 2, 3], 'C:/Users/yangpu/Desktop/study/p.t')
-# to_txt_file_name([1,2,3], 'p')
-#
-#
-# li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
-#
-# to_log()
-#
-# to_log()
-# to_log(1)
-# to_log(1, 2)
-# to_log(1, 2, [1, 2])
-# to_log_file(1, 2, [{'a': 2}])
-# to_log_txt('1.txt', 1, 2, [{'a': 2}])
-# to_txt([{'a': 2}])
-# to_txt_data('yangpu', 1)
-# to_txt_data('yangpu1', 1)
-# to_txt_data('yangpu12', 1)
-#
-# x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-# y_list = json.loads(
-#     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
-#
-
-# # 将 list 转化成 图表的例子
-# x_list = []
-# y_list = []
-# # x 轴有 100 个
-# # 100 个横坐标
-# for i in range(100):
-#     x_list.append(i)
-#
-# # 有 10 条线
-# for i in range(10):  # 0 1 2 3 4 55
-#     n = {}
-#     n['name'] = str(int(random.uniform(0, 1000)))
-#     data = []
-#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
-#     for i in range(100):
-#         data.append(int(random.uniform(0, 1000)))
-#     n['data'] = data
-#     y_list.append(n)
-# #
-# to_chart(x_list, y_list)
-#
-# to_txt_data(x_list, 'operate')
-# to_txt_data(y_list, 'operate')
-
-# to_log_file(1)
-# log_to_file(12)
-# log_to_file('yangpu')
-# print(str_to_int('yan123gpu'))
-# print(str_to_float('yan123gpu'))
-# print(str_to_float('yan123g.12pu'))
-
-#
-# print(to_hump('user_id'))
-# print(to_hump('USER_ID'))
-# print(to_hump('userId'))
-# print(to_hump('user'))
-# print(to_hump(''))
-
-# print(to_hump_more('userId'))
-
-# print(to_underline('userId'))
-
-
-# print(uuid_random(5))
-# print(uuid_random(10))
-# print(uuid_random())
-# print(uuid_random(32))
-# print(uuid_random(64))
-# print(uuid_random(128))
-# print(uuid_random(127))
-# print(uuid_random(129))
-
-
-# print(to_int('a'))
-# print(to_int(2))
-# print(to_int(2.2))
-# print(to_int(2.2))
-
-# print(to_float('a'))
-# print(to_float(2))
-# print(to_float(2.2))
-# print(to_float(2.24))
-
-# print(to_date('2019-09'))
-# print(to_date('2019-09-08'))
-# print(to_date('2019-09-08 12'))
-# print(to_date('2019-09-08 12:13'))
-# print(to_datetime('2019-09-08 12:13:14'))
-# print(to_datetime('2019-09-08 12:13:14.789'))
-# print(to_datetime(1686537485))
-# print(to_datetime(1686537484467))
-# print(to_datetime(datetime.today()))
-#
-# print(do_md5())
-# print(do_md5())
-# print(do_md5('yangpu'))
-# print(do_md5('yangpu12'))
-#
-# log_msg = ''
-# headers = {'Content-Type': 'application/json;charset=utf-8'}
-# data = {}
-# data['merchantId'] = "merchantId"
-# data['currency'] = "IDR"
-# data['accType'] = "payout"
-# data['version'] = "1.0"
-# sign = sort_by_json_key(data)
-# print(sign)
-# hash = hashlib.sha256()
-# hash.update(sign.encode('utf-8'))
-# data['sign'] = hash.hexdigest()
-#
-# print(data)
-
-
-# print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'payout', from_last=False))
-
-# get_file_data_line(r'D:\notepad_file\202306', 'a')
-# get_file_by_content(r'D:\notepad_file\202306', 'a')
-# print(get_file(r'D:\notepad_file\202306', 'a'))
-# print(get_file(r'D:\notepad_file\202306'))
-# print(get_file())
-# print(os.path.abspath('.'))
-
-# print('end')
-# for i in range(100):
-#     print(get_file_name('a'))
-#     # print(random_int(i))
-
-# print(get_file_name('a'))
-
-# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, end_index=1288))
-# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, count=3))
-# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', count=1))
-# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
-# print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
-
-#
-# print(not False)
-# print(not True)
-# print(datetime.now())
-# print(datetime.today())
-# print(datetime.today().strftime('%m%d%H%M_%S_%f'))
-# print(get_file_name('1'))
-#
-# for i in range(100):
-#     print(get_file_name('a'))
-#     # print(random_int(i))
-
-
-# print(json.dumps(to_list(r'C:\Users\yangpu\Desktop\study\12.xls')))
```

### Comparing `yplib-2.3.1/yplib/mail.py` & `yplib-2.3.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/mail_html.py` & `yplib-2.3.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.1/yplib/markdown.py` & `yplib-2.3.2/yplib/markdown.py`

 * *Files identical despite different names*

