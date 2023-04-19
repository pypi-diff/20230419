# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.875.tar", last modified: Tue Apr 18 00:38:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.876.tar", last modified: Wed Apr 19 00:27:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.875.tar` & `tencentcloud-sdk-python-ess-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49089 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   216316 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49192 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217979 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.875/README.rst` & `tencentcloud-sdk-python-ess-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateBatchCancelFlowUrl(self, request):
-        """指定需要批量撤回的签署流程Id，获取批量撤销链接
-        客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回
+        """注：此接口建会废弃，请使用撤销单个签署流程（CancelFlow）接口。
+        指定需要批量撤回的签署流程Id，获取批量撤销链接。
+        客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回。
 
         :param request: Request instance for CreateBatchCancelFlowUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.876/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
 class BindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
     """BindEmployeeUserIdWithClientOpenId请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: OpenId与UserId二选一必填一个，当传入客户系统openId，传入的openId需与电子签员工userId绑定，且渠道channel必填，channel值为INTEGRATE，否则传入userId
+        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param UserId: 电子签系统员工UserId
         :type UserId: str
         :param OpenId: 客户系统OpenId
         :type OpenId: str
         """
         self.Operator = None
@@ -960,15 +960,15 @@
         r"""
         :param Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId代发合同。
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param FlowId: 签署流程编号,由CreateFlow接口返回
         :type FlowId: str
         :param TemplateId: 用户上传的模板ID
         :type TemplateId: str
-        :param FileNames: 文件名列表，单个文件名最大长度200个字符，暂时仅支持单文件发起
+        :param FileNames: 文件名列表，单个文件名最大长度200个字符，暂时仅支持单文件发起。设置后流程对应的文件名称当前设置的值。
         :type FileNames: list of str
         :param FormFields: 内容控件信息数组
         :type FormFields: list of FormField
         :param NeedPreview: 是否需要生成预览文件 默认不生成；
 预览链接有效期300秒；
         :type NeedPreview: bool
         :param PreviewType: 预览链接类型 默认:0-文件流, 1- H5链接 注意:此参数在NeedPreview 为true 时有效,
@@ -2320,30 +2320,38 @@
         :param SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param AutoSignConfig: 自动签开通，签署相关配置
         :type AutoSignConfig: :class:`tencentcloud.ess.v20201111.models.AutoSignConfig`
         :param UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
         :type UrlType: str
+        :param NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短息通知。
+        :type NotifyType: str
+        :param NotifyAddress: 若上方填写为 SMS，则此处为手机号
+        :type NotifyAddress: str
         """
         self.Operator = None
         self.SceneKey = None
         self.AutoSignConfig = None
         self.UrlType = None
+        self.NotifyType = None
+        self.NotifyAddress = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.SceneKey = params.get("SceneKey")
         if params.get("AutoSignConfig") is not None:
             self.AutoSignConfig = AutoSignConfig()
             self.AutoSignConfig._deserialize(params.get("AutoSignConfig"))
         self.UrlType = params.get("UrlType")
+        self.NotifyType = params.get("NotifyType")
+        self.NotifyAddress = params.get("NotifyAddress")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2397,15 +2405,15 @@
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Employees: 待移除员工的信息，userId和openId二选一，必填一个
         :type Employees: list of Staff
-        :param Agent: 代理信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.Employees = None
         self.Agent = None
 
 
@@ -2939,16 +2947,14 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Organization: 企业组织相关信息，一般不用填
-        :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Offset: 查询偏移位置，默认0
         :type Offset: int
         :param Limit: 查询个数，默认20，最大200
         :type Limit: int
         :param Filters: 搜索条件，具体参考Filter结构体。本接口取值：template-id：按照【 **模板唯一标识** 】进行过滤
@@ -2957,53 +2963,55 @@
 IsChannel=false时，ApplicationId参数不起任何作用。
 IsChannel=true时，ApplicationId为空，查询所有第三方应用集成平台企业模板列表；ApplicationId不为空，查询指定应用下的模板列表
 ApplicationId为空，查询所有应用下的模板列表
         :type ApplicationId: str
         :param IsChannel: 默认为false，查询SaaS模板库列表；
 为true，查询第三方应用集成平台企业模板库管理列表
         :type IsChannel: bool
