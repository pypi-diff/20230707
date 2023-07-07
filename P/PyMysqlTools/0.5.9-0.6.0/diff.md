# Comparing `tmp/PyMysqlTools-0.5.9.tar.gz` & `tmp/PyMysqlTools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.5.9.tar", last modified: Thu Nov 10 11:00:27 2022, max compression
+gzip compressed data, was "PyMysqlTools-0.6.0.tar", last modified: Fri Jul  7 10:15:20 2023, max compression
```

## Comparing `PyMysqlTools-0.5.9.tar` & `PyMysqlTools-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.015107 PyMysqlTools-0.5.9/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/LICENSE
--rw-rw-rw-   0        0        0      143 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2594 2022-11-10 11:00:27.015107 PyMysqlTools-0.5.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.000466 PyMysqlTools-0.5.9/PyMysqlTools/
--rw-rw-rw-   0        0        0     2703 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/ClauseGenerator.py
--rw-rw-rw-   0        0        0     4255 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/PlanExecutor.py
--rw-rw-rw-   0        0        0    26690 2022-11-10 10:58:19.000000 PyMysqlTools-0.5.9/PyMysqlTools/PyMysqlTools.py
--rw-rw-rw-   0        0        0     2842 2022-11-10 10:53:46.000000 PyMysqlTools-0.5.9/PyMysqlTools/ResultSet.py
--rw-rw-rw-   0        0        0     1249 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/SqlActuator.py
--rw-rw-rw-   0        0        0     3597 2022-11-09 09:15:02.000000 PyMysqlTools-0.5.9/PyMysqlTools/SqlGenerator.py
--rw-rw-rw-   0        0        0     1240 2022-11-10 10:59:36.000000 PyMysqlTools-0.5.9/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0       68 2022-11-10 03:05:16.000000 PyMysqlTools-0.5.9/PyMysqlTools/config.py
-drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.013159 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2594 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1991 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-10 11:00:27.016083 PyMysqlTools-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.916002 PyMysqlTools-0.6.0/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2610 2023-07-07 10:15:20.914013 PyMysqlTools-0.6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.905030 PyMysqlTools-0.6.0/PyMysqlTools/
+-rw-rw-rw-   0        0        0      432 2023-07-07 10:14:57.000000 PyMysqlTools-0.6.0/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.0/PyMysqlTools/actuator.py
+-rw-rw-rw-   0        0        0     6014 2023-07-07 09:40:25.000000 PyMysqlTools-0.6.0/PyMysqlTools/generator.py
+-rw-rw-rw-   0        0        0    26989 2023-07-07 10:14:57.000000 PyMysqlTools-0.6.0/PyMysqlTools/main.py
+-rw-rw-rw-   0        0        0     3992 2023-07-07 10:15:18.000000 PyMysqlTools-0.6.0/PyMysqlTools/result_set.py
+-rw-rw-rw-   0        0        0       98 2023-07-07 09:32:12.000000 PyMysqlTools-0.6.0/PyMysqlTools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.913009 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2610 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-02-06 01:33:20.000000 PyMysqlTools-0.6.0/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:15:20.916002 PyMysqlTools-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/setup.py
```

### Comparing `PyMysqlTools-0.5.9/LICENSE` & `PyMysqlTools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.9/PKG-INFO` & `PyMysqlTools-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.5.9
+Version: 0.6.0
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
@@ -16,21 +16,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个能以更方便的方式来操作mysql的库
+PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
 
 
 
 **注意**
 
-PyMysqlTools 目前仅支持 Python3.6+ 且 MySQL5.6+ 版本
+PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
 - 下载本项目
 
@@ -47,22 +47,21 @@
   
 
 1. 建立连接
 
    ```python
    import PyMysqlTools
    
+   # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
    print(mysql)
-   
-   # 可以使用上面的示例代码获得一个mysql数据库的连接
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -110,15 +109,15 @@
          print(row)
      ```
 
      
 
    - 其他更多方法详见 api 文档
    
-     - ps: api文档目前还没有。
+     - PS: api文档目前还没有。
 
 
 
 ### 关于社区
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
```

### Comparing `PyMysqlTools-0.5.9/PyMysqlTools/PyMysqlTools.py` & `PyMysqlTools-0.6.0/PyMysqlTools/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import pymysql
 
