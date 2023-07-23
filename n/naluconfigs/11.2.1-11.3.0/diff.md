# Comparing `tmp/naluconfigs-11.2.1.tar.gz` & `tmp/naluconfigs-11.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-11.2.1.tar", last modified: Thu Jun 29 20:55:41 2023, max compression
+gzip compressed data, was "naluconfigs-11.3.0.tar", last modified: Sun Jul 23 22:28:39 2023, max compression
```

## Comparing `naluconfigs-11.2.1.tar` & `naluconfigs-11.3.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.411994 naluconfigs-11.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.411994 naluconfigs-11.2.1/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.423994 naluconfigs-11.2.1/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.905889 naluconfigs-11.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-23 22:28:39.905889 naluconfigs-11.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:28:39.905889 naluconfigs-11.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.897889 naluconfigs-11.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.897889 naluconfigs-11.3.0/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.897889 naluconfigs-11.3.0/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.901889 naluconfigs-11.3.0/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.901889 naluconfigs-11.3.0/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.905889 naluconfigs-11.3.0/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.897889 naluconfigs-11.3.0/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-23 22:28:39.000000 naluconfigs-11.3.0/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-23 22:28:39.000000 naluconfigs-11.3.0/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:28:39.000000 naluconfigs-11.3.0/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-23 22:28:39.000000 naluconfigs-11.3.0/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-23 22:28:39.000000 naluconfigs-11.3.0/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:28:39.905889 naluconfigs-11.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-23 22:28:23.000000 naluconfigs-11.3.0/tests/test_range_keys.py
```

### Comparing `naluconfigs-11.2.1/PKG-INFO` & `naluconfigs-11.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.2.1
+Version: 11.3.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.2.1/README.md` & `naluconfigs-11.3.0/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/pyproject.toml` & `naluconfigs-11.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/setup.py` & `naluconfigs-11.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/__init__.py` & `naluconfigs-11.3.0/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/_constructors.py` & `naluconfigs-11.3.0/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/chips/udc16.yml`

 * *Files 2% similar despite different names*

```diff
@@ -241,28 +241,32 @@
     cmpbias2:
       address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0x000
-    isel:
-      address: 0x13
-      bitposition: 4
-      bitwidth: 8
-      description: ''
-      readwrite: w
-      value: 0xAA  # default 800 mV
-    rampcap:
+    isel_cap_select:
       address: 0x13
       bitposition: 0
       bitwidth: 4
       description: 'Can be used to change the ramp capacitor value, the actual values, ask Chris'
-      readwrite: w
-      value: 0x0
+      value: 0x00
+    isel_ramp_current:
+      address: 0x13
+      bitposition: 4
+      bitwidth: 2
+      description:
+      value: 0x03
+    isel_dac:
+      address: 0x13
+      bitposition: 6
+      bitwidth: 6
+      description:
+      value: 0x28
     scvbias:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0x622
```

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-11.3.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv3_gbe.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/upac96.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 model: upac96
 features:
   adc2mv: false
   dac_sweep: true
   ext_dac: true
+  conversion_ramp_optimizer: true
   pedestals: true
   threshold_scan: false
   tia_dac: false
   timing_calibration: false
   naludaq_rs: false
 params:
   num_chips: 6  # Number of chips, to be replaced with the actual chips
@@ -123,18 +124,14 @@
           value: 0x032
         wrsync2_le:
           value: 0x040
         wrsync2_te:
           value: 0x072
         cmpbias1:
           value: 0x3E8
-        isel:
-          bitposition: 0
-          bitwidth: 12
-          value: 0x000
         transfer:
           value: 0x0FF
   digital_registers:
     !include_registers
       from: udc16::registers::digital_registers
       value_count: 6
       delete:
```

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-11.3.0/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/exceptions.py` & `naluconfigs-11.3.0/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/helpers.py` & `naluconfigs-11.3.0/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs/postprocess.py` & `naluconfigs-11.3.0/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-11.3.0/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.2.1
+Version: 11.3.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.2.1/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-11.3.0/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/tests/test_hex_addr_converter.py` & `naluconfigs-11.3.0/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/tests/test_i2c_registers.py` & `naluconfigs-11.3.0/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/tests/test_multichip.py` & `naluconfigs-11.3.0/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/tests/test_post_processing.py` & `naluconfigs-11.3.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.2.1/tests/test_range_keys.py` & `naluconfigs-11.3.0/tests/test_range_keys.py`

 * *Files identical despite different names*

