# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.0.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.682235 mypy-boto3-chime-sdk-media-pipelines-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-06 20:59:05.674235 mypy-boto3-chime-sdk-media-pipelines-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.662235 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-06 20:34:42.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-06 20:34:42.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38639 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38594 2023-07-06 20:34:42.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.674235 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.682235 mypy-boto3-chime-sdk-media-pipelines-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-06 20:34:40.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57824 2023-07-24 19:47:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57781 2023-07-24 19:46:59.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.10
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,27 +277,32 @@
 ### Literals
 
 `mypy_boto3_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioArtifactsConcatenationStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ConcatenationSinkTypeType,
     ConcatenationSourceTypeType,
     ContentMuxTypeType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     ContentTypeType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LayoutOptionType,
     LiveConnectorMuxTypeType,
     LiveConnectorSinkTypeType,
     LiveConnectorSourceTypeType,
     MediaEncodingType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineSinkTypeType,
@@ -307,136 +312,198 @@
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
     SentimentTypeType,
+    TileOrderType,
+    VerticalTilePositionType,
     VideoMuxTypeType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
     ChimeSDKMediaPipelinesServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationOutputTypeDef,
+    ActiveSpeakerOnlyConfigurationTypeDef,
+    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
+    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
+    AudioConcatenationConfigurationOutputTypeDef,
+    CompositedVideoConcatenationConfigurationOutputTypeDef,
+    ContentConcatenationConfigurationOutputTypeDef,
+    DataChannelConcatenationConfigurationOutputTypeDef,
+    MeetingEventsConcatenationConfigurationOutputTypeDef,
+    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
+    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
+    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
+    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
+    HorizontalLayoutConfigurationOutputTypeDef,
+    PresenterOnlyConfigurationOutputTypeDef,
+    VerticalLayoutConfigurationOutputTypeDef,
+    VideoAttributeOutputTypeDef,
+    HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
+    VerticalLayoutConfigurationTypeDef,
+    VideoAttributeTypeDef,
+    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
+    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
+    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
+    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
+    S3RecordingSinkConfigurationOutputTypeDef,
+    SnsTopicSinkConfigurationOutputTypeDef,
+    SqsQueueSinkConfigurationOutputTypeDef,
+    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
+    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
+    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
+    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
+    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
+    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
+    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
+    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-chime-sdk-media-pipelines
+Version: 1.28.10
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -245,27 +277,32 @@
 ### Literals
 
 `mypy_boto3_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioArtifactsConcatenationStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ConcatenationSinkTypeType,
     ConcatenationSourceTypeType,
     ContentMuxTypeType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     ContentTypeType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LayoutOptionType,
     LiveConnectorMuxTypeType,
     LiveConnectorSinkTypeType,
     LiveConnectorSourceTypeType,
     MediaEncodingType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineSinkTypeType,
@@ -275,136 +312,198 @@
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
     SentimentTypeType,
+    TileOrderType,
+    VerticalTilePositionType,
     VideoMuxTypeType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
     ChimeSDKMediaPipelinesServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationOutputTypeDef,
+    ActiveSpeakerOnlyConfigurationTypeDef,
+    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
+    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
+    AudioConcatenationConfigurationOutputTypeDef,
+    CompositedVideoConcatenationConfigurationOutputTypeDef,
+    ContentConcatenationConfigurationOutputTypeDef,
+    DataChannelConcatenationConfigurationOutputTypeDef,
+    MeetingEventsConcatenationConfigurationOutputTypeDef,
+    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
+    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
+    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
+    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
+    HorizontalLayoutConfigurationOutputTypeDef,
+    PresenterOnlyConfigurationOutputTypeDef,
+    VerticalLayoutConfigurationOutputTypeDef,
+    VideoAttributeOutputTypeDef,
+    HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
+    VerticalLayoutConfigurationTypeDef,
+    VideoAttributeTypeDef,
+    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
+    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
+    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
+    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
+    S3RecordingSinkConfigurationOutputTypeDef,
+    SnsTopicSinkConfigurationOutputTypeDef,
+    SqsQueueSinkConfigurationOutputTypeDef,
+    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
+    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
+    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
+    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
+    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
+    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
+    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
+    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10\nVersion:        "
+        " 1.28.10\nBuilder version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.10")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,46 @@
 Type annotations for chime-sdk-media-pipelines service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+    from mypy_boto3_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
-    data: ArtifactsConcatenationStateType = "Disabled"
+    data: ActiveSpeakerPositionType = "BottomLeft"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ActiveSpeakerPositionType",
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
+    "BorderColorType",
     "CallAnalyticsLanguageCodeType",
+    "CanvasOrientationType",
     "ConcatenationSinkTypeType",
     "ConcatenationSourceTypeType",
     "ContentMuxTypeType",
     "ContentRedactionOutputType",
     "ContentShareLayoutOptionType",
     "ContentTypeType",
     "FragmentSelectorTypeType",
+    "HighlightColorType",
+    "HorizontalTilePositionType",
     "LayoutOptionType",
     "LiveConnectorMuxTypeType",
     "LiveConnectorSinkTypeType",
     "LiveConnectorSourceTypeType",
     "MediaEncodingType",
     "MediaInsightsPipelineConfigurationElementTypeType",
     "MediaPipelineSinkTypeType",
@@ -46,39 +51,48 @@
     "PartialResultsStabilityType",
     "ParticipantRoleType",
     "PresenterPositionType",
     "RealTimeAlertRuleTypeType",
     "RecordingFileFormatType",
     "ResolutionOptionType",
     "SentimentTypeType",
+    "TileOrderType",
+    "VerticalTilePositionType",
     "VideoMuxTypeType",
     "VocabularyFilterMethodType",
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
+ActiveSpeakerPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
+BorderColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
 ]
