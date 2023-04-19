# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.875.tar", last modified: Tue Apr 18 01:05:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.876.tar", last modified: Wed Apr 19 00:43:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.875.tar` & `tencentcloud-sdk-python-waf-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    43870 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164697 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    43894 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   170365 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:43:12.000000 tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.875/README.rst` & `tencentcloud-sdk-python-waf-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyAccessPeriod(self, request):
-        """本接口用于修改访问日志保存期限
+        """本接口用于修改访问日志保存期限及大字段是否存储
 
         :param request: Request instance for ModifyAccessPeriod.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyAccessPeriodRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.ModifyAccessPeriodResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.876/tencentcloud/waf/v20180125/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,15 +557,15 @@
         :type SrcList: list of str
         :param IsHttp2: 是否开启HTTP2,开启HTTP2需要HTTPS支持
         :type IsHttp2: int
         :param HttpsRewrite: 表示是否强制跳转到HTTPS，1强制跳转Https，0不强制跳转
         :type HttpsRewrite: int
         :param Ports: 服务有多端口需要设置此字段
         :type Ports: list of PortItem
-        :param Edition: 版本：sparta-waf、clb-waf、cdn-waf
+        :param Edition: WAF实例类型，sparta-waf表示SAAS型WAF，clb-waf表示负载均衡型WAF，cdn-waf表示CDN上的Web防护能力
         :type Edition: str
         :param IsKeepAlive: 是否开启长连接，仅IP回源时可以用填次参数，域名回源时这个参数无效
         :type IsKeepAlive: str
         :param InstanceID: 实例id，上线之后带上此字段
         :type InstanceID: str
         :param Anycast: anycast IP类型开关： 0 普通IP 1 Anycast IP
         :type Anycast: int
@@ -579,14 +579,20 @@
         :type Ciphers: list of int
         :param CipherTemplate: 0:不支持选择：默认模版  1:通用型模版 2:安全型模版 3:自定义模版
         :type CipherTemplate: int
         :param ProxyReadTimeout: 300s
         :type ProxyReadTimeout: int
         :param ProxySendTimeout: 300s
         :type ProxySendTimeout: int
+        :param SniType: 0:关闭SNI；1:开启SNI，SNI=源请求host；2:开启SNI，SNI=修改为源站host；3：开启SNI，自定义host，SNI=SniHost；
+        :type SniType: int
+        :param SniHost: SniType=3时，需要填此参数，表示自定义的host；
+        :type SniHost: str
+        :param IpHeaders: is_cdn=3时，需要填此参数，表示自定义header
+        :type IpHeaders: list of str
         """
         self.Domain = None
         self.CertType = None
         self.IsCdn = None
         self.UpstreamType = None
         self.IsWebsocket = None
         self.LoadBalance = None
@@ -610,14 +616,17 @@
         self.Weights = None
         self.ActiveCheck = None
         self.TLSVersion = None
         self.Ciphers = None
         self.CipherTemplate = None
         self.ProxyReadTimeout = None
         self.ProxySendTimeout = None
+        self.SniType = None
+        self.SniHost = None
+        self.IpHeaders = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.CertType = params.get("CertType")
         self.IsCdn = params.get("IsCdn")
         self.UpstreamType = params.get("UpstreamType")
@@ -648,14 +657,17 @@
         self.Weights = params.get("Weights")
         self.ActiveCheck = params.get("ActiveCheck")
         self.TLSVersion = params.get("TLSVersion")
         self.Ciphers = params.get("Ciphers")
         self.CipherTemplate = params.get("CipherTemplate")
         self.ProxyReadTimeout = params.get("ProxyReadTimeout")
         self.ProxySendTimeout = params.get("ProxySendTimeout")
+        self.SniType = params.get("SniType")
+        self.SniHost = params.get("SniHost")
+        self.IpHeaders = params.get("IpHeaders")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2361,21 +2373,28 @@
         :type ToTime: str
         :param Domain: 查询的域名，如果查询所有域名数据，该参数不填写
         :type Domain: str
         :param Edition: 只有两个值有效，sparta-waf，clb-waf，不传则不过滤
         :type Edition: str
         :param InstanceID: WAF实例ID，不传则不过滤
         :type InstanceID: str
-        :param MetricName: 六个值可选：
+        :param MetricName: 十三个值可选：
 access-峰值qps趋势图
 botAccess- bot峰值qps趋势图
 down-下行峰值带宽趋势图
 up-上行峰值带宽趋势图
 attack-Web攻击总数趋势图
 cc-CC攻击总数趋势图
+StatusServerError-WAF返回给客户端状态码次数趋势图
+StatusClientError-WAF返回给客户端状态码次数趋势图
+StatusRedirect-WAF返回给客户端状态码次数趋势图
+StatusOk-WAF返回给客户端状态码次数趋势图
+UpstreamServerError-源站返回给WAF状态码次数趋势图
+UpstreamClientError-源站返回给WAF状态码次数趋势图
+UpstreamRedirect-源站返回给WAF状态码次数趋势图
         :type MetricName: str
         """
         self.FromTime = None
         self.ToTime = None
         self.Domain = None
         self.Edition = None
         self.InstanceID = None
