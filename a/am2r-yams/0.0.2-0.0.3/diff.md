# Comparing `tmp/am2r_yams-0.0.2.tar.gz` & `tmp/am2r_yams-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-0.0.2.tar", last modified: Mon Jul 24 16:49:41 2023, max compression
+gzip compressed data, was "am2r_yams-0.0.3.tar", last modified: Mon Jul 24 17:48:53 2023, max compression
```

## Comparing `am2r_yams-0.0.2.tar` & `am2r_yams-0.0.3.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.156072 am2r_yams-0.0.2/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/Patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.156072 am2r_yams-0.0.2/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/__pyinstaller/hook-yams-py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.160072 am2r_yams-0.0.2/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.2/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.2/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.2/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.2/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.2/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.2/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (123)   942080 2023-07-24 16:49:33.000000 am2r_yams-0.0.2/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-24 16:49:31.000000 am2r_yams-0.0.2/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-24 16:49:34.000000 am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (123)   169984 2023-07-24 16:49:34.000000 am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-07-24 16:49:34.000000 am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.152072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.152072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.152072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.160072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.152072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.152072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.164072 am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.156072 am2r_yams-0.0.2/am2r_yams/yams/sprites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.168072 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorArachnus.png
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorBlue.png
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorGenesis.png
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorGuardian.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorLocked.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorQueen.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorScrew.png
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSerris.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSpider.png
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSuper.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTester.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTorizo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.156072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.168072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.168072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.172073 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.172073 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.172073 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.172073 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.176072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.176072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.176072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.176072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.176072 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.180073 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.180073 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.180073 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newA4Doors.png
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newA4Doors2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUIMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUIPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUISMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpHideout.png
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.156072 am2r_yams-0.0.2/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:49:40.000000 am2r_yams-0.0.2/am2r_yams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 16:49:41.000000 am2r_yams-0.0.2/am2r_yams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/am2r_yams_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/am2r_yams_tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 16:49:07.000000 am2r_yams-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:49:41.184073 am2r_yams-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/Patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__pyinstaller/hook-yams-py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.3/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.3/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.3/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.3/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.3/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.3/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   941568 2023-07-24 17:48:43.000000 am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-24 17:48:41.000000 am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (123)   170496 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/sprites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.829160 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorArachnus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBlue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGenesis.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGuardian.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorLocked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorQueen.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorScrew.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSerris.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpider.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSuper.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTester.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTorizo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.829160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.833160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.849160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.849160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUISMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpHideout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams_tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 17:48:53.857160 am2r_yams-0.0.3/setup.cfg
```

### Comparing `am2r_yams-0.0.2/LICENSE` & `am2r_yams-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/PKG-INFO` & `am2r_yams-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 Very WIP
```

### Comparing `am2r_yams-0.0.2/am2r_yams/Patcher.py` & `am2r_yams-0.0.3/am2r_yams/Patcher.py`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-0.0.3/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-0.0.3/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.3/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-0.0.3/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-0.0.3/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-0.0.3/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.dll`

 * *Files 3% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xe758826b
+	             Time stamp: 0xc88c4f81
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2102
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x000e5800
+	              Code Size: 0x000e5600
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000e763e
+	        Entry Point RVA: 0x000e74fe
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00000000
 
 
 NT Header:
 	   Image Base (0x400000): 0x00400000
 	Section Alignment (8192): 0x00002000
@@ -41,109 +41,109 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000e75f0 [0x0000004b]
+	     Import Table: 0x000e74a8 [0x00000053]
 	   Resource Table: 0x000e8000 [0x000003b4]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x000ea000 [0x0000000c]
-	            Debug: 0x000d0ccc [0x00000054]
+	            Debug: 0x000d0b80 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000e5644
+	   Virtual Size: 0x000e5504
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x000e5800
+	  Raw Data Size: 0x000e5600
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x000003b4
 	Virtual Address: 0x000e8000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x000e5a00
+	   Raw Data Ptr: 0x000e5800
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x000ea000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x000e5e00
+	   Raw Data Ptr: 0x000e5c00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0005b604 [0x000756c8]
+	         Metadata: 0x0005b4dc [0x000756a4]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0005b208 [0x00000018]
+	     Resources at: 0x0005b0e0 [0x00000018]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0002a9d0 [174436 == 0x0002a964]
-	    Strings: 0x0002a9d0 - 0x0003af94 [67012 == 0x000105c4]
-	       Blob: 0x0006dda4 - 0x000756c8 [31012 == 0x00007924]
-	User string: 0x0003af94 - 0x0006dd94 [208384 == 0x00032e00]
-	       GUID: 0x0006dd94 - 0x0006dda4 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x0002a9b8 [174412 == 0x0002a94c]
+	    Strings: 0x0002a9b8 - 0x0003af68 [66992 == 0x000105b0]
+	       Blob: 0x0006dd78 - 0x000756a4 [31020 == 0x0000792c]
+	User string: 0x0003af68 - 0x0006dd68 [208384 == 0x00032e00]
+	       GUID: 0x0006dd68 - 0x0006dd78 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 598f8)
-Table TypeRef: 205 records (10 bytes, at 59904)
-Table TypeDef: 434 records (18 bytes, at 5a106)
-Table Field: 2684 records (8 bytes, at 5bf8a)
-Table Method: 3560 records (16 bytes, at 6136a)
-Table Param: 2585 records (8 bytes, at 6f1ea)
-Table InterfaceImpl: 389 records (4 bytes, at 742b2)
-Table MemberRef: 1660 records (8 bytes, at 748c6)
-Table Constant: 1105 records (6 bytes, at 77ca6)
-Table CustomAttribute: 2300 records (8 bytes, at 7968c)
-Table DeclSecurity: 1 records (6 bytes, at 7de6c)
-Table ClassLayout: 14 records (8 bytes, at 7de72)
-Table StandaloneSig: 355 records (2 bytes, at 7dee2)
-Table EventMap: 84 records (4 bytes, at 7e1a8)
-Table Event: 84 records (8 bytes, at 7e2f8)
-Table PropertyMap: 171 records (4 bytes, at 7e598)
-Table Property: 924 records (8 bytes, at 7e844)
-Table MethodSemantics: 1834 records (6 bytes, at 80524)
-Table MethodImpl: 4 records (6 bytes, at 83020)
-Table TypeSpec: 502 records (2 bytes, at 83038)
-Table FieldRVA: 26 records (6 bytes, at 83424)
-Table Assembly: 1 records (26 bytes, at 834c0)
-Table AssemblyRef: 18 records (24 bytes, at 834da)
-Table ManifestResource: 1 records (14 bytes, at 8368a)
-Table NestedClass: 216 records (4 bytes, at 83698)
-Table GenericParam: 33 records (10 bytes, at 839f8)
-Table MethodSpec: 390 records (4 bytes, at 83b42)
-Table GenericParamConstraint: 30 records (4 bytes, at 8415a)
+Table Module: 1 records (12 bytes, at 597d0)
+Table TypeRef: 205 records (10 bytes, at 597dc)
+Table TypeDef: 434 records (18 bytes, at 59fde)
+Table Field: 2684 records (8 bytes, at 5be62)
+Table Method: 3559 records (16 bytes, at 61242)
+Table Param: 2584 records (8 bytes, at 6f0b2)
+Table InterfaceImpl: 389 records (4 bytes, at 74172)
+Table MemberRef: 1660 records (8 bytes, at 74786)
+Table Constant: 1105 records (6 bytes, at 77b66)
+Table CustomAttribute: 2300 records (8 bytes, at 7954c)
+Table DeclSecurity: 1 records (6 bytes, at 7dd2c)
+Table ClassLayout: 14 records (8 bytes, at 7dd32)
+Table StandaloneSig: 355 records (2 bytes, at 7dda2)
+Table EventMap: 84 records (4 bytes, at 7e068)
+Table Event: 84 records (8 bytes, at 7e1b8)
+Table PropertyMap: 171 records (4 bytes, at 7e458)
+Table Property: 924 records (8 bytes, at 7e704)
+Table MethodSemantics: 1834 records (6 bytes, at 803e4)
+Table MethodImpl: 4 records (6 bytes, at 82ee0)
+Table TypeSpec: 502 records (2 bytes, at 82ef8)
+Table FieldRVA: 26 records (6 bytes, at 832e4)
+Table Assembly: 1 records (26 bytes, at 83380)
+Table AssemblyRef: 18 records (24 bytes, at 8339a)
+Table ManifestResource: 1 records (14 bytes, at 8354a)
+Table NestedClass: 216 records (4 bytes, at 83558)
+Table GenericParam: 33 records (10 bytes, at 838b8)
+Table MethodSpec: 390 records (4 bytes, at 83a02)
+Table GenericParamConstraint: 30 records (4 bytes, at 8401a)
```

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/0.0.3': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), delete: ['YAMS-LIB/0.0.2']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'YAMS-LIB/0.0.3': OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Macross.Json.Extensions', '3.0.0'), ('SixLabors.ImageSharp', "*

 * *              "'3.0.1'), ('UndertaleModLib', '1.0.0')])), ('runtime', "*

 * *              "OrderedDict([('YAMS-LIB.dll', OrderedDict())]))]), delete: ['YAMS-LIB/0.0.2' […]*

```diff
@@ -58,15 +58,15 @@
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/0.0.2": {
+        "YAMS-LIB/0.0.3": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         }
     },
     "runtimeTarget": {
         "name": ".NETCoreApp,Version=v6.0",
@@ -159,15 +159,15 @@
                     "SharpZipLib": "1.3.3",
                     "System.Drawing.Common": "5.0.3"
                 },
                 "runtime": {
                     "UndertaleModLib.dll": {}
                 }
             },