+CanvasOrientationType = Literal["Landscape", "Portrait"]
 ConcatenationSinkTypeType = Literal["S3Bucket"]
 ConcatenationSourceTypeType = Literal["MediaCapturePipeline"]
 ContentMuxTypeType = Literal["ContentOnly"]
 ContentRedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
-ContentShareLayoutOptionType = Literal["Horizontal", "PresenterOnly", "Vertical"]
+ContentShareLayoutOptionType = Literal[
+    "ActiveSpeakerOnly", "Horizontal", "PresenterOnly", "Vertical"
+]
 ContentTypeType = Literal["PII"]
 FragmentSelectorTypeType = Literal["ProducerTimestamp", "ServerTimestamp"]
+HighlightColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
+HorizontalTilePositionType = Literal["Bottom", "Top"]
 LayoutOptionType = Literal["GridView"]
 LiveConnectorMuxTypeType = Literal["AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 LiveConnectorSinkTypeType = Literal["RTMP"]
 LiveConnectorSourceTypeType = Literal["ChimeSdkMeeting"]
 MediaEncodingType = Literal["pcm"]
 MediaInsightsPipelineConfigurationElementTypeType = Literal[
     "AmazonTranscribeCallAnalyticsProcessor",
@@ -99,14 +113,16 @@
 PartialResultsStabilityType = Literal["high", "low", "medium"]
 ParticipantRoleType = Literal["AGENT", "CUSTOMER"]
 PresenterPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 RealTimeAlertRuleTypeType = Literal["IssueDetection", "KeywordMatch", "Sentiment"]
 RecordingFileFormatType = Literal["Opus", "Wav"]
 ResolutionOptionType = Literal["FHD", "HD"]
 SentimentTypeType = Literal["NEGATIVE"]
+TileOrderType = Literal["JoinSequence", "SpeakerSequence"]
+VerticalTilePositionType = Literal["Left", "Right"]
 VideoMuxTypeType = Literal["VideoOnly"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VoiceAnalyticsConfigurationStatusType = Literal["Disabled", "Enabled"]
 ChimeSDKMediaPipelinesServiceName = Literal["chime-sdk-media-pipelines"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -320,14 +336,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 Type annotations for chime-sdk-media-pipelines service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+    from mypy_boto3_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
-    data: ArtifactsConcatenationStateType = "Disabled"
+    data: ActiveSpeakerPositionType = "BottomLeft"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ActiveSpeakerPositionType",
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
+    "BorderColorType",
     "CallAnalyticsLanguageCodeType",
+    "CanvasOrientationType",
     "ConcatenationSinkTypeType",
     "ConcatenationSourceTypeType",
     "ContentMuxTypeType",
     "ContentRedactionOutputType",
     "ContentShareLayoutOptionType",
     "ContentTypeType",
     "FragmentSelectorTypeType",
+    "HighlightColorType",
+    "HorizontalTilePositionType",
     "LayoutOptionType",
     "LiveConnectorMuxTypeType",
     "LiveConnectorSinkTypeType",
     "LiveConnectorSourceTypeType",
     "MediaEncodingType",
     "MediaInsightsPipelineConfigurationElementTypeType",
     "MediaPipelineSinkTypeType",
@@ -45,38 +50,47 @@
     "PartialResultsStabilityType",
     "ParticipantRoleType",
     "PresenterPositionType",
     "RealTimeAlertRuleTypeType",
     "RecordingFileFormatType",
     "ResolutionOptionType",
     "SentimentTypeType",
+    "TileOrderType",
+    "VerticalTilePositionType",
     "VideoMuxTypeType",
     "VocabularyFilterMethodType",
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+ActiveSpeakerPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
+BorderColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
 ]
+CanvasOrientationType = Literal["Landscape", "Portrait"]
 ConcatenationSinkTypeType = Literal["S3Bucket"]
 ConcatenationSourceTypeType = Literal["MediaCapturePipeline"]
 ContentMuxTypeType = Literal["ContentOnly"]
 ContentRedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
-ContentShareLayoutOptionType = Literal["Horizontal", "PresenterOnly", "Vertical"]
+ContentShareLayoutOptionType = Literal[
+    "ActiveSpeakerOnly", "Horizontal", "PresenterOnly", "Vertical"
+]
 ContentTypeType = Literal["PII"]
 FragmentSelectorTypeType = Literal["ProducerTimestamp", "ServerTimestamp"]
+HighlightColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
+HorizontalTilePositionType = Literal["Bottom", "Top"]
 LayoutOptionType = Literal["GridView"]
 LiveConnectorMuxTypeType = Literal["AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 LiveConnectorSinkTypeType = Literal["RTMP"]
 LiveConnectorSourceTypeType = Literal["ChimeSdkMeeting"]
 MediaEncodingType = Literal["pcm"]
 MediaInsightsPipelineConfigurationElementTypeType = Literal[
     "AmazonTranscribeCallAnalyticsProcessor",
@@ -97,14 +111,16 @@
 PartialResultsStabilityType = Literal["high", "low", "medium"]
 ParticipantRoleType = Literal["AGENT", "CUSTOMER"]
 PresenterPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 RealTimeAlertRuleTypeType = Literal["IssueDetection", "KeywordMatch", "Sentiment"]
 RecordingFileFormatType = Literal["Opus", "Wav"]
 ResolutionOptionType = Literal["FHD", "HD"]
 SentimentTypeType = Literal["NEGATIVE"]
+TileOrderType = Literal["JoinSequence", "SpeakerSequence"]
+VerticalTilePositionType = Literal["Left", "Right"]
 VideoMuxTypeType = Literal["VideoOnly"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VoiceAnalyticsConfigurationStatusType = Literal["Disabled", "Enabled"]
 ChimeSDKMediaPipelinesServiceName = Literal["chime-sdk-media-pipelines"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -318,14 +334,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -2,154 +2,245 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationOutputTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LiveConnectorMuxTypeType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineStatusType,
     MediaPipelineStatusUpdateType,
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
+    TileOrderType,
+    VerticalTilePositionType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    "PostCallAnalyticsSettingsOutputTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
+    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
+    "AudioConcatenationConfigurationOutputTypeDef",
+    "CompositedVideoConcatenationConfigurationOutputTypeDef",
+    "ContentConcatenationConfigurationOutputTypeDef",
+    "DataChannelConcatenationConfigurationOutputTypeDef",
+    "MeetingEventsConcatenationConfigurationOutputTypeDef",
+    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
+    "VideoConcatenationConfigurationOutputTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
     "TranscriptionMessagesConcatenationConfigurationTypeDef",
     "VideoConcatenationConfigurationTypeDef",
+    "AudioArtifactsConfigurationOutputTypeDef",
+    "ContentArtifactsConfigurationOutputTypeDef",
+    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
+    "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
+    "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
+    "HorizontalLayoutConfigurationOutputTypeDef",
+    "PresenterOnlyConfigurationOutputTypeDef",
+    "VerticalLayoutConfigurationOutputTypeDef",
+    "VideoAttributeOutputTypeDef",
+    "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
+    "VerticalLayoutConfigurationTypeDef",
+    "VideoAttributeTypeDef",
+    "IssueDetectionConfigurationOutputTypeDef",
     "IssueDetectionConfigurationTypeDef",
+    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
+    "KinesisDataStreamSinkConfigurationOutputTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
+    "RecordingStreamConfigurationOutputTypeDef",
     "RecordingStreamConfigurationTypeDef",
+    "LambdaFunctionSinkConfigurationOutputTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     "ListMediaPipelinesRequestRequestTypeDef",
     "MediaPipelineSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "LiveConnectorRTMPConfigurationOutputTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
+    "S3RecordingSinkConfigurationOutputTypeDef",
+    "SnsTopicSinkConfigurationOutputTypeDef",
+    "SqsQueueSinkConfigurationOutputTypeDef",
+    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
+    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
+    "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
+    "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
+    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
+    "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
+    "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LiveConnectorSinkConfigurationOutputTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
+    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
+    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
+    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "CompositedVideoArtifactsConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
+    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
+    "ArtifactsConfigurationOutputTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "ConcatenationSourceOutputTypeDef",
     "ConcatenationSourceTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "MediaInsightsPipelineTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
-    "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
+    "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
+ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+)
+
+ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+    total=False,
+)
+
+PostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "PostCallAnalyticsSettingsOutputTypeDef",
+    {
+        "OutputLocation": str,
+        "DataAccessRoleArn": str,
+        "ContentRedactionOutput": ContentRedactionOutputType,
+        "OutputEncryptionKMSKeyId": str,
+    },
+)
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -158,52 +249,114 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
-
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-
-_RequiredAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeProcessorConfigurationTypeDef",
+AmazonTranscribeProcessorConfigurationOutputTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "ShowSpeakerLabel": bool,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "LanguageModelName": str,
+        "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
 )
-_OptionalAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeProcessorConfigurationTypeDef",
+
+AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationTypeDef",
     {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "ShowSpeakerLabel": bool,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
+AudioConcatenationConfigurationOutputTypeDef = TypedDict(
+    "AudioConcatenationConfigurationOutputTypeDef",
+    {
+        "State": Literal["Enabled"],
+    },
+)
 
-class AmazonTranscribeProcessorConfigurationTypeDef(
-    _RequiredAmazonTranscribeProcessorConfigurationTypeDef,
-    _OptionalAmazonTranscribeProcessorConfigurationTypeDef,
-):
-    pass
+CompositedVideoConcatenationConfigurationOutputTypeDef = TypedDict(
+    "CompositedVideoConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
 
+ContentConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ContentConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+DataChannelConcatenationConfigurationOutputTypeDef = TypedDict(
+    "DataChannelConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+MeetingEventsConcatenationConfigurationOutputTypeDef = TypedDict(
+    "MeetingEventsConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+TranscriptionMessagesConcatenationConfigurationOutputTypeDef = TypedDict(
+    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+VideoConcatenationConfigurationOutputTypeDef = TypedDict(
+    "VideoConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
 
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
@@ -246,14 +399,37 @@
 VideoConcatenationConfigurationTypeDef = TypedDict(
     "VideoConcatenationConfigurationTypeDef",
     {
         "State": ArtifactsConcatenationStateType,
     },
 )
 
+AudioArtifactsConfigurationOutputTypeDef = TypedDict(
+    "AudioArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": AudioMuxTypeType,
+    },
+)
+
+ContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ContentArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+        "MuxType": Literal["ContentOnly"],
+    },
+)
+
+VideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "VideoArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+        "MuxType": Literal["VideoOnly"],
+    },
+)
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -267,41 +443,45 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
-
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
-
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
+)
 
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
@@ -309,20 +489,25 @@
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
-
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
+S3BucketSinkConfigurationOutputTypeDef = TypedDict(
+    "S3BucketSinkConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+    },
+)
 
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
@@ -331,14 +516,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -360,18 +556,19 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TimestampRangeOutputTypeDef = TypedDict(
+    "TimestampRangeOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTimestamp": datetime,
+        "EndTimestamp": datetime,
     },
 )
 
 TimestampRangeTypeDef = TypedDict(
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
@@ -396,29 +593,115 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+HorizontalLayoutConfigurationOutputTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationOutputTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+)
+
+PresenterOnlyConfigurationOutputTypeDef = TypedDict(
+    "PresenterOnlyConfigurationOutputTypeDef",
+    {
+        "PresenterPosition": PresenterPositionType,
+    },
+)
+
+VerticalLayoutConfigurationOutputTypeDef = TypedDict(
+    "VerticalLayoutConfigurationOutputTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+)
+
+VideoAttributeOutputTypeDef = TypedDict(
+    "VideoAttributeOutputTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+)
+
+HorizontalLayoutConfigurationTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
 PresenterOnlyConfigurationTypeDef = TypedDict(
     "PresenterOnlyConfigurationTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
     total=False,
 )
 
+VerticalLayoutConfigurationTypeDef = TypedDict(
+    "VerticalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
+VideoAttributeTypeDef = TypedDict(
+    "VideoAttributeTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+    total=False,
+)
+
+IssueDetectionConfigurationOutputTypeDef = TypedDict(
+    "IssueDetectionConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+    },
+)
+
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
+KeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "KeywordMatchConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "Keywords": List[str],
+        "Negate": bool,
+    },
+)
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -426,37 +709,56 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
+KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
+    "KinesisDataStreamSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
 
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
 
+RecordingStreamConfigurationOutputTypeDef = TypedDict(
+    "RecordingStreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
     total=False,
 )
 
+LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -472,15 +774,14 @@
 
 MediaCapturePipelineSummaryTypeDef = TypedDict(
     "MediaCapturePipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
-    total=False,
 )
 
 ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -491,15 +792,14 @@
 MediaInsightsPipelineConfigurationSummaryTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationId": str,
         "MediaInsightsPipelineConfigurationArn": str,
     },
