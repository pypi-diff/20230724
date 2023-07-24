# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.940.tar", last modified: Fri Jul 21 00:47:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.941.tar", last modified: Mon Jul 24 00:41:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.940.tar` & `tencentcloud-sdk-python-ocr-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115781 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   817596 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:47:05.000000 tencentcloud-sdk-python-ocr-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115781 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   817590 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:41:16.000000 tencentcloud-sdk-python-ocr-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/setup.py` & `tencentcloud-sdk-python-ocr-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-# 帐号已欠费。
+# 账号已欠费。
 FAILEDOPERATION_ARREARSERROR = 'FailedOperation.ArrearsError'
 
 # 身份证CardSide类型错误
 FAILEDOPERATION_CARDSIDEERROR = 'FailedOperation.CardSideError'
 
 # 今日次数达到限制。
 FAILEDOPERATION_COUNTLIMITERROR = 'FailedOperation.CountLimitError'
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.941/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2153,15 +2153,15 @@
         :param _Name: 识别出的字段名称(关键字)，支持以下字段：
 发票代码、 机打代码、 发票号码、 发动机号码、 合格证号、 机打号码、 价税合计(小写)、 销货单位名称、 身份证号码/组织机构代码、 购买方名称、 销售方纳税人识别号、 购买方纳税人识别号、主管税务机关、 主管税务机关代码、 开票日期、 不含税价(小写)、 吨位、增值税税率或征收率、 车辆识别代号/车架号码、 增值税税额、 厂牌型号、 省、 市、 发票消费类型、 销售方电话、 销售方账号、 产地、 进口证明书号、 车辆类型、 机器编号、备注、开票人、限乘人数、商检单号、销售方地址、销售方开户银行、价税合计、发票类型。
         :type Name: str
         :param _Value: 识别出的字段名称对应的值，也就是字段name对应的字符串结果。
         :type Value: str
         :param _Rect: 字段在旋转纠正之后的图像中的像素坐标。
         :type Rect: :class:`tencentcloud.ocr.v20181119.models.Rect`
-        :param _Polygon: 字段在原图中的中的四点坐标。
+        :param _Polygon: 字段在原图中的四点坐标。
 注意：此字段可能返回 null，表示取不到有效值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Polygon: :class:`tencentcloud.ocr.v20181119.models.Polygon`
         """
         self._Name = None
         self._Value = None
         self._Rect = None
@@ -3643,15 +3643,15 @@
     """企业证照单个字段的内容
 
     """
 
     def __init__(self):
         r"""
         :param _Name: 识别出的字段名称（关键字），不同证件类型可能不同，证件类型包含企业登记证书、许可证书、企业执照、三证合一类证书；
-支持以下字段：统一社会信用代码、法定代表人、公司名称、公司地址、注册资金、企业关型、经营范围、成立日期、有效期、开办资金、经费来源、举办单位等；
+支持以下字段：统一社会信用代码、法定代表人、公司名称、公司地址、注册资金、企业类型、经营范围、成立日期、有效期、开办资金、经费来源、举办单位等；
         :type Name: str
         :param _Value: 识别出的字段名称对应的值，也就是字段Name对应的字符串结果。
         :type Value: str
         """
         self._Name = None
         self._Value = None
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.941/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.940/README.rst` & `tencentcloud-sdk-python-ocr-3.0.941/README.rst`

 * *Files identical despite different names*