-        :param GenerateSource: 暂未开放
-        :type GenerateSource: int
         :param ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
         :type ContentType: int
+        :param Organization: 暂未开放
+        :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
+        :param GenerateSource: 暂未开放
+        :type GenerateSource: int
         """
         self.Operator = None
-        self.Organization = None
         self.Agent = None
         self.Offset = None
         self.Limit = None
         self.Filters = None
         self.ApplicationId = None
         self.IsChannel = None
-        self.GenerateSource = None
         self.ContentType = None
+        self.Organization = None
+        self.GenerateSource = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
-        if params.get("Organization") is not None:
-            self.Organization = OrganizationInfo()
-            self.Organization._deserialize(params.get("Organization"))
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.ApplicationId = params.get("ApplicationId")
         self.IsChannel = params.get("IsChannel")
-        self.GenerateSource = params.get("GenerateSource")
         self.ContentType = params.get("ContentType")
+        if params.get("Organization") is not None:
+            self.Organization = OrganizationInfo()
+            self.Organization._deserialize(params.get("Organization"))
+        self.GenerateSource = params.get("GenerateSource")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3276,15 +3284,15 @@
         :type Limit: int
         :param Offset: 页面偏移量
         :type Offset: int
         :param Name: 查询成员企业的企业名，模糊匹配
         :type Name: str
         :param Status: 成员企业加入集团的当前状态:1-待授权;2-已授权待激活;3-拒绝授权;4-已解除;5-已加入
         :type Status: int
-        :param Export: 是否到处当前成员企业数据
+        :param Export: 是否导出当前成员企业数据
         :type Export: bool
         :param Id: 成员企业id
         :type Id: str
         """
         self.Operator = None
         self.Limit = None
         self.Offset = None
@@ -4488,15 +4496,15 @@
         :type Alias: str
         :param OrganizationId: 成员企业id
 注意：此字段可能返回 null，表示取不到有效值。
         :type OrganizationId: str
         :param UpdateTime: 更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: int
-        :param Status: 成员企业状态
+        :param Status: 成员企业加入集团的当前状态:1-待授权;2-已授权待激活;3-拒绝授权;4-已解除;5-已加入
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param IsMainOrganization: 是否为集团主企业
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsMainOrganization: bool
         :param IdCardNumber: 企业社会信用代码
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4762,23 +4770,23 @@
 class OrganizationInfo(AbstractModel):
     """机构信息
 
     """
 
     def __init__(self):
         r"""
-        :param OrganizationId: 机构在平台的编号
+        :param OrganizationId: 机构在平台的编号，内部字段，暂未开放
         :type OrganizationId: str
-        :param Channel: 用户渠道
+        :param Channel: 用户渠道，内部字段，暂未开放
         :type Channel: str
-        :param OrganizationOpenId: 用户在渠道的机构编号
+        :param OrganizationOpenId: 用户在渠道的机构编号，内部字段，暂未开放
         :type OrganizationOpenId: str
-        :param ClientIp: 用户真实的IP
+        :param ClientIp: 用户真实的IP，内部字段，暂未开放
         :type ClientIp: str
-        :param ProxyIp: 机构的代理IP
+        :param ProxyIp: 机构的代理IP，内部字段，暂未开放
         :type ProxyIp: str
         """
         self.OrganizationId = None
         self.Channel = None
         self.OrganizationOpenId = None
         self.ClientIp = None
         self.ProxyIp = None