-    total=False,
 )
 
 ListMediaPipelinesRequestRequestTypeDef = TypedDict(
     "ListMediaPipelinesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -509,24 +809,40 @@
 
 MediaPipelineSummaryTypeDef = TypedDict(
     "MediaPipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+LiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorRTMPConfigurationOutputTypeDef",
+    {
+        "Url": str,
+        "AudioChannels": AudioChannelsOptionType,
+        "AudioSampleRate": str,
+    },
+)
+
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -534,20 +850,48 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
-
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
+S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
+    "S3RecordingSinkConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
+    },
+)
+
+SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
+    "SnsTopicSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
+SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
+    "SqsQueueSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
+VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
+        "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
+    },
+)
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
@@ -575,31 +919,45 @@
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
     total=False,
 )
 
+S3RecordingSinkRuntimeConfigurationOutputTypeDef = TypedDict(
+    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
+    },
+)
+
+SentimentConfigurationOutputTypeDef = TypedDict(
+    "SentimentConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "SentimentType": Literal["NEGATIVE"],
+        "TimePeriod": int,
+    },
+)
+
 SentimentConfigurationTypeDef = TypedDict(
     "SentimentConfigurationTypeDef",
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
     },
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
@@ -620,14 +978,33 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
+AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "FilterPartialResults": bool,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
+        "CallAnalyticsStreamCategories": List[str],
+    },
+)
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -645,146 +1022,220 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
+ArtifactsConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConcatenationConfigurationOutputTypeDef",
+    {
+        "Audio": AudioConcatenationConfigurationOutputTypeDef,
+        "Video": VideoConcatenationConfigurationOutputTypeDef,
+        "Content": ContentConcatenationConfigurationOutputTypeDef,
+        "DataChannel": DataChannelConcatenationConfigurationOutputTypeDef,
+        "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
+        "MeetingEvents": MeetingEventsConcatenationConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoConcatenationConfigurationOutputTypeDef,
+    },
+)
 
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
+StreamChannelDefinitionOutputTypeDef = TypedDict(
+    "StreamChannelDefinitionOutputTypeDef",
+    {
+        "NumberOfChannels": int,
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
+    },
+)
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-
-ConcatenationSinkTypeDef = TypedDict(
-    "ConcatenationSinkTypeDef",
+ConcatenationSinkOutputTypeDef = TypedDict(
+    "ConcatenationSinkOutputTypeDef",
     {
         "Type": Literal["S3Bucket"],
-        "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
+        "S3BucketSinkConfiguration": S3BucketSinkConfigurationOutputTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ConcatenationSinkTypeDef = TypedDict(
+    "ConcatenationSinkTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": Literal["S3Bucket"],
+        "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FragmentSelectorOutputTypeDef = TypedDict(
+    "FragmentSelectorOutputTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeOutputTypeDef,
+    },
+)
+
 FragmentSelectorTypeDef = TypedDict(
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
+GridViewConfigurationOutputTypeDef = TypedDict(
+    "GridViewConfigurationOutputTypeDef",
+    {
+        "ContentShareLayout": ContentShareLayoutOptionType,
+        "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
+        "VideoAttribute": VideoAttributeOutputTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
+    },
+)
+
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
     "_OptionalGridViewConfigurationTypeDef",
     {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
+        "VideoAttribute": VideoAttributeTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
-
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
-
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSinkConfigurationOutputTypeDef",
+    {
+        "SinkType": Literal["RTMP"],
+        "RTMPConfiguration": LiveConnectorRTMPConfigurationOutputTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
+RealTimeAlertRuleOutputTypeDef = TypedDict(
+    "RealTimeAlertRuleOutputTypeDef",
+    {
+        "Type": RealTimeAlertRuleTypeType,
+        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -793,29 +1244,53 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+)
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+MediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "Type": MediaInsightsPipelineConfigurationElementTypeType,
+        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
+            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
+        ),
+        "AmazonTranscribeProcessorConfiguration": (
+            AmazonTranscribeProcessorConfigurationOutputTypeDef
+        ),
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -831,29 +1306,43 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
+ChimeSdkMeetingConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
+    {
+        "ArtifactsConfiguration": ArtifactsConcatenationConfigurationOutputTypeDef,
+    },
+)
 
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
+StreamConfigurationOutputTypeDef = TypedDict(
+    "StreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+        "FragmentNumber": str,
+        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
+    },
+)
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -861,29 +1350,44 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[RecordingStreamConfigurationOutputTypeDef],
+        "FragmentSelector": FragmentSelectorOutputTypeDef,
+    },
+)
 
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
+CompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "CompositedVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "Layout": Literal["GridView"],
+        "Resolution": ResolutionOptionType,
+        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -891,48 +1395,91 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
-
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+RealTimeAlertConfigurationOutputTypeDef = TypedDict(
+    "RealTimeAlertConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "Rules": List[RealTimeAlertRuleOutputTypeDef],
+    },
+)
 
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+MediaCapturePipelineSourceConfigurationOutputTypeDef = TypedDict(
+    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
+    {
+        "MediaPipelineArn": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
+    },
+)
+
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[StreamConfigurationOutputTypeDef],
+        "MediaEncoding": Literal["pcm"],
+        "MediaSampleRate": int,
+    },
+)
+
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
+ArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConfigurationOutputTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationOutputTypeDef,
+        "Video": VideoArtifactsConfigurationOutputTypeDef,
+        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+    },
+)
+
+ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "Arn": str,
+        "MuxType": LiveConnectorMuxTypeType,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -941,21 +1488,19 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -964,21 +1509,33 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+)
 
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
@@ -990,37 +1547,20 @@
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
@@ -1029,30 +1569,57 @@
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+ConcatenationSourceOutputTypeDef = TypedDict(
+    "ConcatenationSourceOutputTypeDef",
+    {
+        "Type": Literal["MediaCapturePipeline"],
+        "MediaCapturePipelineSourceConfiguration": (
+            MediaCapturePipelineSourceConfigurationOutputTypeDef
+        ),
+    },
+)
 
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
 
