# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.928.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.928.tar", last modified: Wed Jul  5 00:35:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.929.tar", last modified: Thu Jul  6 00:35:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.928.tar` & `tencentcloud-sdk-python-teo-3.0.929.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    22107 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   745190 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    84601 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:35:08.000000 tencentcloud-sdk-python-teo-3.0.928/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    22818 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605318 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    60328 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:35:54.000000 tencentcloud-sdk-python-teo-3.0.929/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/setup.py` & `tencentcloud-sdk-python-teo-3.0.929/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.929/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/README.rst` & `tencentcloud-sdk-python-teo-3.0.929/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-# CAM签名/鉴权错误。
-AUTHFAILURE = 'AuthFailure'
-
 # DryRun 操作，代表请求将会是成功的，只是多传了 DryRun 参数。
 DRYRUNOPERATION = 'DryRunOperation'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 证书不存在。
 FAILEDOPERATION_CERTIFICATENOTFOUND = 'FailedOperation.CertificateNotFound'
 
+# 账户余额不足
+FAILEDOPERATION_INSUFFICIENTACCOUNTBALANCE = 'FailedOperation.InsufficientAccountBalance'
+
 # 站点状态不正确。
 FAILEDOPERATION_INVALIDZONESTATUS = 'FailedOperation.InvalidZoneStatus'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 后台处理出错。
@@ -58,65 +58,41 @@
 
 # 后端服务路由地址错误。
 INTERNALERROR_ROUTEERROR = 'InternalError.RouteError'
 
 # 内部错误-系统错误。
 INTERNALERROR_SYSTEMERROR = 'InternalError.SystemError'
 
+# 未知错误。
+INTERNALERROR_UNKNOWERROR = 'InternalError.UnknowError'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 操作频繁，请稍后重试。
 INVALIDPARAMETER_ACTIONINPROGRESS = 'InvalidParameter.ActionInProgress'
 
+# 别称域名不支持配置国密证书。
+INVALIDPARAMETER_ALIASDOMAINNOTSUPPORTSMCERT = 'InvalidParameter.AliasDomainNotSupportSMCert'
+
 # 查询字符串规则超过了限制。
 INVALIDPARAMETER_CACHEKEYQUERYSTRINGTOOMANYVALUE = 'InvalidParameter.CacheKeyQueryStringTooManyValue'
 
-# HTTPS证书链错误。
-INVALIDPARAMETER_CERTCHAINERROR = 'InvalidParameter.CertChainError'
-
-# 证书错误。
-INVALIDPARAMETER_CERTCHECKERROR = 'InvalidParameter.CertCheckError'
-
-# 证书错误。
-INVALIDPARAMETER_CERTCOMPLETEERROR = 'InvalidParameter.CertCompleteError'
-
-# 证书错误。
-INVALIDPARAMETER_CERTFORMATERROR = 'InvalidParameter.CertFormatError'
-
-# HTTPS证书已过期。
-INVALIDPARAMETER_CERTISEXPIRED = 'InvalidParameter.CertIsExpired'
-
-# 证书错误。
-INVALIDPARAMETER_CERTNOCN = 'InvalidParameter.CertNoCn'
-
-# 无效的HTTPS证书。
-INVALIDPARAMETER_CERTNOINFO = 'InvalidParameter.CertNoInfo'
-
 # HTTPS证书和域名不匹配。
 INVALIDPARAMETER_CERTNOTMATCHDOMAIN = 'InvalidParameter.CertNotMatchDomain'
 
-# HTTPS证书和密钥不匹配。
-INVALIDPARAMETER_CERTNOTMATCHKEY = 'InvalidParameter.CertNotMatchKey'
-
-# 证书错误。
-INVALIDPARAMETER_CERTNOTPEM = 'InvalidParameter.CertNotPem'
-
 # 内部错误。
 INVALIDPARAMETER_CERTSYSTEMERROR = 'InvalidParameter.CertSystemError'
 
 # HTTPS证书即将过期。
 INVALIDPARAMETER_CERTTOEXPIRE = 'InvalidParameter.CertToExpire'
 
 # 证书错误。
 INVALIDPARAMETER_CERTTOOSHORTKEYSIZE = 'InvalidParameter.CertTooShortKeySize'
 
-# 证书错误。
-INVALIDPARAMETER_CERTUNSUPPORTEDTYPE = 'InvalidParameter.CertUnsupportedType'
-
 # IPv6 访问与客户端 IP 地理位置功能冲突。
 INVALIDPARAMETER_CLIENTIPCOUNTRYCONFLICTSWITHIPV6 = 'InvalidParameter.ClientIpCountryConflictsWithIpv6'
 
 # CNAME模式下无法申请泛域名证书。
 INVALIDPARAMETER_CNAMEWILDHOSTNOTALLOWAPPLYCERTIFICATE = 'InvalidParameter.CnameWildHostNotAllowApplyCertificate'
 
 # 源站不能和域名一致。
@@ -208,14 +184,17 @@
 
 # 无效的token鉴权密钥。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPESECRETKEY = 'InvalidParameter.InvalidAuthenticationTypeSecretKey'
 
 # 无效的token鉴权参数。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPESIGNPARAM = 'InvalidParameter.InvalidAuthenticationTypeSignParam'
 
+# 无效的第三方对象存储。
+INVALIDPARAMETER_INVALIDAWSPRIVATEACCESS = 'InvalidParameter.InvalidAwsPrivateAccess'
+
 # 无效的备源回源Host。
 INVALIDPARAMETER_INVALIDBACKUPSERVERNAME = 'InvalidParameter.InvalidBackupServerName'
 
 # 无效的节点缓存。
 INVALIDPARAMETER_INVALIDCACHECONFIGCACHE = 'InvalidParameter.InvalidCacheConfigCache'
 
 # 无效的节点缓存，遵循源站行为。
@@ -277,23 +256,29 @@
 
 # 无效的Ipv6开关配置。
 INVALIDPARAMETER_INVALIDIPV6SWITCH = 'InvalidParameter.InvalidIpv6Switch'
 
 # 无效的源站。
 INVALIDPARAMETER_INVALIDORIGIN = 'InvalidParameter.InvalidOrigin'
 
+# 不支持填写内网IP/回环地址作为源站地址
+INVALIDPARAMETER_INVALIDORIGINIP = 'InvalidParameter.InvalidOriginIp'
+
 # 参数错误。
 INVALIDPARAMETER_INVALIDPARAMETER = 'InvalidParameter.InvalidParameter'
 
 # 套餐包不支持最大上传大小。
 INVALIDPARAMETER_INVALIDPOSTMAXSIZEBILLING = 'InvalidParameter.InvalidPostMaxSizeBilling'
 
 # 无效的最大上传大小。
 INVALIDPARAMETER_INVALIDPOSTSIZEVALUE = 'InvalidParameter.InvalidPostSizeValue'
 
+# 请填写AccessKeyId、SecretAccessKey作为第三方对象存储私有访问参数。
+INVALIDPARAMETER_INVALIDPRIVATEACCESSPARAMS = 'InvalidParameter.InvalidPrivateAccessParams'
+
 # 套餐包不支持Quic配置。
 INVALIDPARAMETER_INVALIDQUICBILLING = 'InvalidParameter.InvalidQuicBilling'
 
 # 无效的分片回源。
 INVALIDPARAMETER_INVALIDRANGEORIGINPULL = 'InvalidParameter.InvalidRangeOriginPull'
 
 # 无效的请求头header。
@@ -310,17 +295,14 @@
 
 # 无效的响应头header。
 INVALIDPARAMETER_INVALIDRESPONSEHEADERNAME = 'InvalidParameter.InvalidResponseHeaderName'
 
 # 无效的响应头header。
 INVALIDPARAMETER_INVALIDRESPONSEHEADERVALUE = 'InvalidParameter.InvalidResponseHeaderValue'
 
-# 无效的规则引擎配置。
-INVALIDPARAMETER_INVALIDRULEENGINE = 'InvalidParameter.InvalidRuleEngine'
-
 # 无效的规则引擎操作。
 INVALIDPARAMETER_INVALIDRULEENGINEACTION = 'InvalidParameter.InvalidRuleEngineAction'
 
 # 规则不存在。
 INVALIDPARAMETER_INVALIDRULEENGINENOTFOUND = 'InvalidParameter.InvalidRuleEngineNotFound'
 
 # 无效的规则引擎条件。
@@ -397,14 +379,17 @@
 
 # 与已经添加的记录冲突。
 INVALIDPARAMETERVALUE_CONFLICTRECORD = 'InvalidParameterValue.ConflictRecord'
 
 # DNS 记录与 DNSSEC 功能冲突。
 INVALIDPARAMETERVALUE_CONFLICTWITHDNSSEC = 'InvalidParameterValue.ConflictWithDNSSEC'
 
+# DNS 记录与 NS 记录冲突。
+INVALIDPARAMETERVALUE_CONFLICTWITHNSRECORD = 'InvalidParameterValue.ConflictWithNSRecord'
+
 # 主机记录与记录值不能取值相同。
 INVALIDPARAMETERVALUE_CONTENTSAMEASNAME = 'InvalidParameterValue.ContentSameAsName'
 
 # 入参中的域名与站点参数不匹配，请更正后重试。
 INVALIDPARAMETERVALUE_DOMAINNOTMATCHZONE = 'InvalidParameterValue.DomainNotMatchZone'
 
 # DNS 记录内容错误。
@@ -424,43 +409,64 @@
 
 # 本次提交的资源数超过上限。
 LIMITEXCEEDED_BATCHQUOTA = 'LimitExceeded.BatchQuota'
 
 # 当天提交的资源数超过上限。
 LIMITEXCEEDED_DAILYQUOTA = 'LimitExceeded.DailyQuota'
 
+# 计费套餐不支持。
+LIMITEXCEEDED_PACKNOTALLOW = 'LimitExceeded.PackNotAllow'
+
 # 查询时间范围超出限制。
 LIMITEXCEEDED_QUERYTIMELIMITEXCEEDED = 'LimitExceeded.QueryTimeLimitExceeded'
 
 # 单位时间内接口请求频率达到限制。
 LIMITEXCEEDED_RATELIMITEXCEEDED = 'LimitExceeded.RateLimitExceeded'
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 请联系商务开启「中国大陆网络优化(国际加速)」功能。
 OPERATIONDENIED_ACCELERATEMAINLANDDISABLE = 'OperationDenied.AccelerateMainlandDisable'
 
+# 站点停用未完毕，请稍后再试。
+OPERATIONDENIED_DISABLEZONENOTCOMPLETED = 'OperationDenied.DisableZoneNotCompleted'
+
 # 有域名在共享cname组内，不可切换接入类型。
 OPERATIONDENIED_DOMAININSHARECNAMEGROUP = 'OperationDenied.DomainInShareCnameGroup'
 
 # 域名被封禁，暂时无法操作。
 OPERATIONDENIED_DOMAINISBLOCKED = 'OperationDenied.DomainIsBlocked'
 
 # 域名尚未备案。
 OPERATIONDENIED_DOMAINNOICP = 'OperationDenied.DomainNoICP'
 
+# 站点处于停用状态，请开启后重试。
+OPERATIONDENIED_ERRZONEISALREADYPAUSED = 'OperationDenied.ErrZoneIsAlreadyPaused'
+
+# 开启高防时必须保证安全是开启状态。
+OPERATIONDENIED_INVALIDADVANCEDDEFENSESECURITYTYPE = 'OperationDenied.InvalidAdvancedDefenseSecurityType'
+
+# 开启高防必须保证站点加速区域是国内。
+OPERATIONDENIED_INVALIDADVANCEDDEFENSEZONEAREA = 'OperationDenied.InvalidAdvancedDefenseZoneArea'
+
 # 4层代理资源处于封禁中，禁止操作。
 OPERATIONDENIED_L4PROXYINBANNEDSTATUS = 'OperationDenied.L4ProxyInBannedStatus'
 
+# 存在四层代理实例处于部署中状态，暂不支持停用站点。
+OPERATIONDENIED_L4PROXYINPROGRESSSTATUS = 'OperationDenied.L4ProxyInProgressStatus'
+
+# 存在四层代理实例处于停用中状态，暂不支持停用站点。
+OPERATIONDENIED_L4PROXYINSTOPPINGSTATUS = 'OperationDenied.L4ProxyInStoppingStatus'
+
 # 绑定4层实例有处于非运行中的状态，禁止操作。
 OPERATIONDENIED_L4STATUSNOTINONLINE = 'OperationDenied.L4StatusNotInOnline'
 
-# 回源白名单已经是最新版本，无需更新。
-OPERATIONDENIED_LATESTVERSIONNOW = 'OperationDenied.LatestVersionNow'
+# 存在加速域名处于部署中状态，暂不支持停用站点。
+OPERATIONDENIED_L7HOSTINPROCESSSTATUS = 'OperationDenied.L7HostInProcessStatus'
 
 # 已存在多个Cname接入站点，不允许切换至NS。
 OPERATIONDENIED_MULTIPLECNAMEZONE = 'OperationDenied.MultipleCnameZone'
 
 # NS接入模式不支持域名流量调度功能。
 OPERATIONDENIED_NSNOTALLOWTRAFFICSTRATEGY = 'OperationDenied.NSNotAllowTrafficStrategy'
 
@@ -541,17 +547,14 @@
 
 # 请求的加速域名不存在，请更正后重试。
 RESOURCEUNAVAILABLE_DOMAINNOTFOUND = 'ResourceUnavailable.DomainNotFound'
 
 # 域名不存在或未开启代理。
 RESOURCEUNAVAILABLE_HOSTNOTFOUND = 'ResourceUnavailable.HostNotFound'
 
-# 未拉取到已开启代理的zone信息。
-RESOURCEUNAVAILABLE_PROXYZONENOTFOUND = 'ResourceUnavailable.ProxyZoneNotFound'
-
 # 站点不存在或不属于该账号。
 RESOURCEUNAVAILABLE_ZONENOTFOUND = 'ResourceUnavailable.ZoneNotFound'
 
 # 资源售卖火爆，已售罄，正在加紧补货中，当前无法新增域名，请您耐心等待。
 RESOURCESSOLDOUT_L7LACKOFRESOURCES = 'ResourcesSoldOut.L7LackOfResources'
 
 # 未授权操作。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1594,27 +1594,31 @@
 <li>PPV2：Proxy Protocol传递，协议版本V2；</li>
 <li>OFF：不传递。</li>默认值：OFF。
         :type ForwardClientIp: str
         :param _SessionPersist: 是否开启会话保持，取值有：
 <li>true：开启；</li>
 <li>false：关闭。</li>默认值：false。
         :type SessionPersist: bool
+        :param _SessionPersistTime: 会话保持的时间，只有当SessionPersist为true时，该值才会生效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionPersistTime: int
         :param _OriginPort: 源站端口，支持格式：
 <li>单端口，如：80。</li>
 <li>端口段：81-82，表示81，82两个端口。</li>
         :type OriginPort: str
         """
         self._Proto = None
         self._Port = None
         self._OriginType = None
         self._OriginValue = None
         self._RuleId = None
         self._Status = None
         self._ForwardClientIp = None
         self._SessionPersist = None
+        self._SessionPersistTime = None
         self._OriginPort = None
 
     @property
     def Proto(self):
         return self._Proto
 
     @Proto.setter
@@ -1674,14 +1678,22 @@
         return self._SessionPersist
 
     @SessionPersist.setter
     def SessionPersist(self, SessionPersist):
         self._SessionPersist = SessionPersist
 
     @property
+    def SessionPersistTime(self):
+        return self._SessionPersistTime
+
+    @SessionPersistTime.setter
+    def SessionPersistTime(self, SessionPersistTime):
+        self._SessionPersistTime = SessionPersistTime
+
+    @property
     def OriginPort(self):
         return self._OriginPort
 
     @OriginPort.setter
     def OriginPort(self, OriginPort):
         self._OriginPort = OriginPort
 
@@ -1691,14 +1703,15 @@
         self._Port = params.get("Port")
         self._OriginType = params.get("OriginType")
         self._OriginValue = params.get("OriginValue")
         self._RuleId = params.get("RuleId")
         self._Status = params.get("Status")
         self._ForwardClientIp = params.get("ForwardClientIp")
         self._SessionPersist = params.get("SessionPersist")
+        self._SessionPersistTime = params.get("SessionPersistTime")
         self._OriginPort = params.get("OriginPort")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
@@ -2484,18 +2497,22 @@
 
     @CacheTime.setter
     def CacheTime(self, CacheTime):
         self._CacheTime = CacheTime
 
     @property
     def IgnoreCacheControl(self):
+        warnings.warn("parameter `IgnoreCacheControl` is deprecated", DeprecationWarning) 
+
         return self._IgnoreCacheControl
 
     @IgnoreCacheControl.setter
     def IgnoreCacheControl(self, IgnoreCacheControl):
+        warnings.warn("parameter `IgnoreCacheControl` is deprecated", DeprecationWarning) 
+
         self._IgnoreCacheControl = IgnoreCacheControl
 
 
     def _deserialize(self, params):
         self._Switch = params.get("Switch")
         self._CacheTime = params.get("CacheTime")
         self._IgnoreCacheControl = params.get("IgnoreCacheControl")
@@ -2685,81 +2702,98 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class CheckCertificateRequest(AbstractModel):
-    """CheckCertificate请求参数结构体
+class CheckCnameStatusRequest(AbstractModel):
+    """CheckCnameStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Certificate: 证书内容。
-        :type Certificate: str
-        :param _PrivateKey: 私钥内容。
-        :type PrivateKey: str
+        :param _ZoneId: 站点ID。
+        :type ZoneId: str
+        :param _RecordNames: 记录名称列表。
+        :type RecordNames: list of str
         """
-        self._Certificate = None
-        self._PrivateKey = None
+        self._ZoneId = None
+        self._RecordNames = None
 
     @property
-    def Certificate(self):
-        return self._Certificate
+    def ZoneId(self):
+        return self._ZoneId
 
-    @Certificate.setter
-    def Certificate(self, Certificate):
-        self._Certificate = Certificate
+    @ZoneId.setter
+    def ZoneId(self, ZoneId):
+        self._ZoneId = ZoneId
 
     @property
-    def PrivateKey(self):
-        return self._PrivateKey
+    def RecordNames(self):
+        return self._RecordNames
 
