# Comparing `tmp/LWTools-1.0.0.tar.gz` & `tmp/LWTools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LWTools-1.0.0.tar", last modified: Mon Jul 24 09:41:39 2023, max compression
+gzip compressed data, was "LWTools-1.0.2.tar", last modified: Mon Jul 24 12:16:08 2023, max compression
```

## Comparing `LWTools-1.0.0.tar` & `LWTools-1.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:41:39.665295 LWTools-1.0.0/
--rw-rw-rw-   0        0        0    35149 2023-07-20 12:51:38.000000 LWTools-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-24 09:41:39.612825 LWTools-1.0.0/LWT/
--rw-rw-rw-   0        0        0        0 2023-07-20 12:57:55.000000 LWTools-1.0.0/LWT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:41:39.650295 LWTools-1.0.0/LWT/lmtanalysis/
--rw-rw-rw-   0        0        0    57456 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/Animal.py
--rw-rw-rw-   0        0        0     2057 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BehaviouralSequencesUtil.py
--rw-rw-rw-   0        0        0     2137 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildDataBaseIndex.py
--rw-rw-rw-   0        0        0     6007 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventApproachContact.py
--rw-rw-rw-   0        0        0     3450 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventApproachRear.py
--rw-rw-rw-   0        0        0     2809 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py
--rw-rw-rw-   0        0        0     2402 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventDetection.py
--rw-rw-rw-   0        0        0        0 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventDistance.py
--rw-rw-rw-   0        0        0    11283 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py
--rw-rw-rw-   0        0        0     4112 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py
--rw-rw-rw-   0        0        0     2258 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveUndetected.py
--rw-rw-rw-   0        0        0     2046 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventFloorSniffing.py
--rw-rw-rw-   0        0        0     7767 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventFollowZone.py
--rw-rw-rw-   0        0        0     3385 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGetAway.py
--rw-rw-rw-   0        0        0     3188 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup2.py
--rw-rw-rw-   0        0        0     3642 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup3.py
--rw-rw-rw-   0        0        0     3581 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py
--rw-rw-rw-   0        0        0     3492 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup4.py
--rw-rw-rw-   0        0        0     4147 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py
--rw-rw-rw-   0        0        0     2064 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventHuddling.py
--rw-rw-rw-   0        0        0     6403 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventMove.py
--rw-rw-rw-   0        0        0     6030 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventNest3.py
--rw-rw-rw-   0        0        0    10879 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventNest4.py
--rw-rw-rw-   0        0        0     7587 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventNight.py
--rw-rw-rw-   0        0        0     5675 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNor.py
--rw-rw-rw-   0        0        0     7590 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py
--rw-rw-rw-   0        0        0     7681 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py
--rw-rw-rw-   0        0        0     5457 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventOnHouse.py
--rw-rw-rw-   0        0        0     2482 2023-07-20 12:51:36.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralGenitalContact.py
--rw-rw-rw-   0        0        0     3192 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralOralContact.py
--rw-rw-rw-   0        0        0     6012 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralSideSequence.py
--rw-rw-rw-   0        0        0     3534 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventOtherContact.py
--rw-rw-rw-   0        0        0     2319 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py
--rw-rw-rw-   0        0        0     3043 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventRear5.py
--rw-rw-rw-   0        0        0     2935 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py
--rw-rw-rw-   0        0        0     1789 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSAP.py
--rw-rw-rw-   0        0        0     3476 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideBySide.py
--rw-rw-rw-   0        0        0     3761 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideBySideOpposite.py
--rw-rw-rw-   0        0        0     3976 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideWalk.py
--rw-rw-rw-   0        0        0     3146 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSocialApproach.py
--rw-rw-rw-   0        0        0     2997 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventSocialEscape.py
--rw-rw-rw-   0        0        0     6241 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventStop.py
--rw-rw-rw-   0        0        0     2726 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain2.py
--rw-rw-rw-   0        0        0     3876 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain3.py
--rw-rw-rw-   0        0        0     4421 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain4.py
--rw-rw-rw-   0        0        0     6496 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventWallJump.py
--rw-rw-rw-   0        0        0     3373 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/BuildEventWaterPoint.py
--rw-rw-rw-   0        0        0     1141 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/CheckWrongAnimal.py
--rw-rw-rw-   0        0        0      649 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Chronometer.py
--rw-rw-rw-   0        0        0     5038 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/CorrectDetectionIntegrity.py
--rw-rw-rw-   0        0        0     4799 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Detection.py
--rw-rw-rw-   0        0        0    37530 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Event.py
--rw-rw-rw-   0        0        0     1827 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/EventTimeLineCache.py
--rw-rw-rw-   0        0        0     4668 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Features.py
--rw-rw-rw-   0        0        0    10868 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/FileUtil.py
--rw-rw-rw-   0        0        0     4540 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Mask.py
--rw-rw-rw-   0        0        0     2207 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Measure.py
--rw-rw-rw-   0        0        0      314 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Point.py
--rw-rw-rw-   0        0        0      375 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Rectangle.py
--rw-rw-rw-   0        0        0       91 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/Settings.py
--rw-rw-rw-   0        0        0     3129 2023-07-20 12:51:37.000000 LWTools-1.0.0/LWT/lmtanalysis/TaskLogger.py
--rw-rw-rw-   0        0        0     9461 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/lmtanalysis/Util.py
--rw-rw-rw-   0        0        0       49 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/lmtanalysis/__init__.py
--rw-rw-rw-   0        0        0      129 2023-07-24 09:30:13.000000 LWTools-1.0.0/LWT/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 09:41:39.654294 LWTools-1.0.0/LWT/scripts/
--rw-rw-rw-   0        0        0    24190 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/scripts/LWT_Export.py
--rw-rw-rw-   0        0        0    54274 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/scripts/LWT_Fonct.py
--rw-rw-rw-   0        0        0     4356 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/scripts/LWT_Merge_csv.py
--rw-rw-rw-   0        0        0    39016 2023-07-20 12:51:38.000000 LWTools-1.0.0/LWT/scripts/LWT_Rebuild_Plus_Export.py
--rw-rw-rw-   0        0        0        0 2023-07-20 12:51:34.000000 LWTools-1.0.0/LWT/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:41:39.665295 LWTools-1.0.0/LWTools.egg-info/
--rw-rw-rw-   0        0        0     6652 2023-07-24 09:41:39.000000 LWTools-1.0.0/LWTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2845 2023-07-24 09:41:39.000000 LWTools-1.0.0/LWTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:41:39.000000 LWTools-1.0.0/LWTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-07-24 09:41:39.000000 LWTools-1.0.0/LWTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-24 09:41:39.000000 LWTools-1.0.0/LWTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6652 2023-07-24 09:41:39.666312 LWTools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5923 2023-07-20 12:51:36.000000 LWTools-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-24 09:41:39.667294 LWTools-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2285 2023-07-24 09:38:59.000000 LWTools-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:16:08.872787 LWTools-1.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-07-20 12:51:38.000000 LWTools-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-24 12:16:08.812641 LWTools-1.0.2/LWT/
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:57:55.000000 LWTools-1.0.2/LWT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:16:08.853587 LWTools-1.0.2/LWT/lmtanalysis/
+-rw-rw-rw-   0        0        0    57456 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/Animal.py
+-rw-rw-rw-   0        0        0     2057 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BehaviouralSequencesUtil.py
+-rw-rw-rw-   0        0        0     2137 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildDataBaseIndex.py
+-rw-rw-rw-   0        0        0     6007 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventApproachContact.py
+-rw-rw-rw-   0        0        0     3450 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventApproachRear.py
+-rw-rw-rw-   0        0        0     2809 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py
+-rw-rw-rw-   0        0        0     2402 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventDetection.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventDistance.py
+-rw-rw-rw-   0        0        0    11283 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py
+-rw-rw-rw-   0        0        0     4112 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py
+-rw-rw-rw-   0        0        0     2258 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveUndetected.py
+-rw-rw-rw-   0        0        0     2046 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventFloorSniffing.py
+-rw-rw-rw-   0        0        0     7767 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventFollowZone.py
+-rw-rw-rw-   0        0        0     3385 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGetAway.py
+-rw-rw-rw-   0        0        0     3188 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup2.py
+-rw-rw-rw-   0        0        0     3642 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup3.py
+-rw-rw-rw-   0        0        0     3581 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py
+-rw-rw-rw-   0        0        0     3492 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup4.py
+-rw-rw-rw-   0        0        0     4147 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py
+-rw-rw-rw-   0        0        0     2064 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventHuddling.py
+-rw-rw-rw-   0        0        0     6403 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventMove.py
+-rw-rw-rw-   0        0        0     6030 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventNest3.py
+-rw-rw-rw-   0        0        0    10879 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventNest4.py
+-rw-rw-rw-   0        0        0     7587 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventNight.py
+-rw-rw-rw-   0        0        0     5675 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNor.py
+-rw-rw-rw-   0        0        0     7590 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py
+-rw-rw-rw-   0        0        0     7681 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py
+-rw-rw-rw-   0        0        0     5457 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventOnHouse.py
+-rw-rw-rw-   0        0        0     2482 2023-07-20 12:51:36.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralGenitalContact.py
+-rw-rw-rw-   0        0        0     3192 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralOralContact.py
+-rw-rw-rw-   0        0        0     6012 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralSideSequence.py
+-rw-rw-rw-   0        0        0     3534 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventOtherContact.py
+-rw-rw-rw-   0        0        0     2319 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py
+-rw-rw-rw-   0        0        0     3043 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventRear5.py
+-rw-rw-rw-   0        0        0     2935 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py
+-rw-rw-rw-   0        0        0     1789 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSAP.py
+-rw-rw-rw-   0        0        0     3476 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideBySide.py
+-rw-rw-rw-   0        0        0     3761 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideBySideOpposite.py
+-rw-rw-rw-   0        0        0     3976 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideWalk.py
+-rw-rw-rw-   0        0        0     3146 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSocialApproach.py
+-rw-rw-rw-   0        0        0     2997 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventSocialEscape.py
+-rw-rw-rw-   0        0        0     6241 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventStop.py
+-rw-rw-rw-   0        0        0     2726 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain2.py
+-rw-rw-rw-   0        0        0     3876 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain3.py
+-rw-rw-rw-   0        0        0     4421 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain4.py
+-rw-rw-rw-   0        0        0     6496 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventWallJump.py
+-rw-rw-rw-   0        0        0     3373 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/BuildEventWaterPoint.py
+-rw-rw-rw-   0        0        0     1141 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/CheckWrongAnimal.py
+-rw-rw-rw-   0        0        0      649 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Chronometer.py
+-rw-rw-rw-   0        0        0     5038 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/CorrectDetectionIntegrity.py
+-rw-rw-rw-   0        0        0     4799 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Detection.py
+-rw-rw-rw-   0        0        0    37530 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Event.py
+-rw-rw-rw-   0        0        0     1827 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/EventTimeLineCache.py
+-rw-rw-rw-   0        0        0     4668 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Features.py
+-rw-rw-rw-   0        0        0    10868 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/FileUtil.py
+-rw-rw-rw-   0        0        0     4540 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Mask.py
+-rw-rw-rw-   0        0        0     2207 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Measure.py
+-rw-rw-rw-   0        0        0      314 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Point.py
+-rw-rw-rw-   0        0        0      375 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Rectangle.py
+-rw-rw-rw-   0        0        0       91 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/Settings.py
+-rw-rw-rw-   0        0        0     3129 2023-07-20 12:51:37.000000 LWTools-1.0.2/LWT/lmtanalysis/TaskLogger.py
+-rw-rw-rw-   0        0        0     9461 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/lmtanalysis/Util.py
+-rw-rw-rw-   0        0        0       49 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/lmtanalysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:16:08.856715 LWTools-1.0.2/LWT/scripts/
+-rw-rw-rw-   0        0        0    24190 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/scripts/LWT_Export.py
+-rw-rw-rw-   0        0        0    54274 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/scripts/LWT_Fonct.py
+-rw-rw-rw-   0        0        0     4356 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/scripts/LWT_Merge_csv.py
+-rw-rw-rw-   0        0        0    39016 2023-07-20 12:51:38.000000 LWTools-1.0.2/LWT/scripts/LWT_Rebuild_Plus_Export.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:51:34.000000 LWTools-1.0.2/LWT/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:16:08.872279 LWTools-1.0.2/LWTools.egg-info/
+-rw-rw-rw-   0        0        0     6652 2023-07-24 12:16:08.000000 LWTools-1.0.2/LWTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2836 2023-07-24 12:16:08.000000 LWTools-1.0.2/LWTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:16:08.000000 LWTools-1.0.2/LWTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-07-24 12:16:08.000000 LWTools-1.0.2/LWTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-24 12:16:08.000000 LWTools-1.0.2/LWTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       15 2023-07-24 11:39:39.000000 LWTools-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6652 2023-07-24 12:16:08.872787 LWTools-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5923 2023-07-20 12:51:36.000000 LWTools-1.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-24 12:16:08.876924 LWTools-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2307 2023-07-24 12:15:41.000000 LWTools-1.0.2/setup.py
```

### Comparing `LWTools-1.0.0/LICENSE` & `LWTools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Animal.py` & `LWTools-1.0.2/LWT/lmtanalysis/Animal.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BehaviouralSequencesUtil.py` & `LWTools-1.0.2/LWT/lmtanalysis/BehaviouralSequencesUtil.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildDataBaseIndex.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildDataBaseIndex.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventApproachContact.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventApproachContact.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventApproachRear.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventApproachRear.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventDetection.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventDetection.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventExclusiveUndetected.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventExclusiveUndetected.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventFloorSniffing.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventFloorSniffing.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventFollowZone.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventFollowZone.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGetAway.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGetAway.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup2.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup2.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup3.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup3.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup4.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup4.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventHuddling.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventHuddling.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventMove.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventMove.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventNest3.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventNest3.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventNest4.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventNest4.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventNight.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventNight.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNor.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNor.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventOnHouse.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventOnHouse.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralGenitalContact.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralGenitalContact.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralOralContact.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralOralContact.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventOralSideSequence.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventOralSideSequence.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventOtherContact.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventOtherContact.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventRear5.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventRear5.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSAP.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSAP.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideBySide.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideBySide.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideBySideOpposite.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideBySideOpposite.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSideWalk.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSideWalk.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSocialApproach.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSocialApproach.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventSocialEscape.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventSocialEscape.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventStop.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventStop.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain2.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain2.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain3.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain3.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventTrain4.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventTrain4.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventWallJump.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventWallJump.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/BuildEventWaterPoint.py` & `LWTools-1.0.2/LWT/lmtanalysis/BuildEventWaterPoint.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/CheckWrongAnimal.py` & `LWTools-1.0.2/LWT/lmtanalysis/CheckWrongAnimal.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Chronometer.py` & `LWTools-1.0.2/LWT/lmtanalysis/Chronometer.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/CorrectDetectionIntegrity.py` & `LWTools-1.0.2/LWT/lmtanalysis/CorrectDetectionIntegrity.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Detection.py` & `LWTools-1.0.2/LWT/lmtanalysis/Detection.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Event.py` & `LWTools-1.0.2/LWT/lmtanalysis/Event.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/EventTimeLineCache.py` & `LWTools-1.0.2/LWT/lmtanalysis/EventTimeLineCache.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Features.py` & `LWTools-1.0.2/LWT/lmtanalysis/Features.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/FileUtil.py` & `LWTools-1.0.2/LWT/lmtanalysis/FileUtil.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Mask.py` & `LWTools-1.0.2/LWT/lmtanalysis/Mask.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Measure.py` & `LWTools-1.0.2/LWT/lmtanalysis/Measure.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/TaskLogger.py` & `LWTools-1.0.2/LWT/lmtanalysis/TaskLogger.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/lmtanalysis/Util.py` & `LWTools-1.0.2/LWT/lmtanalysis/Util.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/scripts/LWT_Export.py` & `LWTools-1.0.2/LWT/scripts/LWT_Export.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/scripts/LWT_Fonct.py` & `LWTools-1.0.2/LWT/scripts/LWT_Fonct.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/scripts/LWT_Merge_csv.py` & `LWTools-1.0.2/LWT/scripts/LWT_Merge_csv.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWT/scripts/LWT_Rebuild_Plus_Export.py` & `LWTools-1.0.2/LWT/scripts/LWT_Rebuild_Plus_Export.py`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/LWTools.egg-info/PKG-INFO` & `LWTools-1.0.2/LWTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LWTools
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tool for LMT data analysis
 Home-page: https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT
 Author: Paul Carrascosa, Damien Huzard
 Author-email: paul.carrascosa@igf.cnrs.fr
 License: GNU General Public License v3 (GPLv3)
 Keywords: Live Mouse Tracker,LMT,Tool,Data analysis
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `LWTools-1.0.0/LWTools.egg-info/SOURCES.txt` & `LWTools-1.0.2/LWTools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 LWT/__init__.py
-LWT/requirements.txt
 LWT/lmtanalysis/Animal.py
 LWT/lmtanalysis/BehaviouralSequencesUtil.py
 LWT/lmtanalysis/BuildDataBaseIndex.py
 LWT/lmtanalysis/BuildEventApproachContact.py
 LWT/lmtanalysis/BuildEventApproachRear.py
 LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py
 LWT/lmtanalysis/BuildEventDetection.py
