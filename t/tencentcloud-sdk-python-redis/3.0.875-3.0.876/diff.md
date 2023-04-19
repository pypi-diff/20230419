# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.875.tar", last modified: Tue Apr 18 00:48:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.876.tar", last modified: Wed Apr 19 00:35:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.875.tar` & `tencentcloud-sdk-python-redis-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86576 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   288654 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:48:49.000000 tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86582 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   290895 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:35:13.000000 tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.875/README.rst` & `tencentcloud-sdk-python-redis-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateInstances(self, request):
-        """本接口(CreateInstances)用于创建redis实例。
+        """本接口（CreateInstances）用于创建 Redis 实例。
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.CreateInstancesRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.CreateInstancesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.875/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.876/tencentcloud/redis/v20180412/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -935,66 +935,93 @@
 class CreateInstancesRequest(AbstractModel):
     """CreateInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TypeId: 实例类型：2 – Redis2.8内存版(标准架构)，3 – CKV 3.2内存版(标准架构)，4 – CKV 3.2内存版(集群架构)，6 – Redis4.0内存版(标准架构)，7 – Redis4.0内存版(集群架构)，8 – Redis5.0内存版(标准架构)，9 – Redis5.0内存版(集群架构)，15 – Redis6.0内存版(标准架构)，16 – Redis6.0内存版(集群架构)。
+        :param TypeId: 实例类型。
+<ul><li>2：Redis 2.8 内存版（标准架构）。</li><li>3：CKV 3.2 内存版（标准架构）。</li><li>4：CKV 3.2 内存版（集群架构）。</li><li>6：Redis 4.0 内存版（标准架构）。</li><li>7：Redis 4.0 内存版（集群架构）。</li><li>8：Redis 5.0 内存版（标准架构）。</li><li>9：Redis 5.0 内存版（集群架构）。</li><li>15：Redis 6.2 内存版（标准架构）。</li><li>16：Redis 6.2 内存版（集群架构）。</li></ul>
         :type TypeId: int
-        :param MemSize: 内存容量，单位为MB， 数值需为1024的整数倍，具体规格以 [查询产品售卖规格](https://cloud.tencent.com/document/api/239/30600) 返回的规格为准。
-TypeId为标准架构时，MemSize是实例总内存容量；TypeId为集群架构时，MemSize是单分片内存容量。
+        :param MemSize: 内存容量，单位为MB， 数值需为1024的整数倍。具体规格，请通过 [DescribeProductInfo](https://cloud.tencent.com/document/api/239/30600) 接口查询全地域的售卖规格。
+- **TypeId**为标准架构时，**MemSize**是实例总内存容量；
+- **TypeId**为集群架构时，**MemSize**是单分片内存容量。
         :type MemSize: int
-        :param GoodsNum: 实例数量，单次购买实例数量以 [查询产品售卖规格](https://cloud.tencent.com/document/api/239/30600) 返回的规格为准。
+        :param GoodsNum: 实例数量，单次购买实例数量。具体信息，请通过 [DescribeProductInfo](https://cloud.tencent.com/document/api/239/30600) 接口查询全地域的售卖规格。
         :type GoodsNum: int
-        :param Period: 购买时长，在创建包年包月实例的时候需要填写，按量计费实例填1即可，单位：月，取值范围 [1,2,3,4,5,6,7,8,9,10,11,12,24,36]。
+        :param Period: 购买实例的时长。
+- 若 **BillingMode**为**1**，即计费方式为包年包月时，需设置该参数，指定所购买实例的时长。单位：月，取值范围 [1,2,3,4,5,6,7,8,9,10,11,12,24,36]。
+- 若 **BillingMode**为**0**，即计费方式为按量计费时，该参数配置为1。
         :type Period: int
-        :param BillingMode: 付费方式:0-按量计费，1-包年包月。
+        :param BillingMode: 计费方式。
+- 0：按量计费。
+- 1：包年包月。
         :type BillingMode: int
         :param ZoneId: 实例所属的可用区ID，可参考[地域和可用区](https://cloud.tencent.com/document/product/239/4106)  。
         :type ZoneId: int
-        :param Password: 实例密码，当输入参数NoAuth为true且使用私有网络VPC时，Password为非必填，否则Password为必填参数。
-当实例类型TypeId为Redis2.8、4.0和5.0时，其密码格式为：8-30个字符，至少包含小写字母、大写字母、数字和字符 ()`~!@#$%^&*-+=_|{}[]:;<>,.?/ 中的2种，不能以"/"开头；
-当实例类型TypeId为CKV 3.2时，其密码格式为：8-30个字符，必须包含字母和数字 且 不包含其他字符。
+        :param Password: 访问实例的密码。
+- 当输入参数**NoAuth**为**true**时，指设置实例为免密码访问，Password可不用配置，否则Password为必填参数。
+- 当实例类型**TypeId**为Redis 2.8 内存版标准架构、Redis 4.0、5.0、6.0内存版标准架构或集群架构时，其密码复杂度要求为：8-30个字符，至少包含小写字母、大写字母、数字和字符()`~!@#$%^&*-+=_|{}[]:;<>,.?/ 中的2种，不能以"/"开头。
+- 当实例类型**TypeId**为CKV 3.2 内存版标准架构或集群架构时，其密码复杂度为：8-30个字符，必须包含字母和数字，且 不包含其他字符。
         :type Password: str
-        :param VpcId: 私有网络ID，如果不传则默认选择基础网络，请使用私有网络列表查询，如：vpc-sad23jfdfk。
+        :param VpcId: 私有网络ID。如果不配置该参数则默认选择基础网络。请登录 [私有网络](https://console.cloud.tencent.com/vpc)控制台查询具体的ID。
         :type VpcId: str
-        :param SubnetId: 基础网络下， subnetId无效； vpc子网下，取值以查询子网列表，如：subnet-fdj24n34j2。
+        :param SubnetId: 私有网络VPC的子网。基础网络下， 该参数无需配置。请登录 [私有网络](https://console.cloud.tencent.com/vpc)控制台查询子网列表获取具体的 ID。
         :type SubnetId: str
-        :param ProjectId: 项目id，取值以用户账户>用户账户相关接口查询>项目列表返回的projectId为准。
+        :param ProjectId: 项目 ID。请登录[Redis控制台](https://console.cloud.tencent.com/redis#/)，在右上角的账户信息菜单中，选择**项目管理**查询项目 ID。
         :type ProjectId: int
-        :param AutoRenew: 自动续费标识。0 - 默认状态（手动续费）；1 - 自动续费；2 - 明确不自动续费。
+        :param AutoRenew: 自动续费标识。
+- 0：默认状态（手动续费）。
+- 1：自动续费。
+- 2：到期不续费。
         :type AutoRenew: int
-        :param SecurityGroupIdList: 安全组id数组。
+        :param SecurityGroupIdList: 安全组 ID 数组。请通过[DescribeInstanceSecurityGroup](https://cloud.tencent.com/document/product/239/34447)接口获取实例的安全组 ID。
         :type SecurityGroupIdList: list of str
-        :param VPort: 用户自定义的端口 不填则默认为6379，范围[1024,65535]。
+        :param VPort: 用户自定义的网络端口。默认为6379，范围为 [1024,65535]。
         :type VPort: int
-        :param RedisShardNum: 实例分片数量，购买标准版实例不需要填写，集群版分片数量范围[3,5,8,12,16,24,32,64,96,128]。
+        :param RedisShardNum: 实例分片数量。
+- 标准版实例无需配置该参数。
+- 集群版实例，分片数量范围为：[1、3、5、8、12、16、24、32、40、48、64、80、96、128]。
         :type RedisShardNum: int
-        :param RedisReplicasNum: 实例副本数量，Redis 2.8标准版、CKV标准版只支持1副本，4.0、5.0标准版和集群版支持1-5个副本。
+        :param RedisReplicasNum: 实例副本数量。
+- Redis 内存版 4.0、5.0、6.2 标准架构和集群架构支持副本数量范围为[1,5]。
+- Redis 2.8标准版、CKV标准版只支持1副本。
         :type RedisReplicasNum: int
-        :param ReplicasReadonly: 是否支持副本只读，Redis 2.8标准版、CKV标准版不支持副本只读，开启副本只读，实例将自动读写分离，写请求路由到主节点，读请求路由到副本节点，如需开启副本只读建议副本数>=2。
+        :param ReplicasReadonly: 标识实例是否需支持副本只读。
+- Redis 2.8 标准版、CKV标准版不支持副本只读。
+- 开启副本只读，实例将自动读写分离，写请求路由到主节点，读请求路由到副本节点。
+- 如需开启副本只读，建议副本数量大于等于2。
         :type ReplicasReadonly: bool
-        :param InstanceName: 实例名称，长度小于60的中文/英文/数字/"-"/"_"。
+        :param InstanceName: 实例名称。命名要求：仅支持长度小于60的中文、英文或者数字，短划线"-"、下划线"_"。
         :type InstanceName: str
-        :param NoAuth: 是否支持免密，true-免密实例，false-非免密实例，默认为非免密实例，仅VPC网络的实例支持免密码访问。
+        :param NoAuth: 配置实例是否支持免密码访问。
+- true：免密访问实例。
+- false：非免密访问实例。默认为非免密方式，仅VPC网络的实例支持免密码访问。
         :type NoAuth: bool
-        :param NodeSet: 实例的节点信息，目前支持传入节点的类型（主节点或者副本节点），节点的可用区。单可用区部署不需要传递此参数。
+        :param NodeSet: 实例的节点信息，包含节点 ID、节点类型、节点可用区 ID等。具体信息，请参见[RedisNodeInfo ](https://cloud.tencent.com/document/product/239/20022)。
+目前支持传入节点的类型（主节点或者副本节点），节点的可用区。单可用区部署不需要传递此参数。
         :type NodeSet: list of RedisNodeInfo
-        :param ResourceTags: 购买实例绑定标签
+        :param ResourceTags: 给实例设定标签。
         :type ResourceTags: list of ResourceTag
-        :param ZoneName: 实例所属的可用区名称，可参考[地域和可用区](https://cloud.tencent.com/document/product/239/4106)  。
+        :param ZoneName: 指定实例所属的可用区名称。具体信息，请参见[地域和可用区](https://cloud.tencent.com/document/product/239/4106)  。
         :type ZoneName: str
-        :param TemplateId: 创建实例需要应用的参数模板ID，不传则应用默认的参数模板
+        :param TemplateId: 指定实例相关的参数模板 ID。
+- 若不配置该参数，则系统会依据所选择的兼容版本及架构，自动适配对应的默认模板。
+- 请通过[DescribeParamTemplates](https://cloud.tencent.com/document/product/239/58750)接口，查询实例的参数模板列表，获取模板 ID 编号。
         :type TemplateId: str
-        :param DryRun: false ：默认值,发送正常请求，通过检查后直接创建实例 true：发送检查请求，不会创建实例。
+        :param DryRun: 内部参数，标识创建实例是否需要检查。
+- false ：默认值。发送正常请求，通过检查后直接创建实例。
+- true：发送检查请求，不会创建实例。
         :type DryRun: bool
-        :param ProductVersion: "local"本地盘版，"cloud"云盘版，"cdc"独享集群版，如果不传默认发货为本地盘版本
+        :param ProductVersion: 指定实例的产品版本。
+- local：本地盘版。
+- cloud：云盘版，
+- cdc：独享集群版。如果不传默认发货为本地盘版本。
         :type ProductVersion: str
-        :param RedisClusterId: 独享集群id，ProductVersion="cdc"时必传
+        :param RedisClusterId: 独享集群 ID。当**ProductVersion**设置为**cdc**时，该参数必须设置。
         :type RedisClusterId: str
         """
         self.TypeId = None
         self.MemSize = None
         self.GoodsNum = None
         self.Period = None
         self.BillingMode = None