-    @PrivateKey.setter
-    def PrivateKey(self, PrivateKey):
-        self._PrivateKey = PrivateKey
+    @RecordNames.setter
+    def RecordNames(self, RecordNames):
+        self._RecordNames = RecordNames
 
 
     def _deserialize(self, params):
-        self._Certificate = params.get("Certificate")
-        self._PrivateKey = params.get("PrivateKey")
+        self._ZoneId = params.get("ZoneId")
+        self._RecordNames = params.get("RecordNames")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class CheckCertificateResponse(AbstractModel):
-    """CheckCertificate返回参数结构体
+class CheckCnameStatusResponse(AbstractModel):
+    """CheckCnameStatus返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param _CnameStatus: 域名Cname状态信息列表。
+        :type CnameStatus: list of CnameStatus
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self._CnameStatus = None
         self._RequestId = None
 
     @property
+    def CnameStatus(self):
+        return self._CnameStatus
+
+    @CnameStatus.setter
+    def CnameStatus(self, CnameStatus):
+        self._CnameStatus = CnameStatus
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
+        if params.get("CnameStatus") is not None:
+            self._CnameStatus = []
+            for item in params.get("CnameStatus"):
+                obj = CnameStatus()
+                obj._deserialize(item)
+                self._CnameStatus.append(obj)
         self._RequestId = params.get("RequestId")
 
 
 class ClientIpCountry(AbstractModel):
     """回源时携带客户端IP所属地域信息，值的格式为ISO-3166-1两位字母代码。
 
     """
@@ -2852,310 +2886,65 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ClientRule(AbstractModel):
-    """客户端规则信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ClientIp: 客户端ip。
-        :type ClientIp: str
-        :param _RuleType: 规则类型。
-        :type RuleType: str
-        :param _RuleId: 规则id。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RuleId: int
-        :param _Description: 规则描述。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Description: str
-        :param _IpStatus: 封禁状态，取值有：
-<li>block ：封禁 ；</li>
-<li>allow ：放行 。</li>
-        :type IpStatus: str
-        :param _BlockTime: 封禁时间，采用unix秒级时间戳。
-        :type BlockTime: int
-        :param _Id: 每条数据的唯一标识id。
-        :type Id: str
-        """
-        self._ClientIp = None
-        self._RuleType = None
-        self._RuleId = None
-        self._Description = None
-        self._IpStatus = None
-        self._BlockTime = None
-        self._Id = None
-
-    @property
-    def ClientIp(self):
-        return self._ClientIp
-
-    @ClientIp.setter
-    def ClientIp(self, ClientIp):
-        self._ClientIp = ClientIp
-
-    @property
-    def RuleType(self):
-        return self._RuleType
-
-    @RuleType.setter
-    def RuleType(self, RuleType):
-        self._RuleType = RuleType
-
-    @property
-    def RuleId(self):
-        return self._RuleId
-
-    @RuleId.setter
-    def RuleId(self, RuleId):
-        self._RuleId = RuleId
-
-    @property
-    def Description(self):
-        return self._Description
-
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
-
-    @property
-    def IpStatus(self):
-        return self._IpStatus
-
-    @IpStatus.setter
-    def IpStatus(self, IpStatus):
-        self._IpStatus = IpStatus
-
-    @property
-    def BlockTime(self):
-        return self._BlockTime
-
-    @BlockTime.setter
-    def BlockTime(self, BlockTime):
-        self._BlockTime = BlockTime
-
-    @property
-    def Id(self):
-        return self._Id
-
-    @Id.setter
-    def Id(self, Id):
-        self._Id = Id
-
-
-    def _deserialize(self, params):
-        self._ClientIp = params.get("ClientIp")
-        self._RuleType = params.get("RuleType")
-        self._RuleId = params.get("RuleId")
-        self._Description = params.get("Description")
-        self._IpStatus = params.get("IpStatus")
-        self._BlockTime = params.get("BlockTime")
-        self._Id = params.get("Id")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ClsLogTopicInfo(AbstractModel):
-    """日志任务主题信息
+class CnameStatus(AbstractModel):
+    """CNAME 状态
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskName: 任务名。
-        :type TaskName: str
-        :param _ZoneName: 站点名称。
-        :type ZoneName: str
-        :param _LogSetId: 日志集ID。
-        :type LogSetId: str
-        :param _TopicId: 日志主题ID。
-        :type TopicId: str
-        :param _EntityType: 任务类型。
-        :type EntityType: str
-        :param _Period: 任务主题保存时间。
-        :type Period: int
-        :param _Enabled: 任务主题是否开启。
-        :type Enabled: bool
-        :param _Deleted: 任务主题是否异常。
-        :type Deleted: str
-        :param _CreateTime: 创建时间。
-        :type CreateTime: str
-        :param _Target: 推送目标地址,取值有：
-<li>cls: 推送到cls；</li>
-<li>custom_enpoint: 自定义推送地址。</li>
-        :type Target: str
-        :param _LogSetRegion: 日志集所属地区。
+        :param _RecordName: 记录名称。
+        :type RecordName: str
+        :param _Cname: CNAME 地址。
 注意：此字段可能返回 null，表示取不到有效值。
-        :type LogSetRegion: str
-        :param _ZoneId: 站点id。
+        :type Cname: str
+        :param _Status: Cname状态信息，取值有：
+<li>active：生效；</li>
+<li>moved：不生效。</li>
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ZoneId: str
-        :param _Area: 加速区域，取值有：
-<li>mainland：中国大陆境内;</li>
-<li>overseas：全球（不含中国大陆）。</li>
-        :type Area: str
-        :param _LogSetType: 推送任务类型，取值有：
-<li>cls：推送到cls；</li>
-<li>custom_endpoint：推送到自定义接口。</li>
-        :type LogSetType: str
+        :type Status: str
         """
-        self._TaskName = None
-        self._ZoneName = None
-        self._LogSetId = None
-        self._TopicId = None
-        self._EntityType = None
-        self._Period = None
-        self._Enabled = None
-        self._Deleted = None
-        self._CreateTime = None
-        self._Target = None
-        self._LogSetRegion = None
-        self._ZoneId = None
-        self._Area = None
-        self._LogSetType = None
-
-    @property
-    def TaskName(self):
-        return self._TaskName
-
-    @TaskName.setter
-    def TaskName(self, TaskName):
-        self._TaskName = TaskName
-
-    @property
-    def ZoneName(self):
-        return self._ZoneName
-
-    @ZoneName.setter
-    def ZoneName(self, ZoneName):
-        self._ZoneName = ZoneName
-
-    @property
-    def LogSetId(self):
-        return self._LogSetId
-
-    @LogSetId.setter
-    def LogSetId(self, LogSetId):
-        self._LogSetId = LogSetId
-
-    @property
-    def TopicId(self):
-        return self._TopicId
-
-    @TopicId.setter
-    def TopicId(self, TopicId):
-        self._TopicId = TopicId
-
-    @property
-    def EntityType(self):
-        return self._EntityType
-
-    @EntityType.setter
-    def EntityType(self, EntityType):
-        self._EntityType = EntityType
-
-    @property
-    def Period(self):
-        return self._Period
-
-    @Period.setter
-    def Period(self, Period):
-        self._Period = Period
-
-    @property
-    def Enabled(self):
-        return self._Enabled
-
-    @Enabled.setter
-    def Enabled(self, Enabled):
-        self._Enabled = Enabled
-
-    @property
-    def Deleted(self):
-        return self._Deleted
-
-    @Deleted.setter
-    def Deleted(self, Deleted):
-        self._Deleted = Deleted
-
-    @property
-    def CreateTime(self):
-        return self._CreateTime
-
-    @CreateTime.setter
-    def CreateTime(self, CreateTime):
-        self._CreateTime = CreateTime
-
-    @property
-    def Target(self):
-        return self._Target
-
-    @Target.setter
-    def Target(self, Target):
-        self._Target = Target
-
-    @property
-    def LogSetRegion(self):
-        return self._LogSetRegion
-
-    @LogSetRegion.setter
-    def LogSetRegion(self, LogSetRegion):
-        self._LogSetRegion = LogSetRegion
+        self._RecordName = None
+        self._Cname = None
+        self._Status = None
 
     @property
-    def ZoneId(self):
-        return self._ZoneId
+    def RecordName(self):
+        return self._RecordName
 
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
+    @RecordName.setter
+    def RecordName(self, RecordName):
+        self._RecordName = RecordName
 
     @property
-    def Area(self):
-        return self._Area
+    def Cname(self):
+        return self._Cname
 
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
+    @Cname.setter
+    def Cname(self, Cname):
+        self._Cname = Cname
 
     @property
-    def LogSetType(self):
-        return self._LogSetType
+    def Status(self):
+        return self._Status
 
-    @LogSetType.setter
-    def LogSetType(self, LogSetType):
-        self._LogSetType = LogSetType
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
 
 
     def _deserialize(self, params):
-        self._TaskName = params.get("TaskName")
-        self._ZoneName = params.get("ZoneName")
-        self._LogSetId = params.get("LogSetId")
-        self._TopicId = params.get("TopicId")
-        self._EntityType = params.get("EntityType")
-        self._Period = params.get("Period")
-        self._Enabled = params.get("Enabled")
-        self._Deleted = params.get("Deleted")
-        self._CreateTime = params.get("CreateTime")
-        self._Target = params.get("Target")
-        self._LogSetRegion = params.get("LogSetRegion")
-        self._ZoneId = params.get("ZoneId")
-        self._Area = params.get("Area")
-        self._LogSetType = params.get("LogSetType")
+        self._RecordName = params.get("RecordName")
+        self._Cname = params.get("Cname")
+        self._Status = params.get("Status")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3686,27 +3475,30 @@
 <li>PPV2：Proxy Protocol传递，协议版本V2；</li>
 <li>OFF：不传递。</li>默认值：OFF。
         :type ForwardClientIp: str
         :param _SessionPersist: 是否开启会话保持，取值有：
 <li>true：开启；</li>
 <li>false：关闭。</li>默认值：false。
         :type SessionPersist: bool
+        :param _SessionPersistTime: 会话保持的时间，只有当SessionPersist为true时，该值才会生效。
+        :type SessionPersistTime: int
         :param _OriginPort: 源站端口，支持格式：
 <li>单端口：80；</li>
 <li>端口段：81-90，81至90端口。</li>
         :type OriginPort: str
         """
         self._ZoneId = None
         self._ProxyId = None
         self._Proto = None
         self._Port = None
         self._OriginType = None
         self._OriginValue = None
         self._ForwardClientIp = None
         self._SessionPersist = None
+        self._SessionPersistTime = None
         self._OriginPort = None
 
     @property
     def ZoneId(self):
         return self._ZoneId
 
     @ZoneId.setter
@@ -3766,14 +3558,22 @@
         return self._SessionPersist
 
     @SessionPersist.setter
     def SessionPersist(self, SessionPersist):
         self._SessionPersist = SessionPersist
 
     @property
+    def SessionPersistTime(self):
+        return self._SessionPersistTime
+
+    @SessionPersistTime.setter
+    def SessionPersistTime(self, SessionPersistTime):
+        self._SessionPersistTime = SessionPersistTime
+
+    @property
     def OriginPort(self):
         return self._OriginPort
 
     @OriginPort.setter
     def OriginPort(self, OriginPort):
         self._OriginPort = OriginPort
 
@@ -3783,14 +3583,15 @@
         self._ProxyId = params.get("ProxyId")
         self._Proto = params.get("Proto")
         self._Port = params.get("Port")
         self._OriginType = params.get("OriginType")
         self._OriginValue = params.get("OriginValue")
         self._ForwardClientIp = params.get("ForwardClientIp")
         self._SessionPersist = params.get("SessionPersist")
+        self._SessionPersistTime = params.get("SessionPersistTime")
         self._OriginPort = params.get("OriginPort")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
@@ -3831,45 +3632,14 @@
 
 
     def _deserialize(self, params):
         self._RuleId = params.get("RuleId")
         self._RequestId = params.get("RequestId")
 
 
-class CreateCredentialRequest(AbstractModel):
-    """CreateCredential请求参数结构体
-
-    """
-
-
-class CreateCredentialResponse(AbstractModel):
-    """CreateCredential返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class CreateOriginGroupRequest(AbstractModel):
     """CreateOriginGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4120,14 +3890,15 @@
 
     def __init__(self):
         r"""
         :param _ZoneId: 站点 ID。
         :type ZoneId: str
         :param _Targets: 要预热的资源列表，每个元素格式类似如下:
 http://www.example.com/example.txt。
+注意：提交任务数受计费套餐配额限制，请查看 [EO计费套餐](https://cloud.tencent.com/document/product/1552/77380)。
         :type Targets: list of str
         :param _EncodeUrl: 是否对url进行encode，若内容含有非 ASCII 字符集的字符，请开启此开关进行编码转换（编码规则遵循 RFC3986）。
         :type EncodeUrl: bool
         :param _Headers: 附带的http头部信息。
         :type Headers: list of Header
         """
         self._ZoneId = None
@@ -4246,41 +4017,34 @@
 class CreatePurgeTaskRequest(AbstractModel):
     """CreatePurgeTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ZoneId: 站点ID。
+        :param _ZoneId: 站点 ID。
         :type ZoneId: str
-        :param _Type: 清除缓存类型，取值有：
-<li>purge_url：URL；</li>
-<li>purge_prefix：前缀；</li>
-<li>purge_host：Hostname；</li>
-<li>purge_all：全部缓存；</li>
-<li>purge_cache_tag：cache-tag刷新。</li>
+        :param _Type: 节点缓存清除类型，取值有：
+<li>purge_url：URL刷新；</li>
+<li>purge_prefix：目录刷新；</li>
+<li>purge_host：Hostname 刷新；</li>
+<li>purge_all：站点下全部缓存刷新；</li>
+<li>purge_cache_tag：cache-tag 刷新。</li>缓存清除类型详情请查看[清除缓存](https://cloud.tencent.com/document/product/1552/70759)。
         :type Type: str
-        :param _Targets: 要清除缓存的资源列表，每个元素格式依据Type而定：
-1) Type = purge_host 时：
-形如：www.example.com 或 foo.bar.example.com。
-2) Type = purge_prefix 时：
-形如：http://www.example.com/example。
-3) Type = purge_url 时：
-形如：https://www.example.com/example.jpg。
-4）Type = purge_all 时：
-Targets可为空，不需要填写。
-5）Type = purge_cache_tag 时：
-形如：tag1。
+        :param _Method: 节点缓存清除方法，仅对目录刷新类型有效，取值有：<li> invalidate：仅刷新目录下产生了更新的资源；</li><li> delete：无论目录下资源是否更新都刷新节点资源。</li>注意：使用目录刷新时，默认值： invalidate。
+        :type Method: str
+        :param _Targets: 要清除缓存的资源列表。每个元素格式依据清除缓存类型而定，可参考接口示例。<li>EO 默认针对内容含有非 ASCII 字符集的字符进行转义，编码规则遵循 RFC3986；</li><li>单次提交的任务数受计费套餐配额限制，请查看 [EO计费套餐](https://cloud.tencent.com/document/product/1552/77380)。</li>
         :type Targets: list of str
         :param _EncodeUrl: 若有编码转换，仅清除编码转换后匹配的资源。
 若内容含有非 ASCII 字符集的字符，请开启此开关进行编码转换（编码规则遵循 RFC3986）。
         :type EncodeUrl: bool
         """
         self._ZoneId = None
         self._Type = None
+        self._Method = None
         self._Targets = None
         self._EncodeUrl = None
 
     @property
     def ZoneId(self):
         return self._ZoneId
 
@@ -4293,33 +4057,46 @@
         return self._Type
 
     @Type.setter
     def Type(self, Type):
         self._Type = Type
 
     @property
+    def Method(self):
+        return self._Method
+
+    @Method.setter
+    def Method(self, Method):
+        self._Method = Method
+
+    @property
     def Targets(self):
         return self._Targets
 
     @Targets.setter
     def Targets(self, Targets):
         self._Targets = Targets
 
     @property
     def EncodeUrl(self):
+        warnings.warn("parameter `EncodeUrl` is deprecated", DeprecationWarning) 
+
         return self._EncodeUrl
 
     @EncodeUrl.setter
     def EncodeUrl(self, EncodeUrl):
+        warnings.warn("parameter `EncodeUrl` is deprecated", DeprecationWarning) 
+
         self._EncodeUrl = EncodeUrl
 
 
     def _deserialize(self, params):
         self._ZoneId = params.get("ZoneId")
         self._Type = params.get("Type")
