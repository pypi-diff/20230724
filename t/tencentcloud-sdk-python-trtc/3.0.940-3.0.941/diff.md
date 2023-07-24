# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.940.tar", last modified: Fri Jul 21 00:52:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.941.tar", last modified: Mon Jul 24 00:47:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.940.tar` & `tencentcloud-sdk-python-trtc-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65738 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   287958 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65738 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   287958 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:47:07.000000 tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/setup.py` & `tencentcloud-sdk-python-trtc-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,15 +882,15 @@
 
         您可以控制台开通旁路转推回调功能实现转推cdn状态的事件监控，具体说明请参考官网文档：[旁路转推回调说明](https://cloud.tencent.com/document/product/647/88552)
         您使用转推api时根据使用特性可能会产生如下费用：
         MCU混流转码费用请参考文档：[云端混流转码计费说明](https://cloud.tencent.com/document/product/647/49446)
         转推非腾讯云CDN费用请参考文档：[云端转推计费说明](https://cloud.tencent.com/document/product/647/82155)
 
         参数的使用说明：
-        1、AgentParams：每个转推任务会拉起一个机器人用户进入TRTC房间进行拉流，你需要通过AgentParams.UserId参数进行设置，这个机器人id不能和房间中的普通用户id冲突，否则会导致转推任务由于机器人用户被踢出TRTC房间而异常结束，您可以通过增加特殊前缀的方式规避。您可以通过设置AgentParams.MaxIdleTime控制转推任务的自动结束，当设置此参数时，所有参与混流转推的主播持续离开TRTC房间超过MaxIdleTime的时长，自动停止转推任务。注意：参与混流转推的主播仅是停止音视频上行，转推任务不会自动停止。
+        1、AgentParams：每个转推任务会拉起一个机器人用户进入TRTC房间进行拉流，您需要通过AgentParams.UserId参数进行设置，这个机器人id不能和房间中的普通用户id冲突，否则会导致转推任务由于机器人用户被踢出TRTC房间而异常结束，您可以通过增加特殊前缀的方式规避。您可以通过设置AgentParams.MaxIdleTime控制转推任务的自动结束，当设置此参数时，所有参与混流转推的主播持续离开TRTC房间超过MaxIdleTime的时长，自动停止转推任务。注意：参与混流转推的主播仅是停止音视频上行，转推任务不会自动停止。
         2、WithTranscoding：如果需要将多路音视频流混合到一路时，WithTranscoding必须设置为1。
         3、AudioParams：转推任务音频参数和视频参数是分开设置的，若您想要将指定的用户音频进行混音时，需要明确设置AudioParams.SubscribeAudioList。若您不设置AudioParams.SubscribeAudioList，混音引擎会自动将TRTC房间中所有用户的音频混合。若您想要混合TRTC房间除指定用户之外的所有用户的声音，可以通过AudioParams.UnSubscribeAudioList设置音频黑名单列表。
         4、VideoParams：若您想要将用户的视频混合，可以通过VideoParams设置，若只想要混纯音频，则不用设置VideoParams参数。您可以通过VideoParams.LayoutParams.MixLayoutMode设置画面的布局模式，包括：动态布局（1：悬浮布局（默认），2：屏幕分享布局，3：九宫格布局）和自定义布局。动态布局模式由排版引擎按照固定的布局自动混合，不需要设置VideoParams.LayoutParams.MixLayoutList。当使用悬浮布局和屏幕分享布局时，您可以通过设置VideoParams.LayoutParams.MaxVideoUser参数指定大画面用户。自定义布局模式提供给您自主布局画面的能力，可以通过VideoParams.LayoutParams.MixLayoutList参数指定每个用户所在的布局位置。在每个布局参数中，您可以通过用户媒体流参数（UserMediaStream）指定这个布局位置为指定的用户预留，也可以不设置UserMediaStream，由排版引擎按照用户进入TRTC房间的顺序自动填充，另外您也可以设置每个布局位置的渲染方式（RenderMode）和裁剪方式（CustomCrop）。
         5、VideoParams.WaterMarkList：若您想要混流画面中叠加水印，可以通过VideoParams.WaterMarkList参数设置，支持图片水印和文字水印，支持透明通道。
         6、SingleSubscribeParams：若您想要将TRTC房间中的一路单流推到CDN，可以使用SingleSubscribeParams参数设置，此时需要将WithTranscoding参数设置为0。
         7、PublishCdnParams.N：若您想要推流到CDN，可以使用PublishCdnParams.N参数设置，支持最多同时推流到10个CDN地址。若转推地址是腾讯云CDN时，请将IsTencentCdn明确设置为1；若您有转推非腾讯云CDN的需求时，请联系腾讯云技术支持开通，转推非腾讯云会产生转推费用，费用说明请参考官网文档：[云端转推计费说明](https://cloud.tencent.com/document/product/647/82155)。
         8、FeedBackRoomParams.N：若您想要将混合的音视频流回推到TRTC房间，可以使用FeedBackRoomParams.N参数设置，支持最多同时推10路流回TRTC房间。您需要指定回推的TRTC房间号和机器人ID（UserId），机器人ID不能与普通用户ID冲突，否则会导致转推任务由于机器人用户被踢出TRTC房间而异常结束，您可以通过增加特殊前缀的方式规避。
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/README.rst` & `tencentcloud-sdk-python-trtc-3.0.941/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.941/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