-import PyMysqlTools.config as config
-from PyMysqlTools.ClauseGenerator import ClauseGenerator
-from PyMysqlTools.SqlActuator import SqlActuator
-from PyMysqlTools.SqlGenerator import SqlGenerator
-from PyMysqlTools.ResultSet import ResultSet
+__all__ = ['Connect', 'ConnectPool', 'ConnectType']
+
+from . import settings
+from .generator import ClauseGenerator
+from .actuator import SqlActuator
+from .generator import SqlGenerator
+from .result_set import ResultSet
 
 from enum import Enum
 from dbutils.persistent_db import PersistentDB
 from dbutils.pooled_db import PooledDB
 
 
 class ConnectType(Enum):
     persistent_db = 1
     pooled_db = 2
 
 
-class connect:
+class Connect:
 
     def __init__(
             self,
             database,
             username=None,
             password=None,
             host='localhost',
             port=3306,
-            charset='utf8mb4'
+            charset='utf8mb4',
     ):
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.database = database
         self.charset = charset
@@ -146,66 +148,76 @@
         :param tb_name: 表名
         :param data: 待更新的数据
         :param id_: id
         :return: 受影响的行数
         """
         return self.update_by(tb_name, data, {'id': id_})
 
-    def find_by(self, tb_name: str, fields: list = None, condition=None, type_=config.DEFAULT_RESULT_SET_TYPE) -> ResultSet:
+    def find_by(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询记录
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name).all()
+            fields_=fields or self.show_table_fields(tb_name).all()
         )
 
-    def find_by_id(self, tb_name: str, id_: int, fields: list = None) -> ResultSet:
+    def find_by_id(self, tb_name: str, id_: int, fields: list = None, type_=None) -> ResultSet:
         """
         根据id查询记录
         :param tb_name: 表名
         :param id_: id
         :param fields: 需要查询的字段
+        :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
-        return self.find_by(tb_name, fields, {'id': id_})
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+        return self.find_by(tb_name, fields, {'id': id_}, type_=type_)
 
-    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=config.DEFAULT_RESULT_SET_TYPE) -> ResultSet:
+    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询单条记录
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         sql += self._clause_generator.build_limit_clause(1)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name).all()
+            fields_=fields or self.show_table_fields(tb_name).all()
         )
 
-    def find_all(self, tb_name: str) -> ResultSet:
+    def find_all(self, tb_name: str, type_=None) -> ResultSet:
         """
         查询全表记录
         :param tb_name: 表名
+        :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
-        return self.find_by(tb_name)
-
-    # ====================================================================================================
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+        return self.find_by(tb_name, type_=type_)
 
     def show_table_fields(self, tb_name: str) -> ResultSet:
         """
         查看表字段
         :param tb_name:表名
         :return: 结果集
         """
@@ -230,24 +242,24 @@
     def show_table_size(self, tb_name: str) -> int:
         """
         查询表有多少条记录
         :param tb_name: 表名
         :return: 记录数
         """
         sql = self._sql_generator.show_table_size(tb_name)
-        return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get(0)
+        return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
 
     def show_table_vague_size(self, tb_name: str) -> int:
         """
         估算表有多少条记录, 准确度低, 但速度快
         :param tb_name:
         :return: 记录数
         """
         sql = self._sql_generator.show_table_vague_size(tb_name)
-        return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get(0)
+        return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
 
     def show_databases(self) -> ResultSet:
         """
         查看所有数据库
         :return: 所有数据库
         """
         sql = self._clause_generator.build_show_clause('DATABASES')
@@ -300,16 +312,14 @@
         删除表所有记录
         :param tb_name: 表名
         :return: 执行结果
         """
         sql = self._sql_generator.delete_table(tb_name)
         return self._sql_actuator.actuator_dml(sql) > 0
 
-    # ====================================================================================================
-
     def create_table(self, tb_name: str, schema) -> int:
         """
         创建数据表
         :param tb_name: 表名
         :param schema: 表结构
         :return: 0表示创建成功
         """
@@ -335,15 +345,14 @@
         """
         row_num = 0
         for row in self.find_all(for_tb_name):
             self.insert_one(to_tb_name, dict(zip(self.show_table_fields(to_tb_name), row)))
             row_num += 1
         return row_num
 
-    # ====================================================================================================
     def close(self):
         """
         关闭数据库连接
         :return:
         """
         self._connect.close()
 
@@ -379,15 +388,15 @@
         """
         这个方法是方便作者debugger用的, 未来可能会移除
         :return:
         """
         return self._sql_generator
 
 
-class connect_pool:
+class ConnectPool:
     def __init__(self, connect_type: ConnectType, connect_args: dict, **pool_args):
         self.creator = pymysql
         self.connect_type = connect_type
         self.connect_args = connect_args
         if self.connect_type == ConnectType.persistent_db:
             self._max_usage = pool_args.get('max_usage', None)
             self._set_session = pool_args.get('set_session', None)
@@ -545,67 +554,78 @@
         :param tb_name: 表名
         :param data: 待更新的数据
         :param id_: id
         :return: 受影响的行数
         """
         return self.update_by(tb_name, data, {'id': id_})
 
