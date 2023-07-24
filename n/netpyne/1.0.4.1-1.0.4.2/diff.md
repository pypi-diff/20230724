# Comparing `tmp/netpyne-1.0.4.1-py2.py3-none-any.whl.zip` & `tmp/netpyne-1.0.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,99 +1,115 @@
-Zip file size: 406760 bytes, number of entries: 97
--rw-r--r--  2.0 unx      960 b- defN 23-Apr-12 06:10 netpyne/__init__.py
--rw-r--r--  2.0 unx     2070 b- defN 23-Mar-30 14:15 netpyne/analysis/__init__.py
--rw-r--r--  2.0 unx     7295 b- defN 23-Mar-30 14:15 netpyne/analysis/csd.py
--rw-r--r--  2.0 unx    20991 b- defN 23-Mar-30 14:15 netpyne/analysis/csd_legacy.py
--rw-r--r--  2.0 unx     7834 b- defN 23-Apr-12 06:10 netpyne/analysis/dipole.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Mar-30 14:15 netpyne/analysis/filter.py
--rw-r--r--  2.0 unx    17371 b- defN 23-Mar-30 14:15 netpyne/analysis/info.py
--rw-r--r--  2.0 unx   124721 b- defN 23-Mar-30 14:15 netpyne/analysis/interactive.py
--rw-r--r--  2.0 unx    11047 b- defN 23-Mar-30 14:15 netpyne/analysis/lfp.py
--rw-r--r--  2.0 unx    23008 b- defN 23-Mar-30 14:15 netpyne/analysis/lfp_orig.py
--rw-r--r--  2.0 unx     5813 b- defN 23-Mar-30 14:15 netpyne/analysis/mapping.py
--rw-r--r--  2.0 unx    60766 b- defN 23-Mar-30 14:15 netpyne/analysis/network.py
--rw-r--r--  2.0 unx     4601 b- defN 23-Mar-30 14:15 netpyne/analysis/rxd.py
--rw-r--r--  2.0 unx    14873 b- defN 23-Mar-30 14:15 netpyne/analysis/spikes.py
--rw-r--r--  2.0 unx    94592 b- defN 23-Mar-30 14:15 netpyne/analysis/spikes_legacy.py
--rw-r--r--  2.0 unx    16347 b- defN 23-Mar-30 14:15 netpyne/analysis/tools.py
--rw-r--r--  2.0 unx    22338 b- defN 23-Mar-30 14:15 netpyne/analysis/traces.py
--rw-r--r--  2.0 unx    25127 b- defN 23-Mar-30 14:15 netpyne/analysis/utils.py
--rw-r--r--  2.0 unx     1884 b- defN 23-Mar-30 14:15 netpyne/analysis/wrapper.py
--rw-r--r--  2.0 unx      300 b- defN 23-Mar-30 14:15 netpyne/batch/__init__.py
--rw-r--r--  2.0 unx    25000 b- defN 23-Mar-30 14:15 netpyne/batch/asd_parallel.py
--rw-r--r--  2.0 unx     9449 b- defN 23-Mar-30 14:15 netpyne/batch/batch.py
--rw-r--r--  2.0 unx     7770 b- defN 23-Mar-30 14:15 netpyne/batch/evol.py
--rw-r--r--  2.0 unx    14239 b- defN 23-Mar-30 14:15 netpyne/batch/grid.py
--rw-r--r--  2.0 unx     4997 b- defN 23-Mar-30 14:15 netpyne/batch/optuna_parallel.py
--rw-r--r--  2.0 unx     9105 b- defN 23-Mar-30 14:15 netpyne/batch/sbi_parallel.py
--rw-r--r--  2.0 unx    19610 b- defN 23-Mar-30 14:15 netpyne/batch/utils.py
--rw-r--r--  2.0 unx      843 b- defN 23-Mar-30 14:15 netpyne/cell/NML2Cell.py
--rw-r--r--  2.0 unx     1753 b- defN 23-Mar-30 14:15 netpyne/cell/NML2SpikeSource.py
--rw-r--r--  2.0 unx      414 b- defN 23-Mar-30 14:15 netpyne/cell/__init__.py
--rw-r--r--  2.0 unx    20013 b- defN 23-Mar-30 14:15 netpyne/cell/cell.py
--rw-r--r--  2.0 unx    88978 b- defN 23-Mar-30 14:15 netpyne/cell/compartCell.py
--rw-r--r--  2.0 unx     7190 b- defN 23-Mar-30 14:15 netpyne/cell/inputs.py
--rw-r--r--  2.0 unx    27753 b- defN 23-Mar-30 14:15 netpyne/cell/pointCell.py
--rw-r--r--  2.0 unx      631 b- defN 23-Mar-30 14:15 netpyne/conversion/__init__.py
--rw-r--r--  2.0 unx     3507 b- defN 23-Mar-30 14:15 netpyne/conversion/excel.py
--rw-r--r--  2.0 unx    78633 b- defN 23-Mar-30 14:15 netpyne/conversion/neuromlFormat.py
--rw-r--r--  2.0 unx    23046 b- defN 23-Mar-30 14:15 netpyne/conversion/neuronPyHoc.py
--rw-r--r--  2.0 unx     6120 b- defN 23-Mar-30 14:15 netpyne/conversion/pythonScript.py
--rw-r--r--  2.0 unx    53517 b- defN 23-Mar-30 14:15 netpyne/conversion/sonataImport.py
--rw-r--r--  2.0 unx      292 b- defN 23-Mar-30 14:15 netpyne/metadata/__init__.py
--rw-r--r--  2.0 unx     3330 b- defN 23-Mar-30 14:15 netpyne/metadata/api.py
--rw-r--r--  2.0 unx   170053 b- defN 23-Mar-30 14:15 netpyne/metadata/metadata.py
--rw-r--r--  2.0 unx      321 b- defN 23-Mar-30 14:15 netpyne/network/__init__.py
--rw-r--r--  2.0 unx    41371 b- defN 23-Mar-30 14:15 netpyne/network/conn.py
--rw-r--r--  2.0 unx     5396 b- defN 23-Mar-30 14:15 netpyne/network/modify.py
--rw-r--r--  2.0 unx    25179 b- defN 23-Mar-30 14:15 netpyne/network/netrxd.py
--rw-r--r--  2.0 unx     7519 b- defN 23-Mar-30 14:15 netpyne/network/network.py
--rw-r--r--  2.0 unx    28237 b- defN 23-Mar-30 14:15 netpyne/network/pop.py
--rw-r--r--  2.0 unx     1851 b- defN 23-Mar-30 14:15 netpyne/network/shape.py
--rw-r--r--  2.0 unx    11951 b- defN 23-Mar-30 14:15 netpyne/network/stim.py
--rw-r--r--  2.0 unx    18765 b- defN 23-Mar-30 14:15 netpyne/network/subconn.py
--rw-r--r--  2.0 unx     4515 b- defN 23-Mar-30 14:15 netpyne/plotting/__init__.py
--rw-r--r--  2.0 unx     9786 b- defN 23-Mar-30 14:15 netpyne/plotting/plotCSD.py
--rw-r--r--  2.0 unx     3241 b- defN 23-Mar-30 14:15 netpyne/plotting/plotLFPLocations.py
--rw-r--r--  2.0 unx    10110 b- defN 23-Mar-30 14:15 netpyne/plotting/plotLFPPSD.py
--rw-r--r--  2.0 unx     8566 b- defN 23-Mar-30 14:15 netpyne/plotting/plotLFPSpectrogram.py
--rw-r--r--  2.0 unx     9774 b- defN 23-Mar-30 14:15 netpyne/plotting/plotLFPTimeSeries.py
--rw-r--r--  2.0 unx    12844 b- defN 23-Mar-30 14:15 netpyne/plotting/plotRaster.py
--rw-r--r--  2.0 unx    12176 b- defN 23-Mar-30 14:15 netpyne/plotting/plotShape.py
--rw-r--r--  2.0 unx    18608 b- defN 23-Mar-30 14:15 netpyne/plotting/plotSpikeFreq.py
--rw-r--r--  2.0 unx    15963 b- defN 23-Mar-30 14:15 netpyne/plotting/plotSpikeHist.py
--rw-r--r--  2.0 unx    38248 b- defN 23-Mar-30 14:15 netpyne/plotting/plotter.py
--rw-r--r--  2.0 unx     3217 b- defN 23-Mar-30 14:15 netpyne/sim/__init__.py
--rw-r--r--  2.0 unx    33601 b- defN 23-Mar-30 14:15 netpyne/sim/gather.py
--rw-r--r--  2.0 unx    28969 b- defN 23-Mar-30 14:15 netpyne/sim/load.py
--rw-r--r--  2.0 unx    13703 b- defN 23-Mar-30 14:15 netpyne/sim/run.py
--rw-r--r--  2.0 unx    33895 b- defN 23-Mar-30 14:15 netpyne/sim/save.py
--rw-r--r--  2.0 unx    22874 b- defN 23-Mar-30 14:15 netpyne/sim/setup.py
--rw-r--r--  2.0 unx    30931 b- defN 23-Apr-07 10:11 netpyne/sim/utils.py
--rw-r--r--  2.0 unx     5464 b- defN 23-Mar-30 14:15 netpyne/sim/validate.py
--rw-r--r--  2.0 unx    54566 b- defN 23-Mar-30 14:15 netpyne/sim/validator.py
--rw-r--r--  2.0 unx    20492 b- defN 23-Mar-30 14:15 netpyne/sim/wrappers.py
--rw-r--r--  2.0 unx      402 b- defN 23-Mar-30 14:15 netpyne/specs/__init__.py
--rw-r--r--  2.0 unx     7937 b- defN 23-Mar-30 14:15 netpyne/specs/dicts.py
--rw-r--r--  2.0 unx    28513 b- defN 23-Mar-30 14:15 netpyne/specs/netParams.py
--rw-r--r--  2.0 unx     8937 b- defN 23-Mar-30 14:15 netpyne/specs/simConfig.py
--rw-r--r--  2.0 unx     3963 b- defN 23-Mar-30 14:15 netpyne/specs/utils.py
--rw-r--r--  2.0 unx      445 b- defN 23-Mar-30 14:15 netpyne/support/__init__.py
--rw-r--r--  2.0 unx    12729 b- defN 23-Mar-30 14:15 netpyne/support/bsmart.py
--rw-r--r--  2.0 unx     2264 b- defN 23-Mar-30 14:15 netpyne/support/csd.py
--rw-r--r--  2.0 unx    14818 b- defN 23-Mar-30 14:15 netpyne/support/filter.py
--rw-r--r--  2.0 unx     4830 b- defN 23-Mar-30 14:15 netpyne/support/morlet.py
--rw-r--r--  2.0 unx    18752 b- defN 23-Mar-30 14:15 netpyne/support/morphology.py
--rw-r--r--  2.0 unx     5583 b- defN 23-Mar-30 14:15 netpyne/support/nml_reader.py
--rw-r--r--  2.0 unx     6128 b- defN 23-Mar-30 14:15 netpyne/support/recxelectrode.py
--rw-r--r--  2.0 unx     3714 b- defN 23-Mar-30 14:15 netpyne/support/scalebar.py
--rw-r--r--  2.0 unx    11109 b- defN 23-Mar-30 14:15 netpyne/support/stackedBarGraph.py
--rw-r--r--  2.0 unx       39 b- defN 22-Feb-08 10:02 netpyne/tests/__init__.py
--rw-r--r--  2.0 unx     4395 b- defN 23-Mar-30 14:15 netpyne/tests/checks.py
--rw-r--r--  2.0 unx   219542 b- defN 23-Mar-30 14:15 netpyne/tests/tests.py
--rw-r--r--  2.0 unx   138393 b- defN 23-Mar-30 14:15 netpyne/tests/validate_tests.py
--rw-r--r--  2.0 unx     1086 b- defN 23-Apr-12 06:12 netpyne-1.0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1756 b- defN 23-Apr-12 06:12 netpyne-1.0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 06:12 netpyne-1.0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 06:12 netpyne-1.0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8100 b- defN 23-Apr-12 06:12 netpyne-1.0.4.1.dist-info/RECORD
-97 files, 2089234 bytes uncompressed, 394190 bytes compressed:  81.1%
+Zip file size: 414506 bytes, number of entries: 113
+-rw-r--r--  2.0 unx      960 b- defN 23-Jul-24 16:29 netpyne/__init__.py
+-rw-r--r--  2.0 unx     2070 b- defN 23-Jun-12 09:48 netpyne/analysis/__init__.py
+-rw-r--r--  2.0 unx     7295 b- defN 23-Jun-12 09:48 netpyne/analysis/csd.py
+-rw-r--r--  2.0 unx    20991 b- defN 23-Jun-12 09:48 netpyne/analysis/csd_legacy.py
+-rw-r--r--  2.0 unx     7834 b- defN 23-Jul-24 15:52 netpyne/analysis/dipole.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jun-12 09:48 netpyne/analysis/filter.py
+-rw-r--r--  2.0 unx    17371 b- defN 23-Jun-12 09:48 netpyne/analysis/info.py
+-rw-r--r--  2.0 unx   124721 b- defN 23-Jun-12 09:48 netpyne/analysis/interactive.py
+-rw-r--r--  2.0 unx    11047 b- defN 23-Jun-12 09:48 netpyne/analysis/lfp.py
+-rw-r--r--  2.0 unx    23008 b- defN 23-Jun-12 09:48 netpyne/analysis/lfp_orig.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Jul-24 15:52 netpyne/analysis/mapping.py
+-rw-r--r--  2.0 unx    60766 b- defN 23-Jul-24 15:52 netpyne/analysis/network.py
+-rw-r--r--  2.0 unx     4601 b- defN 23-Jun-12 09:48 netpyne/analysis/rxd.py
+-rw-r--r--  2.0 unx    14873 b- defN 23-Jun-12 09:48 netpyne/analysis/spikes.py
+-rw-r--r--  2.0 unx    94592 b- defN 23-Jul-24 15:52 netpyne/analysis/spikes_legacy.py
+-rw-r--r--  2.0 unx    16347 b- defN 23-Jul-24 15:52 netpyne/analysis/tools.py
+-rw-r--r--  2.0 unx    22338 b- defN 23-Jun-12 09:48 netpyne/analysis/traces.py
+-rw-r--r--  2.0 unx    25127 b- defN 23-Jul-24 15:52 netpyne/analysis/utils.py
+-rw-r--r--  2.0 unx     1884 b- defN 23-Jun-12 09:48 netpyne/analysis/wrapper.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Jun-12 09:48 netpyne/batch/__init__.py
+-rw-r--r--  2.0 unx    25000 b- defN 23-Jun-12 09:48 netpyne/batch/asd_parallel.py
+-rw-r--r--  2.0 unx     9449 b- defN 23-Jun-12 09:48 netpyne/batch/batch.py
+-rw-r--r--  2.0 unx     7770 b- defN 23-Jun-12 09:48 netpyne/batch/evol.py
+-rw-r--r--  2.0 unx    14239 b- defN 23-Jul-24 15:52 netpyne/batch/grid.py
+-rw-r--r--  2.0 unx     4997 b- defN 23-Jun-12 09:48 netpyne/batch/optuna_parallel.py
+-rw-r--r--  2.0 unx     9105 b- defN 23-Jun-12 09:48 netpyne/batch/sbi_parallel.py
+-rw-r--r--  2.0 unx    19610 b- defN 23-Jul-24 15:52 netpyne/batch/utils.py
+-rw-r--r--  2.0 unx      843 b- defN 23-Jun-12 09:48 netpyne/cell/NML2Cell.py
+-rw-r--r--  2.0 unx     1753 b- defN 23-Jun-12 09:48 netpyne/cell/NML2SpikeSource.py
+-rw-r--r--  2.0 unx      414 b- defN 23-Jun-12 09:48 netpyne/cell/__init__.py
+-rw-r--r--  2.0 unx    20013 b- defN 23-Jul-14 15:07 netpyne/cell/cell.py
+-rw-r--r--  2.0 unx    88978 b- defN 23-Jun-12 09:48 netpyne/cell/compartCell.py
+-rw-r--r--  2.0 unx     7190 b- defN 23-Jun-12 09:48 netpyne/cell/inputs.py
+-rw-r--r--  2.0 unx    27753 b- defN 23-Jun-12 09:48 netpyne/cell/pointCell.py
+-rw-r--r--  2.0 unx      631 b- defN 23-Jun-12 09:48 netpyne/conversion/__init__.py
+-rw-r--r--  2.0 unx     3507 b- defN 23-Jun-12 09:48 netpyne/conversion/excel.py
+-rw-r--r--  2.0 unx    78633 b- defN 23-Jun-12 09:48 netpyne/conversion/neuromlFormat.py
+-rw-r--r--  2.0 unx    23046 b- defN 23-Jun-12 09:48 netpyne/conversion/neuronPyHoc.py
+-rw-r--r--  2.0 unx     6120 b- defN 23-Jun-12 09:48 netpyne/conversion/pythonScript.py
+-rw-r--r--  2.0 unx    53517 b- defN 23-Jun-12 09:48 netpyne/conversion/sonataImport.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-12 09:48 netpyne/metadata/__init__.py
+-rw-r--r--  2.0 unx     3330 b- defN 23-Jun-12 09:48 netpyne/metadata/api.py
+-rw-r--r--  2.0 unx   170053 b- defN 23-Jun-12 09:48 netpyne/metadata/metadata.py
+-rw-r--r--  2.0 unx      321 b- defN 23-Jun-12 09:48 netpyne/network/__init__.py
+-rw-r--r--  2.0 unx    41371 b- defN 23-Jun-12 09:48 netpyne/network/conn.py
+-rw-r--r--  2.0 unx     5396 b- defN 23-Jun-12 09:48 netpyne/network/modify.py
+-rw-r--r--  2.0 unx    25179 b- defN 23-Jul-24 15:52 netpyne/network/netrxd.py
+-rw-r--r--  2.0 unx     7519 b- defN 23-Jun-12 09:48 netpyne/network/network.py
+-rw-r--r--  2.0 unx    28237 b- defN 23-Jun-12 09:48 netpyne/network/pop.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Jun-12 09:48 netpyne/network/shape.py
+-rw-r--r--  2.0 unx    11951 b- defN 23-Jun-12 09:48 netpyne/network/stim.py
+-rw-r--r--  2.0 unx    18765 b- defN 23-Jun-12 09:48 netpyne/network/subconn.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-Jun-12 09:48 netpyne/plotting/__init__.py
+-rw-r--r--  2.0 unx     9786 b- defN 23-Jun-12 09:48 netpyne/plotting/plotCSD.py
+-rw-r--r--  2.0 unx     3241 b- defN 23-Jun-12 09:48 netpyne/plotting/plotLFPLocations.py
+-rw-r--r--  2.0 unx    10110 b- defN 23-Jun-12 09:48 netpyne/plotting/plotLFPPSD.py
+-rw-r--r--  2.0 unx     8566 b- defN 23-Jun-12 09:48 netpyne/plotting/plotLFPSpectrogram.py
+-rw-r--r--  2.0 unx     9774 b- defN 23-Jun-12 09:48 netpyne/plotting/plotLFPTimeSeries.py
+-rw-r--r--  2.0 unx    12844 b- defN 23-Jul-24 15:52 netpyne/plotting/plotRaster.py
+-rw-r--r--  2.0 unx    12176 b- defN 23-Jun-12 09:48 netpyne/plotting/plotShape.py
+-rw-r--r--  2.0 unx    18608 b- defN 23-Jun-12 09:48 netpyne/plotting/plotSpikeFreq.py
+-rw-r--r--  2.0 unx    15963 b- defN 23-Jun-12 09:48 netpyne/plotting/plotSpikeHist.py
+-rw-r--r--  2.0 unx    38344 b- defN 23-Jul-24 16:29 netpyne/plotting/plotter.py
+-rw-r--r--  2.0 unx     3217 b- defN 23-Jun-12 09:48 netpyne/sim/__init__.py
+-rw-r--r--  2.0 unx    33601 b- defN 23-Jul-24 15:52 netpyne/sim/gather.py
+-rw-r--r--  2.0 unx    28969 b- defN 23-Jul-24 15:52 netpyne/sim/load.py
+-rw-r--r--  2.0 unx    13703 b- defN 23-Jun-12 09:48 netpyne/sim/run.py
+-rw-r--r--  2.0 unx    33895 b- defN 23-Jul-24 15:52 netpyne/sim/save.py
+-rw-r--r--  2.0 unx    22874 b- defN 23-Jul-24 15:52 netpyne/sim/setup.py
+-rw-r--r--  2.0 unx    30931 b- defN 23-Jul-24 15:52 netpyne/sim/utils.py
+-rw-r--r--  2.0 unx     5464 b- defN 23-Jun-12 09:48 netpyne/sim/validate.py
+-rw-r--r--  2.0 unx    54566 b- defN 23-Jul-24 15:52 netpyne/sim/validator.py
+-rw-r--r--  2.0 unx    20492 b- defN 23-Jun-12 09:48 netpyne/sim/wrappers.py
+-rw-r--r--  2.0 unx      402 b- defN 23-Jun-12 09:48 netpyne/specs/__init__.py
+-rw-r--r--  2.0 unx     7937 b- defN 23-Jun-12 09:48 netpyne/specs/dicts.py
+-rw-r--r--  2.0 unx    28513 b- defN 23-Jun-12 09:48 netpyne/specs/netParams.py
+-rw-r--r--  2.0 unx     8937 b- defN 23-Jun-12 09:48 netpyne/specs/simConfig.py
+-rw-r--r--  2.0 unx     3963 b- defN 23-Jun-12 09:48 netpyne/specs/utils.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-12 09:48 netpyne/support/__init__.py
+-rw-r--r--  2.0 unx    12729 b- defN 23-Jun-12 09:48 netpyne/support/bsmart.py
+-rw-r--r--  2.0 unx     2264 b- defN 23-Jun-12 09:48 netpyne/support/csd.py
+-rw-r--r--  2.0 unx    14818 b- defN 23-Jun-12 09:48 netpyne/support/filter.py
+-rw-r--r--  2.0 unx     4830 b- defN 23-Jun-12 09:48 netpyne/support/morlet.py
+-rw-r--r--  2.0 unx    18752 b- defN 23-Jun-12 09:48 netpyne/support/morphology.py
+-rw-r--r--  2.0 unx     5583 b- defN 23-Jun-12 09:48 netpyne/support/nml_reader.py
+-rw-r--r--  2.0 unx     6128 b- defN 23-Jun-12 09:48 netpyne/support/recxelectrode.py
+-rw-r--r--  2.0 unx     3714 b- defN 23-Jun-12 09:48 netpyne/support/scalebar.py
+-rw-r--r--  2.0 unx    11109 b- defN 23-Jun-12 09:48 netpyne/support/stackedBarGraph.py
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-12 09:48 netpyne/tests/__init__.py
+-rw-r--r--  2.0 unx     4395 b- defN 23-Jun-12 09:48 netpyne/tests/checks.py
+-rw-r--r--  2.0 unx   219542 b- defN 23-Jun-12 09:48 netpyne/tests/tests.py
+-rw-r--r--  2.0 unx   138393 b- defN 23-Jun-12 09:48 netpyne/tests/validate_tests.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 09:48 tests/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 09:48 tests/doc/__init__.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jun-12 09:48 tests/doc/test_tutorials.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 09:48 tests/examples/__init__.py
+-rw-r--r--  2.0 unx      373 b- defN 23-Jun-12 09:48 tests/examples/test_HHTut.py
+-rw-r--r--  2.0 unx      389 b- defN 23-Jun-12 09:48 tests/examples/test_HybridTut.py
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 09:48 tests/examples/test_LFPrecording.py
+-rw-r--r--  2.0 unx      377 b- defN 23-Jun-12 09:48 tests/examples/test_M1.py
+-rw-r--r--  2.0 unx      290 b- defN 23-Jun-12 09:48 tests/examples/test_NeuroMLImport.py
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-12 09:48 tests/examples/test_PTcell.py
+-rw-r--r--  2.0 unx     1246 b- defN 23-Jun-12 09:48 tests/examples/test_batchCell.py
+-rw-r--r--  2.0 unx     3884 b- defN 23-Jun-12 09:48 tests/examples/test_evolCell.py
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-12 09:48 tests/examples/test_rxd_buffering.py
+-rw-r--r--  2.0 unx      278 b- defN 23-Jun-12 09:48 tests/examples/test_rxd_net.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Jun-12 09:48 tests/examples/test_saving.py
+-rw-r--r--  2.0 unx      855 b- defN 23-Jun-12 09:48 tests/examples/utils.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jul-24 16:31 netpyne-1.0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1746 b- defN 23-Jul-24 16:31 netpyne-1.0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 16:31 netpyne-1.0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-24 16:31 netpyne-1.0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9451 b- defN 23-Jul-24 16:31 netpyne-1.0.4.2.dist-info/RECORD
+113 files, 2101253 bytes uncompressed, 399806 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -270,23 +270,71 @@
 
 Filename: netpyne/tests/tests.py
 Comment: 
 
 Filename: netpyne/tests/validate_tests.py
 Comment: 
 