+MediaInsightsPipelineTypeDef = TypedDict(
+    "MediaInsightsPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "Status": MediaPipelineStatusType,
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Dict[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+        "CreatedTimestamp": datetime,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationArn": str,
     },
 )
 _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
@@ -1068,40 +1635,36 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+    },
+)
 
-MediaInsightsPipelineTypeDef = TypedDict(
-    "MediaInsightsPipelineTypeDef",
+LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "Status": MediaPipelineStatusType,
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Dict[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "ChimeSdkMeetingLiveConnectorConfiguration": (
+            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
         ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
     },
-    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
@@ -1119,31 +1682,44 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MediaConcatenationPipelineTypeDef = TypedDict(
+    "MediaConcatenationPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Sources": List[ConcatenationSourceOutputTypeDef],
+        "Sinks": List[ConcatenationSinkOutputTypeDef],
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
@@ -1155,41 +1731,54 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
+CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
+    "CreateMediaInsightsPipelineResponseTypeDef",
+    {
+        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-MediaConcatenationPipelineTypeDef = TypedDict(
-    "MediaConcatenationPipelineTypeDef",
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
-        "Sources": List[ConcatenationSourceTypeDef],
-        "Sinks": List[ConcatenationSinkTypeDef],
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
         "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
-    "CreateMediaInsightsPipelineResponseTypeDef",
+MediaLiveConnectorPipelineTypeDef = TypedDict(
+    "MediaLiveConnectorPipelineTypeDef",
     {
-        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
@@ -1204,39 +1793,20 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
@@ -1245,79 +1815,62 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
-
-MediaLiveConnectorPipelineTypeDef = TypedDict(
-    "MediaLiveConnectorPipelineTypeDef",
-    {
-        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
-        "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
-    total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,153 +2,246 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+    from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationOutputTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LiveConnectorMuxTypeType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineStatusType,
     MediaPipelineStatusUpdateType,
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
+    TileOrderType,
+    VerticalTilePositionType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    "PostCallAnalyticsSettingsOutputTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
+    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
+    "AudioConcatenationConfigurationOutputTypeDef",
+    "CompositedVideoConcatenationConfigurationOutputTypeDef",
+    "ContentConcatenationConfigurationOutputTypeDef",
+    "DataChannelConcatenationConfigurationOutputTypeDef",
+    "MeetingEventsConcatenationConfigurationOutputTypeDef",
+    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
+    "VideoConcatenationConfigurationOutputTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
     "TranscriptionMessagesConcatenationConfigurationTypeDef",
     "VideoConcatenationConfigurationTypeDef",
+    "AudioArtifactsConfigurationOutputTypeDef",
+    "ContentArtifactsConfigurationOutputTypeDef",
+    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
+    "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
+    "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
+    "HorizontalLayoutConfigurationOutputTypeDef",
+    "PresenterOnlyConfigurationOutputTypeDef",
+    "VerticalLayoutConfigurationOutputTypeDef",
+    "VideoAttributeOutputTypeDef",
+    "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
+    "VerticalLayoutConfigurationTypeDef",
+    "VideoAttributeTypeDef",
+    "IssueDetectionConfigurationOutputTypeDef",
     "IssueDetectionConfigurationTypeDef",
+    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
+    "KinesisDataStreamSinkConfigurationOutputTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
+    "RecordingStreamConfigurationOutputTypeDef",
     "RecordingStreamConfigurationTypeDef",
+    "LambdaFunctionSinkConfigurationOutputTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     "ListMediaPipelinesRequestRequestTypeDef",
     "MediaPipelineSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "LiveConnectorRTMPConfigurationOutputTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
+    "S3RecordingSinkConfigurationOutputTypeDef",
+    "SnsTopicSinkConfigurationOutputTypeDef",
+    "SqsQueueSinkConfigurationOutputTypeDef",
+    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
+    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
+    "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
+    "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
+    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
+    "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
+    "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LiveConnectorSinkConfigurationOutputTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
+    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
+    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
+    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    "CompositedVideoArtifactsConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
+    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
+    "ArtifactsConfigurationOutputTypeDef",
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "ConcatenationSourceOutputTypeDef",
     "ConcatenationSourceTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
     "MediaInsightsPipelineTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    "LiveConnectorSourceConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
-    "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
+    "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
+ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationOutputTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+)
+
+ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+    total=False,
+)
+
+PostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "PostCallAnalyticsSettingsOutputTypeDef",
+    {
+        "OutputLocation": str,
+        "DataAccessRoleArn": str,
+        "ContentRedactionOutput": ContentRedactionOutputType,
+        "OutputEncryptionKMSKeyId": str,
+    },
+)
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -157,48 +250,116 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
+
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-_RequiredAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeProcessorConfigurationTypeDef",
+
+AmazonTranscribeProcessorConfigurationOutputTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationOutputTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "ShowSpeakerLabel": bool,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "LanguageModelName": str,
+        "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
 )
-_OptionalAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeProcessorConfigurationTypeDef",
+
+AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationTypeDef",
     {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "ShowSpeakerLabel": bool,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-class AmazonTranscribeProcessorConfigurationTypeDef(
-    _RequiredAmazonTranscribeProcessorConfigurationTypeDef,
-    _OptionalAmazonTranscribeProcessorConfigurationTypeDef,
-):
-    pass
+AudioConcatenationConfigurationOutputTypeDef = TypedDict(
+    "AudioConcatenationConfigurationOutputTypeDef",
+    {
+        "State": Literal["Enabled"],
+    },
+)
+
+CompositedVideoConcatenationConfigurationOutputTypeDef = TypedDict(
+    "CompositedVideoConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+ContentConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ContentConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+DataChannelConcatenationConfigurationOutputTypeDef = TypedDict(
+    "DataChannelConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+MeetingEventsConcatenationConfigurationOutputTypeDef = TypedDict(
+    "MeetingEventsConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+TranscriptionMessagesConcatenationConfigurationOutputTypeDef = TypedDict(
+    "TranscriptionMessagesConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
+
+VideoConcatenationConfigurationOutputTypeDef = TypedDict(
+    "VideoConcatenationConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsConcatenationStateType,
+    },
+)
 
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
@@ -241,14 +402,37 @@
 VideoConcatenationConfigurationTypeDef = TypedDict(
     "VideoConcatenationConfigurationTypeDef",
     {
         "State": ArtifactsConcatenationStateType,
     },
 )
 
+AudioArtifactsConfigurationOutputTypeDef = TypedDict(
+    "AudioArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": AudioMuxTypeType,
+    },
+)
+
+ContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ContentArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+        "MuxType": Literal["ContentOnly"],
+    },
+)
+
+VideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "VideoArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+        "MuxType": Literal["VideoOnly"],
+    },
+)
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -262,57 +446,78 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
+
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
+
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
+
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
+)
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
+
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
+
+S3BucketSinkConfigurationOutputTypeDef = TypedDict(
+    "S3BucketSinkConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+    },
+)
+
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -320,14 +525,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -349,18 +565,19 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TimestampRangeOutputTypeDef = TypedDict(
+    "TimestampRangeOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTimestamp": datetime,
+        "EndTimestamp": datetime,
     },
 )
 
 TimestampRangeTypeDef = TypedDict(
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
@@ -385,29 +602,115 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+HorizontalLayoutConfigurationOutputTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationOutputTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+)
+
+PresenterOnlyConfigurationOutputTypeDef = TypedDict(
+    "PresenterOnlyConfigurationOutputTypeDef",
+    {
+        "PresenterPosition": PresenterPositionType,
+    },
+)
+
+VerticalLayoutConfigurationOutputTypeDef = TypedDict(
+    "VerticalLayoutConfigurationOutputTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+)
+
+VideoAttributeOutputTypeDef = TypedDict(
+    "VideoAttributeOutputTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+)
+
+HorizontalLayoutConfigurationTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
 PresenterOnlyConfigurationTypeDef = TypedDict(
     "PresenterOnlyConfigurationTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
     total=False,
 )
 
+VerticalLayoutConfigurationTypeDef = TypedDict(
+    "VerticalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
+VideoAttributeTypeDef = TypedDict(
+    "VideoAttributeTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+    total=False,
+)
+
+IssueDetectionConfigurationOutputTypeDef = TypedDict(
+    "IssueDetectionConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+    },
+)
+
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
+KeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "KeywordMatchConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "Keywords": List[str],
+        "Negate": bool,
+    },
+)
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -415,35 +718,58 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
+
+KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
+    "KinesisDataStreamSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
 
+RecordingStreamConfigurationOutputTypeDef = TypedDict(
+    "RecordingStreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
     total=False,
 )
 
+LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -459,15 +785,14 @@
 
 MediaCapturePipelineSummaryTypeDef = TypedDict(
     "MediaCapturePipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
-    total=False,
 )
 
 ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -478,15 +803,14 @@
 MediaInsightsPipelineConfigurationSummaryTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationId": str,
         "MediaInsightsPipelineConfigurationArn": str,
     },