-    def find_by(self, tb_name: str, fields: list = None, condition=None, type_=config.DEFAULT_RESULT_SET_TYPE) -> ResultSet:
+    def find_by(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询记录
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         result = ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name).all()
+            fields_=fields or self.show_table_fields(tb_name).all()
         )
         self._connect.close()
         return result
 
-    def find_by_id(self, tb_name: str, id_: int, fields: list = None) -> ResultSet:
+    def find_by_id(self, tb_name: str, id_: int, fields: list = None, type_=None) -> ResultSet:
         """
         根据id查询记录
         :param tb_name: 表名
         :param id_: id
         :param fields: 需要查询的字段
+        :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
-        return self.find_by(tb_name, fields, {'id': id_})
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+        return self.find_by(tb_name, fields, {'id': id_}, type_=type_)
 
-    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=config.DEFAULT_RESULT_SET_TYPE) -> ResultSet:
+    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询单条记录
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
+        :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         sql += self._clause_generator.build_limit_clause(1)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name).all()
+            fields_=fields or self.show_table_fields(tb_name).all()
         )
 
-    def find_all(self, tb_name: str) -> ResultSet:
+    def find_all(self, tb_name: str, type_=None) -> ResultSet:
         """
         查询全表记录
         :param tb_name: 表名
+        :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
-        return self.find_by(tb_name)
-
-    # ====================================================================================================
+        if type_ is None:
+            type_ = settings.DEFAULT_RESULT_SET_TYPE
+        return self.find_by(tb_name, type_=type_)
 
     def show_table_fields(self, tb_name: str) -> ResultSet:
         """
         查看表字段
         :param tb_name:表名
         :return: 结果集
         """