@@ -1068,17 +1095,17 @@
 class CreateInstancesResponse(AbstractModel):
     """CreateInstances返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DealId: 交易的ID
+        :param DealId: 交易的ID。
         :type DealId: str
-        :param InstanceIds: 实例ID
+        :param InstanceIds: 实例ID。
         :type InstanceIds: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DealId = None
         self.InstanceIds = None
         self.RequestId = None
@@ -4707,31 +4734,35 @@
 class InstanceClusterShard(AbstractModel):
     """实例分片列表信息
 
     """
 
     def __init__(self):
         r"""
-        :param ShardName: 分片节点名称
+        :param ShardName: 分片节点名称。
         :type ShardName: str
-        :param ShardId: 分片节点Id
+        :param ShardId: 分片节点序号。
         :type ShardId: str
-        :param Role: 角色
+        :param Role: 分片节点的角色。
+- 0：主节点。
+- 1：副本节点。
         :type Role: int
-        :param Keys: Key数量
+        :param Keys: Key数量。
         :type Keys: int
-        :param Slots: slot信息
+        :param Slots: Slot信息。
         :type Slots: str
-        :param Storage: 使用容量
+        :param Storage: 已使用容量。
         :type Storage: int
-        :param StorageSlope: 容量倾斜率
+        :param StorageSlope: 容量倾斜率。
         :type StorageSlope: float