-    total=False,
 )
 
 ListMediaPipelinesRequestRequestTypeDef = TypedDict(
     "ListMediaPipelinesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -496,24 +820,40 @@
 
 MediaPipelineSummaryTypeDef = TypedDict(
     "MediaPipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+LiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorRTMPConfigurationOutputTypeDef",
+    {
+        "Url": str,
+        "AudioChannels": AudioChannelsOptionType,
+        "AudioSampleRate": str,
+    },
+)
+
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -521,19 +861,51 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
+
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
+
+S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
+    "S3RecordingSinkConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
+    },
+)
+
+SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
+    "SnsTopicSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
+SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
+    "SqsQueueSinkConfigurationOutputTypeDef",
+    {
+        "InsightsTarget": str,
+    },
+)
+
+VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
+        "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
+    },
+)
+
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -560,31 +932,45 @@
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
     total=False,
 )
 
+S3RecordingSinkRuntimeConfigurationOutputTypeDef = TypedDict(
+    "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
+    {
+        "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
+    },
+)
+
+SentimentConfigurationOutputTypeDef = TypedDict(
+    "SentimentConfigurationOutputTypeDef",
+    {
+        "RuleName": str,
+        "SentimentType": Literal["NEGATIVE"],
+        "TimePeriod": int,
+    },
+)
+
 SentimentConfigurationTypeDef = TypedDict(
     "SentimentConfigurationTypeDef",
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
     },
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
@@ -605,14 +991,33 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
+AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
+        "LanguageCode": CallAnalyticsLanguageCodeType,
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "EnablePartialResultsStabilization": bool,
+        "PartialResultsStability": PartialResultsStabilityType,
+        "ContentIdentificationType": Literal["PII"],
+        "ContentRedactionType": Literal["PII"],
+        "PiiEntityTypes": str,
+        "FilterPartialResults": bool,
+        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
+        "CallAnalyticsStreamCategories": List[str],
+    },
+)
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -630,140 +1035,226 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
+
+ArtifactsConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConcatenationConfigurationOutputTypeDef",
+    {
+        "Audio": AudioConcatenationConfigurationOutputTypeDef,
+        "Video": VideoConcatenationConfigurationOutputTypeDef,
+        "Content": ContentConcatenationConfigurationOutputTypeDef,
+        "DataChannel": DataChannelConcatenationConfigurationOutputTypeDef,
+        "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
+        "MeetingEvents": MeetingEventsConcatenationConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoConcatenationConfigurationOutputTypeDef,
+    },
+)
+
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
+StreamChannelDefinitionOutputTypeDef = TypedDict(
+    "StreamChannelDefinitionOutputTypeDef",
+    {
+        "NumberOfChannels": int,
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
+    },
+)
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-ConcatenationSinkTypeDef = TypedDict(
-    "ConcatenationSinkTypeDef",
+
+ConcatenationSinkOutputTypeDef = TypedDict(
+    "ConcatenationSinkOutputTypeDef",
     {
         "Type": Literal["S3Bucket"],
-        "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
+        "S3BucketSinkConfiguration": S3BucketSinkConfigurationOutputTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ConcatenationSinkTypeDef = TypedDict(
+    "ConcatenationSinkTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": Literal["S3Bucket"],
+        "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FragmentSelectorOutputTypeDef = TypedDict(
+    "FragmentSelectorOutputTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeOutputTypeDef,
+    },
+)
+
 FragmentSelectorTypeDef = TypedDict(
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
+GridViewConfigurationOutputTypeDef = TypedDict(
+    "GridViewConfigurationOutputTypeDef",
+    {
+        "ContentShareLayout": ContentShareLayoutOptionType,
+        "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
+        "VideoAttribute": VideoAttributeOutputTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
+    },
+)
+
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
     "_OptionalGridViewConfigurationTypeDef",
     {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
+        "VideoAttribute": VideoAttributeTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
+
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
+
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSinkConfigurationOutputTypeDef",
+    {
+        "SinkType": Literal["RTMP"],
+        "RTMPConfiguration": LiveConnectorRTMPConfigurationOutputTypeDef,
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
+RealTimeAlertRuleOutputTypeDef = TypedDict(
+    "RealTimeAlertRuleOutputTypeDef",
+    {
+        "Type": RealTimeAlertRuleTypeType,
+        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
+        "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
+        "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -772,27 +1263,55 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
+
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+MediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
+        "Type": MediaInsightsPipelineConfigurationElementTypeType,
+        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
+            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
+        ),
+        "AmazonTranscribeProcessorConfiguration": (
+            AmazonTranscribeProcessorConfigurationOutputTypeDef
+        ),
+        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
+        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
+        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
+        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
+        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
+        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -808,27 +1327,45 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
+
+ChimeSdkMeetingConcatenationConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConcatenationConfigurationOutputTypeDef",
+    {
+        "ArtifactsConfiguration": ArtifactsConcatenationConfigurationOutputTypeDef,
+    },
+)
+
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
+StreamConfigurationOutputTypeDef = TypedDict(
+    "StreamConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+        "FragmentNumber": str,
+        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
+    },
+)
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -836,27 +1373,46 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
+KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[RecordingStreamConfigurationOutputTypeDef],
+        "FragmentSelector": FragmentSelectorOutputTypeDef,
+    },
+)
+
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
+CompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "CompositedVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "Layout": Literal["GridView"],
+        "Resolution": ResolutionOptionType,
+        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -864,46 +1420,93 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
+
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+
+RealTimeAlertConfigurationOutputTypeDef = TypedDict(
+    "RealTimeAlertConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "Rules": List[RealTimeAlertRuleOutputTypeDef],
+    },
+)
+
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+MediaCapturePipelineSourceConfigurationOutputTypeDef = TypedDict(
+    "MediaCapturePipelineSourceConfigurationOutputTypeDef",
+    {
+        "MediaPipelineArn": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
+    },
+)
+
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
+KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
+    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
+    {
+        "Streams": List[StreamConfigurationOutputTypeDef],
+        "MediaEncoding": Literal["pcm"],
+        "MediaSampleRate": int,
+    },
+)
+
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
+ArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConfigurationOutputTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationOutputTypeDef,
+        "Video": VideoArtifactsConfigurationOutputTypeDef,
+        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+    },
+)
+
+ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
+        "Arn": str,
+        "MuxType": LiveConnectorMuxTypeType,
+        "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -912,19 +1515,21 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -933,20 +1538,36 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
@@ -957,34 +1578,21 @@
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
 
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
@@ -994,28 +1602,59 @@
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+ConcatenationSourceOutputTypeDef = TypedDict(
+    "ConcatenationSourceOutputTypeDef",
+    {
+        "Type": Literal["MediaCapturePipeline"],
+        "MediaCapturePipelineSourceConfiguration": (
+            MediaCapturePipelineSourceConfigurationOutputTypeDef
+        ),
+    },
+)
+
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
 