@@ -628,26 +648,26 @@
     def show_table_size(self, tb_name: str) -> int:
         """
         查询表有多少条记录
         :param tb_name: 表名
         :return: 记录数
         """
         sql = self._sql_generator.show_table_size(tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get(0)
+        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
         self._connect.close()
         return result
 
     def show_table_vague_size(self, tb_name: str) -> int:
         """
         估算表有多少条记录, 准确度低, 但速度快
         :param tb_name:
         :return: 记录数
         """
         sql = self._sql_generator.show_table_vague_size(tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get(0)
+        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
         self._connect.close()
         return result
 
     def show_databases(self) -> ResultSet:
         """
         查看所有数据库
         :return: 所有数据库
@@ -712,16 +732,14 @@
         :return: 执行结果
         """
         sql = self._sql_generator.delete_table(tb_name)
         result = self._sql_actuator.actuator_dml(sql) > 0
         self._connect.close()
         return result
 
-    # ====================================================================================================
-
     def create_table(self, tb_name: str, schema) -> int:
         """
         创建数据表
         :param tb_name: 表名
         :param schema: 表结构
         :return: 0表示创建成功
         """
@@ -753,15 +771,14 @@
         for row in self.find_all(for_tb_name):
             self.insert_one(to_tb_name, dict(zip(self.show_table_fields(to_tb_name), row)))
             row_num += 1
         result = row_num
         self._connect.close()
         return result
 
-    # ====================================================================================================
     def close(self):
         """
         关闭数据库连接
         :return:
         """
         self._connect.close()
```

### Comparing `PyMysqlTools-0.5.9/PyMysqlTools/ResultSet.py` & `PyMysqlTools-0.6.0/PyMysqlTools/result_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,122 @@
-import PyMysqlTools.config as config
+from . import settings
 
 
 class ResultSet:
 
     def __init__(
             self,
             result=None,
-            type_=config.DEFAULT_RESULT_SET_TYPE,
+            type_=settings.DEFAULT_RESULT_SET_TYPE,
             fields_=None
     ):
         """
         ResultSet 结果集
         :param result: 暂时的结果集存储在这里
         :param type_: 返回的结果集类型
-        :param fields_: 如果 type_ 为dict时, 需要字段名
+        :param fields_: 当type_为dict时, 需要字段名
         """
         if result is None:
             result = []
 
         self._result = []
+        self._type = type_
 
-        if type_ == list:
+        if self._type == list:
             for row in result:
                 if len(row) > 1:
                     self._result.append(list(row))
                 elif len(row) == 1:
                     self._result.append(row[0])
                 else:
                     self._result.append([None])
-        elif type_ == dict:
+        elif self._type == dict:
             if fields_ is None:
                 raise ValueError('[参数错误]', "'type_'为dict时 'fields_' 需要传入参数")
             else:
-                self._fields = fields_[0]
+                if isinstance(fields_[0], list):
+                    self._fields = fields_[0]
+                else:
+                    self._fields = fields_
                 for row in result:
                     self._result.append(_extract_as_dict(self._fields, row))
         else:
             raise ValueError('[参数数据类型错误]', "'type_' 只能是 list/dict 类型")
 
-        if len(result) == 1:
-            self._result = list(result[0])
-
         self._index = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
+        if not isinstance(self._result, list):
+            return self._result
         if self._index < len(self._result):
             next_ = self._result[self._index]
             self._index += 1
             return next_
         else:
             raise StopIteration
 
     def __str__(self):
         return self._result.__str__()
 
     def __len__(self):
         return len(self._result)
 
     def all(self):
+        """
+        将结果集转换为一个方便迭代的结构(List)
+        :return: List结果集
+        """
         if not self._result:
             return []
-        if not isinstance(self._result[0], list):
+        if self._type == list and not isinstance(self._result, list):
+            return [self._result]
+        if isinstance(self._result, dict):
             return [self._result]
         return self._result
 
     def limit(self, num: int = 1):
+        """
+        截取结果集的前n个结果, 仅List结构可用
+        :param num: 需要截取的结果的数量
+        :return:
+        """
+        if not isinstance(self._result, list):
+            raise ValueError('结果集结构类型不为 `list`, 不支持使用limit')
         if num > 0:
             return self._result[: num]
         else:
             raise ValueError("'num' 参数的值必须大于 0 ！")
 
     def next(self):
+        """
+        获取结果集中的下一个结果, 仅List结构可用
+        :return:
+        """
+        if not isinstance(self._result, list):
+            return self._result
         if self._index < len(self._result):
             next_ = self._result[self._index]
             self._index += 1
             return next_
-        else:
-            return None
 
-    def get(self, index):
-        return self._result[index]
+    def get(self, index: int = 0):
+        """
+        获取特定索引位置的结果, 仅List结构可用
+        :param index:
+        :return:
+        """
+        if not self._result:
+            return None
+        if isinstance(self._result, list):
+            return self._result[index]
+        if self._type == dict or len(self._result) == 1:
+            return self._result
 
 
 def _extract_as_dict(fields: list, value: list):
     fields_len = len(fields)
     value_len = len(value)
 
     if fields_len == value_len:
```

### Comparing `PyMysqlTools-0.5.9/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.6.0/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.5.9
+Version: 0.6.0
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
@@ -16,21 +16,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个能以更方便的方式来操作mysql的库
+PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
 
 
 
 **注意**
 
-PyMysqlTools 目前仅支持 Python3.6+ 且 MySQL5.6+ 版本
+PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
 - 下载本项目
 
@@ -47,22 +47,21 @@
   
 
 1. 建立连接
 
    ```python
    import PyMysqlTools
    
+   # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
    print(mysql)
-   
-   # 可以使用上面的示例代码获得一个mysql数据库的连接
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -110,15 +109,15 @@
          print(row)
      ```
 
      
 
    - 其他更多方法详见 api 文档
    
-     - ps: api文档目前还没有。
+     - PS: api文档目前还没有。
 
 
 
 ### 关于社区
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
```

### Comparing `PyMysqlTools-0.5.9/README.md` & `PyMysqlTools-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个能以更方便的方式来操作mysql的库
+PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
 
 
 
 **注意**
 
-PyMysqlTools 目前仅支持 Python3.6+ 且 MySQL5.6+ 版本
+PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
 - 下载本项目
 
@@ -29,22 +29,21 @@
   
 
 1. 建立连接
 
    ```python
    import PyMysqlTools
    
+   # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
    print(mysql)
-   
-   # 可以使用上面的示例代码获得一个mysql数据库的连接
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -92,15 +91,15 @@
          print(row)
      ```
 
      
 
    - 其他更多方法详见 api 文档
    
-     - ps: api文档目前还没有。
+     - PS: api文档目前还没有。
 
 
 
 ### 关于社区
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
```

### Comparing `PyMysqlTools-0.5.9/setup.py` & `PyMysqlTools-0.6.0/setup.py`

 * *Files identical despite different names*