-        :param Runid: 实例运行时节点Id
+        :param Runid: 实例运行时节点 ID。
         :type Runid: str
-        :param Connected: 服务状态：0-down；1-on
+        :param Connected: 服务状态。
+- 0：down。
+- 1：on。
         :type Connected: int
         """
         self.ShardName = None
         self.ShardId = None
         self.Role = None
         self.Keys = None
         self.Slots = None
@@ -5109,15 +5140,16 @@
 
     def __init__(self):
         r"""
         :param InstanceName: 实例名称。
         :type InstanceName: str
         :param InstanceId: 实例 ID。
         :type InstanceId: str
-        :param Appid: 用户的 AppID。
+        :param Appid: 用户APPID。APPID是与账号ID有唯一对应关系的应用 ID，部分腾讯云产品会使用此 APPID。
+
         :type Appid: int
         :param ProjectId: 项目 ID。
         :type ProjectId: int
         :param RegionId: 地域 ID。<ul><li>1：广州。</li><li>4：上海。</li><li>5：中国香港。</li><li>6：多伦多。</li> <li>7：上海金融。</li> <li>8：北京。</li> <li>9：新加坡。</li> <li>11：深圳金融。</li> <li>15：美西（硅谷）。</li><li>16：成都。</li><li>17：法兰克福。</li><li>18：首尔。</li><li>19：重庆。</li><li>21：孟买。</li><li>22：美东（弗吉尼亚）。</li><li>23：曼谷。</li><li>24：莫斯科。</li><li>25：东京。</li></ul>
         :type RegionId: int
         :param ZoneId: 区域 ID。
         :type ZoneId: int