@@ -3066,14 +3085,26 @@
         :type CipherTemplate: int
         :param ProxyReadTimeout: 300s
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProxyReadTimeout: int
         :param ProxySendTimeout: 300s
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProxySendTimeout: int
+        :param SniType: 0:关闭SNI；1:开启SNI，SNI=源请求host；2:开启SNI，SNI=修改为源站host；3：开启SNI，自定义host，SNI=SniHost；
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SniType: int
+        :param SniHost: SniType=3时，需要填此参数，表示自定义的host；
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SniHost: str
+        :param Weights: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Weights: list of str
+        :param IpHeaders: IsCdn=3时，表示自定义header
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpHeaders: list of str
         """
         self.HttpsRewrite = None
         self.HttpsUpstreamPort = None
         self.IsCdn = None
         self.IsGray = None
         self.IsHttp2 = None
         self.IsWebsocket = None
@@ -3092,14 +3123,18 @@
         self.IsKeepAlive = None
         self.ActiveCheck = None
         self.TLSVersion = None
         self.Ciphers = None
         self.CipherTemplate = None
         self.ProxyReadTimeout = None
         self.ProxySendTimeout = None
+        self.SniType = None
+        self.SniHost = None
+        self.Weights = None
+        self.IpHeaders = None
 
 
     def _deserialize(self, params):
         self.HttpsRewrite = params.get("HttpsRewrite")
         self.HttpsUpstreamPort = params.get("HttpsUpstreamPort")
         self.IsCdn = params.get("IsCdn")
         self.IsGray = params.get("IsGray")
@@ -3125,14 +3160,18 @@
         self.IsKeepAlive = params.get("IsKeepAlive")
         self.ActiveCheck = params.get("ActiveCheck")
         self.TLSVersion = params.get("TLSVersion")
         self.Ciphers = params.get("Ciphers")
         self.CipherTemplate = params.get("CipherTemplate")
         self.ProxyReadTimeout = params.get("ProxyReadTimeout")
         self.ProxySendTimeout = params.get("ProxySendTimeout")
+        self.SniType = params.get("SniType")
+        self.SniHost = params.get("SniHost")
+        self.Weights = params.get("Weights")
+        self.IpHeaders = params.get("IpHeaders")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3433,14 +3472,20 @@
         :type Level: int
         :param CdcClusters: 域名需要下发到的cdc集群列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type CdcClusters: list of str
         :param AlbType: 应用型负载均衡类型: clb或者apisix，默认clb
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlbType: str
+        :param IpHeaders: IsCdn=3时，需要填此参数，表示自定义header
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpHeaders: list of str
+        :param EngineType: 规则引擎类型， 1: menshen,   2:tiga
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EngineType: int
         """
         self.Domain = None
         self.DomainId = None
         self.MainDomain = None
         self.Mode = None
         self.Status = None
         self.State = None
@@ -3450,14 +3495,16 @@
         self.Region = None
         self.Edition = None
         self.FlowMode = None
         self.ClsStatus = None
         self.Level = None
         self.CdcClusters = None
         self.AlbType = None