```

### Comparing `LWTools-1.0.0/PKG-INFO` & `LWTools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LWTools
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tool for LMT data analysis
 Home-page: https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT
 Author: Paul Carrascosa, Damien Huzard
 Author-email: paul.carrascosa@igf.cnrs.fr
 License: GNU General Public License v3 (GPLv3)
 Keywords: Live Mouse Tracker,LMT,Tool,Data analysis
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `LWTools-1.0.0/README.md` & `LWTools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `LWTools-1.0.0/setup.py` & `LWTools-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
 
 For license issues, please contact:
 
 Paul Carrascosa
-Institut de Génomique Fonctionnelle
+Institut de Genomique Fonctionnelle
 141 Rue de la Cardonille
 34000, Montpellier
 
 Email: paul.carrascosa@igf.cnrs.fr or damien.huzard@igf.cnrs.fr
 '''
 
 from setuptools import setup, find_packages
@@ -23,23 +23,23 @@
 try:
     with open(os.path.join(path,'README.md'),encoding='utf-8') as readme:
         long_description=readme.read()
 except Exception:
     long_description=''
 
 
-setup(name='LWTools',version='1.0.0',author='Paul Carrascosa, Damien Huzard',
+setup(name='LWTools',version='1.0.2',author='Paul Carrascosa, Damien Huzard',
     author_email='paul.carrascosa@igf.cnrs.fr',
     description='Tool for LMT data analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT',
     packages=find_packages(),
     package_data={
-        '':['*.txt','*.png','*.pb','*.jpg','*.csv','*.index','*.data-00000-of-00001']
+        'LWTools':['*.py''*.ipynb','*.txt','*.png','*.pb','*.jpg','*.csv','*.index','*.data-00000-of-00001']
     },
     license='GNU General Public License v3 (GPLv3)',
     classifiers=[
     'Programming Language :: Python :: 3.10',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Operating System :: OS Independent',
     ],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

