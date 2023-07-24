# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.940.tar", last modified: Fri Jul 21 00:28:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.941.tar", last modified: Mon Jul 24 00:36:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.940.tar` & `tencentcloud-sdk-python-ess-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    62054 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   432941 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    62111 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   437808 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:36:55.000000 tencentcloud-sdk-python-ess-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/setup.py` & `tencentcloud-sdk-python-ess-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.940'
+__version__ = '3.0.941'
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,19 +245,20 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowApprovers(self, request):
-        """补充签署流程本企业签署人信息
-        适用场景：在通过模板或者文件发起合同时，若未指定本企业签署人信息，则流程发起后，可以调用此接口补充签署人。
-        同一签署人可以补充多个员工作为候选签署人,最终签署人取决于谁先领取合同完成签署。
-
-        注：目前暂时只支持补充来源于企业微信的员工作为候选签署人
+        """### 适用场景
+        在通过模板或者文件发起合同时，若未指定企业签署人信息，则流程发起后，可以调用此接口补充或签签署人。
+        同一签署人可以补充多个员工作为或签签署人,最终实际签署人取决于谁先领取合同完成签署。
+        ### 限制条件
+        -  本企业(发起方企业)支持通过企业微信UserId 或者 姓名+手机号补充
+        - 他方企业仅支持通过姓名+手机号补充
 
         :param request: Request instance for CreateFlowApprovers.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowApproversRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowApproversResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.941/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,18 +654,21 @@
         r"""
         :param _Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定。（参数参考示例）
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _UserId: 电子签系统员工UserId
         :type UserId: str
         :param _OpenId: 客户系统OpenId
         :type OpenId: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._UserId = None
         self._OpenId = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -683,21 +686,32 @@
     def OpenId(self):
         return self._OpenId
 
     @OpenId.setter
     def OpenId(self, OpenId):
         self._OpenId = OpenId
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._UserId = params.get("UserId")
         self._OpenId = params.get("OpenId")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2252,19 +2266,24 @@
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _FlowId: 签署流程编号
         :type FlowId: str
         :param _Approvers: 补充签署人信息
         :type Approvers: list of FillApproverInfo
         :param _Initiator: 企微消息中的发起人
         :type Initiator: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作
+
+
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._FlowId = None
         self._Approvers = None
         self._Initiator = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -2290,27 +2309,38 @@
     def Initiator(self):
         return self._Initiator
 
     @Initiator.setter
     def Initiator(self, Initiator):
         self._Initiator = Initiator
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._FlowId = params.get("FlowId")
         if params.get("Approvers") is not None:
             self._Approvers = []
             for item in params.get("Approvers"):
                 obj = FillApproverInfo()
                 obj._deserialize(item)
                 self._Approvers.append(obj)
         self._Initiator = params.get("Initiator")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5585,22 +5615,25 @@
         :type UrlType: str
         :param _NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短信通知。
         :type NotifyType: str
         :param _NotifyAddress: 若上方填写为 SMS，则此处为手机号
         :type NotifyAddress: str
         :param _ExpiredTime: 链接的过期时间，格式为Unix时间戳，不能早于当前时间，且最大为30天。如果不传，默认有效期为7天。
         :type ExpiredTime: int
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._SceneKey = None
         self._AutoSignConfig = None
         self._UrlType = None
         self._NotifyType = None
         self._NotifyAddress = None
         self._ExpiredTime = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -5650,27 +5683,38 @@
     def ExpiredTime(self):
         return self._ExpiredTime
 
     @ExpiredTime.setter
     def ExpiredTime(self, ExpiredTime):
         self._ExpiredTime = ExpiredTime
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._SceneKey = params.get("SceneKey")
         if params.get("AutoSignConfig") is not None:
             self._AutoSignConfig = AutoSignConfig()
             self._AutoSignConfig._deserialize(params.get("AutoSignConfig"))
         self._UrlType = params.get("UrlType")
         self._NotifyType = params.get("NotifyType")
         self._NotifyAddress = params.get("NotifyAddress")
         self._ExpiredTime = params.get("ExpiredTime")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8213,28 +8257,56 @@
 
     """
 
     def __init__(self):
         r"""
         :param _AuthCode: 电子签小程序跳转客户小程序时携带的授权查看码
         :type AuthCode: str
+        :param _Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._AuthCode = None
+        self._Operator = None
+        self._Agent = None
 
     @property
     def AuthCode(self):
         return self._AuthCode
 
     @AuthCode.setter
     def AuthCode(self, AuthCode):
         self._AuthCode = AuthCode
 
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         self._AuthCode = params.get("AuthCode")
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8288,18 +8360,21 @@
         :param _Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param _UserInfo: 查询开启状态的用户信息
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._SceneKey = None
         self._UserInfo = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -8317,23 +8392,34 @@
     def UserInfo(self):
         return self._UserInfo
 
     @UserInfo.setter
     def UserInfo(self, UserInfo):
         self._UserInfo = UserInfo
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._SceneKey = params.get("SceneKey")
         if params.get("UserInfo") is not None:
             self._UserInfo = UserThreeFactor()
             self._UserInfo._deserialize(params.get("UserInfo"))
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8411,18 +8497,21 @@
         :param _Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param _UserInfo: 关闭自动签的个人的三要素
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._SceneKey = None
         self._UserInfo = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -8440,23 +8529,34 @@
     def UserInfo(self):
         return self._UserInfo
 
     @UserInfo.setter
     def UserInfo(self, UserInfo):
         self._UserInfo = UserInfo
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._SceneKey = params.get("SceneKey")
         if params.get("UserInfo") is not None:
             self._UserInfo = UserThreeFactor()
             self._UserInfo._deserialize(params.get("UserInfo"))
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8964,31 +9064,40 @@
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FillApproverInfo(AbstractModel):
     """补充签署人信息
