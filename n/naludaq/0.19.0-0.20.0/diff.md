# Comparing `tmp/naludaq-0.19.0.tar.gz` & `tmp/naludaq-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.19.0.tar", last modified: Sat Jun 17 02:51:40 2023, max compression
+gzip compressed data, was "naludaq-0.20.0.tar", last modified: Sun Jul 23 23:48:55 2023, max compression
```

## Comparing `naludaq-0.19.0.tar` & `naludaq-0.20.0.tar`

### file list

```diff
@@ -1,257 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-17 02:51:24.000000 naludaq-0.19.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-17 02:51:40.535666 naludaq-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-06-17 02:51:24.000000 naludaq-0.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-17 02:51:24.000000 naludaq-0.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 02:51:40.535666 naludaq-0.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-17 02:51:24.000000 naludaq-0.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.499665 naludaq-0.19.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36060 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.507665 naludaq-0.19.0/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.507665 naludaq-0.19.0/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/asocv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/lookup_table/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/aav3.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_acq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/threshold_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 02:51:24.000000 naludaq-0.19.0/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-23 23:48:34.000000 naludaq-0.20.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-23 23:48:55.603492 naludaq-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-23 23:48:34.000000 naludaq-0.20.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-23 23:48:34.000000 naludaq-0.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:48:55.603492 naludaq-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-23 23:48:34.000000 naludaq-0.20.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.539489 naludaq-0.20.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.543489 naludaq-0.20.0/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.547489 naludaq-0.20.0/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.547489 naludaq-0.20.0/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.547489 naludaq-0.20.0/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.551489 naludaq-0.20.0/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (123)    30012 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.555489 naludaq-0.20.0/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.555489 naludaq-0.20.0/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.559490 naludaq-0.20.0/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.563490 naludaq-0.20.0/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.563490 naludaq-0.20.0/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.567490 naludaq-0.20.0/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/asocv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.567490 naludaq-0.20.0/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.571490 naludaq-0.20.0/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.571490 naludaq-0.20.0/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.575490 naludaq-0.20.0/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.575490 naludaq-0.20.0/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.575490 naludaq-0.20.0/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.579491 naludaq-0.20.0/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.579491 naludaq-0.20.0/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.583491 naludaq-0.20.0/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.583491 naludaq-0.20.0/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.587491 naludaq-0.20.0/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.587491 naludaq-0.20.0/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.587491 naludaq-0.20.0/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.591491 naludaq-0.20.0/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.595491 naludaq-0.20.0/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.595491 naludaq-0.20.0/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.599491 naludaq-0.20.0/src/naludaq/tools/optimizers/conversion_ramp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/conversion_ramp/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/src/naludaq/tools/pedestals/_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/_new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/_new/aav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25319 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/_new/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/_new/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/threshold_scan/threshold_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-23 23:48:34.000000 naludaq-0.20.0/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.547489 naludaq-0.20.0/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-23 23:48:55.000000 naludaq-0.20.0/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-23 23:48:55.000000 naludaq-0.20.0/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:48:55.000000 naludaq-0.20.0/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-23 23:48:55.000000 naludaq-0.20.0/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 23:48:55.000000 naludaq-0.20.0/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:48:55.603492 naludaq-0.20.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-23 23:48:34.000000 naludaq-0.20.0/tests/test_naludaq.py
```

### Comparing `naludaq-0.19.0/LICENSE.txt` & `naludaq-0.20.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/PKG-INFO` & `naludaq-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.19.0
+Version: 0.20.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.19.0/README.md` & `naludaq-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/pyproject.toml` & `naludaq-0.20.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   { name="Terry Pham" },
 ]
 description = "Backend package for Nalu Scientific hardware"
 readme = "README.md"
 dynamic = ["version"]
 requires-python = ">=3.9"
 dependencies = [
-  "naluconfigs>=11.0.0",
+  "naluconfigs>=11.3.0",
   "ftd3xx>=1.0",
   "naludaq_rs>=0.1.9",
   "deprecation",
   "ftd2xx>=1.1.2",
   "h5py",
   "numpy<1.24",
   "pyserial==3.4",
```

### Comparing `naludaq-0.19.0/setup.py` & `naludaq-0.20.0/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/client.py` & `naludaq-0.20.0/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/context.py` & `naludaq-0.20.0/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/exceptions.py` & `naludaq-0.20.0/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.20.0/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/managers/config.py` & `naludaq-0.20.0/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/managers/connection.py` & `naludaq-0.20.0/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/managers/io.py` & `naludaq-0.20.0/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/backend/models/acquisition.py` & `naludaq-0.20.0/src/naludaq/backend/models/acquisition.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,21 +95,23 @@
         """Compute the hash for this object"""
         return hash(self._name)
 
     def __len__(self) -> int:
         """Get the number of events in the acquisition"""
         return self.length
 
-    def __getitem__(self, index: "int | slice") -> "bytes | list[bytes]":
+    def __getitem__(self, index: "int | slice | list") -> "bytes | list[bytes]":
         """Get events from the remote"""
         if isinstance(index, int):
             return self.raw_event(index)
         if isinstance(index, slice):
             start, stop, step = index.indices(self.length)
             return [self.raw_event(x) for x in range(start, stop, step)]
+        if isinstance(index, list):
+            return [self.raw_event(x) for x in index]
         raise TypeError("Index must be int or slice")
 
     def __iter__(self) -> Iterator[dict]:
         """Iterate over raw events"""
         return (self[i] for i in range(len(self)))
 
     @property
@@ -824,14 +826,16 @@
         self._raise_if_closed()
         result = None
         if isinstance(index, int):
             index = _resolve_index_or_raise(index, len(self))
             result = self.parsed_event(index)
         elif isinstance(index, slice):
             result = [self.parsed_event(i) for i in range(*index.indices(len(self)))]
+        elif isinstance(index, list):
+            result = [self.parsed_event(i) for i in index]
         else:
             raise TypeError("Index must be an int or slice")
         return result
 
     def open(self):
         """Open the acquisition for reading.
```

### Comparing `naludaq-0.19.0/src/naludaq/backend/models/device.py` & `naludaq-0.20.0/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/__init__.py` & `naludaq-0.20.0/src/naludaq/board/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
         self.fCRC = False
         self.loopback = True
 
         # Calibration
         self.pedestals: dict = None
         self.caldata: dict = None
         self.timingcal: list = None
+        self.tuning = {}
 
     def __del__(self):
         """Cleanup the server if it's running."""
         self.stop_server()
 
     @property
     def context(self) -> "Context | None":
@@ -386,14 +387,15 @@
         try:
             self.connection = get_connection(self.connection_info)
         except ConnectionError as e:
             raise ConnectionError(f"Failed to open connection: {e}") from e
         else:
             self._context = None
             self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def get_ftdi_connection(
         self, board_number=None, comport=None, serial_number=None, baud=None
     ):
         """Connect to the board using FTDI.
 
         Test connecting either using comport or using serial
@@ -420,14 +422,15 @@
         try:
             self.connection = get_connection(self.connection_info)
         except ConnectionError as e:
             raise ConnectionError(f"Failed to open connection: {e}") from e
         else:
             self._context = None
             self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def get_ft60x_connection(
         self,
         *args,
         serial_number=None,
         **kwargs,
     ):
@@ -452,14 +455,15 @@
         try:
             self.connection = get_connection(self.connection_info)
         except ConnectionError as e:
             raise ConnectionError(f"Failed to open connection: {e}") from e
         else:
             self._context = None
             self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def get_tcp_connection(self, ip: str, port: int):
         """Open a TCP connection."""
         self.connection_info = {
             "type": "tcp",
             "model": self.model,
             "stop_word": self.params["stop_word"],
@@ -473,14 +477,15 @@
             self.connection.open()
         except ConnectionError as error_msg:
             self.connection = None
             raise ConnectionError("No connection established due to: %s", error_msg)
         else:
             self._context = None
             self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def get_mock_uart_connection(self, user_port, board_port, ip="127.0.0.1"):
         """Connect to a mock board.
 
         Args:
             user_port (tuple): the port of the user
             board_port (tuple): the port of the board
@@ -504,14 +509,15 @@
         try:
             self.connection = get_connection(self.connection_info)
         except ConnectionError as error_msg:
             raise ConnectionError("No connection established due to: %s", error_msg)
         else:
             self._context = None
             self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def load_clockfile(self, filepath=None):
         """
         Changes the clock_file parameter to filepath
         Loads the clock file into a list that is returned
 
         Args:
```

### Comparing `naludaq-0.19.0/src/naludaq/board/board_inits.py` & `naludaq-0.20.0/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.20.0/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.20.0/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/_UART.py` & `naludaq-0.20.0/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/_USB.py` & `naludaq-0.20.0/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/base_connection.py` & `naludaq-0.20.0/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.20.0/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/tcp.py` & `naludaq-0.20.0/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/connections/udp.py` & `naludaq-0.20.0/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/__init__.py` & `naludaq-0.20.0/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.20.0/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.20.0/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.20.0/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.20.0/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.20.0/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.20.0/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.20.0/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/board/params.py` & `naludaq-0.20.0/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/__init__.py` & `naludaq-0.20.0/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/_chip.py` & `naludaq-0.20.0/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/_common.py` & `naludaq-0.20.0/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/_fpga.py` & `naludaq-0.20.0/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/analog_registers.py` & `naludaq-0.20.0/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/chip_selection.py` & `naludaq-0.20.0/src/naludaq/communication/chip_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     ```py
     with select_chips(board, [0, 1]):
         board.connection.send("write something to chips 0 and 1")
     ```
     """
     validations.validate_chip_list_or_raise(chips, board.params)
     select, deselect = select_chips_commands(board, chips)
-    _send_command(select)
+    _send_command(board, select)
     try:
         yield
     finally:
         if restore:
-            _send_command(deselect)
+            _send_command(board, deselect)
 
 
 def select_chips_commands(board, chips: list[int]) -> tuple[str, str]:
     """Generate a pair of commands to select/restore chips.
 
     Args:
         board (Board): the board
```

### Comparing `naludaq-0.19.0/src/naludaq/communication/control_registers.py` & `naludaq-0.20.0/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/digital_registers.py` & `naludaq-0.20.0/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/i2c.py` & `naludaq-0.20.0/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/i2c_registers.py` & `naludaq-0.20.0/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/communication/registers.py` & `naludaq-0.20.0/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.20.0/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.20.0/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/board/aodsoc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from naludaq.communication import DigitalRegisters, select_chips
+from naludaq.communication import DigitalRegisters
 
 from .default import BoardController
 
 LOGGER = logging.getLogger("naludaq.board_controller_aodsoc")
 
 
 class BoardControllerAodsoc(BoardController):
@@ -15,27 +15,24 @@
     """
 
     def read_scalar(self, channel: int) -> int:
         """Read the scalar for the given channel"""
         channels_per_chip = self.board.channels // self.board.available_chips
         relative_channel = channel % channels_per_chip
         chip = channel // channels_per_chip
-
-        with select_chips(self.board, [chip]):
-            result = super().read_scalar(relative_channel)
-        return result
+        return self._read_scalar_inner(chip, relative_channel)
 
     def _read_scalar_inner(self, chip: int, relative_channel: int) -> int:
         """Read the scalar for the given channel.
 
         This is the inner function that actually reads the scalar.
         It is called by `read_scalar` and should not be called directly.
         """
         name = self.get_scal_name(relative_channel)
-        scal = self._read_digital_register(name)
+        scal = self._read_digital_register(name, chips=chip)
         try:
             scalhigh = self._read_digital_register("scalhigh", chips=chip)
         except (KeyError, AttributeError):
             scalhigh = 0
         shift_amt = DigitalRegisters(self.board).registers[name]["bitwidth"]
         scal += scalhigh << shift_amt
```

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/asocv3.py` & `naludaq-0.20.0/src/naludaq/controllers/board/asocv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/default.py` & `naludaq-0.20.0/src/naludaq/controllers/board/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     It doesn't receive continous data, the data acquisition module should be used for that.
     """
 
     def start_readout(
         self,
         trig="self",
         lb="trigrel",
-        acq="pedsub",
+        acq="raw",
         dig_head=False,
         ped="zero",
         readoutEn=True,
         singleEv=False,
     ):
         """Sends a readout signal to the board.
 
@@ -46,16 +46,16 @@
                 'ext': '01' - use the external trigger.
                 'self': '10' - trigger on input RF signal.
             lbType (str):
                 'forced': '00' - always reads out same set of windows, start window set by lookback
                 'trig': '01' - relative to the trigger.
                 'roi': '10' - complicated...
             acq_type (str):
-                'raw': '00' - Can't ped-subtract.
-                'ped': '01' - sub, spits out headers, channels, and windows.
+                'raw': '00' - Can't ped-subtract. <Default output>
+                'ped': '01' - sub, spits out headers, channels, and windows. <Requires firmware modification>
             dig_head (bool):
                 True: reads out a "digitization" header after each sram read (only works with acq_type="ped")
                 False: doesn't read out that header
             pedMode (str):
                 'z': '00' - all peds = 0
                 'c': '01' - peds = chan*1024, set offset per channel
                 'r': '11' - peds = RAM addr
```

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/oleas.py` & `naludaq-0.20.0/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.20.0/src/naludaq/controllers/board/trbhm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """
 """
 from logging import getLogger
 
-from naludaq.communication import ControlRegisters, DigitalRegisters, select_chips
+from naludaq.communication import ControlRegisters, DigitalRegisters
 
 from .default import BoardController
 
 LOGGER = getLogger("naludaq.board_controller_trbhm")
 
 
 class TrbhmBoardController(BoardController):
     """Special board controller for TRBHM."""
 
     def read_scalar(self, channel: int) -> int:
         """Read the scalar for the given channel"""
         channels_per_chip = self.board.channels // self.board.available_chips
         relative_channel = channel % channels_per_chip
         chip = channel // channels_per_chip
-
-        with select_chips(self.board, [chip]):
-            result = super().read_scalar(relative_channel)
-        return result
+        return self._read_scalar_inner(chip, relative_channel)
 
     def _read_scalar_inner(self, chip: int, relative_channel: int) -> int:
         """Read the scalar for the given channel.
 
         This is the inner function that actually reads the scalar.
         It is called by `read_scalar` and should not be called directly.
         """
         name = self.get_scal_name(relative_channel)
-        scal = self._read_digital_register(name)
+        scal = self._read_digital_register(name, chips=chip)
         try:
             scalhigh = self._read_digital_register("scalhigh", chips=chip)
         except (KeyError, AttributeError):
             scalhigh = 0
         shift_amt = DigitalRegisters(self.board).registers[name]["bitwidth"]
         scal += scalhigh << shift_amt
```

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/udc.py` & `naludaq-0.20.0/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/upac.py` & `naludaq-0.20.0/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/board/upac96.py` & `naludaq-0.20.0/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.20.0/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/connection/upac.py` & `naludaq-0.20.0/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.20.0/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/aardvarcv3.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.20.0/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.20.0/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.20.0/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.20.0/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.20.0/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/readout/default.py` & `naludaq-0.20.0/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.20.0/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.20.0/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/tia/base.py` & `naludaq-0.20.0/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/default.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.20.0/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/__init__.py` & `naludaq-0.20.0/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/debugdaq.py` & `naludaq-0.20.0/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/lightdaq.py` & `naludaq-0.20.0/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/preprocess.py` & `naludaq-0.20.0/src/naludaq/daq/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
         Returns:
             parsed event with a 'data' key.
 
         Raises:
             Doesn't raises errors but will return unparsed if parsing fails.
         """
         event = to_process
-        try:
-            event = self.parser.parse(to_process)
-        except (Exception, BadDataError) as e_msg:
-            LOGGER.error("process_event didn't work due to %s", e_msg)
-
+        if "data" not in event:
+            try:
+                event = self.parser.parse(to_process)
+            except (Exception, BadDataError) as e_msg:
+                LOGGER.error("process_event didn't work due to %s", e_msg)
         return event
 
     def _correct_yaxis(self, event, correct_pedestals: bool, correct_mv: bool):
         """Convert and correct the values on the Y-axis.
 
         Can either pedestals correct Y-axis or convert ADC counts to mV.
         Future upgrade would allow both.
```

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/__init__.py` & `naludaq-0.20.0/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.20.0/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.20.0/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.20.0/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.20.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.20.0/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.20.0/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.20.0/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.20.0/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/devices/eeprom.py` & `naludaq-0.20.0/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/devices/i2c_device.py` & `naludaq-0.20.0/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/devices/ltc2990.py` & `naludaq-0.20.0/src/naludaq/devices/ltc2990.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Driver for the LTC2990 I2C voltage/current/temperature monitor.
 
 Datasheet:
     https://www.analog.com/media/en/technical-documentation/data-sheets/ltc2990.pdf
 
 Mitchell Matsumori-Kelly
 """
-from functools import partial
 import logging
 import time
+from functools import partial
 
 from naludaq.helpers.exceptions import BadDataError, I2CError
 from naludaq.helpers.helper_functions import type_name
 
 from .i2c_device import I2CDevice
 
 logger = logging.getLogger("naludaq.ltc2990")
@@ -86,108 +86,86 @@
         Raises:
             I2CError: if the deivce did not acknowledge the command
         """
         logging.debug(f"{self._log_prefix} - triggering conversion")
         self.write_register(LTC2990.REGISTER_TRIGGER, bytes([1]))
         time.sleep(0.01)
 
-    def read_voltage(self, channel: int, attempts=5) -> float:
+    def read_voltage(self, channel: int) -> float:
         """Reads the voltage for a particular channel on the device.
 
         This function WILL fail if the conversion has not been properly
         triggered.
 
         Args:
             channel (int): the channel number, must be 1-4.
-            attempts (int): number of times to try reading the data.
-                The data comes back flagged as invalid if the device
-                has not been triggered or is not finished converting.
 
         Returns:
             The voltage in volts.
 
         Raises:
             BadDataError if the device has not stored a converted value.
         """
         register = LTC2990.VOLTAGE_REGISTER_MAP.get(channel, None)
         if register is None:
             raise ValueError(f"Channel must be 1-4, not {channel}")
         try:
-            voltage_reg = self._read_voltage_register(register, attempts)
+            voltage_reg = self._read_voltage_register(register)
         except BadDataError:
             raise
         voltage = self._convert_register_to_voltage(voltage_reg)
         logging.debug(
             f"{self._log_prefix} - channel {channel} read back as {voltage} V"
         )
         return voltage
 
-    def read_vcc(self, attempts=5) -> float:
+    def read_vcc(self) -> float:
         """Reads the VCC supply voltage of the device.
 
         This function WILL fail if the conversion has not been properly
         triggered.
 
-        Args:
-            attempts (int): number of times to try reading the data.
-                The data comes back flagged as invalid if the device
-                has not been triggered or is not finished converting.
-
         Returns:
             The voltage in volts.
 
         Raises:
             BadDataError if the device has not stored a converted value.
         """
         try:
             register = LTC2990.REGISTER_VCC_MSB
-            voltage_reg = self._read_voltage_register(register, attempts)
+            voltage_reg = self._read_voltage_register(register)
         except BadDataError:
             raise
         self._fix_device_state()  # weird stuff happens when the register pointer rolls over?
 
         voltage = self._convert_vcc_register_to_voltage(voltage_reg)
         logging.debug(f"{self._log_prefix} - VCC read back as {voltage} V")
         return voltage
 
-    def _read_voltage_register(self, register, attempts=5) -> int:
+    def _read_voltage_register(self, register) -> int:
         """Reads the voltage register for the given channel.
         Make sure a conversion has been triggered before reading!
 
-        Attempts to read the voltage several times until the data
-        is flagged as valid. Otherwise it raises an error if the
-        number of attempts has been exceeded.
-
         Args:
             channel (int): the channel to read from
-            attempts (int): the number of times to read until
-                valid data is received.
 
         Returns:
             int: The value of the register.
 
         Raises:
             BadDataError: if the read operation failed.
         """
-        for _ in range(attempts):
-            try:
-                # Reading one 1-byte wide register results in two bytes thrown back...
-                msb, lsb = self.read_register(register, width=2)[0:2]
-            except:
-                continue
-            data_valid = bool(msb >> 7)
-            if data_valid:
-                break
-            logging.debug(
-                f"{self._log_prefix} - failed to fetch valid data, retrying..."
-            )
-            time.sleep(0.1)
-        else:
+        try:
+            # Reading one 1-byte wide register results in two bytes thrown back...
+            msb, lsb = self.read_register(register, width=2)[0:2]
+        except:
+            raise BadDataError("No valid data returned from LTC2990")
+        data_valid = bool(msb >> 7)
+        if not data_valid:
             raise BadDataError("No valid data returned from LTC2990")
-
         return (msb << 8) | lsb
 
     def _fix_device_state(self):
         """For whatever reason the device gets into an invalid state after reading
         the VCC registers. Right after the VCC registers are read, no write operation
         will be acknowledged by the device.
 
@@ -255,46 +233,47 @@
             data_bits = -(
                 (data_mask ^ data_bits) + 1
             )  # register is stored in two's complement
         voltage = data_bits * factor
         return voltage
 
 
-def read_ltc2990_voltage(board, addr: int, chan: int, samples: int=1) -> float:
+def read_ltc2990_voltage(board, addr: int, chan: int, samples: int = 1) -> float:
     """Read a voltage from an LTC2990 chip.
 
     Args:
         board (_type_): board the LTC2990 is on
         addr (int): 7-bit address of the device
         samples (int): number of readings to average. Default is 1.
 
     Returns:
         float: the averaged voltage.
     """
     _validate_ltc2990_params_or_raise(addr, chan, samples)
 
     device = LTC2990(board, addr)
     reader = partial(device.read_voltage, chan)
-    if isinstance(chan, str) and chan.lower() == 'vcc':
+    if isinstance(chan, str) and chan.lower() == "vcc":
         reader = device.read_vcc
 
     voltages = []
     for _ in range(samples):
         device.trigger_conversion()
         voltages.append(reader())
 
     return sum(voltages) / samples
 
+
 def _validate_ltc2990_params_or_raise(addr: int, chan: int, samples: int):
     """Validate params for the reader helper function"""
     if not isinstance(addr, int):
-        raise TypeError(f'Address must be int, not {type_name(addr)}')
+        raise TypeError(f"Address must be int, not {type_name(addr)}")
     if not isinstance(chan, int):
-        raise TypeError(f'Channel must be int, not {type_name(addr)}')
+        raise TypeError(f"Channel must be int, not {type_name(addr)}")
     if not isinstance(samples, int):
-        raise TypeError(f'Samples must be int, not {type_name(addr)}')
+        raise TypeError(f"Samples must be int, not {type_name(addr)}")
     if not 0 <= addr < 128:
-        raise ValueError(f'Address {addr} is out of bounds')
-    if not chan in [*range(4), 'vcc']:
+        raise ValueError(f"Address {addr} is out of bounds")
+    if not chan in [*range(4), "vcc"]:
         raise ValueError(f'Channel must be 0-4 or "vcc", not {chan}')
     if samples <= 0:
-        raise ValueError(f'Samples must be positive, not {samples}')
+        raise ValueError(f"Samples must be positive, not {samples}")
```

### Comparing `naludaq-0.19.0/src/naludaq/helpers/decorators.py` & `naludaq-0.20.0/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/helpers/exceptions.py` & `naludaq-0.20.0/src/naludaq/helpers/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,7 +139,27 @@
 
 class OperationCanceledError(NaludaqException):
     """The operation was canceled."""
 
 
 class VersionError(NaludaqException):
     """Invalid or unsupported version"""
+
+
+class ProjectIOError(NaludaqException):
+    """Error when reading or writing project files"""
+
+
+class AcquisitionIOError(NaludaqException):
+    """Error when acquiring data"""
+
+
+class PedestalsIOError(NaludaqException):
+    """Error when accessing pedestals files"""
+
+
+class OptimizationError(NaludaqException):
+    """Error while running an optimization script"""
+
+
+class InvalidOptimizationParameters(NaludaqException):
+    """Error with incorrect optimization parameters"""
```

### Comparing `naludaq-0.19.0/src/naludaq/helpers/helper_functions.py` & `naludaq-0.20.0/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/helpers/register_cache.py` & `naludaq-0.20.0/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/helpers/semiton.py` & `naludaq-0.20.0/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/helpers/validations.py` & `naludaq-0.20.0/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/io/__init__.py` & `naludaq-0.20.0/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/io/csv_writer.py` & `naludaq-0.20.0/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/io/hdf5.py` & `naludaq-0.20.0/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/io/io_manager.py` & `naludaq-0.20.0/src/naludaq/io/io_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         sfile = gzip.GzipFile(filename, "r")
         outped = pickle.load(sfile)
     except EOFError as error_msg:
         LOGGER.error("Reached the end of the file, msg: %s", error_msg)
     except IOError as error_msg:
         LOGGER.error("File could not be loaded. %s", error_msg)
     except pickle.UnpicklingError as error_msg:
-        LOGGER.error("Loading pedestals failed: %s", error_msg)
+        LOGGER.error("Loading data failed: %s", error_msg)
     else:
         if not isinstance(outped, dict):
             raise TypeError(f"Not a valid Calibration file: {filename}")
 
         return outped
 
 
@@ -324,19 +324,48 @@
         sfile = gzip.GzipFile(filename, "r")
         output = pickle.load(sfile)
     except EOFError as error_msg:
         LOGGER.error("Reached the end of the file, msg: %s", error_msg)
     except IOError as error_msg:
         LOGGER.error("File could not be loaded. %s", error_msg)
     except pickle.UnpicklingError as error_msg:
-        LOGGER.error("Loading pedestals failed: %s", error_msg)
+        LOGGER.error("Loading data failed: %s", error_msg)
     else:
         return output
 
 
+def save_gzip_data(filename, data):
+    """Save data to a gzip pickled file.
+
+    Args:
+        filename: filepath and filename
+        data: python data to save
+
+    Raises:
+        TypeError if
+        NotADirectoryError if the filename is not in a valid path
+    """
+    if data is None:
+        raise TypeError(f"isel is not valid, got {type(data)}")
+
+    if filename is None:
+        raise TypeError("Supplied pathname is NoneType.")
+    path, _ = os.path.split(filename)
+    if not os.path.isdir(path):
+        raise NotADirectoryError(f"Not a valid directory: {path}")
+
+    try:
+        sfile = gzip.GzipFile(filename, "w", compresslevel=4)
+        pickle.dump(data, sfile, protocol=pickle.HIGHEST_PROTOCOL)
+    except IOError as error_msg:
+        LOGGER.error("File could not be created. %s", error_msg)
+    except pickle.PicklingError as error_msg:
+        LOGGER.error("Saving data failed: %s", error_msg)
+
+
 def load_clockfile(filename):
     """Turns a .txt file into a list, used for clock file loading.
 
     Returns:
         list of the loaded clock commands.
 
     Raises:
```

### Comparing `naludaq-0.19.0/src/naludaq/models/acq_converters.py` & `naludaq-0.20.0/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/models/acquisition.py` & `naludaq-0.20.0/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/naludaq.py` & `naludaq-0.20.0/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/__init__.py` & `naludaq-0.20.0/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/answer_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/base.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/siread.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.20.0/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/parser.py` & `naludaq-0.20.0/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/udc_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/parsers/upac_parser.py` & `naludaq-0.20.0/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.20.0/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.20.0/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.20.0/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.20.0/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/autoaction.py` & `naludaq-0.20.0/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.20.0/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/board_backup.py` & `naludaq-0.20.0/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.20.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/data_collector.py` & `naludaq-0.20.0/src/naludaq/tools/data_collector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+import logging
 import time
 from collections import deque
 
 from naludaq.board import Board
 from naludaq.communication import AnalogRegisters, ControlRegisters, DigitalRegisters
 from naludaq.controllers import get_board_controller, get_readout_controller
+from naludaq.daq import get_daq
+from naludaq.helpers.helper_functions import event_transfer_time
+from naludaq.tools import EventWaiter
 
-# from naludaq.tools.pedestals.pedestals_controller import sleep_calc, increase_margin
+# from naludaq.tools.pedestals.pedestals_controller import sleep_calc,
+
+LOGGER = logging.getLogger("naludaq.ConversionRampOptimizer")
 
 
 class DataCollector:
     def __init__(self, daq, board: Board):
         """Wrapper for the standard readout procedure for most Nalu Scientific ASICs
 
         Takes all of the configuration settings for readout and updates the settings to the chip
@@ -20,15 +26,15 @@
             daq (BenDaq, LightDaq): The Data acquisition object that the DataCollector will use to
                 interface with the chip
             board (Board): The Board object that has the proper parameters and connection to the
                 physical board
         """
 
         self.board = board
-        self.daq = daq
+        self._daq = daq
         self.default_margin = 1.1
         self.margin = self.default_margin
         self.sleeptime = sleep_calc(board, self.margin)
 
     @property
     def board(self):
         return self._board
@@ -109,44 +115,44 @@
         self._validate_readout_settings(readout_settings)
         self._validate_window_settings(window_settings)
         self._validate_channel_settings(channels)
         if amount < 1:
             raise ValueError(f"amount cannot be less than 1")
 
         output_buffer = deque(maxlen=amount)
-        self.daq.output_buffer = output_buffer
+        self._daq.output_buffer = output_buffer
         desired_amount = amount
         reset_count = 0
         self.margin = self.default_margin
         rdt_controller.set_read_window(**window_settings)
         rdt_controller.set_readout_channels(channels)
         while len(output_buffer) < amount:
             desired_amount = amount - len(output_buffer)
             if desired_amount <= 0:
                 break
 
             self.sleeptime = sleep_calc(self.board, self.margin)
 
             rdt_controller.number_events_to_read(desired_amount)
-            self.daq.start_capture()
+            self._daq.start_capture()
             get_board_controller(self.board).start_readout(**readout_settings)
 
             finished = self._wait_for_data(output_buffer, desired_amount)
 
             if not finished:
                 if reset_count >= timeout:
                     raise TimeoutError(
                         f"Something wrong with setup/hardware, "
                         f"reset {timeout} times still no data."
                     )
                 reset_count += 1
                 self.margin = increase_margin(self.margin)
                 self.sleeptime = sleep_calc(self.board, self.margin)
 
-            self.daq.stop_capture()
+            self._daq.stop_capture()
             get_board_controller(self.board).stop_readout()
 
         return output_buffer
 
     def _wait_for_data(self, output_buffer, desired_amount):
         """Wait for the desired amount of data to arrive.
 
@@ -273,14 +279,115 @@
         if not set(channels).issubset(valid_channels):
             raise TypeError(
                 f"{channels} is not in range of valid channels for this board model. \
                 Valid range is from 0 to {self.board.params['channels']}"
             )
 
 
+class UPACDataCollector:
+    def __init__(self, board: Board):
+        """Wrapper for the standard readout procedure for UPAC boards
+
+        Takes all of the configuration settings for readout and updates the settings to the chip
+        when readout is commenced. The Data Collector is very specific with its settings, and will
+        only take in the correctly formatted settings.
+
+        Args:
+            daq (BenDaq, LightDaq): The Data acquisition object that the DataCollector will use to
+                interface with the chip
+            board (Board): The Board object that has the proper parameters and connection to the
+                physical board
+        """
+
+        self.board = board
+
+        self._daq = get_daq(board, parsed=True)
+        self.default_margin = 1.1
+        self._parse_events = True
+        self.timeout = event_transfer_time(
+            board,
+            board.params["windows"],
+            margin=self.default_margin,
+            overhead=3,
+        )
+
+    @property
+    def board(self):
+        return self._board
+
+    @board.setter
+    def board(self, board):
+        self._board = board
+
+    def get_events(
+        self,
+        amount: int,
+        num_attempts: int = 3,
+    ) -> deque:
+        """Returns an exact amount of pre-processed events!
+
+        The return is sizelimited to `amount` by a circular buffer, it'll overwrite the oldest data
+        if the board returns too much data. This is by design and can't be changed.
+
+
+        ## Readout Settings Explanation:
+            `trig_type` (trigger_type):
+                'imm' (immediate): digitize whatever instantly as fast as possible.
+                'ext' (external): use the external trigger.
+                'self' (self): trigger on input RF signal. Uses trigger values
+
+        Args:
+            `amount` (int): desired amount of events, cannot be less than 1
+            `trig_type` (string): How the trigger runs for the acquisition
+            `timeout` (int): timeout in retries per event.
+
+        Returns:
+            A deque with the events, raw or processed depending on the daq.
+
+        Raises:
+            `ValueError` if amount is < 1.
+            `TimeoutError` if no data is captured in `timeout` retries.
+        """
+
+        if amount < 1:
+            raise ValueError(f"amount cannot be less than 1")
+
+        output_buffer = deque(maxlen=amount)
+        self._daq.output_buffer = output_buffer
+
+        bc = get_board_controller(self.board)
+        bc.clear_buffer()
+
+        self._daq.start_capture()
+        time.sleep(0.1)
+        bc.set_continuous_mode(True)
+        bc.start_readout("software")
+        for _ in range(amount):
+            new_amount = len(self._daq.output_buffer) + 1
+            evt_waiter = EventWaiter(self._daq.output_buffer, new_amount)
+            evt_waiter.timeout = self.timeout
+            for attempt in range(num_attempts):
+                try:
+                    bc.toggle_trigger()
+                    evt_waiter.start()
+                except TimeoutError:
+                    continue
+                if attempt + 1 == num_attempts:
+                    bc.stop_readout()
+                    self._daq.stop_capture()
+                    raise TimeoutError(
+                        f"Unable to capture events after {num_attempts} attempts"
+                    )
+                break
+
+        bc.stop_readout()
+        self._daq.stop_capture()
+        return self._daq.output_buffer
+
+
 def increase_margin(margin: float, margin_inc: float = 1.5, max_margin: float = 5):
     """Increases the margin, using an exponential standoff"""
     margin *= margin_inc
     margin = min(margin, max_margin)
     return margin
```

### Comparing `naludaq-0.19.0/src/naludaq/tools/features.py` & `naludaq-0.20.0/src/naludaq/tools/features.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,22 @@
         beta_models=get_available_models(),
     ),
     "ext_dac": Feature(
         description="External DAC",
         long_description="Allows control of the external DAC on the board",
         beta_models=[],
     ),
+    "conversion_ramp_optimizer": Feature(
+        description="Amplitude Linearity Optimizer",
+        long_description=(
+            "Calibrates isel Ramp Current and Cap Select to put individual"
+            "channels in the midrange, which can help with amplitude linearity"
+        ),
+        beta_models=get_available_models(),
+    ),
     "gain_stage_tuner": Feature(
         description="Gain Stage Tuner",
         long_description=(
             "Calibrates external dac and ISEL for a specific "
             "gain stage configuration"
         ),
         beta_models=get_available_models(),
```

### Comparing `naludaq-0.19.0/src/naludaq/tools/ft60x.py` & `naludaq-0.20.0/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/ftdi.py` & `naludaq-0.20.0/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table.py` & `naludaq-0.20.0/src/naludaq/tools/lookup_table/lookup_table.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table_generator.py` & `naludaq-0.20.0/src/naludaq/tools/lookup_table/lookup_table_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/metadata.py` & `naludaq-0.20.0/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.20.0/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.20.0/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/__init__.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/_new/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/aav3.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/_new/aav3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/default.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/_new/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 import numpy as np
 
 from naludaq.backend.managers import AcquisitionManager
 from naludaq.backend.models.acquisition import RemoteAcquisition
 from naludaq.board import Board
 from naludaq.communication import ControlRegisters, DigitalRegisters
 from naludaq.controllers import get_board_controller, get_readout_controller
-from naludaq.helpers.exceptions import OperationCanceledError, PedestalsDataCaptureError
+from naludaq.helpers.exceptions import (
+    OperationCanceledError,
+    PedestalsDataCaptureError,
+    PedestalsIOError,
+)
 from naludaq.helpers.helper_functions import event_transfer_time
 from naludaq.tools.metadata import Metadata
 
 LOGGER = logging.getLogger(
     "naludaq.pedestals_controller_new"
 )  # pylint: disable=invalid-name
 
@@ -164,15 +168,15 @@
     def metadata(self) -> Metadata:
         """Get a proxy object to use for accessing pedestals metadata."""
         return Metadata(self.board.pedestals)
 
     @property
     def raw_events(self) -> list[dict]:
         """List of events used to last generate the pedestals.
-        
+
         These events are parsed, and otherwise not modified in any way.
         They can be used for analysis! 🥳🎉
         """
         return self._debug_raw_events
 
     def generate_pedestals(self):
         """Generates pedestals and stores them in the board.pedestals.
@@ -584,18 +588,18 @@
         path, _ = os.path.split(filename)
         if not os.path.isdir(path):
             raise NotADirectoryError(f"Not a valid directory: {path}")
 
         try:
             with gzip.GzipFile(filename, "wb", compresslevel=4) as f:
                 pickle.dump(pedestals, f, protocol=pickle.HIGHEST_PROTOCOL)
-        except IOError as error_msg:
-            LOGGER.error("File could not be created. %s", error_msg)
-        except pickle.PicklingError as error_msg:
-            LOGGER.error("Saving pedestals failed: %s", error_msg)
+        except IOError as e:
+            raise PedestalsIOError(f"File could not be written: {e}")
+        except pickle.PicklingError as e:
+            raise PedestalsIOError(f"Object cannot be serialized: {e}")
 
     def load_pedestals(self, filename):  # TODO(v.0.1.23): Use IO module.
         """Load the pedestal gziped and pickled.
 
         The pedestals object is loaded to both self.pedestals
         and is returned.
 
@@ -606,20 +610,20 @@
             Pedestals data.
         """
         if not os.path.isfile(filename):
             raise FileNotFoundError(f"No file found: {filename}")
         try:
             with gzip.GzipFile(filename, "rb") as f:
                 outped = pickle.load(f)
-        except EOFError as error_msg:
-            LOGGER.error("Reached the end of the file, msg: %s", error_msg)
-        except IOError as error_msg:
-            LOGGER.error("File could not be loaded. %s", error_msg)
-        except pickle.UnpicklingError as error_msg:
-            LOGGER.error("Loading pedestals failed: %s", error_msg)
+        except EOFError:
+            raise PedestalsIOError("Unexpected end of file")
+        except IOError as e:
+            raise PedestalsIOError(f"File could not be loaded: {e}")
+        except pickle.UnpicklingError as e:
+            raise PedestalsIOError(f"Not a valid pickle file: {e}")
         else:
             if not isinstance(outped, dict):
                 raise TypeError(f"Not a valid Pedestals file: {filename}")
             self.board.pedestals = outped
             return outped
 
     # ================================================================================
```

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/hdsoc.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/_new/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_acq.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_acq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_controller.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from naludaq.communication import control_registers, digital_registers
 from naludaq.controllers import get_board_controller, get_readout_controller
 from naludaq.daq import get_daq
 from naludaq.helpers.exceptions import (
     NotAValidEvent,
     OperationCanceledError,
     PedestalsDataCaptureError,
+    PedestalsIOError,
 )
 from naludaq.io import io_manager
 from naludaq.tools.metadata import Metadata
 
 LOGGER = logging.getLogger(
     "naludaq.pedestals_controller"
 )  # pylint: disable=invalid-name
@@ -805,18 +806,18 @@
         path, _ = os.path.split(filename)
         if not os.path.isdir(path):
             raise NotADirectoryError(f"Not a valid directory: {path}")
 
         try:
             sfile = gzip.GzipFile(filename, "w", compresslevel=4)
             pickle.dump(pedestals, sfile, protocol=pickle.HIGHEST_PROTOCOL)
-        except IOError as error_msg:
-            LOGGER.error("File could not be created. %s", error_msg)
-        except pickle.PicklingError as error_msg:
-            LOGGER.error("Saving pedestals failed: %s", error_msg)
+        except IOError as e:
+            raise PedestalsIOError(f"File could not be written: {e}")
+        except pickle.PicklingError as e:
+            raise PedestalsIOError(f"Object cannot be serialized: {e}")
 
     def load_pedestals(self, filename):  # TODO(v.0.1.23): Use IO module.
         """Load the pedestal gziped and pickled.
 
         The pedestals object is loaded to both self.pedestals
         and is returned.
 
@@ -903,20 +904,20 @@
     """
     if not os.path.isfile(filename):
         raise FileNotFoundError(f"No file found: {filename}")
 
     try:
         sfile = gzip.GzipFile(filename, "r")
         outped = pickle.load(sfile)
-    except EOFError as error_msg:
-        LOGGER.error("Reached the end of the file, msg: %s", error_msg)
-    except IOError as error_msg:
-        LOGGER.error("File could not be loaded. %s", error_msg)
-    except pickle.UnpicklingError as error_msg:
-        LOGGER.error("Loading pedestals failed: %s", error_msg)
+    except EOFError:
+        raise PedestalsIOError("Unexpected end of file")
+    except IOError as e:
+        raise PedestalsIOError(f"File could not be loaded: {e}")
+    except pickle.UnpicklingError as e:
+        raise PedestalsIOError(f"Not a valid pickle file: {e}")
     else:
         if not isinstance(outped, dict):
             raise TypeError(f"Not a valid Pedestals file: {filename}")
 
         return outped
 
 
@@ -929,15 +930,15 @@
     Args:
         receiver (list, deque, or ProgressDialog): the receiver of the progress update.
             Can be None to report nothing
         percent (float): the percent completion of the task
         message (str): a description of what is currently taking place
     """
     if receiver is None:
-        LOGGER.deubg("%s | %s", percent, message)
+        LOGGER.debug("%s | %s", percent, message)
         return
     elif isinstance(receiver, (list, deque)):
         receiver.append((percent, message))
     else:
         try:
             receiver.update_status(percent, message)
         except:
```

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py` & `naludaq-0.20.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.20.0/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.20.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.20.0/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.20.0/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.20.0/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.20.0/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.19.0/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.20.0/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class EventWaiter(AutoAction):
     def __init__(
         self,
         buffer,
         amount,
         interval: "float | Callable" = 0.1,
-        timeout=1,
+        timeout: float = 1.0,
         reset_timeout=False,
     ) -> None:
         """Module for waiting for when a buffer (events) is filled to a specified amount
 
         Args:
             buffer: A list like object that stores events
             amount (int): Desired amount of events for the buffer to be filled, before waiter stops
```

### Comparing `naludaq-0.19.0/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.20.0/src/naludaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.19.0
+Version: 0.20.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.19.0/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.20.0/src/naludaq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,17 @@
 src/naludaq/tools/dac_sweep/dac_sweep_controller.py
 src/naludaq/tools/lookup_table/__init__.py
 src/naludaq/tools/lookup_table/lookup_table.py
 src/naludaq/tools/lookup_table/lookup_table_generator.py
 src/naludaq/tools/optimizers/__init__.py
 src/naludaq/tools/optimizers/bayesian_optimizer.py
 src/naludaq/tools/optimizers/gainstagetuner.py
+src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+src/naludaq/tools/optimizers/conversion_ramp/upac96.py
 src/naludaq/tools/pedestals/__init__.py
 src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
 src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
 src/naludaq/tools/pedestals/pedestals_acq.py
 src/naludaq/tools/pedestals/pedestals_controller.py
 src/naludaq/tools/pedestals/pedestals_correcter.py
 src/naludaq/tools/pedestals/pedestals_processor.py
```

