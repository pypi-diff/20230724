# Comparing `tmp/piel-0.0.43.tar.gz` & `tmp/piel-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.43.tar", last modified: Thu Jul 13 21:52:33 2023, max compression
+gzip compressed data, was "piel-0.0.44.tar", last modified: Mon Jul 24 11:38:09 2023, max compression
```

## Comparing `piel-0.0.43.tar` & `piel-0.0.44.tar`

### file list

```diff
@@ -1,386 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 21:52:16.000000 piel-0.0.43/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 21:52:16.000000 piel-0.0.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 21:52:16.000000 piel-0.0.43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-13 21:52:33.605553 piel-0.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-13 21:52:16.000000 piel-0.0.43/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-13 21:52:16.000000 piel-0.0.43/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.565553 piel-0.0.43/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/_static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-13 21:52:16.000000 piel-0.0.43/docs/_static/img/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/config/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/file_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/file_conversion/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/file_system/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    47512 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/cocotb_sax/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/cocotb_sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/core/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/pyspice_sax/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/pyspice_sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/sax_thewalrus/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/sax_thewalrus/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/all/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/all/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/ideal/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/cable/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/cable/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/basic_heater/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/capacitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/capacitor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/defaults/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/resistor/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/resistor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/thermal/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/units/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/units/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/project_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/project_structure/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27444 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/pyspice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/pyspice/component/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/pyspice/component/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/pyspice/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/sax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/sax/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/data_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/data_conversion/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-13 21:52:16.000000 piel-0.0.43/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 21:52:16.000000 piel-0.0.43/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 21:52:16.000000 piel-0.0.43/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-13 21:52:16.000000 piel-0.0.43/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/about/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/components/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/developer_docker_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/cocotb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/gdsfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/openlane.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/principle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/pyspice.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/sax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/integration/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/integration/sax_qutip.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/models/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 21:52:16.000000 piel-0.0.43/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 21:52:16.000000 piel-0.0.43/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 21:52:16.000000 piel-0.0.43/piel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 21:52:16.000000 piel-0.0.43/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 21:52:16.000000 piel-0.0.43/piel/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-13 21:52:16.000000 piel-0.0.43/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/cocotb_sax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_openlane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/integration/gdsfactory_pyspice/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/pyspice_sax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/sax_qutip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/sax_thewalrus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electro_optic/ideal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/grating_coupler.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/mmi1x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/mmi2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/straight_waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electro_optic/signal_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/photonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electrical/cable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electro_optic/basic_heater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electronic/spice/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/resistor.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-13 21:52:16.000000 piel-0.0.43/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-13 21:52:16.000000 piel-0.0.43/piel/project_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/tools/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/gdsfactory/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/run_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/pyspice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/pyspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/pyspice/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/sax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/visual/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/auto_plot_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 21:52:33.609554 piel-0.0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 21:52:16.000000 piel-0.0.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 21:52:16.000000 piel-0.0.43/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-13 21:52:16.000000 piel-0.0.43/tests/integration/test_gdsfactory_netlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-13 21:52:16.000000 piel-0.0.43/tests/integration/test_gdsfactory_netlist_to_pyspice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/tests/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-13 21:52:16.000000 piel-0.0.43/tests/models/logic/electro_optic/test_signal_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 21:52:16.000000 piel-0.0.43/tests/test_piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/gdsfactory/test_netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/sax/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/visual/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-13 21:52:16.000000 piel-0.0.43/tests/visual/test_data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-24 11:37:50.000000 piel-0.0.44/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 11:37:50.000000 piel-0.0.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-24 11:37:50.000000 piel-0.0.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-24 11:38:09.500708 piel-0.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 11:37:50.000000 piel-0.0.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.460707 piel-0.0.44/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-24 11:37:50.000000 piel-0.0.44/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-24 11:37:50.000000 piel-0.0.44/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.444707 piel-0.0.44/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.460707 piel-0.0.44/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-24 11:37:50.000000 piel-0.0.44/docs/_static/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   491705 2023-07-24 11:37:50.000000 piel-0.0.44/docs/_static/img/piel_microservice_structure.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/file_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/file_conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47846 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/cocotb_sax/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/cocotb_sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/sax_qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/sax_qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/sax_thewalrus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/sax_thewalrus/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/integration/thewalrus_qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/integration/thewalrus_qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/all/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/electro_optic/ideal/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.464707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/frequency/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/frequency/utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/logic/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electrical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electrical/cable/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electrical/cable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electro_optic/basic_heater/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/capacitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/capacitor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/defaults/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/resistor/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/resistor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/straight/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/straight/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/taper/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/taper/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/via_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/electronic/via_stack/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/thermal/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/physical/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/physical/units/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.468707 piel-0.0.44/docs/autoapi/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/transient/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/models/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/project_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/project_structure/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/cocotb/core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/cocotb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/cocotb/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/netlist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/hdl21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/hdl21/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/hdl21/circuit/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/hdl21/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/hdl21/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/hdl21/simulator/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/hdl21/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/hdl21/units/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29951 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/qutip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/qutip/fock/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/qutip/fock/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/qutip/unitary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/qutip/unitary/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/sax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/sax/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/thewalrus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/thewalrus/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/tools/thewalrus/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/tools/thewalrus/operations/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.472707 piel-0.0.44/docs/autoapi/piel/visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/autoapi/piel/visual/auto_plot_multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/autoapi/piel/visual/data_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/visual/data_conversion/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-24 11:37:50.000000 piel-0.0.44/docs/autoapi/piel/visual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-24 11:37:50.000000 piel-0.0.44/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 11:37:50.000000 piel-0.0.44/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.452707 piel-0.0.44/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.452707 piel-0.0.44/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.452707 piel-0.0.44/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.452707 piel-0.0.44/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 11:37:50.000000 piel-0.0.44/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-24 11:37:50.000000 piel-0.0.44/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 11:37:50.000000 piel-0.0.44/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 11:37:50.000000 piel-0.0.44/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 11:37:50.000000 piel-0.0.44/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.456707 piel-0.0.44/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/environment/developer_docker_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/environment/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/microservices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.476707 piel-0.0.44/docs/sections/microservices/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/cocotb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/gdsfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/openlane.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/principle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/sax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/dependencies/spice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.480707 piel-0.0.44/docs/sections/microservices/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/microservices/integration/sax_qutip.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.480707 piel-0.0.44/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/models/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-24 11:37:50.000000 piel-0.0.44/docs/sections/models/spice_integration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.480707 piel-0.0.44/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 11:37:50.000000 piel-0.0.44/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 11:37:50.000000 piel-0.0.44/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.480707 piel-0.0.44/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-24 11:37:50.000000 piel-0.0.44/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-24 11:37:50.000000 piel-0.0.44/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 11:37:50.000000 piel-0.0.44/piel/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-24 11:37:50.000000 piel-0.0.44/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/cocotb_sax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/integration/gdsfactory_hdl21/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/gdsfactory_hdl21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/gdsfactory_hdl21/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/gdsfactory_hdl21/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/gdsfactory_hdl21/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/gdsfactory_openlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/sax_qutip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/sax_thewalrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-24 11:37:50.000000 piel-0.0.44/piel/integration/thewalrus_qutip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/electro_optic/ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.484707 piel-0.0.44/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/photonic/straight_waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/frequency/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/electro_optic/signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.488708 piel-0.0.44/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electro_optic/basic_heater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/resistor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/straight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/electronic/via_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:37:50.000000 piel-0.0.44/piel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-24 11:37:50.000000 piel-0.0.44/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-24 11:37:50.000000 piel-0.0.44/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.492708 piel-0.0.44/piel/tools/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/cocotb/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/gdsfactory/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/hdl21/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/hdl21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/hdl21/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/hdl21/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/hdl21/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/parse/run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/openlane/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/qutip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/qutip/fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/qutip/unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.496708 piel-0.0.44/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/sax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/piel/tools/thewalrus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/thewalrus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 11:37:50.000000 piel-0.0.44/piel/tools/thewalrus/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/piel/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 11:37:50.000000 piel-0.0.44/piel/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-24 11:37:50.000000 piel-0.0.44/piel/visual/auto_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-24 11:37:50.000000 piel-0.0.44/piel/visual/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.480707 piel-0.0.44/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 11:38:09.000000 piel-0.0.44/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 11:38:09.500708 piel-0.0.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-24 11:37:50.000000 piel-0.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 11:37:50.000000 piel-0.0.44/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 11:37:50.000000 piel-0.0.44/tests/integration/test_gdsfactory_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-24 11:37:50.000000 piel-0.0.44/tests/integration/test_gdsfactory_netlist_to_pyspice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.460707 piel-0.0.44/tests/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-24 11:37:50.000000 piel-0.0.44/tests/models/logic/electro_optic/test_signal_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-24 11:37:50.000000 piel-0.0.44/tests/models/test_generator_call_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 11:37:50.000000 piel-0.0.44/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 11:37:50.000000 piel-0.0.44/tests/tools/gdsfactory/test_netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-24 11:37:50.000000 piel-0.0.44/tests/tools/sax/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 11:37:50.000000 piel-0.0.44/tests/tools/test_hdl21.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:38:09.500708 piel-0.0.44/tests/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-24 11:37:50.000000 piel-0.0.44/tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.43/CONTRIBUTING.rst` & `piel-0.0.44/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/LICENSE` & `piel-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/PKG-INFO` & `piel-0.0.44/docs/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,11 @@
-Metadata-Version: 2.1
-Name: piel
-Version: 0.0.43
-Summary: Photonic Integrated Electronics: microservices to codesign photonics, electronics, communications, quantum, and more.
-Home-page: https://github.com/daquintero/piel
-Author: Dario Quintero
-Author-email: darioaquintero@gmail.com
-License: MIT license
-Keywords: piel
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 **P**\hotonic **I**\ntegrated **EL**\ectronics
 ===============================================
 
-|PyPI Version| |Build Status| |Documentation Status| |Updates|
+|PyPI Name| |PyPI Version| |Build Status| |Documentation Status| |MIT| |Black|
 
 Microservices to codesign photonics, electronics, communications,
 quantum, and more.
 
 -  Free software: MIT license
 -  Documentation: https://piel.readthedocs.io
 
@@ -45,41 +23,50 @@
 and electronics, classically and quantum. It does not aim to replace the
 individual functionality of each design tool, but rather provide a glue
 to easily connect them all together and extract the system performance.
 
 Examples
 --------
 
-Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+Follow the many `examples in the documentation <https://piel.readthedocs.io/en/latest/examples.html>`__.
 
 Microservices Toolset
 ---------------------
 
 This package provides interconnection functions to easily co-design
 microelectronics through the functionality of the
 `IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
 photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
 
+.. image:: _static/img/piel_microservice_structure.png
+
 Some existing microservice dependency integrations are:
 
 * `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* `hdl21 <https://github.com/dan-fritchman/Hdl21>`__ - Analog Hardware Description Library in Python
 * `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
 * `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
 * `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
 * `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
 
 Contribution
 ------------
 
 If you feel dedicated enough to become a project maintainer, or just
 want to do a single contribution, let's do this together!
 
-.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
-   :target: https://pypi.python.org/pypi/piel
+
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
 .. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
    :target: https://travis-ci.com/daquintero/piel
 .. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
    :target: https://piel.readthedocs.io/en/latest/?version=latest
+.. |MIT| image:: https://img.shields.io/github/license/gdsfactory/gdsfactory
+   :target: https://choosealicense.com/licenses/mit/
+.. |PyPI Name| image:: https://img.shields.io/badge/pypi-piel-blue
+   :target: https://pypi.python.org/pypi/piel
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
+   :target: https://pypi.python.org/pypi/piel
 .. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
    :target: https://pyup.io/repos/github/daquintero/piel/
```

### Comparing `piel-0.0.43/README.rst` & `piel-0.0.44/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,72 @@
-**P**\hotonic **I**\ntegrated **EL**\ectronics
-===============================================
+# **P**hotonic **I**ntegrated **EL**ectronics
 