-Filename: netpyne-1.0.4.1.dist-info/LICENSE
+Filename: tests/__init__.py
 Comment: 
 
-Filename: netpyne-1.0.4.1.dist-info/METADATA
+Filename: tests/doc/__init__.py
 Comment: 
 
-Filename: netpyne-1.0.4.1.dist-info/WHEEL
+Filename: tests/doc/test_tutorials.py
 Comment: 
 
-Filename: netpyne-1.0.4.1.dist-info/top_level.txt
+Filename: tests/examples/__init__.py
 Comment: 
 
-Filename: netpyne-1.0.4.1.dist-info/RECORD
+Filename: tests/examples/test_HHTut.py
+Comment: 
+
+Filename: tests/examples/test_HybridTut.py
+Comment: 
+
+Filename: tests/examples/test_LFPrecording.py
+Comment: 
+
+Filename: tests/examples/test_M1.py
+Comment: 
+
+Filename: tests/examples/test_NeuroMLImport.py
+Comment: 
+
+Filename: tests/examples/test_PTcell.py
+Comment: 
+
+Filename: tests/examples/test_batchCell.py
+Comment: 
+
+Filename: tests/examples/test_evolCell.py
+Comment: 
+
+Filename: tests/examples/test_rxd_buffering.py
+Comment: 
+
+Filename: tests/examples/test_rxd_net.py
+Comment: 
+
+Filename: tests/examples/test_saving.py
+Comment: 
+
+Filename: tests/examples/utils.py
+Comment: 
+
+Filename: netpyne-1.0.4.2.dist-info/LICENSE
+Comment: 
+
+Filename: netpyne-1.0.4.2.dist-info/METADATA
+Comment: 
+
+Filename: netpyne-1.0.4.2.dist-info/WHEEL
+Comment: 
+
+Filename: netpyne-1.0.4.2.dist-info/top_level.txt
+Comment: 
+
+Filename: netpyne-1.0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netpyne/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 NetPyNE (Networks using Python and NEURON) is a Python package to facilitate the development, simulation, parallelization, analysis, and optimization of biological neuronal networks using the NEURON simulator.
 
 NetPyNE consists of a number of sub-packages and modules.
 """
 
-__version__ = '1.0.4.1'
+__version__ = '1.0.4.2'
 import os, sys
 
 display = os.getenv('DISPLAY')
 nogui = sys.argv.count('-nogui') > 0
 
 __gui__ = True
```

## netpyne/plotting/plotter.py

```diff
@@ -83,27 +83,29 @@
         if not sim:
             from .. import sim
         self.sim = sim
 
         self.kind = kind
 
         # Make a copy of the current matplotlib rcParams and update them
-        self.orig_rcParams = deepcopy(mpl.rcParamsDefault)
+        self.orig_rcParams = deepcopy(mpl.rcParams)
         if 'rcParams' in kwargs:
             new_rcParams = kwargs['rcParams']
             if type(new_rcParams) == dict:
                 for rcParam in new_rcParams:
                     if rcParam in mpl.rcParams:
                         mpl.rcParams[rcParam] = new_rcParams[rcParam]
                     else:
                         print(
                             '  Not found in matplotlib.rcParams:',
                             rcParam,
                         )
                 self.rcParams = mpl.rcParams
+            else:
+                print('Ignoring rcParams argument, since it has to be of type dict')
         else:
             self.rcParams = self.orig_rcParams
 
         # Set up any subplots
         if not subplots:
             nrows = 1
             ncols = 1
```

## Comparing `netpyne-1.0.4.1.dist-info/LICENSE` & `netpyne-1.0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netpyne-1.0.4.1.dist-info/METADATA` & `netpyne-1.0.4.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpyne
-Version: 1.0.4.1
+Version: 1.0.4.2
 Summary: A Python package to develop, simulate and analyse biological neuronal networks in NEURON.
 Home-page: https://github.com/Neurosim-lab/netpyne
 Author: Salvador Dura-Bernal (Neurosim lab)
 Author-email: salvadordura@gmail.com
 License: MIT
 Keywords: neuron,network,developing,framework,biological,simulation
 Platform: UNKNOWN
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: matplotlib (<=3.5.1)
+Requires-Dist: matplotlib
 Requires-Dist: matplotlib-scalebar
 Requires-Dist: future
 Requires-Dist: pandas
 Requires-Dist: bokeh
 Requires-Dist: schema
 Requires-Dist: lfpykit
```

## Comparing `netpyne-1.0.4.1.dist-info/RECORD` & `netpyne-1.0.4.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-netpyne/__init__.py,sha256=6_08e-5YjcGu5Po__aWpSGeINMfAqtlbRYqjt2Dw4CM,960
+netpyne/__init__.py,sha256=jva2DRoJ1pYF4OoVF13K0Ip7QwCLR3_TA_C6fNsgN1Q,960
 netpyne/analysis/__init__.py,sha256=r4FWwg1v8akv6G1N27KjcECMmRziIPa6fY51wiHDWAE,2070
 netpyne/analysis/csd.py,sha256=MlnbgoJ9Cn6Z8COpml398LHq7Rw1clmWAAGW9keg3sk,7295
 netpyne/analysis/csd_legacy.py,sha256=K1ajCYCWE6UgdQsGS3wg5J7kVloa8vX25s-PFWG3bY8,20991
 netpyne/analysis/dipole.py,sha256=kYqqSR_wZBdWSYVJhLAEO7ZOQTqSoW1X5IGgB_9XNaI,7834
 netpyne/analysis/filter.py,sha256=TLcD2yhQy635MbsZo4k7UoiLmiT4sTgKZe1pIv5wI6g,15367
 netpyne/analysis/info.py,sha256=trpjvw3vgex1Wy8dYsd8jYVibo0l2eoIqdy56e7HgcI,17371
 netpyne/analysis/interactive.py,sha256=mKCJjwQ4cQd9sGEVwdaXlnIx5PgwhmyFI-68f9EGppo,124721
@@ -56,15 +56,15 @@
 netpyne/plotting/plotLFPPSD.py,sha256=pugt3G3NgWC5jNd7JBnHqz7eZ7Q1dLkiMRJC8s3-1L4,10110
 netpyne/plotting/plotLFPSpectrogram.py,sha256=5xFB9kvvaF9LI5mQMf-pK2TtO2mDJwMoJdZILixNygU,8566
 netpyne/plotting/plotLFPTimeSeries.py,sha256=z-3M2b-LY-n9PaQwprcFSlchLsDRKOmMBzRyG2uIBYI,9774
 netpyne/plotting/plotRaster.py,sha256=Lw2I1V17-s_7d38xz0mY-_Cryc0CPG6iTGtYJa9e_L0,12844
 netpyne/plotting/plotShape.py,sha256=01dqvTwyWb_Zafhos5uKufIWzICL1iSFGOPi7nhI2Sk,12176
 netpyne/plotting/plotSpikeFreq.py,sha256=f0m-9TRneAoTXvFQE9fYknYVTPHKlEB4zxBQTFJ2eA4,18608
 netpyne/plotting/plotSpikeHist.py,sha256=cnsDRGfa9AjJgEY3H594ZwdumWLrEeoFEfRjCCmIyUU,15963
-netpyne/plotting/plotter.py,sha256=QIG8T_70HveuxO0esHTfXqeTEVuRj_Quswe87LiylvM,38248
+netpyne/plotting/plotter.py,sha256=bNzHXU2yoou0W8sQ1XVN8_IW7N0fj7SpzfEmWy8u3TE,38344
 netpyne/sim/__init__.py,sha256=-LZZKea3Uo0FvtnDj87X9uzi698_a7m2fRRKoUWGhDg,3217
 netpyne/sim/gather.py,sha256=kmq3ByWDmBsFAD5OAFdlu074NBTYeNUkB2NozOKHDVI,33601
 netpyne/sim/load.py,sha256=kwIQXcSoc3-xuvyO8dZKSMLowq3aFs020ZUurUcqhUo,28969
 netpyne/sim/run.py,sha256=Wjstc7O-VMqNsCm9e-fJRZXJ2q5Ee624IDWzvMlGr4Q,13703
 netpyne/sim/save.py,sha256=IDr8ehlXhrDKw-AmUbd4O3NSpelPQ2OdP8Ugk7XVxH4,33895
 netpyne/sim/setup.py,sha256=Lir_0Aj-ynqgud6-qvfJG4kNbMrTmrJYCaEV1sWccXY,22874
 netpyne/sim/utils.py,sha256=OgfUjuNh6XYN70z7YGI-8K4x1ajLtMml2XXrPnOYxNY,30931
@@ -86,12 +86,28 @@
 netpyne/support/recxelectrode.py,sha256=kibQlAc9sYKHa88LZ__H-Nzmy4L1JpYCnOjmkNxXKfI,6128
 netpyne/support/scalebar.py,sha256=JooxLXBaeYVoy6bSsvX4kz4lHPPVT8xY5xssc5rTLYA,3714
 netpyne/support/stackedBarGraph.py,sha256=ZNT4nLBtcffRLwJKcBwmU3xgMg0u0WoYPITynkodv-Y,11109
 netpyne/tests/__init__.py,sha256=qhKTtTUS_LZGZsMCROd6OBpR4ADicJcheBffjAr-wu4,39
 netpyne/tests/checks.py,sha256=eSPJ0aYIATQ_TJojS8SMx1_9h_scYKIyqlZBzB6SDNk,4395
 netpyne/tests/tests.py,sha256=5XZSucIg50MMPPkMkdofVEcPSdAyO6vFB72h4IreuBU,219542
 netpyne/tests/validate_tests.py,sha256=jChJ6d9pDkjPJtynALXP0Pl_zOkE_U0nE_3ahixvkJ8,138393
-netpyne-1.0.4.1.dist-info/LICENSE,sha256=HLJWurv-6_6xf37pz7EvKVJBGsqYs-SYR8Fz5AFYBgQ,1086
-netpyne-1.0.4.1.dist-info/METADATA,sha256=541DFRj4G8U9T34bb6Abq4br0aQw93cR0mujy-NnMOA,1756
-netpyne-1.0.4.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-netpyne-1.0.4.1.dist-info/top_level.txt,sha256=1OoDIpIeeCT67cpLYM4Z9O359GDd96LbC-JRZm_naS4,8
-netpyne-1.0.4.1.dist-info/RECORD,,
+tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/doc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/doc/test_tutorials.py,sha256=xxqrDypOmH59MXja6fngTtw4E4gxzNH1dOCM4pZF1S0,1665
+tests/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/examples/test_HHTut.py,sha256=gOWUUOnXyez31q-h_DbbTTwjMsIKXs3kxQbooOOyLqk,373
+tests/examples/test_HybridTut.py,sha256=XF-LgvSZpajew44ik124TCDXSAWyXsTSV1x13QnGZ0M,389
+tests/examples/test_LFPrecording.py,sha256=WdDGa9Awtqpr2DxYPmUzy7wTyTZQra9ap123VO45jmo,298
+tests/examples/test_M1.py,sha256=leG5M5QpQCeORVxh2FNfKafSKwE0bZIbm350LLa41mo,377
+tests/examples/test_NeuroMLImport.py,sha256=oAUlIUJ4Xc5sYXkla4Kx6bW5OIckuCDCwr_PhY2JR1Y,290
+tests/examples/test_PTcell.py,sha256=FPLpZS2PbpQdTJWiXL2Lx8sLhBWYDtWUFcc-ZPNGryU,343
+tests/examples/test_batchCell.py,sha256=KkPmDXbgjn4Z3ehZWF32Mm0aAuzWrpnlGL5wg16lQM0,1246
+tests/examples/test_evolCell.py,sha256=r9tUxPrcvcoVpexYVgUT_6fVCKYQgh3_V94Mc7ckhN4,3884
+tests/examples/test_rxd_buffering.py,sha256=LqA2Lg0xL--YFltUNGxGzi9wLfNg0iosbYAd0kYMCGM,269
+tests/examples/test_rxd_net.py,sha256=8Cssk5Sa1J4_O7lbifub3Q6O6CZkM6eDnIhOh3OeRVA,278
+tests/examples/test_saving.py,sha256=nCuPmHbz-itxGWphjxJi7jEbTrjVIGKrXVwqUI92T6g,309
+tests/examples/utils.py,sha256=39F4UoVlM1vDBBQ76g8KiiQfSd0q_5i3hvHFdC2G76k,855
+netpyne-1.0.4.2.dist-info/LICENSE,sha256=HLJWurv-6_6xf37pz7EvKVJBGsqYs-SYR8Fz5AFYBgQ,1086
+netpyne-1.0.4.2.dist-info/METADATA,sha256=6d-wXVNcG1wtNDZpQOROhYe_csOY1i6BCiPfwoGlztM,1746
+netpyne-1.0.4.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+netpyne-1.0.4.2.dist-info/top_level.txt,sha256=eh6bRckhcJ4rs5301chotlYdu6Ws62X8jC1PoCoXyjg,14
+netpyne-1.0.4.2.dist-info/RECORD,,
```