+        self.IpHeaders = None
+        self.EngineType = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.DomainId = params.get("DomainId")
         self.MainDomain = params.get("MainDomain")
         self.Mode = params.get("Mode")
@@ -3474,14 +3521,16 @@
         self.Region = params.get("Region")
         self.Edition = params.get("Edition")
         self.FlowMode = params.get("FlowMode")
         self.ClsStatus = params.get("ClsStatus")
         self.Level = params.get("Level")
         self.CdcClusters = params.get("CdcClusters")
         self.AlbType = params.get("AlbType")
+        self.IpHeaders = params.get("IpHeaders")
+        self.EngineType = params.get("EngineType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4307,48 +4356,116 @@
         :param Down: 下行带宽峰值，单位B
         :type Down: int
         :param Attack: Web攻击次数
         :type Attack: int
         :param Cc: CC攻击次数
         :type Cc: int
         :param BotAccess: Bot qps
-注意：此字段可能返回 null，表示取不到有效值。
         :type BotAccess: int
+        :param StatusServerError: WAF返回给客户端状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusServerError: int
+        :param StatusClientError: WAF返回给客户端状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusClientError: int
+        :param StatusRedirect: WAF返回给客户端状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusRedirect: int
+        :param StatusOk: WAF返回给客户端状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusOk: int
+        :param UpstreamServerError: 源站返回给WAF状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpstreamServerError: int
+        :param UpstreamClientError: 源站返回给WAF状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpstreamClientError: int
+        :param UpstreamRedirect: 源站返回给WAF状态码次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpstreamRedirect: int
         """
         self.Time = None
         self.Access = None
         self.Up = None
         self.Down = None
         self.Attack = None
         self.Cc = None
         self.BotAccess = None
+        self.StatusServerError = None
+        self.StatusClientError = None
+        self.StatusRedirect = None
+        self.StatusOk = None
+        self.UpstreamServerError = None
+        self.UpstreamClientError = None
+        self.UpstreamRedirect = None
 
 
     def _deserialize(self, params):
         self.Time = params.get("Time")
         self.Access = params.get("Access")
         self.Up = params.get("Up")
         self.Down = params.get("Down")
         self.Attack = params.get("Attack")
         self.Cc = params.get("Cc")
         self.BotAccess = params.get("BotAccess")
+        self.StatusServerError = params.get("StatusServerError")
+        self.StatusClientError = params.get("StatusClientError")
+        self.StatusRedirect = params.get("StatusRedirect")
+        self.StatusOk = params.get("StatusOk")
+        self.UpstreamServerError = params.get("UpstreamServerError")
+        self.UpstreamClientError = params.get("UpstreamClientError")
+        self.UpstreamRedirect = params.get("UpstreamRedirect")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class PortInfo(AbstractModel):
-    """防护域名端口配置信息
+    """服务端口配置
 
     """
 
+    def __init__(self):
+        r"""
+        :param NginxServerId: Nginx的服务器id
+        :type NginxServerId: int
+        :param Port: 监听端口配置
+        :type Port: str
+        :param Protocol: 与端口对应的协议
+        :type Protocol: str
+        :param UpstreamPort: 回源端口
+        :type UpstreamPort: str
+        :param UpstreamProtocol: 回源协议
+        :type UpstreamProtocol: str
+        """
+        self.NginxServerId = None
+        self.Port = None
+        self.Protocol = None
+        self.UpstreamPort = None
+        self.UpstreamProtocol = None
+
+
+    def _deserialize(self, params):
+        self.NginxServerId = params.get("NginxServerId")
+        self.Port = params.get("Port")
+        self.Protocol = params.get("Protocol")
+        self.UpstreamPort = params.get("UpstreamPort")
+        self.UpstreamProtocol = params.get("UpstreamProtocol")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class PortItem(AbstractModel):
     """防护域名端口配置信息
 
     """
 
     def __init__(self):
```

### Comparing `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.876/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.875'
+__version__ = '3.0.876'
```

### Comparing `tencentcloud-sdk-python-waf-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.876/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.875/setup.py` & `tencentcloud-sdk-python-waf-3.0.876/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.876/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

