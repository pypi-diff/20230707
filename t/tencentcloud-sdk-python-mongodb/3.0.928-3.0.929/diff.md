# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.928.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.928.tar", last modified: Wed Jul  5 00:29:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.929.tar", last modified: Thu Jul  6 00:30:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.928.tar` & `tencentcloud-sdk-python-mongodb-3.0.929.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)     3903 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    13571 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)    76740 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)     7304 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    36443 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)   235397 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:43.000000 tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    13571 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)    76740 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    36443 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)   235050 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:30:20.000000 tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/__init__.py
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.929/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.929/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.929/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.928'
+__version__ = '3.0.929'
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.928/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.929/tencentcloud/mongodb/v20190725/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -924,25 +924,24 @@
         :type InstanceName: str
         :param _AvailabilityZoneList: 多可用区部署的节点列表。具体信息，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567)获取。
 - 多可用区部署节点只能部署在3个不同可用区。不支持将集群的大多数节点部署在同一个可用区。例如：3节点集群不支持2个节点部署在同一个区。
 - 不支持4.2及以上版本。
 - 不支持只读灾备实例。
 - 不能选择基础网络。
         :type AvailabilityZoneList: list of str
-        :param _MongosCpu: Mongos CPU 核数。
-- 购买MongoDB 3.6 WiredTiger存储引擎版本以上的分片集群时，可选择性配置该参数。
-- 若不配置该参数，则根据Mongod节点规格默认适配 Mongos 规格，默认规格免费。
+        :param _MongosCpu: Mongos CPU 核数。购买分片集群时，必须填写。
+
         :type MongosCpu: int
-        :param _MongosMemory: Mongos 内存大小。
-- 购买MongoDB 3.6 WiredTiger存储引擎版本以上的分片集群时，可选择性配置该参数。
-- 若不配置该参数，则根据Mongod节点规格默认适配 Mongos 规格，默认规格免费。
+        :param _MongosMemory: Mongos 内存大小。购买分片集群时，必须填写。
+
+
         :type MongosMemory: int
-        :param _MongosNodeNum: Mongos 数量。
-- 购买MongoDB 3.6 WiredTiger存储引擎版本以上的分片集群时，可选择性配置该参数。
-- 若不配置该参数，则根据Mongod节点规格默认适配 Mongos 规格，默认规格免费。
+        :param _MongosNodeNum: Mongos 数量。购买分片集群时，必须填写。
+
+
         :type MongosNodeNum: int
         :param _ReadonlyNodeNum: 只读节点数量，最大不超过7个。
         :type ReadonlyNodeNum: int
         :param _ReadonlyNodeAvailabilityZoneList: 指只读节点所属可用区。跨可用区部署实例，参数**ReadonlyNodeNum**不为**0**时，必须配置该参数。
         :type ReadonlyNodeAvailabilityZoneList: list of str
         :param _HiddenZone: Hidden节点所属可用区。跨可用区部署实例，必须配置该参数。
         :type HiddenZone: str