-|PyPI Version| |Build Status| |Documentation Status| |Updates|
+[![PyPI
+Name](https://img.shields.io/badge/pypi-piel-blue)](https://pypi.python.org/pypi/piel)
+[![PyPI
+Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
+[![Build
+Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
+[![Documentation
+Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
+[![MIT](https://img.shields.io/github/license/gdsfactory/gdsfactory)](https://choosealicense.com/licenses/mit/)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Microservices to codesign photonics, electronics, communications,
 quantum, and more.
 
--  Free software: MIT license
--  Documentation: https://piel.readthedocs.io
+-   Free software: MIT license
+-   Documentation: <https://piel.readthedocs.io>
 
-Target functionality
---------------------
+## Target functionality
 
--  Co-simulation and optimisation between integrated photonic and
-   electronic chip design.
--  System interconnection modelling in multiple domains.
--  Chip and interposer design integration.
--  Component models translation library between simulation tools.
--  Quantum models of physical circuitry.
+-   Co-simulation and optimisation between integrated photonic and
+    electronic chip design.
+-   System interconnection modelling in multiple domains.
+-   Chip and interposer design integration.
+-   Component models translation library between simulation tools.
+-   Quantum models of physical circuitry.
 
-``piel`` aims to provide an integrated workflow to co-design photonics
-and electronics, classically and quantum. It does not aim to replace the
+`piel` aims to provide an integrated workflow to co-design photonics and
+electronics, classically and quantum. It does not aim to replace the
 individual functionality of each design tool, but rather provide a glue
 to easily connect them all together and extract the system performance.
 
-Examples
---------
+## Examples
 
-Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+Follow the many [examples in the
+documentation](https://piel.readthedocs.io/en/latest/examples.html).
 
-Microservices Toolset
----------------------
+## Microservices Toolset
 
 This package provides interconnection functions to easily co-design
 microelectronics through the functionality of the
-`IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
-photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
+[IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and
+photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+
+![image](docs/_static/img/piel_microservice_structure.png)
 
 Some existing microservice dependency integrations are:
 
-* `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
-* `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
-* `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
-* `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
-* `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
-* `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
+-   [cocotb](https://github.com/cocotb/cocotb) - a coroutine based
+    cosimulation library for writing VHDL and Verilog testbenches in
+    Python.
+-   [hdl21](https://github.com/dan-fritchman/Hdl21) - Analog Hardware
+    Description Library in Python
+-   [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open
+    source platform for end to-end photonic chip design and validation
+-   [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an
+    automated RTL to GDSII flow based on several components including
+    OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for
+    design exploration and optimization
+-   [sax](https://github.com/flaport/sax) - S-parameter based frequency
+    domain circuit simulations and optimizations using JAX.
+-   [thewalrus](https://github.com/XanaduAI/thewalrus) -A library for
+    the calculation of hafnians, Hermite polynomials and Gaussian boson
+    sampling.
+-   [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in
+    Python
 
-Contribution
-------------
+## Contribution
 
 If you feel dedicated enough to become a project maintainer, or just
-want to do a single contribution, let's do this together!
-
-.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
-   :target: https://pypi.python.org/pypi/piel
-.. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
-   :target: https://travis-ci.com/daquintero/piel
-.. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
-   :target: https://piel.readthedocs.io/en/latest/?version=latest
-.. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
-   :target: https://pyup.io/repos/github/daquintero/piel/
+want to do a single contribution, let\'s do this together!
```

### Comparing `piel-0.0.43/docs/Makefile` & `piel-0.0.44/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/_static/img/logo.png` & `piel-0.0.44/docs/_static/img/logo.png`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/file_conversion/index.rst` & `piel-0.0.44/docs/autoapi/piel/file_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.44/docs/autoapi/piel/file_system/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/index.rst` & `piel-0.0.44/docs/autoapi/piel/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,22 @@
    piel.permit_script_execution
    piel.setup_example_design
    piel.read_json
    piel.return_path
    piel.run_script
    piel.write_script
    piel.create_gdsfactory_component_from_openlane
-   piel.gdsfactory_netlist_to_pyspice
-   piel.spice_netlist_to_pyspice_circuit
    piel.gdsfactory_netlist_to_spice_netlist
-   piel.sax_to_s_parameters_standard_matrix
-   piel.unitary_permanent
+   piel.construct_hdl21_module
+   piel.convert_connections_to_tuples
+   piel.gdsfactory_netlist_with_hdl21_generators
    piel.sax_circuit_permanent
+   piel.unitary_permanent
    piel.sax_to_ideal_qutip_unitary
-   piel.standard_s_parameters_to_ideal_qutip_unitary
+   piel.fock_transition_probability_amplitude
    piel.single_parameter_sweep
    piel.multi_parameter_sweep
    piel.check_cocotb_testbench_exists
    piel.configure_cocotb_simulation
    piel.run_cocotb_simulation
    piel.get_simulation_output_files_from_design
    piel.read_simulation_data
@@ -107,45 +107,42 @@
    piel.get_all_timing_data_from_file
    piel.read_sta_rpt_fwf_file
    piel.contains_in_lines
    piel.create_file_lines_dataframe
    piel.get_file_line_by_keyword
    piel.read_file_lines
    piel.run_openlane_flow
+   piel.convert_numeric_to_prefix
    piel.get_sdense_ports_index
    piel.sax_to_s_parameters_standard_matrix
+   piel.fock_state_nonzero_indexes
+   piel.fock_state_to_photon_number_factorial
+   piel.verify_matrix_is_unitary
+   piel.subunitary_selection_on_range
+   piel.subunitary_selection_on_index
 
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.numerical_solver
-   piel.nso
    piel.piel_path_types
    piel.test_spm_open_lane_configuration
    piel.example_open_lane_configuration
    piel.delete_simulation_output_files
    piel.get_simulation_output_files
    piel.snet
+   piel.standard_s_parameters_to_qutip_qobj
    piel.__author__
    piel.__email__
    piel.__version__
 
 
-.. py:data:: numerical_solver
-
-
-
-.. py:data:: nso
-
-
-
 .. py:data:: piel_path_types
 
 
 
 .. py:data:: test_spm_open_lane_configuration
 
 
@@ -336,275 +333,194 @@
    :param v1: If True, it will import the design from the OpenLane v1 configuration.
    :type v1: bool
 
    :returns: GDSFactory component.
    :rtype: component(gf.Component)
 
 
-.. py:function:: gdsfactory_netlist_to_pyspice(gdsfactory_netlist: dict, return_raw_spice: bool = False)
+.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, generators: dict, **kwargs) -> hdl21.Module
 
-   This function converts a GDSFactory electrical netlist into a standard PySpice configuration. It follows the same
-   principle as the `sax` circuit composition. It returns a PySpice circuit and can return it in raw_spice form if
-   necessary.
+   This function converts a GDSFactory electrical netlist into a standard SPICE netlist. It follows the same
+   principle as the `sax` circuit composition.
 
    Each GDSFactory netlist has a set of instances, each with a corresponding model, and each instance with a given
    set of geometrical settings that can be applied to each particular model. We know the type of SPICE model from
    the instance model we provides.
 
    We know that the gdsfactory has a set of instances, and we can map unique models via sax through our own
    composition circuit. Write the SPICE component based on the model into a total circuit representation in string
    from the reshaped gdsfactory dictionary into our own structure.
 
+   :param gdsfactory_netlist: GDSFactory netlist
+   :param generators: Dictionary of Generators
 
-.. py:function:: spice_netlist_to_pyspice_circuit(spice_netlist: dict)
+   :returns: hdl21 module or raw SPICE string
 
-   This function converts a SPICE netlist into a PySpice circuit.
-
-   # TODO implement validators
 
+.. py:function:: construct_hdl21_module(spice_netlist: dict, **kwargs) -> hdl21.Module
 
-.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, models=None)
+   This function converts a gdsfactory-spice converted netlist using the component models into a SPICE circuit.
 
-   This function maps the connections of a netlist to a node that can be used in a SPICE netlist. SPICE netlists are
-   in the form of:
+   Part of the complexity of this function is the multiport nature of some components and models, and assigning the
+   parameters accordingly into the SPICE function. This is because not every SPICE component will be bi-port,
+   and many will have multi-ports and parameters accordingly. Each model can implement the composition into a
+   SPICE circuit, but they depend on a set of parameters that must be set from the instance. Another aspect is
+   that we may want to assign the component ID according to the type of component. However, we can also assign the
+   ID based on the individual instance in the circuit, which is also a reasonable approximation. However,
+   it could be said, that the ideal implementation would be for each component model provided to return the SPICE
+   instance including connectivity except for the ID.
 
-   .. code-block::
-
-       RXXXXXXX N1 N2 <VALUE> <MNAME> <L=LENGTH> <W=WIDTH> <TEMP=T>
-
-   This means that every instance, is an electrical type, and we define the two particular nodes in which it is
-   connected. This means we need to convert the gdsfactory dictionary netlist into a form that allows us to map the
-   connectivity for every instance. Then we can define that as a line of the SPICE netlist with a particular
-   electrical model. For passives this works fine when it's a two port network such as sources, or electrical
-   elements. However, non-passive elements like transistors have three ports or more which are provided in an ordered form.
-
-   This means that the order of translations is as follows:
+   # TODO implement validators
 
-   .. code-block::
 
-       1. Extract all instances and required models from the netlist
-       2. Verify that the models have been provided. Each model describes the type of component this is, how many ports it requires and so on.
-       3. Map the connections to each instance port as part of the instance dictionary.
+.. py:function:: convert_connections_to_tuples(connections: dict)
 
-   We should get as an output a dictionary in the structure:
+   Convert from:
 
    .. code-block::
 
        {
-           instance_1: {
-               ...
-               "connections": [('straight_1,e1', 'taper_1,e2'),
-                               ('straight_1,e2', 'taper_2,e2')],
-               'spice_nets': {'e1': 'straight_1__e1___taper_1__e2',
-                       'e2': 'straight_1__e2___taper_2__e2'},
-               'spice_model': <function piel.models.physical.electronic.spice.resistor.basic_resistor()>},
-           }
-           ...
+       'straight_1,e1': 'taper_1,e2',
+       'straight_1,e2': 'taper_2,e2',
+       'taper_1,e1': 'via_stack_1,e3',
+       'taper_2,e1': 'via_stack_2,e1'
        }
 
+   to:
 
-.. py:function:: sax_to_s_parameters_standard_matrix(sax_input: sax.SType, input_ports_order: tuple | None = None) -> tuple
-
-   A ``sax`` S-parameter SDict is provided as a dictionary of tuples with (port0, port1) as the key. This
-   determines the direction of the scattering relationship. It means that the number of terms in an S-parameter
-   matrix is the number of ports squared.
-
-   In order to generalise, this function returns both the S-parameter matrices and the indexing ports based on the
-   amount provided. In terms of computational speed, we definitely would like this function to be algorithmically
-   very fast. For now, I will write a simple python implementation and optimise in the future.
-
-   It is possible to see the `sax` SDense notation equivalence here:
-   https://flaport.github.io/sax/nbs/08_backends.html
+   .. code-block::
 
-   .. code-block:: python
+       [(('straight_1', 'e1'), ('taper_1', 'e2')), (('straight_1', 'e2'), ('taper_2', 'e2')), (('taper_1', 'e1'),
+       ('via_stack_1', 'e3')), (('taper_2', 'e1'), ('via_stack_2', 'e1'))]
 
-       import jax.numpy as jnp
-       from sax.core import SDense
-
-       # Directional coupler SDense representation
-       dc_sdense: SDense = (
-           jnp.array([[0, 0, τ, κ], [0, 0, κ, τ], [τ, κ, 0, 0], [κ, τ, 0, 0]]),
-           {"in0": 0, "in1": 1, "out0": 2, "out1": 3},
-       )
 
+.. py:function:: gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist: dict, generators=None)
 
-       # Directional coupler SDict representation
-       # Taken from https://flaport.github.io/sax/nbs/05_models.html
-       def coupler(*, coupling: float = 0.5) -> SDict:
-           kappa = coupling**0.5
-           tau = (1 - coupling) ** 0.5
-           sdict = reciprocal(
-               {
-                   ("in0", "out0"): tau,
-                   ("in0", "out1"): 1j * kappa,
-                   ("in1", "out0"): 1j * kappa,
-                   ("in1", "out1"): tau,
-               }
-           )
-           return sdict
+   This function allows us to map the ``hdl21`` models dictionary in a `sax`-like implementation to the ``GDSFactory`` netlist. This allows us to iterate over each instance in the netlist and construct a circuit after this function.]
 
-   If we were to relate the mapping accordingly based on the ports indexes, a S-Parameter matrix in the form of
-   :math:`S_{(output,i),(input,i)}` would be:
+   Example usage:
 
-   .. math::
+   .. code-block::
 
-       S = \begin{bmatrix}
-               S_{00} & S_{10} \\
-               S_{01} & S_{11} \\
-           \end{bmatrix} =
-           \begin{bmatrix}
-           \tau & j \kappa \\
-           j \kappa & \tau \\
-           \end{bmatrix}
+       >>> import gdsfactory as gf
+       >>> from piel.integration.gdsfactory_hdl21.conversion import gdsfactory_netlist_with_hdl21_generators
+       >>> from piel.models.physical.electronic import get_default_models
+       >>> gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist=gf.components.mzi2x2_2x2_phase_shifter().get_netlist(exclude_port_types="optical"),generators=get_default_models())
 
-   Note that the standard S-parameter and hence unitary representation is in the form of:
+   :param gdsfactory_netlist: The netlist from ``GDSFactory`` to map to the ``hdl21`` models dictionary.
+   :param generators: The ``hdl21`` models dictionary to map to the ``GDSFactory`` netlist.
 
-   .. math::
+   :returns: The ``GDSFactory`` netlist with the ``hdl21`` models dictionary.
 
-       S = \begin{bmatrix}
-               S_{00} & S_{01} \\
-               S_{10} & S_{11} \\
-           \end{bmatrix}
 
+.. py:function:: sax_circuit_permanent(sax_input: sax.SType) -> tuple
 
-   .. math::
+   The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
 
-       \begin{bmatrix}
-           b_{1} \\
-           \vdots \\
-           b_{n}
-       \end{bmatrix}
-       =
-       \begin{bmatrix}
-           S_{11} & \dots & S_{1n} \\
-           \vdots & \ddots & \vdots \\
-           S_{n1} & \dots & S_{nn}
-       \end{bmatrix}
-       \begin{bmatrix}
-           a_{1} \\
-           \vdots \\
-           a_{n}
-       \end{bmatrix}
+   ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
 
-   TODO check with Floris, does this mean we need to transpose the matrix?
+   # TODO maybe implement subroutine if computation is taking forever.
 
    :param sax_input: The sax S-parameter dictionary.
    :type sax_input: sax.SType
-   :param input_ports_order: The ports order tuple containing the names and order of the input ports.
-   :type input_ports_order: tuple
 
-   :returns: The S-parameter matrix and the input ports index tuple in the standard S-parameter notation.
+   :returns: The circuit permanent and the time it took to compute it.
    :rtype: tuple
 
 
-.. py:function:: unitary_permanent(unitary_matrix: numpy.ndarray) -> tuple
+.. py:function:: unitary_permanent(unitary_matrix: jax.numpy.ndarray) -> tuple
 
    The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
 
    ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
 
+   Note that this function needs to be as optimised as possible, so we need to minimise our computational complexity of our operation.
+
+   # TODO implement validation
    # TODO maybe implement subroutine if computation is taking forever.
    # TODO why two outputs? Understand this properly later.
 
    :param unitary_permanent: The unitary matrix.
    :type unitary_permanent: np.ndarray
 
    :returns: The circuit permanent and the time it took to compute it.
    :rtype: tuple
 
 
-.. py:function:: sax_circuit_permanent(sax_input: sax.SType) -> tuple
-
-   The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
-
-   ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
-
-   # TODO maybe implement subroutine if computation is taking forever.
-
-   :param sax_input: The sax S-parameter dictionary.
-   :type sax_input: sax.SType
-
-   :returns: The circuit permanent and the time it took to compute it.
-   :rtype: tuple
-
-
 .. py:function:: sax_to_ideal_qutip_unitary(sax_input: sax.SType)
 
    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
    dimensions of the matrix can be observed.
 
    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
    already in described in piel/piel/sax/utils.py.
 
    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly.
    https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
    For example, a ``qutip`` representation of an s-gate gate would be:
 
-   ..code-block:: python
+   ..code-block::
 
        import numpy as np
        import qutip
        # S-Gate
        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
+           1 & 0 \\
+           0 & i \\
        \end{bmatrix}
 
    :param sax_input: A dictionary of S-parameters in the form of a SDict from `sax`.
    :type sax_input: sax.SType
 
    :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
    :rtype: qobj_unitary (qutip.Qobj)
 
 
-.. py:function:: standard_s_parameters_to_ideal_qutip_unitary(s_parameters_standard_matrix: piel.config.nso.ndarray)
+.. py:function:: fock_transition_probability_amplitude(initial_fock_state: qutip.Qobj, final_fock_state: qutip.Qobj, unitary_matrix: jax.numpy.ndarray)
 
-   This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-   dimensions of the matrix can be observed.
+       This function returns the transition probability amplitude between two Fock states when propagating in between
+       the unitary_matrix which represents a quantum state circuit.
 
-   I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-   Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
-   already in described in piel/piel/sax/utils.py.
-
-   From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
-
-   For example, a ``qutip`` representation of an s-gate gate would be:
+       Note that based on (TODO cite Jeremy), the initial Fock state corresponds to the columns of the unitary and the
+       final Fock states corresponds to the rows of the unitary.
 
-   ..code-block:: python
+       .. math ::
 
-       import numpy as np
-       import qutip
+   ewcommand{\ket}[1]{\left|{#1}
+   ight
+   angle}
 
-       # S-Gate
-       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
-       s_gate = qutip.Qobj(mat, dims=[[2], [2]])
+       The subunitary :math:`U_{f_1}^{f_2}` is composed from the larger unitary by selecting the rows from the output state
+       Fock state occupation of :math:`\ket{f_2}`, and columns from the input :math:`\ket{f_1}`. In our case, we need to select the
+       columns indexes :math:`(0,3)` and rows indexes :math:`(1,2)`.
 
-   In mathematical notation, this S-gate would be written as:
+       If we consider a photon number of more than one for the transition Fock states, then the Permanent needs to be
+       normalised. The probability amplitude for the transition is described as:
 
-   ..math::
+       .. math ::
+           a(\ket{f_1}     o \ket{f_2}) =
+   rac{    ext{per}(U_{f_1}^{f_2})}{\sqrt{(j_1! j_2! ... j_N!)(j_1^{'}! j_2^{'}! ... j_N^{'}!)}}
 
-       S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
-       \end{bmatrix}
+       Args:
+           initial_fock_state (qutip.Qobj): A QuTip QObj representation of the initial Fock state.
+           final_fock_state (qutip.Qobj): A QuTip QObj representation of the final Fock state.
+           unitary_matrix (jnp.ndarray): A JAX NumPy array representation of the unitary matrix.
 
-   :param s_parameters_standard_matrix: A dictionary of S-parameters in the form of a SDict from `sax`.
-   :type s_parameters_standard_matrix: nso.ndarray
+       Returns:
+           float: The transition probability amplitude between the initial and final Fock states.
 
-   :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
-   :rtype: qobj_unitary (qutip.Qobj)
 
 
 .. py:function:: single_parameter_sweep(base_design_configuration: dict, parameter_name: str, parameter_sweep_values: list)
 
    This function takes a base_design_configuration dictionary and sweeps a single parameter over a list of values. It returns a list of dictionaries that correspond to the parameter sweep.
 
    :param base_design_configuration: Base design configuration dictionary.
@@ -1224,14 +1140,19 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: piel_path_types
 
    :returns: None
 
 
+.. py:function:: convert_numeric_to_prefix(value: float)
+
+   This function converts a numeric value to a number under a SPICE unit closest to the base prefix. This allows us to connect a particular number real output, into a term that can be used in a SPICE netlist.
+
+
 .. py:function:: get_sdense_ports_index(input_ports_order: tuple, all_ports_index: dict) -> dict
 
    This function returns the ports index of the sax dense S-parameter matrix.
 
    Given that the order of the iteration is provided by the user, the dictionary keys will also be ordered
    accordingly when iterating over them. This requires the user to provide a set of ordered.
 
@@ -1358,19 +1279,86 @@
    :rtype: tuple
 
 
 .. py:data:: snet
 
 
 
+.. py:function:: fock_state_nonzero_indexes(fock_state: qutip.Qobj)
+
+   This function returns the indexes of the nonzero elements of a Fock state.
+
+   :param fock_state: A QuTip QObj representation of the Fock state.
+   :type fock_state: qutip.Qobj
+
+   :returns: The indexes of the nonzero elements of the Fock state.
+   :rtype: tuple
+
+
+.. py:function:: fock_state_to_photon_number_factorial(fock_state: qutip.Qobj)
+
+       This function converts a Fock state defined as:
+
+       .. math::
+
+   ewcommand{\ket}[1]{\left|{#1}
+   ight
+   angle}
+           \ket{f_1} = \ket{j_1, j_2, ... j_N}$
+
+       and returns:
+
+       .. math::
+
+           j_1^{'}! j_2^{'}! ... j_N^{'}!
+
+       Args:
+           fock_state (qutip.Qobj): A QuTip QObj representation of the Fock state.
+
+       Returns:
+           float: The photon number factorial of the Fock state.
+
+
+
+.. py:data:: standard_s_parameters_to_qutip_qobj
+
+
+
+.. py:function:: verify_matrix_is_unitary(matrix: jax.numpy.ndarray) -> bool
+
+   Verify that the matrix is unitary.
+
+   :param matrix: The matrix to verify.
+   :type matrix: jnp.ndarray
+
+   :returns: True if the matrix is unitary, False otherwise.
+   :rtype: bool
+
+
+.. py:function:: subunitary_selection_on_range(unitary_matrix: jax.numpy.ndarray, stop_index: tuple, start_index: Optional[tuple] = (0, 0))
+
+   This function returns a unitary between the indexes selected, and verifies the indexes are valid by checking that
+   the output matrix is also a unitary.
+
+   TODO implement validation of a 2D matrix.
+
+
+.. py:function:: subunitary_selection_on_index(unitary_matrix: jax.numpy.ndarray, rows_index: jax.numpy.ndarray | tuple, columns_index: jax.numpy.ndarray | tuple)
+
+   This function returns a unitary between the indexes selected, and verifies the indexes are valid by checking that
+   the output matrix is also a unitary.
+
+   TODO implement validation of a 2D matrix.
+
+
 .. py:data:: __author__
    :value: 'Dario Quintero'
 
 
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
 
 
 .. py:data:: __version__
-   :value: '0.0.42'
+   :value: '0.0.43'
```

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/core/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/core/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-:py:mod:`piel.integration.gdsfactory_pyspice.core`
-==================================================
+:py:mod:`piel.integration.gdsfactory_hdl21.core`
+================================================
 
-.. py:module:: piel.integration.gdsfactory_pyspice.core
+.. py:module:: piel.integration.gdsfactory_hdl21.core
 
 .. autoapi-nested-parse::
 
-   Most of the ``pyspice``-``gdsfactory`` integration functions will be contributed directly to `gdsfactory`. However,
+   Most of the ``hdl21``-``gdsfactory`` integration functions will be contributed directly to `gdsfactory`. However,
    some `translation language` inherent to the ``piel`` implementation of these tools is included here.
 
    Note that to be able to construct a full circuit model of the netlist tools provided, it is necessary to create
    individual circuit models of the devices that we will interconnect, and then map them to a larger netlist. This means
    that it is necessary to create specific SPICE models for each particular component, say in an electrical netlist.
 
-   This functions convert a GDSFactory netlist, with a set of component models, into `PySPICE` that accounts for the
+   This functions convert a GDSFactory netlist, with a set of component models, into `hdl21` that accounts for the
    instance properties, which can then be connected into a VLSIR compatible `Netlist` implementation.
 
    Eventually we will implement RCX where we can extract the netlist with parasitics directly from the layout,
    but for now this will be the implementation. The output structure of our SPICE should be compatible with the
    `Netlist` package BaseModel.
 
    We follow the principle in: https://eee.guc.edu.eg/Courses/Electronics/ELCT503%20Semiconductors/Lab/spicehowto.pdf
 
-   .. code-block::
+   .. code-block:: spice
 
        Spice Simulation 1-1
        *** MODEL Descriptions ***
        .model nm NMOS level=2 VT0=0.7
        KP=80e-6 LAMBDA=0.01
 
        *** NETLIST Description ***
@@ -36,15 +36,15 @@
 
        *** SIMULATION Commands ***
        .op
        .end
 
    Note that the netlist device connectivity structure of most passive components is in the form:
 
-   .. code-block::
+   .. code-block:: spice
 
        <DEVICE ID> <CONNECTION_0> <CONNECTION_1> <DEVICE_VALUE> <MORE_PARAMETERS>
 
    Our example GDSFactory netlist format is in the simplified form:
 
    .. code-block::
 
@@ -147,49 +147,100 @@
                "e2": "taper_2,e2"
            },
            "name": "straight_heater_metal_simple",
        }
 
    This is particularly useful when creating our components and connectivity, because what we can do is instantiate our
    devices with their corresponding values, and then create our connectivity accordingly. To do this properly from our
-   GDSFactory netlist to PySpice, we can then extract the total SPICE circuit, and convert it to a VLSIR format using
-   the `Netlist` module. The reason why we can't use the Netlist package from Dan Fritchman directly is that we need to
+   GDSFactory netlist to ``hdl21``, we can then extract the total SPICE circuit, and convert it to a VLSIR format using
+   the ``Netlist`` module. The reason why we can't use the Netlist package from Dan Fritchman directly is that we need to
    apply a set of models that translate a particular component instantiation into an electrical model. Because we are
    not yet doing layout extraction as that requires EM solvers, we need to create some sort of SPICE level assignment
    based on the provided dictionary.
 
+   Note that ``hdl21`` already can implement the port connectivity directly from internal instances, and translate this
+   to our connectivity netlist. This means we only need to iterate to create our instances based on our models into a
+   ``hdl21`` module, then we can easily assign the corresponding values. It is also possible to create the assigned
+   parameters as part of the ``hdl21`` component which would form part of our module. Because the gdsfactory names are
+   compatible with ``hdl21``, then it is fine to create the integration accordingly.
+
+   The algorithm can be to:
+
+   1. Parse the gdsfactory netlist, assign the electrical ports for the model. Extract all instances and
+   required models from the netlist.
+   2. Verify that the models have been provided. Each model describes the type of
+   component this is, how many ports it requires and so on. Create a ``hdl21`` top level module for every gdsfactory
+   netlist, this is reasonable as it is composed, and not a generator class. This generates a large amount of instantiated ``hdl21`` modules that are generated from `generators`.
+   3. Map the connections to each instance port as part of the instance dictionary. This parses the connectivity in the ``gdsfactory`` netlist and connects the ports accordingly.
+
+   The connections are a bit more complex. So each of our connections dictionary is in the form:
+
+   .. code-block::
+
+        "connections": {
+                   "straight_1": {
+                       "e1": "taper_1,e2",
+                       "e2": "taper_2,e2"
+                   },
+                   "taper_1": {
+                       "e1": "via_stack_1,e3"
+                   },
+                   "taper_2": {
+                       "e1": "via_stack_2,e1"
+                   }
+               },
+
+   We know what our top model ports are. We know our internal instance ports as well, and this will be provided by the
+   model too. For the sake of easiness, we can describe these as ``hdl21`` equivalent ``InOut`` or ``Port` `ports and
+   not have to deal with directionality. After instance declaration, and models for each of these components with the
+   corresponding port topology, it is then straightforward to parse the connectivity and implement the network,
+   and extract the SPICE.
+
 
 
 Module Contents
 ---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.integration.gdsfactory_pyspice.core.gdsfactory_netlist_to_pyspice
-   piel.integration.gdsfactory_pyspice.core.spice_netlist_to_pyspice_circuit
+   piel.integration.gdsfactory_hdl21.core.gdsfactory_netlist_to_spice_netlist
+   piel.integration.gdsfactory_hdl21.core.construct_hdl21_module
 
 
 
-.. py:function:: gdsfactory_netlist_to_pyspice(gdsfactory_netlist: dict, return_raw_spice: bool = False)
+.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, generators: dict, **kwargs) -> hdl21.Module
 
-   This function converts a GDSFactory electrical netlist into a standard PySpice configuration. It follows the same
-   principle as the `sax` circuit composition. It returns a PySpice circuit and can return it in raw_spice form if
-   necessary.
+   This function converts a GDSFactory electrical netlist into a standard SPICE netlist. It follows the same
+   principle as the `sax` circuit composition.
 
    Each GDSFactory netlist has a set of instances, each with a corresponding model, and each instance with a given
    set of geometrical settings that can be applied to each particular model. We know the type of SPICE model from
    the instance model we provides.
 
    We know that the gdsfactory has a set of instances, and we can map unique models via sax through our own
    composition circuit. Write the SPICE component based on the model into a total circuit representation in string
    from the reshaped gdsfactory dictionary into our own structure.
 
+   :param gdsfactory_netlist: GDSFactory netlist
+   :param generators: Dictionary of Generators
+
+   :returns: hdl21 module or raw SPICE string
+
+
+.. py:function:: construct_hdl21_module(spice_netlist: dict, **kwargs) -> hdl21.Module
 
-.. py:function:: spice_netlist_to_pyspice_circuit(spice_netlist: dict)
+   This function converts a gdsfactory-spice converted netlist using the component models into a SPICE circuit.
 
-   This function converts a SPICE netlist into a PySpice circuit.
+   Part of the complexity of this function is the multiport nature of some components and models, and assigning the
+   parameters accordingly into the SPICE function. This is because not every SPICE component will be bi-port,
+   and many will have multi-ports and parameters accordingly. Each model can implement the composition into a
+   SPICE circuit, but they depend on a set of parameters that must be set from the instance. Another aspect is
+   that we may want to assign the component ID according to the type of component. However, we can also assign the
+   ID based on the individual instance in the circuit, which is also a reasonable approximation. However,
+   it could be said, that the ideal implementation would be for each component model provided to return the SPICE
+   instance including connectivity except for the ID.
 
    # TODO implement validators
```

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/conversion/index.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,68 @@
-:py:mod:`piel.integration.gdsfactory_pyspice`
-=============================================
+:py:mod:`piel.integration.gdsfactory_hdl21.conversion`
+======================================================
 
-.. py:module:: piel.integration.gdsfactory_pyspice
+.. py:module:: piel.integration.gdsfactory_hdl21.conversion
 
+.. autoapi-nested-parse::
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
+   `sax` has very good GDSFactory integration functions, so there is a question on whether implementing our own circuit
+   construction, and SPICE netlist parser from it, accordingly. We need in some form to connect electrical models to our
+   parsed netlist, in order to apply SPICE passive values, and create connectivity for each particular device. Ideally,
+   this would be done from the component instance as that way the component model can be integrated with its geometrical
+   parameters, but does not have to be done necessarily. This comes down to implementing a backend function to compile
+   SAX compiled circuit.
 
-   conversion/index.rst
-   core/index.rst
-   utils/index.rst
 
 
-Package Contents
-----------------
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.integration.gdsfactory_pyspice.gdsfactory_netlist_to_pyspice
-   piel.integration.gdsfactory_pyspice.spice_netlist_to_pyspice_circuit
-   piel.integration.gdsfactory_pyspice.gdsfactory_netlist_to_spice_netlist
+   piel.integration.gdsfactory_hdl21.conversion.convert_connections_to_tuples
+   piel.integration.gdsfactory_hdl21.conversion.gdsfactory_netlist_with_hdl21_generators
 
 
 
-.. py:function:: gdsfactory_netlist_to_pyspice(gdsfactory_netlist: dict, return_raw_spice: bool = False)
+.. py:function:: convert_connections_to_tuples(connections: dict)
 
-   This function converts a GDSFactory electrical netlist into a standard PySpice configuration. It follows the same
-   principle as the `sax` circuit composition. It returns a PySpice circuit and can return it in raw_spice form if
-   necessary.
+   Convert from:
 
-   Each GDSFactory netlist has a set of instances, each with a corresponding model, and each instance with a given
-   set of geometrical settings that can be applied to each particular model. We know the type of SPICE model from
-   the instance model we provides.
-
-   We know that the gdsfactory has a set of instances, and we can map unique models via sax through our own
-   composition circuit. Write the SPICE component based on the model into a total circuit representation in string
-   from the reshaped gdsfactory dictionary into our own structure.
-
-
-.. py:function:: spice_netlist_to_pyspice_circuit(spice_netlist: dict)
-
-   This function converts a SPICE netlist into a PySpice circuit.
+   .. code-block::
 
-   # TODO implement validators
+       {
+       'straight_1,e1': 'taper_1,e2',
+       'straight_1,e2': 'taper_2,e2',
+       'taper_1,e1': 'via_stack_1,e3',
+       'taper_2,e1': 'via_stack_2,e1'
+       }
 
+   to:
 
-.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, models=None)
+   .. code-block::
 
-   This function maps the connections of a netlist to a node that can be used in a SPICE netlist. SPICE netlists are
-   in the form of:
+       [(('straight_1', 'e1'), ('taper_1', 'e2')), (('straight_1', 'e2'), ('taper_2', 'e2')), (('taper_1', 'e1'),
+       ('via_stack_1', 'e3')), (('taper_2', 'e1'), ('via_stack_2', 'e1'))]
 
-   .. code-block::
 
-       RXXXXXXX N1 N2 <VALUE> <MNAME> <L=LENGTH> <W=WIDTH> <TEMP=T>
+.. py:function:: gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist: dict, generators=None)
 
-   This means that every instance, is an electrical type, and we define the two particular nodes in which it is
-   connected. This means we need to convert the gdsfactory dictionary netlist into a form that allows us to map the
-   connectivity for every instance. Then we can define that as a line of the SPICE netlist with a particular
-   electrical model. For passives this works fine when it's a two port network such as sources, or electrical
-   elements. However, non-passive elements like transistors have three ports or more which are provided in an ordered form.
+   This function allows us to map the ``hdl21`` models dictionary in a `sax`-like implementation to the ``GDSFactory`` netlist. This allows us to iterate over each instance in the netlist and construct a circuit after this function.]
 
-   This means that the order of translations is as follows:
+   Example usage:
 
    .. code-block::
 
-       1. Extract all instances and required models from the netlist
-       2. Verify that the models have been provided. Each model describes the type of component this is, how many ports it requires and so on.
-       3. Map the connections to each instance port as part of the instance dictionary.
-
-   We should get as an output a dictionary in the structure:
+       >>> import gdsfactory as gf
+       >>> from piel.integration.gdsfactory_hdl21.conversion import gdsfactory_netlist_with_hdl21_generators
+       >>> from piel.models.physical.electronic import get_default_models
+       >>> gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist=gf.components.mzi2x2_2x2_phase_shifter().get_netlist(exclude_port_types="optical"),generators=get_default_models())
 
-   .. code-block::
+   :param gdsfactory_netlist: The netlist from ``GDSFactory`` to map to the ``hdl21`` models dictionary.
+   :param generators: The ``hdl21`` models dictionary to map to the ``GDSFactory`` netlist.
 
-       {
-           instance_1: {
-               ...
-               "connections": [('straight_1,e1', 'taper_1,e2'),
-                               ('straight_1,e2', 'taper_2,e2')],
-               'spice_nets': {'e1': 'straight_1__e1___taper_1__e2',
-                       'e2': 'straight_1__e2___taper_2__e2'},
-               'spice_model': <function piel.models.physical.electronic.spice.resistor.basic_resistor()>},
-           }
-           ...
-       }
+   :returns: The ``GDSFactory`` netlist with the ``hdl21`` models dictionary.
```

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/utils/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/gdsfactory_hdl21/utils/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-:py:mod:`piel.integration.gdsfactory_pyspice.utils`
-===================================================
+:py:mod:`piel.integration.gdsfactory_hdl21.utils`
+=================================================
 
-.. py:module:: piel.integration.gdsfactory_pyspice.utils
+.. py:module:: piel.integration.gdsfactory_hdl21.utils
 
 
 Module Contents
 ---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.integration.gdsfactory_pyspice.utils.rename_gdsfactory_connections_to_spice
-   piel.integration.gdsfactory_pyspice.utils.convert_tuples_to_strings
+   piel.integration.gdsfactory_hdl21.utils.rename_gdsfactory_connections_to_spice
+   piel.integration.gdsfactory_hdl21.utils.convert_tuples_to_strings
 
 
 
 .. py:function:: rename_gdsfactory_connections_to_spice(connections: dict)
 
    We convert the connection connectivity of the gdsfactory netlist into names that can be integrated into a SPICE
    netlist. It iterates on each key value pair, and replaces each comma with an underscore.
```

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 
 Subpackages
 -----------
 .. toctree::
    :titlesonly:
    :maxdepth: 3
 
-   gdsfactory_pyspice/index.rst
+   gdsfactory_hdl21/index.rst
 
 
 Submodules
 ----------
 .. toctree::
    :titlesonly:
    :maxdepth: 1
 
    cocotb_sax/index.rst
    gdsfactory_openlane/index.rst
-   pyspice_sax/index.rst
    sax_qutip/index.rst
    sax_thewalrus/index.rst
+   thewalrus_qutip/index.rst
 
 
 Package Contents
 ----------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
    piel.integration.create_gdsfactory_component_from_openlane
-   piel.integration.gdsfactory_netlist_to_pyspice
-   piel.integration.spice_netlist_to_pyspice_circuit
    piel.integration.gdsfactory_netlist_to_spice_netlist
-   piel.integration.sax_to_s_parameters_standard_matrix
-   piel.integration.unitary_permanent
+   piel.integration.construct_hdl21_module
+   piel.integration.convert_connections_to_tuples
+   piel.integration.gdsfactory_netlist_with_hdl21_generators
    piel.integration.sax_circuit_permanent
+   piel.integration.unitary_permanent
    piel.integration.sax_to_ideal_qutip_unitary
-   piel.integration.standard_s_parameters_to_ideal_qutip_unitary
+   piel.integration.fock_transition_probability_amplitude
 
 
 
 .. py:function:: create_gdsfactory_component_from_openlane(design_name_v1: str | None = None, design_directory: piel.config.piel_path_types | None = None, run_name: str | None = None, v1: bool = True) -> gdsfactory.Component
 
    This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
 
@@ -62,196 +62,118 @@
    :param v1: If True, it will import the design from the OpenLane v1 configuration.
    :type v1: bool
 
    :returns: GDSFactory component.
    :rtype: component(gf.Component)
 
 
-.. py:function:: gdsfactory_netlist_to_pyspice(gdsfactory_netlist: dict, return_raw_spice: bool = False)
+.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, generators: dict, **kwargs) -> hdl21.Module
 
-   This function converts a GDSFactory electrical netlist into a standard PySpice configuration. It follows the same
-   principle as the `sax` circuit composition. It returns a PySpice circuit and can return it in raw_spice form if
-   necessary.
+   This function converts a GDSFactory electrical netlist into a standard SPICE netlist. It follows the same
+   principle as the `sax` circuit composition.
 
    Each GDSFactory netlist has a set of instances, each with a corresponding model, and each instance with a given
    set of geometrical settings that can be applied to each particular model. We know the type of SPICE model from
    the instance model we provides.
 
    We know that the gdsfactory has a set of instances, and we can map unique models via sax through our own
    composition circuit. Write the SPICE component based on the model into a total circuit representation in string
    from the reshaped gdsfactory dictionary into our own structure.
 
+   :param gdsfactory_netlist: GDSFactory netlist
+   :param generators: Dictionary of Generators
 
-.. py:function:: spice_netlist_to_pyspice_circuit(spice_netlist: dict)
-
-   This function converts a SPICE netlist into a PySpice circuit.
-
-   # TODO implement validators
-
+   :returns: hdl21 module or raw SPICE string
 
-.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, models=None)
 
-   This function maps the connections of a netlist to a node that can be used in a SPICE netlist. SPICE netlists are
-   in the form of:
-
-   .. code-block::
+.. py:function:: construct_hdl21_module(spice_netlist: dict, **kwargs) -> hdl21.Module
 
-       RXXXXXXX N1 N2 <VALUE> <MNAME> <L=LENGTH> <W=WIDTH> <TEMP=T>
+   This function converts a gdsfactory-spice converted netlist using the component models into a SPICE circuit.
 
-   This means that every instance, is an electrical type, and we define the two particular nodes in which it is
-   connected. This means we need to convert the gdsfactory dictionary netlist into a form that allows us to map the
-   connectivity for every instance. Then we can define that as a line of the SPICE netlist with a particular
-   electrical model. For passives this works fine when it's a two port network such as sources, or electrical
-   elements. However, non-passive elements like transistors have three ports or more which are provided in an ordered form.
+   Part of the complexity of this function is the multiport nature of some components and models, and assigning the
+   parameters accordingly into the SPICE function. This is because not every SPICE component will be bi-port,
+   and many will have multi-ports and parameters accordingly. Each model can implement the composition into a
+   SPICE circuit, but they depend on a set of parameters that must be set from the instance. Another aspect is
+   that we may want to assign the component ID according to the type of component. However, we can also assign the
+   ID based on the individual instance in the circuit, which is also a reasonable approximation. However,
+   it could be said, that the ideal implementation would be for each component model provided to return the SPICE
+   instance including connectivity except for the ID.
 
-   This means that the order of translations is as follows:
+   # TODO implement validators
 
-   .. code-block::
 
-       1. Extract all instances and required models from the netlist
-       2. Verify that the models have been provided. Each model describes the type of component this is, how many ports it requires and so on.
-       3. Map the connections to each instance port as part of the instance dictionary.
+.. py:function:: convert_connections_to_tuples(connections: dict)
 
-   We should get as an output a dictionary in the structure:
+   Convert from:
 
    .. code-block::
 
        {
-           instance_1: {
-               ...
-               "connections": [('straight_1,e1', 'taper_1,e2'),
-                               ('straight_1,e2', 'taper_2,e2')],
-               'spice_nets': {'e1': 'straight_1__e1___taper_1__e2',
-                       'e2': 'straight_1__e2___taper_2__e2'},
-               'spice_model': <function piel.models.physical.electronic.spice.resistor.basic_resistor()>},
-           }
-           ...
+       'straight_1,e1': 'taper_1,e2',
+       'straight_1,e2': 'taper_2,e2',
+       'taper_1,e1': 'via_stack_1,e3',
+       'taper_2,e1': 'via_stack_2,e1'
        }
 
+   to:
 
-.. py:function:: sax_to_s_parameters_standard_matrix(sax_input: sax.SType, input_ports_order: tuple | None = None) -> tuple
-
-   A ``sax`` S-parameter SDict is provided as a dictionary of tuples with (port0, port1) as the key. This
-   determines the direction of the scattering relationship. It means that the number of terms in an S-parameter
-   matrix is the number of ports squared.
-
-   In order to generalise, this function returns both the S-parameter matrices and the indexing ports based on the
-   amount provided. In terms of computational speed, we definitely would like this function to be algorithmically
-   very fast. For now, I will write a simple python implementation and optimise in the future.
-
-   It is possible to see the `sax` SDense notation equivalence here:
-   https://flaport.github.io/sax/nbs/08_backends.html
-
-   .. code-block:: python
-
-       import jax.numpy as jnp
-       from sax.core import SDense
-
-       # Directional coupler SDense representation
-       dc_sdense: SDense = (
-           jnp.array([[0, 0, τ, κ], [0, 0, κ, τ], [τ, κ, 0, 0], [κ, τ, 0, 0]]),
-           {"in0": 0, "in1": 1, "out0": 2, "out1": 3},
-       )
-
-
-       # Directional coupler SDict representation
-       # Taken from https://flaport.github.io/sax/nbs/05_models.html
-       def coupler(*, coupling: float = 0.5) -> SDict:
-           kappa = coupling**0.5
-           tau = (1 - coupling) ** 0.5
-           sdict = reciprocal(
-               {
-                   ("in0", "out0"): tau,
-                   ("in0", "out1"): 1j * kappa,
-                   ("in1", "out0"): 1j * kappa,
-                   ("in1", "out1"): tau,
-               }
-           )
-           return sdict
-
-   If we were to relate the mapping accordingly based on the ports indexes, a S-Parameter matrix in the form of
-   :math:`S_{(output,i),(input,i)}` would be:
-
-   .. math::
-
-       S = \begin{bmatrix}
-               S_{00} & S_{10} \\
-               S_{01} & S_{11} \\
-           \end{bmatrix} =
-           \begin{bmatrix}
-           \tau & j \kappa \\
-           j \kappa & \tau \\
-           \end{bmatrix}
+   .. code-block::
 
-   Note that the standard S-parameter and hence unitary representation is in the form of:
+       [(('straight_1', 'e1'), ('taper_1', 'e2')), (('straight_1', 'e2'), ('taper_2', 'e2')), (('taper_1', 'e1'),
+       ('via_stack_1', 'e3')), (('taper_2', 'e1'), ('via_stack_2', 'e1'))]
 
-   .. math::
 
-       S = \begin{bmatrix}
-               S_{00} & S_{01} \\
-               S_{10} & S_{11} \\
-           \end{bmatrix}
+.. py:function:: gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist: dict, generators=None)
 
+   This function allows us to map the ``hdl21`` models dictionary in a `sax`-like implementation to the ``GDSFactory`` netlist. This allows us to iterate over each instance in the netlist and construct a circuit after this function.]
 
-   .. math::
+   Example usage:
 
-       \begin{bmatrix}
-           b_{1} \\
-           \vdots \\
-           b_{n}
-       \end{bmatrix}
-       =
-       \begin{bmatrix}
-           S_{11} & \dots & S_{1n} \\
-           \vdots & \ddots & \vdots \\
-           S_{n1} & \dots & S_{nn}
-       \end{bmatrix}
-       \begin{bmatrix}
-           a_{1} \\
-           \vdots \\
-           a_{n}
-       \end{bmatrix}
+   .. code-block::
 
-   TODO check with Floris, does this mean we need to transpose the matrix?
+       >>> import gdsfactory as gf
+       >>> from piel.integration.gdsfactory_hdl21.conversion import gdsfactory_netlist_with_hdl21_generators
+       >>> from piel.models.physical.electronic import get_default_models
+       >>> gdsfactory_netlist_with_hdl21_generators(gdsfactory_netlist=gf.components.mzi2x2_2x2_phase_shifter().get_netlist(exclude_port_types="optical"),generators=get_default_models())
 
-   :param sax_input: The sax S-parameter dictionary.
-   :type sax_input: sax.SType
-   :param input_ports_order: The ports order tuple containing the names and order of the input ports.
-   :type input_ports_order: tuple
+   :param gdsfactory_netlist: The netlist from ``GDSFactory`` to map to the ``hdl21`` models dictionary.
+   :param generators: The ``hdl21`` models dictionary to map to the ``GDSFactory`` netlist.
 
-   :returns: The S-parameter matrix and the input ports index tuple in the standard S-parameter notation.
-   :rtype: tuple
+   :returns: The ``GDSFactory`` netlist with the ``hdl21`` models dictionary.
 
 
-.. py:function:: unitary_permanent(unitary_matrix: numpy.ndarray) -> tuple
+.. py:function:: sax_circuit_permanent(sax_input: sax.SType) -> tuple
 
    The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
 
    ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
 
    # TODO maybe implement subroutine if computation is taking forever.
-   # TODO why two outputs? Understand this properly later.
 
-   :param unitary_permanent: The unitary matrix.
-   :type unitary_permanent: np.ndarray
+   :param sax_input: The sax S-parameter dictionary.
+   :type sax_input: sax.SType
 
    :returns: The circuit permanent and the time it took to compute it.
    :rtype: tuple
 
 
-.. py:function:: sax_circuit_permanent(sax_input: sax.SType) -> tuple
+.. py:function:: unitary_permanent(unitary_matrix: jax.numpy.ndarray) -> tuple
 
    The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
 
    ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
 
+   Note that this function needs to be as optimised as possible, so we need to minimise our computational complexity of our operation.
+
+   # TODO implement validation
    # TODO maybe implement subroutine if computation is taking forever.
+   # TODO why two outputs? Understand this properly later.
 
-   :param sax_input: The sax S-parameter dictionary.
-   :type sax_input: sax.SType
+   :param unitary_permanent: The unitary matrix.
+   :type unitary_permanent: np.ndarray
 
    :returns: The circuit permanent and the time it took to compute it.
    :rtype: tuple
 
 
 .. py:function:: sax_to_ideal_qutip_unitary(sax_input: sax.SType)
 
@@ -263,67 +185,63 @@
    already in described in piel/piel/sax/utils.py.
 
    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly.
    https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
    For example, a ``qutip`` representation of an s-gate gate would be:
 
-   ..code-block:: python
+   ..code-block::
 
        import numpy as np
        import qutip
        # S-Gate
        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
+           1 & 0 \\
+           0 & i \\
        \end{bmatrix}
 
    :param sax_input: A dictionary of S-parameters in the form of a SDict from `sax`.
    :type sax_input: sax.SType
 
    :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
    :rtype: qobj_unitary (qutip.Qobj)
 
 
-.. py:function:: standard_s_parameters_to_ideal_qutip_unitary(s_parameters_standard_matrix: piel.config.nso.ndarray)
-
-   This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-   dimensions of the matrix can be observed.
-
-   I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-   Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
-   already in described in piel/piel/sax/utils.py.
-
-   From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
+.. py:function:: fock_transition_probability_amplitude(initial_fock_state: qutip.Qobj, final_fock_state: qutip.Qobj, unitary_matrix: jax.numpy.ndarray)
 
-   For example, a ``qutip`` representation of an s-gate gate would be:
+       This function returns the transition probability amplitude between two Fock states when propagating in between
+       the unitary_matrix which represents a quantum state circuit.
 
-   ..code-block:: python
+       Note that based on (TODO cite Jeremy), the initial Fock state corresponds to the columns of the unitary and the
+       final Fock states corresponds to the rows of the unitary.
 
-       import numpy as np
-       import qutip
+       .. math ::
 
-       # S-Gate
-       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
-       s_gate = qutip.Qobj(mat, dims=[[2], [2]])
+   ewcommand{\ket}[1]{\left|{#1}
+   ight
+   angle}
 
-   In mathematical notation, this S-gate would be written as:
+       The subunitary :math:`U_{f_1}^{f_2}` is composed from the larger unitary by selecting the rows from the output state
+       Fock state occupation of :math:`\ket{f_2}`, and columns from the input :math:`\ket{f_1}`. In our case, we need to select the
+       columns indexes :math:`(0,3)` and rows indexes :math:`(1,2)`.
 
-   ..math::
+       If we consider a photon number of more than one for the transition Fock states, then the Permanent needs to be
+       normalised. The probability amplitude for the transition is described as:
 
-       S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
-       \end{bmatrix}
+       .. math ::
+           a(\ket{f_1}     o \ket{f_2}) =
+   rac{    ext{per}(U_{f_1}^{f_2})}{\sqrt{(j_1! j_2! ... j_N!)(j_1^{'}! j_2^{'}! ... j_N^{'}!)}}
 
-   :param s_parameters_standard_matrix: A dictionary of S-parameters in the form of a SDict from `sax`.
-   :type s_parameters_standard_matrix: nso.ndarray
+       Args:
+           initial_fock_state (qutip.Qobj): A QuTip QObj representation of the initial Fock state.
+           final_fock_state (qutip.Qobj): A QuTip QObj representation of the final Fock state.
+           unitary_matrix (jnp.ndarray): A JAX NumPy array representation of the unitary matrix.
 
-   :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
-   :rtype: qobj_unitary (qutip.Qobj)
+       Returns:
+           float: The transition probability amplitude between the initial and final Fock states.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/index.rst` & `piel-0.0.44/docs/autoapi/piel/integration/sax_qutip/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -9,86 +9,47 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.integration.sax_qutip.standard_s_parameters_to_ideal_qutip_unitary
    piel.integration.sax_qutip.sax_to_ideal_qutip_unitary
 
 
 
-.. py:function:: standard_s_parameters_to_ideal_qutip_unitary(s_parameters_standard_matrix: piel.config.nso.ndarray)
-
-   This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-   dimensions of the matrix can be observed.
-
-   I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-   Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
-   already in described in piel/piel/sax/utils.py.
-
-   From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
-
-   For example, a ``qutip`` representation of an s-gate gate would be:
-
-   ..code-block:: python
-
-       import numpy as np
-       import qutip
-
-       # S-Gate
-       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
-       s_gate = qutip.Qobj(mat, dims=[[2], [2]])
-
-   In mathematical notation, this S-gate would be written as:
-
-   ..math::
-
-       S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
-       \end{bmatrix}
-
-   :param s_parameters_standard_matrix: A dictionary of S-parameters in the form of a SDict from `sax`.
-   :type s_parameters_standard_matrix: nso.ndarray
-
-   :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
-   :rtype: qobj_unitary (qutip.Qobj)
-
-
 .. py:function:: sax_to_ideal_qutip_unitary(sax_input: sax.SType)
 
    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
    dimensions of the matrix can be observed.
 
    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
    already in described in piel/piel/sax/utils.py.
 
    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly.
    https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
    For example, a ``qutip`` representation of an s-gate gate would be:
 
-   ..code-block:: python
+   ..code-block::
 
        import numpy as np
        import qutip
        # S-Gate
        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
+           1 & 0 \\
+           0 & i \\
        \end{bmatrix}
 
    :param sax_input: A dictionary of S-parameters in the form of a SDict from `sax`.
    :type sax_input: sax.SType
 
    :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
    :rtype: qobj_unitary (qutip.Qobj)
```

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/defaults/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/frequency/utils/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/frequency/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/capacitor/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/physical/electronic/capacitor/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-:py:mod:`piel.models.physical.electronic.spice.capacitor`
-=========================================================
+:py:mod:`piel.models.physical.electronic.capacitor`
+===================================================
 
-.. py:module:: piel.models.physical.electronic.spice.capacitor
+.. py:module:: piel.models.physical.electronic.capacitor
 
 .. autoapi-nested-parse::
 
+   # TODO move and update.
    The way each of these models should work is that they use the settings from the `gdsfactory` component,
    to create a parametric SPICE directive.
 
    These functions map a particular model, with an instance representation that corresponds to the given netlist
-   connectivity, and returns a PySpice representation of the circuit. This function will be called after parsing the
+   connectivity, and returns a SPICE representation of the circuit. This function will be called after parsing the
    circuit netlist accordingly, and creating a mapping from the instance definitions to the fundamental components.
 
 
 
 Module Contents
 ---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.models.physical.electronic.spice.capacitor.add_basic_capacitor
+   piel.models.physical.electronic.capacitor.add_basic_capacitor
 
 
 
 .. py:function:: add_basic_capacitor(settings) -> str
 
    This function takes in the settings from a gdsfactory component, some connectivity node translated directly from
    the gdsfactory netlist.
```

### Comparing `piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/defaults/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/physical/electronic/defaults/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-:py:mod:`piel.models.physical.electronic.spice.defaults`
-========================================================
+:py:mod:`piel.models.physical.electronic.defaults`
+==================================================
 
-.. py:module:: piel.models.physical.electronic.spice.defaults
+.. py:module:: piel.models.physical.electronic.defaults
 
 
 Module Contents
 ---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.models.physical.electronic.spice.defaults.get_default_models
-
-
-
-Attributes
-~~~~~~~~~~
-
-.. autoapisummary::
-
-   piel.models.physical.electronic.spice.defaults.__default_models_dictionary__
-
-
-.. py:data:: __default_models_dictionary__
+   piel.models.physical.electronic.defaults.get_default_models
 
 
 
 .. py:function:: get_default_models(custom_defaults: dict | None = None) -> dict
 
    Returns the default models dictionary.
```

### Comparing `piel-0.0.43/docs/autoapi/piel/models/physical/geometry/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/physical/geometry/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/physical/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/physical/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/models/physical/units/index.rst` & `piel-0.0.44/docs/autoapi/piel/models/physical/units/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.44/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/project_structure/index.rst` & `piel-0.0.44/docs/autoapi/piel/project_structure/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/cocotb/core/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/cocotb/data/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/cocotb/data/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/cocotb/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/cocotb/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 -----------
 .. toctree::
    :titlesonly:
    :maxdepth: 3
 
    cocotb/index.rst
    gdsfactory/index.rst
+   hdl21/index.rst
    openlane/index.rst
-   pyspice/index.rst
+   qutip/index.rst
    sax/index.rst
+   thewalrus/index.rst
 
 
 Package Contents
 ----------------
 
 
 Functions
@@ -62,27 +64,34 @@
    piel.tools.get_all_timing_data_from_file
    piel.tools.read_sta_rpt_fwf_file
    piel.tools.contains_in_lines
    piel.tools.create_file_lines_dataframe
    piel.tools.get_file_line_by_keyword
    piel.tools.read_file_lines
    piel.tools.run_openlane_flow
+   piel.tools.convert_numeric_to_prefix
    piel.tools.get_sdense_ports_index
    piel.tools.sax_to_s_parameters_standard_matrix
+   piel.tools.fock_state_nonzero_indexes
+   piel.tools.fock_state_to_photon_number_factorial
+   piel.tools.verify_matrix_is_unitary
+   piel.tools.subunitary_selection_on_range
+   piel.tools.subunitary_selection_on_index
 
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
    piel.tools.delete_simulation_output_files
    piel.tools.get_simulation_output_files
    piel.tools.snet
+   piel.tools.standard_s_parameters_to_qutip_qobj
 
 
 .. py:function:: check_cocotb_testbench_exists(design_directory: str | pathlib.Path) -> bool
 
    Checks if a cocotb testbench exists in the design directory.
 
    :param design_directory: Design directory.
@@ -654,14 +663,19 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: piel_path_types
 
    :returns: None
 
 
+.. py:function:: convert_numeric_to_prefix(value: float)
+
+   This function converts a numeric value to a number under a SPICE unit closest to the base prefix. This allows us to connect a particular number real output, into a term that can be used in a SPICE netlist.
+
+
 .. py:function:: get_sdense_ports_index(input_ports_order: tuple, all_ports_index: dict) -> dict
 
    This function returns the ports index of the sax dense S-parameter matrix.
 
    Given that the order of the iteration is provided by the user, the dictionary keys will also be ordered
    accordingly when iterating over them. This requires the user to provide a set of ordered.
 
@@ -785,7 +799,75 @@
    :type input_ports_order: tuple
 
    :returns: The S-parameter matrix and the input ports index tuple in the standard S-parameter notation.
    :rtype: tuple
 
 
 .. py:data:: snet
+
+
+
+.. py:function:: fock_state_nonzero_indexes(fock_state: qutip.Qobj)
+
+   This function returns the indexes of the nonzero elements of a Fock state.
+
+   :param fock_state: A QuTip QObj representation of the Fock state.
+   :type fock_state: qutip.Qobj
+
+   :returns: The indexes of the nonzero elements of the Fock state.
+   :rtype: tuple
+
+
+.. py:function:: fock_state_to_photon_number_factorial(fock_state: qutip.Qobj)
+
+       This function converts a Fock state defined as:
+
+       .. math::
+
+   ewcommand{\ket}[1]{\left|{#1}
+   ight
+   angle}
+           \ket{f_1} = \ket{j_1, j_2, ... j_N}$
+
+       and returns:
+
+       .. math::
+
+           j_1^{'}! j_2^{'}! ... j_N^{'}!
+
+       Args:
+           fock_state (qutip.Qobj): A QuTip QObj representation of the Fock state.
+
+       Returns:
+           float: The photon number factorial of the Fock state.
+
+
+
+.. py:data:: standard_s_parameters_to_qutip_qobj
+
+
+
+.. py:function:: verify_matrix_is_unitary(matrix: jax.numpy.ndarray) -> bool
+
+   Verify that the matrix is unitary.
+
+   :param matrix: The matrix to verify.
+   :type matrix: jnp.ndarray
+
+   :returns: True if the matrix is unitary, False otherwise.
+   :rtype: bool
+
+
+.. py:function:: subunitary_selection_on_range(unitary_matrix: jax.numpy.ndarray, stop_index: tuple, start_index: Optional[tuple] = (0, 0))
+
+   This function returns a unitary between the indexes selected, and verifies the indexes are valid by checking that
+   the output matrix is also a unitary.
+
+   TODO implement validation of a 2D matrix.
+
+
+.. py:function:: subunitary_selection_on_index(unitary_matrix: jax.numpy.ndarray, rows_index: jax.numpy.ndarray | tuple, columns_index: jax.numpy.ndarray | tuple)
+
+   This function returns a unitary between the indexes selected, and verifies the indexes are valid by checking that
+   the output matrix is also a unitary.
+
+   TODO implement validation of a 2D matrix.
```

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/migrate/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/parse/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/v1/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/openlane/v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/pyspice/component/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/hdl21/circuit/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,22 @@
-:py:mod:`piel.tools.pyspice.component`
-======================================
+:py:mod:`piel.tools.hdl21.circuit`
+==================================
 
-.. py:module:: piel.tools.pyspice.component
+.. py:module:: piel.tools.hdl21.circuit
 
 .. autoapi-nested-parse::
 
    The way the construction of the SPICE models is implemented in ``piel`` is also microservice-esque. Larger
    circuits are constructed out of smaller building blocks. This means that simulation configurations and so on are
    constructed upon a provided initial circuit, and the SPICE directives are appended accordingly.
 
    As mentioned previously, ``piel`` creates circuits based on fundamental SPICE because this opens the possibility to
    large scale integration of these circuit models on different SPICE solvers, including proprietary ones as long as the
    SPICE circuit can be written to particular directories. However, due to the ease of circuit integration,
-   and translation that ``PySpice`` provides, it's API can also be used to implement parametrised functionality,
+   and translation that ``hdl21`` provides, it's API can also be used to implement parametrised functionality,
    although it is easy to export the circuit as a raw SPICE directive after composition.
 
-   This composition tends to be implemented in a `SubCircuit` hierarchical implementation, as this allows for more modularisation of the netlisted devices. Another aspect of complexity is that `PySpice` is class-based composed, so that means that functions define class definitions and return them, or instantiate default ones.
+   This composition tends to be implemented in a `SubCircuit` hierarchical implementation, as this allows for more modularisation of the netlisted devices.
 
    Let's assume that we can get an extracted SPICE netlist of our circuit, that includes all nodes, and component
    circuit definitions. This could then be simulated accordingly for the whole circuit between inputs and outputs. This
    would have to be constructed out of component models and a provided netlist in a similar fashion to ``SAX``.
-
-
-
-Module Contents
----------------
-
-
-Functions
-~~~~~~~~~
-
-.. autoapisummary::
-
-   piel.tools.pyspice.component.write_pyspice_circuit
-   piel.tools.pyspice.component.write_pyspice_circuit_from_raw_spice
-
-
-
-.. py:function:: write_pyspice_circuit(circuit_name: str = 'c')
-
-   This function returns a generic PySPICE circuit.
-   TODO Docs
-
-
-.. py:function:: write_pyspice_circuit_from_raw_spice(raw_spice: str, circuit_name: str = 'c')
-
-   This function returns a PySpice circuit composed from raw SPICE text.
-   TODO Docs
```

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/sax/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/sax/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/tools/sax/utils/index.rst` & `piel-0.0.44/docs/autoapi/piel/tools/sax/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/index.rst` & `piel-0.0.44/docs/autoapi/piel/visual/auto_plot_multiple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/visual/data_conversion/index.rst` & `piel-0.0.44/docs/autoapi/piel/visual/data_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/autoapi/piel/visual/index.rst` & `piel-0.0.44/docs/autoapi/piel/visual/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/conf.py` & `piel-0.0.44/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,20 @@
 ]
 html_logo = "_static/img/logo.png"
 html_show_sourcelink = (
     True  # Remove 'view source code' from top of page (for html, not python)
 )
 html_static_path = ["_static"]
 html_theme = "sphinx_book_theme"
-html_title = "s "
+html_title = "piel"
+html_theme_options = {
+    "repository_url": "https://github.com/daquintero/piel",
+    "use_repository_button": True,
+    "use_issues_button": True,
+}
 htmlhelp_basename = "pieldoc"
 man_pages = [(master_doc, "piel", "piel Documentation", [author], 1)]
 project = "piel"
 pygments_style = "sphinx"
 release = piel.__version__
 set_type_checking_flag = True  # Enable 'expensive' imports for sphinx_autodoc_typehints
 source_suffix = [".rst", ".md"]
```

### Comparing `piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/Makefile` & `piel-0.0.44/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/make.bat` & `piel-0.0.44/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/sections/environment/developer_docker_configuration.rst` & `piel-0.0.44/docs/sections/environment/developer_docker_configuration.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/sections/environment/setup.rst` & `piel-0.0.44/docs/sections/environment/setup.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         - *
         - Many
       * - ``openlane``
         -
         - *
         -
         -
-      * - ``pyspice``
+      * - ``hdl21``
         - ``ngspice`` & ``xyce``
         - ``ngspice`` & ``xyce``
         - ``ngspice`` & ``xyce``
         - ``ngspice``, ``xyce``
       * - ``sax``
         - *
         - *
```

### Comparing `piel-0.0.43/docs/sections/microservices/dependencies/cocotb.rst` & `piel-0.0.44/docs/sections/microservices/dependencies/cocotb.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/sections/microservices/dependencies/openlane.rst` & `piel-0.0.44/docs/sections/microservices/dependencies/openlane.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/sections/microservices/dependencies/pyspice.rst` & `piel-0.0.44/docs/sections/microservices/dependencies/spice.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,80 @@
-00000000: 6060 7370 6963 6560 6020 2620 6060 7079  ``spice`` & ``py
-00000010: 7370 6963 6560 600a 3d3d 3d3d 3d3d 3d3d  spice``.========
-00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00000030: 0a4d 6f73 7420 7068 6f74 6f6e 6963 2063  .Most photonic c
-00000040: 6f6d 706f 6e65 6e74 7320 6172 6520 636f  omponents are co
-00000050: 6d6d 6f6e 6c79 2064 7269 7665 6e20 6672  mmonly driven fr
-00000060: 6f6d 2061 6e61 6c6f 6775 6520 7369 676e  om analogue sign
-00000070: 616c 7320 7468 6174 2072 6570 7265 7365  als that represe
-00000080: 6e74 2065 6c65 6374 7269 6361 6c2d 6f70  nt electrical-op
-00000090: 7469 6361 6c20 7369 676e 616c 2063 6f6e  tical signal con
-000000a0: 7665 7273 696f 6e2e 2049 7420 6973 206e  version. It is n
-000000b0: 6563 6573 7361 7279 2074 6f20 7265 7072  ecessary to repr
-000000c0: 6573 656e 7420 7468 6573 6520 616e 616c  esent these anal
-000000d0: 6f67 7565 2073 6967 6e61 6c73 2062 6566  ogue signals bef
-000000e0: 6f72 6520 7468 6579 2063 616e 2062 6520  ore they can be 
-000000f0: 6469 6769 7469 7365 642e 2054 6865 2061  digitised. The a
-00000100: 6e61 6c6f 6775 6520 656c 6563 7472 6963  nalogue electric
-00000110: 616c 206c 6f61 6420 6566 6665 6374 7320  al load effects 
-00000120: 6e65 6564 2074 6f20 6265 2063 6f6e 7369  need to be consi
-00000130: 6465 7265 6420 6173 2077 656c 6c2c 206f  dered as well, o
-00000140: 7468 6572 7769 7365 2c20 6369 7263 7569  therwise, circui
-00000150: 7473 2069 6d70 6c65 6d65 6e74 6564 2069  ts implemented i
-00000160: 6e20 7468 6573 6520 746f 6f6c 7320 7769  n these tools wi
-00000170: 6c6c 2069 6e61 6363 7572 6174 656c 7920  ll inaccurately 
-00000180: 6d65 6173 7572 6520 7369 676e 616c 2074  measure signal t
-00000190: 7261 6e73 6665 7220 6265 7477 6565 6e20  ransfer between 
-000001a0: 646f 6d61 696e 732e 0a0a 416e 6f74 6865  domains...Anothe
-000001b0: 7220 6f62 6a65 6374 6976 6520 6f66 2069  r objective of i
-000001c0: 6d70 6c65 6d65 6e74 696e 6720 7468 6973  mplementing this
-000001d0: 2074 6f6f 6c20 6973 2074 6f20 656e 6162   tool is to enab
-000001e0: 6c65 2061 2063 6c65 6172 2064 7269 7665  le a clear drive
-000001f0: 722d 6c6f 6164 2d6d 6561 7375 7265 6d65  r-load-measureme
-00000200: 6e74 2072 656c 6174 696f 6e73 6869 7020  nt relationship 
-00000210: 6265 7477 6565 6e20 656c 6563 7472 6f6e  between electron
-00000220: 6963 2063 6972 6375 6974 7279 2061 6e64  ic circuitry and
-00000230: 2070 686f 746f 6e69 6320 7379 7374 656d   photonic system
-00000240: 732e 2057 6520 6361 6e20 696e 7465 6772  s. We can integr
-00000250: 6174 6520 6053 5049 4345 6020 736f 6c76  ate `SPICE` solv
-00000260: 6572 7320 7769 7468 206f 7468 6572 206f  ers with other o
-00000270: 7065 6e20 736f 7572 6365 2074 6f6f 6c73  pen source tools
-00000280: 2074 6f20 736f 6c76 6520 7068 6f74 6f6e   to solve photon
-00000290: 6963 2063 6f6d 7075 7461 7469 6f6e 616c  ic computational
-000002a0: 2066 756e 6374 696f 6e73 2061 6e64 206d   functions and m
-000002b0: 6f72 652e 0a0a 5061 7274 206f 6620 7468  ore...Part of th
-000002c0: 6520 6f62 6a65 6374 6976 6520 6f66 2060  e objective of `
-000002d0: 7069 656c 6020 6973 2074 6f20 6265 2061  piel` is to be a
-000002e0: 7320 696e 7465 6772 6162 6c65 2061 7320  s integrable as 
-000002f0: 706f 7373 6962 6c65 2c20 616e 6420 6173  possible, and as
-00000300: 206d 6f64 756c 6172 2061 7320 706f 7373   modular as poss
-00000310: 6962 6c65 2c20 6265 6361 7573 6520 7468  ible, because th
-00000320: 6520 6d61 696e 7461 696e 6572 7320 6265  e maintainers be
-00000330: 6c69 6576 6520 7468 6973 2065 6e73 7572  lieve this ensur
-00000340: 6573 206c 6f6e 6765 722d 7465 726d 2075  es longer-term u
-00000350: 7365 6675 6c6e 6573 7320 7468 616e 206d  sefulness than m
-00000360: 6f6e 6f6c 6974 6873 2e0a 0a49 6e74 6567  onoliths...Integ
-00000370: 7261 7469 6f6e 2053 6368 656d 650a 2d2d  ration Scheme.--
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000390: 0a0a 496e 2060 7069 656c 602c 2074 6865  ..In `piel`, the
-000003a0: 2060 5350 4943 4560 2d67 656e 6572 6174   `SPICE`-generat
-000003b0: 6564 2063 6972 6375 6974 7320 7769 6c6c  ed circuits will
-000003c0: 2061 6c77 6179 7320 6265 2072 6177 2060   always be raw `
-000003d0: 5350 4943 4560 2072 6174 6865 7220 7468  SPICE` rather th
-000003e0: 616e 2075 7369 6e67 2061 2070 6163 6b61  an using a packa
-000003f0: 6765 2074 6f20 6372 6561 7465 2061 2063  ge to create a c
-00000400: 6972 6375 6974 206d 6f64 656c 206f 7220  ircuit model or 
-00000410: 7265 6c61 7465 642e 2054 6869 7320 6973  related. This is
-00000420: 2062 6563 6175 7365 2061 6e79 2073 6572   because any ser
-00000430: 696f 7573 2060 5350 4943 4560 2070 726f  ious `SPICE` pro
-00000440: 6772 616d 2077 696c 6c20 616c 7761 7973  gram will always
-00000450: 2061 6363 6570 7420 7261 7720 696e 7075   accept raw inpu
-00000460: 7473 2074 6861 7420 6361 6e20 6265 2069  ts that can be i
-00000470: 6e74 6567 7261 7465 6420 696e 746f 2069  ntegrated into i
-00000480: 7473 2073 6f6c 7665 7273 2e20 5468 6973  ts solvers. This
-00000490: 2077 696c 6c20 616c 6c6f 7720 7573 2069   will allow us i
-000004a0: 6e20 7468 6520 6675 7475 7265 2074 6f20  n the future to 
-000004b0: 696e 7465 6772 6174 6520 7769 7468 2060  integrate with `
-000004c0: 5350 4543 5452 4560 2061 6e64 206f 7468  SPECTRE` and oth
-000004d0: 6572 2072 656c 6174 6564 2070 726f 6772  er related progr
-000004e0: 616d 732e 0a0a 2e2e 2074 6f63 7472 6565  ams..... toctree
-000004f0: 3a3a 0a0a 2020 2020 7265 6c65 7661 6e74  ::..    relevant
-00000500: 5f73 7069 6365 5f70 726f 6a65 6374 730a  _spice_projects.
+00000000: 6060 5350 4943 4560 600a 3d3d 3d3d 3d3d  ``SPICE``.======
+00000010: 3d3d 3d0a 0a4d 6f73 7420 7068 6f74 6f6e  ===..Most photon
+00000020: 6963 2063 6f6d 706f 6e65 6e74 7320 6172  ic components ar
+00000030: 6520 636f 6d6d 6f6e 6c79 2064 7269 7665  e commonly drive
+00000040: 6e20 6672 6f6d 2061 6e61 6c6f 6775 6520  n from analogue 
+00000050: 7369 676e 616c 7320 7468 6174 2072 6570  signals that rep
+00000060: 7265 7365 6e74 2065 6c65 6374 7269 6361  resent electrica
+00000070: 6c2d 6f70 7469 6361 6c20 7369 676e 616c  l-optical signal
+00000080: 2063 6f6e 7665 7273 696f 6e2e 2049 7420   conversion. It 
+00000090: 6973 206e 6563 6573 7361 7279 2074 6f20  is necessary to 
+000000a0: 7265 7072 6573 656e 7420 7468 6573 6520  represent these 
+000000b0: 616e 616c 6f67 7565 2073 6967 6e61 6c73  analogue signals
+000000c0: 2062 6566 6f72 6520 7468 6579 2063 616e   before they can
+000000d0: 2062 6520 6469 6769 7469 7365 642e 2054   be digitised. T
+000000e0: 6865 2061 6e61 6c6f 6775 6520 656c 6563  he analogue elec
+000000f0: 7472 6963 616c 206c 6f61 6420 6566 6665  trical load effe
+00000100: 6374 7320 6e65 6564 2074 6f20 6265 2063  cts need to be c
+00000110: 6f6e 7369 6465 7265 6420 6173 2077 656c  onsidered as wel
+00000120: 6c2c 206f 7468 6572 7769 7365 2c20 6369  l, otherwise, ci
+00000130: 7263 7569 7473 2069 6d70 6c65 6d65 6e74  rcuits implement
+00000140: 6564 2069 6e20 7468 6573 6520 746f 6f6c  ed in these tool
+00000150: 7320 7769 6c6c 2069 6e61 6363 7572 6174  s will inaccurat
+00000160: 656c 7920 6d65 6173 7572 6520 7369 676e  ely measure sign
+00000170: 616c 2074 7261 6e73 6665 7220 6265 7477  al transfer betw
+00000180: 6565 6e20 646f 6d61 696e 732e 0a0a 416e  een domains...An
+00000190: 6f74 6865 7220 6f62 6a65 6374 6976 6520  other objective 
+000001a0: 6f66 2069 6d70 6c65 6d65 6e74 696e 6720  of implementing 
+000001b0: 7468 6973 2074 6f6f 6c20 6973 2074 6f20  this tool is to 
+000001c0: 656e 6162 6c65 2061 2063 6c65 6172 2064  enable a clear d
+000001d0: 7269 7665 722d 6c6f 6164 2d6d 6561 7375  river-load-measu
+000001e0: 7265 6d65 6e74 2072 656c 6174 696f 6e73  rement relations
+000001f0: 6869 7020 6265 7477 6565 6e20 656c 6563  hip between elec
+00000200: 7472 6f6e 6963 2063 6972 6375 6974 7279  tronic circuitry
+00000210: 2061 6e64 2070 686f 746f 6e69 6320 7379   and photonic sy
+00000220: 7374 656d 732e 2057 6520 6361 6e20 696e  stems. We can in
+00000230: 7465 6772 6174 6520 6053 5049 4345 6020  tegrate `SPICE` 
+00000240: 736f 6c76 6572 7320 7769 7468 206f 7468  solvers with oth
+00000250: 6572 206f 7065 6e20 736f 7572 6365 2074  er open source t
+00000260: 6f6f 6c73 2074 6f20 736f 6c76 6520 7068  ools to solve ph
+00000270: 6f74 6f6e 6963 2063 6f6d 7075 7461 7469  otonic computati
+00000280: 6f6e 616c 2066 756e 6374 696f 6e73 2061  onal functions a
+00000290: 6e64 206d 6f72 652e 0a0a 5061 7274 206f  nd more...Part o
+000002a0: 6620 7468 6520 6f62 6a65 6374 6976 6520  f the objective 
+000002b0: 6f66 2060 7069 656c 6020 6973 2074 6f20  of `piel` is to 
+000002c0: 6265 2061 7320 696e 7465 6772 6162 6c65  be as integrable
+000002d0: 2061 7320 706f 7373 6962 6c65 2c20 616e   as possible, an
+000002e0: 6420 6173 206d 6f64 756c 6172 2061 7320  d as modular as 
+000002f0: 706f 7373 6962 6c65 2c20 6265 6361 7573  possible, becaus
+00000300: 6520 7468 6520 6d61 696e 7461 696e 6572  e the maintainer
+00000310: 7320 6265 6c69 6576 6520 7468 6973 2065  s believe this e
+00000320: 6e73 7572 6573 206c 6f6e 6765 722d 7465  nsures longer-te
+00000330: 726d 2075 7365 6675 6c6e 6573 7320 7468  rm usefulness th
+00000340: 616e 206d 6f6e 6f6c 6974 6873 2e0a 0a49  an monoliths...I
+00000350: 6e74 6567 7261 7469 6f6e 2053 6368 656d  ntegration Schem
+00000360: 650a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e.--------------
+00000370: 2d2d 2d2d 0a0a 496e 2060 7069 656c 602c  ----..In `piel`,
+00000380: 2074 6865 2060 5350 4943 4560 2d67 656e   the `SPICE`-gen
+00000390: 6572 6174 6564 2063 6972 6375 6974 7320  erated circuits 
+000003a0: 7769 6c6c 2061 6c77 6179 7320 6265 2072  will always be r
+000003b0: 6177 2060 5350 4943 4560 2072 6174 6865  aw `SPICE` rathe
+000003c0: 7220 7468 616e 2075 7369 6e67 2061 2070  r than using a p
+000003d0: 6163 6b61 6765 2074 6f20 6372 6561 7465  ackage to create
+000003e0: 2061 2063 6972 6375 6974 206d 6f64 656c   a circuit model
+000003f0: 206f 7220 7265 6c61 7465 642e 2054 6869   or related. Thi
+00000400: 7320 6973 2062 6563 6175 7365 2061 6e79  s is because any
+00000410: 2073 6572 696f 7573 2060 5350 4943 4560   serious `SPICE`
+00000420: 2070 726f 6772 616d 2077 696c 6c20 616c   program will al
+00000430: 7761 7973 2061 6363 6570 7420 7261 7720  ways accept raw 
+00000440: 696e 7075 7473 2074 6861 7420 6361 6e20  inputs that can 
+00000450: 6265 2069 6e74 6567 7261 7465 6420 696e  be integrated in
+00000460: 746f 2069 7473 2073 6f6c 7665 7273 2e20  to its solvers. 
+00000470: 5468 6973 2077 696c 6c20 616c 6c6f 7720  This will allow 
+00000480: 7573 2069 6e20 7468 6520 6675 7475 7265  us in the future
+00000490: 2074 6f20 696e 7465 6772 6174 6520 7769   to integrate wi
+000004a0: 7468 2060 5350 4543 5452 4560 2061 6e64  th `SPECTRE` and
+000004b0: 206f 7468 6572 2072 656c 6174 6564 2070   other related p
+000004c0: 726f 6772 616d 732e 0a0a 2e2e 2074 6f63  rograms..... toc
+000004d0: 7472 6565 3a3a 0a20 2020 2072 656c 6576  tree::.    relev
+000004e0: 616e 745f 7370 6963 655f 7072 6f6a 6563  ant_spice_projec
+000004f0: 7473 0a                                  ts.
```

### Comparing `piel-0.0.43/docs/sections/microservices/dependencies/sax.rst` & `piel-0.0.44/docs/sections/microservices/dependencies/sax.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/docs/sections/microservices/integration/sax_qutip.rst` & `piel-0.0.44/docs/sections/microservices/integration/sax_qutip.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/__init__.py` & `piel-0.0.44/piel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 os.environ["PIEL_PACKAGE_DIRECTORY"] = str(
     pathlib.Path(__file__).parent.parent.resolve()
 )
 
 __author__ = """Dario Quintero"""
 __email__ = "darioaquintero@gmail.com"
-__version__ = "0.0.43"
+__version__ = "0.0.44"
```

### Comparing `piel-0.0.43/piel/defaults.py` & `piel-0.0.44/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/file_conversion.py` & `piel-0.0.44/piel/file_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-from pyDigitalWaveTools.vcd.parser import VcdParser
 from .file_system import return_path
 from .config import piel_path_types
 
 __all__ = [
     "read_csv_to_pandas",
     "read_vcd_to_json",
 ]
@@ -15,13 +14,15 @@
     """
     file_path = return_path(file_path)
     simulation_data = pd.read_csv(file_path)
     return simulation_data
 
 
 def read_vcd_to_json(file_path: piel_path_types):
+    from pyDigitalWaveTools.vcd.parser import VcdParser
+
     file_path = return_path(file_path)
     with open(str(file_path.resolve())) as vcd_file:
         vcd = VcdParser()
         vcd.parse(vcd_file)
         json_data = vcd.scope.toJson()
     return json_data
```

### Comparing `piel-0.0.43/piel/file_system.py` & `piel-0.0.44/piel/file_system.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/integration/gdsfactory_openlane.py` & `piel-0.0.44/piel/integration/gdsfactory_openlane.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/integration/gdsfactory_pyspice/utils.py` & `piel-0.0.44/piel/integration/gdsfactory_hdl21/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__all__ = ["rename_gdsfactory_connections_to_spice", "convert_tuples_to_strings"]
+
+
 def rename_gdsfactory_connections_to_spice(connections: dict):
     """
     We convert the connection connectivity of the gdsfactory netlist into names that can be integrated into a SPICE
     netlist. It iterates on each key value pair, and replaces each comma with an underscore.
 
     # TODO docs
     """
```

### Comparing `piel-0.0.43/piel/integration/sax_qutip.py` & `piel-0.0.44/piel/integration/sax_qutip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,16 @@
 import qutip  # NOQA : F401
 import sax
-from ..config import nso
+import numpy as np
+from ..tools.qutip.unitary import matrix_to_qutip_qobj
 from piel.tools.sax.utils import sax_to_s_parameters_standard_matrix
 
-__all__ = ["sax_to_ideal_qutip_unitary", "standard_s_parameters_to_ideal_qutip_unitary"]
-
-
-def standard_s_parameters_to_ideal_qutip_unitary(
-    s_parameters_standard_matrix: nso.ndarray,
-):
-    """
-    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-    dimensions of the matrix can be observed.
-
-    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
-    already in described in piel/piel/sax/utils.py.
-
-    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
-
-    For example, a ``qutip`` representation of an s-gate gate would be:
-
-    ..code-block:: python
-
-        import numpy as np
-        import qutip
-
-        # S-Gate
-        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
-        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
-
-    In mathematical notation, this S-gate would be written as:
-
-    ..math::
-
-        S = \\begin{bmatrix}
-            1 & 0 \\
-            0 & i \\
-        \\end{bmatrix}
-
-    Args:
-        s_parameters_standard_matrix (nso.ndarray): A dictionary of S-parameters in the form of a SDict from `sax`.
-
-    Returns:
-        qobj_unitary (qutip.Qobj): A QuTip QObj representation of the S-parameters in a unitary matrix.
-
-    """
-    # TODO make a function any SAX input.
-    qobj_unitary = qutip.Qobj(s_parameters_standard_matrix)
-    return qobj_unitary
+__all__ = [
+    "sax_to_ideal_qutip_unitary",
+]
 
 
 def sax_to_ideal_qutip_unitary(sax_input: sax.SType):
     """
     This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
     dimensions of the matrix can be observed.
 
@@ -61,39 +19,38 @@
     already in described in piel/piel/sax/utils.py.
 
     From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly.
     https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
     For example, a ``qutip`` representation of an s-gate gate would be:
 
-    ..code-block:: python
+    ..code-block::
 
         import numpy as np
         import qutip
         # S-Gate
         s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
         s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
     In mathematical notation, this S-gate would be written as:
 
     ..math::
 
         S = \\begin{bmatrix}
-            1 & 0 \\
-            0 & i \\
+            1 & 0 \\\\
+            0 & i \\\\
         \\end{bmatrix}
 
     Args:
         sax_input (sax.SType): A dictionary of S-parameters in the form of a SDict from `sax`.
 
     Returns:
         qobj_unitary (qutip.Qobj): A QuTip QObj representation of the S-parameters in a unitary matrix.
     """
     # TODO make a function any SAX input.
     (
         s_parameters_standard_matrix,
         input_ports_index_tuple_order,
     ) = sax_to_s_parameters_standard_matrix(sax_input)
-    qobj_unitary = standard_s_parameters_to_ideal_qutip_unitary(
-        s_parameters_standard_matrix
-    )
+    s_parameter_standard_matrix_numpy = np.asarray(s_parameters_standard_matrix)
+    qobj_unitary = matrix_to_qutip_qobj(s_parameter_standard_matrix_numpy)
     return qobj_unitary
```

### Comparing `piel-0.0.43/piel/integration/sax_thewalrus.py` & `piel-0.0.44/piel/integration/sax_thewalrus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,13 @@
-import numpy as np
 import sax
-import time
-import thewalrus
 from ..tools.sax import sax_to_s_parameters_standard_matrix
+from ..tools.thewalrus import unitary_permanent
 
 
-def unitary_permanent(
-    unitary_matrix: np.ndarray,
-) -> tuple:
-    """
-    The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
-
-    ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
-
-    # TODO maybe implement subroutine if computation is taking forever.
-    # TODO why two outputs? Understand this properly later.
-
-    Args:
-        unitary_permanent (np.ndarray): The unitary matrix.
-
-    Returns:
-        tuple: The circuit permanent and the time it took to compute it.
-
-    """
-    start_time = time.time()
-    circuit_permanent = thewalrus.perm(unitary_matrix)
-    end_time = time.time()
-    computed_time = end_time - start_time
-    return circuit_permanent, computed_time
+__all__ = ["sax_circuit_permanent", "unitary_permanent"]
 
 
 def sax_circuit_permanent(
     sax_input: sax.SType,
 ) -> tuple:
     """
     The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
```

### Comparing `piel-0.0.43/piel/models/frequency/all.py` & `piel-0.0.44/piel/models/frequency/all.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/models/frequency/defaults.py` & `piel-0.0.44/piel/models/frequency/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/models/frequency/photonic/directional_coupler_length.py` & `piel-0.0.44/piel/models/frequency/photonic/directional_coupler_length.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
+import jax.numpy as jnp
 import sax
-from ....config import nso
 
 __all__ = ["directional_coupler_with_length"]
 
 
 def directional_coupler_with_length(
     length=1e-5, coupling=0.5, loss=0, neff=2.34, wl0=1.55e-6, ng=3.40, phase=0
 ):
     kappa = coupling**0.5
     tau = (1 - coupling) ** 0.5
     loss = 10 ** (-loss * length / 20)  # factor 20 bc amplitudes, not intensities.
-    cos_phase = nso.cos(phase)
-    sin_phase = nso.sin(phase)
+    cos_phase = jnp.cos(phase)
+    sin_phase = jnp.sin(phase)
     sdict = sax.reciprocal(
         {
             ("port0", "port1"): tau * loss * cos_phase,
             ("port0", "port2"): -kappa * loss * sin_phase,
             ("port1", "port3"): -kappa * loss * sin_phase,
             ("port2", "port3"): tau * loss * cos_phase,
         }
```

### Comparing `piel-0.0.43/piel/models/frequency/photonic/directional_coupler_real.py` & `piel-0.0.44/piel/models/frequency/photonic/directional_coupler_real.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/models/frequency/photonic/grating_coupler.py` & `piel-0.0.44/piel/models/frequency/photonic/grating_coupler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
-from ....config import nso
+import jax.numpy as jnp
 
 __all__ = ["grating_coupler_simple"]
 
 
 def grating_coupler_simple(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=0.06e-6, wl0=1.55e-6):
     # Constants
-    fwhm2sigma = 1.0 / (2 * nso.sqrt(2 * nso.log(2)))
+    fwhm2sigma = 1.0 / (2 * jnp.sqrt(2 * jnp.log(2)))
 
     # Compute sigma
     sigma = fwhm2sigma * bandwidth
 
     # Assume the wavelength of the environment matches the center wavelength of the grating coupler
     wls = wl0
 
     # Compute loss
-    loss = nso.sqrt(Tmax * nso.exp(-((wl0 - wls) ** 2) / (2 * sigma**2)))
+    loss = jnp.sqrt(Tmax * jnp.exp(-((wl0 - wls) ** 2) / (2 * sigma**2)))
 
     # Create scattering dictionary
     sdict = {
         ("in0", "out1"): loss,
         ("in1", "out0"): loss,
         ("in0", "out0"): R_in,
         ("in1", "out1"): R,
```

### Comparing `piel-0.0.43/piel/models/frequency/photonic/straight_waveguide.py` & `piel-0.0.44/piel/models/frequency/photonic/straight_waveguide.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
 import sax
-from ....config import nso
+import jax.numpy as jnp
 
 __all__ = ["ideal_active_waveguide", "waveguide", "simple_straight"]
 
 
 def waveguide(wl=1.55, wl0=1.55, neff=2.34, ng=3.4, length=10.0, loss=0.0):
     dwl = wl - wl0
     dneff_dwl = (ng - neff) / wl0
     neff = neff - dwl * dneff_dwl
-    phase = 2 * nso.pi * neff * length / wl
-    amplitude = nso.asarray(10 ** (-loss * length / 20), dtype=complex)
-    transmission = amplitude * nso.exp(1j * phase)
+    phase = 2 * jnp.pi * neff * length / wl
+    amplitude = jnp.asarray(10 ** (-loss * length / 20), dtype=complex)
+    transmission = amplitude * jnp.exp(1j * phase)
     sdict = sax.reciprocal({("o1", "o2"): transmission})
     return sdict
 
 
 def ideal_active_waveguide(
     wl=1.55, wl0=1.55, neff=2.34, ng=3.4, length=10.0, loss=0.0, active_phase_rad=0.0
 ):
     dwl = wl - wl0
     dneff_dwl = (ng - neff) / wl0
     neff = neff - dwl * dneff_dwl
-    phase = (2 * nso.pi * neff * length / wl) + active_phase_rad
-    amplitude = nso.asarray(10 ** (-loss * length / 20), dtype=complex)
-    transmission = amplitude * nso.exp(1j * phase)
+    phase = (2 * jnp.pi * neff * length / wl) + active_phase_rad
+    amplitude = jnp.asarray(10 ** (-loss * length / 20), dtype=complex)
+    transmission = amplitude * jnp.exp(1j * phase)
     sdict = sax.reciprocal({("o1", "o2"): transmission})
     return sdict
 
 
 def simple_straight(length=10.0, width=0.5):
     S = {("o1", "o2"): 1.0}  # we'll improve this model later!
     return sax.reciprocal(S)
```

### Comparing `piel-0.0.43/piel/models/logic/electro_optic/signal_mapping.py` & `piel-0.0.44/piel/models/logic/electro_optic/signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/models/physical/electronic/spice/capacitor.py` & `piel-0.0.44/piel/models/physical/electronic/capacitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-"""The way each of these models should work is that they use the settings from the `gdsfactory` component,
+"""
+# TODO move and update.
+The way each of these models should work is that they use the settings from the `gdsfactory` component,
 to create a parametric SPICE directive.
 
 These functions map a particular model, with an instance representation that corresponds to the given netlist
-connectivity, and returns a PySpice representation of the circuit. This function will be called after parsing the
+connectivity, and returns a SPICE representation of the circuit. This function will be called after parsing the
 circuit netlist accordingly, and creating a mapping from the instance definitions to the fundamental components.
 """
 
 
 def add_basic_capacitor(settings) -> str:
     """
     This function takes in the settings from a gdsfactory component, some connectivity node translated directly from
```

### Comparing `piel-0.0.43/piel/parametric.py` & `piel-0.0.44/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/project_structure.py` & `piel-0.0.44/piel/project_structure.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/cocotb/core.py` & `piel-0.0.44/piel/tools/cocotb/core.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/cocotb/data.py` & `piel-0.0.44/piel/tools/cocotb/data.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/gdsfactory/netlist.py` & `piel-0.0.44/piel/tools/gdsfactory/netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/migrate.py` & `piel-0.0.44/piel/tools/openlane/migrate.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/parse/run_output.py` & `piel-0.0.44/piel/tools/openlane/parse/run_output.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/parse/sta_rpt.py` & `piel-0.0.44/piel/tools/openlane/parse/sta_rpt.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/parse/utils.py` & `piel-0.0.44/piel/tools/openlane/parse/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/utils.py` & `piel-0.0.44/piel/tools/openlane/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/v1.py` & `piel-0.0.44/piel/tools/openlane/v1.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/openlane/v2.py` & `piel-0.0.44/piel/tools/openlane/v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/tools/pyspice/component.py` & `piel-0.0.44/piel/tools/hdl21/circuit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 """The way the construction of the SPICE models is implemented in ``piel`` is also microservice-esque. Larger
 circuits are constructed out of smaller building blocks. This means that simulation configurations and so on are
 constructed upon a provided initial circuit, and the SPICE directives are appended accordingly.
 
 As mentioned previously, ``piel`` creates circuits based on fundamental SPICE because this opens the possibility to
 large scale integration of these circuit models on different SPICE solvers, including proprietary ones as long as the
 SPICE circuit can be written to particular directories. However, due to the ease of circuit integration,
-and translation that ``PySpice`` provides, it's API can also be used to implement parametrised functionality,
+and translation that ``hdl21`` provides, it's API can also be used to implement parametrised functionality,
 although it is easy to export the circuit as a raw SPICE directive after composition.
 
-This composition tends to be implemented in a `SubCircuit` hierarchical implementation, as this allows for more modularisation of the netlisted devices. Another aspect of complexity is that `PySpice` is class-based composed, so that means that functions define class definitions and return them, or instantiate default ones.
+This composition tends to be implemented in a `SubCircuit` hierarchical implementation, as this allows for more modularisation of the netlisted devices.
 
 Let's assume that we can get an extracted SPICE netlist of our circuit, that includes all nodes, and component
 circuit definitions. This could then be simulated accordingly for the whole circuit between inputs and outputs. This
 would have to be constructed out of component models and a provided netlist in a similar fashion to ``SAX``. """
-from PySpice.Spice.Netlist import Circuit
+# Another aspect of complexity is that `hdl21` is class-based composed, so that means that functions define class definitions and return them, or instantiate default ones.
 
-
-def write_pyspice_circuit(circuit_name: str = "c"):
-    """
-    This function returns a generic PySPICE circuit.
-    TODO Docs
-    """
-    circuit = Circuit(circuit_name)
-    return circuit
-
-
-def write_pyspice_circuit_from_raw_spice(raw_spice: str, circuit_name: str = "c"):
-    """
-    This function returns a PySpice circuit composed from raw SPICE text.
-    TODO Docs
-    """
-    circuit = Circuit(circuit_name)
-    circuit.raw_spice = raw_spice
-    return circuit
+# __all__ = ["create_pyspice_circuit", "write_raw_spice_to_pyspice_circuit"]
+#
+#
+# def create_pyspice_circuit(circuit_name: str = "c") -> Circuit:
+#     """
+#     This function returns a generic PySPICE circuit. This is useful for adding SPICE directives to a circuit.
+#
+#     Args:
+#         circuit_name (str): Name of the circuit
+#
+#     Returns:
+#         Circuit: PySpice circuit
+#     """
+#     circuit = Circuit(circuit_name)
+#     return circuit
+#
+#
+# def write_raw_spice_to_pyspice_circuit(circuit: Circuit, raw_spice: str) -> Circuit:
+#     """
+#     This function returns a PySpice circuit including the raw SPICE text. This is useful for adding SPICE directives
+#     to a circuit.
+#
+#     Args:
+#         circuit (Circuit): PySpice circuit
+#         raw_spice (str): Raw SPICE text
+#
+#     Returns:
+#         Circuit: PySpice circuit including the raw SPICE text
+#     """
+#     circuit.raw_spice += raw_spice
+#     return circuit
```

### Comparing `piel-0.0.43/piel/tools/sax/utils.py` & `piel-0.0.44/piel/tools/sax/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This file provides a set of utilities that allow much easier integration between `sax` and the relevant tools that we use.
 """
-import numpy as np
+import jax.numpy as jnp
 import sax
 from ..gdsfactory.netlist import get_matched_ports_tuple_index
 from typing import Optional  # NOQA : F401
 
 __all__ = ["get_sdense_ports_index", "sax_to_s_parameters_standard_matrix", "snet"]
 
 
@@ -176,23 +176,22 @@
         (
             output_ports_index_tuple_order,
             output_matched_ports_name_tuple_order,
         ) = get_matched_ports_tuple_index(
             ports_index=dense_s_parameter_index, prefix="out"
         )
 
+    output_ports_index_tuple_order_jax = jnp.asarray(output_ports_index_tuple_order)
+    input_ports_index_tuple_order_jax = jnp.asarray(input_ports_index_tuple_order)
     # We now select the SDense columns that we care about.
-    dense_s_parameter_matrix = np.asarray(
-        dense_s_parameter_matrix
-    )  # TODO port to JAX multiindexing
-    s_parameters_standard_matrix = dense_s_parameter_matrix[
-        [output_ports_index_tuple_order]
-    ][0]
+    s_parameters_standard_matrix = dense_s_parameter_matrix.at[
+        output_ports_index_tuple_order_jax
+    ].get()
+    s_parameters_standard_matrix = s_parameters_standard_matrix.at[
+        :, input_ports_index_tuple_order_jax
+    ].get()
     # Now we select the SDense rows that we care about after transposing the matrix.
-    s_parameters_standard_matrix = s_parameters_standard_matrix[
-        :, [input_ports_index_tuple_order][0]
-    ]
-    # TODO verify matrix transpose for unitary match.
+    # TODO verify matrix transpose for unitary match. I think it is right.
     return s_parameters_standard_matrix.T, input_matched_ports_name_tuple_order
 
 
 snet = sax_to_s_parameters_standard_matrix
```

### Comparing `piel-0.0.43/piel/visual/auto_plot_multiple.py` & `piel-0.0.44/piel/visual/auto_plot_multiple.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel/visual/data_conversion.py` & `piel-0.0.44/piel/visual/data_conversion.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/piel.egg-info/PKG-INFO` & `piel-0.0.44/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.43
+Version: 0.0.44
 Summary: Photonic Integrated Electronics: microservices to codesign photonics, electronics, communications, quantum, and more.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,70 +16,79 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-**P**\hotonic **I**\ntegrated **EL**\ectronics
-===============================================
+# **P**hotonic **I**ntegrated **EL**ectronics
 
-|PyPI Version| |Build Status| |Documentation Status| |Updates|
+[![PyPI
+Name](https://img.shields.io/badge/pypi-piel-blue)](https://pypi.python.org/pypi/piel)
+[![PyPI
+Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
+[![Build
+Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
+[![Documentation
+Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
+[![MIT](https://img.shields.io/github/license/gdsfactory/gdsfactory)](https://choosealicense.com/licenses/mit/)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Microservices to codesign photonics, electronics, communications,
 quantum, and more.
 
--  Free software: MIT license
--  Documentation: https://piel.readthedocs.io
+-   Free software: MIT license
+-   Documentation: <https://piel.readthedocs.io>
 
-Target functionality
---------------------
+## Target functionality
 
--  Co-simulation and optimisation between integrated photonic and
-   electronic chip design.
--  System interconnection modelling in multiple domains.
--  Chip and interposer design integration.
--  Component models translation library between simulation tools.
--  Quantum models of physical circuitry.
+-   Co-simulation and optimisation between integrated photonic and
+    electronic chip design.
+-   System interconnection modelling in multiple domains.
+-   Chip and interposer design integration.
+-   Component models translation library between simulation tools.
+-   Quantum models of physical circuitry.
 
-``piel`` aims to provide an integrated workflow to co-design photonics
-and electronics, classically and quantum. It does not aim to replace the
+`piel` aims to provide an integrated workflow to co-design photonics and
+electronics, classically and quantum. It does not aim to replace the
 individual functionality of each design tool, but rather provide a glue
 to easily connect them all together and extract the system performance.
 
-Examples
---------
+## Examples
 
-Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+Follow the many [examples in the
+documentation](https://piel.readthedocs.io/en/latest/examples.html).
 
-Microservices Toolset
----------------------
+## Microservices Toolset
 
 This package provides interconnection functions to easily co-design
 microelectronics through the functionality of the
-`IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
-photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
+[IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and
+photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+
+![image](docs/_static/img/piel_microservice_structure.png)
 
 Some existing microservice dependency integrations are:
 
-* `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
-* `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
-* `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
-* `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
-* `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
-* `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
+-   [cocotb](https://github.com/cocotb/cocotb) - a coroutine based
+    cosimulation library for writing VHDL and Verilog testbenches in
+    Python.
+-   [hdl21](https://github.com/dan-fritchman/Hdl21) - Analog Hardware
+    Description Library in Python
+-   [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open
+    source platform for end to-end photonic chip design and validation
+-   [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an
+    automated RTL to GDSII flow based on several components including
+    OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for
+    design exploration and optimization
+-   [sax](https://github.com/flaport/sax) - S-parameter based frequency
+    domain circuit simulations and optimizations using JAX.
+-   [thewalrus](https://github.com/XanaduAI/thewalrus) -A library for
+    the calculation of hafnians, Hermite polynomials and Gaussian boson
+    sampling.
+-   [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in
+    Python
 
-Contribution
-------------
+## Contribution
 
 If you feel dedicated enough to become a project maintainer, or just
-want to do a single contribution, let's do this together!
-
-.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
-   :target: https://pypi.python.org/pypi/piel
-.. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
-   :target: https://travis-ci.com/daquintero/piel
-.. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
-   :target: https://piel.readthedocs.io/en/latest/?version=latest
-.. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
-   :target: https://pyup.io/repos/github/daquintero/piel/
+want to do a single contribution, let\'s do this together!
```

### Comparing `piel-0.0.43/piel.egg-info/SOURCES.txt` & `piel-0.0.44/piel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.cfg
 setup.py
 docs/Makefile
+docs/README.rst
 docs/conf.py
 docs/contributing.rst
 docs/examples.rst
 docs/index.rst
 docs/make.bat
 docs/_static/img/logo.png
+docs/_static/img/piel_microservice_structure.png
 docs/autoapi/index.rst
 docs/autoapi/piel/index.rst
 docs/autoapi/piel/cli/index.rst
 docs/autoapi/piel/components/index.rst
 docs/autoapi/piel/config/index.rst
 docs/autoapi/piel/defaults/index.rst
 docs/autoapi/piel/file_conversion/index.rst
 docs/autoapi/piel/file_system/index.rst
 docs/autoapi/piel/integration/index.rst
 docs/autoapi/piel/integration/cocotb_sax/index.rst
+docs/autoapi/piel/integration/gdsfactory_hdl21/index.rst
+docs/autoapi/piel/integration/gdsfactory_hdl21/conversion/index.rst
+docs/autoapi/piel/integration/gdsfactory_hdl21/core/index.rst
+docs/autoapi/piel/integration/gdsfactory_hdl21/utils/index.rst
 docs/autoapi/piel/integration/gdsfactory_openlane/index.rst
-docs/autoapi/piel/integration/gdsfactory_pyspice/index.rst
-docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/index.rst
-docs/autoapi/piel/integration/gdsfactory_pyspice/core/index.rst
-docs/autoapi/piel/integration/gdsfactory_pyspice/utils/index.rst
-docs/autoapi/piel/integration/pyspice_sax/index.rst
 docs/autoapi/piel/integration/sax_qutip/index.rst
 docs/autoapi/piel/integration/sax_thewalrus/index.rst
+docs/autoapi/piel/integration/thewalrus_qutip/index.rst
 docs/autoapi/piel/models/index.rst
 docs/autoapi/piel/models/frequency/index.rst
 docs/autoapi/piel/models/frequency/all/index.rst
 docs/autoapi/piel/models/frequency/defaults/index.rst
 docs/autoapi/piel/models/frequency/electrical/index.rst
 docs/autoapi/piel/models/frequency/electro_optic/index.rst
 docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
@@ -57,18 +59,20 @@
 docs/autoapi/piel/models/logic/photonic/index.rst
 docs/autoapi/piel/models/physical/index.rst
 docs/autoapi/piel/models/physical/electrical/index.rst
 docs/autoapi/piel/models/physical/electrical/cable/index.rst
 docs/autoapi/piel/models/physical/electro_optic/index.rst
 docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
 docs/autoapi/piel/models/physical/electronic/index.rst
-docs/autoapi/piel/models/physical/electronic/spice/index.rst
-docs/autoapi/piel/models/physical/electronic/spice/capacitor/index.rst
-docs/autoapi/piel/models/physical/electronic/spice/defaults/index.rst
-docs/autoapi/piel/models/physical/electronic/spice/resistor/index.rst
+docs/autoapi/piel/models/physical/electronic/capacitor/index.rst
+docs/autoapi/piel/models/physical/electronic/defaults/index.rst
+docs/autoapi/piel/models/physical/electronic/resistor/index.rst
+docs/autoapi/piel/models/physical/electronic/straight/index.rst
+docs/autoapi/piel/models/physical/electronic/taper/index.rst
+docs/autoapi/piel/models/physical/electronic/via_stack/index.rst
 docs/autoapi/piel/models/physical/geometry/index.rst
 docs/autoapi/piel/models/physical/opto_electronic/index.rst
 docs/autoapi/piel/models/physical/photonic/index.rst
 docs/autoapi/piel/models/physical/thermal/index.rst
 docs/autoapi/piel/models/physical/units/index.rst
 docs/autoapi/piel/models/transient/index.rst
 docs/autoapi/piel/models/transient/electrical/index.rst
@@ -81,26 +85,33 @@
 docs/autoapi/piel/project_structure/index.rst
 docs/autoapi/piel/tools/index.rst
 docs/autoapi/piel/tools/cocotb/index.rst
 docs/autoapi/piel/tools/cocotb/core/index.rst
 docs/autoapi/piel/tools/cocotb/data/index.rst
 docs/autoapi/piel/tools/gdsfactory/index.rst
 docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
+docs/autoapi/piel/tools/hdl21/index.rst
+docs/autoapi/piel/tools/hdl21/circuit/index.rst
+docs/autoapi/piel/tools/hdl21/simulator/index.rst
+docs/autoapi/piel/tools/hdl21/units/index.rst
 docs/autoapi/piel/tools/openlane/index.rst
 docs/autoapi/piel/tools/openlane/migrate/index.rst
 docs/autoapi/piel/tools/openlane/parse/index.rst
 docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
 docs/autoapi/piel/tools/openlane/parse/utils/index.rst
 docs/autoapi/piel/tools/openlane/utils/index.rst
 docs/autoapi/piel/tools/openlane/v1/index.rst
 docs/autoapi/piel/tools/openlane/v2/index.rst
-docs/autoapi/piel/tools/pyspice/index.rst
-docs/autoapi/piel/tools/pyspice/component/index.rst
+docs/autoapi/piel/tools/qutip/index.rst
+docs/autoapi/piel/tools/qutip/fock/index.rst
+docs/autoapi/piel/tools/qutip/unitary/index.rst
 docs/autoapi/piel/tools/sax/index.rst
 docs/autoapi/piel/tools/sax/utils/index.rst
+docs/autoapi/piel/tools/thewalrus/index.rst
+docs/autoapi/piel/tools/thewalrus/operations/index.rst
 docs/autoapi/piel/visual/index.rst
 docs/autoapi/piel/visual/auto_plot_multiple/index.rst
 docs/autoapi/piel/visual/data_conversion/index.rst
 docs/examples/designs/simple_design/simple_design/tb/Makefile
 docs/examples/designs/simple_design/simple_design/tb/default/Makefile
 docs/sections/about/AUTHORS.rst
 docs/sections/about/index.rst
@@ -111,19 +122,20 @@
 docs/sections/environment/setup.rst
 docs/sections/microservices/index.rst
 docs/sections/microservices/dependencies/cocotb.rst
 docs/sections/microservices/dependencies/gdsfactory.rst
 docs/sections/microservices/dependencies/index.rst
 docs/sections/microservices/dependencies/openlane.rst
 docs/sections/microservices/dependencies/principle.rst
-docs/sections/microservices/dependencies/pyspice.rst
 docs/sections/microservices/dependencies/sax.rst
+docs/sections/microservices/dependencies/spice.rst
 docs/sections/microservices/integration/index.rst
 docs/sections/microservices/integration/sax_qutip.rst
 docs/sections/models/index.rst
+docs/sections/models/spice_integration.rst
 piel/__init__.py
 piel/cli.py
 piel/config.py
 piel/defaults.py
 piel/file_conversion.py
 piel/file_system.py
 piel/parametric.py
@@ -135,21 +147,21 @@
 piel.egg-info/not-zip-safe
 piel.egg-info/requires.txt
 piel.egg-info/top_level.txt
 piel/components/__init__.py
 piel/integration/__init__.py
 piel/integration/cocotb_sax.py
 piel/integration/gdsfactory_openlane.py
-piel/integration/pyspice_sax.py
 piel/integration/sax_qutip.py
 piel/integration/sax_thewalrus.py
-piel/integration/gdsfactory_pyspice/__init__.py
-piel/integration/gdsfactory_pyspice/conversion.py
-piel/integration/gdsfactory_pyspice/core.py
-piel/integration/gdsfactory_pyspice/utils.py
+piel/integration/thewalrus_qutip.py
+piel/integration/gdsfactory_hdl21/__init__.py
+piel/integration/gdsfactory_hdl21/conversion.py
+piel/integration/gdsfactory_hdl21/core.py
+piel/integration/gdsfactory_hdl21/utils.py
 piel/models/__init__.py
 piel/models/utils.py
 piel/models/frequency/__init__.py
 piel/models/frequency/all.py
 piel/models/frequency/defaults.py
 piel/models/frequency/utils.py
 piel/models/frequency/electrical/__init__.py
@@ -178,52 +190,60 @@
 piel/models/physical/thermal.py
 piel/models/physical/units.py
 piel/models/physical/electrical/__init__.py
 piel/models/physical/electrical/cable.py
 piel/models/physical/electro_optic/__init__.py
 piel/models/physical/electro_optic/basic_heater.py
 piel/models/physical/electronic/__init__.py
-piel/models/physical/electronic/spice/__init__.py
-piel/models/physical/electronic/spice/capacitor.py
-piel/models/physical/electronic/spice/defaults.py
-piel/models/physical/electronic/spice/resistor.py
+piel/models/physical/electronic/capacitor.py
+piel/models/physical/electronic/defaults.py
+piel/models/physical/electronic/resistor.py
+piel/models/physical/electronic/straight.py
+piel/models/physical/electronic/taper.py
+piel/models/physical/electronic/via_stack.py
 piel/models/physical/opto_electronic/__init__.py
 piel/models/physical/photonic/__init__.py
 piel/models/transient/__init__.py
 piel/models/transient/electrical/__init__.py
 piel/models/transient/electro_optic/__init__.py
 piel/models/transient/electronic/__init__.py
 piel/models/transient/opto_electronic/__init__.py
 piel/models/transient/photonic/__init__.py
 piel/tools/__init__.py
 piel/tools/cocotb/__init__.py
 piel/tools/cocotb/core.py
 piel/tools/cocotb/data.py
 piel/tools/gdsfactory/__init__.py
 piel/tools/gdsfactory/netlist.py
+piel/tools/hdl21/__init__.py
+piel/tools/hdl21/circuit.py
+piel/tools/hdl21/simulator.py
+piel/tools/hdl21/units.py
 piel/tools/openlane/__init__.py
 piel/tools/openlane/migrate.py
 piel/tools/openlane/utils.py
 piel/tools/openlane/v1.py
 piel/tools/openlane/v2.py
 piel/tools/openlane/parse/__init__.py
 piel/tools/openlane/parse/run_output.py
 piel/tools/openlane/parse/sta_rpt.py
 piel/tools/openlane/parse/utils.py
-piel/tools/pyspice/__init__.py
-piel/tools/pyspice/component.py
+piel/tools/qutip/__init__.py
+piel/tools/qutip/fock.py
+piel/tools/qutip/unitary.py
 piel/tools/sax/__init__.py
 piel/tools/sax/utils.py
+piel/tools/thewalrus/__init__.py
+piel/tools/thewalrus/operations.py
 piel/visual/__init__.py
 piel/visual/auto_plot_multiple.py
 piel/visual/data_conversion.py
 tests/__init__.py
 tests/test_piel.py
 tests/integration/test_gdsfactory_netlist.py
 tests/integration/test_gdsfactory_netlist_to_pyspice.py
+tests/models/test_generator_call_connectivity.py
 tests/models/logic/electro_optic/test_signal_mapping.py
-tests/tools/__init__.py
-tests/tools/gdsfactory/__init__.py
+tests/tools/test_hdl21.py
 tests/tools/gdsfactory/test_netlist.py
-tests/tools/sax/__init__.py
 tests/tools/sax/test_utils.py
 tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.43/setup.py` & `piel-0.0.44/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open("README.rst") as readme_file:
+with open("README.md") as readme_file:
     readme = readme_file.read()
 
 requirements = [
     "bokeh",
     "jupyter_bokeh",
     "jupytext",
     "Click>=7.0",
     "cocotb",
+    "hdl21",
+    "jax",
     "gdsfactory",
     "networkx",
     "openlane",
     "pandas",
-    "pyspice",
     "sax",
-    "thewalrus" "qutip",
+    "thewalrus",
+    "vlsir",
+    "qutip",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
@@ -68,10 +71,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.43",
+    version="0.0.44",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.43/tests/integration/test_gdsfactory_netlist.py` & `piel-0.0.44/tests/integration/test_gdsfactory_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/tests/integration/test_gdsfactory_netlist_to_pyspice.py` & `piel-0.0.44/tests/integration/test_gdsfactory_netlist_to_pyspice.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/tests/models/logic/electro_optic/test_signal_mapping.py` & `piel-0.0.44/tests/models/logic/electro_optic/test_signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/tests/test_piel.py` & `piel-0.0.44/tests/test_piel.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/tests/tools/gdsfactory/test_netlist.py` & `piel-0.0.44/tests/tools/gdsfactory/test_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.43/tests/tools/sax/test_utils.py` & `piel-0.0.44/tests/tools/sax/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,10 +74,15 @@
 
 
 def test_sax_s_parameters_to_matrix():
     matrix = piel.sax_to_s_parameters_standard_matrix(sax_input=test_s_parameters)
     return matrix
 
 
+def test_sax_multi_indexing():
+    matrix = piel.sax_to_s_parameters_standard_matrix(sax_input=test_s_parameters)
+    return matrix
+
+
 if __name__ == "__main__":
     test_import_functions()
     test_sax_s_parameters_to_matrix()
```

### Comparing `piel-0.0.43/tests/visual/test_data_conversion.py` & `piel-0.0.44/tests/visual/test_data_conversion.py`

 * *Files identical despite different names*