+    - RecipientId 必须指定
+    -  通过企业自定义账号ID补充签署人时，ApproverSource 和 CustomUserId 必填
+    - 通过二要素（姓名/手机号）补充签署人时，ApproverName 和 ApproverMobile 必填
 
     """
 
     def __init__(self):
         r"""
         :param _RecipientId: 对应模板中的参与方ID
         :type RecipientId: str
         :param _ApproverSource: 签署人来源
 WEWORKAPP: 企业微信
         :type ApproverSource: str
         :param _CustomUserId: 企业自定义账号ID
 WEWORKAPP场景下指企业自有应用获取企微明文的userid
         :type CustomUserId: str
+        :param _ApproverName: 补充签署人姓名
+        :type ApproverName: str
+        :param _ApproverMobile: 补充签署人手机号
+        :type ApproverMobile: str
         """
         self._RecipientId = None
         self._ApproverSource = None
         self._CustomUserId = None
+        self._ApproverName = None
+        self._ApproverMobile = None
 
     @property
     def RecipientId(self):
         return self._RecipientId
 
     @RecipientId.setter
     def RecipientId(self, RecipientId):
@@ -9006,19 +9115,37 @@
     def CustomUserId(self):
         return self._CustomUserId
 
     @CustomUserId.setter
     def CustomUserId(self, CustomUserId):
         self._CustomUserId = CustomUserId
 
+    @property
+    def ApproverName(self):
+        return self._ApproverName
+
+    @ApproverName.setter
+    def ApproverName(self, ApproverName):
+        self._ApproverName = ApproverName
+
+    @property
+    def ApproverMobile(self):
+        return self._ApproverMobile
+
+    @ApproverMobile.setter
+    def ApproverMobile(self, ApproverMobile):
+        self._ApproverMobile = ApproverMobile
+
 
     def _deserialize(self, params):
         self._RecipientId = params.get("RecipientId")
         self._ApproverSource = params.get("ApproverSource")
         self._CustomUserId = params.get("CustomUserId")
+        self._ApproverName = params.get("ApproverName")
+        self._ApproverMobile = params.get("ApproverMobile")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -13381,18 +13508,21 @@
         r"""
         :param _Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定(参数用法参考示例)
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _UserId: 电子签系统员工UserId
         :type UserId: str
         :param _OpenId: 客户系统OpenId
         :type OpenId: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._UserId = None
         self._OpenId = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -13410,21 +13540,32 @@
     def OpenId(self):
         return self._OpenId
 
     @OpenId.setter
     def OpenId(self, OpenId):
         self._OpenId = OpenId
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._UserId = params.get("UserId")
         self._OpenId = params.get("OpenId")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.941/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.940/README.rst` & `tencentcloud-sdk-python-ess-3.0.941/README.rst`

 * *Files identical despite different names*