+        self._Method = params.get("Method")
         self._Targets = params.get("Targets")
         self._EncodeUrl = params.get("EncodeUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
@@ -4331,15 +4108,15 @@
 class CreatePurgeTaskResponse(AbstractModel):
     """CreatePurgeTask返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _JobId: 任务ID。
+        :param _JobId: 任务 ID。
         :type JobId: str
         :param _FailedList: 失败的任务列表及原因。
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailedList: list of FailReason
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
@@ -4379,101 +4156,14 @@
             for item in params.get("FailedList"):
                 obj = FailReason()
                 obj._deserialize(item)
                 self._FailedList.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class CreateReplayTaskRequest(AbstractModel):
-    """CreateReplayTask请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Ids: 重放任务的 ID 列表。
-        :type Ids: list of str
-        """
-        self._Ids = None
-
-    @property
-    def Ids(self):
-        return self._Ids
-
-    @Ids.setter
-    def Ids(self, Ids):
-        self._Ids = Ids
-
-
-    def _deserialize(self, params):
-        self._Ids = params.get("Ids")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CreateReplayTaskResponse(AbstractModel):
-    """CreateReplayTask返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _JobId: 此次任务ID。
-        :type JobId: str
-        :param _FailedList: 失败的任务列表及原因。
-        :type FailedList: list of FailReason
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._JobId = None
-        self._FailedList = None
-        self._RequestId = None
-
-    @property
-    def JobId(self):
-        return self._JobId
-
-    @JobId.setter
-    def JobId(self, JobId):
-        self._JobId = JobId
-
-    @property
-    def FailedList(self):
-        return self._FailedList
-
-    @FailedList.setter
-    def FailedList(self, FailedList):
-        self._FailedList = FailedList
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._JobId = params.get("JobId")
-        if params.get("FailedList") is not None:
-            self._FailedList = []
-            for item in params.get("FailedList"):
-                obj = FailReason()
-                obj._deserialize(item)
-                self._FailedList.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class CreateRuleRequest(AbstractModel):
     """CreateRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4675,96 +4365,27 @@
 
 
     def _deserialize(self, params):
         self._GroupId = params.get("GroupId")
         self._RequestId = params.get("RequestId")
 
 
-class CreateSpeedTestingRequest(AbstractModel):
-    """CreateSpeedTesting请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点 ID。
-        :type ZoneId: str
-        :param _Host: 拨测子域名。
-        :type Host: str
-        """
-        self._ZoneId = None
-        self._Host = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def Host(self):
-        return self._Host
-
-    @Host.setter
-    def Host(self, Host):
-        self._Host = Host
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._Host = params.get("Host")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CreateSpeedTestingResponse(AbstractModel):
-    """CreateSpeedTesting返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class CreateZoneRequest(AbstractModel):
     """CreateZone请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _ZoneName: 站点名称。
         :type ZoneName: str
         :param _Type: 接入方式，取值有：
 <li> full：NS接入；</li>
-<li> partial：CNAME接入，请先调用认证站点API（IdentifyZone）进行站点归属权校验，校验通过后继续调用本接口创建站点。</li>不填写使用默认值full。
+<li> partial：CNAME接入，请先调用认证站点API（IdentifyZone）进行站点归属权校验，校验通过后继续调用本接口创建站点；<li>noDomainAccess：无域名接入，取此值时仅Tags字段有效。</li>
+</li>不填写使用默认值full。
         :type Type: str
         :param _JumpStart: 是否跳过站点现有的DNS记录扫描。默认值：false。
         :type JumpStart: bool
         :param _Tags: 资源标签。
         :type Tags: list of Tag
         :param _AllowDuplicates: 是否允许重复接入。
 <li> true：允许重复接入；</li>
@@ -6048,129 +5669,14 @@
             for item in params.get("AccelerationDomains"):
                 obj = AccelerationDomain()
                 obj._deserialize(item)
                 self._AccelerationDomains.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeAddableEntityListRequest(AbstractModel):
-    """DescribeAddableEntityList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _EntityType: 推送数据类型，取值有:
-<li>domain：七层加速日志；</li>
-<li>application：四层加速日志；</li>
-<li>web-rateLiming：速率限制日志；</li>
-<li>web-attack：web攻击防护日志；</li>
-<li>web-rule：自定义规则日志；</li>
-<li>web-bot：Bot管理日志。</li>
-        :type EntityType: str
-        :param _Area: 服务区域，取值有：
-<li>mainland：中国大陆境内；</li>
-<li>overseas：全球（不含中国大陆）。</li>若为国内站账号，则默认取值为mainland；若为国际站账号，则默认取值为overseas。
-        :type Area: str
-        """
-        self._ZoneId = None
-        self._EntityType = None
-        self._Area = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def EntityType(self):
-        return self._EntityType
-
-    @EntityType.setter
-    def EntityType(self, EntityType):
-        self._EntityType = EntityType
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._EntityType = params.get("EntityType")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeAddableEntityListResponse(AbstractModel):
-    """DescribeAddableEntityList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _EntityList: 可添加的实体列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type EntityList: list of str
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._TotalCount = None
-        self._EntityList = None
-        self._RequestId = None
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def EntityList(self):
-        return self._EntityList
-
-    @EntityList.setter
-    def EntityList(self, EntityList):
-        self._EntityList = EntityList
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._TotalCount = params.get("TotalCount")
-        self._EntityList = params.get("EntityList")
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeAliasDomainsRequest(AbstractModel):
     """DescribeAliasDomains请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6457,190 +5963,14 @@
             for item in params.get("PlanInfo"):
                 obj = PlanInfo()
                 obj._deserialize(item)
                 self._PlanInfo.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeClientRuleListRequest(AbstractModel):
-    """DescribeClientRuleList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 查询的站点ID.
-        :type ZoneId: str
-        :param _Domain: 查询的子域名。
-        :type Domain: str
-        :param _RuleType: 规则类型，取值有：
-<li>acl：自定义规则；</li>
-<li>rate：限速规则。</li>不填表示查询所有规则。
-        :type RuleType: str
-        :param _RuleId: 规则ID。
-        :type RuleId: int
-        :param _SourceClientIp: 客户端IP。
-        :type SourceClientIp: str
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._ZoneId = None
-        self._Domain = None
-        self._RuleType = None
-        self._RuleId = None
-        self._SourceClientIp = None
-        self._Limit = None
-        self._Offset = None
-        self._Area = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def Domain(self):
-        return self._Domain
-
-    @Domain.setter
-    def Domain(self, Domain):
-        self._Domain = Domain
-
-    @property
-    def RuleType(self):
-        return self._RuleType
-
-    @RuleType.setter
-    def RuleType(self, RuleType):
-        self._RuleType = RuleType
-
-    @property
-    def RuleId(self):
-        return self._RuleId
-
-    @RuleId.setter
-    def RuleId(self, RuleId):
-        self._RuleId = RuleId
-
-    @property
-    def SourceClientIp(self):
-        return self._SourceClientIp
-
-    @SourceClientIp.setter
-    def SourceClientIp(self, SourceClientIp):
-        self._SourceClientIp = SourceClientIp
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._Domain = params.get("Domain")
-        self._RuleType = params.get("RuleType")
-        self._RuleId = params.get("RuleId")
-        self._SourceClientIp = params.get("SourceClientIp")
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeClientRuleListResponse(AbstractModel):
-    """DescribeClientRuleList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: 封禁客户端数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of ClientRule
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = ClientRule()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeContentQuotaRequest(AbstractModel):
     """DescribeContentQuota请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7428,139 +6758,14 @@
             for item in params.get("DefaultServerCertInfo"):
                 obj = DefaultServerCertInfo()
                 obj._deserialize(item)
                 self._DefaultServerCertInfo.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeDnsDataRequest(AbstractModel):
-    """DescribeDnsData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 起始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _Filters: 过滤条件，Filters.Values的上限为20。详细的过滤条件如下：
-<li>zone<br>   按照【<strong>站点名称</strong>】进行过滤。站点名称形如：tencent.com<br>   类型：String<br>   必选：否，仅支持填写一个站点
-<li>host<br>   按照【<strong>域名</strong>】进行过滤。域名形如：test.tencent.com<br>   类型：String<br>   必选：否，仅支持填写一个域名
-<li>type<br>   按照【<strong>DNS解析类型</strong>】进行过滤<br>   类型：String<br>   必选：否<br>   可选项：<br>   A：A记录<br>   AAAA：AAAA记录<br>   CNAME：CNAME记录<br>   MX：MX记录<br>   TXT：TXT记录<br>   NS：NS记录<br>   SRV：SRV记录<br>   CAA：CAA记录
-<li>code<br>   按照【<strong>DNS解析状态码</strong>】进行过滤。<br>   类型：String<br>   必选：否<br>   可选项：<br>   NoError：成功<br>   NXDomain：请求域不存在<br>   NotImp：不支持的请求类型<br>   Refused：域名服务器因为策略的原因拒绝执行请求
-<li>area<br>   按照【<strong>DNS解析地域</strong>】进行过滤。<br>   类型：String<br>   必选：否。<br>   可选项：<br>   亚洲：Asia<br>   欧洲：Europe<br>   非洲：Africa<br>   大洋洲：Oceania<br>   美洲：Americas
-        :type Filters: list of Filter
-        :param _Interval: 时间粒度，取值有：
-<li>min：1分钟粒度；</li>
-<li>5min：5分钟粒度；</li>
-<li>hour：1小时粒度；</li>
-<li>day：天粒度。</li>不填写，默认值为：min。
-        :type Interval: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._Filters = None
-        self._Interval = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        if params.get("Filters") is not None:
-            self._Filters = []
-            for item in params.get("Filters"):
-                obj = Filter()
-                obj._deserialize(item)
-                self._Filters.append(obj)
-        self._Interval = params.get("Interval")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeDnsDataResponse(AbstractModel):
-    """DescribeDnsData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: 统计数据。
-        :type Data: list of DnsData
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = DnsData()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeHostsSettingRequest(AbstractModel):
     """DescribeHostsSetting请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7799,238 +7004,14 @@
             for item in params.get("Identifications"):
                 obj = Identification()
                 obj._deserialize(item)
                 self._Identifications.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeLogSetsRequest(AbstractModel):
-    """DescribeLogSets请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _LogSetRegion: 日志集所属的地域。
-        :type LogSetRegion: str
-        :param _LogSetId: 日志集ID。
-        :type LogSetId: str
-        :param _LogSetName: 日志集名称。
-        :type LogSetName: str
-        """
-        self._LogSetRegion = None
-        self._LogSetId = None
-        self._LogSetName = None
-
-    @property
-    def LogSetRegion(self):
-        return self._LogSetRegion
-
-    @LogSetRegion.setter
-    def LogSetRegion(self, LogSetRegion):
-        self._LogSetRegion = LogSetRegion
-
-    @property
-    def LogSetId(self):
-        return self._LogSetId
-
-    @LogSetId.setter
-    def LogSetId(self, LogSetId):
-        self._LogSetId = LogSetId
-
-    @property
-    def LogSetName(self):
-        return self._LogSetName
-
-    @LogSetName.setter
-    def LogSetName(self, LogSetName):
-        self._LogSetName = LogSetName
-
-
-    def _deserialize(self, params):
-        self._LogSetRegion = params.get("LogSetRegion")
-        self._LogSetId = params.get("LogSetId")
-        self._LogSetName = params.get("LogSetName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeLogSetsResponse(AbstractModel):
-    """DescribeLogSets返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _LogSetList: 日志集列表数据。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type LogSetList: list of LogSetInfo
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._LogSetList = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def LogSetList(self):
-        return self._LogSetList
-
-    @LogSetList.setter
-    def LogSetList(self, LogSetList):
-        self._LogSetList = LogSetList
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("LogSetList") is not None:
-            self._LogSetList = []
-            for item in params.get("LogSetList"):
-                obj = LogSetInfo()
-                obj._deserialize(item)
-                self._LogSetList.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeLogTopicTasksRequest(AbstractModel):
-    """DescribeLogTopicTasks请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        """
-        self._ZoneId = None
-        self._Limit = None
-        self._Offset = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeLogTopicTasksResponse(AbstractModel):
-    """DescribeLogTopicTasks返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TopicList: 推送任务列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TopicList: list of ClsLogTopicInfo
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._TopicList = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def TopicList(self):
-        return self._TopicList
-
-    @TopicList.setter
-    def TopicList(self, TopicList):
-        self._TopicList = TopicList
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("TopicList") is not None:
-            self._TopicList = []
-            for item in params.get("TopicList"):
-                obj = ClsLogTopicInfo()
-                obj._deserialize(item)
-                self._TopicList.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeOriginGroupRequest(AbstractModel):
     """DescribeOriginGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8917,411 +7898,14 @@
             for item in params.get("Actions"):
                 obj = RulesSettingAction()
                 obj._deserialize(item)
                 self._Actions.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeSingleL7AnalysisDataRequest(AbstractModel):
-    """DescribeSingleL7AnalysisData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _MetricNames: 查询的指标，取值有:
-<li> l7Flow_singleIpRequest：独立IP请求数。</li>
-        :type MetricNames: list of str
-        :param _ZoneIds: 站点集合。
-若不填写，默认选择全部站点，且最多只能查询近30天的数据；
-若填写，则可查询站点绑定套餐支持的<a href="https://cloud.tencent.com/document/product/1552/77380#edgeone-.E5.A5.97.E9.A4.90">数据分析最大查询范围</a>。
-        :type ZoneIds: list of str
-        :param _Filters: 过滤条件，详细的过滤条件Key值如下：
-<li>country<br>   按照【<strong>国家/地区</strong>】进行过滤，国家/地区遵循<a href="https://zh.wikipedia.org/wiki/ISO_3166-1">ISO 3166</a>规范。</li>
-<li>domain<br>   按照【<strong>子域名</strong>】进行过滤，子域名形如： test.example.com。</li>
-<li>protocol<br>   按照【<strong>HTTP协议版本</strong>】进行过滤。<br>   对应的Value可选项如下：<br>   HTTP/1.0：HTTP 1.0；<br>   HTTP/1.1：HTTP 1.1；<br>   HTTP/2.0：HTTP 2.0；<br>   HTTP/3.0：HTTP 3.0；<br>   WebSocket：WebSocket。</li>
-<li>socket<br>   按照【<strong>HTTP协议类型</strong>】进行过滤。<br>   对应的Value可选项如下：<br>   HTTP：HTTP 协议；<br>   HTTPS：HTTPS协议；<br>   QUIC：QUIC协议。</li>
-<li>tagKey<br>   按照【<strong>标签Key</strong>】进行过滤。</li>
-<li>tagValue<br>   按照【<strong>标签Value</strong>】进行过滤。</li>
-        :type Filters: list of QueryCondition
-        :param _Interval: 查询时间粒度，取值有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天;。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：1小时范围内以min粒度查询，2天范围内以5min粒度查询，7天范围内以hour粒度查询，超过7天以day粒度查询。
-        :type Interval: str
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据；</li>
-<li>global：全球数据。</li>不填默认取值为global。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._MetricNames = None
-        self._ZoneIds = None
-        self._Filters = None
-        self._Interval = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def MetricNames(self):
-        return self._MetricNames
-
-    @MetricNames.setter
-    def MetricNames(self, MetricNames):
-        self._MetricNames = MetricNames
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._MetricNames = params.get("MetricNames")
-        self._ZoneIds = params.get("ZoneIds")
-        if params.get("Filters") is not None:
-            self._Filters = []
-            for item in params.get("Filters"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._Filters.append(obj)
-        self._Interval = params.get("Interval")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeSingleL7AnalysisDataResponse(AbstractModel):
-    """DescribeSingleL7AnalysisData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _Data: 单值流量数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SingleDataRecord
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._TotalCount = None
-        self._Data = None
-        self._RequestId = None
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._TotalCount = params.get("TotalCount")
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SingleDataRecord()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeSpeedTestingDetailsRequest(AbstractModel):
-    """DescribeSpeedTestingDetails请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        """
-        self._ZoneId = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeSpeedTestingDetailsResponse(AbstractModel):
-    """DescribeSpeedTestingDetails返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SpeedTestingDetailData: 分地域拨测统计数据。
-        :type SpeedTestingDetailData: :class:`tencentcloud.teo.v20220901.models.SpeedTestingDetailData`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._SpeedTestingDetailData = None
-        self._RequestId = None
-
-    @property
-    def SpeedTestingDetailData(self):
-        return self._SpeedTestingDetailData
-
-    @SpeedTestingDetailData.setter
-    def SpeedTestingDetailData(self, SpeedTestingDetailData):
-        self._SpeedTestingDetailData = SpeedTestingDetailData
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("SpeedTestingDetailData") is not None:
-            self._SpeedTestingDetailData = SpeedTestingDetailData()
-            self._SpeedTestingDetailData._deserialize(params.get("SpeedTestingDetailData"))
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeSpeedTestingMetricDataRequest(AbstractModel):
-    """DescribeSpeedTestingMetricData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        """
-        self._ZoneId = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeSpeedTestingMetricDataResponse(AbstractModel):
-    """DescribeSpeedTestingMetricData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SpeedTestingMetricData: 站点拨测维度数据。
-        :type SpeedTestingMetricData: :class:`tencentcloud.teo.v20220901.models.SpeedTestingMetricData`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._SpeedTestingMetricData = None
-        self._RequestId = None
-
-    @property
-    def SpeedTestingMetricData(self):
-        return self._SpeedTestingMetricData
-
-    @SpeedTestingMetricData.setter
-    def SpeedTestingMetricData(self, SpeedTestingMetricData):
-        self._SpeedTestingMetricData = SpeedTestingMetricData
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("SpeedTestingMetricData") is not None:
-            self._SpeedTestingMetricData = SpeedTestingMetricData()
-            self._SpeedTestingMetricData._deserialize(params.get("SpeedTestingMetricData"))
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeSpeedTestingQuotaRequest(AbstractModel):
-    """DescribeSpeedTestingQuota请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        """
-        self._ZoneId = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeSpeedTestingQuotaResponse(AbstractModel):
-    """DescribeSpeedTestingQuota返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SpeedTestingQuota: 配额数据。
-        :type SpeedTestingQuota: :class:`tencentcloud.teo.v20220901.models.SpeedTestingQuota`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._SpeedTestingQuota = None
-        self._RequestId = None
-
-    @property
-    def SpeedTestingQuota(self):
-        return self._SpeedTestingQuota
-
-    @SpeedTestingQuota.setter
-    def SpeedTestingQuota(self, SpeedTestingQuota):
-        self._SpeedTestingQuota = SpeedTestingQuota
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("SpeedTestingQuota") is not None:
-            self._SpeedTestingQuota = SpeedTestingQuota()
-            self._SpeedTestingQuota._deserialize(params.get("SpeedTestingQuota"))
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeTimingL4DataRequest(AbstractModel):
     """DescribeTimingL4Data请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9886,195 +8470,14 @@
             for item in params.get("Data"):
                 obj = TimingDataRecord()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeTimingL7SourceDataRequest(AbstractModel):
-    """DescribeTimingL7SourceData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _MetricNames: 指标列表，取值有:
-<li>l7Flow_outFlux_hy: Edgeone请求流量；</li>
-<li>l7Flow_outBandwidth_hy: Edgeone请求带宽；</li>
-<li>l7Flow_inFlux_hy: 源站响应流量；</li>
-<li>l7Flow_inBandwidth_hy: 源站响应带宽；</li>
-<li>l7Flow_request_hy: 回源请求数；</li>
-        :type MetricNames: list of str
-        :param _ZoneIds: 待查询的站点列表，此参数必填。
-        :type ZoneIds: list of str
-        :param _Interval: 查询时间粒度，取值有：
-<li>min: 1分钟；</li>
-<li>5min: 5分钟；</li>
-<li>hour: 1小时；</li>
-<li>day: 1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _Filters: 过滤条件，详细的过滤条件如下：
-<li>domain<br>   按照【<strong>回源Host</strong>】进行过滤。<br>   类型：String<br>   必选：否</li>
-<li>origin<br>   按照【<strong>源站</strong>】进行过滤。<br>   类型：String<br>   必选：否</li>
-<li>originGroup<br>   按照【<strong>源站组</strong>】进行过滤，源站组形如：origin-xxxxx。<br>   类型：String<br>   必选：否</li>
-<li>flowType<br>   按照【<strong>源站响应类型</strong>】进行过滤，优先级高于 MetricNames.N 参数。<br>   类型：String<br>   必选：否<br>   可选项：<br>   inFlow：源站响应流量，对应MetricNames中l7Flow_inFlux_hy、l7Flow_inBandwidth_hy、l7Flow_request_hy三个指标；<br>   outFlow：EdgeOne请求流量，对应MetricNames中l7Flow_outFlux_hy、l7Flow_outBandwidth_hy、l7Flow_request_hy三个指标。</li>
-        :type Filters: list of QueryCondition
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据；</li>
-<li>global：全球数据。</li>不填默认取值为global。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._MetricNames = None
-        self._ZoneIds = None
-        self._Interval = None
-        self._Filters = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def MetricNames(self):
-        return self._MetricNames
-
-    @MetricNames.setter
-    def MetricNames(self, MetricNames):
-        self._MetricNames = MetricNames
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._MetricNames = params.get("MetricNames")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Interval = params.get("Interval")
-        if params.get("Filters") is not None:
-            self._Filters = []
-            for item in params.get("Filters"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._Filters.append(obj)
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeTimingL7SourceDataResponse(AbstractModel):
-    """DescribeTimingL7SourceData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _TimingDataRecords: 时序流量数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TimingDataRecords: list of TimingDataRecord
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._TotalCount = None
-        self._TimingDataRecords = None
-        self._RequestId = None
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def TimingDataRecords(self):
-        return self._TimingDataRecords
-
-    @TimingDataRecords.setter
-    def TimingDataRecords(self, TimingDataRecords):
-        self._TimingDataRecords = TimingDataRecords
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._TotalCount = params.get("TotalCount")
-        if params.get("TimingDataRecords") is not None:
-            self._TimingDataRecords = []
-            for item in params.get("TimingDataRecords"):
-                obj = TimingDataRecord()
-                obj._deserialize(item)
-                self._TimingDataRecords.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeTopL7AnalysisDataRequest(AbstractModel):
     """DescribeTopL7AnalysisData请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10484,1379 +8887,14 @@
             for item in params.get("Data"):
                 obj = TopDataRecord()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeWebManagedRulesDataRequest(AbstractModel):
-    """DescribeWebManagedRulesData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _MetricNames: 统计指标列表，取值有：
-<li>waf_interceptNum：waf拦截次数。</li>
-        :type MetricNames: list of str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 子域名集合，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action：执行动作。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Interval: 查询时间粒度，取值有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._MetricNames = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._QueryCondition = None
-        self._Interval = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def MetricNames(self):
-        return self._MetricNames
-
-    @MetricNames.setter
-    def MetricNames(self, MetricNames):
-        self._MetricNames = MetricNames
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._MetricNames = params.get("MetricNames")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Interval = params.get("Interval")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebManagedRulesDataResponse(AbstractModel):
-    """DescribeWebManagedRulesData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: WAF攻击的时序数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SecEntry
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SecEntry()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebManagedRulesHitRuleDetailRequest(AbstractModel):
-    """DescribeWebManagedRulesHitRuleDetail请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 子域名列表，不填默认选择全部全部子域名。
-        :type Domains: list of str
-        :param _Interval: 查询时间粒度，取值有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天 。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action ：执行动作 。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._Interval = None
-        self._QueryCondition = None
-        self._Limit = None
-        self._Offset = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        self._Interval = params.get("Interval")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebManagedRulesHitRuleDetailResponse(AbstractModel):
-    """DescribeWebManagedRulesHitRuleDetail返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: 命中规则的详细列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SecHitRuleInfo
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SecHitRuleInfo()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebManagedRulesLogRequest(AbstractModel):
-    """DescribeWebManagedRulesLog请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 域名集合，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>attackType：攻击类型；</li>
-<li>riskLevel：风险等级；</li>
-<li>action：执行动作（处置方式）；</li>
-<li>ruleId：规则id；</li>
-<li>sipCountryCode：ip所在国家；</li>
-<li>attackIp：攻击ip；</li>
-<li>realClientIp：真实客户端ip；</li>
-<li>oriDomain：被攻击的子域名；</li>
-<li>eventId：事件id；</li>
-<li>ua：用户代理；</li>
-<li>requestMethod：请求方法；</li>
-<li>uri：统一资源标识符。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._Limit = None
-        self._Offset = None
-        self._QueryCondition = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebManagedRulesLogResponse(AbstractModel):
-    """DescribeWebManagedRulesLog返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: Web攻击日志数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of WebLogs
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = WebLogs()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebProtectionClientIpListRequest(AbstractModel):
-    """DescribeWebProtectionClientIpList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 域名集合，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _Interval: 查询的时间粒度，支持的粒度有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action：执行动作。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._Interval = None
-        self._QueryCondition = None
-        self._Limit = None
-        self._Offset = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        self._Interval = params.get("Interval")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebProtectionClientIpListResponse(AbstractModel):
-    """DescribeWebProtectionClientIpList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: CC防护客户端（攻击源）ip信息列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SecClientIp
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SecClientIp()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebProtectionDataRequest(AbstractModel):
-    """DescribeWebProtectionData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _MetricNames: 统计指标，取值有：
-<li>ccRate_interceptNum：速率限制规则限制次数；</li>
-<li>ccAcl_interceptNum：自定义规则拦截次数。</li>
-        :type MetricNames: list of str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 域名集合，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _Interval: 查询时间粒度，支持的时间粒度有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action：执行动作。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._MetricNames = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._Interval = None
-        self._QueryCondition = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def MetricNames(self):
-        return self._MetricNames
-
-    @MetricNames.setter
-    def MetricNames(self, MetricNames):
-        self._MetricNames = MetricNames
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._MetricNames = params.get("MetricNames")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        self._Interval = params.get("Interval")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebProtectionDataResponse(AbstractModel):
-    """DescribeWebProtectionData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: CC防护时序数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SecEntry
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SecEntry()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebProtectionHitRuleDetailRequest(AbstractModel):
-    """DescribeWebProtectionHitRuleDetail请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _EntityType: 所属规则数据类型，支持的规则有：
-<li>rate：限速规则；</li>
-<li>acl：自定义规则。</li>
-        :type EntityType: str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 域名列表，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action：执行动作。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Limit: 分页查询的限制数目，默认值为20，最大查询条目为1000。
-        :type Limit: int
-        :param _Offset: 分页的偏移量，默认值为0。
-        :type Offset: int
-        :param _Interval: 查询时间粒度，支持的时间粒度有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._EntityType = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._QueryCondition = None
-        self._Limit = None
-        self._Offset = None
-        self._Interval = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def EntityType(self):
-        return self._EntityType
-
-    @EntityType.setter
-    def EntityType(self, EntityType):
-        self._EntityType = EntityType
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._EntityType = params.get("EntityType")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Limit = params.get("Limit")
-        self._Offset = params.get("Offset")
-        self._Interval = params.get("Interval")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebProtectionHitRuleDetailResponse(AbstractModel):
-    """DescribeWebProtectionHitRuleDetail返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: cc防护命中规则列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of SecHitRuleInfo
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = SecHitRuleInfo()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
-class DescribeWebProtectionTopDataRequest(AbstractModel):
-    """DescribeWebProtectionTopData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _MetricName: 统计指标列表，取值有：
-<li>ccRate_requestNum_url：速率限制规则请求次数url分布排行；</li>
-<li>ccRate_cipRequestNum_region：速率限制规则请求次数区域客户端ip分布排行；</li>
-<li>ccAcl_requestNum_url：自定义规则请求次数url分布排行；</li>
-<li>ccAcl_requestNum_cip：自定义规则请求次数客户端ip分布排行；</li>
-<li>ccAcl_cipRequestNum_region：自定义规则请求次数客户端区域分布排行。</li>
-        :type MetricName: str
-        :param _Interval: 查询时间粒度，取值有：
-<li>min：1分钟；</li>
-<li>5min：5分钟；</li>
-<li>hour：1小时；</li>
-<li>day：1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
-        :type Interval: str
-        :param _ZoneIds: 站点集合，不填默认选择全部站点。
-        :type ZoneIds: list of str
-        :param _Domains: 域名集合，不填默认选择全部子域名。
-        :type Domains: list of str
-        :param _Limit: 查询前多少个数据，不填默认默认为10， 表示查询前top 10的数据。
-        :type Limit: int
-        :param _QueryCondition: 筛选条件，key可选的值有：
-<li>action：执行动作 。</li>
-        :type QueryCondition: list of QueryCondition
-        :param _Area: 数据归属地区，取值有：
-<li>overseas：全球（除中国大陆地区）数据；</li>
-<li>mainland：中国大陆地区数据。</li>不填将根据用户所在地智能选择地区。
-        :type Area: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._MetricName = None
-        self._Interval = None
-        self._ZoneIds = None
-        self._Domains = None
-        self._Limit = None
-        self._QueryCondition = None
-        self._Area = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def MetricName(self):
-        return self._MetricName
-
-    @MetricName.setter
-    def MetricName(self, MetricName):
-        self._MetricName = MetricName
-
-    @property
-    def Interval(self):
-        return self._Interval
-
-    @Interval.setter
-    def Interval(self, Interval):
-        self._Interval = Interval
-
-    @property
-    def ZoneIds(self):
-        return self._ZoneIds
-
-    @ZoneIds.setter
-    def ZoneIds(self, ZoneIds):
-        self._ZoneIds = ZoneIds
-
-    @property
-    def Domains(self):
-        return self._Domains
-
-    @Domains.setter
-    def Domains(self, Domains):
-        self._Domains = Domains
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def QueryCondition(self):
-        return self._QueryCondition
-
-    @QueryCondition.setter
-    def QueryCondition(self, QueryCondition):
-        self._QueryCondition = QueryCondition
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._MetricName = params.get("MetricName")
-        self._Interval = params.get("Interval")
-        self._ZoneIds = params.get("ZoneIds")
-        self._Domains = params.get("Domains")
-        self._Limit = params.get("Limit")
-        if params.get("QueryCondition") is not None:
-            self._QueryCondition = []
-            for item in params.get("QueryCondition"):
-                obj = QueryCondition()
-                obj._deserialize(item)
-                self._QueryCondition.append(obj)
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeWebProtectionTopDataResponse(AbstractModel):
-    """DescribeWebProtectionTopData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Data: CC防护的TopN数据列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: list of TopEntry
-        :param _TotalCount: 查询结果的总条数。
-        :type TotalCount: int
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Data = None
-        self._TotalCount = None
-        self._RequestId = None
-
-    @property
-    def Data(self):
-        return self._Data
-
-    @Data.setter
-    def Data(self, Data):
-        self._Data = Data
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self._Data = []
-            for item in params.get("Data"):
-                obj = TopEntry()
-                obj._deserialize(item)
-                self._Data.append(obj)
-        self._TotalCount = params.get("TotalCount")
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeZoneSettingRequest(AbstractModel):
     """DescribeZoneSetting请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12490,104 +9528,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DistrictStatistics(AbstractModel):
-    """拨测分地域统计数据
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Alpha2: ISO 3166-2 国家/地区简写，详情请参考[ISO 3166-2](https://zh.m.wikipedia.org/zh-hans/ISO_3166-2)。
-        :type Alpha2: str
-        :param _LoadTime: 整体拨测用时，单位ms。
-        :type LoadTime: int
-        """
-        self._Alpha2 = None
-        self._LoadTime = None
-
-    @property
-    def Alpha2(self):
-        return self._Alpha2
-
-    @Alpha2.setter
-    def Alpha2(self, Alpha2):
-        self._Alpha2 = Alpha2
-
-    @property
-    def LoadTime(self):
-        return self._LoadTime
-
-    @LoadTime.setter
-    def LoadTime(self, LoadTime):
-        self._LoadTime = LoadTime
-
-
-    def _deserialize(self, params):
-        self._Alpha2 = params.get("Alpha2")
-        self._LoadTime = params.get("LoadTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DnsData(AbstractModel):
-    """Dns统计曲线数据项
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Time: 时间。
-        :type Time: str
-        :param _Value: 数值。
-        :type Value: int
-        """
-        self._Time = None
-        self._Value = None
-
-    @property
-    def Time(self):
-        return self._Time
-
-    @Time.setter
-    def Time(self, Time):
-        self._Time = Time
-
-    @property
-    def Value(self):
-        return self._Value
-
-    @Value.setter
-    def Value(self, Value):
-        self._Value = Value
-
-
-    def _deserialize(self, params):
-        self._Time = params.get("Time")
-        self._Value = params.get("Value")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class DownloadL4LogsRequest(AbstractModel):
     """DownloadL4Logs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14839,85 +11787,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class LogSetInfo(AbstractModel):
-    """日志集基本信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _LogSetRegion: 日志集所属地区。
-        :type LogSetRegion: str
-        :param _LogSetName: 日志集名
-        :type LogSetName: str
-        :param _LogSetId: 日志集Id
-        :type LogSetId: str
-        :param _Deleted: 该日志集是否已被删除, 可选的值有：
-<li>no: 日志集没有被删除；</li>
-<li>yes: 日志集已经被删除；</li>
-        :type Deleted: str
-        """
-        self._LogSetRegion = None
-        self._LogSetName = None
-        self._LogSetId = None
-        self._Deleted = None
-
-    @property
-    def LogSetRegion(self):
-        return self._LogSetRegion
-
-    @LogSetRegion.setter
-    def LogSetRegion(self, LogSetRegion):
-        self._LogSetRegion = LogSetRegion
-
-    @property
-    def LogSetName(self):
-        return self._LogSetName
-
-    @LogSetName.setter
-    def LogSetName(self, LogSetName):
-        self._LogSetName = LogSetName
-
-    @property
-    def LogSetId(self):
-        return self._LogSetId
-
-    @LogSetId.setter
-    def LogSetId(self, LogSetId):
-        self._LogSetId = LogSetId
-
-    @property
-    def Deleted(self):
-        return self._Deleted
-
-    @Deleted.setter
-    def Deleted(self, Deleted):
-        self._Deleted = Deleted
-
-
-    def _deserialize(self, params):
-        self._LogSetRegion = params.get("LogSetRegion")
-        self._LogSetName = params.get("LogSetName")
-        self._LogSetId = params.get("LogSetId")
-        self._Deleted = params.get("Deleted")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class MaxAge(AbstractModel):
     """浏览器缓存规则配置，用于设置 MaxAge 默认值，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
@@ -15512,28 +12389,31 @@
 <li>PPV2：Proxy Protocol传递，协议版本V2；</li>
 <li>OFF：不传递。</li>不填保持原有值。
         :type ForwardClientIp: str
         :param _SessionPersist: 是否开启会话保持，取值有：
 <li>true：开启；</li>
 <li>false：关闭。</li>不填为false。
         :type SessionPersist: bool
+        :param _SessionPersistTime: 会话保持的时间，只有当SessionPersist为true时，该值才会生效。
+        :type SessionPersistTime: int
         :param _OriginPort: 源站端口，支持格式：
 <li>单端口：80；</li>
 <li>端口段：81-90，81至90端口。</li>
         :type OriginPort: str
         """
         self._ZoneId = None
         self._ProxyId = None
         self._RuleId = None
         self._OriginType = None
         self._Port = None
         self._Proto = None
         self._OriginValue = None
         self._ForwardClientIp = None
         self._SessionPersist = None
+        self._SessionPersistTime = None
         self._OriginPort = None
 
     @property
     def ZoneId(self):
         return self._ZoneId
 
     @ZoneId.setter
@@ -15601,14 +12481,22 @@
         return self._SessionPersist
 
     @SessionPersist.setter
     def SessionPersist(self, SessionPersist):
         self._SessionPersist = SessionPersist
 
     @property
+    def SessionPersistTime(self):
+        return self._SessionPersistTime
+
+    @SessionPersistTime.setter
+    def SessionPersistTime(self, SessionPersistTime):
+        self._SessionPersistTime = SessionPersistTime
+
+    @property
     def OriginPort(self):
         return self._OriginPort
 
     @OriginPort.setter
     def OriginPort(self, OriginPort):
         self._OriginPort = OriginPort
 
@@ -15619,14 +12507,15 @@
         self._RuleId = params.get("RuleId")
         self._OriginType = params.get("OriginType")
         self._Port = params.get("Port")
         self._Proto = params.get("Proto")
         self._OriginValue = params.get("OriginValue")
         self._ForwardClientIp = params.get("ForwardClientIp")
         self._SessionPersist = params.get("SessionPersist")
+        self._SessionPersistTime = params.get("SessionPersistTime")
         self._OriginPort = params.get("OriginPort")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
@@ -15835,98 +12724,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class ModifyDefaultCertificateRequest(AbstractModel):
-    """ModifyDefaultCertificate请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _CertId: 默认证书ID。
-        :type CertId: str
-        :param _Status: 证书状态，取值有：
-<li>deployed ：部署证书；</li>
-<li>disabled ：禁用证书。</li>失败状态下重新deployed即可重试。
-        :type Status: str
-        """
-        self._ZoneId = None
-        self._CertId = None
-        self._Status = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def CertId(self):
-        return self._CertId
-
-    @CertId.setter
-    def CertId(self, CertId):
-        self._CertId = CertId
-
-    @property
-    def Status(self):
-        return self._Status
-
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._CertId = params.get("CertId")
-        self._Status = params.get("Status")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ModifyDefaultCertificateResponse(AbstractModel):
-    """ModifyDefaultCertificate返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class ModifyHostsCertificateRequest(AbstractModel):
     """ModifyHostsCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -16162,84 +12967,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class ModifyRulePriorityRequest(AbstractModel):
-    """ModifyRulePriority请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点 ID。
-        :type ZoneId: str
-        :param _RuleIds: 规则 ID 的顺序，多条规则执行顺序依次往下。
-        :type RuleIds: list of str
-        """
-        self._ZoneId = None
-        self._RuleIds = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def RuleIds(self):
-        return self._RuleIds
-
-    @RuleIds.setter
-    def RuleIds(self, RuleIds):
-        self._RuleIds = RuleIds
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._RuleIds = params.get("RuleIds")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ModifyRulePriorityResponse(AbstractModel):
-    """ModifyRulePriority返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class ModifyRuleRequest(AbstractModel):
     """ModifyRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -16552,208 +13287,45 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class ModifySecurityWafGroupPolicyRequest(AbstractModel):
-    """ModifySecurityWafGroupPolicy请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点Id。当使用ZoneId和Entity时可不填写TemplateId，否则必须填写TemplateId。
-        :type ZoneId: str
-        :param _Entity: 子域名。当使用ZoneId和Entity时可不填写TemplateId，否则必须填写TemplateId。
-        :type Entity: str
-        :param _Switch: 总开关，取值有：
-<li>on：开启；</li>
-<li>off：关闭。</li>不填默认为上次的配置。
-        :type Switch: str
-        :param _Level: 规则等级，取值有：
-<li> loose：宽松；</li>
-<li> normal：正常；</li>
-<li> strict：严格；</li>
-<li> stricter：超严格；</li>
-<li> custom：自定义。</li>不填默认为上次的配置。
-        :type Level: str
-        :param _Mode: 处置方式，取值有：
-<li> block：阻断；</li>
-<li> observe：观察。</li>不填默认为上次的配置。
-        :type Mode: str
-        :param _WafRules: 托管规则。不填默认为上次的配置。
-        :type WafRules: :class:`tencentcloud.teo.v20220901.models.WafRule`
-        :param _AiRule: AI引擎模式。不填默认为上次的配置。
-        :type AiRule: :class:`tencentcloud.teo.v20220901.models.AiRule`
-        :param _WafGroups: 托管规则等级组。不填默认为上次的配置。
-        :type WafGroups: list of WafGroup
-        :param _TemplateId: 模板Id。当使用模板Id时可不填ZoneId和Entity，否则必须填写ZoneId和Entity。
-        :type TemplateId: str
-        """
-        self._ZoneId = None
-        self._Entity = None
-        self._Switch = None
-        self._Level = None
-        self._Mode = None
-        self._WafRules = None
-        self._AiRule = None
-        self._WafGroups = None
-        self._TemplateId = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def Entity(self):
-        return self._Entity
-
-    @Entity.setter
-    def Entity(self, Entity):
-        self._Entity = Entity
-
-    @property
-    def Switch(self):
-        return self._Switch
-
-    @Switch.setter
-    def Switch(self, Switch):
-        self._Switch = Switch
-
-    @property
-    def Level(self):
-        return self._Level
-
-    @Level.setter
-    def Level(self, Level):
-        self._Level = Level
-
-    @property
-    def Mode(self):
-        return self._Mode
-
-    @Mode.setter
-    def Mode(self, Mode):
-        self._Mode = Mode
-
-    @property
-    def WafRules(self):
-        return self._WafRules
-
-    @WafRules.setter
-    def WafRules(self, WafRules):
-        self._WafRules = WafRules
-
-    @property
-    def AiRule(self):
-        return self._AiRule
-
-    @AiRule.setter
-    def AiRule(self, AiRule):
-        self._AiRule = AiRule
-
-    @property
-    def WafGroups(self):
-        return self._WafGroups
-
-    @WafGroups.setter
-    def WafGroups(self, WafGroups):
-        self._WafGroups = WafGroups
-
-    @property
-    def TemplateId(self):
-        return self._TemplateId
-
-    @TemplateId.setter
-    def TemplateId(self, TemplateId):
-        self._TemplateId = TemplateId
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._Entity = params.get("Entity")
-        self._Switch = params.get("Switch")
-        self._Level = params.get("Level")
-        self._Mode = params.get("Mode")
-        if params.get("WafRules") is not None:
-            self._WafRules = WafRule()
-            self._WafRules._deserialize(params.get("WafRules"))
-        if params.get("AiRule") is not None:
-            self._AiRule = AiRule()
-            self._AiRule._deserialize(params.get("AiRule"))
-        if params.get("WafGroups") is not None:
-            self._WafGroups = []
-            for item in params.get("WafGroups"):
-                obj = WafGroup()
-                obj._deserialize(item)
-                self._WafGroups.append(obj)
-        self._TemplateId = params.get("TemplateId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ModifySecurityWafGroupPolicyResponse(AbstractModel):
-    """ModifySecurityWafGroupPolicy返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class ModifyZoneRequest(AbstractModel):
     """ModifyZone请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _ZoneId: 站点 ID。
         :type ZoneId: str
         :param _Type: 站点接入方式，取值有：
 <li> full：NS 接入；</li>
-<li> partial：CNAME 接入。</li>不填写保持原有配置。
+<li> partial：CNAME 接入，如果站点当前是无域名接入，仅支持切换到CNAME接入。</li>不填写保持原有配置。
         :type Type: str
-        :param _VanityNameServers: 自定义站点信息，以替代系统默认分配的名称服务器。不填写保持原有配置。
+        :param _VanityNameServers: 自定义站点信息，以替代系统默认分配的名称服务器。不填写保持原有配置。当站点是无域名接入方式时不允许传此参数。
         :type VanityNameServers: :class:`tencentcloud.teo.v20220901.models.VanityNameServers`
         :param _AliasZoneName: 站点别名。数字、英文、-和_组合，限制20个字符。
         :type AliasZoneName: str
+        :param _Area: 站点接入地域，取值有：
+<li> global：全球；</li>
+<li> mainland：中国大陆；</li>
+<li> overseas：境外区域。</li>当站点是无域名接入方式时，不允许传此参数。
+        :type Area: str
+        :param _ZoneName: 站点名称。仅当站点由无域名接入方式切换到CNAME接入方式的场景下有效。
+        :type ZoneName: str
         """
         self._ZoneId = None
         self._Type = None
         self._VanityNameServers = None
         self._AliasZoneName = None
+        self._Area = None
+        self._ZoneName = None
 
     @property
     def ZoneId(self):
         return self._ZoneId
 
     @ZoneId.setter
     def ZoneId(self, ZoneId):
@@ -16779,22 +13351,40 @@
     def AliasZoneName(self):
         return self._AliasZoneName
 
     @AliasZoneName.setter
     def AliasZoneName(self, AliasZoneName):
         self._AliasZoneName = AliasZoneName
 
+    @property
+    def Area(self):
+        return self._Area
+
+    @Area.setter
+    def Area(self, Area):
+        self._Area = Area
+
+    @property
+    def ZoneName(self):
+        return self._ZoneName
+
+    @ZoneName.setter
+    def ZoneName(self, ZoneName):
+        self._ZoneName = ZoneName
+
 
     def _deserialize(self, params):
         self._ZoneId = params.get("ZoneId")
         self._Type = params.get("Type")
         if params.get("VanityNameServers") is not None:
             self._VanityNameServers = VanityNameServers()
             self._VanityNameServers._deserialize(params.get("VanityNameServers"))
         self._AliasZoneName = params.get("AliasZoneName")
+        self._Area = params.get("Area")
+        self._ZoneName = params.get("ZoneName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -16888,14 +13478,16 @@
         :type ClientIpCountry: :class:`tencentcloud.teo.v20220901.models.ClientIpCountry`
         :param _Grpc: Grpc 协议支持配置。
 不填写表示保持原有配置。
         :type Grpc: :class:`tencentcloud.teo.v20220901.models.Grpc`
         :param _ImageOptimize: 图片优化配置。
 不填写表示关闭。
         :type ImageOptimize: :class:`tencentcloud.teo.v20220901.models.ImageOptimize`
+        :param _StandardDebug: 标准 Debug 配置。
+        :type StandardDebug: :class:`tencentcloud.teo.v20220901.models.StandardDebug`
         """
         self._ZoneId = None
         self._CacheConfig = None
         self._CacheKey = None
         self._MaxAge = None
         self._OfflineCache = None
         self._Quic = None
@@ -16909,14 +13501,15 @@
         self._WebSocket = None
         self._ClientIpHeader = None
         self._CachePrefresh = None
         self._Ipv6 = None
         self._ClientIpCountry = None
         self._Grpc = None
         self._ImageOptimize = None
+        self._StandardDebug = None
 
     @property
     def ZoneId(self):
         return self._ZoneId
 
     @ZoneId.setter
     def ZoneId(self, ZoneId):
@@ -17070,14 +13663,22 @@
     def ImageOptimize(self):
         return self._ImageOptimize
 
     @ImageOptimize.setter
     def ImageOptimize(self, ImageOptimize):
         self._ImageOptimize = ImageOptimize
 
+    @property
+    def StandardDebug(self):
+        return self._StandardDebug
+
+    @StandardDebug.setter
+    def StandardDebug(self, StandardDebug):
+        self._StandardDebug = StandardDebug
+
 
     def _deserialize(self, params):
         self._ZoneId = params.get("ZoneId")
         if params.get("CacheConfig") is not None:
             self._CacheConfig = CacheConfig()
             self._CacheConfig._deserialize(params.get("CacheConfig"))
         if params.get("CacheKey") is not None:
@@ -17130,14 +13731,17 @@
             self._ClientIpCountry._deserialize(params.get("ClientIpCountry"))
         if params.get("Grpc") is not None:
             self._Grpc = Grpc()
             self._Grpc._deserialize(params.get("Grpc"))
         if params.get("ImageOptimize") is not None:
             self._ImageOptimize = ImageOptimize()
             self._ImageOptimize._deserialize(params.get("ImageOptimize"))
+        if params.get("StandardDebug") is not None:
+            self._StandardDebug = StandardDebug()
+            self._StandardDebug._deserialize(params.get("StandardDebug"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -17357,86 +13961,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class OptimizeAction(AbstractModel):
-    """站点拨测优化建议
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Name: 站点性能优化配置项，取值有：
-<li>Http2；</li>
-<li>Http3；</li>
-<li>Brotli。</li>
-        :type Name: str
-        :param _Connectivity: 网络环境。
-        :type Connectivity: str
-        :param _Value: 开启配置项后，预估性能优化效果，单位ms。
-        :type Value: int
-        :param _Ratio: 开启配置项后，预估性能提升比例，单位%。
-        :type Ratio: int
-        """
-        self._Name = None
-        self._Connectivity = None
-        self._Value = None
-        self._Ratio = None
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def Connectivity(self):
-        return self._Connectivity
-
-    @Connectivity.setter
-    def Connectivity(self, Connectivity):
-        self._Connectivity = Connectivity
-
-    @property
-    def Value(self):
-        return self._Value
-
-    @Value.setter
-    def Value(self, Value):
-        self._Value = Value
-
-    @property
-    def Ratio(self):
-        return self._Ratio
-
-    @Ratio.setter
-    def Ratio(self, Ratio):
-        self._Ratio = Ratio
-
-
-    def _deserialize(self, params):
-        self._Name = params.get("Name")
-        self._Connectivity = params.get("Connectivity")
-        self._Value = params.get("Value")
-        self._Ratio = params.get("Ratio")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class Origin(AbstractModel):
     """源站配置。
 
     """
 
     def __init__(self):
         r"""
@@ -17778,14 +14310,15 @@
     def __init__(self):
         r"""
         :param _OriginType: 源站类型，取值有：
 <li>IP_DOMAIN：IPV4、IPV6或域名类型源站；</li>
 <li>COS：COS源。</li>
 <li>ORIGIN_GROUP：源站组类型源站。</li>
 <li>AWS_S3：AWS S3对象存储源站。</li>
+<li>SPACE：Edgeone源站Space存储，Space存储不允许配置该类型源站。</li>
         :type OriginType: str
         :param _Origin: 源站地址，当OriginType参数指定为ORIGIN_GROUP时，该参数填写源站组ID，其他情况下填写源站地址。
         :type Origin: str
         :param _BackupOrigin: 备用源站组ID，该参数在OriginType参数指定为ORIGIN_GROUP时生效，为空表示不使用备用源站。
         :type BackupOrigin: str
         :param _PrivateAccess: 指定是否允许访问私有对象存储源站，当源站类型OriginType=COS或AWS_S3时有效，取值有：
 <li>on：使用私有鉴权；</li>
@@ -19172,142 +15705,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ReclaimAliasDomainRequest(AbstractModel):
-    """ReclaimAliasDomain请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点 ID。
-        :type ZoneId: str
-        :param _ZoneName: 站点名称。
-        :type ZoneName: str
-        """
-        self._ZoneId = None
-        self._ZoneName = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def ZoneName(self):
-        return self._ZoneName
-
-    @ZoneName.setter
-    def ZoneName(self, ZoneName):
-        self._ZoneName = ZoneName
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._ZoneName = params.get("ZoneName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ReclaimAliasDomainResponse(AbstractModel):
-    """ReclaimAliasDomain返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
-class ReclaimZoneRequest(AbstractModel):
-    """ReclaimZone请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneName: 站点名称。
-        :type ZoneName: str
-        """
-        self._ZoneName = None
-
-    @property
-    def ZoneName(self):
-        return self._ZoneName
-
-    @ZoneName.setter
-    def ZoneName(self, ZoneName):
-        self._ZoneName = ZoneName
-
-
-    def _deserialize(self, params):
-        self._ZoneName = params.get("ZoneName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ReclaimZoneResponse(AbstractModel):
-    """ReclaimZone返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class Resource(AbstractModel):
     """计费资源
 
     """
 
     def __init__(self):
         r"""
@@ -19337,25 +15742,36 @@
         :param _PlanId: 套餐关联资源 ID。
         :type PlanId: str
         :param _Area: 地域，取值有：
 <li>mainland：国内；</li>
 <li>overseas：海外。</li>
 <li>global：全球。</li>
         :type Area: str
+        :param _Group: 资源类型，取值有：
+<li>plan：套餐类型；</li>
+<li>pay-as-you-go：后付费类型。</li>
+<li>value-added：增值服务类型。</li>
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Group: str
+        :param _ZoneNumber: 当前资源绑定的站点数量。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ZoneNumber: int
         """
         self._Id = None
         self._PayMode = None
         self._CreateTime = None
         self._EnableTime = None
         self._ExpireTime = None
         self._Status = None
         self._Sv = None
         self._AutoRenewFlag = None
         self._PlanId = None
         self._Area = None
+        self._Group = None
+        self._ZoneNumber = None
 
     @property
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
@@ -19429,14 +15845,30 @@
     def Area(self):
         return self._Area
 
     @Area.setter
     def Area(self, Area):
         self._Area = Area
 
+    @property
+    def Group(self):
+        return self._Group
+
+    @Group.setter
+    def Group(self, Group):
+        self._Group = Group
+
+    @property
+    def ZoneNumber(self):
+        return self._ZoneNumber
+
+    @ZoneNumber.setter
+    def ZoneNumber(self, ZoneNumber):
+        self._ZoneNumber = ZoneNumber
+
 
     def _deserialize(self, params):
         self._Id = params.get("Id")
         self._PayMode = params.get("PayMode")
         self._CreateTime = params.get("CreateTime")
         self._EnableTime = params.get("EnableTime")
         self._ExpireTime = params.get("ExpireTime")
@@ -19446,14 +15878,16 @@
             for item in params.get("Sv"):
                 obj = Sv()
                 obj._deserialize(item)
                 self._Sv.append(obj)
         self._AutoRenewFlag = params.get("AutoRenewFlag")
         self._PlanId = params.get("PlanId")
         self._Area = params.get("Area")
+        self._Group = params.get("Group")
+        self._ZoneNumber = params.get("ZoneNumber")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -20406,71 +16840,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class SecClientIp(AbstractModel):
-    """客户端ip信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ClientIp: 客户端ip。
-        :type ClientIp: str
-        :param _RequestMaxQps: 最大qps。
-        :type RequestMaxQps: int
-        :param _RequestNum: 请求数。
-        :type RequestNum: int
-        """
-        self._ClientIp = None
-        self._RequestMaxQps = None
-        self._RequestNum = None
-
-    @property
-    def ClientIp(self):
-        return self._ClientIp
-
-    @ClientIp.setter
-    def ClientIp(self, ClientIp):
-        self._ClientIp = ClientIp
-
-    @property
-    def RequestMaxQps(self):
-        return self._RequestMaxQps
-
-    @RequestMaxQps.setter
-    def RequestMaxQps(self, RequestMaxQps):
-        self._RequestMaxQps = RequestMaxQps
-
-    @property
-    def RequestNum(self):
-        return self._RequestNum
-
-    @RequestNum.setter
-    def RequestNum(self, RequestNum):
-        self._RequestNum = RequestNum
-
-
-    def _deserialize(self, params):
-        self._ClientIp = params.get("ClientIp")
-        self._RequestMaxQps = params.get("RequestMaxQps")
-        self._RequestNum = params.get("RequestNum")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class SecEntry(AbstractModel):
     """安全数据Entry返回值
 
     """
 
     def __init__(self):
         r"""
@@ -20599,365 +16976,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class SecHitRuleInfo(AbstractModel):
-    """命中规则信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _RuleId: 规则ID。
-        :type RuleId: int
-        :param _RuleTypeName: 规则类型名称。
-        :type RuleTypeName: str
-        :param _HitTime: 命中时间，采用unix秒级时间戳。
-        :type HitTime: int
-        :param _RequestNum: 请求数。
-        :type RequestNum: int
-        :param _Description: 规则描述。
-        :type Description: str
-        :param _Domain: 子域名。
-        :type Domain: str
-        :param _Action: 执行动作（处置方式），取值有：
-<li>trans ：通过 ；</li>
-<li>alg ：算法挑战 ；</li>
-<li>drop ：丢弃 ；</li>
-<li>ban ：封禁源ip ；</li>
-<li>redirect ：重定向 ；</li>
-<li>page ：返回指定页面 ；</li>
-<li>monitor ：观察 。</li>
-        :type Action: str
-        :param _BotLabel: Bot标签，取值有:
-<li>evil_bot：恶意Bot；</li>
-<li>suspect_bot：疑似Bot；</li>
-<li>good_bot：正常Bot；</li>
-<li>normal：正常请求；</li>
-<li>none：未分类。</li>
-        :type BotLabel: str
-        :param _RuleEnabled: 规则是否启用。
-        :type RuleEnabled: bool
-        :param _AlarmEnabled: 规则是否启用监控告警。
-        :type AlarmEnabled: bool
-        :param _RuleDeleted: 规则是否存在，取值有：
-<li>true: 规则不存在；</li>
-<li>false: 规则存在。</li>
-        :type RuleDeleted: bool
-        """
-        self._ZoneId = None
-        self._RuleId = None
-        self._RuleTypeName = None
-        self._HitTime = None
-        self._RequestNum = None
-        self._Description = None
-        self._Domain = None
-        self._Action = None
-        self._BotLabel = None
-        self._RuleEnabled = None
-        self._AlarmEnabled = None
-        self._RuleDeleted = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def RuleId(self):
-        return self._RuleId
-
-    @RuleId.setter
-    def RuleId(self, RuleId):
-        self._RuleId = RuleId
-
-    @property
-    def RuleTypeName(self):
-        return self._RuleTypeName
-
-    @RuleTypeName.setter
-    def RuleTypeName(self, RuleTypeName):
-        self._RuleTypeName = RuleTypeName
-
-    @property
-    def HitTime(self):
-        return self._HitTime
-
-    @HitTime.setter
-    def HitTime(self, HitTime):
-        self._HitTime = HitTime
-
-    @property
-    def RequestNum(self):
-        return self._RequestNum
-
-    @RequestNum.setter
-    def RequestNum(self, RequestNum):
-        self._RequestNum = RequestNum
-
-    @property
-    def Description(self):
-        return self._Description
-
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
-
-    @property
-    def Domain(self):
-        return self._Domain
-
-    @Domain.setter
-    def Domain(self, Domain):
-        self._Domain = Domain
-
-    @property
-    def Action(self):
-        return self._Action
-
-    @Action.setter
-    def Action(self, Action):
-        self._Action = Action
-
-    @property
-    def BotLabel(self):
-        return self._BotLabel
-
-    @BotLabel.setter
-    def BotLabel(self, BotLabel):
-        self._BotLabel = BotLabel
-
-    @property
-    def RuleEnabled(self):
-        return self._RuleEnabled
-
-    @RuleEnabled.setter
-    def RuleEnabled(self, RuleEnabled):
-        self._RuleEnabled = RuleEnabled
-
-    @property
-    def AlarmEnabled(self):
-        return self._AlarmEnabled
-
-    @AlarmEnabled.setter
-    def AlarmEnabled(self, AlarmEnabled):
-        self._AlarmEnabled = AlarmEnabled
-
-    @property
-    def RuleDeleted(self):
-        return self._RuleDeleted
-
-    @RuleDeleted.setter
-    def RuleDeleted(self, RuleDeleted):
-        self._RuleDeleted = RuleDeleted
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._RuleId = params.get("RuleId")
-        self._RuleTypeName = params.get("RuleTypeName")
-        self._HitTime = params.get("HitTime")
-        self._RequestNum = params.get("RequestNum")
-        self._Description = params.get("Description")
-        self._Domain = params.get("Domain")
-        self._Action = params.get("Action")
-        self._BotLabel = params.get("BotLabel")
-        self._RuleEnabled = params.get("RuleEnabled")
-        self._AlarmEnabled = params.get("AlarmEnabled")
-        self._RuleDeleted = params.get("RuleDeleted")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SecRuleRelatedInfo(AbstractModel):
-    """安全规则（cc/waf/bot）相关信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RuleId: 规则ID。
-        :type RuleId: int
-        :param _Action: 执行动作（处置方式），取值有：
-<li>trans ：通过 ；</li>
-<li>alg ：算法挑战 ；</li>
-<li>drop ：丢弃 ；</li>
-<li>ban ：封禁源ip ；</li>
-<li>redirect ：重定向 ；</li>
-<li>page ：返回指定页面 ；</li>
-<li>monitor ：观察 。</li>
-        :type Action: str
-        :param _RiskLevel: 风险等级（waf日志中独有），取值有：
-<li>high risk ：高危 ；</li>
-<li>middle risk ：中危 ；</li>
-<li>low risk ：低危 ；</li>
-<li>unkonw ：未知 。</li>
-        :type RiskLevel: str
-        :param _RuleLevel: 规则等级，取值有：
-<li>normal  ：正常 。</li>
-        :type RuleLevel: str
-        :param _Description: 规则描述。
-        :type Description: str
-        :param _RuleTypeName: 规则类型名称。
-        :type RuleTypeName: str
-        :param _AttackContent: 攻击内容。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AttackContent: str
-        :param _RuleType: 规则类型，取值有：
-<li>waf: 托管规则；</li>
-<li>acl：自定义规则；</li>
-<li>rate：速率限制规则；</li>
-<li>bot：bot防护规则。</li>
-        :type RuleType: str
-        :param _RuleEnabled: 规则是否开启。
-        :type RuleEnabled: bool
-        :param _RuleDeleted: 规则是否存在，取值有：
-<li>true: 规则不存在；</li>
-<li>false: 规则存在。</li>
-        :type RuleDeleted: bool
-        :param _AlarmEnabled: 规则是否启用监控告警。
-        :type AlarmEnabled: bool
-        """
-        self._RuleId = None
-        self._Action = None
-        self._RiskLevel = None
-        self._RuleLevel = None
-        self._Description = None
-        self._RuleTypeName = None
-        self._AttackContent = None
-        self._RuleType = None
-        self._RuleEnabled = None
-        self._RuleDeleted = None
-        self._AlarmEnabled = None
-
-    @property
-    def RuleId(self):
-        return self._RuleId
-
-    @RuleId.setter
-    def RuleId(self, RuleId):
-        self._RuleId = RuleId
-
-    @property
-    def Action(self):
-        return self._Action
-
-    @Action.setter
-    def Action(self, Action):
-        self._Action = Action
-
-    @property
-    def RiskLevel(self):
-        return self._RiskLevel
-
-    @RiskLevel.setter
-    def RiskLevel(self, RiskLevel):
-        self._RiskLevel = RiskLevel
-
-    @property
-    def RuleLevel(self):
-        return self._RuleLevel
-
-    @RuleLevel.setter
-    def RuleLevel(self, RuleLevel):
-        self._RuleLevel = RuleLevel
-
-    @property
-    def Description(self):
-        return self._Description
-
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
-
-    @property
-    def RuleTypeName(self):
-        return self._RuleTypeName
-
-    @RuleTypeName.setter
-    def RuleTypeName(self, RuleTypeName):
-        self._RuleTypeName = RuleTypeName
-
-    @property
-    def AttackContent(self):
-        return self._AttackContent
-
-    @AttackContent.setter
-    def AttackContent(self, AttackContent):
-        self._AttackContent = AttackContent
-
-    @property
-    def RuleType(self):
-        return self._RuleType
-
-    @RuleType.setter
-    def RuleType(self, RuleType):
-        self._RuleType = RuleType
-
-    @property
-    def RuleEnabled(self):
-        return self._RuleEnabled
-
-    @RuleEnabled.setter
-    def RuleEnabled(self, RuleEnabled):
-        self._RuleEnabled = RuleEnabled
-
-    @property
-    def RuleDeleted(self):
-        return self._RuleDeleted
-
-    @RuleDeleted.setter
-    def RuleDeleted(self, RuleDeleted):
-        self._RuleDeleted = RuleDeleted
-
-    @property
-    def AlarmEnabled(self):
-        return self._AlarmEnabled
-
-    @AlarmEnabled.setter
-    def AlarmEnabled(self, AlarmEnabled):
-        self._AlarmEnabled = AlarmEnabled
-
-
-    def _deserialize(self, params):
-        self._RuleId = params.get("RuleId")
-        self._Action = params.get("Action")
-        self._RiskLevel = params.get("RiskLevel")
-        self._RuleLevel = params.get("RuleLevel")
-        self._Description = params.get("Description")
-        self._RuleTypeName = params.get("RuleTypeName")
-        self._AttackContent = params.get("AttackContent")
-        self._RuleType = params.get("RuleType")
-        self._RuleEnabled = params.get("RuleEnabled")
-        self._RuleDeleted = params.get("RuleDeleted")
-        self._AlarmEnabled = params.get("AlarmEnabled")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class SecurityConfig(AbstractModel):
     """安全配置
 
     """
 
     def __init__(self):
         r"""
@@ -21271,109 +17297,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class SingleDataRecord(AbstractModel):
-    """单值类数据记录
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TypeKey: 查询维度值。
-        :type TypeKey: str
-        :param _TypeValue: 查询维度下具体指标值。
-        :type TypeValue: list of SingleTypeValue
-        """
-        self._TypeKey = None
-        self._TypeValue = None
-
-    @property
-    def TypeKey(self):
-        return self._TypeKey
-
-    @TypeKey.setter
-    def TypeKey(self, TypeKey):
-        self._TypeKey = TypeKey
-
-    @property
-    def TypeValue(self):
-        return self._TypeValue
-
-    @TypeValue.setter
-    def TypeValue(self, TypeValue):
-        self._TypeValue = TypeValue
-
-
-    def _deserialize(self, params):
-        self._TypeKey = params.get("TypeKey")
-        if params.get("TypeValue") is not None:
-            self._TypeValue = []
-            for item in params.get("TypeValue"):
-                obj = SingleTypeValue()
-                obj._deserialize(item)
-                self._TypeValue.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SingleTypeValue(AbstractModel):
-    """单值指标数据
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _MetricName: 指标名。
-        :type MetricName: str
-        :param _DetailData: 指标值。
-        :type DetailData: int
-        """
-        self._MetricName = None
-        self._DetailData = None
-
-    @property
-    def MetricName(self):
-        return self._MetricName
-
-    @MetricName.setter
-    def MetricName(self, MetricName):
-        self._MetricName = MetricName
-
-    @property
-    def DetailData(self):
-        return self._DetailData
-
-    @DetailData.setter
-    def DetailData(self, DetailData):
-        self._DetailData = DetailData
-
-
-    def _deserialize(self, params):
-        self._MetricName = params.get("MetricName")
-        self._DetailData = params.get("DetailData")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class SkipCondition(AbstractModel):
     """例外规则的跳过匹配条件，即在例外时根据本匹配条件，略过指定字段及内容。
 
     """
 
     def __init__(self):
         r"""
@@ -21667,666 +17598,63 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class SpeedTestingConfig(AbstractModel):
-    """站点拨测配置
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TaskType: 任务类型，取值有：
-<li>1：页面性能;</li>
-<li>2：文件上传;</li>
-<li>3：文件下载;</li>
-<li>4：端口性能;</li>
-<li>5：网络质量;</li>
-<li>6：音视频体验。</li>
-        :type TaskType: int
-        :param _Url: 拨测 url。
-        :type Url: str
-        :param _UA: 拨测 UA。
-        :type UA: str
-        :param _Connectivity: 网络类型。
-        :type Connectivity: str
-        """
-        self._TaskType = None
-        self._Url = None
-        self._UA = None
-        self._Connectivity = None
-
-    @property
-    def TaskType(self):
-        return self._TaskType
-
-    @TaskType.setter
-    def TaskType(self, TaskType):
-        self._TaskType = TaskType
-
-    @property
-    def Url(self):
-        return self._Url
-
-    @Url.setter
-    def Url(self, Url):
-        self._Url = Url
-
-    @property
-    def UA(self):
-        return self._UA
-
-    @UA.setter
-    def UA(self, UA):
-        self._UA = UA
-
-    @property
-    def Connectivity(self):
-        return self._Connectivity
-
-    @Connectivity.setter
-    def Connectivity(self, Connectivity):
-        self._Connectivity = Connectivity
-
-
-    def _deserialize(self, params):
-        self._TaskType = params.get("TaskType")
-        self._Url = params.get("Url")
-        self._UA = params.get("UA")
-        self._Connectivity = params.get("Connectivity")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingDetailData(AbstractModel):
-    """拨测详细数据，包括各地域性能数据。
+class StandardDebug(AbstractModel):
+    """支持标准debug结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _ZoneName: 站点名称。
-        :type ZoneName: str
-        :param _DistrictStatistics: 地域性能数据。
-        :type DistrictStatistics: list of DistrictStatistics
-        """
-        self._ZoneId = None
-        self._ZoneName = None
-        self._DistrictStatistics = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def ZoneName(self):
-        return self._ZoneName
-
-    @ZoneName.setter
-    def ZoneName(self, ZoneName):
-        self._ZoneName = ZoneName
-
-    @property
-    def DistrictStatistics(self):
-        return self._DistrictStatistics
-
-    @DistrictStatistics.setter
-    def DistrictStatistics(self, DistrictStatistics):
-        self._DistrictStatistics = DistrictStatistics
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._ZoneName = params.get("ZoneName")
-        if params.get("DistrictStatistics") is not None:
-            self._DistrictStatistics = []
-            for item in params.get("DistrictStatistics"):
-                obj = DistrictStatistics()
-                obj._deserialize(item)
-                self._DistrictStatistics.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingInfo(AbstractModel):
-    """拨测结果信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StatusCode: 任务状态，取值有：
-<li> 200：任务完成;</li>
-<li> 100：任务进行中；</li>
-<li> 503: 任务失败。</li>
-        :type StatusCode: int
-        :param _TestId: 拨测任务 ID。
-        :type TestId: str
-        :param _SpeedTestingConfig: 拨测任务配置。
-        :type SpeedTestingConfig: :class:`tencentcloud.teo.v20220901.models.SpeedTestingConfig`
-        :param _SpeedTestingStatistics: 拨测任务统计结果。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type SpeedTestingStatistics: :class:`tencentcloud.teo.v20220901.models.SpeedTestingStatistics`
-        """
-        self._StatusCode = None
-        self._TestId = None
-        self._SpeedTestingConfig = None
-        self._SpeedTestingStatistics = None
-
-    @property
-    def StatusCode(self):
-        return self._StatusCode
-
-    @StatusCode.setter
-    def StatusCode(self, StatusCode):
-        self._StatusCode = StatusCode
-
-    @property
-    def TestId(self):
-        return self._TestId
-
-    @TestId.setter
-    def TestId(self, TestId):
-        self._TestId = TestId
-
-    @property
-    def SpeedTestingConfig(self):
-        return self._SpeedTestingConfig
-
-    @SpeedTestingConfig.setter
-    def SpeedTestingConfig(self, SpeedTestingConfig):
-        self._SpeedTestingConfig = SpeedTestingConfig
-
-    @property
-    def SpeedTestingStatistics(self):
-        return self._SpeedTestingStatistics
-
-    @SpeedTestingStatistics.setter
-    def SpeedTestingStatistics(self, SpeedTestingStatistics):
-        self._SpeedTestingStatistics = SpeedTestingStatistics
-
-
-    def _deserialize(self, params):
-        self._StatusCode = params.get("StatusCode")
-        self._TestId = params.get("TestId")
-        if params.get("SpeedTestingConfig") is not None:
-            self._SpeedTestingConfig = SpeedTestingConfig()
-            self._SpeedTestingConfig._deserialize(params.get("SpeedTestingConfig"))
-        if params.get("SpeedTestingStatistics") is not None:
-            self._SpeedTestingStatistics = SpeedTestingStatistics()
-            self._SpeedTestingStatistics._deserialize(params.get("SpeedTestingStatistics"))
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingMetricData(AbstractModel):
-    """不同维度的测速数据。
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        :param _ZoneName: 站点名称。
-        :type ZoneName: str
-        :param _OriginSpeedTestingInfo: 源站拨测信息。
-        :type OriginSpeedTestingInfo: list of SpeedTestingInfo
-        :param _ProxySpeedTestingInfo: EO 拨测信息。
-        :type ProxySpeedTestingInfo: list of SpeedTestingInfo
-        :param _SpeedTestingStatus: 站点状态。
-        :type SpeedTestingStatus: :class:`tencentcloud.teo.v20220901.models.SpeedTestingStatus`
-        :param _OptimizeAction: 优化建议。
-        :type OptimizeAction: list of OptimizeAction
-        :param _ProxyLoadTime: EO 整体性能，单位ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyLoadTime: int
-        :param _OriginLoadTime: 源站整体性能，单位ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type OriginLoadTime: int
-        """
-        self._ZoneId = None
-        self._ZoneName = None
-        self._OriginSpeedTestingInfo = None
-        self._ProxySpeedTestingInfo = None
-        self._SpeedTestingStatus = None
-        self._OptimizeAction = None
-        self._ProxyLoadTime = None
-        self._OriginLoadTime = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-    @property
-    def ZoneName(self):
-        return self._ZoneName
-
-    @ZoneName.setter
-    def ZoneName(self, ZoneName):
-        self._ZoneName = ZoneName
-
-    @property
-    def OriginSpeedTestingInfo(self):
-        return self._OriginSpeedTestingInfo
-
-    @OriginSpeedTestingInfo.setter
-    def OriginSpeedTestingInfo(self, OriginSpeedTestingInfo):
-        self._OriginSpeedTestingInfo = OriginSpeedTestingInfo
-
-    @property
-    def ProxySpeedTestingInfo(self):
-        return self._ProxySpeedTestingInfo
-
-    @ProxySpeedTestingInfo.setter
-    def ProxySpeedTestingInfo(self, ProxySpeedTestingInfo):
-        self._ProxySpeedTestingInfo = ProxySpeedTestingInfo
-
-    @property
-    def SpeedTestingStatus(self):
-        return self._SpeedTestingStatus
-
-    @SpeedTestingStatus.setter
-    def SpeedTestingStatus(self, SpeedTestingStatus):
-        self._SpeedTestingStatus = SpeedTestingStatus
-
-    @property
-    def OptimizeAction(self):
-        return self._OptimizeAction
-
-    @OptimizeAction.setter
-    def OptimizeAction(self, OptimizeAction):
-        self._OptimizeAction = OptimizeAction
-
-    @property
-    def ProxyLoadTime(self):
-        return self._ProxyLoadTime
-
-    @ProxyLoadTime.setter
-    def ProxyLoadTime(self, ProxyLoadTime):
-        self._ProxyLoadTime = ProxyLoadTime
-
-    @property
-    def OriginLoadTime(self):
-        return self._OriginLoadTime
-
-    @OriginLoadTime.setter
-    def OriginLoadTime(self, OriginLoadTime):
-        self._OriginLoadTime = OriginLoadTime
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        self._ZoneName = params.get("ZoneName")
-        if params.get("OriginSpeedTestingInfo") is not None:
-            self._OriginSpeedTestingInfo = []
-            for item in params.get("OriginSpeedTestingInfo"):
-                obj = SpeedTestingInfo()
-                obj._deserialize(item)
-                self._OriginSpeedTestingInfo.append(obj)
-        if params.get("ProxySpeedTestingInfo") is not None:
-            self._ProxySpeedTestingInfo = []
-            for item in params.get("ProxySpeedTestingInfo"):
-                obj = SpeedTestingInfo()
-                obj._deserialize(item)
-                self._ProxySpeedTestingInfo.append(obj)
-        if params.get("SpeedTestingStatus") is not None:
-            self._SpeedTestingStatus = SpeedTestingStatus()
-            self._SpeedTestingStatus._deserialize(params.get("SpeedTestingStatus"))
-        if params.get("OptimizeAction") is not None:
-            self._OptimizeAction = []
-            for item in params.get("OptimizeAction"):
-                obj = OptimizeAction()
-                obj._deserialize(item)
-                self._OptimizeAction.append(obj)
-        self._ProxyLoadTime = params.get("ProxyLoadTime")
-        self._OriginLoadTime = params.get("OriginLoadTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingQuota(AbstractModel):
-    """拨测配额数据。
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TotalTestRuns: 站点总拨测次数。
-        :type TotalTestRuns: int
-        :param _AvailableTestRuns: 站点剩余可用拨测次数。
-        :type AvailableTestRuns: int
-        """
-        self._TotalTestRuns = None
-        self._AvailableTestRuns = None
-
-    @property
-    def TotalTestRuns(self):
-        return self._TotalTestRuns
-
-    @TotalTestRuns.setter
-    def TotalTestRuns(self, TotalTestRuns):
-        self._TotalTestRuns = TotalTestRuns
-
-    @property
-    def AvailableTestRuns(self):
-        return self._AvailableTestRuns
-
-    @AvailableTestRuns.setter
-    def AvailableTestRuns(self, AvailableTestRuns):
-        self._AvailableTestRuns = AvailableTestRuns
-
-
-    def _deserialize(self, params):
-        self._TotalTestRuns = params.get("TotalTestRuns")
-        self._AvailableTestRuns = params.get("AvailableTestRuns")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingStatistics(AbstractModel):
-    """拨测统计结果
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _FirstContentfulPaint: 首屏时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type FirstContentfulPaint: int
-        :param _FirstMeaningfulPaint: 首屏完全渲染时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type FirstMeaningfulPaint: int
-        :param _OverallDownloadSpeed: 整体下载速度，单位 KB/s。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type OverallDownloadSpeed: float
-        :param _RenderTime: 渲染时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RenderTime: int
-        :param _DocumentFinishTime: 文档完成时间, 单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DocumentFinishTime: int
-        :param _TcpConnectionTime: 基础文档TCP连接时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TcpConnectionTime: int
-        :param _ResponseTime: 基础文档服务器响应时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ResponseTime: int
-        :param _FileDownloadTime: 基础文档下载时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type FileDownloadTime: int
-        :param _LoadTime: 整体性能，测试总时间，单位 ms。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type LoadTime: int
-        """
-        self._FirstContentfulPaint = None
-        self._FirstMeaningfulPaint = None
-        self._OverallDownloadSpeed = None
-        self._RenderTime = None
-        self._DocumentFinishTime = None
-        self._TcpConnectionTime = None
-        self._ResponseTime = None
-        self._FileDownloadTime = None
-        self._LoadTime = None
-
-    @property
-    def FirstContentfulPaint(self):
-        return self._FirstContentfulPaint
-
-    @FirstContentfulPaint.setter
-    def FirstContentfulPaint(self, FirstContentfulPaint):
-        self._FirstContentfulPaint = FirstContentfulPaint
-
-    @property
-    def FirstMeaningfulPaint(self):
-        return self._FirstMeaningfulPaint
-
-    @FirstMeaningfulPaint.setter
-    def FirstMeaningfulPaint(self, FirstMeaningfulPaint):
-        self._FirstMeaningfulPaint = FirstMeaningfulPaint
-
-    @property
-    def OverallDownloadSpeed(self):
-        return self._OverallDownloadSpeed
-
-    @OverallDownloadSpeed.setter
-    def OverallDownloadSpeed(self, OverallDownloadSpeed):
-        self._OverallDownloadSpeed = OverallDownloadSpeed
-
-    @property
-    def RenderTime(self):
-        return self._RenderTime
-
-    @RenderTime.setter
-    def RenderTime(self, RenderTime):
-        self._RenderTime = RenderTime
-
-    @property
-    def DocumentFinishTime(self):
-        return self._DocumentFinishTime
-
-    @DocumentFinishTime.setter
-    def DocumentFinishTime(self, DocumentFinishTime):
-        self._DocumentFinishTime = DocumentFinishTime
-
-    @property
-    def TcpConnectionTime(self):
-        return self._TcpConnectionTime
-
-    @TcpConnectionTime.setter
-    def TcpConnectionTime(self, TcpConnectionTime):
-        self._TcpConnectionTime = TcpConnectionTime
-
-    @property
-    def ResponseTime(self):
-        return self._ResponseTime
-
-    @ResponseTime.setter
-    def ResponseTime(self, ResponseTime):
-        self._ResponseTime = ResponseTime
-
-    @property
-    def FileDownloadTime(self):
-        return self._FileDownloadTime
-
-    @FileDownloadTime.setter
-    def FileDownloadTime(self, FileDownloadTime):
-        self._FileDownloadTime = FileDownloadTime
-
-    @property
-    def LoadTime(self):
-        return self._LoadTime
-
-    @LoadTime.setter
-    def LoadTime(self, LoadTime):
-        self._LoadTime = LoadTime
-
-
-    def _deserialize(self, params):
-        self._FirstContentfulPaint = params.get("FirstContentfulPaint")
-        self._FirstMeaningfulPaint = params.get("FirstMeaningfulPaint")
-        self._OverallDownloadSpeed = params.get("OverallDownloadSpeed")
-        self._RenderTime = params.get("RenderTime")
-        self._DocumentFinishTime = params.get("DocumentFinishTime")
-        self._TcpConnectionTime = params.get("TcpConnectionTime")
-        self._ResponseTime = params.get("ResponseTime")
-        self._FileDownloadTime = params.get("FileDownloadTime")
-        self._LoadTime = params.get("LoadTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SpeedTestingStatus(AbstractModel):
-    """拨测任务状态信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Url: 拨测 url。
-        :type Url: str
-        :param _Tls: 拨测 url 是否使用 https。
-        :type Tls: bool
-        :param _CreatedOn: 任务创建时间。
-        :type CreatedOn: str
-        :param _StatusCode: 任务状态，取值有：
-<li> 200：任务完成;</li>
-<li> 100：任务进行中。</li>
-<li> 503: 任务失败。</li>
-注意：此字段可能返回 null，表示取不到有效值。
-        :type StatusCode: int
-        :param _UA: 拨测 UA。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type UA: str
-        :param _Connectivity: 网络环境。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Connectivity: str
-        :param _Reachable: 是否可达，取值：
-<li> true：可达；</li>
-<li> false：不可达。</li>
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Reachable: bool
-        :param _TimedOut: 是否超时，取值：
-<li> true：超时；</li>
-<li> false：不超时。</li>
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TimedOut: bool
+        :param _Switch: Debug 功能开关，取值有：
+<li>on：开启；</li>
+<li>off：关闭。</li>
+        :type Switch: str
+        :param _AllowClientIPList: 允许的客户端来源。支持填写 IPV4 以及 IPV6 的 IP/IP 段，不填则表示允许任意客户端 IP。
+        :type AllowClientIPList: list of str
+        :param _ExpireTime: Debug 功能到期时间。超出设置的时间，则功能失效。
+        :type ExpireTime: str
         """
-        self._Url = None
-        self._Tls = None
-        self._CreatedOn = None
-        self._StatusCode = None
-        self._UA = None
-        self._Connectivity = None
-        self._Reachable = None
-        self._TimedOut = None
-
-    @property
-    def Url(self):
-        return self._Url
-
-    @Url.setter
-    def Url(self, Url):
-        self._Url = Url
-
-    @property
-    def Tls(self):
-        return self._Tls
-
-    @Tls.setter
-    def Tls(self, Tls):
-        self._Tls = Tls
-
-    @property
-    def CreatedOn(self):
-        return self._CreatedOn
-
-    @CreatedOn.setter
-    def CreatedOn(self, CreatedOn):
-        self._CreatedOn = CreatedOn
-
-    @property
-    def StatusCode(self):
-        return self._StatusCode
-
-    @StatusCode.setter
-    def StatusCode(self, StatusCode):
-        self._StatusCode = StatusCode
-
-    @property
-    def UA(self):
-        return self._UA
-
-    @UA.setter
-    def UA(self, UA):
-        self._UA = UA
+        self._Switch = None
+        self._AllowClientIPList = None
+        self._ExpireTime = None
 
     @property
-    def Connectivity(self):
-        return self._Connectivity
+    def Switch(self):
+        return self._Switch
 
-    @Connectivity.setter
-    def Connectivity(self, Connectivity):
-        self._Connectivity = Connectivity
+    @Switch.setter
+    def Switch(self, Switch):
+        self._Switch = Switch
 
     @property
-    def Reachable(self):
-        return self._Reachable
+    def AllowClientIPList(self):
+        return self._AllowClientIPList
 
-    @Reachable.setter
-    def Reachable(self, Reachable):
-        self._Reachable = Reachable
+    @AllowClientIPList.setter
+    def AllowClientIPList(self, AllowClientIPList):
+        self._AllowClientIPList = AllowClientIPList
 
     @property
-    def TimedOut(self):
-        return self._TimedOut
+    def ExpireTime(self):
+        return self._ExpireTime
 
-    @TimedOut.setter
-    def TimedOut(self, TimedOut):
-        self._TimedOut = TimedOut
+    @ExpireTime.setter
+    def ExpireTime(self, ExpireTime):
+        self._ExpireTime = ExpireTime
 
 
     def _deserialize(self, params):
-        self._Url = params.get("Url")
-        self._Tls = params.get("Tls")
-        self._CreatedOn = params.get("CreatedOn")
-        self._StatusCode = params.get("StatusCode")
-        self._UA = params.get("UA")
-        self._Connectivity = params.get("Connectivity")
-        self._Reachable = params.get("Reachable")
-        self._TimedOut = params.get("TimedOut")
+        self._Switch = params.get("Switch")
+        self._AllowClientIPList = params.get("AllowClientIPList")
+        self._ExpireTime = params.get("ExpireTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -22446,17 +17774,34 @@
 
     def __init__(self):
         r"""
         :param _Key: 询价参数键。
         :type Key: str
         :param _Value: 询价参数值。
         :type Value: str
+        :param _Pack: 询价参数映射的配额，取值有：
+<li>zone：站点数；</li>
+<li>custom-rule：自定义规则数；</li>
+<li>rate-limiting-rule：速率限制规则数；</li>
+<li>l4-proxy-instance：四层代理实例数。</li>
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Pack: str
+        :param _InstanceId: 询价参数映射的四层代理实例Id。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param _ProtectionSpecs: 询价参数对应的防护等级。
+取值有： <li> cm_30G：中国大陆加速区域保底防护30Gbps；</li><li> cm_60G：中国大陆加速区域保底防护60Gbps；</li><li> cm_100G：中国大陆加速区域保底防护100Gbps；</li><li> anycast_300G：全球加速区域（除中国大陆）Anycast联防300Gbps；</li><li> anycast_unlimited：全球加速区域（除中国大陆）Anycast无上限全力防护；</li><li> cm_30G_anycast_300G：中国大陆加速区域保底防护30Gbps，全球加速区域（除中国大陆）Anycast联防300Gbps；</li><li> cm_30G_anycast_unlimited：中国大陆加速区域保底防护30Gbps，全球加速区域（除中国大陆）Anycast无上限全力防护；</li><li> cm_60G_anycast_300G：中国大陆加速区域保底防护60Gbps，全球加速区域（除中国大陆）Anycast联防300Gbps；</li><li> cm_60G_anycast_unlimited：中国大陆加速区域保底防护60Gbps，全球加速区域（除中国大陆）Anycast无上限全力防护；</li><li> cm_100G_anycast_300G：中国大陆加速区域保底防护100Gbps，全球加速区域（除中国大陆）Anycast联防300Gbps；</li><li> cm_100G_anycast_unlimited：中国大陆加速区域保底防护100Gbps，全球加速区域（除中国大陆）Anycast无上限全力防护。</li>
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProtectionSpecs: str
         """
         self._Key = None
         self._Value = None
+        self._Pack = None
+        self._InstanceId = None
+        self._ProtectionSpecs = None
 
     @property
     def Key(self):
         return self._Key
 
     @Key.setter
     def Key(self, Key):
@@ -22466,18 +17811,45 @@
     def Value(self):
         return self._Value
 
     @Value.setter
     def Value(self, Value):
         self._Value = Value
 
+    @property
+    def Pack(self):
+        return self._Pack
+
+    @Pack.setter
+    def Pack(self, Pack):
+        self._Pack = Pack
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def ProtectionSpecs(self):
+        return self._ProtectionSpecs
+
+    @ProtectionSpecs.setter
+    def ProtectionSpecs(self, ProtectionSpecs):
+        self._ProtectionSpecs = ProtectionSpecs
+
 
     def _deserialize(self, params):
         self._Key = params.get("Key")
         self._Value = params.get("Value")
+        self._Pack = params.get("Pack")
+        self._InstanceId = params.get("InstanceId")
+        self._ProtectionSpecs = params.get("ProtectionSpecs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -23072,72 +18444,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class UpdateOriginProtectionIPWhitelistRequest(AbstractModel):
-    """UpdateOriginProtectionIPWhitelist请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ZoneId: 站点ID。
-        :type ZoneId: str
-        """
-        self._ZoneId = None
-
-    @property
-    def ZoneId(self):
-        return self._ZoneId
-
-    @ZoneId.setter
-    def ZoneId(self, ZoneId):
-        self._ZoneId = ZoneId
-
-
-    def _deserialize(self, params):
-        self._ZoneId = params.get("ZoneId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class UpdateOriginProtectionIPWhitelistResponse(AbstractModel):
-    """UpdateOriginProtectionIPWhitelist返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class UpstreamHttp2(AbstractModel):
     """Http2回源配置
 
     """
 
     def __init__(self):
         r"""
@@ -23398,81 +18712,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class WafGroup(AbstractModel):
-    """Waf托管规则组
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Action: 执行动作，取值有：
-<li> block：阻断；</li>
-<li> observe：观察。</li>
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Action: str
-        :param _Level: 防护级别，取值有：
-<li> loose：宽松；</li>
-<li> normal：正常；</li>
-<li> strict：严格；</li>
-<li> stricter：超严格；</li>
-<li> custom：自定义。</li>
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Level: str
-        :param _TypeId: 规则类型id。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TypeId: int
-        """
-        self._Action = None
-        self._Level = None
-        self._TypeId = None
-
-    @property
-    def Action(self):
-        return self._Action
-
-    @Action.setter
-    def Action(self, Action):
-        self._Action = Action
-
-    @property
-    def Level(self):
-        return self._Level
-
-    @Level.setter
-    def Level(self, Level):
-        self._Level = Level
-
-    @property
-    def TypeId(self):
-        return self._TypeId
-
-    @TypeId.setter
-    def TypeId(self, TypeId):
-        self._TypeId = TypeId
-
-
-    def _deserialize(self, params):
-        self._Action = params.get("Action")
-        self._Level = params.get("Level")
-        self._TypeId = params.get("TypeId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class WafRule(AbstractModel):
     """Waf规则
 
     """
 
     def __init__(self):
         r"""
@@ -23524,200 +18771,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class WebLogs(AbstractModel):
-    """web攻击日志
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _EventId: 请求（事件）ID。
-        :type EventId: str
-        :param _HttpLog: http 日志内容。
-        :type HttpLog: str
-        :param _Domain: 受攻击子域名。
-        :type Domain: str
-        :param _AttackIp: 攻击源（客户端）Ip。
-        :type AttackIp: str
-        :param _SipCountryCode: IP所在国家iso-3166中alpha-2编码，编码信息请参考[ISO-3166](https://git.woa.com/edgeone/iso-3166/blob/master/all/all.json)
-        :type SipCountryCode: str
-        :param _RealClientIp: 真实客户端Ip。
-        :type RealClientIp: str
-        :param _RealClientIpCountryCode: 真实客户端Ip所在国家iso-3166中alpha-2编码。
-        :type RealClientIpCountryCode: str
-        :param _AttackTime: 攻击时间，采用unix秒级时间戳。
-        :type AttackTime: int
-        :param _RequestUri: 请求地址。
-        :type RequestUri: str
-        :param _ReqMethod: 请求类型。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ReqMethod: str
-        :param _RuleDetailList: 规则相关信息列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RuleDetailList: list of SecRuleRelatedInfo
-        :param _AttackContent: 攻击内容。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AttackContent: str
-        :param _Area: 日志所属区域。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Area: str
-        """
-        self._EventId = None
-        self._HttpLog = None
-        self._Domain = None
-        self._AttackIp = None
-        self._SipCountryCode = None
-        self._RealClientIp = None
-        self._RealClientIpCountryCode = None
-        self._AttackTime = None
-        self._RequestUri = None
-        self._ReqMethod = None
-        self._RuleDetailList = None
-        self._AttackContent = None
-        self._Area = None
-
-    @property
-    def EventId(self):
-        return self._EventId
-
-    @EventId.setter
-    def EventId(self, EventId):
-        self._EventId = EventId
-
-    @property
-    def HttpLog(self):
-        return self._HttpLog
-
-    @HttpLog.setter
-    def HttpLog(self, HttpLog):
-        self._HttpLog = HttpLog
-
-    @property
-    def Domain(self):
-        return self._Domain
-
-    @Domain.setter
-    def Domain(self, Domain):
-        self._Domain = Domain
-
-    @property
-    def AttackIp(self):
-        return self._AttackIp
-
-    @AttackIp.setter
-    def AttackIp(self, AttackIp):
-        self._AttackIp = AttackIp
-
-    @property
-    def SipCountryCode(self):
-        return self._SipCountryCode
-
-    @SipCountryCode.setter
-    def SipCountryCode(self, SipCountryCode):
-        self._SipCountryCode = SipCountryCode
-
-    @property
-    def RealClientIp(self):
-        return self._RealClientIp
-
-    @RealClientIp.setter
-    def RealClientIp(self, RealClientIp):
-        self._RealClientIp = RealClientIp
-
-    @property
-    def RealClientIpCountryCode(self):
-        return self._RealClientIpCountryCode
-
-    @RealClientIpCountryCode.setter
-    def RealClientIpCountryCode(self, RealClientIpCountryCode):
-        self._RealClientIpCountryCode = RealClientIpCountryCode
-
-    @property
-    def AttackTime(self):
-        return self._AttackTime
-
-    @AttackTime.setter
-    def AttackTime(self, AttackTime):
-        self._AttackTime = AttackTime
-
-    @property
-    def RequestUri(self):
-        return self._RequestUri
-
-    @RequestUri.setter
-    def RequestUri(self, RequestUri):
-        self._RequestUri = RequestUri
-
-    @property
-    def ReqMethod(self):
-        return self._ReqMethod
-
-    @ReqMethod.setter
-    def ReqMethod(self, ReqMethod):
-        self._ReqMethod = ReqMethod
-
-    @property
-    def RuleDetailList(self):
-        return self._RuleDetailList
-
-    @RuleDetailList.setter
-    def RuleDetailList(self, RuleDetailList):
-        self._RuleDetailList = RuleDetailList
-
-    @property
-    def AttackContent(self):
-        return self._AttackContent
-
-    @AttackContent.setter
-    def AttackContent(self, AttackContent):
-        self._AttackContent = AttackContent
-
-    @property
-    def Area(self):
-        return self._Area
-
-    @Area.setter
-    def Area(self, Area):
-        self._Area = Area
-
-
-    def _deserialize(self, params):
-        self._EventId = params.get("EventId")
-        self._HttpLog = params.get("HttpLog")
-        self._Domain = params.get("Domain")
-        self._AttackIp = params.get("AttackIp")
-        self._SipCountryCode = params.get("SipCountryCode")
-        self._RealClientIp = params.get("RealClientIp")
-        self._RealClientIpCountryCode = params.get("RealClientIpCountryCode")
-        self._AttackTime = params.get("AttackTime")
-        self._RequestUri = params.get("RequestUri")
-        self._ReqMethod = params.get("ReqMethod")
-        if params.get("RuleDetailList") is not None:
-            self._RuleDetailList = []
-            for item in params.get("RuleDetailList"):
-                obj = SecRuleRelatedInfo()
-                obj._deserialize(item)
-                self._RuleDetailList.append(obj)
-        self._AttackContent = params.get("AttackContent")
-        self._Area = params.get("Area")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class WebSocket(AbstractModel):
     """WebSocket配置
 
     """
 
     def __init__(self):
         r"""
@@ -23780,15 +18841,16 @@
 <li> active：NS 已切换； </li>
 <li> pending：NS 未切换；</li>
 <li> moved：NS 已切走；</li>
 <li> deactivated：被封禁。 </li>
         :type Status: str
         :param _Type: 站点接入方式，取值有
 <li> full：NS 接入； </li>
-<li> partial：CNAME 接入。</li>
+<li> partial：CNAME 接入；</li>
+<li> noDomainAccess：无域名接入。</li>
         :type Type: str
         :param _Paused: 站点是否关闭。
         :type Paused: bool
         :param _CnameSpeedUp: 是否开启 CNAME 加速，取值有：
 <li> enabled：开启；</li>
 <li> disabled：关闭。</li>
         :type CnameSpeedUp: str
@@ -24129,14 +19191,17 @@
         :type Grpc: :class:`tencentcloud.teo.v20220901.models.Grpc`
         :param _ImageOptimize: 图片优化相关配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ImageOptimize: :class:`tencentcloud.teo.v20220901.models.ImageOptimize`
         :param _AccelerateMainland: 中国大陆加速优化配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccelerateMainland: :class:`tencentcloud.teo.v20220901.models.AccelerateMainland`
+        :param _StandardDebug: 标准 Debug 配置。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StandardDebug: :class:`tencentcloud.teo.v20220901.models.StandardDebug`
         """
         self._ZoneName = None
         self._Area = None
         self._CacheKey = None
         self._Quic = None
         self._PostMaxSize = None
         self._Compression = None
@@ -24152,14 +19217,15 @@
         self._CachePrefresh = None
         self._Ipv6 = None
         self._Https = None
         self._ClientIpCountry = None
         self._Grpc = None
         self._ImageOptimize = None
         self._AccelerateMainland = None
+        self._StandardDebug = None
 
     @property
     def ZoneName(self):
         return self._ZoneName
 
     @ZoneName.setter
     def ZoneName(self, ZoneName):
@@ -24329,14 +19395,22 @@
     def AccelerateMainland(self):
         return self._AccelerateMainland
 
     @AccelerateMainland.setter
     def AccelerateMainland(self, AccelerateMainland):
         self._AccelerateMainland = AccelerateMainland
 
+    @property
+    def StandardDebug(self):
+        return self._StandardDebug
+
+    @StandardDebug.setter
+    def StandardDebug(self, StandardDebug):
+        self._StandardDebug = StandardDebug
+
 
     def _deserialize(self, params):
         self._ZoneName = params.get("ZoneName")
         self._Area = params.get("Area")
         if params.get("CacheKey") is not None:
             self._CacheKey = CacheKey()
             self._CacheKey._deserialize(params.get("CacheKey"))
@@ -24393,14 +19467,17 @@
             self._Grpc._deserialize(params.get("Grpc"))
         if params.get("ImageOptimize") is not None:
             self._ImageOptimize = ImageOptimize()
             self._ImageOptimize._deserialize(params.get("ImageOptimize"))
         if params.get("AccelerateMainland") is not None:
             self._AccelerateMainland = AccelerateMainland()
             self._AccelerateMainland._deserialize(params.get("AccelerateMainland"))
+        if params.get("StandardDebug") is not None:
+            self._StandardDebug = StandardDebug()
+            self._StandardDebug._deserialize(params.get("StandardDebug"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/teo/v20220901/teo_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,28 +45,28 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CheckCertificate(self, request):
-        """校验证书
+    def CheckCnameStatus(self, request):
+        """校验域名 CNAME 状态
 
-        :param request: Request instance for CheckCertificate.
-        :type request: :class:`tencentcloud.teo.v20220901.models.CheckCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.CheckCertificateResponse`
+        :param request: Request instance for CheckCnameStatus.
+        :type request: :class:`tencentcloud.teo.v20220901.models.CheckCnameStatusRequest`
+        :rtype: :class:`tencentcloud.teo.v20220901.models.CheckCnameStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CheckCertificate", params, headers=headers)
+            body = self.call("CheckCnameStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.CheckCertificateResponse()
+            model = models.CheckCnameStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
@@ -160,37 +160,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateCredential(self, request):
-        """用于创建COS回源私有凭证
-
-        :param request: Request instance for CreateCredential.
-        :type request: :class:`tencentcloud.teo.v20220901.models.CreateCredentialRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateCredentialResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateCredential", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateCredentialResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def CreateOriginGroup(self, request):
         """创建源站组
 
         :param request: Request instance for CreateOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateOriginGroupRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.CreateOriginGroupResponse`
 
@@ -253,15 +230,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePurgeTask(self, request):
-        """创建清除缓存任务
+        """当源站资源更新，但节点缓存 TTL 未过期时，用户仍会访问到旧的资源，此时可以通过该接口实现节点资源更新。触发更新的方法有以下两种：<li>直接删除：不做任何校验，直接删除节点缓存，用户请求时触发回源拉取；</li><li>标记过期：将节点资源置为过期，用户请求时触发回源校验，即发送带有 If-None-Match 和 If-Modified-Since 头部的 HTTP 条件请求。若源站响应 200，则节点会回源拉取新的资源并更新缓存；若源站响应 304，则节点不会更新缓存；</li>
+
+        清除缓存任务详情请查看[清除缓存](https://cloud.tencent.com/document/product/1552/70759)。</li>
 
         :param request: Request instance for CreatePurgeTask.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreatePurgeTaskRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.CreatePurgeTaskResponse`
 
         """
         try:
@@ -275,37 +254,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateReplayTask(self, request):
-        """创建刷新/预热重放任务
-
-        :param request: Request instance for CreateReplayTask.
-        :type request: :class:`tencentcloud.teo.v20220901.models.CreateReplayTaskRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateReplayTaskResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateReplayTask", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateReplayTaskResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def CreateRule(self, request):
         """规则引擎创建规则。
 
         :param request: Request instance for CreateRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateRuleRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.CreateRuleResponse`
 
@@ -344,37 +300,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateSpeedTesting(self, request):
-        """对用户指定的域名进行一次站点拨测
-
-        :param request: Request instance for CreateSpeedTesting.
-        :type request: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.CreateSpeedTestingResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateSpeedTesting", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateSpeedTestingResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def CreateZone(self, request):
         """用于用户接入新的站点。
 
         :param request: Request instance for CreateZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateZoneRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.CreateZoneResponse`
 
@@ -597,37 +530,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeAddableEntityList(self, request):
-        """本接口（DescribeAddableEntityList）用于查询剩余可添加的日志推送实体列表。
-
-        :param request: Request instance for DescribeAddableEntityList.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAddableEntityListRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAddableEntityListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeAddableEntityList", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeAddableEntityListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeAliasDomains(self, request):
         """查询别称域名信息列表。
 
         :param request: Request instance for DescribeAliasDomains.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAliasDomainsRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeAliasDomainsResponse`
 
@@ -689,37 +599,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeClientRuleList(self, request):
-        """本接口（DescribeClientRuleList）用于查询封禁客户端信息列表。
-
-        :param request: Request instance for DescribeClientRuleList.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeClientRuleListRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeClientRuleListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeClientRuleList", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeClientRuleListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeContentQuota(self, request):
         """查询内容管理接口配额
 
         :param request: Request instance for DescribeContentQuota.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeContentQuotaRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeContentQuotaResponse`
 
@@ -827,37 +714,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeDnsData(self, request):
-        """获取DNS请求数统计曲线
-
-        :param request: Request instance for DescribeDnsData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDnsDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeDnsDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDnsData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDnsDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeHostsSetting(self, request):
         """用于查询域名配置信息
 
         :param request: Request instance for DescribeHostsSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeHostsSettingRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeHostsSettingResponse`
 
@@ -896,60 +760,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeLogSets(self, request):
-        """本接口（DescribeLogSets）用于获取日志集列表。
-
-        :param request: Request instance for DescribeLogSets.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeLogSetsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeLogSetsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeLogSets", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeLogSetsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeLogTopicTasks(self, request):
-        """本接口（DescribeLogTopicTasks）用于获取日志推送任务列表。
-
-        :param request: Request instance for DescribeLogTopicTasks.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeLogTopicTasksRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeLogTopicTasksResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeLogTopicTasks", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeLogTopicTasksResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeOriginGroup(self, request):
         """获取源站组列表
 
         :param request: Request instance for DescribeOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOriginGroupRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeOriginGroupResponse`
 
@@ -1103,106 +921,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSingleL7AnalysisData(self, request):
-        """本接口（DescribeSingleL7AnalysisData）用于查询七层流量数据分析单值数据列表，单值数据表示：指标在查询时间范围内的单个统计数据，通常表现为接口仅返回一个统计数值。
-
-        :param request: Request instance for DescribeSingleL7AnalysisData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSingleL7AnalysisDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSingleL7AnalysisDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSingleL7AnalysisData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSingleL7AnalysisDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeSpeedTestingDetails(self, request):
-        """用于查询拨测分地区数据
-
-        :param request: Request instance for DescribeSpeedTestingDetails.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingDetailsRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingDetailsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSpeedTestingDetails", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSpeedTestingDetailsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeSpeedTestingMetricData(self, request):
-        """查询站点拨测结果
-
-        :param request: Request instance for DescribeSpeedTestingMetricData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingMetricDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingMetricDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSpeedTestingMetricData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSpeedTestingMetricDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeSpeedTestingQuota(self, request):
-        """查询站点拨测配额
-
-        :param request: Request instance for DescribeSpeedTestingQuota.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingQuotaRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeSpeedTestingQuotaResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSpeedTestingQuota", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSpeedTestingQuotaResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeTimingL4Data(self, request):
         """本接口（DescribeTimingL4Data）用于查询四层时序流量数据列表。
 
         :param request: Request instance for DescribeTimingL4Data.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL4DataRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL4DataResponse`
 
@@ -1264,37 +990,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeTimingL7SourceData(self, request):
-        """本接口（DescribeTimingL7SourceData）查询七层回源分析时序数据。
-
-        :param request: Request instance for DescribeTimingL7SourceData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7SourceDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7SourceDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeTimingL7SourceData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeTimingL7SourceDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeTopL7AnalysisData(self, request):
         """本接口（DescribeTopL7AnalysisData）用于查询七层流量前topN的数据。
 
         :param request: Request instance for DescribeTopL7AnalysisData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7AnalysisDataRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7AnalysisDataResponse`
 
@@ -1333,175 +1036,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeWebManagedRulesData(self, request):
-        """本接口（DescribeWebManagedRulesData）用于查询WAF攻击的时序数据。
-
-        :param request: Request instance for DescribeWebManagedRulesData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebManagedRulesData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebManagedRulesDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebManagedRulesHitRuleDetail(self, request):
-        """本接口（DescribeWebManagedRulesHitRuleDetail）用于查询WAF攻击命中规则详情。
-
-        :param request: Request instance for DescribeWebManagedRulesHitRuleDetail.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesHitRuleDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesHitRuleDetailResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebManagedRulesHitRuleDetail", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebManagedRulesHitRuleDetailResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebManagedRulesLog(self, request):
-        """本接口（DescribeWebManagedRulesLog）用于查询Web攻击日志。
-
-        :param request: Request instance for DescribeWebManagedRulesLog.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesLogRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebManagedRulesLogResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebManagedRulesLog", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebManagedRulesLogResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebProtectionClientIpList(self, request):
-        """本接口（DescribeWebProtectionClientIpList）用于查询CC防护客户端（攻击源）IP信息。
-
-        :param request: Request instance for DescribeWebProtectionClientIpList.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionClientIpListRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionClientIpListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebProtectionClientIpList", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebProtectionClientIpListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebProtectionData(self, request):
-        """本接口（DescribeWebProtectionData）用于查询CC防护时序数据。
-
-        :param request: Request instance for DescribeWebProtectionData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebProtectionData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebProtectionDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebProtectionHitRuleDetail(self, request):
-        """本接口（DescribeWebProtectionHitRuleDetail）用于查询CC防护命中规则详情列表。
-
-        :param request: Request instance for DescribeWebProtectionHitRuleDetail.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionHitRuleDetailRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionHitRuleDetailResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebProtectionHitRuleDetail", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebProtectionHitRuleDetailResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeWebProtectionTopData(self, request):
-        """本接口（DescribeWebProtectionTopData）用于查询CC防护的Top数据。
-
-        :param request: Request instance for DescribeWebProtectionTopData.
-        :type request: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionTopDataRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeWebProtectionTopDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeWebProtectionTopData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeWebProtectionTopDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeZoneSetting(self, request):
         """用于查询站点的所有配置信息。
 
         :param request: Request instance for DescribeZoneSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeZoneSettingRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.DescribeZoneSettingResponse`
 
@@ -1793,37 +1335,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyDefaultCertificate(self, request):
-        """修改默认证书状态
-
-        :param request: Request instance for ModifyDefaultCertificate.
-        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyDefaultCertificateRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyDefaultCertificateResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyDefaultCertificate", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyDefaultCertificateResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def ModifyHostsCertificate(self, request):
         """用于修改域名证书
 
         :param request: Request instance for ModifyHostsCertificate.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyHostsCertificateRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyHostsCertificateResponse`
 
@@ -1885,37 +1404,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyRulePriority(self, request):
-        """修改规则引擎规则优先级
-
-        :param request: Request instance for ModifyRulePriority.
-        :type request: :class:`tencentcloud.teo.v20220901.models.ModifyRulePriorityRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyRulePriorityResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyRulePriority", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyRulePriorityResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def ModifySecurityIPGroup(self, request):
         """修改安全 IP 组。
 
         :param request: Request instance for ModifySecurityIPGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityIPGroupRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.ModifySecurityIPGroupResponse`
 
@@ -1954,37 +1450,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifySecurityWafGroupPolicy(self, request):
-        """修改安全配置托管规则
-
-        :param request: Request instance for ModifySecurityWafGroupPolicy.
-        :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityWafGroupPolicyRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.ModifySecurityWafGroupPolicyResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifySecurityWafGroupPolicy", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifySecurityWafGroupPolicyResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def ModifyZone(self, request):
         """修改站点信息。
 
         :param request: Request instance for ModifyZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneRequest`
         :rtype: :class:`tencentcloud.teo.v20220901.models.ModifyZoneResponse`
 
@@ -2043,77 +1516,8 @@
             model = models.ModifyZoneStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def ReclaimAliasDomain(self, request):
-        """当客户取回站定的同时会取回此站点下关联的别称域名，此时入参为ZoneId；当客户接入站点发现已被别称域名接入时通过验证之后可取回域名，此时入参为ZoneName。
-
-        :param request: Request instance for ReclaimAliasDomain.
-        :type request: :class:`tencentcloud.teo.v20220901.models.ReclaimAliasDomainRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.ReclaimAliasDomainResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ReclaimAliasDomain", params, headers=headers)
-            response = json.loads(body)
-            model = models.ReclaimAliasDomainResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def ReclaimZone(self, request):
-        """站点被其他用户接入后，验证了站点所有权之后，可以找回该站点。
-
-        :param request: Request instance for ReclaimZone.
-        :type request: :class:`tencentcloud.teo.v20220901.models.ReclaimZoneRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.ReclaimZoneResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ReclaimZone", params, headers=headers)
-            response = json.loads(body)
-            model = models.ReclaimZoneResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def UpdateOriginProtectionIPWhitelist(self, request):
-        """更新源站防护IP白名单
-
-        :param request: Request instance for UpdateOriginProtectionIPWhitelist.
-        :type request: :class:`tencentcloud.teo.v20220901.models.UpdateOriginProtectionIPWhitelistRequest`
-        :rtype: :class:`tencentcloud.teo.v20220901.models.UpdateOriginProtectionIPWhitelistResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("UpdateOriginProtectionIPWhitelist", params, headers=headers)
-            response = json.loads(body)
-            model = models.UpdateOriginProtectionIPWhitelistResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-teo-3.0.928/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.929/tencentcloud/__init__.py`

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

