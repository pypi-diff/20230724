# Comparing `tmp/am2r_yams-0.0.3.tar.gz` & `tmp/am2r_yams-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-0.0.3.tar", last modified: Mon Jul 24 17:48:53 2023, max compression
+gzip compressed data, was "am2r_yams-0.0.4.tar", last modified: Mon Jul 24 20:20:12 2023, max compression
```

## Comparing `am2r_yams-0.0.3.tar` & `am2r_yams-0.0.4.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/Patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/__pyinstaller/hook-yams-py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.3/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.3/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.3/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.3/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.3/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.3/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (123)   941568 2023-07-24 17:48:43.000000 am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-24 17:48:41.000000 am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (123)   170496 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-07-24 17:48:45.000000 am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.821160 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/sprites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.829160 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorArachnus.png
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBlue.png
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGenesis.png
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGuardian.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorLocked.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorQueen.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorScrew.png
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSerris.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpider.png
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSuper.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTester.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTorizo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.809160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.829160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.833160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.837160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.841160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.845160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.849160 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.849160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors.png
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUISMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpHideout.png
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.813160 am2r_yams-0.0.3/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 17:48:53.000000 am2r_yams-0.0.3/am2r_yams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:48:53.853160 am2r_yams-0.0.3/am2r_yams_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/am2r_yams_tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 17:48:19.000000 am2r_yams-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 17:48:53.857160 am2r_yams-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.926026 am2r_yams-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 20:20:12.926026 am2r_yams-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/Patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/__pyinstaller/hook-am2r_yams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.906026 am2r_yams-0.0.4/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.4/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.4/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.4/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.4/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.4/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.4/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   941568 2023-07-24 20:20:03.000000 am2r_yams-0.0.4/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-24 20:20:02.000000 am2r_yams-0.0.4/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-24 20:20:05.000000 am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (123)   170496 2023-07-24 20:20:05.000000 am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-07-24 20:20:05.000000 am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.906026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.4/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.906026 am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/sprites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.910026 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorArachnus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorBlue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorGenesis.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorGuardian.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorLocked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorQueen.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorScrew.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSerris.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSpider.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSuper.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTester.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTorizo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.910026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.910026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.914026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.914026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.914026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.914026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.918026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.918026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.918026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.918026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.918026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.922026 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.922026 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.922026 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newA4Doors.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newA4Doors2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.922026 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUIMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUIPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUISMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpHideout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.926026 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.898026 am2r_yams-0.0.4/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 20:20:12.000000 am2r_yams-0.0.4/am2r_yams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:20:12.926026 am2r_yams-0.0.4/am2r_yams_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/am2r_yams_tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 20:19:44.000000 am2r_yams-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 20:20:12.926026 am2r_yams-0.0.4/setup.cfg
```

### Comparing `am2r_yams-0.0.3/LICENSE` & `am2r_yams-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/PKG-INFO` & `am2r_yams-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 0.0.3
+Version: 0.0.4
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `am2r_yams-0.0.3/am2r_yams/Patcher.py` & `am2r_yams-0.0.4/am2r_yams/Patcher.py`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-0.0.4/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-0.0.4/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.4/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-0.0.4/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-0.0.4/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-0.0.4/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-0.0.4/am2r_yams/yams/UndertaleModLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-0.0.4/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/0.0.4': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), delete: ['YAMS-LIB/0.0.3']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'YAMS-LIB/0.0.4': OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Macross.Json.Extensions', '3.0.0'), ('SixLabors.ImageSharp', "*

 * *              "'3.0.1'), ('UndertaleModLib', '1.0.0')])), ('runtime', "*

 * *              "OrderedDict([('YAMS-LIB.dll', OrderedDict())]))]), delete: ['YAMS-LIB/0.0.3' […]*

```diff
@@ -58,15 +58,15 @@
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/0.0.3": {
+        "YAMS-LIB/0.0.4": {
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
-            "YAMS-LIB/0.0.3": {
+            "YAMS-LIB/0.0.4": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
                     "SixLabors.ImageSharp": "3.0.1",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
                     "YAMS-LIB.dll": {}
```

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 0% similar despite different names*

#### pedump {}

```diff
@@ -1,12 +1,12 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xdc7e48b0
+	             Time stamp: 0x86d84bd8
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
```

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/YAMS-LIB.pdb` & `am2r_yams-0.0.4/am2r_yams/yams/YAMS-LIB.pdb`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 00000000: 4253 4a42 0100 0100 0000 0000 0c00 0000  BSJB............
 00000010: 5044 4220 7631 2e30 0000 0000 0000 0600  PDB v1.0........
 00000020: 7c00 0000 6400 0000 2350 6462 0000 0000  |...d...#Pdb....
 00000030: e000 0000 540c 0000 237e 0000 340d 0000  ....T...#~..4...
 00000040: a805 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
 00000050: dc12 0000 0400 0000 2355 5300 e012 0000  ........#US.....
 00000060: 5000 0000 2347 5549 4400 0000 3013 0000  P...#GUID...0...
-00000070: 5441 0000 2342 6c6f 6200 0000 be86 ceaf  TA..#Blob.......
-00000080: 2db3 ce4f 8309 6100 97cb fad8 e94d 468e  -..O..a......MF.
+00000070: 5441 0000 2342 6c6f 6200 0000 25c1 3895  TA..#Blob...%.8.
+00000080: 9f77 0440 ad90 a9aa 878a 4f5d 930f 2ad4  .w.@......O]..*.
 00000090: 0000 0000 579d 0228 090a 0000 0100 0000  ....W..(........
 000000a0: 6b00 0000 1800 0000 c900 0000 4700 0000  k...........G...
 000000b0: 4700 0000 0a01 0000 6e00 0000 3001 0000  G.......n...0...
 000000c0: 0100 0000 0600 0000 2b00 0000 0100 0000  ........+.......
 000000d0: 0100 0000 0900 0000 0600 0000 1400 0000  ................
 000000e0: 0000 0000 0200 0001 0000 0000 0000 bf00  ................
 000000f0: 0000 0000 0000 8400 0500 0000 4700 0000  ............G...
@@ -324,17 +324,17 @@
 00001430: 696f 6e3d 7636 2e30 2e41 7373 656d 626c  ion=v6.0.Assembl
 00001440: 7941 7474 7269 6275 7465 732e 6373 102f  yAttributes.cs./
 00001450: 0001 060d 1212 1780 8f80 9380 9b80 ef20  ............... 
 00001460: 7897 e595 3cb5 cd51 3150 9b35 0421 8634  x...<..Q1P.5.!.4
 00001470: c24b 9ce7 a68b 984f fb5a 1668 6eb5 af5c  .K.....O.Z.hn..\
 00001480: 1859 414d 532d 4c49 422e 4173 7365 6d62  .YAMS-LIB.Assemb
 00001490: 6c79 496e 666f 2e63 7310 2f00 0106 0d12  lyInfo.cs./.....
-000014a0: 1217 808f 8093 809b 8150 20b3 6d04 3831  .........P .m.81
-000014b0: 1077 0013 335d a311 2fb4 9cad d51a 19ee  .w..3]../.......
-000014c0: 52a3 9f5f 4e55 4995 a566 a501 0282 2476  R.._NUI..f....$v
+000014a0: 1217 808f 8093 809b 8150 20d3 6c00 4e2f  .........P .l.N/
+000014b0: 5800 db22 f788 458a d8af 8ef0 6f4f 2637  X.."..E.....oO&7
+000014c0: 8651 5c94 e175 b094 ecee 0001 0282 2476  .Q\..u........$v
 000014d0: 6572 7369 6f6e 0032 0063 6f6d 7069 6c65  ersion.2.compile
 000014e0: 722d 7665 7273 696f 6e00 342e 362e 302d  r-version.4.6.0-
 000014f0: 332e 3233 3235 392e 382b 6333 6363 3164  3.23259.8+c3cc1d
 00001500: 3063 6565 6162 3161 3635 6461 3032 3137  0ceeab1a65da0217
 00001510: 6534 3033 3835 3161 3165 3861 3330 3038  e403851a1e8a3008
 00001520: 3661 006c 616e 6775 6167 6500 4323 0073  6a.language.C#.s
 00001530: 6f75 7263 652d 6669 6c65 2d63 6f75 6e74  ource-file-count
```

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.4/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.4/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorAnim_9.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorAnim_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorArachnus.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorArachnus.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBlue.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorBlue.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorBomb.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPA3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGenesis.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorGenesis.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorGuardian.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorGuardian.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorIceBeam.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorIceBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorLocked.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorLocked.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorMissile.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPBomb.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorQueen.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorQueen.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorScrew.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorScrew.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSerris.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSerris.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSpider.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSpider.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorSuper.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorSuper.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTester.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTester.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTorizo.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTorizo.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/bg_MapBottom2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/bg_MapBottom2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newA4Doors.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/newA4Doors2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/newA4Doors2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIMissile.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUIMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUIPBomb.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUIPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/sGUISMissile.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/sGUISMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpHideout.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpHideout.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png` & `am2r_yams-0.0.4/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.3/am2r_yams.egg-info/PKG-INFO` & `am2r_yams-0.0.4/am2r_yams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r-yams
-Version: 0.0.3
+Version: 0.0.4
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `am2r_yams-0.0.3/am2r_yams.egg-info/SOURCES.txt` & `am2r_yams-0.0.4/am2r_yams.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 am2r_yams.egg-info/SOURCES.txt
 am2r_yams.egg-info/dependency_links.txt
 am2r_yams.egg-info/entry_points.txt
 am2r_yams.egg-info/not-zip-safe
 am2r_yams.egg-info/requires.txt
 am2r_yams.egg-info/top_level.txt
 am2r_yams/__pyinstaller/__init__.py
-am2r_yams/__pyinstaller/hook-yams-py.py
+am2r_yams/__pyinstaller/hook-am2r_yams.py
 am2r_yams/yams/ICSharpCode.SharpZipLib.dll
 am2r_yams/yams/Macross.Json.Extensions.dll
 am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
 am2r_yams/yams/PropertyChanged.dll
 am2r_yams/yams/SixLabors.ImageSharp.dll
 am2r_yams/yams/System.Drawing.Common.dll
 am2r_yams/yams/UndertaleModLib.dll
```

### Comparing `am2r_yams-0.0.3/setup.cfg` & `am2r_yams-0.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = am2r_yams
-version = 0.0.3
+version = 0.0.4
 description = An open source randomizer patcher for AM2R.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Miepee/YAMS
 author = Miepee
 license_files = 
 	LICENSE
```