@@ -5127,17 +5159,17 @@
         :type SubnetId: int
         :param Status: 实例当前状态。<ul><li>0：待初始化。</li><li>1：实例在流程中。</li><li>2：实例运行中。</li><li>-2：实例已隔离。</li><li>-3：实例待删除。</li></ul>
         :type Status: int
         :param WanIp: 实例 VIP。
         :type WanIp: str
         :param Port: 实例端口号。
         :type Port: int
-        :param Createtime: 实例创建时间。
+        :param Createtime: 实例创建时间。格式如：2020-01-15 10:20:00。
         :type Createtime: str
-        :param Size: 实例容量大小，单位：MB。
+        :param Size: 实例内存容量大小。单位：MB，1MB=1024KB。
         :type Size: float
         :param SizeUsed: 该字段已废弃。请使用腾讯云可观测平台API 接口 [GetMonitorData](https://cloud.tencent.com/document/product/248/31014) 获取实例已使用的内存容量。
         :type SizeUsed: float
         :param Type: 实例类型。
 - 2：Redis 2.8内存版（标准架构）。
 - 3：CKV 3.2内存版（标准架构）。
 - 4：CKV 3.2内存版（集群架构）。
@@ -5147,29 +5179,29 @@
 - 8：Redis 5.0内存版（标准架构）。
 - 9：Redis 5.0内存版（集群架构）。
 - 15：Redis 6.2内存版（标准架构）。
 - 16：Redis 6.2内存版（集群架构）。
         :type Type: int
         :param AutoRenewFlag: 实例是否设置自动续费标识。<ul><li>1：设置自动续费。</li><li>0：未设置自动续费。</li></ul>
         :type AutoRenewFlag: int
-        :param DeadlineTime: 实例到期时间。
+        :param DeadlineTime: 包年包月计费实例到期的时间。
         :type DeadlineTime: str
         :param Engine: 引擎：社区版Redis、腾讯云CKV。
         :type Engine: str
         :param ProductType: 产品类型。<ul><li>standalone：标准版。</li><li>cluster ：集群版。</li></ul>
         :type ProductType: str
         :param UniqVpcId: vpc网络id，例如vpc-fk33jsf43kgv。
         :type UniqVpcId: str
         :param UniqSubnetId: vpc网络下子网id，例如：subnet-fd3j6l35mm0。
         :type UniqSubnetId: str
         :param BillingMode: 计费模式。<ul><li>0：按量计费。</li><li>1：包年包月。</li></ul>
         :type BillingMode: int
         :param InstanceTitle: 实例运行状态描述：如”实例运行中“。
         :type InstanceTitle: str
-        :param OfflineTime: 计划下线时间。
+        :param OfflineTime: 已隔离实例默认下线时间。按量计费实例隔离后默认两小时后下线，包年包月默认7天后下线。格式如：2020-02-15 10:20:00。
         :type OfflineTime: str
         :param SubStatus: 流程中的实例，返回子状态。
         :type SubStatus: int
         :param Tags: 反亲和性标签。
         :type Tags: list of str
         :param InstanceNode: 实例节点信息。
         :type InstanceNode: list of InstanceNode
@@ -5177,15 +5209,15 @@
         :type RedisShardSize: int
         :param RedisShardNum: 分片数量。
         :type RedisShardNum: int
         :param RedisReplicasNum: 副本数量。
         :type RedisReplicasNum: int
         :param PriceId: 计费 ID。
         :type PriceId: int
-        :param CloseTime: 隔离时间。
+        :param CloseTime: 实例隔离开始的时间。
         :type CloseTime: str
         :param SlaveReadWeight: 从节点读取权重。
         :type SlaveReadWeight: int
         :param InstanceTags: 实例关联的标签信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceTags: list of InstanceTagInfo
         :param ProjectName: 项目名称。
@@ -5214,15 +5246,15 @@
         :type ReadOnly: int
         :param RemainBandwidthDuration: 内部参数，用户可忽略。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RemainBandwidthDuration: str
         :param DiskSize: Redis实例请忽略该参数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiskSize: int
-        :param MonitorVersion: 监控版本。<ul><li>1m：1分钟粒度监控。</li><li>5s：5秒粒度监控。</li></ul>
+        :param MonitorVersion: 监控版本。<ul><li>1m：1分钟粒度监控。目前该监控粒度已下线，具体信息，请参见[云数据库 Redis 1分钟粒度下线公告](https://cloud.tencent.com/document/product/239/80653)。</li><li>5s：5秒粒度监控。</li></ul>
 注意：此字段可能返回 null，表示取不到有效值。
         :type MonitorVersion: str
         :param ClientLimitMin: 客户端最大连接数可设置的最小值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClientLimitMin: int
         :param ClientLimitMax: 客户端最大连接数可设置的最大值。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5232,15 +5264,15 @@
         :type NodeSet: list of RedisNodeInfo
         :param Region: 实例所在的地域信息，比如ap-guangzhou。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Region: str
         :param WanAddress: 外网地址。
 注意：此字段可能返回 null，表示取不到有效值。
         :type WanAddress: str
-        :param PolarisServer: 北极星服务地址。
+        :param PolarisServer: 北极星服务地址，内部使用。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PolarisServer: str
         :param CurrentProxyVersion: 实例当前Proxy版本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type CurrentProxyVersion: str
         :param CurrentRedisVersion: 实例当前Cache小版本。
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-redis-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.876/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.875/setup.py` & `tencentcloud-sdk-python-redis-3.0.876/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.875/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.876/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