@@ -1277,71 +1276,96 @@
 class CreateDBInstanceRequest(AbstractModel):
     """CreateDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _NodeNum: 每个副本集内节点个数，具体参照查询云数据库的售卖规格返回参数
+        :param _NodeNum: 指每个副本集内节点个数。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
         :type NodeNum: int
-        :param _Memory: 实例内存大小，单位：GB
+        :param _Memory: 实例内存大小，单位：GB。
         :type Memory: int
-        :param _Volume: 实例硬盘大小，单位：GB
+        :param _Volume: 实例硬盘大小，单位：GB。
         :type Volume: int
-        :param _MongoVersion: 版本号，具体支持的售卖版本请参照查询云数据库的售卖规格（DescribeSpecInfo）返回结果。参数与版本对应关系是MONGO_3_WT：MongoDB 3.2 WiredTiger存储引擎版本，MONGO_3_ROCKS：MongoDB 3.2 RocksDB存储引擎版本，MONGO_36_WT：MongoDB 3.6 WiredTiger存储引擎版本，MONGO_40_WT：MongoDB 4.0 WiredTiger存储引擎版本，MONGO_42_WT：MongoDB 4.2 WiredTiger存储引擎版本
+        :param _MongoVersion: 指版本信息。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
+- MONGO_36_WT：MongoDB 3.6 WiredTiger存储引擎版本。
+- MONGO_40_WT：MongoDB 4.0 WiredTiger存储引擎版本。
+- MONGO_42_WT：MongoDB 4.2 WiredTiger存储引擎版本。
+- MONGO_44_WT：MongoDB 4.4 WiredTiger存储引擎版本。
         :type MongoVersion: str
-        :param _GoodsNum: 实例数量, 最小值1，最大值为10
+        :param _GoodsNum: 实例数量, 最小值1，最大值为10。
         :type GoodsNum: int
-        :param _Zone: 实例所属区域名称，格式如：ap-guangzhou-2。注：此参数填写的是主可用区，如果选择多可用区部署，Zone必须是AvailabilityZoneList中的一个
+        :param _Zone: 可用区信息，输入格式如：ap-guangzhou-2。
+- 具体信息，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
+- 该参数为主可用区，如果多可用区部署，Zone必须是AvailabilityZoneList中的一个。
         :type Zone: str
-        :param _Period: 实例时长，单位：月，可选值包括 [1,2,3,4,5,6,7,8,9,10,11,12,24,36]
+        :param _Period: 实例时长，单位：月，可选值包括 [1,2,3,4,5,6,7,8,9,10,11,12,24,36]。
         :type Period: int
-        :param _MachineCode: 机器类型，HIO：高IO型；HIO10G：高IO万兆型；STDS5：标准型
+        :param _MachineCode: 机器类型。
+- HIO：高IO型。
+- HIO10G：高IO万兆。
         :type MachineCode: str
-        :param _ClusterType: 实例类型，REPLSET-副本集，SHARD-分片集群，STANDALONE-单节点
+        :param _ClusterType: 实例架构类型。
+- REPLSET：副本集。
+- SHARD：分片集群。
         :type ClusterType: str
-        :param _ReplicateSetNum: 副本集个数，创建副本集实例时，该参数必须设置为1；创建分片实例时，具体参照查询云数据库的售卖规格返回参数；若为单节点实例，该参数设置为0
+        :param _ReplicateSetNum: 指副本集数量。
+- 创建副本集实例，该参数只能为1。
+- 创建分片实例，指分片的数量。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
         :type ReplicateSetNum: int
-        :param _ProjectId: 项目ID，不设置为默认项目
+        :param _ProjectId: 项目ID。若不设置该参数，则为默认项目。
         :type ProjectId: int
-        :param _VpcId: 私有网络 ID，如果不传则默认选择基础网络，请使用 查询私有网络列表
+        :param _VpcId: 私有网络ID。如果不设置该参数，则默认选择基础网络。
         :type VpcId: str
-        :param _SubnetId: 私有网络下的子网 ID，如果设置了 UniqVpcId，则 UniqSubnetId 必填，请使用 查询子网列表
+        :param _SubnetId: 私有网络下的子网 ID，如果配置参数 VpcId，则 SubnetId必须配置。
         :type SubnetId: str
-        :param _Password: 实例密码，不设置该参数则默认密码规则为 实例ID+"@"+主账户uin。举例实例id为cmgo-higv73ed，uin为100000001，则默认密码为"cmgo-higv73ed@100000001"。 自定义密码格式为8-32个字符长度，至少包含字母、数字和字符（!@#%^*()_）中的两种
+        :param _Password: 实例密码。自定义密码长度为8-32个字符，至少包含字母、数字和字符（!@#%^*()_）中的两种。
         :type Password: str
-        :param _Tags: 实例标签信息
+        :param _Tags: 实例标签信息。
         :type Tags: list of TagInfo
-        :param _AutoRenewFlag: 自动续费标记，可选值为：0 - 不自动续费；1 - 自动续费。默认为不自动续费
+        :param _AutoRenewFlag: 自动续费标记。
+- 0：不自动续费。默认为不自动续费。
+- 1：自动续费。
         :type AutoRenewFlag: int
-        :param _AutoVoucher: 是否自动选择代金券，可选值为：1 - 是；0 - 否； 默认为0
+        :param _AutoVoucher: 是否自动选择代金券。
+- 1：是。
+- 0：否。默认为0。
         :type AutoVoucher: int
-        :param _Clone: 1:正式实例,2:临时实例,3:只读实例,4:灾备实例,5:克隆实例
+        :param _Clone: 实例类型。
+- 1：正式实例。
+- 3：只读实例。
+- 4：灾备实例。
         :type Clone: int
-        :param _Father: 若是只读，灾备实例或克隆实例，Father必须填写，即主实例ID
+        :param _Father: 父实例 ID。当参数**Clone**为3或者4时，即实例为只读或灾备实例时，该参数必须配置。
         :type Father: str
-        :param _SecurityGroup: 安全组
+        :param _SecurityGroup: 安全组。
         :type SecurityGroup: list of str
-        :param _RestoreTime: 克隆实例回档时间。若是克隆实例，则必须填写，格式：2021-08-13 16:30:00。注：只能回档7天内的时间点
+        :param _RestoreTime: 克隆实例回档时间。
+- 若为克隆实例，则必须配置该参数。输入格式示例：2021-08-13 16:30:00。
+- 回档时间范围：仅能回档7天内时间点的数据。
         :type RestoreTime: str
-        :param _InstanceName: 实例名称。注：名称只支持长度为60个字符的中文、英文、数字、下划线_、分隔符-
+        :param _InstanceName: 实例名称。仅支持长度为60个字符的中文、英文、数字、下划线_、分隔符- 。
         :type InstanceName: str
-        :param _AvailabilityZoneList: 多可用区部署的节点列表，具体支持的售卖版本请参照查询云数据库的售卖规格（DescribeSpecInfo）返回结果。注：1、多可用区部署节点只能部署在3个不同可用区；2、为了保障跨可用区切换，不支持将集群的大多数节点部署在同一个可用区（如3节点集群不支持2个节点部署在同一个区）；3、不支持4.2及以上版本；4、不支持只读灾备实例；5、不能选择基础网络
+        :param _AvailabilityZoneList: 多可用区部署的节点列表。具体信息，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567)获取。
+- 多可用区部署节点只能部署在3个不同可用区。不支持将集群的大多数节点部署在同一个可用区。例如：3节点集群不支持2个节点部署在同一个区。
+- 不支持4.2及以上版本。
+- 不支持只读灾备实例。
+- 不能选择基础网络。
         :type AvailabilityZoneList: list of str
-        :param _MongosCpu: mongos cpu数量，购买MongoDB 4.2 WiredTiger存储引擎版本的分片集群时必须填写，具体支持的售卖版本请参照查询云数据库的售卖规格（DescribeSpecInfo）返回结果
+        :param _MongosCpu: Mongos CPU 核数，购买MongoDB 4.2 及以上WiredTiger存储引擎版本的分片集群时，必须填写。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
         :type MongosCpu: int
-        :param _MongosMemory: mongos 内存大小，购买MongoDB 4.2 WiredTiger存储引擎版本的分片集群时必须填写，具体支持的售卖版本请参照查询云数据库的售卖规格（DescribeSpecInfo）返回结果
+        :param _MongosMemory: Mongos 内存大小。购买MongoDB 4.2 及以上WiredTiger存储引擎版本的分片集群时，必须填写。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
         :type MongosMemory: int
-        :param _MongosNodeNum: mongos 数量，购买MongoDB 4.2 WiredTiger存储引擎版本的分片集群时必须填写，具体支持的售卖版本请参照查询云数据库的售卖规格（DescribeSpecInfo）返回结果。注：为了保障高可用，最低需要购买3个mongos，上限为32个
+        :param _MongosNodeNum: Mongos 数量。购买MongoDB 4.2 及以上WiredTiger存储引擎版本的分片集群时，必须填写。具体售卖规格，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。为了保障高可用，取值范围为[3,32]。
         :type MongosNodeNum: int
-        :param _ReadonlyNodeNum: 只读节点数量，最大不超过7个
+        :param _ReadonlyNodeNum: 只读节点数量，取值范围[0,5]。
         :type ReadonlyNodeNum: int
-        :param _ReadonlyNodeAvailabilityZoneList: 只读节点部署可用区
+        :param _ReadonlyNodeAvailabilityZoneList: 指只读节点所属可用区。跨可用区部署实例，参数**ReadonlyNodeNum**不为**0**时，必须配置该参数。
         :type ReadonlyNodeAvailabilityZoneList: list of str
-        :param _HiddenZone: Hidden节点所在的可用区，跨可用区实例必传
+        :param _HiddenZone: Hidden节点所属可用区。跨可用区部署实例，必须配置该参数。
         :type HiddenZone: str
         """
         self._NodeNum = None
         self._Memory = None
         self._Volume = None
         self._MongoVersion = None
         self._GoodsNum = None
@@ -1886,15 +1910,15 @@
     def __init__(self):
         r"""
         :param _UnitPrice: 单价
 注意：此字段可能返回 null，表示取不到有效值。
         :type UnitPrice: float
         :param _OriginalPrice: 原价
         :type OriginalPrice: float
-        :param _DiscountPrice: 折扣加
+        :param _DiscountPrice: 折扣价
         :type DiscountPrice: float
         """
         self._UnitPrice = None
         self._OriginalPrice = None
         self._DiscountPrice = None
 
     @property
```