+MediaInsightsPipelineTypeDef = TypedDict(
+    "MediaInsightsPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "Status": MediaPipelineStatusType,
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Dict[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+        "CreatedTimestamp": datetime,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationArn": str,
     },
 )
 _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
@@ -1031,38 +1670,38 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
-MediaInsightsPipelineTypeDef = TypedDict(
-    "MediaInsightsPipelineTypeDef",
+
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "Status": MediaPipelineStatusType,
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Dict[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+    },
+)
+
+LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
+    "LiveConnectorSourceConfigurationOutputTypeDef",
+    {
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "ChimeSdkMeetingLiveConnectorConfiguration": (
+            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
         ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
     },
-    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
@@ -1080,31 +1719,44 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MediaConcatenationPipelineTypeDef = TypedDict(
+    "MediaConcatenationPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Sources": List[ConcatenationSourceOutputTypeDef],
+        "Sinks": List[ConcatenationSinkOutputTypeDef],
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
@@ -1116,39 +1768,56 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
-MediaConcatenationPipelineTypeDef = TypedDict(
-    "MediaConcatenationPipelineTypeDef",
+
+CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
+    "CreateMediaInsightsPipelineResponseTypeDef",
+    {
+        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
-        "Sources": List[ConcatenationSourceTypeDef],
-        "Sinks": List[ConcatenationSinkTypeDef],
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
         "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
-    "CreateMediaInsightsPipelineResponseTypeDef",
+MediaLiveConnectorPipelineTypeDef = TypedDict(
+    "MediaLiveConnectorPipelineTypeDef",
     {
-        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "Status": MediaPipelineStatusType,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
@@ -1163,36 +1832,21 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
@@ -1202,77 +1856,64 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
-MediaLiveConnectorPipelineTypeDef = TypedDict(
-    "MediaLiveConnectorPipelineTypeDef",
-    {
-        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
-        "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "Status": MediaPipelineStatusType,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
-    total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,27 +245,32 @@
 ### Literals
 
 `mypy_boto3_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioArtifactsConcatenationStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ConcatenationSinkTypeType,
     ConcatenationSourceTypeType,
     ContentMuxTypeType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     ContentTypeType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LayoutOptionType,
     LiveConnectorMuxTypeType,
     LiveConnectorSinkTypeType,
     LiveConnectorSourceTypeType,
     MediaEncodingType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineSinkTypeType,
@@ -307,136 +280,198 @@
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
     SentimentTypeType,
+    TileOrderType,
+    VerticalTilePositionType,
     VideoMuxTypeType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
     ChimeSDKMediaPipelinesServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationOutputTypeDef,
+    ActiveSpeakerOnlyConfigurationTypeDef,
+    PostCallAnalyticsSettingsOutputTypeDef,
     PostCallAnalyticsSettingsTypeDef,
+    AmazonTranscribeProcessorConfigurationOutputTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
+    AudioConcatenationConfigurationOutputTypeDef,
+    CompositedVideoConcatenationConfigurationOutputTypeDef,
+    ContentConcatenationConfigurationOutputTypeDef,
+    DataChannelConcatenationConfigurationOutputTypeDef,
+    MeetingEventsConcatenationConfigurationOutputTypeDef,
+    TranscriptionMessagesConcatenationConfigurationOutputTypeDef,
+    VideoConcatenationConfigurationOutputTypeDef,
     AudioConcatenationConfigurationTypeDef,
     CompositedVideoConcatenationConfigurationTypeDef,
     ContentConcatenationConfigurationTypeDef,
     DataChannelConcatenationConfigurationTypeDef,
     MeetingEventsConcatenationConfigurationTypeDef,
     TranscriptionMessagesConcatenationConfigurationTypeDef,
     VideoConcatenationConfigurationTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
+    ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
+    S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
+    HorizontalLayoutConfigurationOutputTypeDef,
+    PresenterOnlyConfigurationOutputTypeDef,
+    VerticalLayoutConfigurationOutputTypeDef,
+    VideoAttributeOutputTypeDef,
+    HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
+    VerticalLayoutConfigurationTypeDef,
+    VideoAttributeTypeDef,
+    IssueDetectionConfigurationOutputTypeDef,
     IssueDetectionConfigurationTypeDef,
+    KeywordMatchConfigurationOutputTypeDef,
     KeywordMatchConfigurationTypeDef,
+    KinesisDataStreamSinkConfigurationOutputTypeDef,
     KinesisDataStreamSinkConfigurationTypeDef,
+    RecordingStreamConfigurationOutputTypeDef,
     RecordingStreamConfigurationTypeDef,
+    LambdaFunctionSinkConfigurationOutputTypeDef,
     LambdaFunctionSinkConfigurationTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     MediaCapturePipelineSummaryTypeDef,
     ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationSummaryTypeDef,
     ListMediaPipelinesRequestRequestTypeDef,
     MediaPipelineSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LiveConnectorRTMPConfigurationOutputTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
+    S3RecordingSinkConfigurationOutputTypeDef,
+    SnsTopicSinkConfigurationOutputTypeDef,
+    SqsQueueSinkConfigurationOutputTypeDef,
+    VoiceAnalyticsProcessorConfigurationOutputTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
+    S3RecordingSinkRuntimeConfigurationOutputTypeDef,
+    SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
+    AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
+    ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
+    StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
+    ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
+    GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LiveConnectorSinkConfigurationOutputTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
+    ChimeSdkMeetingConcatenationConfigurationOutputTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
+    StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    CompositedVideoArtifactsConfigurationOutputTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    MediaCapturePipelineSourceConfigurationOutputTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
+    ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
-    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
+    ConcatenationSourceOutputTypeDef,
     ConcatenationSourceTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
     MediaInsightsPipelineTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
-    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
+    CreateMediaConcatenationPipelineRequestRequestTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> PostCallAnalyticsSettingsTypeDef:
+def get_structure() -> ActiveSpeakerOnlyConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.0/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.28.0",
+    version="1.28.10",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