-            "YAMS-LIB/0.0.2": {
+            "YAMS-LIB/0.0.3": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
                     "SixLabors.ImageSharp": "3.0.1",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
                     "YAMS-LIB.dll": {}
```

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 6% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xd9eda03d
+	             Time stamp: 0xdc7e48b0
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00029000
+	              Code Size: 0x00029200
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0002af6e
+	        Entry Point RVA: 0x0002b00a
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0002c000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,66 +41,66 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0002af1c [0x0000004f]
+	     Import Table: 0x0002afb8 [0x0000004f]
 	   Resource Table: 0x0002c000 [0x0000031c]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0002e000 [0x0000000c]
-	            Debug: 0x0002ae44 [0x00000054]
+	            Debug: 0x0002aee0 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00028fa0
+	   Virtual Size: 0x00029038
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00029000
+	  Raw Data Size: 0x00029200
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x0000031c
 	Virtual Address: 0x0002c000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00029200
+	   Raw Data Ptr: 0x00029400
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x0002e000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00029600
+	   Raw Data Ptr: 0x00029800
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0000d074 [0x0001ddd0]
+	         Metadata: 0x0000d084 [0x0001de5c]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -109,30 +109,30 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00002040 [8148 == 0x00001fd4]
-	    Strings: 0x00002040 - 0x00003ba4 [7012 == 0x00001b64]
-	       Blob: 0x0001c480 - 0x0001ddd0 [6480 == 0x00001950]
-	User string: 0x00003ba4 - 0x0001c470 [100556 == 0x000188cc]
-	       GUID: 0x0001c470 - 0x0001c480 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x0000207c [8208 == 0x00002010]
+	    Strings: 0x0000207c - 0x00003bf8 [7036 == 0x00001b7c]
+	       Blob: 0x0001c4d4 - 0x0001de5c [6536 == 0x00001988]
+	User string: 0x00003bf8 - 0x0001c4c4 [100556 == 0x000188cc]
+	       GUID: 0x0001c4c4 - 0x0001c4d4 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at b33c)
-Table TypeRef: 107 records (6 bytes, at b346)
-Table TypeDef: 23 records (14 bytes, at b5c8)
-Table Field: 200 records (6 bytes, at b70a)
-Table Method: 70 records (14 bytes, at bbba)
-Table Param: 71 records (6 bytes, at bf8e)
-Table MemberRef: 266 records (6 bytes, at c138)
-Table Constant: 110 records (6 bytes, at c774)
-Table CustomAttribute: 300 records (6 bytes, at ca08)
-Table ClassLayout: 1 records (8 bytes, at d110)
-Table StandaloneSig: 6 records (2 bytes, at d118)
-Table TypeSpec: 43 records (2 bytes, at d124)
-Table FieldRVA: 1 records (6 bytes, at d17a)
-Table Assembly: 1 records (22 bytes, at d180)
-Table AssemblyRef: 9 records (20 bytes, at d196)
-Table NestedClass: 6 records (4 bytes, at d24a)
-Table MethodSpec: 20 records (4 bytes, at d262)
+Table Module: 1 records (10 bytes, at b34c)
+Table TypeRef: 107 records (6 bytes, at b356)
+Table TypeDef: 24 records (14 bytes, at b5d8)
+Table Field: 201 records (6 bytes, at b728)
+Table Method: 71 records (14 bytes, at bbde)
+Table Param: 71 records (6 bytes, at bfc0)
+Table MemberRef: 266 records (6 bytes, at c16a)
+Table Constant: 110 records (6 bytes, at c7a6)
+Table CustomAttribute: 304 records (6 bytes, at ca3a)
+Table ClassLayout: 1 records (8 bytes, at d15a)
+Table StandaloneSig: 6 records (2 bytes, at d162)
+Table TypeSpec: 43 records (2 bytes, at d16e)
+Table FieldRVA: 1 records (6 bytes, at d1c4)
+Table Assembly: 1 records (22 bytes, at d1ca)
+Table AssemblyRef: 9 records (20 bytes, at d1e0)
+Table NestedClass: 6 records (4 bytes, at d294)
+Table MethodSpec: 20 records (4 bytes, at d2ac)
```

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/YAMS-LIB.pdb` & `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.pdb`

 * *Files 7% similar despite different names*

```diff
@@ -1,1352 +1,1353 @@
 00000000: 4253 4a42 0100 0100 0000 0000 0c00 0000  BSJB............
 00000010: 5044 4220 7631 2e30 0000 0000 0000 0600  PDB v1.0........
 00000020: 7c00 0000 6400 0000 2350 6462 0000 0000  |...d...#Pdb....
-00000030: e000 0000 500c 0000 237e 0000 300d 0000  ....P...#~..0...
+00000030: e000 0000 540c 0000 237e 0000 340d 0000  ....T...#~..4...
 00000040: a805 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
-00000050: d812 0000 0400 0000 2355 5300 dc12 0000  ........#US.....
-00000060: 5000 0000 2347 5549 4400 0000 2c13 0000  P...#GUID...,...
-00000070: 5441 0000 2342 6c6f 6200 0000 43f5 8efd  TA..#Blob...C...
-00000080: dc1f 4c4c acab a5d7 0154 7aac c0bc 37f0  ..LL.....Tz...7.
+00000050: dc12 0000 0400 0000 2355 5300 e012 0000  ........#US.....
+00000060: 5000 0000 2347 5549 4400 0000 3013 0000  P...#GUID...0...
+00000070: 5441 0000 2342 6c6f 6200 0000 be86 ceaf  TA..#Blob.......
+00000080: 2db3 ce4f 8309 6100 97cb fad8 e94d 468e  -..O..a......MF.
 00000090: 0000 0000 579d 0228 090a 0000 0100 0000  ....W..(........
-000000a0: 6b00 0000 1700 0000 c800 0000 4600 0000  k...........F...
-000000b0: 4700 0000 0a01 0000 6e00 0000 2c01 0000  G.......n...,...
+000000a0: 6b00 0000 1800 0000 c900 0000 4700 0000  k...........G...
+000000b0: 4700 0000 0a01 0000 6e00 0000 3001 0000  G.......n...0...
 000000c0: 0100 0000 0600 0000 2b00 0000 0100 0000  ........+.......
 000000d0: 0100 0000 0900 0000 0600 0000 1400 0000  ................
 000000e0: 0000 0000 0200 0001 0000 0000 0000 bf00  ................
-000000f0: 0000 0000 0000 8400 0500 0000 4600 0000  ............F...
+000000f0: 0000 0000 0000 8400 0500 0000 4700 0000  ............G...
 00000100: 7300 0000 8e00 0000 0400 0000 0500 0000  s...............
 00000110: 0800 0000 2b00 0100 3500 0200 6400 0100  ....+...5...d...
 00000120: 6e00 0200 bd00 0100 ce00 0200 1e01 0100  n...............
 00000130: 2f01 0200 6901 0100 7a01 0200 0000 0000  /...i...z.......
-00000140: 0000 0000 0000 0000 0000 0000 0100 8127  ...............'
-00000150: 0100 2d29 0000 0000 0100 1d3e 0200 243e  ..-).......>..$>
-00000160: 0000 0000 0000 0000 0200 c73e 0000 0000  ...........>....
-00000170: 0000 0000 0200 d43e 0200 dc3e 0200 e93e  .......>...>...>
-00000180: 0000 0000 0000 0000 0100 f13e 0100 f93e  ...........>...>
-00000190: 0100 013f 0100 093f 0100 113f 0100 193f  ...?...?...?...?
-000001a0: 0100 213f 0100 293f 0100 313f 0100 393f  ..!?..)?..1?..9?
-000001b0: 0100 413f 0100 493f 0100 513f 0100 593f  ..A?..I?..Q?..Y?
-000001c0: 0100 623f 0100 6a3f 0100 733f 0100 7b3f  ..b?..j?..s?..{?
-000001d0: 0100 833f 0100 8b3f 0100 933f 0100 9b3f  ...?...?...?...?
-000001e0: 0100 a33f 0100 ab3f 0100 b33f 0100 bb3f  ...?...?...?...?
-000001f0: 0100 c33f 0100 cb3f 0100 d33f 0100 db3f  ...?...?...?...?
-00000200: 0100 e33f 0100 eb3f 0100 f33f 0000 0000  ...?...?...?....
-00000210: 0100 fb3f 0100 0240 0100 2240 0100 3840  ...?...@.."@..8@
-00000220: 0100 4e40 0100 5a40 0100 6640 0100 7240  ..N@..Z@..f@..r@
-00000230: 0100 1c41 0100 2441 0000 0000 0100 2c41  ...A..$A......,A
-00000240: 0000 0000 0100 3441 0100 3c41 0100 4441  ......4A..<A..DA
-00000250: 0100 4c41 0500 0300 0100 0100 0000 0000  ..LA............
-00000260: 6900 0000 0600 0300 0200 0100 0000 0000  i...............
-00000270: 8ca1 0000 0600 0300 3600 0500 2800 0000  ........6...(...
-00000280: 2b00 0000 0600 0300 3700 0500 fa00 0000  +.......7.......
-00000290: 4400 0000 0600 0300 3800 0500 3e01 0000  D.......8...>...
-000002a0: 0502 0000 0600 0300 3b00 0500 0402 0000  ........;.......
-000002b0: 4000 0000 0600 0300 3c00 0500 0303 0000  @.......<.......
-000002c0: 4000 0000 0600 0300 3d00 0500 a63f 0000  @.......=....?..
-000002d0: 4f00 0000 0600 0300 3e00 0500 3a41 0000  O.......>...:A..
-000002e0: 2500 0000 0600 0300 3f00 0500 c542 0000  %.......?....B..
-000002f0: 2500 0000 0600 0300 4000 0500 3644 0000  %.......@...6D..
-00000300: 2800 0000 0600 0300 4100 0500 8c44 0000  (.......A....D..
-00000310: 4500 0000 0600 0300 4200 0500 6945 0000  E.......B...iE..
-00000320: 4500 0000 0600 0300 4300 0500 8746 0000  E.......C....F..
-00000330: 2b00 0000 0600 0300 4400 0500 fd4b 0000  +.......D....K..
-00000340: c801 0000 0600 0300 4500 0500 094c 0000  ........E....L..
-00000350: aa01 0000 0600 0300 4a00 0500 fb4e 0000  ........J....N..
-00000360: 2b00 0000 0600 0300 4b00 0500 714f 0000  +.......K...qO..
-00000370: 2b00 0000 0600 0300 4c00 0500 0b51 0000  +.......L....Q..
-00000380: d50d 0000 0600 0300 5b00 0500 0167 0000  ........[....g..
-00000390: 2b00 0000 0600 0300 5c00 0500 a567 0000  +.......\....g..
-000003a0: 2100 0000 0600 0300 5d00 0500 7868 0000  !.......]...xh..
-000003b0: 1c00 0000 0600 0300 5e00 0500 6e69 0000  ........^...ni..
-000003c0: 1c00 0000 0600 0300 5f00 0500 0c6a 0000  ........_....j..
-000003d0: 2b00 0000 0600 0300 6000 0500 a36a 0000  +.......`....j..
-000003e0: 1c00 0000 0600 0300 6100 0500 346b 0000  ........a...4k..
-000003f0: 1c00 0000 0600 0300 6200 0500 2b6c 0000  ........b...+l..
-00000400: 2b00 0000 0600 0300 6300 0500 166d 0000  +.......c....m..
-00000410: 2b00 0000 0600 0300 6400 0500 e06d 0000  +.......d....m..
-00000420: 2b00 0000 0600 0300 6500 0500 ec6f 0000  +.......e....o..
-00000430: 1b00 0000 0600 0300 6600 0500 d173 0000  ........f....s..
-00000440: 2b00 0000 0600 0300 6700 0500 ee74 0000  +.......g....t..
-00000450: cc06 0000 0600 0300 6800 0500 3277 0000  ........h...2w..
-00000460: 3800 0000 0600 0300 6900 0500 767e 0000  8.......i...v~..
-00000470: 5304 0000 0600 0300 6b00 0500 927e 0000  S.......k....~..
-00000480: 3704 0000 0600 0300 6c00 0500 ac7e 0000  7.......l....~..
-00000490: c703 0000 0600 0300 6d00 0500 c87e 0000  ........m....~..
-000004a0: 8b03 0000 0600 0300 6e00 0500 d17e 0000  ........n....~..
-000004b0: 8203 0000 0600 0300 6f00 0500 437f 0000  ........o...C...
-000004c0: 8900 0000 0600 0300 7000 0500 f782 0000  ........p.......
-000004d0: 8b03 0000 0600 0300 7200 0500 1383 0000  ........r.......
-000004e0: 6f03 0000 0600 0300 7600 0500 7b85 0000  o.......v...{...
-000004f0: 2c00 0000 0600 0300 7700 0500 a28b 0000  ,.......w.......
-00000500: 1600 0000 0600 0300 7800 0500 1e8c 0000  ........x.......
-00000510: 2100 0000 0600 0300 7900 0500 f98c 0000  !.......y.......
-00000520: 2500 0000 0600 0300 7a00 0500 2c8d 0000  %.......z...,...
-00000530: 6000 0000 0600 0300 7b00 0500 628e 0000  `.......{...b...
-00000540: 4900 0000 0600 0300 7c00 0500 0a8f 0000  I.......|.......
-00000550: 3700 0000 0600 0300 7d00 0500 a08f 0000  7.......}.......
-00000560: 2100 0000 0600 0300 7e00 0500 2090 0000  !.......~... ...
-00000570: 3700 0000 0600 0300 7f00 0500 b690 0000  7...............
-00000580: 4c00 0000 0600 0300 8000 0500 3691 0000  L...........6...
-00000590: 2b00 0000 0600 0300 8100 0500 1592 0000  +...............
-000005a0: 1001 0000 0600 0300 8200 0500 3192 0000  ............1...
-000005b0: da00 0000 0600 0300 8300 0500 7792 0000  ............w...
-000005c0: 8200 0000 0600 0300 8400 0500 a095 0000  ................
-000005d0: 5d00 0000 0600 0300 8500 0500 ba95 0000  ]...............
-000005e0: 4300 0000 0600 0300 8700 0500 48a1 0000  C...........H...
-000005f0: 4300 0000 0800 0300 8800 0500 0000 0000  C...............
-00000600: 0b00 0000 0900 0500 8800 0500 0000 0000  ................
-00000610: 3300 0000 0c00 0500 8800 0500 0000 0000  3...............
-00000620: 1d00 0000 0f00 0500 8800 0500 0000 0000  ................
-00000630: 1200 0000 1000 0500 8800 0500 0000 0000  ................
-00000640: 1d00 0000 1100 0500 8800 0500 0000 0000  ................
-00000650: 1200 0000 1400 0300 8800 0500 0000 0000  ................
-00000660: 0e00 0000 1500 0300 8800 0500 0000 0000  ................
-00000670: 0e00 0000 1600 0300 8800 0500 0000 0000  ................
-00000680: 0e00 0000 1700 0300 8800 0500 0000 0000  ................
-00000690: 0e00 0000 1800 0300 8800 0500 0000 0000  ................
-000006a0: 1d00 0000 1900 0300 8800 0500 0000 0000  ................
-000006b0: 1a00 0000 1a00 0300 8800 0500 0000 0000  ................
-000006c0: 1a00 0000 1b00 0300 8800 0500 0000 0000  ................
-000006d0: 1a00 0000 1c00 0300 8800 0500 0000 0000  ................
-000006e0: 1d00 0000 1d00 0300 8800 0500 0000 0000  ................
-000006f0: 1d00 0000 1e00 0300 8800 0500 0000 0000  ................
-00000700: 1d00 0000 1f00 0300 8800 0500 0000 0000  ................
-00000710: 1d00 0000 2000 0300 8800 0500 0000 0000  .... ...........
-00000720: 4300 0000 2100 0300 8800 0500 0000 0000  C...!...........
-00000730: 5a00 0000 2200 0300 8800 0500 0000 0000  Z..."...........
-00000740: 5a00 0000 2300 0300 8800 0500 0000 0000  Z...#...........
-00000750: 4300 0000 2400 0300 8800 0500 0000 0000  C...$...........
-00000760: 1600 0000 2500 0300 8800 0500 0000 0000  ....%...........
-00000770: 1b00 0000 2600 0300 8800 0500 0000 0000  ....&...........
-00000780: 1100 0000 2700 0300 8800 0500 0000 0000  ....'...........
-00000790: 1100 0000 2800 0300 8800 0500 0000 0000  ....(...........
-000007a0: 1100 0000 2900 0300 8800 0500 0000 0000  ....)...........
-000007b0: 1100 0000 2a00 0300 8800 0500 0000 0000  ....*...........
-000007c0: 1100 0000 2b00 0300 8800 0500 0000 0000  ....+...........
-000007d0: 1100 0000 2c00 0300 8800 0500 0000 0000  ....,...........
-000007e0: 1100 0000 2d00 0300 8800 0500 0000 0000  ....-...........
-000007f0: 1100 0000 2e00 0300 8800 0500 0000 0000  ................
-00000800: 1100 0000 2f00 0300 8800 0500 0000 0000  ..../...........
-00000810: 1600 0000 3000 0300 8800 0500 0000 0000  ....0...........
-00000820: 1b00 0000 3100 0300 8800 0500 0000 0000  ....1...........
-00000830: 1b00 0000 3200 0300 8800 0500 0000 0000  ....2...........
-00000840: 1b00 0000 3300 0300 8800 0500 0000 0000  ....3...........
-00000850: 1b00 0000 3400 0300 8800 0500 0000 0000  ....4...........
-00000860: 1b00 0000 3600 0300 8800 0500 0000 0000  ....6...........
-00000870: 0e00 0000 3700 0300 8800 0500 0000 0000  ....7...........
-00000880: 8700 0000 3800 0300 8900 0500 0000 0000  ....8...........
-00000890: 2900 0000 3900 0300 8a00 0500 0000 0000  )...9...........
-000008a0: 2900 0000 3a00 0300 8b00 0500 0000 0000  )...:...........
-000008b0: 0e00 0000 3b00 0300 8b00 0500 0000 0000  ....;...........
-000008c0: 8500 0000 3c00 0300 8b00 0500 0000 0000  ....<...........
-000008d0: 7700 0000 3d00 0300 8b00 0500 0000 0000  w...=...........
-000008e0: 7f02 0000 3d00 0300 8b00 0500 0b00 0000  ....=...........
-000008f0: 0b00 0000 3d00 0300 8c00 0500 2e00 0000  ....=...........
-00000900: 4302 0000 3d00 0300 8d00 0500 3200 0000  C...=.......2...
-00000910: 3f02 0000 3e00 0300 8f00 0500 0000 0000  ?...>...........
-00000920: 1d00 0000 3f00 0300 8f00 0500 0000 0000  ....?...........
-00000930: 1d00 0000 4100 0300 8f00 0500 0000 0000  ....A...........
-00000940: 2400 0000 4300 0300 8f00 0500 0000 0000  $...C...........
-00000950: 3900 0000 4400 0300 8f00 0500 0000 0000  9...D...........
-00000960: 3100 0000 4500 0300 8f00 0500 0000 0000  1...E...........
-00000970: 3900 0000 4600 0300 8f00 0500 0000 0000  9...F...........
-00000980: 3100 0000 0000 0000 9305 0000 0000 0100  1...............
-00000990: 0000 0100 c103 0000 0200 6402 0000 0300  ..........d.....
-000009a0: 4102 0000 0400 0f03 0000 0500 8304 0000  A...............
-000009b0: 0600 7303 0000 0700 cc01 0000 0800 9801  ..s.............
-000009c0: 0000 0900 4f01 0000 0a00 3d05 0000 0b00  ....O.....=.....
-000009d0: e402 0000 0c00 2303 0000 0d00 ef04 0000  ......#.........
-000009e0: 0e00 1505 0000 0f00 4c03 0000 1000 3803  ........L.....8.
-000009f0: 0000 1100 4800 0000 1200 5800 0000 1300  ....H.....X.....
-00000a00: 3500 0000 1400 fc01 0000 1500 7704 0000  5...........w...
-00000a10: 1600 f703 0000 1700 6403 0000 1800 5f01  ........d....._.
-00000a20: 0000 1900 2100 0000 1a00 8702 0000 1b00  ....!...........
-00000a30: 6b01 0000 1c00 ea00 0000 1d00 d900 0000  k...............
-00000a40: 1e00 3501 0000 1f00 7801 0000 2000 c504  ..5.....x... ...
-00000a50: 0000 2100 aa04 0000 2200 9604 0000 2300  ..!.....".....#.
-00000a60: db04 0000 2400 8503 0000 2500 2c05 0000  ....$.....%.,...
-00000a70: 2600 4405 0000 2700 5605 0000 2800 fc04  &.D...'.V...(...
-00000a80: 0000 2900 0502 0000 2a00 bc01 0000 2b00  ..).....*.....+.
-00000a90: ac01 0000 2c00 5c02 0000 2d00 b600 0000  ....,.\...-.....
-00000aa0: 2e00 af03 0000 2f00 a503 0000 3000 7505  ....../.....0.u.
-00000ab0: 0000 3100 8405 0000 3200 6805 0000 3300  ..1.....2.h...3.
-00000ac0: 0304 0000 3400 ac03 0000 3600 be03 0000  ....4.....6.....
-00000ad0: 3700 1100 0000 3800 f001 0000 3900 e301  7.....8.....9...
-00000ae0: 0000 3a00 be03 0000 3b00 be03 0000 3d00  ..:.....;.....=.
-00000af0: de01 0000 3e00 1202 0000 3f00 1202 0000  ....>.....?.....
-00000b00: 4000 1202 0000 4200 af00 0000 4400 af00  @.....B.....D...
-00000b10: 0000 4500 1202 0000 4700 7c02 0000 4800  ..E.....G.|...H.
-00000b20: 7003 0000 4900 5502 0000 4a00 3103 0000  p...I.U...J.1...
-00000b30: 4b00 8f04 0000 4c00 f702 0000 4d00 3c02  K.....L.....M.<.
-00000b40: 0000 4e00 3c02 0000 4f00 c802 0000 5000  ..N.<...O.....P.
-00000b50: 6404 0000 5100 1e04 0000 5200 4e04 0000  d...Q.....R.N...
-00000b60: 5300 3804 0000 5400 1004 0000 5500 cc03  S.8...T.....U...
-00000b70: 0000 5600 e303 0000 5700 2501 0000 5800  ..V.....W.%...X.
-00000b80: bb02 0000 5900 1801 0000 5a00 9902 0000  ....Y.....Z.....
-00000b90: 5b00 f600 0000 5c00 a802 0000 5d00 0501  [.....\.....]...
-00000ba0: 0000 6000 de01 0000 6400 7003 0000 6600  ..`.....d.p...f.
-00000bb0: de01 0000 6700 de01 0000 6800 de01 0000  ....g.....h.....
-00000bc0: 6900 de01 0000 6a00 de01 0000 6b00 de01  i.....j.....k...
-00000bd0: 0000 6c00 de01 0000 6d00 de01 0000 6e00  ..l.....m.....n.
-00000be0: df02 0000 6f00 de01 0000 7100 9c05 0000  ....o.....q.....
-00000bf0: 7400 9105 0000 7600 be00 0000 7700 7e02  t.....v.....w.~.
-00000c00: 0000 7a00 c100 0000 7b00 df02 0000 7c00  ..z.....{.....|.
-00000c10: d803 0000 7d00 0c05 0000 7e00 de01 0000  ....}.....~.....
-00000c20: 8200 3102 0000 8300 9703 0000 8600 ee03  ..1.............
-00000c30: 0000 8700 4401 0000 8800 8a01 0000 8900  ....D...........
-00000c40: c700 0000 8a00 9105 0000 8b00 de01 0000  ................
-00000c50: 8c00 7003 0000 8d00 1202 0000 8e00 7c02  ..p...........|.
-00000c60: 0000 8f00 d803 0000 9000 d803 0000 9100  ................
-00000c70: d803 0000 9200 d803 0000 9300 d803 0000  ................
-00000c80: 9400 1202 0000 9500 df02 0000 9600 7003  ..............p.
-00000c90: 0000 9700 de01 0000 9a00 1b02 0000 9d00  ................
-00000ca0: 2802 0000 9e00 d802 0000 9f00 ac03 0000  (...............
-00000cb0: 0000 0c05 0000 0000 0c05 0000 0000 0c05  ................
-00000cc0: 0000 0200 9e03 0000 0300 7302 0000 0400  ..........s.....
-00000cd0: 0100 0000 0500 9002 6900 053e 9800 0b3e  ........i..>...>
-00000ce0: 7f00 113e 0103 173e 0000 0000 0100 f928  ...>...>.......(
-00000cf0: 0200 0000 0100 9c3e 0400 0000 2700 0400  .......>....'...
-00000d00: 9d01 2700 0500 c503 e300 0300 9b01 0301  ..'.............
-00000d10: 0300 9b01 2301 0300 9b01 6301 0300 9b01  ....#.....c.....
-00000d20: 8301 0300 9b01 a301 0300 9b01 0000 0000  ................
-00000d30: 0043 5324 3c3e 385f 5f6c 6f63 616c 7330  .CS$<>8__locals0
-00000d40: 0043 5324 3c3e 385f 5f6c 6f63 616c 7331  .CS$<>8__locals1
-00000d50: 006f 7074 696f 6e73 4469 7370 6c61 7955  .optionsDisplayU
-00000d60: 7365 7232 0077 6174 6572 5475 7262 696e  ser2.waterTurbin
-00000d70: 6544 6f6f 7243 4300 7468 6f74 684c 6566  eDoorCC.thothLef
-00000d80: 7444 6f6f 7243 4300 7468 6f74 6852 6967  tDoorCC.thothRig
-00000d90: 6874 446f 6f72 4343 0054 686f 7468 4272  htDoorCC.ThothBr
-00000da0: 6964 6765 4c65 6674 446f 6f72 4944 0041  idgeLeftDoorID.A
-00000db0: 3257 6174 6572 5475 7262 696e 654c 6566  2WaterTurbineLef
-00000dc0: 7444 6f6f 7249 4400 5468 6f74 6842 7269  tDoorID.ThothBri
-00000dd0: 6467 6552 6967 6874 446f 6f72 4944 0064  dgeRightDoorID.d
-00000de0: 6f6f 7249 4400 7376 366c 6f61 6400 6964  oorID.sv6load.id
-00000df0: 0066 6f75 6e64 0063 6f6c 6c69 7369 6f6e  .found.collision
-00000e00: 436f 6465 546f 4265 0073 686f 6f74 4d69  CodeToBe.shootMi
-00000e10: 7373 696c 6543 6f64 6500 6e65 7747 616d  ssileCode.newGam
-00000e20: 6543 6f64 6500 6465 7074 6873 5069 7065  eCode.depthsPipe
-00000e30: 436f 6465 0077 6174 6572 6661 6c6c 7350  Code.waterfallsP
-00000e40: 6970 6543 6f64 6500 6e65 7374 5069 7065  ipeCode.nestPipe
-00000e50: 436f 6465 0068 6964 656f 7574 5069 7065  Code.hideoutPipe
-00000e60: 436f 6465 0063 6853 7465 7046 6972 6543  Code.chStepFireC
-00000e70: 6f64 6500 6372 6561 7465 436f 6465 0075  ode.createCode.u
-00000e80: 6e6c 6f63 6b53 7475 6666 436f 6465 0064  nlockStuffCode.d
-00000e90: 7261 7747 7569 436f 6465 006c 6162 426c  rawGuiCode.labBl
-00000ea0: 6f63 6b43 6f64 6500 6368 5374 6570 436f  ockCode.chStepCo
-00000eb0: 6e74 726f 6c43 6f64 6500 636f 6c6c 6973  ntrolCode.collis
-00000ec0: 696f 6e43 6f64 6500 6761 6d65 5365 6c4d  ionCode.gameSelM
-00000ed0: 656e 7553 7465 7043 6f64 6500 6c6f 6164  enuStepCode.load
-00000ee0: 476c 6f62 616c 7343 6f64 6500 7361 7665  GlobalsCode.save
-00000ef0: 476c 6f62 616c 7343 6f64 6500 6368 6172  GlobalsCode.char
-00000f00: 6163 7465 7256 6172 7343 6f64 6500 636f  acterVarsCode.co
-00000f10: 6465 0061 3450 6167 6532 496d 6167 6500  de.a4Page2Image.
-00000f20: 6134 5061 6765 496d 6167 6500 7465 6d70  a4PageImage.temp
-00000f30: 5469 6c65 0073 7461 7274 4e65 7747 616d  Tile.startNewGam
-00000f40: 6500 636f 6465 4e61 6d65 0069 6e74 6572  e.codeName.inter
-00000f50: 6e61 6c4e 616d 6500 726f 6f6d 4e61 6d65  nalName.roomName
-00000f60: 0070 6963 6b75 704e 616d 6500 6e61 6d65  .pickupName.name
-00000f70: 0077 6973 646f 6d53 6570 746f 6767 4372  .wisdomSeptoggCr
-00000f80: 6561 7465 0063 7265 6174 6500 7376 3653  eate.create.sv6S
-00000f90: 6176 6500 6f57 6973 646f 6d53 6570 746f  ave.oWisdomSepto
-00000fa0: 6767 0066 696c 6550 6174 6800 6900 646f  gg.filePath.i.do
-00000fb0: 6f72 4c6f 636b 006c 6162 426c 6f63 6b00  orLock.labBlock.
-00000fc0: 7061 6765 4974 656d 0064 6570 7468 7350  pageItem.depthsP
-00000fd0: 6970 6552 6f6f 6d00 7761 7465 7266 616c  ipeRoom.waterfal
-00000fe0: 6c73 5069 7065 526f 6f6d 006e 6573 7450  lsPipeRoom.nestP
-00000ff0: 6970 6552 6f6f 6d00 6869 6465 6f75 7450  ipeRoom.hideoutP
-00001000: 6970 6552 6f6f 6d00 676d 526f 6f6d 0072  ipeRoom.gmRoom.r
-00001010: 6f6f 6d00 646f 6f72 5361 6d75 7343 6f6c  oom.doorSamusCol
-00001020: 6c69 7369 6f6e 0063 6f6c 6c69 7369 6f6e  lision.collision
-00001030: 0070 6167 6544 696d 656e 7369 6f6e 0077  .pageDimension.w
-00001040: 6973 646f 6d53 6570 746f 6767 4163 7469  isdomSeptoggActi
-00001050: 6f6e 0076 6172 446f 6f72 4163 7469 6f6e  on.varDoorAction
-00001060: 0061 6374 696f 6e00 6135 4163 7469 7661  .action.a5Activa
-00001070: 7465 436f 6e64 6974 696f 6e00 656d 7042  teCondition.empB
-00001080: 6174 7465 7279 4365 6c6c 436f 6e64 6974  atteryCellCondit
-00001090: 696f 6e00 7363 7244 4e41 5370 6177 6e00  ion.scrDNASpawn.
-000010a0: 676f 0077 6973 646f 6d53 6570 746f 6767  go.wisdomSeptogg
-000010b0: 5374 6570 0073 7562 7363 7265 656e 4d65  Step.subscreenMe
-000010c0: 6e75 5374 6570 0070 6963 6b75 7000 7375  nuStep.pickup.su
-000010d0: 6244 6972 0061 3544 6f6f 7200 6673 0073  bDir.a5Door.fs.s
-000010e0: 7636 6c6f 6164 4465 7461 696c 7300 6d73  v6loadDetails.ms
-000010f0: 0073 6565 644f 626a 6563 7400 736f 6c69  .seedObject.soli
-00001100: 644f 626a 6563 7400 6761 6d65 4f62 6a65  dObject.gameObje
-00001110: 6374 0070 6970 654f 626a 6563 7400 676d  ct.pipeObject.gm
-00001120: 4f62 6a65 6374 0065 6e65 6d79 4f62 6a65  Object.enemyObje
-00001130: 6374 0065 7461 6e6b 536e 6970 7065 7400  ct.etankSnippet.
-00001140: 7069 7065 4247 5469 6c65 7365 7400 6465  pipeBGTileset.de
-00001150: 7074 6873 456e 7472 616e 6365 5069 7065  pthsEntrancePipe
-00001160: 5469 6c65 7365 7400 7761 7465 7266 616c  Tileset.waterfal
-00001170: 6c73 5069 7065 5469 6c65 7365 7400 6465  lsPipeTileset.de
-00001180: 7074 6873 4578 6974 5069 7065 5469 6c65  pthsExitPipeTile
-00001190: 7365 7400 6869 6465 6f75 7450 6970 6554  set.hideoutPipeT
-000011a0: 696c 6573 6574 0064 6f6f 7254 696c 6573  ileset.doorTiles
-000011b0: 6574 0077 6973 646f 6d53 6570 746f 6767  et.wisdomSeptogg
-000011c0: 4576 656e 7400 7042 6f6d 6243 6861 7261  Event.pBombChara
-000011d0: 6374 6572 4576 656e 7400 7375 7065 724d  cterEvent.superM
-000011e0: 6973 7369 6c65 4368 6172 6163 7465 7245  issileCharacterE
-000011f0: 7665 6e74 006d 6973 7369 6c65 4368 6172  vent.missileChar
-00001200: 6163 7465 7245 7665 6e74 0065 5461 6e6b  acterEvent.eTank
-00001210: 4368 6172 6163 7465 7245 7665 6e74 0076  CharacterEvent.v
-00001220: 6172 446f 6f72 4576 656e 7400 6974 656d  arDoorEvent.item
-00001230: 7353 7761 7053 6372 6970 7400 636f 6465  sSwapScript.code
-00001240: 5465 7874 006e 6577 446f 6f72 5265 706c  Text.newDoorRepl
-00001250: 6163 656d 656e 7454 6578 7400 7375 6273  acementText.subs
-00001260: 6372 6565 6e4d 6973 6344 6177 0073 7344  creenMiscDaw.ssD
-00001270: 7261 7700 7375 6263 7265 656e 426f 6f74  raw.subcreenBoot
-00001280: 7344 7261 7700 7375 6273 6372 6565 6e53  sDraw.subscreenS
-00001290: 7569 7444 7261 7700 6472 6177 456e 6449  uitDraw.drawEndI
-000012a0: 6e64 6578 0064 6f6f 7245 7665 6e74 496e  ndex.doorEventIn
-000012b0: 6465 7800 6472 6177 5374 6172 7449 6e64  dex.drawStartInd
-000012c0: 6578 0061 7373 656d 626c 7900 7175 616e  ex.assembly.quan
-000012d0: 7469 7479 0000 0000 0000 0000 0fd0 2988  tity..........).
-000012e0: b811 1342 878b 770e 8597 ac16 f862 513f  ...B..w......bQ?
-000012f0: c607 d311 9053 00c0 4fa3 02a1 bc74 2e93  .....S..O....t..
-00001300: a9db 7844 8d46 0f32 a7ba b3d3 05ec feb5  ..xD.F.2........
-00001310: d08c 834a 96da 4662 84bb 4bd8 0847 4d7e  ...J..Fb..K..GM~
-00001320: 6e09 5c4c aeda cb10 ba6a 740d 0004 686f  n.\L.....jt...ho
-00001330: 6d65 0672 756e 6e65 7204 776f 726b 0459  me.runner.work.Y
-00001340: 414d 5308 5941 4d53 2d4c 4942 0a50 726f  AMS.YAMS-LIB.Pro
-00001350: 6772 616d 2e63 7309 2f00 0106 0d12 1217  gram.cs./.......
-00001360: 2020 fcd7 b607 0947 2a7f 005f d4dc 8bfa    .....G*.._....
-00001370: 96be 9c69 7aa0 808c d517 10d9 d077 717a  ...iz........wqz
-00001380: 270f 0d53 6565 644f 626a 6563 742e 6373  '..SeedObject.cs
-00001390: 092f 0001 060d 1212 1756 2056 65af b720  ./.......V Ve.. 
-000013a0: c3e8 22d1 155a 7563 de4b a863 e3cc 373b  .."..Zuc.K.c..7;
-000013b0: 3f57 25d2 3772 9abe a3a6 0a03 6f62 6a07  ?W%.7r......obj.
-000013c0: 5265 6c65 6173 6506 6e65 7436 2e30 1a59  Release.net6.0.Y
-000013d0: 414d 532d 4c49 422e 476c 6f62 616c 5573  AMS-LIB.GlobalUs
-000013e0: 696e 6773 2e67 2e63 7310 2f00 0106 0d12  ings.g.cs./.....
-000013f0: 1217 808f 8093 809b 80a2 205d d6d5 28fd  .......... ]..(.
-00001400: d6c4 4688 4302 02cd 32e6 b714 4a8a ec9d  ..F.C...2...J...
-00001410: fc9f 674a 11e9 0331 1930 c42e 2e4e 4554  ..gJ...1.0...NET
-00001420: 436f 7265 4170 702c 5665 7273 696f 6e3d  CoreApp,Version=
-00001430: 7636 2e30 2e41 7373 656d 626c 7941 7474  v6.0.AssemblyAtt
-00001440: 7269 6275 7465 732e 6373 102f 0001 060d  ributes.cs./....
-00001450: 1212 1780 8f80 9380 9b80 ef20 1b52 e6e7  ........... .R..
-00001460: b036 6edd 343e 8ff5 9513 2040 b1a2 8fb8  .6n.4>.... @....
-00001470: 8b5c 0213 ce84 0ad9 5cd9 8c80 1859 414d  .\......\....YAM
-00001480: 532d 4c49 422e 4173 7365 6d62 6c79 496e  S-LIB.AssemblyIn
-00001490: 666f 2e63 7310 2f00 0106 0d12 1217 808f  fo.cs./.........
-000014a0: 8093 809b 8150 2064 53b2 a2d9 9100 5cda  .....P dS.....\.
-000014b0: b8a4 1a2c ba44 9f9e 5f09 54dd 1ad3 f7d4  ...,.D.._.T.....
-000014c0: 9328 961c f1a2 5801 0282 2676 6572 7369  .(....X...&versi
-000014d0: 6f6e 0032 0063 6f6d 7069 6c65 722d 7665  on.2.compiler-ve
-000014e0: 7273 696f 6e00 342e 332e 312d 332e 3232  rsion.4.3.1-3.22
-000014f0: 3532 362e 3133 2b34 3161 3561 6639 6432  526.13+41a5af9d2
-00001500: 6334 3539 6130 3663 3037 3935 6266 3231  c459a06c0795bf21
-00001510: 6131 6330 3436 3230 3066 3337 3562 6600  a1c046200f375bf.
-00001520: 6c61 6e67 7561 6765 0043 2300 736f 7572  language.C#.sour
-00001530: 6365 2d66 696c 652d 636f 756e 7400 3500  ce-file-count.5.
-00001540: 6f75 7470 7574 2d6b 696e 6400 4479 6e61  output-kind.Dyna
-00001550: 6d69 6361 6c6c 794c 696e 6b65 644c 6962  micallyLinkedLib
-00001560: 7261 7279 006f 7074 696d 697a 6174 696f  rary.optimizatio
-00001570: 6e00 7265 6c65 6173 6500 706c 6174 666f  n.release.platfo
-00001580: 726d 0041 6e79 4370 7500 7275 6e74 696d  rm.AnyCpu.runtim
-00001590: 652d 7665 7273 696f 6e00 362e 302e 3230  e-version.6.0.20
-000015a0: 2b61 3038 6439 6365 3263 6166 3032 3435  +a08d9ce2caf0245
-000015b0: 3563 3062 3832 3562 6364 6333 3239 3734  5c0b825bcdc32974
-000015c0: 6264 6637 3639 6138 3000 6c61 6e67 7561  bdf769a80.langua
-000015d0: 6765 2d76 6572 7369 6f6e 0070 7265 7669  ge-version.previ
-000015e0: 6577 006e 756c 6c61 626c 6500 456e 6162  ew.nullable.Enab
-000015f0: 6c65 0064 6566 696e 6500 5452 4143 452c  le.define.TRACE,
-00001600: 5245 4c45 4153 452c 4e45 542c 4e45 5436  RELEASE,NET,NET6
-00001610: 5f30 2c4e 4554 434f 5245 4150 502c 4e45  _0,NETCOREAPP,NE
-00001620: 5435 5f30 5f4f 525f 4752 4541 5445 522c  T5_0_OR_GREATER,
-00001630: 4e45 5436 5f30 5f4f 525f 4752 4541 5445  NET6_0_OR_GREATE
-00001640: 522c 4e45 5443 4f52 4541 5050 315f 305f  R,NETCOREAPP1_0_
-00001650: 4f52 5f47 5245 4154 4552 2c4e 4554 434f  OR_GREATER,NETCO
-00001660: 5245 4150 5031 5f31 5f4f 525f 4752 4541  REAPP1_1_OR_GREA
-00001670: 5445 522c 4e45 5443 4f52 4541 5050 325f  TER,NETCOREAPP2_
-00001680: 305f 4f52 5f47 5245 4154 4552 2c4e 4554  0_OR_GREATER,NET
-00001690: 434f 5245 4150 5032 5f31 5f4f 525f 4752  COREAPP2_1_OR_GR
-000016a0: 4541 5445 522c 4e45 5443 4f52 4541 5050  EATER,NETCOREAPP
-000016b0: 325f 325f 4f52 5f47 5245 4154 4552 2c4e  2_2_OR_GREATER,N
-000016c0: 4554 434f 5245 4150 5033 5f30 5f4f 525f  ETCOREAPP3_0_OR_
-000016d0: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
-000016e0: 5050 335f 315f 4f52 5f47 5245 4154 4552  PP3_1_OR_GREATER
-000016f0: 00a3 ba49 4353 6861 7270 436f 6465 2e53  ...ICSharpCode.S
-00001700: 6861 7270 5a69 704c 6962 2e64 6c6c 0000  harpZipLib.dll..
-00001710: 016c 9904 9800 8003 0087 d282 16a4 95d1  .l..............
-00001720: 4abd 3f1f c402 13b4 ed4d 6163 726f 7373  J.?......Macross
-00001730: 2e4a 736f 6e2e 4578 7465 6e73 696f 6e73  .Json.Extensions
-00001740: 2e64 6c6c 0000 0155 c478 ba00 0001 00b2  .dll...U.x......
-00001750: 09ba d9ca d5dc 4e93 a42a 22b1 17ec 344d  ......N..*"...4M
-00001760: 6963 726f 736f 6674 2e43 5368 6172 702e  icrosoft.CSharp.
-00001770: 646c 6c00 0001 47c6 efd8 0080 0000 d96a  dll...G........j
-00001780: 5649 dd54 0c49 95c1 72e2 bede 4a9c 4d69  VI.T.I..r...J.Mi
-00001790: 6372 6f73 6f66 742e 5669 7375 616c 4261  crosoft.VisualBa
-000017a0: 7369 632e 436f 7265 2e64 6c6c 0000 015d  sic.Core.dll...]
-000017b0: c239 b300 2001 007a 712b af16 36a1 4597  .9.. ..zq+..6.E.
-000017c0: d099 df6a 10cb 084d 6963 726f 736f 6674  ...j...Microsoft
-000017d0: 2e56 6973 7561 6c42 6173 6963 2e64 6c6c  .VisualBasic.dll
-000017e0: 0000 01fa e955 eb00 8000 00bf f4e5 5cab  .....U........\.
-000017f0: 9b16 449d 61ef f7f0 cd2e 9b4d 6963 726f  ..D.a......Micro
-00001800: 736f 6674 2e57 696e 3332 2e50 7269 6d69  soft.Win32.Primi
-00001810: 7469 7665 732e 646c 6c00 0001 1c33 b5f2  tives.dll....3..
-00001820: 0080 0000 8bfb f897 ddfa 6d48 b60a 7e75  ..........mH..~u
-00001830: afde ee60 4d69 6372 6f73 6f66 742e 5769  ...`Microsoft.Wi
-00001840: 6e33 322e 5265 6769 7374 7279 2e64 6c6c  n32.Registry.dll
-00001850: 0000 012c 6d4a f000 a000 00f3 5176 e66b  ...,mJ......Qv.k
-00001860: 083b 4f93 4de7 b364 50f0 c56d 7363 6f72  .;O.M..dP..mscor
-00001870: 6c69 622e 646c 6c00 0001 078e a2d1 0020  lib.dll........ 
-00001880: 0100 46ac e58d 3099 4b4e 9d5f 2d92 40b9  ..F...0.KN._-.@.
-00001890: 5686 6e65 7473 7461 6e64 6172 642e 646c  V.netstandard.dl
-000018a0: 6c00 0001 289a 95e9 00c0 0100 42e4 4c29  l...(.......B.L)
-000018b0: 7e46 9546 9c21 3273 ea0b 0637 5072 6f70  ~F.F.!2s...7Prop
-000018c0: 6572 7479 4368 616e 6765 642e 646c 6c00  ertyChanged.dll.
-000018d0: 0001 8b5a 978a 0080 0000 3174 ff35 d3a6  ...Z......1t.5..
-000018e0: 344c 90ea 21b0 de57 7fe0 5369 784c 6162  4L..!..W..SixLab
-000018f0: 6f72 732e 496d 6167 6553 6861 7270 2e64  ors.ImageSharp.d
-00001900: 6c6c 0000 016c 8a3e dd00 601f 007f 776a  ll...l.>..`...wj
-00001910: e7b5 74d7 4aaa 9d41 db13 6c03 4353 7973  ..t.J..A..l.CSys
-00001920: 7465 6d2e 4170 7043 6f6e 7465 7874 2e64  tem.AppContext.d
-00001930: 6c6c 0000 015b 8ade d200 8000 0089 a4ac  ll...[..........
-00001940: c404 5a58 43a8 2833 44be d8fb be53 7973  ..ZXC.(3D....Sys
-00001950: 7465 6d2e 4275 6666 6572 732e 646c 6c00  tem.Buffers.dll.
-00001960: 0001 9615 a3d6 0080 0000 30db c586 fa12  ..........0.....
-00001970: cc48 9915 4529 34dc 734e 5379 7374 656d  .H..E)4.sNSystem
-00001980: 2e43 6f6c 6c65 6374 696f 6e73 2e43 6f6e  .Collections.Con
-00001990: 6375 7272 656e 742e 646c 6c00 0001 30aa  current.dll...0.
-000019a0: 53a0 00a0 0000 16c7 20b5 ca16 254c 9538  S....... ...%L.8
-000019b0: 30f8 8895 97e6 5379 7374 656d 2e43 6f6c  0.....System.Col
-000019c0: 6c65 6374 696f 6e73 2e64 6c6c 0000 0119  lections.dll....
-000019d0: ff1b c900 0001 005b 723e 7c55 d1d0 40ba  .......[r>|U..@.
-000019e0: dbf1 a37d 710f 2853 7973 7465 6d2e 436f  ...}q.(System.Co
-000019f0: 6c6c 6563 7469 6f6e 732e 496d 6d75 7461  llections.Immuta
-00001a00: 626c 652e 646c 6c00 0001 7470 3481 0040  ble.dll...tp4..@
-00001a10: 0100 94ab c85d 6d2d a546 98cf e522 935d  .....]m-.F...".]
-00001a20: 76d9 5379 7374 656d 2e43 6f6c 6c65 6374  v.System.Collect
-00001a30: 696f 6e73 2e4e 6f6e 4765 6e65 7269 632e  ions.NonGeneric.
-00001a40: 646c 6c00 0001 8a35 8787 00a0 0000 4907  dll....5......I.
-00001a50: 4905 ea31 6447 9ff3 c50e 856c eeae 5379  I..1dG.....l..Sy
-00001a60: 7374 656d 2e43 6f6c 6c65 6374 696f 6e73  stem.Collections
-00001a70: 2e53 7065 6369 616c 697a 6564 2e64 6c6c  .Specialized.dll
-00001a80: 0000 01f4 073b 9000 a000 0033 2054 df37  .....;.....3 T.7
-00001a90: b8cb 4d8b fc7d f812 16b3 6753 7973 7465  ..M..}....gSyste
-00001aa0: 6d2e 436f 6d70 6f6e 656e 744d 6f64 656c  m.ComponentModel
-00001ab0: 2e41 6e6e 6f74 6174 696f 6e73 2e64 6c6c  .Annotations.dll
-00001ac0: 0000 0113 6f38 f000 c000 0062 9284 9f82  ....o8.....b....
-00001ad0: d9cb 499d b5f6 60b4 e219 3f53 7973 7465  ..I...`...?Syste
-00001ae0: 6d2e 436f 6d70 6f6e 656e 744d 6f64 656c  m.ComponentModel
-00001af0: 2e44 6174 6141 6e6e 6f74 6174 696f 6e73  .DataAnnotations
-00001b00: 2e64 6c6c 0000 01ef 516e bb00 8000 00f2  .dll....Qn......
-00001b10: 06dc d38b c43c 4db2 f9b9 51fb 456a ca53  .....<M...Q.Ej.S
-00001b20: 7973 7465 6d2e 436f 6d70 6f6e 656e 744d  ystem.ComponentM
-00001b30: 6f64 656c 2e64 6c6c 0000 0158 e551 f900  odel.dll...X.Q..
-00001b40: 8000 002d e94b 5057 d67f 4ebf 345e d87e  ...-.KPW..N.4^.~
-00001b50: 5509 7553 7973 7465 6d2e 436f 6d70 6f6e  U.uSystem.Compon
-00001b60: 656e 744d 6f64 656c 2e45 7665 6e74 4261  entModel.EventBa
-00001b70: 7365 6441 7379 6e63 2e64 6c6c 0000 01fd  sedAsync.dll....
-00001b80: 1359 d900 8000 00d6 5d84 875a 916b 4c85  .Y......]..Z.kL.
-00001b90: cf06 6ec1 3ced 5953 7973 7465 6d2e 436f  ..n.<.YSystem.Co
-00001ba0: 6d70 6f6e 656e 744d 6f64 656c 2e50 7269  mponentModel.Pri
-00001bb0: 6d69 7469 7665 732e 646c 6c00 0001 b35c  mitives.dll....\
-00001bc0: cff3 00a0 0000 f825 95b8 06f2 b94c 88ec  .......%.....L..
-00001bd0: 71b1 2573 bb96 5379 7374 656d 2e43 6f6d  q.%s..System.Com
-00001be0: 706f 6e65 6e74 4d6f 6465 6c2e 5479 7065  ponentModel.Type
-00001bf0: 436f 6e76 6572 7465 722e 646c 6c00 0001  Converter.dll...
-00001c00: 87d4 77c6 00c0 0100 32f6 39fa e49c 614a  ..w.....2.9...aJ
-00001c10: 9459 2036 2da6 e4ce 5379 7374 656d 2e43  .Y 6-...System.C
-00001c20: 6f6e 6669 6775 7261 7469 6f6e 2e64 6c6c  onfiguration.dll
-00001c30: 0000 01f8 596f e700 8000 0042 fffc 8a7c  ....Yo.....B...|
-00001c40: 5d53 4181 a5e6 a6c7 b46c 7d53 7973 7465  ]SA......l}Syste
-00001c50: 6d2e 436f 6e73 6f6c 652e 646c 6c00 0001  m.Console.dll...
-00001c60: acd4 e7ea 00a0 0000 187d c652 3fb9 ee40  .........}.R?..@
-00001c70: 9bc2 1608 5d29 0e96 5379 7374 656d 2e43  ....])..System.C
-00001c80: 6f72 652e 646c 6c00 0001 ef54 abf3 00a0  ore.dll....T....
-00001c90: 0000 00de 77c9 e7d6 ee4d b8d3 90d7 c041  ....w....M.....A
-00001ca0: 2abb 5379 7374 656d 2e44 6174 612e 436f  *.System.Data.Co
-00001cb0: 6d6d 6f6e 2e64 6c6c 0000 0127 3883 a500  mmon.dll...'8...
-00001cc0: 8002 0060 9e73 825f 4f55 4599 d51f 935c  ...`.s._OUE....\
-00001cd0: 1b73 ec53 7973 7465 6d2e 4461 7461 2e44  .s.System.Data.D
-00001ce0: 6174 6153 6574 4578 7465 6e73 696f 6e73  ataSetExtensions
-00001cf0: 2e64 6c6c 0000 01c0 b73e d100 8000 00e8  .dll.....>......
-00001d00: fc4d 95e8 7eba 48a0 66d1 a1b6 8d65 3653  .M..~.H.f....e6S
-00001d10: 7973 7465 6d2e 4461 7461 2e64 6c6c 0000  ystem.Data.dll..
-00001d20: 0192 225e b000 a000 0065 917c b94f 066f  .."^.....e.|.O.o
-00001d30: 42a8 2ef1 5b20 6890 3653 7973 7465 6d2e  B...[ h.6System.
-00001d40: 4469 6167 6e6f 7374 6963 732e 436f 6e74  Diagnostics.Cont
-00001d50: 7261 6374 732e 646c 6c00 0001 72de dce7  racts.dll...r...
-00001d60: 0080 0000 5ebd c6fb 2ecf c347 8b76 9e5f  ....^......G.v._
-00001d70: f651 6344 5379 7374 656d 2e44 6961 676e  .QcDSystem.Diagn
-00001d80: 6f73 7469 6373 2e44 6562 7567 2e64 6c6c  ostics.Debug.dll
-00001d90: 0000 0125 93e8 be00 8000 0061 3e0d d53d  ...%.......a>..=
-00001da0: 94d6 4c9a bd3a 9596 1e8e d653 7973 7465  ..L..:.....Syste
-00001db0: 6d2e 4469 6167 6e6f 7374 6963 732e 4469  m.Diagnostics.Di
-00001dc0: 6167 6e6f 7374 6963 536f 7572 6365 2e64  agnosticSource.d
-00001dd0: 6c6c 0000 01ea 4e14 ab00 c000 008e 30dd  ll....N.......0.
-00001de0: 7896 2587 4780 29f1 6450 7118 dd53 7973  x.%.G.).dPq..Sys
-00001df0: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
-00001e00: 4669 6c65 5665 7273 696f 6e49 6e66 6f2e  FileVersionInfo.
-00001e10: 646c 6c00 0001 5104 04dc 0080 0000 6228  dll...Q.......b(
-00001e20: ad7f a93c 3e4f aca5 fca4 7f6b 877a 5379  ...<>O.....k.zSy
-00001e30: 7374 656d 2e44 6961 676e 6f73 7469 6373  stem.Diagnostics
-00001e40: 2e50 726f 6365 7373 2e64 6c6c 0000 0159  .Process.dll...Y
-00001e50: 7ca6 cc00 c000 0091 36b0 c21a c4a1 4db9  |.......6.....M.
-00001e60: a58f 052e a50e ea53 7973 7465 6d2e 4469  .......System.Di
-00001e70: 6167 6e6f 7374 6963 732e 5374 6163 6b54  agnostics.StackT
-00001e80: 7261 6365 2e64 6c6c 0000 015f 4645 9300  race.dll..._FE..
-00001e90: a000 004e 1214 b218 211a 4daf febf 03e1  ...N....!.M.....
-00001ea0: 54e1 d253 7973 7465 6d2e 4469 6167 6e6f  T..System.Diagno
-00001eb0: 7374 6963 732e 5465 7874 5772 6974 6572  stics.TextWriter
-00001ec0: 5472 6163 654c 6973 7465 6e65 722e 646c  TraceListener.dl
-00001ed0: 6c00 0001 0845 2dd5 0080 0000 bca0 6548  l....E-.......eH
-00001ee0: fd85 0a4e a070 85e6 9977 d562 5379 7374  ...N.p...w.bSyst
-00001ef0: 656d 2e44 6961 676e 6f73 7469 6373 2e54  em.Diagnostics.T
-00001f00: 6f6f 6c73 2e64 6c6c 0000 01e9 a48d db00  ools.dll........
-00001f10: 8000 00e4 34e6 e117 ed03 4dab db4c d23c  ....4.....M..L.<
-00001f20: d2b7 f653 7973 7465 6d2e 4469 6167 6e6f  ...System.Diagno
-00001f30: 7374 6963 732e 5472 6163 6553 6f75 7263  stics.TraceSourc
-00001f40: 652e 646c 6c00 0001 b9e1 c39c 00a0 0000  e.dll...........
-00001f50: 768e a771 85a5 c64b 88e2 2e20 7920 ca97  v..q...K... y ..
-00001f60: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
-00001f70: 6373 2e54 7261 6369 6e67 2e64 6c6c 0000  cs.Tracing.dll..
-00001f80: 01c7 1cda 8200 a000 005a 29e3 5590 7730  .........Z).U.w0
-00001f90: 4ea2 16ac bd1e 85dd 1f53 7973 7465 6d2e  N........System.
-00001fa0: 646c 6c00 0001 9ff7 2f95 0000 0100 72c2  dll...../.....r.
-00001fb0: a52c fc98 1545 bf36 65fb d680 63c6 5379  .,...E.6e...c.Sy
-00001fc0: 7374 656d 2e44 7261 7769 6e67 2e43 6f6d  stem.Drawing.Com
-00001fd0: 6d6f 6e2e 646c 6c00 0001 218d 42d5 0020  mon.dll...!.B.. 
-00001fe0: 0200 0843 fec0 6a78 bb46 9f62 dc8a c5b5  ...C..jx.F.b....
-00001ff0: 5abc 5379 7374 656d 2e44 7261 7769 6e67  Z.System.Drawing
-00002000: 2e64 6c6c 0000 016a deb2 a700 8000 005c  .dll...j.......\
-00002010: 62ba eee5 9288 498f 8887 e6ce 48b8 2753  b.....I.....H.'S
-00002020: 7973 7465 6d2e 4472 6177 696e 672e 5072  ystem.Drawing.Pr
-00002030: 696d 6974 6976 6573 2e64 6c6c 0000 01a1  imitives.dll....
-00002040: ed2e b100 c000 00ef a9bd 94b0 b301 4bad  ..............K.
-00002050: 8c71 e2bc 5086 b653 7973 7465 6d2e 4479  .q..P..System.Dy
-00002060: 6e61 6d69 632e 5275 6e74 696d 652e 646c  namic.Runtime.dl
-00002070: 6c00 0001 5ec8 ffb4 0080 0000 3e67 ee57  l...^.......>g.W
-00002080: f1d0 3a40 91cb c858 bc2b 07fb 5379 7374  ..:@...X.+..Syst
-00002090: 656d 2e46 6f72 6d61 7473 2e41 736e 312e  em.Formats.Asn1.
-000020a0: 646c 6c00 0001 173d 2fc4 00a0 0000 66e9  dll....=/.....f.
-000020b0: 9511 811c 2441 97b3 7ab9 7786 6d95 5379  ....$A..z.w.m.Sy
-000020c0: 7374 656d 2e47 6c6f 6261 6c69 7a61 7469  stem.Globalizati
-000020d0: 6f6e 2e43 616c 656e 6461 7273 2e64 6c6c  on.Calendars.dll
-000020e0: 0000 013c 9ca9 9200 8000 00fd 659e 1a8f  ...<........e...
-000020f0: 1109 47a9 cddc 0792 481d 7a53 7973 7465  ..G.....H.zSyste
-00002100: 6d2e 476c 6f62 616c 697a 6174 696f 6e2e  m.Globalization.
-00002110: 646c 6c00 0001 bbbb 2cf0 0080 0000 0532  dll.....,......2
-00002120: beb2 1b2d 0640 a8f0 19db 03af fa75 5379  ...-.@.......uSy
-00002130: 7374 656d 2e47 6c6f 6261 6c69 7a61 7469  stem.Globalizati
-00002140: 6f6e 2e45 7874 656e 7369 6f6e 732e 646c  on.Extensions.dl
-00002150: 6c00 0001 e836 bdee 0080 0000 5db4 08af  l....6......]...
-00002160: c052 114f 8782 5a7b d0bd b845 5379 7374  .R.O..Z{...ESyst
-00002170: 656d 2e49 4f2e 436f 6d70 7265 7373 696f  em.IO.Compressio
-00002180: 6e2e 4272 6f74 6c69 2e64 6c6c 0000 0141  n.Brotli.dll...A
-00002190: ef5d 8c00 8000 004f 3138 25ab 6cbf 48b2  .].....O18%.l.H.
-000021a0: 4a0a 9d25 10e6 e753 7973 7465 6d2e 494f  J..%...System.IO
-000021b0: 2e43 6f6d 7072 6573 7369 6f6e 2e64 6c6c  .Compression.dll
-000021c0: 0000 0180 1919 f600 a000 00b6 ddf3 e1d9  ................
-000021d0: 529a 418a 0686 b535 3604 0653 7973 7465  R.A....56..Syste
-000021e0: 6d2e 494f 2e43 6f6d 7072 6573 7369 6f6e  m.IO.Compression
-000021f0: 2e46 696c 6553 7973 7465 6d2e 646c 6c00  .FileSystem.dll.
-00002200: 0001 ad3b 45d6 0080 0000 0c9a 1bff 9e05  ...;E...........
-00002210: b842 8afb 18f3 a38a 2c82 5379 7374 656d  .B......,.System
-00002220: 2e49 4f2e 436f 6d70 7265 7373 696f 6e2e  .IO.Compression.
-00002230: 5a69 7046 696c 652e 646c 6c00 0001 da36  ZipFile.dll....6
-00002240: 6cfd 0080 0000 191c 89be afef 0240 bb3f  l............@.?
-00002250: 8613 a91c 17b3 5379 7374 656d 2e49 4f2e  ......System.IO.
-00002260: 646c 6c00 0001 5526 a3e1 0080 0000 cc3d  dll...U&.......=
-00002270: a9d0 4ba2 ee45 b67f 9a4d d5cb d130 5379  ..K..E...M...0Sy
-00002280: 7374 656d 2e49 4f2e 4669 6c65 5379 7374  stem.IO.FileSyst
-00002290: 656d 2e41 6363 6573 7343 6f6e 7472 6f6c  em.AccessControl
-000022a0: 2e64 6c6c 0000 019d 302f e400 a000 00eb  .dll....0/......
-000022b0: 3f6e a58d 4d04 4a93 2900 8682 7336 5253  ?n..M.J.)...s6RS
-000022c0: 7973 7465 6d2e 494f 2e46 696c 6553 7973  ystem.IO.FileSys
-000022d0: 7465 6d2e 646c 6c00 0001 062f 1abc 0080  tem.dll..../....
-000022e0: 0000 8bc3 fef2 74b3 aa44 bf94 ce4a a16d  ......t..D...J.m
-000022f0: 73ff 5379 7374 656d 2e49 4f2e 4669 6c65  s.System.IO.File
-00002300: 5379 7374 656d 2e44 7269 7665 496e 666f  System.DriveInfo
-00002310: 2e64 6c6c 0000 01cb 9c82 e100 8000 0031  .dll...........1
-00002320: 49ad b6e6 e4d7 4683 f1b0 4426 fc00 4e53  I.....F...D&..NS
-00002330: 7973 7465 6d2e 494f 2e46 696c 6553 7973  ystem.IO.FileSys
-00002340: 7465 6d2e 5072 696d 6974 6976 6573 2e64  tem.Primitives.d
-00002350: 6c6c 0000 016a bd8a f900 8000 0007 7706  ll...j........w.
-00002360: a4d6 3c3a 4eb1 9bc6 9dc1 b7d2 6753 7973  ..<:N.......gSys
-00002370: 7465 6d2e 494f 2e46 696c 6553 7973 7465  tem.IO.FileSyste
-00002380: 6d2e 5761 7463 6865 722e 646c 6c00 0001  m.Watcher.dll...
-00002390: a79b a9de 00a0 0000 a353 92b0 b0f9 c74a  .........S.....J
-000023a0: 83c4 d353 34da 117a 5379 7374 656d 2e49  ...S4..zSystem.I
-000023b0: 4f2e 4973 6f6c 6174 6564 5374 6f72 6167  O.IsolatedStorag
-000023c0: 652e 646c 6c00 0001 c228 8fc9 00a0 0000  e.dll....(......
-000023d0: a292 5ad8 1c16 a845 ad56 30b4 f934 9811  ..Z....E.V0..4..
-000023e0: 5379 7374 656d 2e49 4f2e 4d65 6d6f 7279  System.IO.Memory
-000023f0: 4d61 7070 6564 4669 6c65 732e 646c 6c00  MappedFiles.dll.
-00002400: 0001 a0ea 5490 0080 0000 d3e6 ebb7 6b95  ....T.........k.
-00002410: 6347 a586 6584 8570 f51a 5379 7374 656d  cG..e..p..System
-00002420: 2e49 4f2e 5069 7065 732e 4163 6365 7373  .IO.Pipes.Access
-00002430: 436f 6e74 726f 6c2e 646c 6c00 0001 0367  Control.dll....g
-00002440: 10da 0080 0000 fc19 0aca 8d4d c54d 949d  ...........M.M..
-00002450: 6663 06bb c0aa 5379 7374 656d 2e49 4f2e  fc....System.IO.
-00002460: 5069 7065 732e 646c 6c00 0001 c75d 7ae4  Pipes.dll....]z.
-00002470: 00a0 0000 0b85 4220 a9db f04f a006 3c12  ......B ...O..<.
-00002480: 1a57 6f3f 5379 7374 656d 2e49 4f2e 556e  .Wo?System.IO.Un
-00002490: 6d61 6e61 6765 644d 656d 6f72 7953 7472  managedMemoryStr
-000024a0: 6561 6d2e 646c 6c00 0001 b727 a8c8 0080  eam.dll....'....
-000024b0: 0000 78f2 7124 2f15 8d43 8f1b 9f8c 7dbd  ..x.q$/..C....}.
-000024c0: 49f3 5379 7374 656d 2e4c 696e 712e 646c  I.System.Linq.dl
-000024d0: 6c00 0001 ecba 89d4 00c0 0000 50d2 d044  l...........P..D
-000024e0: f7e4 544d 8ceb 9f33 11e6 9565 5379 7374  ..TM...3...eSyst
-000024f0: 656d 2e4c 696e 712e 4578 7072 6573 7369  em.Linq.Expressi
-00002500: 6f6e 732e 646c 6c00 0001 aeab 34d1 0040  ons.dll.....4..@
-00002510: 0100 179a d71a f148 2c4c 8f91 b678 48f0  .......H,L...xH.
-00002520: bc45 5379 7374 656d 2e4c 696e 712e 5061  .ESystem.Linq.Pa
-00002530: 7261 6c6c 656c 2e64 6c6c 0000 0171 f92d  rallel.dll...q.-
-00002540: fd00 c000 005b 7a8b 25a6 13dd 40b7 9157  .....[z.%...@..W
-00002550: 9a48 f31d 6553 7973 7465 6d2e 4c69 6e71  .H..eSystem.Linq
-00002560: 2e51 7565 7279 6162 6c65 2e64 6c6c 0000  .Queryable.dll..
-00002570: 01bf 6453 b400 c000 0016 962a 0bf2 e78f  ..dS.......*....
-00002580: 47aa bd26 32d7 c910 6153 7973 7465 6d2e  G..&2...aSystem.
-00002590: 4d65 6d6f 7279 2e64 6c6c 0000 012d 8b86  Memory.dll...-..
-000025a0: cb00 e000 008e e400 8c69 9bab 4ba7 36a0  .........i..K.6.
-000025b0: d5f6 e593 0353 7973 7465 6d2e 4e65 742e  .....System.Net.
-000025c0: 646c 6c00 0001 0980 6ea0 0080 0000 a225  dll.....n......%
-000025d0: c34a 55cb a24a adc1 3e87 8d45 29bf 5379  .JU..J..>..E).Sy
-000025e0: 7374 656d 2e4e 6574 2e48 7474 702e 646c  stem.Net.Http.dl
-000025f0: 6c00 0001 d221 b7f5 0020 0100 fb7d 3bd4  l....!... ...};.
-00002600: 96eb bf4d a0f3 2ffd 1862 c8a7 5379 7374  ...M../..b..Syst
-00002610: 656d 2e4e 6574 2e48 7474 702e 4a73 6f6e  em.Net.Http.Json
-00002620: 2e64 6c6c 0000 0136 39b1 9300 8000 0050  .dll...69......P
-00002630: 41cc 88dc 6bfb 4194 4d0a 420e c558 6053  A...k.A.M.B..X`S
-00002640: 7973 7465 6d2e 4e65 742e 4874 7470 4c69  ystem.Net.HttpLi
-00002650: 7374 656e 6572 2e64 6c6c 0000 016d 7d75  stener.dll...m}u
-00002660: ec00 a000 0058 cc44 dd90 7278 44a4 9390  .....X.D..rxD...
-00002670: 0ee2 1d37 2f53 7973 7465 6d2e 4e65 742e  ...7/System.Net.
-00002680: 4d61 696c 2e64 6c6c 0000 0114 a2ee f800  Mail.dll........
-00002690: c000 00b9 ac14 7e53 c633 4793 93ef a225  ......~S.3G....%
-000026a0: 9b6a 9c53 7973 7465 6d2e 4e65 742e 4e61  .j.System.Net.Na
-000026b0: 6d65 5265 736f 6c75 7469 6f6e 2e64 6c6c  meResolution.dll
-000026c0: 0000 010e 31a1 e800 8000 0017 54e0 d2a3  ....1.......T...
-000026d0: b831 4185 8389 daa1 11e4 4a53 7973 7465  .1A.......JSyste
-000026e0: 6d2e 4e65 742e 4e65 7477 6f72 6b49 6e66  m.Net.NetworkInf
-000026f0: 6f72 6d61 7469 6f6e 2e64 6c6c 0000 0184  ormation.dll....
-00002700: 8010 db00 c000 0002 ec9b e527 f590 4f9c  ...........'..O.
-00002710: a084 92bb 9cd0 0653 7973 7465 6d2e 4e65  .......System.Ne
-00002720: 742e 5069 6e67 2e64 6c6c 0000 0150 a9ef  t.Ping.dll...P..
-00002730: ae00 8000 00fb 0f9e 9d92 7ced 4abe 7468  ..........|.J.th
-00002740: b1b1 0fbb 7253 7973 7465 6d2e 4e65 742e  ....rSystem.Net.
-00002750: 5072 696d 6974 6976 6573 2e64 6c6c 0000  Primitives.dll..
-00002760: 0122 5f3d 9c00 c000 00b3 f312 5c38 f5a6  ."_=........\8..
-00002770: 44a2 6443 ddb2 b957 8753 7973 7465 6d2e  D.dC...W.System.
-00002780: 4e65 742e 5265 7175 6573 7473 2e64 6c6c  Net.Requests.dll
-00002790: 0000 01b1 e6d6 e200 e000 0012 2a7d f4cc  ............*}..
-000027a0: 6686 43b3 7e9c 3d4a 095b 6853 7973 7465  f.C.~.=J.[hSyste
-000027b0: 6d2e 4e65 742e 5365 6375 7269 7479 2e64  m.Net.Security.d
-000027c0: 6c6c 0000 0127 cb34 a100 0001 0005 3537  ll...'.4......57
-000027d0: 2f56 07c3 41a9 cb3e 1a6b cfd1 a353 7973  /V..A..>.k...Sys
-000027e0: 7465 6d2e 4e65 742e 5365 7276 6963 6550  tem.Net.ServiceP
-000027f0: 6f69 6e74 2e64 6c6c 0000 01dd 25a4 de00  oint.dll....%...
-00002800: 8000 00ed 725d 73aa 9d5e 43ba 48ff fe44  ....r]s..^C.H..D
-00002810: 12af e153 7973 7465 6d2e 4e65 742e 536f  ...System.Net.So
-00002820: 636b 6574 732e 646c 6c00 0001 4bd3 a1bb  ckets.dll...K...
-00002830: 0000 0100 2bf1 3882 33fb 644e 9f6f f7d9  ....+.8.3.dN.o..
-00002840: 78a5 252f 5379 7374 656d 2e4e 6574 2e57  x.%/System.Net.W
-00002850: 6562 436c 6965 6e74 2e64 6c6c 0000 01b6  ebClient.dll....
-00002860: fd0c 9e00 a000 0046 df99 c9ca 5709 44af  .......F....W.D.
-00002870: 279d 66f8 9b3d 0553 7973 7465 6d2e 4e65  '.f..=.System.Ne
-00002880: 742e 5765 6248 6561 6465 7243 6f6c 6c65  t.WebHeaderColle
-00002890: 6374 696f 6e2e 646c 6c00 0001 6a1a e1fd  ction.dll...j...
-000028a0: 0080 0000 a27b f64a fc24 574d b8a9 963d  .....{.J.$WM...=
-000028b0: 4516 74e0 5379 7374 656d 2e4e 6574 2e57  E.t.System.Net.W
-000028c0: 6562 5072 6f78 792e 646c 6c00 0001 9af5  ebProxy.dll.....
-000028d0: 2896 0080 0000 0f24 8fb0 36d6 d440 a983  (......$..6..@..
-000028e0: c95e 29ea cefe 5379 7374 656d 2e4e 6574  .^)...System.Net
-000028f0: 2e57 6562 536f 636b 6574 732e 436c 6965  .WebSockets.Clie
-00002900: 6e74 2e64 6c6c 0000 0110 ab9a ef00 8000  nt.dll..........
-00002910: 006e a6d2 6d31 e9ee 44b0 71a4 e42b df89  .n..m1..D.q..+..
-00002920: 3a53 7973 7465 6d2e 4e65 742e 5765 6253  :System.Net.WebS
-00002930: 6f63 6b65 7473 2e64 6c6c 0000 0104 8ed9  ockets.dll......
-00002940: bf00 a000 00e5 53b0 5f28 5128 4e8b 98c7  ......S._(Q(N...
-00002950: 16ed 5710 4d53 7973 7465 6d2e 4e75 6d65  ..W.MSystem.Nume
-00002960: 7269 6373 2e64 6c6c 0000 011e 3a6e da00  rics.dll....:n..
-00002970: 8000 009a ac6a 5a97 81db 468d 2e74 842b  .....jZ...F..t.+
-00002980: 7926 0553 7973 7465 6d2e 4e75 6d65 7269  y&.System.Numeri
-00002990: 6373 2e56 6563 746f 7273 2e64 6c6c 0000  cs.Vectors.dll..
-000029a0: 01c5 797f e000 c000 0048 2159 1d6c 0961  ..y......H!Y.l.a
-000029b0: 408f 705c 1849 c826 9f53 7973 7465 6d2e  @.p\.I.&.System.
-000029c0: 4f62 6a65 6374 4d6f 6465 6c2e 646c 6c00  ObjectModel.dll.
-000029d0: 0001 faaa 3990 00c0 0000 0a0f 24e7 04e0  ....9.......$...
-000029e0: 6f4e b449 6ef8 be77 cb96 5379 7374 656d  oN.In..w..System
-000029f0: 2e52 6566 6c65 6374 696f 6e2e 4469 7370  .Reflection.Disp
-00002a00: 6174 6368 5072 6f78 792e 646c 6c00 0001  atchProxy.dll...
-00002a10: 2772 2cec 0080 0000 1698 c373 6c97 204c  'r,........sl. L
-00002a20: 9596 3afb 764e c10f 5379 7374 656d 2e52  ..:.vN..System.R
-00002a30: 6566 6c65 6374 696f 6e2e 646c 6c00 0001  eflection.dll...
-00002a40: bd34 27cf 0080 0000 054f 9a90 eb0c 4644  .4'......O....FD
-00002a50: b3e6 2a92 44f8 700f 5379 7374 656d 2e52  ..*.D.p.System.R
-00002a60: 6566 6c65 6374 696f 6e2e 456d 6974 2e64  eflection.Emit.d
-00002a70: 6c6c 0000 019b a4f7 9100 e000 00d4 17f5  ll..............
-00002a80: 4cf1 03c4 4a87 0dca c522 764c e853 7973  L...J...."vL.Sys
-00002a90: 7465 6d2e 5265 666c 6563 7469 6f6e 2e45  tem.Reflection.E
-00002aa0: 6d69 742e 494c 4765 6e65 7261 7469 6f6e  mit.ILGeneration
-00002ab0: 2e64 6c6c 0000 0124 f749 e600 a000 0096  .dll...$.I......
-00002ac0: 3ff7 7b06 112f 4e84 c255 f1ab 45b2 3653  ?.{../N..U..E.6S
-00002ad0: 7973 7465 6d2e 5265 666c 6563 7469 6f6e  ystem.Reflection
-00002ae0: 2e45 6d69 742e 4c69 6768 7477 6569 6768  .Emit.Lightweigh
-00002af0: 742e 646c 6c00 0001 8d8c 18c1 0080 0000  t.dll...........
-00002b00: 7abf 3e49 5c46 6b41 8e1e 1287 ee95 2a37  z.>I\FkA......*7
-00002b10: 5379 7374 656d 2e52 6566 6c65 6374 696f  System.Reflectio
-00002b20: 6e2e 4578 7465 6e73 696f 6e73 2e64 6c6c  n.Extensions.dll
-00002b30: 0000 017b 4679 8800 8000 00b0 9bbe a18d  ...{Fy..........
-00002b40: 8924 46a0 0079 200a 96d5 6553 7973 7465  .$F..y ...eSyste
-00002b50: 6d2e 5265 666c 6563 7469 6f6e 2e4d 6574  m.Reflection.Met
-00002b60: 6164 6174 612e 646c 6c00 0001 9185 f5dc  adata.dll.......
-00002b70: 0020 0200 957c e741 e662 dd4e ae71 2827  . ...|.A.b.N.q('
-00002b80: de74 6fdf 5379 7374 656d 2e52 6566 6c65  .to.System.Refle
-00002b90: 6374 696f 6e2e 5072 696d 6974 6976 6573  ction.Primitives
-00002ba0: 2e64 6c6c 0000 01be 3cc3 b000 a000 009c  .dll....<.......
-00002bb0: d456 8863 e4cb 499b f7fd 26b7 b608 3253  .V.c..I...&...2S
-00002bc0: 7973 7465 6d2e 5265 666c 6563 7469 6f6e  ystem.Reflection
-00002bd0: 2e54 7970 6545 7874 656e 7369 6f6e 732e  .TypeExtensions.
-00002be0: 646c 6c00 0001 cd87 87f0 0080 0000 5c48  dll...........\H
-00002bf0: 4518 1ace ee4d 81de 7d10 c3aa 89dc 5379  E....M..}.....Sy
-00002c00: 7374 656d 2e52 6573 6f75 7263 6573 2e52  stem.Resources.R
-00002c10: 6561 6465 722e 646c 6c00 0001 65fd 089e  eader.dll...e...
-00002c20: 0080 0000 e16f 0044 72de db47 9d23 be04  .....o.Dr..G.#..
-00002c30: a5a6 1c49 5379 7374 656d 2e52 6573 6f75  ...ISystem.Resou
-00002c40: 7263 6573 2e52 6573 6f75 7263 654d 616e  rces.ResourceMan
-00002c50: 6167 6572 2e64 6c6c 0000 0140 c061 9900  ager.dll...@.a..
-00002c60: 8000 0026 7baa 39d7 ce0d 41b2 8948 5c6c  ...&{.9...A..H\l
-00002c70: 703a 7753 7973 7465 6d2e 5265 736f 7572  p:wSystem.Resour
-00002c80: 6365 732e 5772 6974 6572 2e64 6c6c 0000  ces.Writer.dll..
-00002c90: 01b2 f475 8700 8000 00b6 e3ab edad 3c4f  ...u..........<O
-00002ca0: 4497 234e 1478 202f 1d53 7973 7465 6d2e  D.#N.x /.System.
-00002cb0: 5275 6e74 696d 652e 436f 6d70 696c 6572  Runtime.Compiler
-00002cc0: 5365 7276 6963 6573 2e55 6e73 6166 652e  Services.Unsafe.
-00002cd0: 646c 6c00 0001 e8cd 63c0 0080 0000 c064  dll.....c......d
-00002ce0: 945f 1680 9043 9783 ffcf 791d 15a3 5379  ._...C....y...Sy
-00002cf0: 7374 656d 2e52 756e 7469 6d65 2e43 6f6d  stem.Runtime.Com
-00002d00: 7069 6c65 7253 6572 7669 6365 732e 5669  pilerServices.Vi
-00002d10: 7375 616c 432e 646c 6c00 0001 2449 43ae  sualC.dll...$IC.
-00002d20: 0080 0000 9f3e 656f 662e ae4b b5d4 0a54  .....>eof..K...T
-00002d30: 4678 3422 5379 7374 656d 2e52 756e 7469  Fx4"System.Runti
-00002d40: 6d65 2e64 6c6c 0000 01bf 8954 b600 8007  me.dll.....T....
-00002d50: 00e7 437d d555 b958 41af ecbc dc7d 56c8  ..C}.U.XA....}V.
-00002d60: 8653 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
-00002d70: 4578 7465 6e73 696f 6e73 2e64 6c6c 0000  Extensions.dll..
-00002d80: 015f 2b89 9900 8000 0086 8512 1f40 0c2e  ._+..........@..
-00002d90: 4cab d8b7 af99 e1f0 1a53 7973 7465 6d2e  L........System.
-00002da0: 5275 6e74 696d 652e 4861 6e64 6c65 732e  Runtime.Handles.
-00002db0: 646c 6c00 0001 d3eb c8ba 0080 0000 149d  dll.............
-00002dc0: 6d9d 9fe0 df41 b571 bc52 3862 c115 5379  m....A.q.R8b..Sy
-00002dd0: 7374 656d 2e52 756e 7469 6d65 2e49 6e74  stem.Runtime.Int
-00002de0: 6572 6f70 5365 7276 6963 6573 2e64 6c6c  eropServices.dll
-00002df0: 0000 0125 255e b400 4001 00cb bc2f 91fc  ...%%^..@..../..
-00002e00: 4400 47a5 bffd b402 d23a 0c53 7973 7465  D.G......:.Syste
-00002e10: 6d2e 5275 6e74 696d 652e 496e 7465 726f  m.Runtime.Intero
-00002e20: 7053 6572 7669 6365 732e 5275 6e74 696d  pServices.Runtim
-00002e30: 6549 6e66 6f72 6d61 7469 6f6e 2e64 6c6c  eInformation.dll
-00002e40: 0000 0102 bbc2 c600 8000 0012 e6ce 96d8  ................
-00002e50: 6458 4f80 1245 97c8 86a0 dd53 7973 7465  dXO..E.....Syste
-00002e60: 6d2e 5275 6e74 696d 652e 496e 7472 696e  m.Runtime.Intrin
-00002e70: 7369 6373 2e64 6c6c 0000 0192 0503 e300  sics.dll........
-00002e80: c002 00fb af84 1b4c 75b3 4bb7 d6bf 3c99  .......Lu.K...<.
-00002e90: c33c 9c53 7973 7465 6d2e 5275 6e74 696d  .<.System.Runtim
-00002ea0: 652e 4c6f 6164 6572 2e64 6c6c 0000 015b  e.Loader.dll...[
-00002eb0: 2286 d600 8000 001c a246 11fa 600b 43b0  "........F..`.C.
-00002ec0: 7044 fb74 f66a 8f53 7973 7465 6d2e 5275  pD.t.j.System.Ru
-00002ed0: 6e74 696d 652e 4e75 6d65 7269 6373 2e64  ntime.Numerics.d
-00002ee0: 6c6c 0000 0131 659d dd00 a000 0014 f2d9  ll...1e.........
-00002ef0: 18c2 0653 4c83 3495 6a63 8df8 6253 7973  ...SL.4.jc..bSys
-00002f00: 7465 6d2e 5275 6e74 696d 652e 5365 7269  tem.Runtime.Seri
-00002f10: 616c 697a 6174 696f 6e2e 646c 6c00 0001  alization.dll...
-00002f20: fdbb 2fdf 0080 0000 e3b7 a154 0b4c 8c49  ../........T.L.I
-00002f30: b13c 7f1a fb4a 5238 5379 7374 656d 2e52  .<...JR8System.R
-00002f40: 756e 7469 6d65 2e53 6572 6961 6c69 7a61  untime.Serializa
-00002f50: 7469 6f6e 2e46 6f72 6d61 7474 6572 732e  tion.Formatters.
-00002f60: 646c 6c00 0001 459b adaa 00a0 0000 b754  dll...E........T
-00002f70: 8818 fc66 f440 850f 5201 c285 fd87 5379  ...f.@..R.....Sy
-00002f80: 7374 656d 2e52 756e 7469 6d65 2e53 6572  stem.Runtime.Ser
-00002f90: 6961 6c69 7a61 7469 6f6e 2e4a 736f 6e2e  ialization.Json.
-00002fa0: 646c 6c00 0001 642f 34a9 0080 0000 0b35  dll...d/4......5
-00002fb0: eae0 1874 d441 abe3 c377 bb91 25c0 5379  ...t.A...w..%.Sy
-00002fc0: 7374 656d 2e52 756e 7469 6d65 2e53 6572  stem.Runtime.Ser
-00002fd0: 6961 6c69 7a61 7469 6f6e 2e50 7269 6d69  ialization.Primi
-00002fe0: 7469 7665 732e 646c 6c00 0001 e1b6 80c5  tives.dll.......
-00002ff0: 0080 0000 3b2f 2733 7550 dc48 8880 aac3  ....;/'3uP.H....
-00003000: 1683 74c1 5379 7374 656d 2e52 756e 7469  ..t.System.Runti
-00003010: 6d65 2e53 6572 6961 6c69 7a61 7469 6f6e  me.Serialization
-00003020: 2e58 6d6c 2e64 6c6c 0000 016b cc9d 8300  .Xml.dll...k....
-00003030: c000 00d3 10de 2455 2c1e 46b0 6be0 0dc8  ......$U,.F.k...
-00003040: b32f d753 7973 7465 6d2e 5365 6375 7269  ./.System.Securi
-00003050: 7479 2e41 6363 6573 7343 6f6e 7472 6f6c  ty.AccessControl
-00003060: 2e64 6c6c 0000 01c6 8554 ad00 e000 006d  .dll.....T.....m
-00003070: d9e4 ef6d 65ed 4da8 95ad 65d8 5600 0853  ...me.M...e.V..S
-00003080: 7973 7465 6d2e 5365 6375 7269 7479 2e43  ystem.Security.C
-00003090: 6c61 696d 732e 646c 6c00 0001 d51b 3e97  laims.dll.....>.
-000030a0: 00c0 0000 e611 cad5 7c7f a34a b001 6c2e  ........|..J..l.
-000030b0: 1dbb 6201 5379 7374 656d 2e53 6563 7572  ..b.System.Secur
-000030c0: 6974 792e 4372 7970 746f 6772 6170 6879  ity.Cryptography
-000030d0: 2e41 6c67 6f72 6974 686d 732e 646c 6c00  .Algorithms.dll.
-000030e0: 0001 3c1e 9efd 0000 0100 c36e f353 6021  ..<........n.S`!
-000030f0: 2141 926f c2d1 dfec cd48 5379 7374 656d  !A.o.....HSystem
-00003100: 2e53 6563 7572 6974 792e 4372 7970 746f  .Security.Crypto
-00003110: 6772 6170 6879 2e43 6e67 2e64 6c6c 0000  graphy.Cng.dll..
-00003120: 01e0 a15c a500 c000 00dc 3da2 1f65 85fc  ...\......=..e..
-00003130: 4b93 569a b1e1 3f01 8b53 7973 7465 6d2e  K.V...?..System.
-00003140: 5365 6375 7269 7479 2e43 7279 7074 6f67  Security.Cryptog
-00003150: 7261 7068 792e 4373 702e 646c 6c00 0001  raphy.Csp.dll...
-00003160: 5380 3cbb 00a0 0000 d655 7828 fc10 3945  S.<......Ux(..9E
-00003170: bcfc 09c5 ddc3 7d87 5379 7374 656d 2e53  ......}.System.S
-00003180: 6563 7572 6974 792e 4372 7970 746f 6772  ecurity.Cryptogr
-00003190: 6170 6879 2e45 6e63 6f64 696e 672e 646c  aphy.Encoding.dl
-000031a0: 6c00 0001 d4f7 90cf 00a0 0000 61ef 1c33  l...........a..3
-000031b0: 1ffc 0c42 82a9 f95a 4a3c 0210 5379 7374  ...B...ZJ<..Syst
-000031c0: 656d 2e53 6563 7572 6974 792e 4372 7970  em.Security.Cryp
-000031d0: 746f 6772 6170 6879 2e4f 7065 6e53 736c  tography.OpenSsl
-000031e0: 2e64 6c6c 0000 0133 7574 9500 8000 00c8  .dll...3ut......
-000031f0: 8e54 21e0 29d9 4e93 b460 168b bae5 ab53  .T!.).N..`.....S
-00003200: 7973 7465 6d2e 5365 6375 7269 7479 2e43  ystem.Security.C
-00003210: 7279 7074 6f67 7261 7068 792e 5072 696d  ryptography.Prim
-00003220: 6974 6976 6573 2e64 6c6c 0000 0147 62c0  itives.dll...Gb.
-00003230: aa00 a000 00e5 c4ae 8a61 2a8b 4a91 b6db  .........a*.J...
-00003240: 9cc8 e03d 2053 7973 7465 6d2e 5365 6375  ...= System.Secu
-00003250: 7269 7479 2e43 7279 7074 6f67 7261 7068  rity.Cryptograph
-00003260: 792e 5835 3039 4365 7274 6966 6963 6174  y.X509Certificat
-00003270: 6573 2e64 6c6c 0000 015e ebd1 aa00 e000  es.dll...^......
-00003280: 00f7 362a 79bd 9443 44b6 d1f0 7262 e71c  ..6*y..CD...rb..
-00003290: c453 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
-000032a0: 2e64 6c6c 0000 0155 c3f0 9000 8000 00b1  .dll...U........
-000032b0: ef68 ebcc 027f 46bd b323 4f6d 501c 0453  .h....F..#OmP..S
-000032c0: 7973 7465 6d2e 5365 6375 7269 7479 2e50  ystem.Security.P
-000032d0: 7269 6e63 6970 616c 2e64 6c6c 0000 01b3  rincipal.dll....
-000032e0: ece5 9300 8000 0028 f027 67ce 1653 4699  .......(.'g..SF.
-000032f0: 4b5d 7242 35d3 7c53 7973 7465 6d2e 5365  K]rB5.|System.Se
-00003300: 6375 7269 7479 2e50 7269 6e63 6970 616c  curity.Principal
-00003310: 2e57 696e 646f 7773 2e64 6c6c 0000 012a  .Windows.dll...*
-00003320: 2c96 f600 a000 00c6 cf87 eee2 9dc1 47bf  ,.............G.
-00003330: de8e 88fd 2df4 a553 7973 7465 6d2e 5365  ....-..System.Se
-00003340: 6375 7269 7479 2e53 6563 7572 6553 7472  curity.SecureStr
-00003350: 696e 672e 646c 6c00 0001 6d70 ebd5 0080  ing.dll...mp....
-00003360: 0000 b966 5d46 6a67 c542 8aad 9de3 e7ee  ...f]Fjg.B......
-00003370: b093 5379 7374 656d 2e53 6572 7669 6365  ..System.Service
-00003380: 4d6f 6465 6c2e 5765 622e 646c 6c00 0001  Model.Web.dll...
-00003390: 1092 8a91 0080 0000 1e5b 470c cc18 234b  .........[G...#K
-000033a0: b279 39c9 a373 179d 5379 7374 656d 2e53  .y9..s..System.S
-000033b0: 6572 7669 6365 5072 6f63 6573 732e 646c  erviceProcess.dl
-000033c0: 6c00 0001 a07e 48df 0080 0000 85ae 4c40  l....~H.......L@
-000033d0: 2f8d 744f 8ab8 4c05 93b7 6184 5379 7374  /.tO..L...a.Syst
-000033e0: 656d 2e54 6578 742e 456e 636f 6469 6e67  em.Text.Encoding
-000033f0: 2e43 6f64 6550 6167 6573 2e64 6c6c 0000  .CodePages.dll..
-00003400: 016f 3804 c300 8000 00af c423 87a8 0177  .o8........#...w
-00003410: 4a98 164e 7acc a55d 9e53 7973 7465 6d2e  J..Nz..].System.
-00003420: 5465 7874 2e45 6e63 6f64 696e 672e 646c  Text.Encoding.dl
-00003430: 6c00 0001 49ed f0da 0080 0000 a0af 7ca1  l...I.........|.
-00003440: 6a0d ed4e 871e d1e0 fb5b 5e56 5379 7374  j..N.....[^VSyst
-00003450: 656d 2e54 6578 742e 456e 636f 6469 6e67  em.Text.Encoding
-00003460: 2e45 7874 656e 7369 6f6e 732e 646c 6c00  .Extensions.dll.
-00003470: 0001 7749 18b5 00a0 0000 788b aa6e 72da  ..wI......x..nr.
-00003480: b340 930b 4205 1372 4879 5379 7374 656d  .@..B..rHySystem
-00003490: 2e54 6578 742e 456e 636f 6469 6e67 732e  .Text.Encodings.
-000034a0: 5765 622e 646c 6c00 0001 d8c3 deb4 00a0  Web.dll.........
-000034b0: 0000 2143 d0a9 94be e646 8644 4880 f0b6  ..!C.....F.DH...
-000034c0: 3754 5379 7374 656d 2e54 6578 742e 4a73  7TSystem.Text.Js
-000034d0: 6f6e 2e64 6c6c 0000 01c2 0dee c800 2001  on.dll........ .
-000034e0: 00c8 9236 85cc b0c6 4bbc 1fe9 06cf fe3a  ...6....K......:
-000034f0: 2e53 7973 7465 6d2e 5465 7874 2e52 6567  .System.Text.Reg
-00003500: 756c 6172 4578 7072 6573 7369 6f6e 732e  ularExpressions.
-00003510: 646c 6c00 0001 1323 b4c1 00c0 0000 1ba0  dll....#........
-00003520: 2960 956b a743 ac84 0f10 eb5c face 5379  )`.k.C.....\..Sy
-00003530: 7374 656d 2e54 6872 6561 6469 6e67 2e43  stem.Threading.C
-00003540: 6861 6e6e 656c 732e 646c 6c00 0001 6be2  hannels.dll...k.
-00003550: 928f 0080 0000 4305 a14c ac11 ab4e ae5c  ......C..L...N.\
-00003560: ca46 dd26 a9e6 5379 7374 656d 2e54 6872  .F.&..System.Thr
-00003570: 6561 6469 6e67 2e64 6c6c 0000 0197 d865  eading.dll.....e
-00003580: 8200 c000 0035 1795 6273 5bfb 46af 9cc3  .....5..bs[.F...
-00003590: 2ca0 4bcd a453 7973 7465 6d2e 5468 7265  ,.K..System.Thre
-000035a0: 6164 696e 672e 4f76 6572 6c61 7070 6564  ading.Overlapped
-000035b0: 2e64 6c6c 0000 013c fbd5 d900 8000 00a3  .dll...<........
-000035c0: 0026 d46e 86bc 4a97 ebb4 9f7a 3773 1753  .&.n..J....z7s.S
-000035d0: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
-000035e0: 5461 736b 732e 4461 7461 666c 6f77 2e64  Tasks.Dataflow.d
-000035f0: 6c6c 0000 0119 279e b500 c000 009a 4a2d  ll....'.......J-
-00003600: 0eda 8f0d 4199 7be5 6190 1d7c e153 7973  ....A.{.a..|.Sys
-00003610: 7465 6d2e 5468 7265 6164 696e 672e 5461  tem.Threading.Ta
-00003620: 736b 732e 646c 6c00 0001 e3a4 32e0 0080  sks.dll.....2...
-00003630: 0000 179d 784b fdf0 4d46 87dc 01bb c363  ....xK..MF.....c
-00003640: 31fd 5379 7374 656d 2e54 6872 6561 6469  1.System.Threadi
-00003650: 6e67 2e54 6173 6b73 2e45 7874 656e 7369  ng.Tasks.Extensi
-00003660: 6f6e 732e 646c 6c00 0001 ee59 d0d5 0080  ons.dll....Y....
-00003670: 0000 7b13 3b46 bbe3 9c48 9308 43cd 6617  ..{.;F...H..C.f.
-00003680: e6f8 5379 7374 656d 2e54 6872 6561 6469  ..System.Threadi
-00003690: 6e67 2e54 6173 6b73 2e50 6172 616c 6c65  ng.Tasks.Paralle
-000036a0: 6c2e 646c 6c00 0001 e998 df97 0080 0000  l.dll...........
-000036b0: 6370 2f5c 6b8b 0541 9479 1401 6a08 bc3d  cp/\k..A.y..j..=
-000036c0: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
-000036d0: 2e54 6872 6561 642e 646c 6c00 0001 e96c  .Thread.dll....l
-000036e0: 3b91 00a0 0000 2a55 b25c 791b ff4d 9f6f  ;.....*U.\y..M.o
-000036f0: 7dca 7567 1cbd 5379 7374 656d 2e54 6872  }.ug..System.Thr
-00003700: 6561 6469 6e67 2e54 6872 6561 6450 6f6f  eading.ThreadPoo
-00003710: 6c2e 646c 6c00 0001 26ea 10aa 0080 0000  l.dll...&.......
-00003720: cfea 1d32 0968 cd49 bce1 66d4 5ec3 1288  ...2.h.I..f.^...
-00003730: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
-00003740: 2e54 696d 6572 2e64 6c6c 0000 0166 78db  .Timer.dll...fx.
-00003750: fc00 8000 0053 b37f 4868 def6 40b8 3618  .....S..Hh..@.6.
-00003760: 4e3f 80a1 0253 7973 7465 6d2e 5472 616e  N?...System.Tran
-00003770: 7361 6374 696f 6e73 2e64 6c6c 0000 0164  sactions.dll...d
-00003780: 2dbe c700 8000 0022 4b04 e04c df5e 41a6  -......"K..L.^A.
-00003790: 8f4d 24a6 62cc d253 7973 7465 6d2e 5472  .M$.b..System.Tr
-000037a0: 616e 7361 6374 696f 6e73 2e4c 6f63 616c  ansactions.Local
-000037b0: 2e64 6c6c 0000 01b8 414f ee00 a000 006e  .dll....AO.....n
-000037c0: a9ce 8dc7 1944 41b3 1d87 316a fda6 6f53  .....DA...1j..oS
-000037d0: 7973 7465 6d2e 5661 6c75 6554 7570 6c65  ystem.ValueTuple
-000037e0: 2e64 6c6c 0000 01a3 152f 8000 8000 004d  .dll...../.....M
-000037f0: f2c8 7b43 cd7b 4db0 e77f 204b c891 0853  ..{C.{M... K...S
-00003800: 7973 7465 6d2e 5765 622e 646c 6c00 0001  ystem.Web.dll...
-00003810: 9f91 73ea 0080 0000 ab94 35b9 5d34 d14e  ..s.......5.]4.N
-00003820: a755 5b39 d1a0 2a83 5379 7374 656d 2e57  .U[9..*.System.W
-00003830: 6562 2e48 7474 7055 7469 6c69 7479 2e64  eb.HttpUtility.d
-00003840: 6c6c 0000 01ae d716 c700 8000 0096 fa45  ll.............E
-00003850: c2bf 5af2 4ca1 11b1 d4e2 b183 a253 7973  ..Z.L........Sys
-00003860: 7465 6d2e 5769 6e64 6f77 732e 646c 6c00  tem.Windows.dll.
-00003870: 0001 f53b 40a8 0080 0000 a898 c72c 168e  ...;@........,..
-00003880: 3c40 8189 166b 81e3 23a4 5379 7374 656d  <@...k..#.System
-00003890: 2e58 6d6c 2e64 6c6c 0000 016d 48c0 d300  .Xml.dll...mH...
-000038a0: a000 00d6 3405 ed6e 2980 44a8 639d cf21  ....4..n).D.c..!
-000038b0: ad74 b253 7973 7465 6d2e 586d 6c2e 4c69  .t.System.Xml.Li
-000038c0: 6e71 2e64 6c6c 0000 0137 abde 8900 8000  nq.dll...7......
-000038d0: 00f1 b2f0 6422 622a 46ad 799e 2880 89c2  ....d"b*F.y.(...
-000038e0: 9053 7973 7465 6d2e 586d 6c2e 5265 6164  .System.Xml.Read
-000038f0: 6572 5772 6974 6572 2e64 6c6c 0000 019f  erWriter.dll....
-00003900: aa14 b900 0002 000b b1ae 0c7d b5a1 438b  ...........}..C.
-00003910: 7fb0 b97f a0f8 1253 7973 7465 6d2e 586d  .......System.Xm
-00003920: 6c2e 5365 7269 616c 697a 6174 696f 6e2e  l.Serialization.
-00003930: 646c 6c00 0001 b24c c599 0080 0000 e657  dll....L.......W
-00003940: 988f 3e36 1a4d 8205 1b27 86b6 9f2b 5379  ..>6.M...'...+Sy
-00003950: 7374 656d 2e58 6d6c 2e58 446f 6375 6d65  stem.Xml.XDocume
-00003960: 6e74 2e64 6c6c 0000 014b a5fd e400 c000  nt.dll...K......
-00003970: 00a9 1635 2d3d 9962 4ca5 b32c 50b3 e98b  ...5-=.bL..,P...
-00003980: 4153 7973 7465 6d2e 586d 6c2e 586d 6c44  ASystem.Xml.XmlD
-00003990: 6f63 756d 656e 742e 646c 6c00 0001 8d94  ocument.dll.....
-000039a0: 85ab 0080 0000 8754 a5b6 c593 4f41 87a9  .......T....OA..
-000039b0: d8bd c426 cd27 5379 7374 656d 2e58 6d6c  ...&.'System.Xml
-000039c0: 2e58 6d6c 5365 7269 616c 697a 6572 2e64  .XmlSerializer.d
-000039d0: 6c6c 0000 0161 b7ce b300 0001 0081 d2c2  ll...a..........
-000039e0: 5c5b fca9 4fa7 e666 09e7 8541 1953 7973  \[..O..f...A.Sys
-000039f0: 7465 6d2e 586d 6c2e 5850 6174 682e 646c  tem.Xml.XPath.dl
-00003a00: 6c00 0001 c7d3 4fe3 0080 0000 2cdd d1db  l.....O.....,...
-00003a10: f37e 264c 8b7d 4202 62c5 b5b4 5379 7374  .~&L.}B.b...Syst
-00003a20: 656d 2e58 6d6c 2e58 5061 7468 2e58 446f  em.Xml.XPath.XDo
-00003a30: 6375 6d65 6e74 2e64 6c6c 0000 01cd 16d7  cument.dll......
-00003a40: b500 8000 0015 bcdd b47a 2ff7 4f95 34d4  .........z/.O.4.
-00003a50: 3666 d37b ca55 6e64 6572 7461 6c65 4d6f  6f.{.UndertaleMo
-00003a60: 644c 6962 2e64 6c6c 0000 01a1 15a1 9700  dLib.dll........
-00003a70: 2003 0036 517c c8db 8c83 4682 a40e 21d6   ..6Q|....F...!.
-00003a80: 85cf 3457 696e 646f 7773 4261 7365 2e64  ..4WindowsBase.d
-00003a90: 6c6c 0000 010a 1cbf 8600 8000 0034 aea9  ll...........4..
-00003aa0: 4936 2c5a 4d81 7e2b 0185 bd74 ca15 0100  I6,ZM.~+...t....
-00003ab0: 0046 0f09 1000 1502 0003 000a 002c 0600  .F...........,..
-00003ac0: 3d04 5514 5369 784c 6162 6f72 732e 496d  =.U.SixLabors.Im
-00003ad0: 6167 6553 6861 7270 2153 6978 4c61 626f  ageSharp!SixLabo
-00003ae0: 7273 2e49 6d61 6765 5368 6172 702e 5069  rs.ImageSharp.Pi
-00003af0: 7865 6c46 6f72 6d61 7473 1f53 6978 4c61  xelFormats.SixLa
-00003b00: 626f 7273 2e49 6d61 6765 5368 6172 702e  bors.ImageSharp.
-00003b10: 5072 6f63 6573 7369 6e67 0653 7973 7465  Processing.Syste
-00003b20: 6d1a 5379 7374 656d 2e43 6f6c 6c65 6374  m.System.Collect
-00003b30: 696f 6e73 2e47 656e 6572 6963 0953 7973  ions.Generic.Sys
-00003b40: 7465 6d2e 494f 0b53 7973 7465 6d2e 4c69  tem.IO.System.Li
-00003b50: 6e71 0f53 7973 7465 6d2e 4e65 742e 4874  nq.System.Net.Ht
-00003b60: 7470 1053 7973 7465 6d2e 5468 7265 6164  tp.System.Thread
-00003b70: 696e 6716 5379 7374 656d 2e54 6872 6561  ing.System.Threa
-00003b80: 6469 6e67 2e54 6173 6b73 1453 7973 7465  ding.Tasks.Syste
-00003b90: 6d2e 476c 6f62 616c 697a 6174 696f 6e11  m.Globalization.
-00003ba0: 5379 7374 656d 2e52 6566 6c65 6374 696f  System.Reflectio
-00003bb0: 6e10 5379 7374 656d 2e54 6578 742e 4a73  n.System.Text.Js
-00003bc0: 6f6e 0f55 6e64 6572 7461 6c65 4d6f 644c  on.UndertaleModL
-00003bd0: 6962 1a55 6e64 6572 7461 6c65 4d6f 644c  ib.UndertaleModL
-00003be0: 6962 2e44 6563 6f6d 7069 6c65 7216 556e  ib.Decompiler.Un
-00003bf0: 6465 7274 616c 654d 6f64 4c69 622e 4d6f  dertaleModLib.Mo
-00003c00: 6465 6c73 2053 6978 4c61 626f 7273 2e49  dels SixLabors.I
-00003c10: 6d61 6765 5368 6172 702e 466f 726d 6174  mageSharp.Format
-00003c20: 732e 506e 6733 01a7 9701 a7ac 01a7 ce01  s.Png3..........
-00003c30: a7ee 01a7 f501 a810 01a8 1a01 a826 01a8  .............&..
-00003c40: 3601 a847 01a8 5e01 a873 01a8 8501 a896  6..G..^..s......
-00003c50: 01a8 a601 a8c1 01a8 d894 d602 0000 0006  ................
-00003c60: 003a 2009 0a00 5404 000d 0021 1600 0b00  .: ...T....!....
-00003c70: 3104 0e0d 001e 047b 1000 0102 7902 0000  1......{....y...
-00003c80: 0b00 0001 0041 0200 1200 4b80 8a00 0b00  .....A....K.....
-00003c90: 1104 0007 000d 0026 0700 1600 1e07 0045  .......&.......E
-00003ca0: 023d 1500 3302 000b 0049 0200 2000 2b02  .=..3....I.. .+.
-00003cb0: 0016 0063 5400 1f00 1b02 0e07 002c 047b  ...cT........,.{
-00003cc0: 1200 6202 001d 0001 0279 0200 000b 0000  ..b......y......
-00003cd0: 0100 0007 004a 0808 2700 4c02 0027 0080  .....J..'.L..'..
-00003ce0: 8602 0019 003d 0200 2200 4802 0022 0064  .....=..".H..".d
-00003cf0: 0200 1400 1b02 0e07 0029 047b 0e00 3902  .........).{..9.
-00003d00: 001d 0001 0279 0200 000b 0000 0100 4c04  .....y........L.
-00003d10: 0027 004e 0200 2700 808b 0200 1900 3f02  .'.N..'.......?.
-00003d20: 0022 004a 0200 2200 6802 0014 001b 020e  .".J..".h.......
-00003d30: 0700 2a04 7b0e 003a 0200 1d00 0102 7902  ..*.{..:......y.
-00003d40: 0000 0b00 0001 0072 0679 3b00 7802 003b  .......r.y;.x..;
-00003d50: 0078 0200 3b00 7e02 003b 006b 0200 3b00  .x..;.~..;.k..;.
-00003d60: 80a6 0200 5600 80a6 0200 5600 80a6 0200  ....V.....V.....
-00003d70: 5600 80a6 0200 5600 80a6 0200 5600 80a6  V.....V.....V...
-00003d80: 0200 5600 80a6 0200 5600 80ae 0400 5600  ..V.....V.....V.
-00003d90: 80bc 0200 5600 80b4 0200 5600 80b2 0200  ....V.....V.....
-00003da0: 5600 809d 0600 4b00 809f 0200 4b00 8099  V.....K.....K...
-00003db0: 0200 4b00 7506 0046 0078 0200 4600 7602  ..K.u..F.x..F.v.
-00003dc0: 0046 0076 0200 4600 7702 0046 0080 a206  .F.v..F.w..F....
-00003dd0: 004b 0080 a002 004b 0080 a202 004b 0080  .K.....K.....K..
-00003de0: a202 004b 0080 9f02 004b 0080 9c02 004b  ...K.....K.....K
-00003df0: 0080 9e02 004b 0080 9d02 004b 0080 a402  .....K.....K....
-00003e00: 004b 0080 9e02 004b 0080 a002 004b 0080  .K.....K.....K..
-00003e10: a002 004b 0080 9e02 004b 0080 9e02 004b  ...K.....K.....K
-00003e20: 0080 9f02 004b 0080 9d02 004b 0080 a402  .....K.....K....
-00003e30: 004b 0080 9d02 004b 0080 9d02 004b 0080  .K.....K.....K..
-00003e40: 9d02 004b 0032 0600 2000 8099 0200 4b00  ...K.2.. .....K.
-00003e50: 8099 0200 4b00 8099 0200 4b00 8099 0200  ....K.....K.....
-00003e60: 4b00 8099 0200 4b00 8099 0200 4b00 8099  K.....K.....K...
-00003e70: 0200 4b00 8099 0200 4b00 8099 0200 4b0b  ..K.....K.....K.
-00003e80: 0604 0081 450b 061a 0081 370e 061a 0082  ....E.....7.....
-00003e90: 0f18 0620 0084 2b0b 0634 0081 450b 061a  ... ..+..4..E...
-00003ea0: 0081 4500 391a 0020 0080 a602 004b 0080  ..E.9.. .....K..
-00003eb0: a602 004b 0080 a602 004b 0080 a602 004b  ...K.....K.....K
-00003ec0: 0039 0400 2000 80a6 0200 4b00 80a6 0200  .9.. .....K.....
-00003ed0: 4b00 80a6 0200 4b00 80a6 0200 4b00 80a6  K.....K.....K...
-00003ee0: 0200 4b00 80a6 0200 4b00 80a6 0200 4b00  ..K.....K.....K.
-00003ef0: 80a6 0200 4b00 80a6 0200 4b00 80a7 0200  ....K.....K.....
-00003f00: 4b00 80a7 0200 4b00 80a7 0200 4b00 80a7  K.....K.....K...
-00003f10: 0200 4b00 80a7 0200 4b00 80a7 0200 4b00  ..K.....K.....K.
-00003f20: 80a7 0200 4b0a 0604 0081 1637 0618 008a  ....K......7....
-00003f30: 9612 0672 0082 e712 0628 0082 e712 0628  ...r.....(.....(
-00003f40: 0082 e70f 0628 0082 450a 0624 0081 4705  .....(..E..$..G.
-00003f50: 0480 8400 4500 790c 0021 0056 0200 0c00  ....E.y..!.V....
-00003f60: 2502 0011 0037 0200 0c00 4002 0007 0031  %....7....@....1
-00003f70: 0200 0800 3902 0007 0024 0200 0800 3402  ....9....$....4.
-00003f80: 000e 0030 0200 0700 7502 0022 0075 0200  ...0....u..".u..
-00003f90: 0d00 2302 0012 0035 0200 0c00 3c02 0007  ..#....5....<...
-00003fa0: 002f 0200 0900 3502 0007 0024 0200 0800  ./....5....$....
-00003fb0: 3402 000e 002e 0200 0700 2702 0011 004d  4.........'....M
-00003fc0: 0400 1800 3406 001c 0035 0200 1d00 4f06  ....4....5....O.
-00003fd0: 0018 0057 0200 1301 80d2 0200 2700 4808  ...W........'.H.
-00003fe0: 0018 005f 0200 0d00 5902 0021 0056 0600  ..._....Y..!.V..
-00003ff0: 2100 8090 0600 2702 80a6 0600 2700 809e  !.....'.....'...
-00004000: 0a00 2700 3c06 0018 0080 8a02 0013 0080  ..'.<...........
-00004010: 8202 0013 0080 8402 0013 007f 0200 1300  ................
-00004020: 5e02 2a2a 0000 0200 0800 6907 0048 0477  ^.**......i..H.w
-00004030: 2400 4802 0024 0000 0600 027b 1c08 0180  $.H..$.....{....
-00004040: 9a0e 5d27 0068 0600 2700 5906 0021 0080  ..]'.h..'.Y..!..
-00004050: 8502 0027 0074 0600 2100 7402 0021 0074  ...'.t..!.t..!.t
-00004060: 0200 2100 7402 0021 004c 0632 1b00 0002  ..!.t..!.L.2....
-00004070: 000c 0061 0700 3d02 771e 0000 0600 027f  ...a..=.w.......
-00004080: 2408 002d 0855 1200 6802 0827 0180 da06  $..-.U..h..'....
-00004090: 7921 0069 0400 2100 7706 0027 007e 0200  y!.i..!.w..'.~..
-000040a0: 2700 7502 0027 0363 0632 6600 0002 000c  '.u..'.c.2f.....
-000040b0: 0061 0700 3408 771e 0000 0600 0279 2408  .a..4.w......y$.
-000040c0: 0080 900a 5521 0380 e406 0027 0072 0e00  ....U!.....'.r..
-000040d0: 2700 2d02 0007 0057 0200 1c02 6e02 000d  '.-....W....n...
-000040e0: 0024 0600 1200 4502 0021 003a 0200 0700  .$....E..!.:....
-000040f0: 2a02 0009 0033 0200 0700 2002 000c 0028  *....3.... ....(
-00004100: 0200 0e00 2402 0007 0680 8808 0007 0080  ....$...........
-00004110: 8e10 322b 0000 0200 0c00 6107 0054 0277  ..2+......a..T.w
-00004120: 2100 0006 0002 7f24 0800 290a 5507 005b  !......$..).U..[
-00004130: 022e 1700 0002 000a 0065 0700 2e04 770f  .........e....w.
-00004140: 0031 0208 2f00 0006 0002 7b18 0804 8090  .1../.....{.....
-00004150: 0a59 3304 8086 0a00 3300 250c 0007 001b  .Y3.....3.%.....
-00004160: 022e 1b00 0002 000a 0065 0700 2e04 770f  .........e....w.
-00004170: 002d 0208 2f00 0006 0002 7b18 0804 8088  .-../.....{.....
-00004180: 0a59 3304 7e0a 0033 0061 1400 2700 4f06  .Y3.~..3.a..'.O.
-00004190: 0021 0055 0632 1b00 0002 000c 0061 0700  .!.U.2.......a..
-000041a0: 7c02 7724 0000 0600 027f 2408 0071 0c55  |.w$......$..q.U
-000041b0: 2200 7402 0022 0021 0200 1200 2202 0012  ".t..".!...."...
-000041c0: 0906 0200 7a09 0614 007d 0078 1800 2200  ....z....}.x..".
-000041d0: 2402 0012 002f 0200 1609 0602 0065 0043  $..../.......e.C
-000041e0: 1600 2c00 1002 0009 0036 0200 1800 2c02  ..,......6....,.
-000041f0: 0009 0017 0200 0900 1602 0009 003f 0400  .............?..
-00004200: 2c00 1002 0009 002c 0200 0900 1702 0009  ,......,........
-00004210: 0016 0200 0900 3f04 002c 0010 0200 0900  ......?..,......
-00004220: 2c02 0009 0017 0200 0900 1602 0009 003f  ,..............?
-00004230: 0400 2c00 1002 0009 002c 0200 0900 1702  ..,......,......
-00004240: 0009 0015 0200 080a 0404 0065 001d 1600  ...........e....
-00004250: 0d0a 0404 0065 001d 1600 0d0a 0404 0062  .....e.........b
-00004260: 001d 1600 0d0a 0404 0061 001d 1600 0c00  .........a......
-00004270: 3506 0018 000b 020a 0700 0005 0023 047f  5............#..
-00004280: 0700 3502 0028 001a 0200 0900 2104 0007  ..5..(......!...
-00004290: 004d 0200 4900 4402 001e 0018 0200 1200  .M..I.D.........
-000042a0: 2302 000d 0033 0200 0700 1702 0009 002d  #....3.........-
-000042b0: 0200 0700 1b02 000e 001c 0200 0700 2404  ..............$.
-000042c0: 0007 0055 0200 4900 1b02 0012 0026 0200  ...U..I......&..
-000042d0: 0d00 2f02 0007 001a 0200 0900 2902 0007  ../.........)...
-000042e0: 001a 0200 0c00 1b02 000e 001f 0200 0700  ................
-000042f0: 1b02 0012 0003 4b30 0600 0800 6d0c 0e12  ......K0....m...
-00004300: 3e5d 1300 501e 0027 0050 0200 2700 2606  >]..P..'.P..'.&.
-00004310: 0007 0048 0200 1c5d 1202 000d 001d 80bc  ...H...]........
-00004320: 0012 0071 0200 3801 817a 0600 1301 817a  ...q..8..z.....z
-00004330: 0400 1300 80aa 082a 3300 0002 0008 0069  .......*3......i
-00004340: 0700 3c02 7724 0000 0600 027f 1c08 0080  ..<.w$..........
-00004350: ef08 0c3b 0000 0200 0b00 6307 0063 0277  ...;......c..c.w
-00004360: 2400 0006 0002 7f22 0800 3c08 5718 0043  $......"..<.W..C
-00004370: 0200 1300 4802 0013 0080 9302 0027 0080  ....H........'..
-00004380: 9302 0027 0168 0200 2700 5404 0018 0072  ...'.h..'.T....r
-00004390: 0200 1300 7002 0013 0080 8902 0013 0080  ....p...........
-000043a0: af02 0013 0080 8d02 0013 006e 0200 2700  ...........n..'.
-000043b0: 2106 0010 0036 0608 1800 4b02 0018 004b  !....6....K....K
-000043c0: 0200 1800 4902 0018 004a 0200 1800 3d02  ....I....J....=.
-000043d0: 0018 0037 0200 1800 3f02 0018 005c 0200  ...7....?....\..
-000043e0: 3100 5502 0031 0056 0200 3200 5502 0031  1.U..1.V..2.U..1
-000043f0: 0055 0200 3100 5602 0032 0056 0200 3200  .U..1.V..2.V..2.
-00004400: 5602 0032 0056 0200 2e00 5204 002b 0049  V..2.V....R..+.I
-00004410: 0200 2b00 5202 002b 0072 0400 2200 6602  ..+.R..+.r..".f.
-00004420: 000d 0021 0200 1200 5902 002c 0069 0200  ...!....Y..,.i..
-00004430: 1200 3306 0018 0060 0200 3100 5802 0030  ..3....`..1.X..0
-00004440: 005a 0200 3200 5902 0031 005a 0200 3200  .Z..2.Y..1.Z..2.
-00004450: 5902 0031 005a 0200 3200 5a02 0032 004f  Y..1.Z..2.Z..2.O
-00004460: 0600 2b00 4602 002b 004f 0200 2b00 4604  ..+.F..+.O..+.F.
-00004470: 0012 006f 0400 2200 6402 000d 001e 0200  ...o..".d.......
-00004480: 1200 5302 002c 005d 0600 3200 3508 0018  ..S..,.]..2.5...
-00004490: 005d 0200 2e00 5602 002e 0057 0200 2f00  .]....V....W../.
-000044a0: 5702 002e 0056 0200 2e00 5702 002f 0057  W....V....W../.W
-000044b0: 0200 2f00 5802 002f 0057 0800 3800 5602  ../.X../.W..8.V.
-000044c0: 0038 005e 0200 3200 5004 0028 0047 0200  .8.^..2.P..(.G..
-000044d0: 2800 5002 0028 0049 0400 1200 7104 0022  (.P..(.I....q.."
-000044e0: 0066 0200 0d00 2002 0012 0056 0200 2900  .f.... ....V..).
-000044f0: 3906 0018 0062 0200 3100 5a02 0030 005c  9....b..1.Z..0.\
-00004500: 0200 3200 5b02 0031 005c 0200 3200 5b02  ..2.[..1.\..2.[.
-00004510: 0031 005c 0200 3200 5c02 0032 005f 0800  .1.\..2.\..2._..
-00004520: 3800 5f02 0038 005f 0200 3800 5f02 0038  8._..8._..8._..8
-00004530: 006f 0200 4500 5504 002b 004c 0200 2b00  .o..E.U..+.L..+.
-00004540: 5502 002b 0075 0400 2200 6802 000d 0024  U..+.u..".h....$
-00004550: 0200 1200 5f02 002c 004a 0400 1200 8089  ...._..,.J......
-00004560: 0600 2700 8089 0200 2700 8087 0200 2700  ..'.....'.....'.
-00004570: 8089 0200 2701 816c 1e79 2701 816c 0400  ....'..l.y'..l..
-00004580: 2701 816c 0400 2701 816c 0400 2700 80ba  '..l..'..l..'...
-00004590: 0800 2100 3006 0016 002e 0200 0700 1002  ..!.0...........
-000045a0: 0009 0010 0200 0900 1402 000c 0014 0200  ................
-000045b0: 0c00 3302 0025 0041 0200 1d00 2702 0007  ..3..%.A....'...
-000045c0: 0056 0200 1c00 6f02 000d 001e 0200 1200  .V....o.........
-000045d0: 2502 0009 0023 0200 0d0b 0602 0080 8a0b  %....#..........
-000045e0: 0618 0080 8c00 7c1c 0027 0280 9806 004d  ......|..'.....M
-000045f0: 003f 0a00 1800 6302 0013 0070 0600 1300  .?....c....p....
-00004600: 5c06 0027 005c 0200 2701 8094 0600 2701  \..'.\..'.....'.
-00004610: 812c 0e00 0d00 6d0c 0013 0080 8102 0013  .,....m.........
-00004620: 0055 0200 1300 6a02 0013 004f 0200 1300  .U....j....O....
-00004630: 6102 0013 0068 0200 1300 4606 0018 0281  a....h....F.....
-00004640: 5602 0013 0041 0600 1800 6902 0013 087b  V....A....i....{
-00004650: 0800 1308 7b12 0013 087b 1600 1308 7b12  ....{....{....{.
-00004660: 0013 087b 1600 1308 7b12 0013 0047 1600  ...{....{....G..
-00004670: 1800 8096 0200 1300 80b5 0200 1309 1206  ................
-00004680: 0013 005a 1400 1301 80e8 0e00 0d00 3c08  ...Z..........<.
-00004690: 000d 006b 0600 0d00 8080 0600 2600 8084  ...k........&...
-000046a0: 0200 2c01 8104 0600 0d01 80ce 0800 0d00  ..,.............
-000046b0: 5904 0018 087b 0200 1300 7912 0013 0063  Y....{....y....c
-000046c0: 0400 1808 7b02 0013 0080 8312 0013 0059  ....{..........Y
-000046d0: 0400 1808 7b02 0013 0079 1200 1300 5a04  ....{....y....Z.
-000046e0: 0018 087b 0200 1300 7612 0013 0281 4c06  ...{....v.....L.
-000046f0: 000d 1e1a 0a00 1301 8100 3e00 1300 7b08  ..........>...{.
-00004700: 0027 004f 0600 1800 4f02 0013 004e 0200  .'.O....O....N..
-00004710: 1800 4802 0013 036b 0428 4b00 0002 0008  ..H....k.(K.....
-00004720: 0069 0700 5008 7924 0000 0600 0279 1a08  .i..P.y$.....y..
-00004730: 003e 0a5f 1c00 0c02 3e12 0000 0200 1200  .>._....>.......
-00004740: 5507 0060 0446 3200 0002 001b 0043 0900  U..`.F2......C..
-00004750: 4d02 7718 0002 7f42 0b00 000b 0000 0100  M.w....B........
-00004760: 027d 670b 0000 0b00 0001 004c 1049 1300  .}g........L.I..
-00004770: 5302 0013 004d 0600 1300 5402 0013 0180  S....M....T.....
-00004780: 8402 3e36 0000 0200 1200 5509 0041 0477  ..>6......U..A.w
-00004790: 1300 027d 300b 0000 0b00 0001 004b 0a49  ...}0........K.I
-000047a0: 1300 5202 0013 0076 0200 2700 5006 0018  ..R....v..'.P...
-000047b0: 004a 0200 1300 5002 0013 0181 3a02 2836  .J....P.....:.(6
-000047c0: 0000 0200 0800 6909 003d 0479 1300 027d  ......i..=.y...}
-000047d0: 1a0b 0000 0b00 0001 004f 0a5f 1800 4902  .........O._..I.
-000047e0: 0013 004f 0200 1300 8088 0228 2b00 0002  ...O.......(+...
-000047f0: 0008 0069 0700 5002 7924 0000 0600 027f  ...i..P.y$......
-00004800: 1a08 004d 085f 1300 5302 0013 0280 9602  ...M._..S.......
-00004810: 2836 0000 0200 0800 6909 0046 0679 1300  (6......i..F.y..
-00004820: 027b 1a0b 0000 0b00 0001 0050 0c5f 1300  .{.........P._..
-00004830: 5602 0013 0180 d602 2836 0000 0200 0800  V.......(6......
-00004840: 6909 0049 0479 1300 027d 1a0b 0000 0b00  i..I.y...}......
-00004850: 0001 004e 0c5f 1300 5502 0013 056b 0228  ...N._..U....k.(
-00004860: 809c 0000 0200 0800 6907 0056 0c79 2400  ........i..V.y$.
-00004870: 0006 0002 751a 0800 4b14 5f13 0051 0200  ....u...K._..Q..
-00004880: 1304 6b04 2880 8a00 0002 0008 0069 0700  ..k.(........i..
-00004890: 520a 7924 0000 0600 0277 1a08 004a 105f  R.y$.....w...J._
-000048a0: 1800 4802 0013 0050 0200 1300 4806 0013  ..H....P....H...
-000048b0: 0050 0200 1300 8089 0228 2b00 0002 0008  .P.......(+.....
-000048c0: 0069 0700 5702 7924 0000 0600 027f 1a08  .i..W.y$........
-000048d0: 0048 085f 1300 5002 0013 0048 0600 1300  .H._..P....H....
-000048e0: 5002 0013 0048 0600 1300 5002 0013 081a  P....H....P.....
-000048f0: 0600 1308 1a12 0013 081a 1200 1312 1a12  ................
-00004900: 0013 0812 2800 1300 7e16 0061 0067 0600  ....(...~..a.g..
-00004910: 2700 6602 0021 0060 0200 2100 3a06 2a36  '.f..!.`..!.:.*6
-00004920: 0000 0200 0800 6909 0041 0277 1200 027f  ......i..A.w....
-00004930: 1c0b 0000 0b00 0001 0040 085d 0d00 4302  .........@.]..C.
-00004940: 0018 0480 ca02 0013 1012 0e00 2100 6f22  ............!.o"
-00004950: 0027 0712 0200 2127 1210 0027 0712 5000  .'....!'...'..P.
-00004960: 2100 6810 0021 0812 0200 2100 2a16 0007  !.h..!....!.*...
-00004970: 0052 0200 1c2d 1202 000d 0021 5c00 1200  .R...-.....!\...
-00004980: 7b02 0038 002a 0400 0700 5202 001c 2612  {..8.*....R...&.
-00004990: 0200 0d00 214e 0012 007a 0200 3800 3804  ....!N...z..8.8.
-000049a0: 0018 0080 8102 0013 002e 0200 1300 3802  ..............8.
-000049b0: 0013 0038 0400 1800 2e02 0013 0075 0200  ...8.........u..
-000049c0: 1300 7202 0013 0d1a 0200 1300 7720 0061  ..r.........w .a
-000049d0: 0460 0200 1300 4710 0018 0035 0200 1300  .`....G....5....
-000049e0: 7c02 0013 006c 042a 2b00 0002 0008 0069  |....l.*+......i
-000049f0: 0700 3f02 7724 0000 0600 027f 1c08 0040  ..?.w$.........@
-00004a00: 085d 2500 4402 0025 0080 8006 004b 0080  .]%.D..%.....K..
-00004a10: 9d02 003d 0018 064a 0d00 0005 0018 0049  ...=...J.......I
-00004a20: 1a00 0d04 7702 0000 808e 0059 0610 4001  ....w......Y..@.
-00004a30: 80ec 0200 8086 0006 0400 0500 5d04 0040  ............]..@
-00004a40: 0006 0200 0500 5f04 0040 0006 0200 0500  ......_..@......
-00004a50: 5904 0040 0006 0200 0500 0004 0023 1a0e  Y..@.........#..
-00004a60: 1c00 4802 7313 0006 0200 0500 5d06 0040  ..H.s.......]..@
-00004a70: 0006 0200 0500 6504 0040 0006 0200 0500  ......e..@......
-00004a80: 6704 0040 0006 0200 0500 6304 0040 0006  g..@......c..@..
-00004a90: 0200 0500 5f04 0040 0006 0200 0500 5d04  ...._..@......].
-00004aa0: 0040 0006 0200 0500 6504 0040 0006 0200  .@......e..@....
-00004ab0: 0500 6b04 0040 0006 0200 0500 6904 0040  ..k..@......i..@
-00004ac0: 0006 0200 0500 6104 0040 0006 0200 0500  ......a..@......
-00004ad0: 5d0a 0040 0006 0200 0500 5d04 0040 0006  ]..@......]..@..
-00004ae0: 0200 0500 5d04 0040 0006 0200 0500 5d04  ....]..@......].
-00004af0: 0040 0006 0200 0500 5d04 0040 0006 0200  .@......]..@....
-00004b00: 0200 5d04 0040 0006 0200 0200 2808 0006  ..]..@......(...
-00004b10: 0002 bf51 2c0e 0000 0e00 7180 ba3d 1c00  ...Q,.....q..=..
-00004b20: 6002 0813 0074 0279 1c00 6202 0813 006a  `....t.y..b....j
-00004b30: 0279 1c00 5c02 0813 0080 8006 793d 007a  .y..\.......y=.z
-00004b40: 0200 3d08 1206 0027 0062 1200 2701 8172  ..=....'.b..'..r
-00004b50: 0800 270e 120a 0013 0051 1e00 2700 5102  ..'......Q..'.Q.
-00004b60: 0027 0032 0600 1800 0c02 2a12 0000 0200  .'.2......*.....
-00004b70: 0800 6907 0052 0420 3000 0002 0008 0069  ..i..R. 0......i
-00004b80: 0700 1f04 7707 0002 7d1c 0b00 000b 0000  ....w...}.......
-00004b90: 0100 027d 790b 0000 0b00 0001 0013 105d  ...}y..........]
-00004ba0: 0900 1906 0007 0014 0246 0d00 0005 0016  .........F......
-00004bb0: 004d 1c00 1304 7703 000c 022a 1200 0005  .M....w....*....
-00004bc0: 0008 0069 0900 1004 2c0e 0000 0500 0e00  ...i....,.......
-00004bd0: 5d09 0020 0477 0e00 4204 001d 0055 0208  ].. .w..B....U..
-00004be0: 3800 0d04 7903 0024 0200 0c00 7304 086e  8...y..$....s..n
-00004bf0: 0016 0200 1200 1f02 0009 1c04 0679 7900  .............yy.
-00004c00: 1704 360c 003b 0202 3900 3b02 0a39 003b  ..6..;..9.;..9.;
-00004c10: 0273 3900 2d02 020c 002d 0200 0c00 2d02  .s9.-....-....-.
-00004c20: 7d0c 002d 0204 0c00 2d02 000c 002d 027b  }..-....-....-.{
-00004c30: 0c00 2d02 020c 002d 0204 0c00 2d02 7f0c  ..-....-....-...
-00004c40: 002d 020e 0c00 2d02 7d0c 002d 0204 0c00  .-....-.}..-....
-00004c50: 2d02 000c 002d 027d 0c00 2d02 000c 002d  -....-.}..-....-
-00004c60: 0202 0900 2d02 7d09 002d 0206 0900 2d02  ....-.}..-....-.
-00004c70: 7309 002d 0200 0900 2d02 0009 005d 025f  s..-....-....]._
-00004c80: 5200 0004 0033 066f 0f00 1102 0006 0006  R....3.o........
-00004c90: 0200 0200 0223 280e 0000 0b00 0001 000a  .....#(.........
-00004ca0: 6451 0400 0600 1602 0002 1906 0e00 000b  dQ..............
-00004cb0: 0000 0100 0b6e 5d04 0043 0208 3800 020b  .....n]..C..8...
-00004cc0: 300e 0000 0e00 1880 8024 0d00 0005 0025  0........$.....%
-00004cd0: 002f 1c00 3504 7715 0043 0200 2400 1c02  ./..5.w..C..$...
-00004ce0: 0009 006a 0208 5700 3904 7925 0180 8802  ...j..W.9.y%....
-00004cf0: 0080 8e00 3c08 0025 3f04 0200 80a3 0022  ....<..%?......"
-00004d00: 0436 0c00 1f02 0c0c 0181 0002 7f0c 0024  .6.............$
-00004d10: 040c 0c01 810a 027f 0c00 2104 730c 0180  ..........!.s...
-00004d20: ec02 000c 0000 0400 2304 591c 0045 004e  ........#.Y..E.N
-00004d30: 0c00 6202 4b0c 0055 0206 0c00 6c02 040c  ..b.K..U....l...
-00004d40: 0069 0200 0c00 8085 0202 0c10 6b02 750c  .i..........k.u.
-00004d50: 007f 2208 0900 5902 0609 004d 0275 0910  .."...Y....M.u..
-00004d60: 6702 0209 0061 227f 0900 4b02 7b09 004b  g....a"...K.{..K
-00004d70: 0202 0900 4b02 0409 004b 0200 0900 4f02  ....K....K....O.
-00004d80: 0609 0014 027d 0900 4902 6322 0000 0400  .....}..I.c"....
-00004d90: 3404 6f0a 0002 bf67 560e 0000 0e07 7b80  4.o....gV.....{.
-00004da0: a223 7107 7b12 0071 077b 1200 7100 5616  .#q.{..q.{..q.V.
-00004db0: 002c 0181 2002 0876 005b 0679 2c01 812c  .,.. ..v.[.y,..,
-00004dc0: 0208 7600 5406 792c 0181 1802 0876 0712  ..v.T.y,.....v..
-00004dd0: 0a79 809b 0046 1600 0e00 4402 000d 0049  .y...F....D....I
-00004de0: 0200 0d00 5802 000e 1312 0200 80a2 0026  ....X..........&
-00004df0: 2c00 0d00 5e02 0813 004d 0222 3600 0002  ,...^....M."6...
-00004e00: 0008 0069 0900 4302 770d 0002 7f1c 0b00  ...i..C.w.......
-00004e10: 000b 0000 0100 0c06 1a12 0000 0200 1200  ................
-00004e20: 5507 0060 0446 3200 0002 001b 0043 0901  U..`.F2......C..
-00004e30: 6c02 7718 0002 7f42 0b00 000b 0000 0100  l.w....B........
-00004e40: 027d 670b 0000 0b00 0001 0150 0c49 2700  .}g........P.I'.
-00004e50: 270c 000d 0060 0208 1300 80ca 042a 4300  '....`.......*C.
-00004e60: 0002 000c 0061 0700 7702 771e 0000 0600  .....a..w.w.....
-00004e70: 027f 2408 000a 065f 0400 0002 007f 027f  ..$...._........
-00004e80: 4e00 037f 2c06 0007 006f 0600 2808 5f0d  N...,....o..(._.
-00004e90: 0051 0208 1301 3802 7927 002a 0800 0d00  .Q....8.y'.*....
-00004ea0: 6702 0813 2912 0679 2700 6858 3646 0000  g...)..y'.hX6F..
-00004eb0: 0200 0e00 5d09 0017 0677 0b03 1202 0818  ....]....w......
-00004ec0: 0017 0c79 0b00 5f02 0812 0002 6b20 0b00  ...y.._.....k ..
-00004ed0: 000b 0000 0100 681e 0646 0000 0200 0e00  ......h..F......
-00004ee0: 5d09 002d 0477 1601 4202 0818 0002 7b20  ]..-.w..B.....{ 
-00004ef0: 0b00 000b 0000 0100 6710 0646 0000 0200  ........g..F....
-00004f00: 0e00 5d09 0142 0477 1800 027d 280b 0000  ..]..B.w...}(...
-00004f10: 0b00 0001 0067 0e06 4600 0002 000e 005d  .....g..F......]
-00004f20: 0900 2e04 7716 0142 0208 1800 027b 200b  ....w..B.....{ .
-00004f30: 0000 0b00 0001 006c 0e06 4600 0002 000e  .......l..F.....
-00004f40: 005d 0900 1706 770b 0412 0208 1800 180e  .]....w.........
-00004f50: 790e 005f 0208 1200 0269 200b 0000 0b00  y.._.....i .....
-00004f60: 0001 004c 2208 1b00 0002 000f 005b 0700  ...L"........[..
-00004f70: 8087 0277 2400 0006 0002 7f2a 0801 2408  ...w$......*..$.
-00004f80: 4f27 0124 0400 2700 809b 0800 2100 2906  O'.$..'.....!.).
-00004f90: 000d 0064 0208 1300 0c02 3612 0000 0500  ...d......6.....
-00004fa0: 1200 5509 0010 041c 0e00 0005 0006 006d  ..U............m
-00004fb0: 0900 5a06 7731 001c 0400 0c00 8088 0408  ..Z.w1..........
-00004fc0: 6700 1602 0012 0017 0200 0900 5204 7912  g...........R.y.
-00004fd0: 0002 6b18 0e00 000b 0000 0100 027d 100e  ..k..........}..
-00004fe0: 0000 0b00 0001 005d 2649 2700 5f02 0027  .......]&I'._..'
-00004ff0: 0029 0600 0d00 5d02 0813 1412 0279 2707  .)....]......y'.
-00005000: 1a2c 0027 0080 af12 0027 0080 af02 0027  .,.'.....'.....'
-00005010: 0180 ce0a 0021 0025 0800 0d00 5c04 0813  .....!.%....\...
-00005020: 0061 0879 2100 4d04 000d 0b12 0400 2100  .a.y!.M.......!.
-00005030: 4f1a 000d 004f 0400 0d00 4f04 000d 1912  O....O....O.....
-00005040: 0400 2100 5336 000d 0081 3b04 0021 0081  ..!.S6....;..!..
-00005050: 3804 0021 005d 0400 2100 1614 520d 0000  8..!.]..!...R...
-00005060: 0200 1c00 411a 0020 0477 0700 2802 0009  ....A.. .w..(...
-00005070: 002f 0400 1500 4602 001e 0002 7544 0b00  ./....F.....uD..
-00005080: 000e 0080 9014 3557 0512 0600 7800 691a  ......5W....x.i.
-00005090: 0027 0080 a804 0027 0080 ae04 0038 0080  .'.....'.....8..
-000050a0: 8f04 0027 005f 0a00 2700 5f02 0027 1412  ...'._..'._..'..
-000050b0: 0400 2106 122c 0027 0712 1000 2704 1212  ..!..,.'....'...
-000050c0: 0027 0612 0c00 271d 120e 0027 1712 3e00  .'....'....'..>.
-000050d0: 85f4 005c 3600 3b00 6f02 0021 005c 0400  ...\6.;.o..!.\..
-000050e0: 3e00 6f02 0021 005c 0400 3b00 6f02 0021  >.o..!.\..;.o..!
-000050f0: 005c 0400 3e00 6f02 0021 005b 0400 3b00  .\..>.o..!.[..;.
-00005100: 6e02 0021 005c 0400 3e00 6f02 0021 005c  n..!.\..>.o..!.\
-00005110: 0400 3e00 6f02 0021 0038 0e0e 0d00 3104  ..>.o..!.8....1.
-00005120: 7b28 0001 0279 0200 000b 0000 0100 0102  {(...y..........
-00005130: 7905 0980 1a06 0005 0981 1a06 0005 0982  y...............
-00005140: 1a06 0005 0800 0400 0006 0000 0035 1505  .............5..
-00005150: 1500 0000 5f17 050b 0059 0800 0b00 5108  ...._....Y....Q.
-00005160: 000b 004f 1000 2553 7973 7465 6d2e 436f  ...O..%System.Co
-00005170: 6d70 6f6e 656e 744d 6f64 656c 2e44 6174  mponentModel.Dat
-00005180: 6141 6e6e 6f74 6174 696f 6e73 1c53 7973  aAnnotations.Sys
-00005190: 7465 6d2e 5275 6e74 696d 652e 5365 7269  tem.Runtime.Seri
-000051a0: 616c 697a 6174 696f 6e1e 5379 7374 656d  alization.System
-000051b0: 2e54 6578 742e 4a73 6f6e 2e53 6572 6961  .Text.Json.Seria
-000051c0: 6c69 7a61 7469 6f6e 2a01 a797 01a7 ac01  lization*.......
-000051d0: a7ce 01a7 ee01 a7f5 01a8 1001 a81a 01a8  ................
-000051e0: 2601 a836 01a8 4701 be3a 01be 6001 a885  &..6..G..:..`...
-000051f0: 01be 7d0c 0000 0018 80ac 050b 001c 0800  ..}.............
-00005200: 0700 0000 2481 7805 0c00 0000 2681 8205  ....$.x.....&...
-00005210: 0b00 3208 0007 0000 001f 818d 0507 0000  ..2.............
-00005220: 0018 8346 3207 0000 0018 834d 2e07 0000  ...F2......M....
-00005230: 0018 8353 2e07 0000 0018 8359 2e07 0000  ...S.......Y....
-00005240: 0018 8480 3107 0000 0018 8490 4907 0000  ....1.......I...
-00005250: 0017 8491 4907 0000 0017 8492 3307 0000  ....I.......3...
-00005260: 0018 84ac 5107 0000 0018 84ad 5107 0000  ....Q.......Q...
-00005270: 0018 84ae 5107 0000 0018 84af 5107 0000  ....Q.......Q...
-00005280: 0154 8612 3f08 0000 0181 0a86 1f34 0700  .T..?........4..
-00005290: 0002 6686 2d34 0800 0001 80a6 8635 3407  ..f.-4.......54.
-000052a0: 0000 0021 86ab 3607 0000 0034 8830 3f07  ...!..6....4.0?.
-000052b0: 0000 002f 88d1 4907 0000 0034 88da 4a07  .../..I....4..J.
-000052c0: 0000 002d 88e3 4707 0000 002e 88e8 2f07  ...-..G......./.
-000052d0: 0000 002e 88ea 5a07 0000 0033 88ec 2f07  ......Z....3../.
-000052e0: 0000 0033 88ee 5b07 0000 002c 88f0 2f07  ...3..[....,../.
-000052f0: 0000 002c 88f2 5807 0000 0035 891d 3507  ...,..X....5..5.
-00005300: 0000 0030 896c 5b07 0000 0030 897b 5b07  ...0.l[....0.{[.
-00005310: 0000 002f 8983 5b07 0000 002f 898a 5b07  .../..[..../..[.
-00005320: 0000 0034 8991 5b06 0000 0034 380d 1f03  ...4..[....48...
-00005330: 0000 3c3d 0d0e 0037 0200 0d00 6a02 0855  ..<=...7....j..U
-00005340: 003c 0279 0900 2202 000d 0001 0279 1504  .<.y.."......y..
-00005350: 0000 3c46 0d0e 002b 0200 0d00 2202 000d  ..<F...+...."...
-00005360: 0001 0279 1504 0000 3c4d 0d0e 002a 0200  ...y....<M...*..
-00005370: 0d00 2202 000d 0001 0279 0b00 0000 2454  .."......y....$T
-00005380: 0d0d 0001 0279 0b05 0000 2559 0d35 0b04  .....y....%Y.5..
-00005390: 0200 0b05 0000 246a 0d35 0904 0200 80a8  ......$j.5......
-000053a0: 0600 0021 8083 2709 0000 0200 0d00 5f04  ...!..'......._.
-000053b0: 001d 0477 0700 0004 0002 7d26 0600 1b0a  ...w......}&....
-000053c0: 0409 0000 0500 0c00 6104 0000 0700 2204  ........a.....".
-000053d0: 770d 0041 0200 1d00 2f02 001d 000e 0408  w..A..../.......
-000053e0: 0700 2002 0013 0027 0200 1400 2104 0013  .. ....'....!...
-000053f0: 0080 8302 084f 0030 0671 1a00 6d02 083b  .....O.0.q..m..;
-00005400: 0017 0479 0d00 1702 000d 004e 0200 1800  ...y.......N....
-00005410: 2e02 0007 0022 0200 0f00 2202 000f 005c  ....."...."....\
-00005420: 0200 2c00 6002 002c 0025 0200 0d00 2602  ..,.`..,.%....&.
-00005430: 0012 001e 0200 1b00 6602 0023 0000 0400  ........f..#....
-00005440: 0249 2409 0001 3c4d 0700 0000 4286 0652  .I$...<M....B..R
-00005450: 0700 0000 4289 2252 0700 0000 3180 9b2c  ....B."R....1..,
-00005460: 0700 0000 6a80 b326 0700 0000 4a80 b625  ....j..&....J..%
-00005470: 0700 0000 6e80 bf27 0700 0000 4d80 c226  ....n..'....M..&
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0100 7f27 0100 2b29 0000 0000 0100 1b3e  ...'..+).......>
+00000160: 0200 223e 0000 0000 0000 0000 0200 c53e  ..">...........>
+00000170: 0000 0000 0000 0000 0200 d23e 0200 da3e  ...........>...>
+00000180: 0200 e73e 0000 0000 0000 0000 0100 ef3e  ...>...........>
+00000190: 0100 f73e 0100 ff3e 0100 073f 0100 0f3f  ...>...>...?...?
+000001a0: 0100 173f 0100 1f3f 0100 273f 0100 2f3f  ...?...?..'?../?
+000001b0: 0100 373f 0100 3f3f 0100 473f 0100 4f3f  ..7?..??..G?..O?
+000001c0: 0100 573f 0100 603f 0100 683f 0100 713f  ..W?..`?..h?..q?
+000001d0: 0100 793f 0100 813f 0100 893f 0100 913f  ..y?...?...?...?
+000001e0: 0100 993f 0100 a13f 0100 a93f 0100 b13f  ...?...?...?...?
+000001f0: 0100 b93f 0100 c13f 0100 c93f 0100 d13f  ...?...?...?...?
+00000200: 0100 d93f 0100 e13f 0100 e93f 0100 f13f  ...?...?...?...?
+00000210: 0000 0000 0100 f93f 0100 0040 0100 2040  .......?...@.. @
+00000220: 0100 3640 0100 4c40 0100 5840 0100 6440  ..6@..L@..X@..d@
+00000230: 0100 7040 0100 1a41 0100 2241 0000 0000  ..p@...A.."A....
+00000240: 0100 2a41 0000 0000 0100 3241 0100 3a41  ..*A......2A..:A
+00000250: 0100 4241 0100 4a41 0600 0300 0100 0100  ..BA..JA........
+00000260: 0000 0000 6900 0000 0700 0300 0200 0100  ....i...........
+00000270: 0000 0000 8ca1 0000 0700 0300 3600 0500  ............6...
+00000280: 2800 0000 2b00 0000 0700 0300 3700 0500  (...+.......7...
+00000290: fa00 0000 4400 0000 0700 0300 3800 0500  ....D.......8...
+000002a0: 3e01 0000 0502 0000 0700 0300 3b00 0500  >...........;...
+000002b0: 0402 0000 4000 0000 0700 0300 3c00 0500  ....@.......<...
+000002c0: 0303 0000 4000 0000 0700 0300 3d00 0500  ....@.......=...
+000002d0: a63f 0000 4f00 0000 0700 0300 3e00 0500  .?..O.......>...
+000002e0: 3a41 0000 2500 0000 0700 0300 3f00 0500  :A..%.......?...
+000002f0: c542 0000 2500 0000 0700 0300 4000 0500  .B..%.......@...
+00000300: 3644 0000 2800 0000 0700 0300 4100 0500  6D..(.......A...
+00000310: 8c44 0000 4500 0000 0700 0300 4200 0500  .D..E.......B...
+00000320: 6945 0000 4500 0000 0700 0300 4300 0500  iE..E.......C...
+00000330: 8746 0000 2b00 0000 0700 0300 4400 0500  .F..+.......D...
+00000340: fd4b 0000 c801 0000 0700 0300 4500 0500  .K..........E...
+00000350: 094c 0000 aa01 0000 0700 0300 4a00 0500  .L..........J...
+00000360: fb4e 0000 2b00 0000 0700 0300 4b00 0500  .N..+.......K...
+00000370: 714f 0000 2b00 0000 0700 0300 4c00 0500  qO..+.......L...
+00000380: 0b51 0000 d50d 0000 0700 0300 5b00 0500  .Q..........[...
+00000390: 0167 0000 2b00 0000 0700 0300 5c00 0500  .g..+.......\...
+000003a0: a567 0000 2100 0000 0700 0300 5d00 0500  .g..!.......]...
+000003b0: 7868 0000 1c00 0000 0700 0300 5e00 0500  xh..........^...
+000003c0: 6e69 0000 1c00 0000 0700 0300 5f00 0500  ni.........._...
+000003d0: 0c6a 0000 2b00 0000 0700 0300 6000 0500  .j..+.......`...
+000003e0: a36a 0000 1c00 0000 0700 0300 6100 0500  .j..........a...
+000003f0: 346b 0000 1c00 0000 0700 0300 6200 0500  4k..........b...
+00000400: 2b6c 0000 2b00 0000 0700 0300 6300 0500  +l..+.......c...
+00000410: 166d 0000 2b00 0000 0700 0300 6400 0500  .m..+.......d...
+00000420: e06d 0000 2b00 0000 0700 0300 6500 0500  .m..+.......e...
+00000430: ec6f 0000 1b00 0000 0700 0300 6600 0500  .o..........f...
+00000440: d173 0000 2b00 0000 0700 0300 6700 0500  .s..+.......g...
+00000450: ee74 0000 cc06 0000 0700 0300 6800 0500  .t..........h...
+00000460: 3277 0000 3800 0000 0700 0300 6900 0500  2w..8.......i...
+00000470: 767e 0000 5304 0000 0700 0300 6b00 0500  v~..S.......k...
+00000480: 927e 0000 3704 0000 0700 0300 6c00 0500  .~..7.......l...
+00000490: ac7e 0000 c703 0000 0700 0300 6d00 0500  .~..........m...
+000004a0: c87e 0000 8b03 0000 0700 0300 6e00 0500  .~..........n...
+000004b0: d17e 0000 8203 0000 0700 0300 6f00 0500  .~..........o...
+000004c0: 437f 0000 8900 0000 0700 0300 7000 0500  C...........p...
+000004d0: f782 0000 8b03 0000 0700 0300 7200 0500  ............r...
+000004e0: 1383 0000 6f03 0000 0700 0300 7600 0500  ....o.......v...
+000004f0: 7b85 0000 2c00 0000 0700 0300 7700 0500  {...,.......w...
+00000500: a28b 0000 1600 0000 0700 0300 7800 0500  ............x...
+00000510: 1e8c 0000 2100 0000 0700 0300 7900 0500  ....!.......y...
+00000520: f98c 0000 2500 0000 0700 0300 7a00 0500  ....%.......z...
+00000530: 2c8d 0000 6000 0000 0700 0300 7b00 0500  ,...`.......{...
+00000540: 628e 0000 4900 0000 0700 0300 7c00 0500  b...I.......|...
+00000550: 0a8f 0000 3700 0000 0700 0300 7d00 0500  ....7.......}...
+00000560: a08f 0000 2100 0000 0700 0300 7e00 0500  ....!.......~...
+00000570: 2090 0000 3700 0000 0700 0300 7f00 0500   ...7...........
+00000580: b690 0000 4c00 0000 0700 0300 8000 0500  ....L...........
+00000590: 3691 0000 2b00 0000 0700 0300 8100 0500  6...+...........
+000005a0: 1592 0000 1001 0000 0700 0300 8200 0500  ................
+000005b0: 3192 0000 da00 0000 0700 0300 8300 0500  1...............
+000005c0: 7792 0000 8200 0000 0700 0300 8400 0500  w...............
+000005d0: a095 0000 5d00 0000 0700 0300 8500 0500  ....]...........
+000005e0: ba95 0000 4300 0000 0700 0300 8700 0500  ....C...........
+000005f0: 48a1 0000 4300 0000 0900 0300 8800 0500  H...C...........
+00000600: 0000 0000 0b00 0000 0a00 0500 8800 0500  ................
+00000610: 0000 0000 3300 0000 0d00 0500 8800 0500  ....3...........
+00000620: 0000 0000 1d00 0000 1000 0500 8800 0500  ................
+00000630: 0000 0000 1200 0000 1100 0500 8800 0500  ................
+00000640: 0000 0000 1d00 0000 1200 0500 8800 0500  ................
+00000650: 0000 0000 1200 0000 1500 0300 8800 0500  ................
+00000660: 0000 0000 0e00 0000 1600 0300 8800 0500  ................
+00000670: 0000 0000 0e00 0000 1700 0300 8800 0500  ................
+00000680: 0000 0000 0e00 0000 1800 0300 8800 0500  ................
+00000690: 0000 0000 0e00 0000 1900 0300 8800 0500  ................
+000006a0: 0000 0000 1d00 0000 1a00 0300 8800 0500  ................
+000006b0: 0000 0000 1a00 0000 1b00 0300 8800 0500  ................
+000006c0: 0000 0000 1a00 0000 1c00 0300 8800 0500  ................
+000006d0: 0000 0000 1a00 0000 1d00 0300 8800 0500  ................
+000006e0: 0000 0000 1d00 0000 1e00 0300 8800 0500  ................
+000006f0: 0000 0000 1d00 0000 1f00 0300 8800 0500  ................
+00000700: 0000 0000 1d00 0000 2000 0300 8800 0500  ........ .......
+00000710: 0000 0000 1d00 0000 2100 0300 8800 0500  ........!.......
+00000720: 0000 0000 4300 0000 2200 0300 8800 0500  ....C...".......
+00000730: 0000 0000 5a00 0000 2300 0300 8800 0500  ....Z...#.......
+00000740: 0000 0000 5a00 0000 2400 0300 8800 0500  ....Z...$.......
+00000750: 0000 0000 4300 0000 2500 0300 8800 0500  ....C...%.......
+00000760: 0000 0000 1600 0000 2600 0300 8800 0500  ........&.......
+00000770: 0000 0000 1b00 0000 2700 0300 8800 0500  ........'.......
+00000780: 0000 0000 1100 0000 2800 0300 8800 0500  ........(.......
+00000790: 0000 0000 1100 0000 2900 0300 8800 0500  ........).......
+000007a0: 0000 0000 1100 0000 2a00 0300 8800 0500  ........*.......
+000007b0: 0000 0000 1100 0000 2b00 0300 8800 0500  ........+.......
+000007c0: 0000 0000 1100 0000 2c00 0300 8800 0500  ........,.......
+000007d0: 0000 0000 1100 0000 2d00 0300 8800 0500  ........-.......
+000007e0: 0000 0000 1100 0000 2e00 0300 8800 0500  ................
+000007f0: 0000 0000 1100 0000 2f00 0300 8800 0500  ......../.......
+00000800: 0000 0000 1100 0000 3000 0300 8800 0500  ........0.......
+00000810: 0000 0000 1600 0000 3100 0300 8800 0500  ........1.......
+00000820: 0000 0000 1b00 0000 3200 0300 8800 0500  ........2.......
+00000830: 0000 0000 1b00 0000 3300 0300 8800 0500  ........3.......
+00000840: 0000 0000 1b00 0000 3400 0300 8800 0500  ........4.......
+00000850: 0000 0000 1b00 0000 3500 0300 8800 0500  ........5.......
+00000860: 0000 0000 1b00 0000 3700 0300 8800 0500  ........7.......
+00000870: 0000 0000 0e00 0000 3800 0300 8800 0500  ........8.......
+00000880: 0000 0000 8700 0000 3900 0300 8900 0500  ........9.......
+00000890: 0000 0000 2900 0000 3a00 0300 8a00 0500  ....)...:.......
+000008a0: 0000 0000 2900 0000 3b00 0300 8b00 0500  ....)...;.......
+000008b0: 0000 0000 0e00 0000 3c00 0300 8b00 0500  ........<.......
+000008c0: 0000 0000 8500 0000 3d00 0300 8b00 0500  ........=.......
+000008d0: 0000 0000 7700 0000 3e00 0300 8b00 0500  ....w...>.......
+000008e0: 0000 0000 7f02 0000 3e00 0300 8b00 0500  ........>.......
+000008f0: 0b00 0000 0b00 0000 3e00 0300 8c00 0500  ........>.......
+00000900: 2e00 0000 4302 0000 3e00 0300 8d00 0500  ....C...>.......
+00000910: 3200 0000 3f02 0000 3f00 0300 8f00 0500  2...?...?.......
+00000920: 0000 0000 1d00 0000 4000 0300 8f00 0500  ........@.......
+00000930: 0000 0000 1d00 0000 4200 0300 8f00 0500  ........B.......
+00000940: 0000 0000 2400 0000 4400 0300 8f00 0500  ....$...D.......
+00000950: 0000 0000 3900 0000 4500 0300 8f00 0500  ....9...E.......
+00000960: 0000 0000 3100 0000 4600 0300 8f00 0500  ....1...F.......
+00000970: 0000 0000 3900 0000 4700 0300 8f00 0500  ....9...G.......
+00000980: 0000 0000 3100 0000 0000 0000 9305 0000  ....1...........
+00000990: 0000 0100 0000 0100 c103 0000 0200 6402  ..............d.
+000009a0: 0000 0300 4102 0000 0400 0f03 0000 0500  ....A...........
+000009b0: 8304 0000 0600 7303 0000 0700 cc01 0000  ......s.........
+000009c0: 0800 9801 0000 0900 4f01 0000 0a00 3d05  ........O.....=.
+000009d0: 0000 0b00 e402 0000 0c00 2303 0000 0d00  ..........#.....
+000009e0: ef04 0000 0e00 1505 0000 0f00 4c03 0000  ............L...
+000009f0: 1000 3803 0000 1100 4800 0000 1200 5800  ..8.....H.....X.
+00000a00: 0000 1300 3500 0000 1400 fc01 0000 1500  ....5...........
+00000a10: 7704 0000 1600 f703 0000 1700 6403 0000  w...........d...
+00000a20: 1800 5f01 0000 1900 2100 0000 1a00 8702  .._.....!.......
+00000a30: 0000 1b00 6b01 0000 1c00 ea00 0000 1d00  ....k...........
+00000a40: d900 0000 1e00 3501 0000 1f00 7801 0000  ......5.....x...
+00000a50: 2000 c504 0000 2100 aa04 0000 2200 9604   .....!....."...
+00000a60: 0000 2300 db04 0000 2400 8503 0000 2500  ..#.....$.....%.
+00000a70: 2c05 0000 2600 4405 0000 2700 5605 0000  ,...&.D...'.V...
+00000a80: 2800 fc04 0000 2900 0502 0000 2a00 bc01  (.....).....*...
+00000a90: 0000 2b00 ac01 0000 2c00 5c02 0000 2d00  ..+.....,.\...-.
+00000aa0: b600 0000 2e00 af03 0000 2f00 a503 0000  ........../.....
+00000ab0: 3000 7505 0000 3100 8405 0000 3200 6805  0.u...1.....2.h.
+00000ac0: 0000 3300 0304 0000 3400 ac03 0000 3600  ..3.....4.....6.
+00000ad0: be03 0000 3700 1100 0000 3800 f001 0000  ....7.....8.....
+00000ae0: 3900 e301 0000 3a00 be03 0000 3b00 be03  9.....:.....;...
+00000af0: 0000 3d00 de01 0000 3e00 1202 0000 3f00  ..=.....>.....?.
+00000b00: 1202 0000 4000 1202 0000 4200 af00 0000  ....@.....B.....
+00000b10: 4400 af00 0000 4500 1202 0000 4700 7c02  D.....E.....G.|.
+00000b20: 0000 4800 7003 0000 4900 5502 0000 4a00  ..H.p...I.U...J.
+00000b30: 3103 0000 4b00 8f04 0000 4c00 f702 0000  1...K.....L.....
+00000b40: 4d00 3c02 0000 4e00 3c02 0000 4f00 c802  M.<...N.<...O...
+00000b50: 0000 5000 6404 0000 5100 1e04 0000 5200  ..P.d...Q.....R.
+00000b60: 4e04 0000 5300 3804 0000 5400 1004 0000  N...S.8...T.....
+00000b70: 5500 cc03 0000 5600 e303 0000 5700 2501  U.....V.....W.%.
+00000b80: 0000 5800 bb02 0000 5900 1801 0000 5a00  ..X.....Y.....Z.
+00000b90: 9902 0000 5b00 f600 0000 5c00 a802 0000  ....[.....\.....
+00000ba0: 5d00 0501 0000 6000 de01 0000 6400 7003  ].....`.....d.p.
+00000bb0: 0000 6600 de01 0000 6700 de01 0000 6800  ..f.....g.....h.
+00000bc0: de01 0000 6900 de01 0000 6a00 de01 0000  ....i.....j.....
+00000bd0: 6b00 de01 0000 6c00 de01 0000 6d00 de01  k.....l.....m...
+00000be0: 0000 6e00 df02 0000 6f00 de01 0000 7100  ..n.....o.....q.
+00000bf0: 9c05 0000 7400 9105 0000 7600 be00 0000  ....t.....v.....
+00000c00: 7700 7e02 0000 7a00 c100 0000 7b00 df02  w.~...z.....{...
+00000c10: 0000 7c00 d803 0000 7d00 0c05 0000 7e00  ..|.....}.....~.
+00000c20: de01 0000 8200 3102 0000 8300 9703 0000  ......1.........
+00000c30: 8600 ee03 0000 8700 4401 0000 8800 8a01  ........D.......
+00000c40: 0000 8900 c700 0000 8a00 9105 0000 8b00  ................
+00000c50: de01 0000 8c00 7003 0000 8d00 1202 0000  ......p.........
+00000c60: 8e00 7c02 0000 8f00 d803 0000 9000 d803  ..|.............
+00000c70: 0000 9100 d803 0000 9200 d803 0000 9300  ................
+00000c80: d803 0000 9400 1202 0000 9500 df02 0000  ................
+00000c90: 9600 7003 0000 9700 de01 0000 9a00 1b02  ..p.............
+00000ca0: 0000 9d00 2802 0000 9e00 d802 0000 9f00  ....(...........
+00000cb0: ac03 0000 0000 0c05 0000 0000 0c05 0000  ................
+00000cc0: 0000 0c05 0000 0200 9e03 0000 0300 7302  ..............s.
+00000cd0: 0000 0400 0100 0000 0500 9002 6900 033e  ............i..>
+00000ce0: 9800 093e 7f00 0f3e 0103 153e 0000 0000  ...>...>...>....
+00000cf0: 0100 f728 0200 0000 0100 9a3e 0400 0000  ...(.......>....
+00000d00: 2700 0400 9d01 2700 0500 c303 0301 0300  '.....'.........
+00000d10: 9b01 2301 0300 9b01 4301 0300 9b01 8301  ..#.....C.......
+00000d20: 0300 9b01 a301 0300 9b01 c301 0300 9b01  ................
+00000d30: 0000 0000 0043 5324 3c3e 385f 5f6c 6f63  .....CS$<>8__loc
+00000d40: 616c 7330 0043 5324 3c3e 385f 5f6c 6f63  als0.CS$<>8__loc
+00000d50: 616c 7331 006f 7074 696f 6e73 4469 7370  als1.optionsDisp
+00000d60: 6c61 7955 7365 7232 0077 6174 6572 5475  layUser2.waterTu
+00000d70: 7262 696e 6544 6f6f 7243 4300 7468 6f74  rbineDoorCC.thot
+00000d80: 684c 6566 7444 6f6f 7243 4300 7468 6f74  hLeftDoorCC.thot
+00000d90: 6852 6967 6874 446f 6f72 4343 0054 686f  hRightDoorCC.Tho
+00000da0: 7468 4272 6964 6765 4c65 6674 446f 6f72  thBridgeLeftDoor
+00000db0: 4944 0041 3257 6174 6572 5475 7262 696e  ID.A2WaterTurbin
+00000dc0: 654c 6566 7444 6f6f 7249 4400 5468 6f74  eLeftDoorID.Thot
+00000dd0: 6842 7269 6467 6552 6967 6874 446f 6f72  hBridgeRightDoor
+00000de0: 4944 0064 6f6f 7249 4400 7376 366c 6f61  ID.doorID.sv6loa
+00000df0: 6400 6964 0066 6f75 6e64 0063 6f6c 6c69  d.id.found.colli
+00000e00: 7369 6f6e 436f 6465 546f 4265 0073 686f  sionCodeToBe.sho
+00000e10: 6f74 4d69 7373 696c 6543 6f64 6500 6e65  otMissileCode.ne
+00000e20: 7747 616d 6543 6f64 6500 6465 7074 6873  wGameCode.depths
+00000e30: 5069 7065 436f 6465 0077 6174 6572 6661  PipeCode.waterfa
+00000e40: 6c6c 7350 6970 6543 6f64 6500 6e65 7374  llsPipeCode.nest
+00000e50: 5069 7065 436f 6465 0068 6964 656f 7574  PipeCode.hideout
+00000e60: 5069 7065 436f 6465 0063 6853 7465 7046  PipeCode.chStepF
+00000e70: 6972 6543 6f64 6500 6372 6561 7465 436f  ireCode.createCo
+00000e80: 6465 0075 6e6c 6f63 6b53 7475 6666 436f  de.unlockStuffCo
+00000e90: 6465 0064 7261 7747 7569 436f 6465 006c  de.drawGuiCode.l
+00000ea0: 6162 426c 6f63 6b43 6f64 6500 6368 5374  abBlockCode.chSt
+00000eb0: 6570 436f 6e74 726f 6c43 6f64 6500 636f  epControlCode.co
+00000ec0: 6c6c 6973 696f 6e43 6f64 6500 6761 6d65  llisionCode.game
+00000ed0: 5365 6c4d 656e 7553 7465 7043 6f64 6500  SelMenuStepCode.
+00000ee0: 6c6f 6164 476c 6f62 616c 7343 6f64 6500  loadGlobalsCode.
+00000ef0: 7361 7665 476c 6f62 616c 7343 6f64 6500  saveGlobalsCode.
+00000f00: 6368 6172 6163 7465 7256 6172 7343 6f64  characterVarsCod
+00000f10: 6500 636f 6465 0061 3450 6167 6532 496d  e.code.a4Page2Im
+00000f20: 6167 6500 6134 5061 6765 496d 6167 6500  age.a4PageImage.
+00000f30: 7465 6d70 5469 6c65 0073 7461 7274 4e65  tempTile.startNe
+00000f40: 7747 616d 6500 636f 6465 4e61 6d65 0069  wGame.codeName.i
+00000f50: 6e74 6572 6e61 6c4e 616d 6500 726f 6f6d  nternalName.room
+00000f60: 4e61 6d65 0070 6963 6b75 704e 616d 6500  Name.pickupName.
+00000f70: 6e61 6d65 0077 6973 646f 6d53 6570 746f  name.wisdomSepto
+00000f80: 6767 4372 6561 7465 0063 7265 6174 6500  ggCreate.create.
+00000f90: 7376 3653 6176 6500 6f57 6973 646f 6d53  sv6Save.oWisdomS
+00000fa0: 6570 746f 6767 0066 696c 6550 6174 6800  eptogg.filePath.
+00000fb0: 6900 646f 6f72 4c6f 636b 006c 6162 426c  i.doorLock.labBl
+00000fc0: 6f63 6b00 7061 6765 4974 656d 0064 6570  ock.pageItem.dep
+00000fd0: 7468 7350 6970 6552 6f6f 6d00 7761 7465  thsPipeRoom.wate
+00000fe0: 7266 616c 6c73 5069 7065 526f 6f6d 006e  rfallsPipeRoom.n
+00000ff0: 6573 7450 6970 6552 6f6f 6d00 6869 6465  estPipeRoom.hide
+00001000: 6f75 7450 6970 6552 6f6f 6d00 676d 526f  outPipeRoom.gmRo
+00001010: 6f6d 0072 6f6f 6d00 646f 6f72 5361 6d75  om.room.doorSamu
+00001020: 7343 6f6c 6c69 7369 6f6e 0063 6f6c 6c69  sCollision.colli
+00001030: 7369 6f6e 0070 6167 6544 696d 656e 7369  sion.pageDimensi
+00001040: 6f6e 0077 6973 646f 6d53 6570 746f 6767  on.wisdomSeptogg
+00001050: 4163 7469 6f6e 0076 6172 446f 6f72 4163  Action.varDoorAc
+00001060: 7469 6f6e 0061 6374 696f 6e00 6135 4163  tion.action.a5Ac
+00001070: 7469 7661 7465 436f 6e64 6974 696f 6e00  tivateCondition.
+00001080: 656d 7042 6174 7465 7279 4365 6c6c 436f  empBatteryCellCo
+00001090: 6e64 6974 696f 6e00 7363 7244 4e41 5370  ndition.scrDNASp
+000010a0: 6177 6e00 676f 0077 6973 646f 6d53 6570  awn.go.wisdomSep
+000010b0: 746f 6767 5374 6570 0073 7562 7363 7265  toggStep.subscre
+000010c0: 656e 4d65 6e75 5374 6570 0070 6963 6b75  enMenuStep.picku
+000010d0: 7000 7375 6244 6972 0061 3544 6f6f 7200  p.subDir.a5Door.
+000010e0: 6673 0073 7636 6c6f 6164 4465 7461 696c  fs.sv6loadDetail
+000010f0: 7300 6d73 0073 6565 644f 626a 6563 7400  s.ms.seedObject.
+00001100: 736f 6c69 644f 626a 6563 7400 6761 6d65  solidObject.game
+00001110: 4f62 6a65 6374 0070 6970 654f 626a 6563  Object.pipeObjec
+00001120: 7400 676d 4f62 6a65 6374 0065 6e65 6d79  t.gmObject.enemy
+00001130: 4f62 6a65 6374 0065 7461 6e6b 536e 6970  Object.etankSnip
+00001140: 7065 7400 7069 7065 4247 5469 6c65 7365  pet.pipeBGTilese
+00001150: 7400 6465 7074 6873 456e 7472 616e 6365  t.depthsEntrance
+00001160: 5069 7065 5469 6c65 7365 7400 7761 7465  PipeTileset.wate
+00001170: 7266 616c 6c73 5069 7065 5469 6c65 7365  rfallsPipeTilese
+00001180: 7400 6465 7074 6873 4578 6974 5069 7065  t.depthsExitPipe
+00001190: 5469 6c65 7365 7400 6869 6465 6f75 7450  Tileset.hideoutP
+000011a0: 6970 6554 696c 6573 6574 0064 6f6f 7254  ipeTileset.doorT
+000011b0: 696c 6573 6574 0077 6973 646f 6d53 6570  ileset.wisdomSep
+000011c0: 746f 6767 4576 656e 7400 7042 6f6d 6243  toggEvent.pBombC
+000011d0: 6861 7261 6374 6572 4576 656e 7400 7375  haracterEvent.su
+000011e0: 7065 724d 6973 7369 6c65 4368 6172 6163  perMissileCharac
+000011f0: 7465 7245 7665 6e74 006d 6973 7369 6c65  terEvent.missile
+00001200: 4368 6172 6163 7465 7245 7665 6e74 0065  CharacterEvent.e
+00001210: 5461 6e6b 4368 6172 6163 7465 7245 7665  TankCharacterEve
+00001220: 6e74 0076 6172 446f 6f72 4576 656e 7400  nt.varDoorEvent.
+00001230: 6974 656d 7353 7761 7053 6372 6970 7400  itemsSwapScript.
+00001240: 636f 6465 5465 7874 006e 6577 446f 6f72  codeText.newDoor
+00001250: 5265 706c 6163 656d 656e 7454 6578 7400  ReplacementText.
+00001260: 7375 6273 6372 6565 6e4d 6973 6344 6177  subscreenMiscDaw
+00001270: 0073 7344 7261 7700 7375 6263 7265 656e  .ssDraw.subcreen
+00001280: 426f 6f74 7344 7261 7700 7375 6273 6372  BootsDraw.subscr
+00001290: 6565 6e53 7569 7444 7261 7700 6472 6177  eenSuitDraw.draw
+000012a0: 456e 6449 6e64 6578 0064 6f6f 7245 7665  EndIndex.doorEve
+000012b0: 6e74 496e 6465 7800 6472 6177 5374 6172  ntIndex.drawStar
+000012c0: 7449 6e64 6578 0061 7373 656d 626c 7900  tIndex.assembly.
+000012d0: 7175 616e 7469 7479 0000 0000 0000 0000  quantity........
+000012e0: 0fd0 2988 b811 1342 878b 770e 8597 ac16  ..)....B..w.....
+000012f0: f862 513f c607 d311 9053 00c0 4fa3 02a1  .bQ?.....S..O...
+00001300: bc74 2e93 a9db 7844 8d46 0f32 a7ba b3d3  .t....xD.F.2....
+00001310: 05ec feb5 d08c 834a 96da 4662 84bb 4bd8  .......J..Fb..K.
+00001320: 0847 4d7e 6e09 5c4c aeda cb10 ba6a 740d  .GM~n.\L.....jt.
+00001330: 0004 686f 6d65 0672 756e 6e65 7204 776f  ..home.runner.wo
+00001340: 726b 0459 414d 5308 5941 4d53 2d4c 4942  rk.YAMS.YAMS-LIB
+00001350: 0a50 726f 6772 616d 2e63 7309 2f00 0106  .Program.cs./...
+00001360: 0d12 1217 2020 fcd7 b607 0947 2a7f 005f  ....  .....G*.._
+00001370: d4dc 8bfa 96be 9c69 7aa0 808c d517 10d9  .......iz.......
+00001380: d077 717a 270f 0d53 6565 644f 626a 6563  .wqz'..SeedObjec
+00001390: 742e 6373 092f 0001 060d 1212 1756 2056  t.cs./.......V V
+000013a0: 65af b720 c3e8 22d1 155a 7563 de4b a863  e.. .."..Zuc.K.c
+000013b0: e3cc 373b 3f57 25d2 3772 9abe a3a6 0a03  ..7;?W%.7r......
+000013c0: 6f62 6a07 5265 6c65 6173 6506 6e65 7436  obj.Release.net6
+000013d0: 2e30 1a59 414d 532d 4c49 422e 476c 6f62  .0.YAMS-LIB.Glob
+000013e0: 616c 5573 696e 6773 2e67 2e63 7310 2f00  alUsings.g.cs./.
+000013f0: 0106 0d12 1217 808f 8093 809b 80a2 205d  .............. ]
+00001400: d6d5 28fd d6c4 4688 4302 02cd 32e6 b714  ..(...F.C...2...
+00001410: 4a8a ec9d fc9f 674a 11e9 0331 1930 c42e  J.....gJ...1.0..
+00001420: 2e4e 4554 436f 7265 4170 702c 5665 7273  .NETCoreApp,Vers
+00001430: 696f 6e3d 7636 2e30 2e41 7373 656d 626c  ion=v6.0.Assembl
+00001440: 7941 7474 7269 6275 7465 732e 6373 102f  yAttributes.cs./
+00001450: 0001 060d 1212 1780 8f80 9380 9b80 ef20  ............... 
+00001460: 7897 e595 3cb5 cd51 3150 9b35 0421 8634  x...<..Q1P.5.!.4
+00001470: c24b 9ce7 a68b 984f fb5a 1668 6eb5 af5c  .K.....O.Z.hn..\
+00001480: 1859 414d 532d 4c49 422e 4173 7365 6d62  .YAMS-LIB.Assemb
+00001490: 6c79 496e 666f 2e63 7310 2f00 0106 0d12  lyInfo.cs./.....
+000014a0: 1217 808f 8093 809b 8150 20b3 6d04 3831  .........P .m.81
+000014b0: 1077 0013 335d a311 2fb4 9cad d51a 19ee  .w..3]../.......
+000014c0: 52a3 9f5f 4e55 4995 a566 a501 0282 2476  R.._NUI..f....$v
+000014d0: 6572 7369 6f6e 0032 0063 6f6d 7069 6c65  ersion.2.compile
+000014e0: 722d 7665 7273 696f 6e00 342e 362e 302d  r-version.4.6.0-
+000014f0: 332e 3233 3235 392e 382b 6333 6363 3164  3.23259.8+c3cc1d
+00001500: 3063 6565 6162 3161 3635 6461 3032 3137  0ceeab1a65da0217
+00001510: 6534 3033 3835 3161 3165 3861 3330 3038  e403851a1e8a3008
+00001520: 3661 006c 616e 6775 6167 6500 4323 0073  6a.language.C#.s
+00001530: 6f75 7263 652d 6669 6c65 2d63 6f75 6e74  ource-file-count
+00001540: 0035 006f 7574 7075 742d 6b69 6e64 0044  .5.output-kind.D
+00001550: 796e 616d 6963 616c 6c79 4c69 6e6b 6564  ynamicallyLinked
+00001560: 4c69 6272 6172 7900 6f70 7469 6d69 7a61  Library.optimiza
+00001570: 7469 6f6e 0072 656c 6561 7365 0070 6c61  tion.release.pla
+00001580: 7466 6f72 6d00 416e 7943 7075 0072 756e  tform.AnyCpu.run
+00001590: 7469 6d65 2d76 6572 7369 6f6e 0037 2e30  time-version.7.0
+000015a0: 2e39 2b38 6539 6131 3762 3232 3136 6635  .9+8e9a17b2216f5
+000015b0: 3161 3537 3838 6638 6231 6334 3637 6134  1a5788f8b1c467a4
+000015c0: 6366 3362 3736 3965 3764 3700 6c61 6e67  cf3b769e7d7.lang
+000015d0: 7561 6765 2d76 6572 7369 6f6e 0070 7265  uage-version.pre
+000015e0: 7669 6577 006e 756c 6c61 626c 6500 456e  view.nullable.En
+000015f0: 6162 6c65 0064 6566 696e 6500 5452 4143  able.define.TRAC
+00001600: 452c 5245 4c45 4153 452c 4e45 542c 4e45  E,RELEASE,NET,NE
+00001610: 5436 5f30 2c4e 4554 434f 5245 4150 502c  T6_0,NETCOREAPP,
+00001620: 4e45 5435 5f30 5f4f 525f 4752 4541 5445  NET5_0_OR_GREATE
+00001630: 522c 4e45 5436 5f30 5f4f 525f 4752 4541  R,NET6_0_OR_GREA
+00001640: 5445 522c 4e45 5443 4f52 4541 5050 315f  TER,NETCOREAPP1_
+00001650: 305f 4f52 5f47 5245 4154 4552 2c4e 4554  0_OR_GREATER,NET
+00001660: 434f 5245 4150 5031 5f31 5f4f 525f 4752  COREAPP1_1_OR_GR
+00001670: 4541 5445 522c 4e45 5443 4f52 4541 5050  EATER,NETCOREAPP
+00001680: 325f 305f 4f52 5f47 5245 4154 4552 2c4e  2_0_OR_GREATER,N
+00001690: 4554 434f 5245 4150 5032 5f31 5f4f 525f  ETCOREAPP2_1_OR_
+000016a0: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
+000016b0: 5050 325f 325f 4f52 5f47 5245 4154 4552  PP2_2_OR_GREATER
+000016c0: 2c4e 4554 434f 5245 4150 5033 5f30 5f4f  ,NETCOREAPP3_0_O
+000016d0: 525f 4752 4541 5445 522c 4e45 5443 4f52  R_GREATER,NETCOR
+000016e0: 4541 5050 335f 315f 4f52 5f47 5245 4154  EAPP3_1_OR_GREAT
+000016f0: 4552 00a3 ba49 4353 6861 7270 436f 6465  ER...ICSharpCode
+00001700: 2e53 6861 7270 5a69 704c 6962 2e64 6c6c  .SharpZipLib.dll
+00001710: 0000 016c 9904 9800 8003 0087 d282 16a4  ...l............
+00001720: 95d1 4abd 3f1f c402 13b4 ed4d 6163 726f  ..J.?......Macro
+00001730: 7373 2e4a 736f 6e2e 4578 7465 6e73 696f  ss.Json.Extensio
+00001740: 6e73 2e64 6c6c 0000 0155 c478 ba00 0001  ns.dll...U.x....
+00001750: 00b2 09ba d9ca d5dc 4e93 a42a 22b1 17ec  ........N..*"...
+00001760: 344d 6963 726f 736f 6674 2e43 5368 6172  4Microsoft.CShar
+00001770: 702e 646c 6c00 0001 0749 52d7 0080 0000  p.dll....IR.....
+00001780: 17e1 8671 93a1 9e42 a11d 4bf1 cb94 691c  ...q...B..K...i.
+00001790: 4d69 6372 6f73 6f66 742e 5669 7375 616c  Microsoft.Visual
+000017a0: 4261 7369 632e 436f 7265 2e64 6c6c 0000  Basic.Core.dll..
+000017b0: 01fd f562 8500 2001 0008 ae07 b107 183f  ...b.. ........?
+000017c0: 4282 f29e 3548 56b3 9f4d 6963 726f 736f  B...5HV..Microso
+000017d0: 6674 2e56 6973 7561 6c42 6173 6963 2e64  ft.VisualBasic.d
+000017e0: 6c6c 0000 019a 0054 d700 8000 00a8 a4e9  ll.....T........
+000017f0: c9a3 ffc3 4aae 82d9 bfb4 281d 754d 6963  ....J.....(.uMic
+00001800: 726f 736f 6674 2e57 696e 3332 2e50 7269  rosoft.Win32.Pri
+00001810: 6d69 7469 7665 732e 646c 6c00 0001 66d5  mitives.dll...f.
+00001820: 2dfc 0080 0000 e73e d1c6 4da4 f344 8f16  -......>..M..D..
+00001830: 2586 5dd6 7d54 4d69 6372 6f73 6f66 742e  %.].}TMicrosoft.
+00001840: 5769 6e33 322e 5265 6769 7374 7279 2e64  Win32.Registry.d
+00001850: 6c6c 0000 0161 b328 9f00 a000 007a 4531  ll...a.(.....zE1
+00001860: 5af2 af1d 489d 9445 67ef 8b8b 1e6d 7363  Z...H..Eg....msc
+00001870: 6f72 6c69 622e 646c 6c00 0001 cdd0 f4f6  orlib.dll.......
+00001880: 0020 0100 fcaf 6eca 8e72 524a bf2b 9464  . ....n..rRJ.+.d
+00001890: ddc5 4cef 6e65 7473 7461 6e64 6172 642e  ..L.netstandard.
+000018a0: 646c 6c00 0001 2f8c b0fe 00c0 0100 faf8  dll.../.........
+000018b0: f92e a718 f040 8eb8 58ce cd30 4898 5072  .....@..X..0H.Pr
+000018c0: 6f70 6572 7479 4368 616e 6765 642e 646c  opertyChanged.dl
+000018d0: 6c00 0001 8b5a 978a 0080 0000 3174 ff35  l....Z......1t.5
+000018e0: d3a6 344c 90ea 21b0 de57 7fe0 5369 784c  ..4L..!..W..SixL
+000018f0: 6162 6f72 732e 496d 6167 6553 6861 7270  abors.ImageSharp
+00001900: 2e64 6c6c 0000 016c 8a3e dd00 601f 007f  .dll...l.>..`...
+00001910: 776a e7b5 74d7 4aaa 9d41 db13 6c03 4353  wj..t.J..A..l.CS
+00001920: 7973 7465 6d2e 4170 7043 6f6e 7465 7874  ystem.AppContext
+00001930: 2e64 6c6c 0000 0170 94a2 e200 8000 0025  .dll...p.......%
+00001940: 2e6c 6fa8 98f6 4d8c 7a65 cb60 d06b d753  .lo...M.ze.`.k.S
+00001950: 7973 7465 6d2e 4275 6666 6572 732e 646c  ystem.Buffers.dl
+00001960: 6c00 0001 4862 a3da 0080 0000 b7aa 5ee8  l...Hb........^.
+00001970: 37bf c340 a7a9 80fb 3588 0655 5379 7374  7..@....5..USyst
+00001980: 656d 2e43 6f6c 6c65 6374 696f 6e73 2e43  em.Collections.C
+00001990: 6f6e 6375 7272 656e 742e 646c 6c00 0001  oncurrent.dll...
+000019a0: 801f 71e1 00a0 0000 9df2 9458 7ad0 f54d  ..q........Xz..M
+000019b0: 89ee e2ea 7478 52a8 5379 7374 656d 2e43  ....txR.System.C
+000019c0: 6f6c 6c65 6374 696f 6e73 2e64 6c6c 0000  ollections.dll..
+000019d0: 0189 c9a8 ca00 0001 0048 1fec 5634 526b  .........H..V4Rk
+000019e0: 4082 f7a3 b914 aaec c953 7973 7465 6d2e  @........System.
+000019f0: 436f 6c6c 6563 7469 6f6e 732e 496d 6d75  Collections.Immu
+00001a00: 7461 626c 652e 646c 6c00 0001 7a6e d5f0  table.dll...zn..
+00001a10: 0040 0100 3840 68b9 d79c 9746 8218 e630  .@..8@h....F...0
+00001a20: 2acc ca10 5379 7374 656d 2e43 6f6c 6c65  *...System.Colle
+00001a30: 6374 696f 6e73 2e4e 6f6e 4765 6e65 7269  ctions.NonGeneri
+00001a40: 632e 646c 6c00 0001 d8e6 4cac 00a0 0000  c.dll.....L.....
+00001a50: d21c c278 ed7e a648 858e 03c2 f6be df33  ...x.~.H.......3
+00001a60: 5379 7374 656d 2e43 6f6c 6c65 6374 696f  System.Collectio
+00001a70: 6e73 2e53 7065 6369 616c 697a 6564 2e64  ns.Specialized.d
+00001a80: 6c6c 0000 019c fa3c d300 a000 0023 9f8f  ll.....<.....#..
+00001a90: 8a45 230e 44b8 cc5f c180 b6bf c653 7973  .E#.D.._.....Sys
+00001aa0: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
+00001ab0: 656c 2e41 6e6e 6f74 6174 696f 6e73 2e64  el.Annotations.d
+00001ac0: 6c6c 0000 01be 614b ec00 c000 0055 a438  ll....aK.....U.8
+00001ad0: af72 c4c4 4e90 86bc 1224 07f2 eb53 7973  .r..N....$...Sys
+00001ae0: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
+00001af0: 656c 2e44 6174 6141 6e6e 6f74 6174 696f  el.DataAnnotatio
+00001b00: 6e73 2e64 6c6c 0000 0184 683a fe00 8000  ns.dll....h:....
+00001b10: 0005 d0f9 02c1 73b8 4b89 44c0 7c3c 00f1  ......s.K.D.|<..
+00001b20: ab53 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
+00001b30: 744d 6f64 656c 2e64 6c6c 0000 014e 2422  tModel.dll...N$"
+00001b40: 8700 8000 00e9 ad6e e8bd 5995 4ea9 e15c  .......n..Y.N..\
+00001b50: 5c7c a0bd 0353 7973 7465 6d2e 436f 6d70  \|...System.Comp
+00001b60: 6f6e 656e 744d 6f64 656c 2e45 7665 6e74  onentModel.Event
+00001b70: 4261 7365 6441 7379 6e63 2e64 6c6c 0000  BasedAsync.dll..
+00001b80: 01e2 a443 9700 8000 00fd e5d9 3533 23ce  ...C........53#.
+00001b90: 4081 038b a246 c95b d253 7973 7465 6d2e  @....F.[.System.
+00001ba0: 436f 6d70 6f6e 656e 744d 6f64 656c 2e50  ComponentModel.P
+00001bb0: 7269 6d69 7469 7665 732e 646c 6c00 0001  rimitives.dll...
+00001bc0: 4296 8faf 00a0 0000 f190 fdcb 2f09 1540  B.........../..@
+00001bd0: b5ed 6b66 648c ea66 5379 7374 656d 2e43  ..kfd..fSystem.C
+00001be0: 6f6d 706f 6e65 6e74 4d6f 6465 6c2e 5479  omponentModel.Ty
+00001bf0: 7065 436f 6e76 6572 7465 722e 646c 6c00  peConverter.dll.
+00001c00: 0001 78b1 0aa1 00c0 0100 f5c9 711b 41c1  ..x.........q.A.
+00001c10: 2b4f a387 838a 4ca9 04c5 5379 7374 656d  +O....L...System
+00001c20: 2e43 6f6e 6669 6775 7261 7469 6f6e 2e64  .Configuration.d
+00001c30: 6c6c 0000 0142 606d 9700 8000 0047 fc59  ll...B`m.....G.Y
+00001c40: 3fb8 f598 4bb7 c800 e5d4 fe5d 2853 7973  ?...K......](Sys
+00001c50: 7465 6d2e 436f 6e73 6f6c 652e 646c 6c00  tem.Console.dll.
+00001c60: 0001 c631 eba4 00a0 0000 01fb ca4e 49e4  ...1.........NI.
+00001c70: fd47 8ba7 a6a6 0d03 5401 5379 7374 656d  .G......T.System
+00001c80: 2e43 6f72 652e 646c 6c00 0001 0f44 62a6  .Core.dll....Db.
+00001c90: 00a0 0000 1145 5732 5df8 7844 88f9 180f  .....EW2].xD....
+00001ca0: b7c6 af61 5379 7374 656d 2e44 6174 612e  ...aSystem.Data.
+00001cb0: 436f 6d6d 6f6e 2e64 6c6c 0000 0171 db86  Common.dll...q..
+00001cc0: f800 8002 0070 101f 3c3b 13f1 42a8 564f  .....p..<;..B.VO
+00001cd0: 2861 4a19 ac53 7973 7465 6d2e 4461 7461  (aJ..System.Data
+00001ce0: 2e44 6174 6153 6574 4578 7465 6e73 696f  .DataSetExtensio
+00001cf0: 6e73 2e64 6c6c 0000 01d9 8f9f bf00 8000  ns.dll..........
+00001d00: 00a0 76e7 b0b2 20f3 4c91 083a bbe6 ac79  ..v... .L..:...y
+00001d10: ef53 7973 7465 6d2e 4461 7461 2e64 6c6c  .System.Data.dll
+00001d20: 0000 010c 4483 9e00 a000 002d 7ff2 3276  ....D......-..2v
+00001d30: 1ae6 44ae 9eb3 76fe e7e2 dc53 7973 7465  ..D...v....Syste
+00001d40: 6d2e 4469 6167 6e6f 7374 6963 732e 436f  m.Diagnostics.Co
+00001d50: 6e74 7261 6374 732e 646c 6c00 0001 b13e  ntracts.dll....>
+00001d60: 63fc 0080 0000 276b 11c6 c4f0 2544 b417  c.....'k....%D..
+00001d70: 4af0 15a4 eb81 5379 7374 656d 2e44 6961  J.....System.Dia
+00001d80: 676e 6f73 7469 6373 2e44 6562 7567 2e64  gnostics.Debug.d
+00001d90: 6c6c 0000 01ed 49cb f400 8000 004b 9eb6  ll....I......K..
+00001da0: 499b 2776 4cae b41c 2924 2a3e e553 7973  I.'vL...)$*>.Sys
+00001db0: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
+00001dc0: 4469 6167 6e6f 7374 6963 536f 7572 6365  DiagnosticSource
+00001dd0: 2e64 6c6c 0000 018c f22c f800 c000 0031  .dll.....,.....1
+00001de0: 3552 2d2c 67e3 4487 e849 98de 1554 b053  5R-,g.D..I...T.S
+00001df0: 7973 7465 6d2e 4469 6167 6e6f 7374 6963  ystem.Diagnostic
+00001e00: 732e 4669 6c65 5665 7273 696f 6e49 6e66  s.FileVersionInf
+00001e10: 6f2e 646c 6c00 0001 5fe3 fcf2 0080 0000  o.dll..._.......
+00001e20: 4d91 ef25 cb82 d040 b004 9607 0811 7076  M..%...@......pv
+00001e30: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
+00001e40: 6373 2e50 726f 6365 7373 2e64 6c6c 0000  cs.Process.dll..
+00001e50: 0128 cad2 b200 c000 007d 9733 70f0 bac2  .(.......}.3p...
+00001e60: 45a1 fa60 16b0 497e 2353 7973 7465 6d2e  E..`..I~#System.
+00001e70: 4469 6167 6e6f 7374 6963 732e 5374 6163  Diagnostics.Stac
+00001e80: 6b54 7261 6365 2e64 6c6c 0000 0135 fff9  kTrace.dll...5..
+00001e90: b200 a000 00ad 5f8a 71cb 64c7 459c 731d  ......_.q.d.E.s.
+00001ea0: 01da b22d 7953 7973 7465 6d2e 4469 6167  ...-ySystem.Diag
+00001eb0: 6e6f 7374 6963 732e 5465 7874 5772 6974  nostics.TextWrit
+00001ec0: 6572 5472 6163 654c 6973 7465 6e65 722e  erTraceListener.
+00001ed0: 646c 6c00 0001 5a50 95c4 0080 0000 88d5  dll...ZP........
+00001ee0: 8bd4 95e2 d24b 94d5 f302 b798 1df6 5379  .....K........Sy
+00001ef0: 7374 656d 2e44 6961 676e 6f73 7469 6373  stem.Diagnostics
+00001f00: 2e54 6f6f 6c73 2e64 6c6c 0000 01a0 613c  .Tools.dll....a<
+00001f10: fe00 8000 00cc 118d eff1 3cf0 42a5 309f  ..........<.B.0.
+00001f20: 6b00 7903 fb53 7973 7465 6d2e 4469 6167  k.y..System.Diag
+00001f30: 6e6f 7374 6963 732e 5472 6163 6553 6f75  nostics.TraceSou
+00001f40: 7263 652e 646c 6c00 0001 66d5 d884 00a0  rce.dll...f.....
+00001f50: 0000 5722 142a d78a e144 b398 42db 6ad1  ..W".*...D..B.j.
+00001f60: b885 5379 7374 656d 2e44 6961 676e 6f73  ..System.Diagnos
+00001f70: 7469 6373 2e54 7261 6369 6e67 2e64 6c6c  tics.Tracing.dll
+00001f80: 0000 016e 9980 de00 a000 00e8 77f8 d4fb  ...n........w...
+00001f90: 6360 43aa 5057 a2c1 5c08 9553 7973 7465  c`C.PW..\..Syste
+00001fa0: 6d2e 646c 6c00 0001 1b34 e8f0 0000 0100  m.dll....4......
+00001fb0: 042d f79f 0ace ff43 9292 a2bb 74fc e9ac  .-.....C....t...
+00001fc0: 5379 7374 656d 2e44 7261 7769 6e67 2e43  System.Drawing.C
+00001fd0: 6f6d 6d6f 6e2e 646c 6c00 0001 218d 42d5  ommon.dll...!.B.
+00001fe0: 0020 0200 0843 fec0 6a78 bb46 9f62 dc8a  . ...C..jx.F.b..
+00001ff0: c5b5 5abc 5379 7374 656d 2e44 7261 7769  ..Z.System.Drawi
+00002000: 6e67 2e64 6c6c 0000 012a c527 8600 8000  ng.dll...*.'....
+00002010: 0053 29d0 50ec d5fd 41b7 5dc0 3bb4 fec2  .S).P...A.].;...
+00002020: aa53 7973 7465 6d2e 4472 6177 696e 672e  .System.Drawing.
+00002030: 5072 696d 6974 6976 6573 2e64 6c6c 0000  Primitives.dll..
+00002040: 0130 b401 ca00 c000 008e 8f7f 0f67 cfeb  .0...........g..
+00002050: 438c aca0 408d d5b7 8853 7973 7465 6d2e  C...@....System.
+00002060: 4479 6e61 6d69 632e 5275 6e74 696d 652e  Dynamic.Runtime.
+00002070: 646c 6c00 0001 7af8 ba93 0080 0000 00d2  dll...z.........
+00002080: 3986 f2b3 5047 98a0 8d09 122b 601d 5379  9...PG.....+`.Sy
+00002090: 7374 656d 2e46 6f72 6d61 7473 2e41 736e  stem.Formats.Asn
+000020a0: 312e 646c 6c00 0001 d5eb 2df8 00a0 0000  1.dll.....-.....
+000020b0: 6809 fe95 7ccf be4c aa8e 7879 c0e9 dd04  h...|..L..xy....
+000020c0: 5379 7374 656d 2e47 6c6f 6261 6c69 7a61  System.Globaliza
+000020d0: 7469 6f6e 2e43 616c 656e 6461 7273 2e64  tion.Calendars.d
+000020e0: 6c6c 0000 0119 2fbb 9a00 8000 008e 0099  ll..../.........
+000020f0: e074 bd7f 4caa 3458 690f b25a 7b53 7973  .t..L.4Xi..Z{Sys
+00002100: 7465 6d2e 476c 6f62 616c 697a 6174 696f  tem.Globalizatio
+00002110: 6e2e 646c 6c00 0001 d1af f6a4 0080 0000  n.dll...........
+00002120: 4f43 3c41 90af 6f45 9f16 2060 991e 4966  OC<A..oE.. `..If
+00002130: 5379 7374 656d 2e47 6c6f 6261 6c69 7a61  System.Globaliza
+00002140: 7469 6f6e 2e45 7874 656e 7369 6f6e 732e  tion.Extensions.
+00002150: 646c 6c00 0001 f33d 8be4 0080 0000 198b  dll....=........
+00002160: dc84 e703 df49 959b ece8 5b61 08d3 5379  .....I....[a..Sy
+00002170: 7374 656d 2e49 4f2e 436f 6d70 7265 7373  stem.IO.Compress
+00002180: 696f 6e2e 4272 6f74 6c69 2e64 6c6c 0000  ion.Brotli.dll..
+00002190: 01bc 6117 e100 8000 003c 5edd 0f96 2796  ..a......<^...'.
+000021a0: 41bc 60e7 167c 93ec ff53 7973 7465 6d2e  A.`..|...System.
+000021b0: 494f 2e43 6f6d 7072 6573 7369 6f6e 2e64  IO.Compression.d
+000021c0: 6c6c 0000 01ea 16ee b900 a000 00b4 df97  ll..............
+000021d0: ee7e bd80 459a 36f1 fbf4 4867 3853 7973  .~..E.6...Hg8Sys
+000021e0: 7465 6d2e 494f 2e43 6f6d 7072 6573 7369  tem.IO.Compressi
+000021f0: 6f6e 2e46 696c 6553 7973 7465 6d2e 646c  on.FileSystem.dl
+00002200: 6c00 0001 6b99 aed3 0080 0000 523d 5710  l...k.......R=W.
+00002210: 75f0 1a48 ada5 d1b7 890b 0c6c 5379 7374  u..H.......lSyst
+00002220: 656d 2e49 4f2e 436f 6d70 7265 7373 696f  em.IO.Compressio
+00002230: 6e2e 5a69 7046 696c 652e 646c 6c00 0001  n.ZipFile.dll...
+00002240: 5853 7cc3 0080 0000 580d 2f60 b7c2 004e  XS|.....X./`...N
+00002250: a5bf 0576 acb1 67d9 5379 7374 656d 2e49  ...v..g.System.I
+00002260: 4f2e 646c 6c00 0001 1ced 88ed 0080 0000  O.dll...........
+00002270: 2b3c c477 14f7 844c bba2 c24f 55c2 8603  +<.w...L...OU...
+00002280: 5379 7374 656d 2e49 4f2e 4669 6c65 5379  System.IO.FileSy
+00002290: 7374 656d 2e41 6363 6573 7343 6f6e 7472  stem.AccessContr
+000022a0: 6f6c 2e64 6c6c 0000 01a5 3b8d 9000 a000  ol.dll....;.....
+000022b0: 007a eb3c 18a8 34fc 4c9a 38c0 0ddf dedc  .z.<..4.L.8.....
+000022c0: 8853 7973 7465 6d2e 494f 2e46 696c 6553  .System.IO.FileS
+000022d0: 7973 7465 6d2e 646c 6c00 0001 f9c7 0dbf  ystem.dll.......
+000022e0: 0080 0000 eca4 c059 9fbc 744e a4af 37c2  .......Y..tN..7.
+000022f0: dca4 b1f9 5379 7374 656d 2e49 4f2e 4669  ....System.IO.Fi
+00002300: 6c65 5379 7374 656d 2e44 7269 7665 496e  leSystem.DriveIn
+00002310: 666f 2e64 6c6c 0000 0175 7d28 cf00 8000  fo.dll...u}(....
+00002320: 006e a90f b3e5 511d 47b0 7485 905f 7688  .n....Q.G.t.._v.
+00002330: 0553 7973 7465 6d2e 494f 2e46 696c 6553  .System.IO.FileS
+00002340: 7973 7465 6d2e 5072 696d 6974 6976 6573  ystem.Primitives
+00002350: 2e64 6c6c 0000 01b3 710c 9800 8000 0050  .dll....q......P
+00002360: 7c76 ce46 08de 4499 13d6 6755 6ff3 ed53  |v.F..D...gUo..S
+00002370: 7973 7465 6d2e 494f 2e46 696c 6553 7973  ystem.IO.FileSys
+00002380: 7465 6d2e 5761 7463 6865 722e 646c 6c00  tem.Watcher.dll.
+00002390: 0001 eeb6 f7b2 00a0 0000 d4b5 5f3a 5fd9  ............_:_.
+000023a0: 3b41 8dc2 cac6 4bde 7572 5379 7374 656d  ;A....K.urSystem
+000023b0: 2e49 4f2e 4973 6f6c 6174 6564 5374 6f72  .IO.IsolatedStor
+000023c0: 6167 652e 646c 6c00 0001 a38e dec4 00a0  age.dll.........
+000023d0: 0000 3710 05cc 327d f64d b4ce 8a5c 6c81  ..7...2}.M...\l.
+000023e0: 614e 5379 7374 656d 2e49 4f2e 4d65 6d6f  aNSystem.IO.Memo
+000023f0: 7279 4d61 7070 6564 4669 6c65 732e 646c  ryMappedFiles.dl
+00002400: 6c00 0001 47f5 1ff4 0080 0000 9151 f98c  l...G........Q..
+00002410: 5e36 494b 90f8 515d 8b59 68cf 5379 7374  ^6IK..Q].Yh.Syst
+00002420: 656d 2e49 4f2e 5069 7065 732e 4163 6365  em.IO.Pipes.Acce
+00002430: 7373 436f 6e74 726f 6c2e 646c 6c00 0001  ssControl.dll...
+00002440: 7f6c 5bfc 0080 0000 3bd5 5395 4e3d 4b4d  .l[.....;.S.N=KM
+00002450: 9687 50e1 5508 b91f 5379 7374 656d 2e49  ..P.U...System.I
+00002460: 4f2e 5069 7065 732e 646c 6c00 0001 26a5  O.Pipes.dll...&.
+00002470: fdc3 00a0 0000 d904 bc24 8b94 9a47 9743  .........$...G.C
+00002480: a06e d131 4978 5379 7374 656d 2e49 4f2e  .n.1IxSystem.IO.
+00002490: 556e 6d61 6e61 6765 644d 656d 6f72 7953  UnmanagedMemoryS
+000024a0: 7472 6561 6d2e 646c 6c00 0001 d746 0fa0  tream.dll....F..
+000024b0: 0080 0000 d3a0 8040 199b 5441 b8d9 284f  .......@..TA..(O
+000024c0: 57b3 9292 5379 7374 656d 2e4c 696e 712e  W...System.Linq.
+000024d0: 646c 6c00 0001 d06e d586 00c0 0000 697d  dll....n......i}
+000024e0: 34b4 dfec 2b40 bd36 4017 1269 d6a6 5379  4...+@.6@..i..Sy
+000024f0: 7374 656d 2e4c 696e 712e 4578 7072 6573  stem.Linq.Expres
+00002500: 7369 6f6e 732e 646c 6c00 0001 85c6 9691  sions.dll.......
+00002510: 0040 0100 1ac9 5fc9 1258 fc47 aa66 0d42  .@...._..X.G.f.B
+00002520: 9ed0 c519 5379 7374 656d 2e4c 696e 712e  ....System.Linq.
+00002530: 5061 7261 6c6c 656c 2e64 6c6c 0000 019a  Parallel.dll....
+00002540: e108 c500 c000 00f0 26d0 c04a 43cf 4286  ........&..JC.B.
+00002550: 80d5 7630 02e0 4e53 7973 7465 6d2e 4c69  ..v0..NSystem.Li
+00002560: 6e71 2e51 7565 7279 6162 6c65 2e64 6c6c  nq.Queryable.dll
+00002570: 0000 012f 3dc9 8700 c000 00b4 2fac f0a4  .../=......./...
+00002580: 719c 4596 cef1 c318 bcdc e853 7973 7465  q.E........Syste
+00002590: 6d2e 4d65 6d6f 7279 2e64 6c6c 0000 01d1  m.Memory.dll....
+000025a0: f194 9700 e000 0039 ecd5 1a26 3372 43a1  .......9...&3rC.
+000025b0: 3b0a 2cd8 c030 3853 7973 7465 6d2e 4e65  ;.,..08System.Ne
+000025c0: 742e 646c 6c00 0001 d616 97d6 0080 0000  t.dll...........
+000025d0: 5be1 7e6f d1ef d447 bb98 0601 2b17 a015  [.~o...G....+...
+000025e0: 5379 7374 656d 2e4e 6574 2e48 7474 702e  System.Net.Http.
+000025f0: 646c 6c00 0001 9234 82c2 0020 0100 4285  dll....4... ..B.
+00002600: 9141 8cd2 c44a 9267 5fb6 c70d fe03 5379  .A...J.g_.....Sy
+00002610: 7374 656d 2e4e 6574 2e48 7474 702e 4a73  stem.Net.Http.Js
+00002620: 6f6e 2e64 6c6c 0000 01d6 70c7 eb00 8000  on.dll....p.....
+00002630: 00c5 125f 9f70 f8f9 4491 411f 3d51 8729  ..._.p..D.A.=Q.)
+00002640: 2053 7973 7465 6d2e 4e65 742e 4874 7470   System.Net.Http
+00002650: 4c69 7374 656e 6572 2e64 6c6c 0000 0131  Listener.dll...1
+00002660: 7ce3 f600 a000 00e5 f981 6441 2a43 4eb3  |.........dA*CN.
+00002670: e76c 51b6 41a4 2353 7973 7465 6d2e 4e65  .lQ.A.#System.Ne
+00002680: 742e 4d61 696c 2e64 6c6c 0000 012f 7bf6  t.Mail.dll.../{.
+00002690: d600 c000 00ec ef60 8c04 4e6a 499b d4ff  .......`..NjI...
+000026a0: 1379 5c16 2553 7973 7465 6d2e 4e65 742e  .y\.%System.Net.
+000026b0: 4e61 6d65 5265 736f 6c75 7469 6f6e 2e64  NameResolution.d
+000026c0: 6c6c 0000 017a 3c48 e300 8000 0089 4311  ll...z<H......C.
+000026d0: e3dc 4efa 4681 2104 d992 6096 b953 7973  ..N.F.!...`..Sys
+000026e0: 7465 6d2e 4e65 742e 4e65 7477 6f72 6b49  tem.Net.NetworkI
+000026f0: 6e66 6f72 6d61 7469 6f6e 2e64 6c6c 0000  nformation.dll..
+00002700: 01b1 ee6a 8600 c000 0006 798a 0663 7c93  ...j......y..c|.
+00002710: 4780 d5ac 2183 564d 9e53 7973 7465 6d2e  G...!.VM.System.
+00002720: 4e65 742e 5069 6e67 2e64 6c6c 0000 0126  Net.Ping.dll...&
+00002730: c08c eb00 8000 00e1 52c0 3460 a08b 46ac  ........R.4`..F.
+00002740: 6865 8747 2a97 0b53 7973 7465 6d2e 4e65  he.G*..System.Ne
+00002750: 742e 5072 696d 6974 6976 6573 2e64 6c6c  t.Primitives.dll
+00002760: 0000 0112 d83d 8800 c000 0084 7bc3 b094  .....=......{...
+00002770: 397b 4da0 2fc9 34b4 6560 b853 7973 7465  9{M./.4.e`.Syste
+00002780: 6d2e 4e65 742e 5265 7175 6573 7473 2e64  m.Net.Requests.d
+00002790: 6c6c 0000 01a2 8b03 cf00 e000 0081 1a5b  ll.............[
+000027a0: 1c42 02c0 40b0 a164 f25d 024e 4153 7973  .B..@..d.].NASys
+000027b0: 7465 6d2e 4e65 742e 5365 6375 7269 7479  tem.Net.Security
+000027c0: 2e64 6c6c 0000 0125 1d0d 9100 0001 0016  .dll...%........
+000027d0: 0258 8074 d086 4eb7 e3fc b0e2 cd22 3553  .X.t..N......"5S
+000027e0: 7973 7465 6d2e 4e65 742e 5365 7276 6963  ystem.Net.Servic
+000027f0: 6550 6f69 6e74 2e64 6c6c 0000 01ea 7bb7  ePoint.dll....{.
+00002800: c800 8000 000a cce3 6eaa fc06 4292 947c  ........n...B..|
+00002810: 79ae d821 0a53 7973 7465 6d2e 4e65 742e  y..!.System.Net.
+00002820: 536f 636b 6574 732e 646c 6c00 0001 b667  Sockets.dll....g
+00002830: 82e2 0000 0100 52ba 356f 9cb6 b547 958a  ......R.5o...G..
+00002840: 3902 0297 251a 5379 7374 656d 2e4e 6574  9...%.System.Net
+00002850: 2e57 6562 436c 6965 6e74 2e64 6c6c 0000  .WebClient.dll..
+00002860: 01de 75d8 b100 a000 0061 c26e 6835 0ccd  ..u......a.nh5..
+00002870: 4f85 dc2f 9b1f 8e52 0053 7973 7465 6d2e  O../...R.System.
+00002880: 4e65 742e 5765 6248 6561 6465 7243 6f6c  Net.WebHeaderCol
+00002890: 6c65 6374 696f 6e2e 646c 6c00 0001 5298  lection.dll...R.
+000028a0: a3af 0080 0000 9b0f bdce c94d dc4a 819b  ...........M.J..
+000028b0: 4efd 3172 d63f 5379 7374 656d 2e4e 6574  N.1r.?System.Net
+000028c0: 2e57 6562 5072 6f78 792e 646c 6c00 0001  .WebProxy.dll...
+000028d0: 4c21 05ed 0080 0000 b4ff cb6a 98e5 2546  L!.........j..%F
+000028e0: bcfe 7ace a33e 78db 5379 7374 656d 2e4e  ..z..>x.System.N
+000028f0: 6574 2e57 6562 536f 636b 6574 732e 436c  et.WebSockets.Cl
+00002900: 6965 6e74 2e64 6c6c 0000 018e 6030 ea00  ient.dll....`0..
+00002910: 8000 00d1 cbc2 a741 9dde 489b 9ef3 e424  .......A..H....$
+00002920: 25e4 2a53 7973 7465 6d2e 4e65 742e 5765  %.*System.Net.We
+00002930: 6253 6f63 6b65 7473 2e64 6c6c 0000 01f2  bSockets.dll....
+00002940: 6bd8 a000 a000 0018 fa75 49d6 02fa 4cb6  k........uI...L.
+00002950: a320 9f5a bdce 1053 7973 7465 6d2e 4e75  . .Z...System.Nu
+00002960: 6d65 7269 6373 2e64 6c6c 0000 0184 9828  merics.dll.....(
+00002970: ab00 8000 005e c453 95d3 d45e 44bb 10b8  .....^.S...^D...
+00002980: 106a aec7 6153 7973 7465 6d2e 4e75 6d65  .j..aSystem.Nume
+00002990: 7269 6373 2e56 6563 746f 7273 2e64 6c6c  rics.Vectors.dll
+000029a0: 0000 0128 605a dc00 c000 007e 186e 89d2  ...(`Z.....~.n..
+000029b0: cdb6 418a a3b7 3df7 dc27 d753 7973 7465  ..A...=..'.Syste
+000029c0: 6d2e 4f62 6a65 6374 4d6f 6465 6c2e 646c  m.ObjectModel.dl
+000029d0: 6c00 0001 9f0e 5aac 00c0 0000 67a6 7345  l.....Z.....g.sE
+000029e0: dcc6 104c 8668 0bb2 638b 7324 5379 7374  ...L.h..c.s$Syst
+000029f0: 656d 2e52 6566 6c65 6374 696f 6e2e 4469  em.Reflection.Di
+00002a00: 7370 6174 6368 5072 6f78 792e 646c 6c00  spatchProxy.dll.
+00002a10: 0001 309b 53d8 0080 0000 3a9b 950e d84e  ..0.S.....:....N
+00002a20: 184c 83d5 f836 66cd e4b5 5379 7374 656d  .L...6f...System
+00002a30: 2e52 6566 6c65 6374 696f 6e2e 646c 6c00  .Reflection.dll.
+00002a40: 0001 7aef 99f4 0080 0000 d4a3 74c6 ac2d  ..z.........t..-
+00002a50: da40 a910 978d 3860 89b2 5379 7374 656d  .@....8`..System
+00002a60: 2e52 6566 6c65 6374 696f 6e2e 456d 6974  .Reflection.Emit
+00002a70: 2e64 6c6c 0000 01bd ed33 c000 e000 003e  .dll.....3.....>
+00002a80: e0e1 3102 dfa7 4c9c 39a7 d340 04f3 7553  ..1...L.9..@..uS
+00002a90: 7973 7465 6d2e 5265 666c 6563 7469 6f6e  ystem.Reflection
+00002aa0: 2e45 6d69 742e 494c 4765 6e65 7261 7469  .Emit.ILGenerati
+00002ab0: 6f6e 2e64 6c6c 0000 01ea 8ba1 b100 a000  on.dll..........
+00002ac0: 0061 47ef bfb1 5a7b 4495 6eab 804d a813  .aG...Z{D.n..M..
+00002ad0: 3d53 7973 7465 6d2e 5265 666c 6563 7469  =System.Reflecti
+00002ae0: 6f6e 2e45 6d69 742e 4c69 6768 7477 6569  on.Emit.Lightwei
+00002af0: 6768 742e 646c 6c00 0001 3990 09cb 0080  ght.dll...9.....
+00002b00: 0000 6599 3a9e d785 854c a454 6ac0 387f  ..e.:....L.Tj.8.
+00002b10: d650 5379 7374 656d 2e52 6566 6c65 6374  .PSystem.Reflect
+00002b20: 696f 6e2e 4578 7465 6e73 696f 6e73 2e64  ion.Extensions.d
+00002b30: 6c6c 0000 01e7 0a6e 9a00 8000 00b0 bb2a  ll.....n.......*
+00002b40: d038 0c35 4c94 2514 b83e f83a d553 7973  .8.5L.%..>.:.Sys
+00002b50: 7465 6d2e 5265 666c 6563 7469 6f6e 2e4d  tem.Reflection.M
+00002b60: 6574 6164 6174 612e 646c 6c00 0001 a1e5  etadata.dll.....
+00002b70: 61c2 0020 0200 1e2f 7240 4688 fa4a a99a  a.. .../r@F..J..
+00002b80: 89ad 2bf2 7020 5379 7374 656d 2e52 6566  ..+.p System.Ref
+00002b90: 6c65 6374 696f 6e2e 5072 696d 6974 6976  lection.Primitiv
+00002ba0: 6573 2e64 6c6c 0000 0191 2932 ee00 a000  es.dll....)2....
+00002bb0: 007c 4929 f4b5 222d 4596 77b6 5a5b 4d24  .|I).."-E.w.Z[M$
+00002bc0: f353 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
+00002bd0: 6f6e 2e54 7970 6545 7874 656e 7369 6f6e  on.TypeExtension
+00002be0: 732e 646c 6c00 0001 3a94 eae3 0080 0000  s.dll...:.......
+00002bf0: 89a1 ba5e 6a57 7c45 92e9 ef81 f8e6 d8da  ...^jW|E........
+00002c00: 5379 7374 656d 2e52 6573 6f75 7263 6573  System.Resources
+00002c10: 2e52 6561 6465 722e 646c 6c00 0001 febc  .Reader.dll.....
+00002c20: a5b5 0080 0000 c3e8 8ab1 6ba5 8849 a02b  ..........k..I.+
+00002c30: 6f9c 54f3 bae2 5379 7374 656d 2e52 6573  o.T...System.Res
+00002c40: 6f75 7263 6573 2e52 6573 6f75 7263 654d  ources.ResourceM
+00002c50: 616e 6167 6572 2e64 6c6c 0000 01bc 85f7  anager.dll......
+00002c60: ce00 8000 0017 6017 82e9 ade6 4988 c3d0  ......`.....I...
+00002c70: 60bb 8c8c 5d53 7973 7465 6d2e 5265 736f  `...]System.Reso
+00002c80: 7572 6365 732e 5772 6974 6572 2e64 6c6c  urces.Writer.dll
+00002c90: 0000 0183 6b9b 8d00 8000 00f9 827c bb7f  ....k........|..
+00002ca0: 0463 4b99 b7f5 a734 22ca 0853 7973 7465  .cK....4"..Syste
+00002cb0: 6d2e 5275 6e74 696d 652e 436f 6d70 696c  m.Runtime.Compil
+00002cc0: 6572 5365 7276 6963 6573 2e55 6e73 6166  erServices.Unsaf
+00002cd0: 652e 646c 6c00 0001 6c72 7bc8 0080 0000  e.dll...lr{.....
+00002ce0: 8cd2 862d 3c11 ef44 8746 70b8 60b6 a3c6  ...-<..D.Fp.`...
+00002cf0: 5379 7374 656d 2e52 756e 7469 6d65 2e43  System.Runtime.C
+00002d00: 6f6d 7069 6c65 7253 6572 7669 6365 732e  ompilerServices.
+00002d10: 5669 7375 616c 432e 646c 6c00 0001 e4e9  VisualC.dll.....
+00002d20: 92c1 0080 0000 bbf3 2cba 4956 e44c 85e2  ........,.IV.L..
+00002d30: eab1 f356 d66c 5379 7374 656d 2e52 756e  ...V.lSystem.Run
+00002d40: 7469 6d65 2e64 6c6c 0000 014f a117 ce00  time.dll...O....
+00002d50: 8007 00a3 ef9c 58c3 b940 4d90 cede 3294  ......X..@M...2.
+00002d60: d4f3 0453 7973 7465 6d2e 5275 6e74 696d  ...System.Runtim
+00002d70: 652e 4578 7465 6e73 696f 6e73 2e64 6c6c  e.Extensions.dll
+00002d80: 0000 01fb 93c6 cd00 8000 0079 3b4b 0168  ...........y;K.h
+00002d90: 882e 4592 2115 ec92 b811 7253 7973 7465  ..E.!.....rSyste
+00002da0: 6d2e 5275 6e74 696d 652e 4861 6e64 6c65  m.Runtime.Handle
+00002db0: 732e 646c 6c00 0001 ebda e6f5 0080 0000  s.dll...........
+00002dc0: 9cc4 740a 05b5 1a4d 808c 076b abad a534  ..t....M...k...4
+00002dd0: 5379 7374 656d 2e52 756e 7469 6d65 2e49  System.Runtime.I
+00002de0: 6e74 6572 6f70 5365 7276 6963 6573 2e64  nteropServices.d
+00002df0: 6c6c 0000 01af cc8a 9c00 4001 0080 3b45  ll........@...;E
+00002e00: 973f ea70 4db5 d1a6 3ac2 986c 8b53 7973  .?.pM...:..l.Sys
+00002e10: 7465 6d2e 5275 6e74 696d 652e 496e 7465  tem.Runtime.Inte
+00002e20: 726f 7053 6572 7669 6365 732e 5275 6e74  ropServices.Runt
+00002e30: 696d 6549 6e66 6f72 6d61 7469 6f6e 2e64  imeInformation.d
+00002e40: 6c6c 0000 0119 3232 d500 8000 0007 f899  ll....22........
+00002e50: ecaf 3300 41b1 033e e1e8 7154 d753 7973  ..3.A..>..qT.Sys
+00002e60: 7465 6d2e 5275 6e74 696d 652e 496e 7472  tem.Runtime.Intr
+00002e70: 696e 7369 6373 2e64 6c6c 0000 0132 532d  insics.dll...2S-
+00002e80: 8100 c002 008f 41a5 9a68 4bba 4fb9 819d  ......A..hK.O...
+00002e90: 1b29 7f51 1f53 7973 7465 6d2e 5275 6e74  .).Q.System.Runt
+00002ea0: 696d 652e 4c6f 6164 6572 2e64 6c6c 0000  ime.Loader.dll..
+00002eb0: 01bd 89ce 9900 8000 00cb e5cd 3ba8 4a1f  ............;.J.
+00002ec0: 4892 5b14 edbf bd26 bd53 7973 7465 6d2e  H.[....&.System.
+00002ed0: 5275 6e74 696d 652e 4e75 6d65 7269 6373  Runtime.Numerics
+00002ee0: 2e64 6c6c 0000 0124 2e2e fc00 a000 00c6  .dll...$........
+00002ef0: 9bca 61ba aead 4fa2 bcf1 8b03 35d5 a853  ..a...O.....5..S
+00002f00: 7973 7465 6d2e 5275 6e74 696d 652e 5365  ystem.Runtime.Se
+00002f10: 7269 616c 697a 6174 696f 6e2e 646c 6c00  rialization.dll.
+00002f20: 0001 5732 cda0 0080 0000 96e2 9c85 b24f  ..W2...........O
+00002f30: 0c41 aa16 4e58 5d80 311b 5379 7374 656d  .A..NX].1.System
+00002f40: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
+00002f50: 7a61 7469 6f6e 2e46 6f72 6d61 7474 6572  zation.Formatter
+00002f60: 732e 646c 6c00 0001 8cf0 ff9b 00a0 0000  s.dll...........
+00002f70: e825 4dad c610 d949 9dbb 619b 1a21 4f2e  .%M....I..a..!O.
+00002f80: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
+00002f90: 6572 6961 6c69 7a61 7469 6f6e 2e4a 736f  erialization.Jso
+00002fa0: 6e2e 646c 6c00 0001 8772 c189 0080 0000  n.dll....r......
+00002fb0: dfbb 2c4f b09b 474a 80eb af14 4c47 2a68  ..,O..GJ....LG*h
+00002fc0: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
+00002fd0: 6572 6961 6c69 7a61 7469 6f6e 2e50 7269  erialization.Pri
+00002fe0: 6d69 7469 7665 732e 646c 6c00 0001 ca14  mitives.dll.....
+00002ff0: 3ec6 0080 0000 6ed2 d5f7 b8da f446 9b4b  >.....n......F.K
+00003000: be28 0c09 e6e8 5379 7374 656d 2e52 756e  .(....System.Run
+00003010: 7469 6d65 2e53 6572 6961 6c69 7a61 7469  time.Serializati
+00003020: 6f6e 2e58 6d6c 2e64 6c6c 0000 0152 bc99  on.Xml.dll...R..
+00003030: d400 c000 00c4 715b 4877 e90c 41bc 7941  ......q[Hw..A.yA
+00003040: 423c b424 5253 7973 7465 6d2e 5365 6375  B<.$RSystem.Secu
+00003050: 7269 7479 2e41 6363 6573 7343 6f6e 7472  rity.AccessContr
+00003060: 6f6c 2e64 6c6c 0000 01de 06e9 b000 e000  ol.dll..........
+00003070: 00fb c501 60dd 56b5 4b8e 958c 0bbf e0d6  ....`.V.K.......
+00003080: 4753 7973 7465 6d2e 5365 6375 7269 7479  GSystem.Security
+00003090: 2e43 6c61 696d 732e 646c 6c00 0001 3fae  .Claims.dll...?.
+000030a0: 48a4 00c0 0000 edad 319d 89bd 704d 90a5  H.......1...pM..
+000030b0: 3185 0c1e 2b37 5379 7374 656d 2e53 6563  1...+7System.Sec
+000030c0: 7572 6974 792e 4372 7970 746f 6772 6170  urity.Cryptograp
+000030d0: 6879 2e41 6c67 6f72 6974 686d 732e 646c  hy.Algorithms.dl
+000030e0: 6c00 0001 c701 8c95 0000 0100 e8b0 26da  l.............&.
+000030f0: db55 544d 84db 4f31 51f8 23db 5379 7374  .UTM..O1Q.#.Syst
+00003100: 656d 2e53 6563 7572 6974 792e 4372 7970  em.Security.Cryp
+00003110: 746f 6772 6170 6879 2e43 6e67 2e64 6c6c  tography.Cng.dll
+00003120: 0000 01a7 2137 a900 c000 00d2 d896 fb91  ....!7..........
+00003130: 538c 4ab8 cd2f c889 004e f053 7973 7465  S.J../...N.Syste
+00003140: 6d2e 5365 6375 7269 7479 2e43 7279 7074  m.Security.Crypt
+00003150: 6f67 7261 7068 792e 4373 702e 646c 6c00  ography.Csp.dll.
+00003160: 0001 52ed 5ec5 00a0 0000 ab21 6ba9 89a5  ..R.^......!k...
+00003170: be41 88ad bbeb 1330 938f 5379 7374 656d  .A.....0..System
+00003180: 2e53 6563 7572 6974 792e 4372 7970 746f  .Security.Crypto
+00003190: 6772 6170 6879 2e45 6e63 6f64 696e 672e  graphy.Encoding.
+000031a0: 646c 6c00 0001 82cb 6986 00a0 0000 de52  dll.....i......R
+000031b0: 53ff 2cb4 1d43 a6fe 0857 4f4a a648 5379  S.,..C...WOJ.HSy
+000031c0: 7374 656d 2e53 6563 7572 6974 792e 4372  stem.Security.Cr
+000031d0: 7970 746f 6772 6170 6879 2e4f 7065 6e53  yptography.OpenS
+000031e0: 736c 2e64 6c6c 0000 01d9 3597 c800 8000  sl.dll....5.....
+000031f0: 002f 85b5 187e 8878 44b2 9b7a 5607 e643  ./...~.xD..zV..C
+00003200: c653 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
+00003210: 2e43 7279 7074 6f67 7261 7068 792e 5072  .Cryptography.Pr
+00003220: 696d 6974 6976 6573 2e64 6c6c 0000 01f8  imitives.dll....
+00003230: 48bd b500 a000 0008 e488 d541 95c4 42a9  H..........A..B.
+00003240: c1d9 b932 5124 3153 7973 7465 6d2e 5365  ...2Q$1System.Se
+00003250: 6375 7269 7479 2e43 7279 7074 6f67 7261  curity.Cryptogra
+00003260: 7068 792e 5835 3039 4365 7274 6966 6963  phy.X509Certific
+00003270: 6174 6573 2e64 6c6c 0000 011e 8a31 f300  ates.dll.....1..
+00003280: e000 0038 99aa b575 db67 4e91 674a 6366  ...8...u.gN.gJcf
+00003290: 4066 c153 7973 7465 6d2e 5365 6375 7269  @f.System.Securi
+000032a0: 7479 2e64 6c6c 0000 01d7 281a af00 8000  ty.dll....(.....
+000032b0: 00fb e9da 24ff 618c 46bd 1b68 2e35 d8f5  ....$.a.F..h.5..
+000032c0: 0453 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
+000032d0: 2e50 7269 6e63 6970 616c 2e64 6c6c 0000  .Principal.dll..
+000032e0: 0197 afa4 d700 8000 0027 8a16 bac0 9544  .........'.....D
+000032f0: 4aa4 52ae 3e07 2e8d 6253 7973 7465 6d2e  J.R.>...bSystem.
+00003300: 5365 6375 7269 7479 2e50 7269 6e63 6970  Security.Princip
+00003310: 616c 2e57 696e 646f 7773 2e64 6c6c 0000  al.Windows.dll..
+00003320: 0137 b68c a200 a000 0007 4c72 b4ef d98a  .7........Lr....
+00003330: 4a8d 474f 44c7 e710 ea53 7973 7465 6d2e  J.GOD....System.
+00003340: 5365 6375 7269 7479 2e53 6563 7572 6553  Security.SecureS
+00003350: 7472 696e 672e 646c 6c00 0001 8ba7 83bf  tring.dll.......
+00003360: 0080 0000 cb5c 39de 14de 2e48 ac1c 4ab6  .....\9....H..J.
+00003370: b5b4 9011 5379 7374 656d 2e53 6572 7669  ....System.Servi
+00003380: 6365 4d6f 6465 6c2e 5765 622e 646c 6c00  ceModel.Web.dll.
+00003390: 0001 3dd3 54b3 0080 0000 a43a 99fe eb55  ..=.T......:...U
+000033a0: 9248 bbc3 a67b b1ba 123d 5379 7374 656d  .H...{...=System
+000033b0: 2e53 6572 7669 6365 5072 6f63 6573 732e  .ServiceProcess.
+000033c0: 646c 6c00 0001 899a cec1 0080 0000 5539  dll...........U9
+000033d0: 1e62 bd38 4d42 896d f311 a44b efb1 5379  .b.8MB.m...K..Sy
+000033e0: 7374 656d 2e54 6578 742e 456e 636f 6469  stem.Text.Encodi
+000033f0: 6e67 2e43 6f64 6550 6167 6573 2e64 6c6c  ng.CodePages.dll
+00003400: 0000 013c 2e5d f600 8000 00e1 b1ec fb2f  ...<.]........./
+00003410: d5b5 44a0 24ad c731 b431 0053 7973 7465  ..D.$..1.1.Syste
+00003420: 6d2e 5465 7874 2e45 6e63 6f64 696e 672e  m.Text.Encoding.
+00003430: 646c 6c00 0001 80b4 14a3 0080 0000 9ce3  dll.............
+00003440: b249 0b7e 8e43 9049 d265 90a2 e97d 5379  .I.~.C.I.e...}Sy
+00003450: 7374 656d 2e54 6578 742e 456e 636f 6469  stem.Text.Encodi
+00003460: 6e67 2e45 7874 656e 7369 6f6e 732e 646c  ng.Extensions.dl
+00003470: 6c00 0001 3f1b b5b0 00a0 0000 354c 6745  l...?.......5LgE
+00003480: cf2e 034a ad89 10f2 c783 bf90 5379 7374  ...J........Syst
+00003490: 656d 2e54 6578 742e 456e 636f 6469 6e67  em.Text.Encoding
+000034a0: 732e 5765 622e 646c 6c00 0001 b007 b8df  s.Web.dll.......
+000034b0: 00a0 0000 b7cd 6a87 6293 da46 8545 efbb  ......j.b..F.E..
+000034c0: 2261 49c1 5379 7374 656d 2e54 6578 742e  "aI.System.Text.
+000034d0: 4a73 6f6e 2e64 6c6c 0000 012f 3d98 cb00  Json.dll.../=...
+000034e0: 2001 00b1 04e5 583b b9ad 419e 3eda 6af1   .....X;..A.>.j.
+000034f0: 8497 7d53 7973 7465 6d2e 5465 7874 2e52  ..}System.Text.R
+00003500: 6567 756c 6172 4578 7072 6573 7369 6f6e  egularExpression
+00003510: 732e 646c 6c00 0001 7742 4fab 00c0 0000  s.dll...wBO.....
+00003520: c770 ed57 161f 3e47 af43 d65f 9424 cc8a  .p.W..>G.C._.$..
+00003530: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
+00003540: 2e43 6861 6e6e 656c 732e 646c 6c00 0001  .Channels.dll...
+00003550: 34bd fda0 0080 0000 3eb0 35d8 8199 f847  4.......>.5....G
+00003560: a870 6faa 4125 5e13 5379 7374 656d 2e54  .po.A%^.System.T
+00003570: 6872 6561 6469 6e67 2e64 6c6c 0000 01d3  hreading.dll....
+00003580: c2ec 9700 c000 0079 d76d 0a6c 4cde 42b1  .......y.m.lL.B.
+00003590: e029 f8d3 f114 1f53 7973 7465 6d2e 5468  .).....System.Th
+000035a0: 7265 6164 696e 672e 4f76 6572 6c61 7070  reading.Overlapp
+000035b0: 6564 2e64 6c6c 0000 0178 ccd2 a700 8000  ed.dll...x......
+000035c0: 0007 8bfa 9af2 34bb 42a1 453c abbf a67e  ......4.B.E<...~
+000035d0: b753 7973 7465 6d2e 5468 7265 6164 696e  .System.Threadin
+000035e0: 672e 5461 736b 732e 4461 7461 666c 6f77  g.Tasks.Dataflow
+000035f0: 2e64 6c6c 0000 016a 9fb3 f100 c000 0057  .dll...j.......W
+00003600: 1ee8 dc8f c8e2 4a9a 65f4 a83c 8ea0 fb53  ......J.e..<...S
+00003610: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
+00003620: 5461 736b 732e 646c 6c00 0001 0ec2 eab6  Tasks.dll.......
+00003630: 0080 0000 6555 7af7 eadb 8e4a b632 8c91  ....eUz....J.2..
+00003640: 7360 3ac0 5379 7374 656d 2e54 6872 6561  s`:.System.Threa
+00003650: 6469 6e67 2e54 6173 6b73 2e45 7874 656e  ding.Tasks.Exten
+00003660: 7369 6f6e 732e 646c 6c00 0001 0d9a feea  sions.dll.......
+00003670: 0080 0000 f3e4 81af 9578 2242 bb05 7b41  .........x"B..{A
+00003680: 707b b388 5379 7374 656d 2e54 6872 6561  p{..System.Threa
+00003690: 6469 6e67 2e54 6173 6b73 2e50 6172 616c  ding.Tasks.Paral
+000036a0: 6c65 6c2e 646c 6c00 0001 a67f 5b80 0080  lel.dll.....[...
+000036b0: 0000 5c62 7c74 ec73 8e4e b839 6f02 5da1  ..\b|t.s.N.9o.].
+000036c0: a896 5379 7374 656d 2e54 6872 6561 6469  ..System.Threadi
+000036d0: 6e67 2e54 6872 6561 642e 646c 6c00 0001  ng.Thread.dll...
+000036e0: bb81 fb87 00a0 0000 e0b9 fc04 8874 0b40  .............t.@
+000036f0: 9ba3 b7d0 1384 5979 5379 7374 656d 2e54  ......YySystem.T
+00003700: 6872 6561 6469 6e67 2e54 6872 6561 6450  hreading.ThreadP
+00003710: 6f6f 6c2e 646c 6c00 0001 13dd 58a8 0080  ool.dll.....X...
+00003720: 0000 9b33 fec3 3559 9e4a a6d4 0131 935f  ...3..5Y.J...1._
+00003730: 9a55 5379 7374 656d 2e54 6872 6561 6469  .USystem.Threadi
+00003740: 6e67 2e54 696d 6572 2e64 6c6c 0000 012c  ng.Timer.dll...,
+00003750: 6170 9600 8000 008f a3c6 bd14 b84c 4ea9  ap...........LN.
+00003760: 0b55 2fa7 ee6f 7c53 7973 7465 6d2e 5472  .U/..o|System.Tr
+00003770: 616e 7361 6374 696f 6e73 2e64 6c6c 0000  ansactions.dll..
+00003780: 01b6 6269 8000 8000 0032 370a 9851 5f81  ..bi.....27..Q_.
+00003790: 4882 e391 2b9c ba95 e953 7973 7465 6d2e  H...+....System.
+000037a0: 5472 616e 7361 6374 696f 6e73 2e4c 6f63  Transactions.Loc
+000037b0: 616c 2e64 6c6c 0000 01d1 1503 9700 a000  al.dll..........
+000037c0: 0065 2922 d1f3 3d59 4dbc 04a1 7e7c 7099  .e)"..=YM...~|p.
+000037d0: ee53 7973 7465 6d2e 5661 6c75 6554 7570  .System.ValueTup
+000037e0: 6c65 2e64 6c6c 0000 0157 aaac b900 8000  le.dll...W......
+000037f0: 009d 5a87 c7ad 3ff1 47a7 9196 b0b9 8f8d  ..Z...?.G.......
+00003800: 8f53 7973 7465 6d2e 5765 622e 646c 6c00  .System.Web.dll.
+00003810: 0001 4e23 e2cb 0080 0000 e6e7 1a23 27f3  ..N#.........#'.
+00003820: 4c49 94ec a1a6 803d 461c 5379 7374 656d  LI.....=F.System
+00003830: 2e57 6562 2e48 7474 7055 7469 6c69 7479  .Web.HttpUtility
+00003840: 2e64 6c6c 0000 0131 94f5 db00 8000 007a  .dll...1.......z
+00003850: ac04 a898 e8be 4792 f630 01a8 f4ec c453  ......G..0.....S
+00003860: 7973 7465 6d2e 5769 6e64 6f77 732e 646c  ystem.Windows.dl
+00003870: 6c00 0001 6f48 e4a1 0080 0000 f3d1 e27f  l...oH..........
+00003880: 7302 b54a a4db e65a e300 054e 5379 7374  s..J...Z...NSyst
+00003890: 656d 2e58 6d6c 2e64 6c6c 0000 01d6 1f9e  em.Xml.dll......
+000038a0: c900 a000 008f 30e0 f426 0edf 42a4 a2ad  ......0..&..B...
+000038b0: eeb4 311a c753 7973 7465 6d2e 586d 6c2e  ..1..System.Xml.
+000038c0: 4c69 6e71 2e64 6c6c 0000 01a6 3c94 9f00  Linq.dll....<...
+000038d0: 8000 0057 8590 7147 a8f6 46b3 0f20 8504  ...W..qG..F.. ..
+000038e0: 17ca 0e53 7973 7465 6d2e 586d 6c2e 5265  ...System.Xml.Re
+000038f0: 6164 6572 5772 6974 6572 2e64 6c6c 0000  aderWriter.dll..
+00003900: 0118 5d09 c400 0002 00cc 4d0c 99ac a283  ..].......M.....
+00003910: 4da7 237e 2215 a46b 5553 7973 7465 6d2e  M.#~"..kUSystem.
+00003920: 586d 6c2e 5365 7269 616c 697a 6174 696f  Xml.Serializatio
+00003930: 6e2e 646c 6c00 0001 ba95 f98d 0080 0000  n.dll...........
+00003940: e090 daba 8a7c 774e bbd6 4159 9902 3cf0  .....|wN..AY..<.
+00003950: 5379 7374 656d 2e58 6d6c 2e58 446f 6375  System.Xml.XDocu
+00003960: 6d65 6e74 2e64 6c6c 0000 01e7 a6eb a600  ment.dll........
+00003970: c000 004f c15e 4b58 f36a 4182 97ea 9b66  ...O.^KX.jA....f
+00003980: 8fac 4053 7973 7465 6d2e 586d 6c2e 586d  ..@System.Xml.Xm
+00003990: 6c44 6f63 756d 656e 742e 646c 6c00 0001  lDocument.dll...
+000039a0: 598a 6bbf 0080 0000 a48e 3b4b 693f 6544  Y.k.......;Ki?eD
+000039b0: 9260 55b3 fc15 0f6b 5379 7374 656d 2e58  .`U....kSystem.X
+000039c0: 6d6c 2e58 6d6c 5365 7269 616c 697a 6572  ml.XmlSerializer
+000039d0: 2e64 6c6c 0000 0154 3213 e500 0001 00d7  .dll...T2.......
+000039e0: 2bb6 9ceb 003d 488b 5a6d baac 634c 1d53  +....=H.Zm..cL.S
+000039f0: 7973 7465 6d2e 586d 6c2e 5850 6174 682e  ystem.Xml.XPath.
+00003a00: 646c 6c00 0001 7d58 6acd 0080 0000 b5ae  dll...}Xj.......
+00003a10: a120 b4fc aa4d b1b1 b538 b71e 8822 5379  . ...M...8..."Sy
+00003a20: 7374 656d 2e58 6d6c 2e58 5061 7468 2e58  stem.Xml.XPath.X
+00003a30: 446f 6375 6d65 6e74 2e64 6c6c 0000 0183  Document.dll....
+00003a40: 736c c600 8000 0058 b7df 8d54 8252 4a8a  sl.....X...T.RJ.
+00003a50: 97c7 8e66 9354 a555 6e64 6572 7461 6c65  ...f.T.Undertale
+00003a60: 4d6f 644c 6962 2e64 6c6c 0000 019b f66e  ModLib.dll.....n
+00003a70: ff00 2003 0090 9cab 0b12 8da2 418c 4e3a  .. .........A.N:
+00003a80: 2c98 30b2 3357 696e 646f 7773 4261 7365  ,.0.3WindowsBase
+00003a90: 2e64 6c6c 0000 0114 1787 b000 8000 003c  .dll...........<
+00003aa0: 440f c83d 91f4 4796 13af 540a 1d28 c015  D..=..G...T..(..
+00003ab0: 0100 0046 0f09 1000 1502 0003 000a 002c  ...F...........,
+00003ac0: 0600 3d04 5514 5369 784c 6162 6f72 732e  ..=.U.SixLabors.
+00003ad0: 496d 6167 6553 6861 7270 2153 6978 4c61  ImageSharp!SixLa
+00003ae0: 626f 7273 2e49 6d61 6765 5368 6172 702e  bors.ImageSharp.
+00003af0: 5069 7865 6c46 6f72 6d61 7473 1f53 6978  PixelFormats.Six
+00003b00: 4c61 626f 7273 2e49 6d61 6765 5368 6172  Labors.ImageShar
+00003b10: 702e 5072 6f63 6573 7369 6e67 0653 7973  p.Processing.Sys
+00003b20: 7465 6d1a 5379 7374 656d 2e43 6f6c 6c65  tem.System.Colle
+00003b30: 6374 696f 6e73 2e47 656e 6572 6963 0953  ctions.Generic.S
+00003b40: 7973 7465 6d2e 494f 0b53 7973 7465 6d2e  ystem.IO.System.
+00003b50: 4c69 6e71 0f53 7973 7465 6d2e 4e65 742e  Linq.System.Net.
+00003b60: 4874 7470 1053 7973 7465 6d2e 5468 7265  Http.System.Thre
+00003b70: 6164 696e 6716 5379 7374 656d 2e54 6872  ading.System.Thr
+00003b80: 6561 6469 6e67 2e54 6173 6b73 1453 7973  eading.Tasks.Sys
+00003b90: 7465 6d2e 476c 6f62 616c 697a 6174 696f  tem.Globalizatio
+00003ba0: 6e11 5379 7374 656d 2e52 6566 6c65 6374  n.System.Reflect
+00003bb0: 696f 6e10 5379 7374 656d 2e54 6578 742e  ion.System.Text.
+00003bc0: 4a73 6f6e 0f55 6e64 6572 7461 6c65 4d6f  Json.UndertaleMo
+00003bd0: 644c 6962 1a55 6e64 6572 7461 6c65 4d6f  dLib.UndertaleMo
+00003be0: 644c 6962 2e44 6563 6f6d 7069 6c65 7216  dLib.Decompiler.
+00003bf0: 556e 6465 7274 616c 654d 6f64 4c69 622e  UndertaleModLib.
+00003c00: 4d6f 6465 6c73 2053 6978 4c61 626f 7273  Models SixLabors
+00003c10: 2e49 6d61 6765 5368 6172 702e 466f 726d  .ImageSharp.Form
+00003c20: 6174 732e 506e 6733 01a7 9501 a7aa 01a7  ats.Png3........
+00003c30: cc01 a7ec 01a7 f301 a80e 01a8 1801 a824  ...............$
+00003c40: 01a8 3401 a845 01a8 5c01 a871 01a8 8301  ..4..E..\..q....
+00003c50: a894 01a8 a401 a8bf 01a8 d694 d602 0000  ................
+00003c60: 0006 003a 2009 0a00 5404 000d 0021 1600  ...: ...T....!..
+00003c70: 0b00 3104 0e0d 001e 047b 1000 0102 7902  ..1......{....y.
+00003c80: 0000 0b00 0001 0041 0200 1200 4b80 8a00  .......A....K...
+00003c90: 0b00 1104 0007 000d 0026 0700 1600 1e07  .........&......
+00003ca0: 0045 023d 1500 3302 000b 0049 0200 2000  .E.=..3....I.. .
+00003cb0: 2b02 0016 0063 5400 1f00 1b02 0e07 002c  +....cT........,
+00003cc0: 047b 1200 6202 001d 0001 0279 0200 000b  .{..b......y....
+00003cd0: 0000 0100 0007 004a 0808 2700 4c02 0027  .......J..'.L..'
+00003ce0: 0080 8602 0019 003d 0200 2200 4802 0022  .......=..".H.."
+00003cf0: 0064 0200 1400 1b02 0e07 0029 047b 0e00  .d.........).{..
+00003d00: 3902 001d 0001 0279 0200 000b 0000 0100  9......y........
+00003d10: 4c04 0027 004e 0200 2700 808b 0200 1900  L..'.N..'.......
+00003d20: 3f02 0022 004a 0200 2200 6802 0014 001b  ?..".J..".h.....
+00003d30: 020e 0700 2a04 7b0e 003a 0200 1d00 0102  ....*.{..:......
+00003d40: 7902 0000 0b00 0001 0072 0679 3b00 7802  y........r.y;.x.
+00003d50: 003b 0078 0200 3b00 7e02 003b 006b 0200  .;.x..;.~..;.k..
+00003d60: 3b00 80a6 0200 5600 80a6 0200 5600 80a6  ;.....V.....V...
+00003d70: 0200 5600 80a6 0200 5600 80a6 0200 5600  ..V.....V.....V.
+00003d80: 80a6 0200 5600 80a6 0200 5600 80ae 0400  ....V.....V.....
+00003d90: 5600 80bc 0200 5600 80b4 0200 5600 80b2  V.....V.....V...
+00003da0: 0200 5600 809d 0600 4b00 809f 0200 4b00  ..V.....K.....K.
+00003db0: 8099 0200 4b00 7506 0046 0078 0200 4600  ....K.u..F.x..F.
+00003dc0: 7602 0046 0076 0200 4600 7702 0046 0080  v..F.v..F.w..F..
+00003dd0: a206 004b 0080 a002 004b 0080 a202 004b  ...K.....K.....K
+00003de0: 0080 a202 004b 0080 9f02 004b 0080 9c02  .....K.....K....
+00003df0: 004b 0080 9e02 004b 0080 9d02 004b 0080  .K.....K.....K..
+00003e00: a402 004b 0080 9e02 004b 0080 a002 004b  ...K.....K.....K
+00003e10: 0080 a002 004b 0080 9e02 004b 0080 9e02  .....K.....K....
+00003e20: 004b 0080 9f02 004b 0080 9d02 004b 0080  .K.....K.....K..
+00003e30: a402 004b 0080 9d02 004b 0080 9d02 004b  ...K.....K.....K
+00003e40: 0080 9d02 004b 0032 0600 2000 8099 0200  .....K.2.. .....
+00003e50: 4b00 8099 0200 4b00 8099 0200 4b00 8099  K.....K.....K...
+00003e60: 0200 4b00 8099 0200 4b00 8099 0200 4b00  ..K.....K.....K.
+00003e70: 8099 0200 4b00 8099 0200 4b00 8099 0200  ....K.....K.....
+00003e80: 4b0b 0604 0081 450b 061a 0081 370e 061a  K.....E.....7...
+00003e90: 0082 0f18 0620 0084 2b0b 0634 0081 450b  ..... ..+..4..E.
+00003ea0: 061a 0081 4500 391a 0020 0080 a602 004b  ....E.9.. .....K
+00003eb0: 0080 a602 004b 0080 a602 004b 0080 a602  .....K.....K....
+00003ec0: 004b 0039 0400 2000 80a6 0200 4b00 80a6  .K.9.. .....K...
+00003ed0: 0200 4b00 80a6 0200 4b00 80a6 0200 4b00  ..K.....K.....K.
+00003ee0: 80a6 0200 4b00 80a6 0200 4b00 80a6 0200  ....K.....K.....
+00003ef0: 4b00 80a6 0200 4b00 80a6 0200 4b00 80a7  K.....K.....K...
+00003f00: 0200 4b00 80a7 0200 4b00 80a7 0200 4b00  ..K.....K.....K.
+00003f10: 80a7 0200 4b00 80a7 0200 4b00 80a7 0200  ....K.....K.....
+00003f20: 4b00 80a7 0200 4b0a 0604 0081 1637 0618  K.....K......7..
+00003f30: 008a 9612 0672 0082 e712 0628 0082 e712  .....r.....(....
+00003f40: 0628 0082 e70f 0628 0082 450a 0624 0081  .(.....(..E..$..
+00003f50: 4705 0480 8400 4500 790c 0021 0056 0200  G.....E.y..!.V..
+00003f60: 0c00 2502 0011 0037 0200 0c00 4002 0007  ..%....7....@...
+00003f70: 0031 0200 0800 3902 0007 0024 0200 0800  .1....9....$....
+00003f80: 3402 000e 0030 0200 0700 7502 0022 0075  4....0....u..".u
+00003f90: 0200 0d00 2302 0012 0035 0200 0c00 3c02  ....#....5....<.
+00003fa0: 0007 002f 0200 0900 3502 0007 0024 0200  .../....5....$..
+00003fb0: 0800 3402 000e 002e 0200 0700 2702 0011  ..4.........'...
+00003fc0: 004d 0400 1800 3406 001c 0035 0200 1d00  .M....4....5....
+00003fd0: 4f06 0018 0057 0200 1301 80d2 0200 2700  O....W........'.
+00003fe0: 4808 0018 005f 0200 0d00 5902 0021 0056  H...._....Y..!.V
+00003ff0: 0600 2100 8090 0600 2702 80a6 0600 2700  ..!.....'.....'.
+00004000: 809e 0a00 2700 3c06 0018 0080 8a02 0013  ....'.<.........
+00004010: 0080 8202 0013 0080 8402 0013 007f 0200  ................
+00004020: 1300 5e02 2a2a 0000 0200 0800 6907 0048  ..^.**......i..H
+00004030: 0477 2400 4802 0024 0000 0600 027b 1c08  .w$.H..$.....{..
+00004040: 0180 9a0e 5d27 0068 0600 2700 5906 0021  ....]'.h..'.Y..!
+00004050: 0080 8502 0027 0074 0600 2100 7402 0021  .....'.t..!.t..!
+00004060: 0074 0200 2100 7402 0021 004c 0632 1b00  .t..!.t..!.L.2..
+00004070: 0002 000c 0061 0700 3d02 771e 0000 0600  .....a..=.w.....
+00004080: 027f 2408 002d 0855 1200 6802 0827 0180  ..$..-.U..h..'..
+00004090: da06 7921 0069 0400 2100 7706 0027 007e  ..y!.i..!.w..'.~
+000040a0: 0200 2700 7502 0027 0363 0632 6600 0002  ..'.u..'.c.2f...
+000040b0: 000c 0061 0700 3408 771e 0000 0600 0279  ...a..4.w......y
+000040c0: 2408 0080 900a 5521 0380 e406 0027 0072  $.....U!.....'.r
+000040d0: 0e00 2700 2d02 0007 0057 0200 1c02 6e02  ..'.-....W....n.
+000040e0: 000d 0024 0600 1200 4502 0021 003a 0200  ...$....E..!.:..
+000040f0: 0700 2a02 0009 0033 0200 0700 2002 000c  ..*....3.... ...
+00004100: 0028 0200 0e00 2402 0007 0680 8808 0007  .(....$.........
+00004110: 0080 8e10 322b 0000 0200 0c00 6107 0054  ....2+......a..T
+00004120: 0277 2100 0006 0002 7f24 0800 290a 5507  .w!......$..).U.
+00004130: 005b 022e 1700 0002 000a 0065 0700 2e04  .[.........e....
+00004140: 770f 0031 0208 2f00 0006 0002 7b18 0804  w..1../.....{...
+00004150: 8090 0a59 3304 8086 0a00 3300 250c 0007  ...Y3.....3.%...
+00004160: 001b 022e 1b00 0002 000a 0065 0700 2e04  ...........e....
+00004170: 770f 002d 0208 2f00 0006 0002 7b18 0804  w..-../.....{...
+00004180: 8088 0a59 3304 7e0a 0033 0061 1400 2700  ...Y3.~..3.a..'.
+00004190: 4f06 0021 0055 0632 1b00 0002 000c 0061  O..!.U.2.......a
+000041a0: 0700 7c02 7724 0000 0600 027f 2408 0071  ..|.w$......$..q
+000041b0: 0c55 2200 7402 0022 0021 0200 1200 2202  .U".t..".!....".
+000041c0: 0012 0906 0200 7a09 0614 007d 0078 1800  ......z....}.x..
+000041d0: 2200 2402 0012 002f 0200 1609 0602 0065  ".$..../.......e
+000041e0: 0043 1600 2c00 1002 0009 0036 0200 1800  .C..,......6....
+000041f0: 2c02 0009 0017 0200 0900 1602 0009 003f  ,..............?
+00004200: 0400 2c00 1002 0009 002c 0200 0900 1702  ..,......,......
+00004210: 0009 0016 0200 0900 3f04 002c 0010 0200  ........?..,....
+00004220: 0900 2c02 0009 0017 0200 0900 1602 0009  ..,.............
+00004230: 003f 0400 2c00 1002 0009 002c 0200 0900  .?..,......,....
+00004240: 1702 0009 0015 0200 080a 0404 0065 001d  .............e..
+00004250: 1600 0d0a 0404 0065 001d 1600 0d0a 0404  .......e........
+00004260: 0062 001d 1600 0d0a 0404 0061 001d 1600  .b.........a....
+00004270: 0c00 3506 0018 000b 020a 0700 0005 0023  ..5............#
+00004280: 047f 0700 3502 0028 001a 0200 0900 2104  ....5..(......!.
+00004290: 0007 004d 0200 4900 4402 001e 0018 0200  ...M..I.D.......
+000042a0: 1200 2302 000d 0033 0200 0700 1702 0009  ..#....3........
+000042b0: 002d 0200 0700 1b02 000e 001c 0200 0700  .-..............
+000042c0: 2404 0007 0055 0200 4900 1b02 0012 0026  $....U..I......&
+000042d0: 0200 0d00 2f02 0007 001a 0200 0900 2902  ..../.........).
+000042e0: 0007 001a 0200 0c00 1b02 000e 001f 0200  ................
+000042f0: 0700 1b02 0012 0003 4b30 0600 0800 6d0c  ........K0....m.
+00004300: 0e12 3e5d 1300 501e 0027 0050 0200 2700  ..>]..P..'.P..'.
+00004310: 2606 0007 0048 0200 1c5d 1202 000d 001d  &....H...]......
+00004320: 80bc 0012 0071 0200 3801 817a 0600 1301  .....q..8..z....
+00004330: 817a 0400 1300 80aa 082a 3300 0002 0008  .z.......*3.....
+00004340: 0069 0700 3c02 7724 0000 0600 027f 1c08  .i..<.w$........
+00004350: 0080 ef08 0c3b 0000 0200 0b00 6307 0063  .....;......c..c
+00004360: 0277 2400 0006 0002 7f22 0800 3c08 5718  .w$......"..<.W.
+00004370: 0043 0200 1300 4802 0013 0080 9302 0027  .C....H........'
+00004380: 0080 9302 0027 0168 0200 2700 5404 0018  .....'.h..'.T...
+00004390: 0072 0200 1300 7002 0013 0080 8902 0013  .r....p.........
+000043a0: 0080 af02 0013 0080 8d02 0013 006e 0200  .............n..
+000043b0: 2700 2106 0010 0036 0608 1800 4b02 0018  '.!....6....K...
+000043c0: 004b 0200 1800 4902 0018 004a 0200 1800  .K....I....J....
+000043d0: 3d02 0018 0037 0200 1800 3f02 0018 005c  =....7....?....\
+000043e0: 0200 3100 5502 0031 0056 0200 3200 5502  ..1.U..1.V..2.U.
+000043f0: 0031 0055 0200 3100 5602 0032 0056 0200  .1.U..1.V..2.V..
+00004400: 3200 5602 0032 0056 0200 2e00 5204 002b  2.V..2.V....R..+
+00004410: 0049 0200 2b00 5202 002b 0072 0400 2200  .I..+.R..+.r..".
+00004420: 6602 000d 0021 0200 1200 5902 002c 0069  f....!....Y..,.i
+00004430: 0200 1200 3306 0018 0060 0200 3100 5802  ....3....`..1.X.
+00004440: 0030 005a 0200 3200 5902 0031 005a 0200  .0.Z..2.Y..1.Z..
+00004450: 3200 5902 0031 005a 0200 3200 5a02 0032  2.Y..1.Z..2.Z..2
+00004460: 004f 0600 2b00 4602 002b 004f 0200 2b00  .O..+.F..+.O..+.
+00004470: 4604 0012 006f 0400 2200 6402 000d 001e  F....o..".d.....
+00004480: 0200 1200 5302 002c 005d 0600 3200 3508  ....S..,.]..2.5.
+00004490: 0018 005d 0200 2e00 5602 002e 0057 0200  ...]....V....W..
+000044a0: 2f00 5702 002e 0056 0200 2e00 5702 002f  /.W....V....W../
+000044b0: 0057 0200 2f00 5802 002f 0057 0800 3800  .W../.X../.W..8.
+000044c0: 5602 0038 005e 0200 3200 5004 0028 0047  V..8.^..2.P..(.G
+000044d0: 0200 2800 5002 0028 0049 0400 1200 7104  ..(.P..(.I....q.
+000044e0: 0022 0066 0200 0d00 2002 0012 0056 0200  .".f.... ....V..
+000044f0: 2900 3906 0018 0062 0200 3100 5a02 0030  ).9....b..1.Z..0
+00004500: 005c 0200 3200 5b02 0031 005c 0200 3200  .\..2.[..1.\..2.
+00004510: 5b02 0031 005c 0200 3200 5c02 0032 005f  [..1.\..2.\..2._
+00004520: 0800 3800 5f02 0038 005f 0200 3800 5f02  ..8._..8._..8._.
+00004530: 0038 006f 0200 4500 5504 002b 004c 0200  .8.o..E.U..+.L..
+00004540: 2b00 5502 002b 0075 0400 2200 6802 000d  +.U..+.u..".h...
+00004550: 0024 0200 1200 5f02 002c 004a 0400 1200  .$...._..,.J....
+00004560: 8089 0600 2700 8089 0200 2700 8087 0200  ....'.....'.....
+00004570: 2700 8089 0200 2701 816c 1e79 2701 816c  '.....'..l.y'..l
+00004580: 0400 2701 816c 0400 2701 816c 0400 2700  ..'..l..'..l..'.
+00004590: 80ba 0800 2100 3006 0016 002e 0200 0700  ....!.0.........
+000045a0: 1002 0009 0010 0200 0900 1402 000c 0014  ................
+000045b0: 0200 0c00 3302 0025 0041 0200 1d00 2702  ....3..%.A....'.
+000045c0: 0007 0056 0200 1c00 6f02 000d 001e 0200  ...V....o.......
+000045d0: 1200 2502 0009 0023 0200 0d0b 0602 0080  ..%....#........
+000045e0: 8a0b 0618 0080 8c00 7c1c 0027 0280 9806  ........|..'....
+000045f0: 004d 003f 0a00 1800 6302 0013 0070 0600  .M.?....c....p..
+00004600: 1300 5c06 0027 005c 0200 2701 8094 0600  ..\..'.\..'.....
+00004610: 2701 812c 0e00 0d00 6d0c 0013 0080 8102  '..,....m.......
+00004620: 0013 0055 0200 1300 6a02 0013 004f 0200  ...U....j....O..
+00004630: 1300 6102 0013 0068 0200 1300 4606 0018  ..a....h....F...
+00004640: 0281 5602 0013 0041 0600 1800 6902 0013  ..V....A....i...
+00004650: 087b 0800 1308 7b12 0013 087b 1600 1308  .{....{....{....
+00004660: 7b12 0013 087b 1600 1308 7b12 0013 0047  {....{....{....G
+00004670: 1600 1800 8096 0200 1300 80b5 0200 1309  ................
+00004680: 1206 0013 005a 1400 1301 80e8 0e00 0d00  .....Z..........
+00004690: 3c08 000d 006b 0600 0d00 8080 0600 2600  <....k........&.
+000046a0: 8084 0200 2c01 8104 0600 0d01 80ce 0800  ....,...........
+000046b0: 0d00 5904 0018 087b 0200 1300 7912 0013  ..Y....{....y...
+000046c0: 0063 0400 1808 7b02 0013 0080 8312 0013  .c....{.........
+000046d0: 0059 0400 1808 7b02 0013 0079 1200 1300  .Y....{....y....
+000046e0: 5a04 0018 087b 0200 1300 7612 0013 0281  Z....{....v.....
+000046f0: 4c06 000d 1e1a 0a00 1301 8100 3e00 1300  L...........>...
+00004700: 7b08 0027 004f 0600 1800 4f02 0013 004e  {..'.O....O....N
+00004710: 0200 1800 4802 0013 036b 0428 4b00 0002  ....H....k.(K...
+00004720: 0008 0069 0700 5008 7924 0000 0600 0279  ...i..P.y$.....y
+00004730: 1a08 003e 0a5f 1c00 0c02 3e12 0000 0200  ...>._....>.....
+00004740: 1200 5507 0060 0446 3200 0002 001b 0043  ..U..`.F2......C
+00004750: 0900 4d02 7718 0002 7f42 0b00 000b 0000  ..M.w....B......
+00004760: 0100 027d 670b 0000 0b00 0001 004c 1049  ...}g........L.I
+00004770: 1300 5302 0013 004d 0600 1300 5402 0013  ..S....M....T...
+00004780: 0180 8402 3e36 0000 0200 1200 5509 0041  ....>6......U..A
+00004790: 0477 1300 027d 300b 0000 0b00 0001 004b  .w...}0........K
+000047a0: 0a49 1300 5202 0013 0076 0200 2700 5006  .I..R....v..'.P.
+000047b0: 0018 004a 0200 1300 5002 0013 0181 3a02  ...J....P.....:.
+000047c0: 2836 0000 0200 0800 6909 003d 0479 1300  (6......i..=.y..
+000047d0: 027d 1a0b 0000 0b00 0001 004f 0a5f 1800  .}.........O._..
+000047e0: 4902 0013 004f 0200 1300 8088 0228 2b00  I....O.......(+.
+000047f0: 0002 0008 0069 0700 5002 7924 0000 0600  .....i..P.y$....
+00004800: 027f 1a08 004d 085f 1300 5302 0013 0280  .....M._..S.....
+00004810: 9602 2836 0000 0200 0800 6909 0046 0679  ..(6......i..F.y
+00004820: 1300 027b 1a0b 0000 0b00 0001 0050 0c5f  ...{.........P._
+00004830: 1300 5602 0013 0180 d602 2836 0000 0200  ..V.......(6....
+00004840: 0800 6909 0049 0479 1300 027d 1a0b 0000  ..i..I.y...}....
+00004850: 0b00 0001 004e 0c5f 1300 5502 0013 056b  .....N._..U....k
+00004860: 0228 809c 0000 0200 0800 6907 0056 0c79  .(........i..V.y
+00004870: 2400 0006 0002 751a 0800 4b14 5f13 0051  $.....u...K._..Q
+00004880: 0200 1304 6b04 2880 8a00 0002 0008 0069  ....k.(........i
+00004890: 0700 520a 7924 0000 0600 0277 1a08 004a  ..R.y$.....w...J
+000048a0: 105f 1800 4802 0013 0050 0200 1300 4806  ._..H....P....H.
+000048b0: 0013 0050 0200 1300 8089 0228 2b00 0002  ...P.......(+...
+000048c0: 0008 0069 0700 5702 7924 0000 0600 027f  ...i..W.y$......
+000048d0: 1a08 0048 085f 1300 5002 0013 0048 0600  ...H._..P....H..
+000048e0: 1300 5002 0013 0048 0600 1300 5002 0013  ..P....H....P...
+000048f0: 081a 0600 1308 1a12 0013 081a 1200 1312  ................
+00004900: 1a12 0013 0812 2800 1300 7e16 0061 0067  ......(...~..a.g
+00004910: 0600 2700 6602 0021 0060 0200 2100 3a06  ..'.f..!.`..!.:.
+00004920: 2a36 0000 0200 0800 6909 0041 0277 1200  *6......i..A.w..
+00004930: 027f 1c0b 0000 0b00 0001 0040 085d 0d00  ...........@.]..
+00004940: 4302 0018 0480 ca02 0013 1012 0e00 2100  C.............!.
+00004950: 6f22 0027 0712 0200 2127 1210 0027 0712  o".'....!'...'..
+00004960: 5000 2100 6810 0021 0812 0200 2100 2a16  P.!.h..!....!.*.
+00004970: 0007 0052 0200 1c2d 1202 000d 0021 5c00  ...R...-.....!\.
+00004980: 1200 7b02 0038 002a 0400 0700 5202 001c  ..{..8.*....R...
+00004990: 2612 0200 0d00 214e 0012 007a 0200 3800  &.....!N...z..8.
+000049a0: 3804 0018 0080 8102 0013 002e 0200 1300  8...............
+000049b0: 3802 0013 0038 0400 1800 2e02 0013 0075  8....8.........u
+000049c0: 0200 1300 7202 0013 0d1a 0200 1300 7720  ....r.........w 
+000049d0: 0061 0460 0200 1300 4710 0018 0035 0200  .a.`....G....5..
+000049e0: 1300 7c02 0013 006c 042a 2b00 0002 0008  ..|....l.*+.....
+000049f0: 0069 0700 3f02 7724 0000 0600 027f 1c08  .i..?.w$........
+00004a00: 0040 085d 2500 4402 0025 0080 8006 004b  .@.]%.D..%.....K
+00004a10: 0080 9d02 003d 0018 064a 0d00 0005 0018  .....=...J......
+00004a20: 0049 1a00 0d04 7702 0000 808e 0059 0610  .I....w......Y..
+00004a30: 4001 80ec 0200 8086 0006 0400 0500 5d04  @.............].
+00004a40: 0040 0006 0200 0500 5f04 0040 0006 0200  .@......_..@....
+00004a50: 0500 5904 0040 0006 0200 0500 0004 0023  ..Y..@.........#
+00004a60: 1a0e 1c00 4802 7313 0006 0200 0500 5d06  ....H.s.......].
+00004a70: 0040 0006 0200 0500 6504 0040 0006 0200  .@......e..@....
+00004a80: 0500 6704 0040 0006 0200 0500 6304 0040  ..g..@......c..@
+00004a90: 0006 0200 0500 5f04 0040 0006 0200 0500  ......_..@......
+00004aa0: 5d04 0040 0006 0200 0500 6504 0040 0006  ]..@......e..@..
+00004ab0: 0200 0500 6b04 0040 0006 0200 0500 6904  ....k..@......i.
+00004ac0: 0040 0006 0200 0500 6104 0040 0006 0200  .@......a..@....
+00004ad0: 0500 5d0a 0040 0006 0200 0500 5d04 0040  ..]..@......]..@
+00004ae0: 0006 0200 0500 5d04 0040 0006 0200 0500  ......]..@......
+00004af0: 5d04 0040 0006 0200 0500 5d04 0040 0006  ]..@......]..@..
+00004b00: 0200 0200 5d04 0040 0006 0200 0200 2808  ....]..@......(.
+00004b10: 0006 0002 bf51 2c0e 0000 0e00 7180 ba3d  .....Q,.....q..=
+00004b20: 1c00 6002 0813 0074 0279 1c00 6202 0813  ..`....t.y..b...
+00004b30: 006a 0279 1c00 5c02 0813 0080 8006 793d  .j.y..\.......y=
+00004b40: 007a 0200 3d08 1206 0027 0062 1200 2701  .z..=....'.b..'.
+00004b50: 8172 0800 270e 120a 0013 0051 1e00 2700  .r..'......Q..'.
+00004b60: 5102 0027 0032 0600 1800 0c02 2a12 0000  Q..'.2......*...
+00004b70: 0200 0800 6907 0052 0420 3000 0002 0008  ....i..R. 0.....
+00004b80: 0069 0700 1f04 7707 0002 7d1c 0b00 000b  .i....w...}.....
+00004b90: 0000 0100 027d 790b 0000 0b00 0001 0013  .....}y.........
+00004ba0: 105d 0900 1906 0007 0014 0246 0d00 0005  .].........F....
+00004bb0: 0016 004d 1c00 1304 7703 000c 022a 1200  ...M....w....*..
+00004bc0: 0005 0008 0069 0900 1004 2c0e 0000 0500  .....i....,.....
+00004bd0: 0e00 5d09 0020 0477 0e00 4204 001d 0055  ..].. .w..B....U
+00004be0: 0208 3800 0d04 7903 0024 0200 0c00 7304  ..8...y..$....s.
+00004bf0: 086e 0016 0200 1200 1f02 0009 1c04 0679  .n.............y
+00004c00: 7900 1704 360c 003b 0202 3900 3b02 0a39  y...6..;..9.;..9
+00004c10: 003b 0273 3900 2d02 020c 002d 0200 0c00  .;.s9.-....-....
+00004c20: 2d02 7d0c 002d 0204 0c00 2d02 000c 002d  -.}..-....-....-
+00004c30: 027b 0c00 2d02 020c 002d 0204 0c00 2d02  .{..-....-....-.
+00004c40: 7f0c 002d 020e 0c00 2d02 7d0c 002d 0204  ...-....-.}..-..
+00004c50: 0c00 2d02 000c 002d 027d 0c00 2d02 000c  ..-....-.}..-...
+00004c60: 002d 0202 0900 2d02 7d09 002d 0206 0900  .-....-.}..-....
+00004c70: 2d02 7309 002d 0200 0900 2d02 0009 005d  -.s..-....-....]
+00004c80: 025f 5200 0004 0033 066f 0f00 1102 0006  ._R....3.o......
+00004c90: 0006 0200 0200 0223 280e 0000 0b00 0001  .......#(.......
+00004ca0: 000a 6451 0400 0600 1602 0002 1906 0e00  ..dQ............
+00004cb0: 000b 0000 0100 0b6e 5d04 0043 0208 3800  .......n]..C..8.
+00004cc0: 020b 300e 0000 0e00 1880 8024 0d00 0005  ..0........$....
+00004cd0: 0025 002f 1c00 3504 7715 0043 0200 2400  .%./..5.w..C..$.
+00004ce0: 1c02 0009 006a 0208 5700 3904 7925 0180  .....j..W.9.y%..
+00004cf0: 8802 0080 8e00 3c08 0025 3f04 0200 80a3  ......<..%?.....
+00004d00: 0022 0436 0c00 1f02 0c0c 0181 0002 7f0c  .".6............
+00004d10: 0024 040c 0c01 810a 027f 0c00 2104 730c  .$..........!.s.
+00004d20: 0180 ec02 000c 0000 0400 2304 591c 0045  ..........#.Y..E
+00004d30: 004e 0c00 6202 4b0c 0055 0206 0c00 6c02  .N..b.K..U....l.
+00004d40: 040c 0069 0200 0c00 8085 0202 0c10 6b02  ...i..........k.
+00004d50: 750c 007f 2208 0900 5902 0609 004d 0275  u..."...Y....M.u
+00004d60: 0910 6702 0209 0061 227f 0900 4b02 7b09  ..g....a"...K.{.
+00004d70: 004b 0202 0900 4b02 0409 004b 0200 0900  .K....K....K....
+00004d80: 4f02 0609 0014 027d 0900 4902 6322 0000  O......}..I.c"..
+00004d90: 0400 3404 6f0a 0002 bf67 560e 0000 0e07  ..4.o....gV.....
+00004da0: 7b80 a223 7107 7b12 0071 077b 1200 7100  {..#q.{..q.{..q.
+00004db0: 5616 002c 0181 2002 0876 005b 0679 2c01  V..,.. ..v.[.y,.
+00004dc0: 812c 0208 7600 5406 792c 0181 1802 0876  .,..v.T.y,.....v
+00004dd0: 0712 0a79 809b 0046 1600 0e00 4402 000d  ...y...F....D...
+00004de0: 0049 0200 0d00 5802 000e 1312 0200 80a2  .I....X.........
+00004df0: 0026 2c00 0d00 5e02 0813 004d 0222 3600  .&,...^....M."6.
+00004e00: 0002 0008 0069 0900 4302 770d 0002 7f1c  .....i..C.w.....
+00004e10: 0b00 000b 0000 0100 0c06 1a12 0000 0200  ................
+00004e20: 1200 5507 0060 0446 3200 0002 001b 0043  ..U..`.F2......C
+00004e30: 0901 6c02 7718 0002 7f42 0b00 000b 0000  ..l.w....B......
+00004e40: 0100 027d 670b 0000 0b00 0001 0150 0c49  ...}g........P.I
+00004e50: 2700 270c 000d 0060 0208 1300 80ca 042a  '.'....`.......*
+00004e60: 4300 0002 000c 0061 0700 7702 771e 0000  C......a..w.w...
+00004e70: 0600 027f 2408 000a 065f 0400 0002 007f  ....$...._......
+00004e80: 027f 4e00 037f 2c06 0007 006f 0600 2808  ..N...,....o..(.
+00004e90: 5f0d 0051 0208 1301 3802 7927 002a 0800  _..Q....8.y'.*..
+00004ea0: 0d00 6702 0813 2912 0679 2700 6858 3646  ..g...)..y'.hX6F
+00004eb0: 0000 0200 0e00 5d09 0017 0677 0b03 1202  ......]....w....
+00004ec0: 0818 0017 0c79 0b00 5f02 0812 0002 6b20  .....y.._.....k 
+00004ed0: 0b00 000b 0000 0100 681e 0646 0000 0200  ........h..F....
+00004ee0: 0e00 5d09 002d 0477 1601 4202 0818 0002  ..]..-.w..B.....
+00004ef0: 7b20 0b00 000b 0000 0100 6710 0646 0000  { ........g..F..
+00004f00: 0200 0e00 5d09 0142 0477 1800 027d 280b  ....]..B.w...}(.
+00004f10: 0000 0b00 0001 0067 0e06 4600 0002 000e  .......g..F.....
+00004f20: 005d 0900 2e04 7716 0142 0208 1800 027b  .]....w..B.....{
+00004f30: 200b 0000 0b00 0001 006c 0e06 4600 0002   ........l..F...
+00004f40: 000e 005d 0900 1706 770b 0412 0208 1800  ...]....w.......
+00004f50: 180e 790e 005f 0208 1200 0269 200b 0000  ..y.._.....i ...
+00004f60: 0b00 0001 004c 2208 1b00 0002 000f 005b  .....L"........[
+00004f70: 0700 8087 0277 2400 0006 0002 7f2a 0801  .....w$......*..
+00004f80: 2408 4f27 0124 0400 2700 809b 0800 2100  $.O'.$..'.....!.
+00004f90: 2906 000d 0064 0208 1300 0c02 3612 0000  )....d......6...
+00004fa0: 0500 1200 5509 0010 041c 0e00 0005 0006  ....U...........
+00004fb0: 006d 0900 5a06 7731 001c 0400 0c00 8088  .m..Z.w1........
+00004fc0: 0408 6700 1602 0012 0017 0200 0900 5204  ..g...........R.
+00004fd0: 7912 0002 6b18 0e00 000b 0000 0100 027d  y...k..........}
+00004fe0: 100e 0000 0b00 0001 005d 2649 2700 5f02  .........]&I'._.
+00004ff0: 0027 0029 0600 0d00 5d02 0813 1412 0279  .'.)....]......y
+00005000: 2707 1a2c 0027 0080 af12 0027 0080 af02  '..,.'.....'....
+00005010: 0027 0180 ce0a 0021 0025 0800 0d00 5c04  .'.....!.%....\.
+00005020: 0813 0061 0879 2100 4d04 000d 0b12 0400  ...a.y!.M.......
+00005030: 2100 4f1a 000d 004f 0400 0d00 4f04 000d  !.O....O....O...
+00005040: 1912 0400 2100 5336 000d 0081 3b04 0021  ....!.S6....;..!
+00005050: 0081 3804 0021 005d 0400 2100 1614 520d  ..8..!.]..!...R.
+00005060: 0000 0200 1c00 411a 0020 0477 0700 2802  ......A.. .w..(.
+00005070: 0009 002f 0400 1500 4602 001e 0002 7544  .../....F.....uD
+00005080: 0b00 000e 0080 9014 3557 0512 0600 7800  ........5W....x.
+00005090: 691a 0027 0080 a804 0027 0080 ae04 0038  i..'.....'.....8
+000050a0: 0080 8f04 0027 005f 0a00 2700 5f02 0027  .....'._..'._..'
+000050b0: 1412 0400 2106 122c 0027 0712 1000 2704  ....!..,.'....'.
+000050c0: 1212 0027 0612 0c00 271d 120e 0027 1712  ...'....'....'..
+000050d0: 3e00 85f4 005c 3600 3b00 6f02 0021 005c  >....\6.;.o..!.\
+000050e0: 0400 3e00 6f02 0021 005c 0400 3b00 6f02  ..>.o..!.\..;.o.
+000050f0: 0021 005c 0400 3e00 6f02 0021 005b 0400  .!.\..>.o..!.[..
+00005100: 3b00 6e02 0021 005c 0400 3e00 6f02 0021  ;.n..!.\..>.o..!
+00005110: 005c 0400 3e00 6f02 0021 0038 0e0e 0d00  .\..>.o..!.8....
+00005120: 3104 7b28 0001 0279 0200 000b 0000 0100  1.{(...y........
+00005130: 0102 7905 0980 1a06 0005 0981 1a06 0005  ..y.............
+00005140: 0982 1a06 0005 0800 0400 0006 0000 0035  ...............5
+00005150: 1505 1500 0000 5f17 050b 0059 0800 0b00  ......_....Y....
+00005160: 5108 000b 004f 1000 2553 7973 7465 6d2e  Q....O..%System.
+00005170: 436f 6d70 6f6e 656e 744d 6f64 656c 2e44  ComponentModel.D
+00005180: 6174 6141 6e6e 6f74 6174 696f 6e73 1c53  ataAnnotations.S
+00005190: 7973 7465 6d2e 5275 6e74 696d 652e 5365  ystem.Runtime.Se
+000051a0: 7269 616c 697a 6174 696f 6e1e 5379 7374  rialization.Syst
+000051b0: 656d 2e54 6578 742e 4a73 6f6e 2e53 6572  em.Text.Json.Ser
+000051c0: 6961 6c69 7a61 7469 6f6e 2a01 a795 01a7  ialization*.....
+000051d0: aa01 a7cc 01a7 ec01 a7f3 01a8 0e01 a818  ................
+000051e0: 01a8 2401 a834 01a8 4501 be38 01be 5e01  ..$..4..E..8..^.
+000051f0: a883 01be 7b0c 0000 0018 80ac 050b 001c  ....{...........
+00005200: 0800 0700 0000 2481 7805 0c00 0000 2681  ......$.x.....&.
+00005210: 8205 0b00 3208 0007 0000 001f 818d 0507  ....2...........
+00005220: 0000 0018 8346 3207 0000 0018 834d 2e07  .....F2......M..
+00005230: 0000 0018 8353 2e07 0000 0018 8359 2e07  .....S.......Y..
+00005240: 0000 0018 8480 3107 0000 0018 8490 4907  ......1.......I.
+00005250: 0000 0017 8491 4907 0000 0017 8492 3307  ......I.......3.
+00005260: 0000 0018 84ac 5107 0000 0018 84ad 5107  ......Q.......Q.
+00005270: 0000 0018 84ae 5107 0000 0018 84af 5107  ......Q.......Q.
+00005280: 0000 0154 8612 3f08 0000 0181 0a86 1f34  ...T..?........4
+00005290: 0700 0002 6686 2d34 0800 0001 80a6 8635  ....f.-4.......5
+000052a0: 3407 0000 0021 86ab 3607 0000 0034 8830  4....!..6....4.0
+000052b0: 3f07 0000 002f 88d1 4907 0000 0034 88da  ?..../..I....4..
+000052c0: 4a07 0000 002d 88e3 4707 0000 002e 88e8  J....-..G.......
+000052d0: 2f07 0000 002e 88ea 5a07 0000 0033 88ec  /.......Z....3..
+000052e0: 2f07 0000 0033 88ee 5b07 0000 002c 88f0  /....3..[....,..
+000052f0: 2f07 0000 002c 88f2 5807 0000 0035 891d  /....,..X....5..
+00005300: 3507 0000 0030 896c 5b07 0000 0030 897b  5....0.l[....0.{
+00005310: 5b07 0000 002f 8983 5b07 0000 002f 898a  [..../..[..../..
+00005320: 5b07 0000 0034 8991 5b06 0000 0034 380d  [....4..[....48.
+00005330: 1f03 0000 3c3d 0d0e 0037 0200 0d00 6a02  ....<=...7....j.
+00005340: 0855 003c 0279 0900 2202 000d 0001 0279  .U.<.y.."......y
+00005350: 1504 0000 3c46 0d0e 002b 0200 0d00 2202  ....<F...+....".
+00005360: 000d 0001 0279 1504 0000 3c4d 0d0e 002a  .....y....<M...*
+00005370: 0200 0d00 2202 000d 0001 0279 0b00 0000  ...."......y....
+00005380: 2454 0d0d 0001 0279 0b05 0000 2559 0d35  $T.....y....%Y.5
+00005390: 0b04 0200 0b05 0000 246a 0d35 0904 0200  ........$j.5....
+000053a0: 80a8 0600 0021 8083 2709 0000 0200 0d00  .....!..'.......
+000053b0: 5f04 001d 0477 0700 0004 0002 7d26 0600  _....w......}&..
+000053c0: 1b0a 0409 0000 0500 0c00 6104 0000 0700  ..........a.....
+000053d0: 2204 770d 0041 0200 1d00 2f02 001d 000e  ".w..A..../.....
+000053e0: 0408 0700 2002 0013 0027 0200 1400 2104  .... ....'....!.
+000053f0: 0013 0080 8302 084f 0030 0671 1a00 6d02  .......O.0.q..m.
+00005400: 083b 0017 0479 0d00 1702 000d 004e 0200  .;...y.......N..
+00005410: 1800 2e02 0007 0022 0200 0f00 2202 000f  ......."...."...
+00005420: 005c 0200 2c00 6002 002c 0025 0200 0d00  .\..,.`..,.%....
+00005430: 2602 0012 001e 0200 1b00 6602 0023 0000  &.........f..#..
+00005440: 0400 0249 2409 0001 3c4d 0700 0000 4286  ...I$...<M....B.
+00005450: 0652 0700 0000 4289 2252 0700 0000 3180  .R....B."R....1.
+00005460: 9b2c 0700 0000 6a80 b326 0700 0000 4a80  .,....j..&....J.
+00005470: b625 0700 0000 6e80 bf27 0700 0000 4d80  .%....n..'....M.
+00005480: c226 0000                                .&..
```

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorAnim_9.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorArachnus.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorArachnus.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorBlue.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBlue.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorBomb.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPA3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorGenesis.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGenesis.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorGuardian.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGuardian.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorIceBeam.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorIceBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorLocked.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorLocked.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorMissile.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorPBomb.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorQueen.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorQueen.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorScrew.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorScrew.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSerris.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSerris.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSpider.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpider.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorSuper.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSuper.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTester.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTester.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTorizo.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTorizo.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/bg_MapBottom2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bg_MapBottom2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newA4Doors.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/newA4Doors2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUIMissile.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUIPBomb.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/sGUISMissile.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUISMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpHideout.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpHideout.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png` & `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.2/am2r_yams.egg-info/SOURCES.txt` & `am2r_yams-0.0.3/am2r_yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