@@ -4802,17 +4810,17 @@
 class PdfVerifyResult(AbstractModel):
     """合同文件验签单个结果结构体
 
     """
 
     def __init__(self):
         r"""
-        :param VerifyResult: 验签结果
+        :param VerifyResult: 验签结果。0-签名域未签名；1-验签成功； 3-验签失败；4-未找到签名域：文件内没有签名域；5-签名值格式不正确。
         :type VerifyResult: int
-        :param SignPlatform: 签署平台
+        :param SignPlatform: 签署平台，如果文件是在腾讯电子签平台签署，则返回腾讯电子签，如果文件不在腾讯电子签平台签署，则返回其他平台。
         :type SignPlatform: str
         :param SignerName: 签署人名称
         :type SignerName: str
         :param SignTime: 签署时间
         :type SignTime: int
         :param SignAlgorithm: 签名算法
         :type SignAlgorithm: str
@@ -4876,15 +4884,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param RecipientId: 签署参与者ID
         :type RecipientId: str
-        :param RecipientType: 参与者类型（ENTERPRISE/INDIVIDUAL）
+        :param RecipientType: 参与者类型。默认为空。ENTERPRISE-企业；INDIVIDUAL-个人；PROMOTER-发起方
         :type RecipientType: str
         :param Description: 描述信息
         :type Description: str
         :param RoleName: 角色名称
         :type RoleName: str
         :param RequireValidation: 是否需要验证，默认为false
         :type RequireValidation: bool
@@ -4896,15 +4904,15 @@
         :type RequireDelivery: bool
         :param Email: 邮箱地址
         :type Email: str
         :param Mobile: 电话号码
         :type Mobile: str
         :param UserId: 关联的用户ID
         :type UserId: str
-        :param DeliveryMethod: 发送方式（EMAIL/MOBILE）
+        :param DeliveryMethod: 发送方式。默认为EMAIL。EMAIL-邮件；MOBILE-手机短信；WECHAT-微信通知
         :type DeliveryMethod: str
         :param RecipientExtra: 附属信息
         :type RecipientExtra: str
         """
         self.RecipientId = None
         self.RecipientType = None
         self.Description = None
@@ -5457,15 +5465,15 @@
         :type Status: int
         :param Creator: 模板的创建人
         :type Creator: str
         :param CreatedOn: 模板创建的时间戳（精确到秒）
         :type CreatedOn: int
         :param Promoter: 发起人角色信息
         :type Promoter: :class:`tencentcloud.ess.v20201111.models.Recipient`
-        :param Available: 模板可用状态，取值：0未知，但默认会被转成启用；1启用（默认），2停用
+        :param Available: 模板可用状态，取值：1启用（默认），2停用
         :type Available: int
         :param OrganizationId: 模板创建组织id
         :type OrganizationId: str
         :param PreviewUrl: 模板预览链接
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
         :param TemplateVersion: 模板版本。默认为空时，全数字字符，初始版本为yyyyMMdd001。
@@ -5550,15 +5558,15 @@
 class UnbindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
     """UnbindEmployeeUserIdWithClientOpenId请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: OpenId与UserId二选一必填一个，当传入客户系统openId，传入的openId需与电子签员工userId绑定，且渠道channel必填，channel值为INTEGRATE，否则传入userId
+        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param UserId: 电子签系统员工UserId
         :type UserId: str
         :param OpenId: 客户系统OpenId
         :type OpenId: str
         """
         self.Operator = None
@@ -5607,37 +5615,37 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Agent: 代理信息
-        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Employees: 员工信息
         :type Employees: list of Staff
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
-        self.Agent = None
         self.Employees = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
-        if params.get("Agent") is not None:
-            self.Agent = Agent()
-            self.Agent._deserialize(params.get("Agent"))
         if params.get("Employees") is not None:
             self.Employees = []
             for item in params.get("Employees"):
                 obj = Staff()
                 obj._deserialize(item)
                 self.Employees.append(obj)
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5797,21 +5805,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param UserId: 用户在平台的编号
         :type UserId: str
-        :param Channel: 用户的来源渠道
+        :param Channel: 用户的来源渠道，一般不用传，特定场景根据接口说明传值
         :type Channel: str
-        :param OpenId: 用户在渠道的编号
+        :param OpenId: 用户在渠道的编号，一般不用传，特定场景根据接口说明传值
         :type OpenId: str
-        :param ClientIp: 用户真实IP
+        :param ClientIp: 用户真实IP，内部字段，暂未开放
         :type ClientIp: str
-        :param ProxyIp: 用户代理IP
+        :param ProxyIp: 用户代理IP，内部字段，暂未开放
         :type ProxyIp: str
         """
         self.UserId = None
         self.Channel = None
         self.OpenId = None
         self.ClientIp = None
         self.ProxyIp = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.876/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.875/setup.py` & `tencentcloud-sdk-python-ess-3.0.876/setup.py`

 * *Files identical despite different names*

