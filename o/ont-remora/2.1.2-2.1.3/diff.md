# Comparing `tmp/ont-remora-2.1.2.tar.gz` & `tmp/ont-remora-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-remora-2.1.2.tar", last modified: Mon Jun  5 23:01:35 2023, max compression
+gzip compressed data, was "ont-remora-2.1.3.tar", last modified: Mon Jul 24 14:06:07 2023, max compression
```

## Comparing `ont-remora-2.1.2.tar` & `ont-remora-2.1.3.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.369026 ont-remora-2.1.2/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont-remora-2.1.2/LICENSE.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont-remora-2.1.2/MANIFEST.in
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    11706 2023-06-05 23:01:35.369150 ont-remora-2.1.2/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     9399 2023-06-05 22:56:02.000000 ont-remora-2.1.2/README.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-05-18 20:02:58.000000 ont-remora-2.1.2/pyproject.toml
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1628 2023-06-05 23:01:35.369734 ont-remora-2.1.2/setup.cfg
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2023-05-18 20:02:58.000000 ont-remora-2.1.2/setup.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.361251 ont-remora-2.1.2/src/
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.363567 ont-remora-2.1.2/src/ont_remora.egg-info/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    11706 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      868 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/SOURCES.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/dependency_links.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       44 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/entry_points.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-2.1.2/src/ont_remora.egg-info/not-zip-safe
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      172 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/requires.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-06-05 23:01:35.000000 ont-remora-2.1.2/src/ont_remora.egg-info/top_level.txt
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.368423 ont-remora-2.1.2/src/remora/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-06-05 22:56:02.000000 ont-remora-2.1.2/src/remora/__init__.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/activations.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     4795 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/constants.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    61354 2023-06-05 22:31:56.000000 ont-remora-2.1.2/src/remora/data_chunks.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/download.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/duplex_utils.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/encoded_kmers.pyx
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19661 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/inference.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    66346 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/io.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2393 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/log.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1896 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/main.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/metrics.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    21010 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/model_util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    58747 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/parsers.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7270 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/prepare_train_data.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    25051 2023-06-05 22:07:36.000000 ont-remora-2.1.2/src/remora/refine_signal_map.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18990 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/refine_signal_map_core.pyx
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    17738 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/train_model.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-06-05 23:01:35.368747 ont-remora-2.1.2/src/remora/trained_models/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/trained_models/readme.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    16903 2023-06-05 22:07:47.000000 ont-remora-2.1.2/src/remora/util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    21001 2023-05-18 20:02:58.000000 ont-remora-2.1.2/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.429655 ont-remora-2.1.3/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2023-05-18 20:02:58.000000 ont-remora-2.1.3/LICENSE.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2023-05-18 20:02:58.000000 ont-remora-2.1.3/MANIFEST.in
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     9823 2023-07-24 14:06:07.429741 ont-remora-2.1.3/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     9399 2023-07-24 13:21:57.000000 ont-remora-2.1.3/README.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2023-07-19 22:44:10.000000 ont-remora-2.1.3/pyproject.toml
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1628 2023-07-24 14:06:07.430368 ont-remora-2.1.3/setup.cfg
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2023-07-24 13:21:57.000000 ont-remora-2.1.3/setup.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.414588 ont-remora-2.1.3/src/
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.419487 ont-remora-2.1.3/src/ont_remora.egg-info/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     9823 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      939 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/SOURCES.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/dependency_links.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       43 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/entry_points.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-18 20:26:40.000000 ont-remora-2.1.3/src/ont_remora.egg-info/not-zip-safe
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      172 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/requires.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-07-24 14:06:07.000000 ont-remora-2.1.3/src/ont_remora.egg-info/top_level.txt
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.427874 ont-remora-2.1.3/src/remora/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-07-24 14:03:35.000000 ont-remora-2.1.3/src/remora/__init__.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2023-05-18 20:02:58.000000 ont-remora-2.1.3/src/remora/activations.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     4795 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/constants.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    61354 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/data_chunks.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-05-18 20:02:58.000000 ont-remora-2.1.3/src/remora/download.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-06-05 22:07:36.000000 ont-remora-2.1.3/src/remora/duplex_utils.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/encoded_kmers.pyx
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19661 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/inference.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    66346 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/io.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2393 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/log.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1896 2023-05-18 20:02:58.000000 ont-remora-2.1.3/src/remora/main.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-05-18 20:02:58.000000 ont-remora-2.1.3/src/remora/metrics.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    21010 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/model_util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    58747 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/parsers.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7270 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/prepare_train_data.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    25051 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/refine_signal_map.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18995 2023-07-24 13:23:47.000000 ont-remora-2.1.3/src/remora/refine_signal_map_core.pyx
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    17738 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/train_model.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.428228 ont-remora-2.1.3/src/remora/trained_models/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2023-05-18 20:02:58.000000 ont-remora-2.1.3/src/remora/trained_models/readme.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    16903 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    21001 2023-07-24 13:21:57.000000 ont-remora-2.1.3/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-07-24 14:06:07.429367 ont-remora-2.1.3/tests/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      679 2023-05-18 20:02:58.000000 ont-remora-2.1.3/tests/test_coding_standards.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12174 2023-05-18 20:02:58.000000 ont-remora-2.1.3/tests/test_duplex.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     8835 2023-07-24 13:21:57.000000 ont-remora-2.1.3/tests/test_main.py
```

### Comparing `ont-remora-2.1.2/LICENSE.txt` & `ont-remora-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/PKG-INFO` & `ont-remora-2.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,250 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.1.2
+Version: 2.1.3
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
-Description: .. image:: /ONT_logo.png
-          :width: 800
-          :alt: [Oxford Nanopore Technologies]
-          :target: https://nanoporetech.com/
-        
-        Remora
-        """"""
-        
-        Methylation/modified base calling separated from basecalling.
-        Remora primarily provides an API to call modified bases for basecaller programs such as Bonito.
-        Remora also provides the tools to prepare datasets, train modified base models and run simple inference.
-        
-        Installation
-        ------------
-        
-        Install from pypi:
-        
-        ::
-        
-           pip install ont-remora
-        
-        Install from github source for development:
-        
-        ::
-        
-           git clone git@github.com:nanoporetech/remora.git
-           pip install -e remora/[tests]
-        
-        It is recommended that Remora be installed in a virtual environment.
-        For example ``python3.8 -m venv --prompt remora --copies venv; source venv/bin/activate``.
-        
-        See help for any Remora sub-command with the ``-h`` flag.
-        
-        Getting Started
-        ---------------
-        
-        Remora models are trained to perform binary or categorical prediction of modified base content of a nanopore read.
-        Models may also be trained to perform canonical base prediction, but this feature may be removed at a later time.
-        The rest of the documentation will focus on the modified base detection task.
-        
-        The Remora training/prediction input unit (referred to as a chunk) consists of:
-        
-        1. Section of normalized signal
-        2. Canonical bases attributed to the section of signal
-        3. Mapping between these two
-        
-        Chunks have a fixed signal length defined at data preparation time and saved as a model attribute.
-        A fixed position within the chunk is defined as the "focus position".
-        By default, this position is the center of the "focus base" being interrogated by the model.
-        
-        Pre-trained Models
-        ------------------
-        
-        See the selection of current released models with ``remora model list_pretrained``.
-        Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
-        
-        Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
-        See Bonito documentation to apply Remora models.
-        
-        More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
-        Note that older ONNX format models require Remora version < 2.0.
-        
-        Python API
-        ----------
-        
-        The Remora API can be applied to make modified base calls given a basecalled read via a ``RemoraRead`` object.
-        
-        * ``dacs`` (Data acquisition values) should be an int16 numpy array.
-        * ``shift`` and ``scale`` are float values to convert dacs to mean=0 SD=1 scaling (or similar) for input to the Remora neural network.
-        * ``str_seq`` is a string derived from ``sig`` (can be either basecalls or other downstream derived sequence; e.g. mapped reference positions).
-        * ``seq_to_sig_map`` should be an int32 numpy array of length ``len(seq) + 1`` and elements should be indices within ``sig`` array assigned to each base in ``seq``.
-        
-        .. code-block:: python
-        
-          from remora.model_util import load_model
-          from remora.data_chunks import RemoraRead
-          from remora.inference import call_read_mods
-        
-          model, model_metadata = load_model("remora_train_results/model_best.pt")
-          read = RemoraRead(dacs, shift, scale, seq_to_sig_map, str_seq=seq)
-          mod_probs, _, pos = call_read_mods(
-            read,
-            model,
-            model_metadata,
-            return_mod_probs=True,
-          )
-        
-        ``mod_probs`` will contain the probability of each modeled modified base as found in model_metadata["mod_long_names"].
-        For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
-        ``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
-        
-        Data Preparation
-        ----------------
-        
-        Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
-        Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
-        
-        The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
-        Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
-        
-        K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
-        
-        .. code-block:: bash
-        
-          remora \
-            dataset prepare \
-            can_reads.pod5 \
-            can_mappings.bam \
-            --output-remora-training-file can_chunks.npz \
-            --log-filename prep_can.log \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --motif CG 0 \
-            --mod-base-control
-          remora \
-            dataset prepare \
-            mod_reads.pod5 \
-            mod_mappings.bam \
-            --output-remora-training-file mod_chunks.npz \
-            --log-filename prep_can.log \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --motif CG 0 \
-            --mod-base m 5mC
-          remora \
-            dataset merge \
-            --input-dataset can_chunks.npz 10_000_000 \
-            --input-dataset mod_chunks.npz 10_000_000 \
-            --output-dataset chunks.npz
-        
-        The resulting ``chunks.npz`` file can then be used to train a Remora model.
-        
-        Model Training
-        --------------
-        
-        Models are trained with the ``remora model train`` command.
-        For example a model can be trained with the following command.
-        
-        .. code-block:: bash
-        
-          remora \
-            model train \
-            chunks.npz \
-            --model remora/models/ConvLSTM_w_ref.py \
-            --device 0 \
-            --output-path train_results
-        
-        This command will produce a "best" model in torchscript format for use in Bonito, or ``remora infer`` commands.
-        
-        Model Inference
-        ---------------
-        
-        For testing purposes inference within Remora is provided.
-        
-        .. code-block:: bash
-        
-          remora \
-            infer from_pod5_and_bam \
-            can_signal.pod5 \
-            can_basecalls.bam \
-            --model train_results/model_best.pt \
-            --out-file can_infer.bam \
-            --device 0
-          remora \
-            infer from_pod5_and_bam \
-            mod_signal.pod5 \
-            mod_basecalls.bam \
-            --model train_results/model_best.pt \
-            --out-file mod_infer.bam \
-            --device 0
-        
-        Finally, ``Remora`` provides tools to validate these results.
-        Ground truth BED files references positions where each read should be called as the modified or canonical base listed in the BED name field.
-        
-        .. code-block:: bash
-        
-          remora \
-            validate from_modbams \
-            --bam-and-bed can_infer.bam can_ground_truth.bed \
-            --bam-and-bed mod_infer.bam mod_ground_truth.bed \
-            --full-output-filename validation_results.txt
-        
-        Raw Signal Analysis
-        -------------------
-        
-        As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
-        The ``remora analyze`` command group contains the ``plot ref_region`` command.
-        Additional commands will be added to this group to produce more useful raw signal analysis tasks.
-        
-        The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
-        
-        As an example using the test data, the following command produces the plot below.
-        
-        .. code-block:: bash
-        
-          remora \
-            analyze plot ref_region \
-            --pod5-and-bam can_reads.pod5 can_mappings.bam \
-            --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
-            --ref-regions ref_regions.bed \
-            --highlight-ranges mod_gt.bed \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --log-filename log.txt
-        
-        .. image:: images/plot_ref_region_fwd.png
-           :width: 600
-           :alt: Plot reference region image (forward strand)
-        
-        .. image:: images/plot_ref_region_rev.png
-           :width: 600
-           :alt: Plot reference region image (reverse strand)
-        
-        Raw Signal Analysis
-        -------------------
-        
-        The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
-        This is API is primarily accessed via the ``remora.io.Read`` object.
-        
-        The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
-        
-        Terms and Licence
-        -----------------
-        
-        This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
-        Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
-        Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
-        Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
-        Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
-        
-        © 2021 Oxford Nanopore Technologies Ltd.
-        Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
-        
-        Research Release
-        ----------------
-        
-        Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
 Provides-Extra: tests
+License-File: LICENSE.txt
+
+.. image:: /ONT_logo.png
+  :width: 800
+  :alt: [Oxford Nanopore Technologies]
+  :target: https://nanoporetech.com/
+
+Remora
+""""""
+
+Methylation/modified base calling separated from basecalling.
+Remora primarily provides an API to call modified bases for basecaller programs such as Bonito.
+Remora also provides the tools to prepare datasets, train modified base models and run simple inference.
+
+Installation
+------------
+
+Install from pypi:
+
+::
+
+   pip install ont-remora
+
+Install from github source for development:
+
+::
+
+   git clone git@github.com:nanoporetech/remora.git
+   pip install -e remora/[tests]
+
+It is recommended that Remora be installed in a virtual environment.
+For example ``python3.8 -m venv --prompt remora --copies venv; source venv/bin/activate``.
+
+See help for any Remora sub-command with the ``-h`` flag.
+
+Getting Started
+---------------
+
+Remora models are trained to perform binary or categorical prediction of modified base content of a nanopore read.
+Models may also be trained to perform canonical base prediction, but this feature may be removed at a later time.
+The rest of the documentation will focus on the modified base detection task.
+
+The Remora training/prediction input unit (referred to as a chunk) consists of:
+
+1. Section of normalized signal
+2. Canonical bases attributed to the section of signal
+3. Mapping between these two
+
+Chunks have a fixed signal length defined at data preparation time and saved as a model attribute.
+A fixed position within the chunk is defined as the "focus position".
+By default, this position is the center of the "focus base" being interrogated by the model.
+
+Pre-trained Models
+------------------
+
+See the selection of current released models with ``remora model list_pretrained``.
+Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
+
+Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
+See Bonito documentation to apply Remora models.
+
+More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
+Note that older ONNX format models require Remora version < 2.0.
+
+Python API
+----------
+
+The Remora API can be applied to make modified base calls given a basecalled read via a ``RemoraRead`` object.
+
+* ``dacs`` (Data acquisition values) should be an int16 numpy array.
+* ``shift`` and ``scale`` are float values to convert dacs to mean=0 SD=1 scaling (or similar) for input to the Remora neural network.
+* ``str_seq`` is a string derived from ``sig`` (can be either basecalls or other downstream derived sequence; e.g. mapped reference positions).
+* ``seq_to_sig_map`` should be an int32 numpy array of length ``len(seq) + 1`` and elements should be indices within ``sig`` array assigned to each base in ``seq``.
+
+.. code-block:: python
+
+  from remora.model_util import load_model
+  from remora.data_chunks import RemoraRead
+  from remora.inference import call_read_mods
+
+  model, model_metadata = load_model("remora_train_results/model_best.pt")
+  read = RemoraRead(dacs, shift, scale, seq_to_sig_map, str_seq=seq)
+  mod_probs, _, pos = call_read_mods(
+    read,
+    model,
+    model_metadata,
+    return_mod_probs=True,
+  )
+
+``mod_probs`` will contain the probability of each modeled modified base as found in model_metadata["mod_long_names"].
+For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
+``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
+
+Data Preparation
+----------------
+
+Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
+Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
+
+The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
+Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
+
+K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
+
+.. code-block:: bash
+
+  remora \
+    dataset prepare \
+    can_reads.pod5 \
+    can_mappings.bam \
+    --output-remora-training-file can_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --motif CG 0 \
+    --mod-base-control
+  remora \
+    dataset prepare \
+    mod_reads.pod5 \
+    mod_mappings.bam \
+    --output-remora-training-file mod_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --motif CG 0 \
+    --mod-base m 5mC
+  remora \
+    dataset merge \
+    --input-dataset can_chunks.npz 10_000_000 \
+    --input-dataset mod_chunks.npz 10_000_000 \
+    --output-dataset chunks.npz
+
+The resulting ``chunks.npz`` file can then be used to train a Remora model.
+
+Model Training
+--------------
+
+Models are trained with the ``remora model train`` command.
+For example a model can be trained with the following command.
+
+.. code-block:: bash
+
+  remora \
+    model train \
+    chunks.npz \
+    --model remora/models/ConvLSTM_w_ref.py \
+    --device 0 \
+    --output-path train_results
+
+This command will produce a "best" model in torchscript format for use in Bonito, or ``remora infer`` commands.
+
+Model Inference
+---------------
+
+For testing purposes inference within Remora is provided.
+
+.. code-block:: bash
+
+  remora \
+    infer from_pod5_and_bam \
+    can_signal.pod5 \
+    can_basecalls.bam \
+    --model train_results/model_best.pt \
+    --out-file can_infer.bam \
+    --device 0
+  remora \
+    infer from_pod5_and_bam \
+    mod_signal.pod5 \
+    mod_basecalls.bam \
+    --model train_results/model_best.pt \
+    --out-file mod_infer.bam \
+    --device 0
+
+Finally, ``Remora`` provides tools to validate these results.
+Ground truth BED files references positions where each read should be called as the modified or canonical base listed in the BED name field.
+
+.. code-block:: bash
+
+  remora \
+    validate from_modbams \
+    --bam-and-bed can_infer.bam can_ground_truth.bed \
+    --bam-and-bed mod_infer.bam mod_ground_truth.bed \
+    --full-output-filename validation_results.txt
+
+Raw Signal Analysis
+-------------------
+
+As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
+The ``remora analyze`` command group contains the ``plot ref_region`` command.
+Additional commands will be added to this group to produce more useful raw signal analysis tasks.
+
+The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
+
+As an example using the test data, the following command produces the plot below.
+
+.. code-block:: bash
+
+  remora \
+    analyze plot ref_region \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
+    --ref-regions ref_regions.bed \
+    --highlight-ranges mod_gt.bed \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --log-filename log.txt
+
+.. image:: images/plot_ref_region_fwd.png
+   :width: 600
+   :alt: Plot reference region image (forward strand)
+
+.. image:: images/plot_ref_region_rev.png
+   :width: 600
+   :alt: Plot reference region image (reverse strand)
+
+Raw Signal Analysis
+-------------------
+
+The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
+This is API is primarily accessed via the ``remora.io.Read`` object.
+
+The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
+
+Terms and Licence
+-----------------
+
+This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
+Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
+Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
+Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
+Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
+
+© 2021 Oxford Nanopore Technologies Ltd.
+Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
+
+Research Release
+----------------
+
+Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
```

### Comparing `ont-remora-2.1.2/README.rst` & `ont-remora-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/setup.cfg` & `ont-remora-2.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/setup.py` & `ont-remora-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/ont_remora.egg-info/PKG-INFO` & `ont-remora-2.1.3/src/ont_remora.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,250 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.1.2
+Version: 2.1.3
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
-Description: .. image:: /ONT_logo.png
-          :width: 800
-          :alt: [Oxford Nanopore Technologies]
-          :target: https://nanoporetech.com/
-        
-        Remora
-        """"""
-        
-        Methylation/modified base calling separated from basecalling.
-        Remora primarily provides an API to call modified bases for basecaller programs such as Bonito.
-        Remora also provides the tools to prepare datasets, train modified base models and run simple inference.
-        
-        Installation
-        ------------
-        
-        Install from pypi:
-        
-        ::
-        
-           pip install ont-remora
-        
-        Install from github source for development:
-        
-        ::
-        
-           git clone git@github.com:nanoporetech/remora.git
-           pip install -e remora/[tests]
-        
-        It is recommended that Remora be installed in a virtual environment.
-        For example ``python3.8 -m venv --prompt remora --copies venv; source venv/bin/activate``.
-        
-        See help for any Remora sub-command with the ``-h`` flag.
-        
-        Getting Started
-        ---------------
-        
-        Remora models are trained to perform binary or categorical prediction of modified base content of a nanopore read.
-        Models may also be trained to perform canonical base prediction, but this feature may be removed at a later time.
-        The rest of the documentation will focus on the modified base detection task.
-        
-        The Remora training/prediction input unit (referred to as a chunk) consists of:
-        
-        1. Section of normalized signal
-        2. Canonical bases attributed to the section of signal
-        3. Mapping between these two
-        
-        Chunks have a fixed signal length defined at data preparation time and saved as a model attribute.
-        A fixed position within the chunk is defined as the "focus position".
-        By default, this position is the center of the "focus base" being interrogated by the model.
-        
-        Pre-trained Models
-        ------------------
-        
-        See the selection of current released models with ``remora model list_pretrained``.
-        Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
-        
-        Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
-        See Bonito documentation to apply Remora models.
-        
-        More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
-        Note that older ONNX format models require Remora version < 2.0.
-        
-        Python API
-        ----------
-        
-        The Remora API can be applied to make modified base calls given a basecalled read via a ``RemoraRead`` object.
-        
-        * ``dacs`` (Data acquisition values) should be an int16 numpy array.
-        * ``shift`` and ``scale`` are float values to convert dacs to mean=0 SD=1 scaling (or similar) for input to the Remora neural network.
-        * ``str_seq`` is a string derived from ``sig`` (can be either basecalls or other downstream derived sequence; e.g. mapped reference positions).
-        * ``seq_to_sig_map`` should be an int32 numpy array of length ``len(seq) + 1`` and elements should be indices within ``sig`` array assigned to each base in ``seq``.
-        
-        .. code-block:: python
-        
-          from remora.model_util import load_model
-          from remora.data_chunks import RemoraRead
-          from remora.inference import call_read_mods
-        
-          model, model_metadata = load_model("remora_train_results/model_best.pt")
-          read = RemoraRead(dacs, shift, scale, seq_to_sig_map, str_seq=seq)
-          mod_probs, _, pos = call_read_mods(
-            read,
-            model,
-            model_metadata,
-            return_mod_probs=True,
-          )
-        
-        ``mod_probs`` will contain the probability of each modeled modified base as found in model_metadata["mod_long_names"].
-        For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
-        ``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
-        
-        Data Preparation
-        ----------------
-        
-        Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
-        Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
-        
-        The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
-        Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
-        
-        K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
-        
-        .. code-block:: bash
-        
-          remora \
-            dataset prepare \
-            can_reads.pod5 \
-            can_mappings.bam \
-            --output-remora-training-file can_chunks.npz \
-            --log-filename prep_can.log \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --motif CG 0 \
-            --mod-base-control
-          remora \
-            dataset prepare \
-            mod_reads.pod5 \
-            mod_mappings.bam \
-            --output-remora-training-file mod_chunks.npz \
-            --log-filename prep_can.log \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --motif CG 0 \
-            --mod-base m 5mC
-          remora \
-            dataset merge \
-            --input-dataset can_chunks.npz 10_000_000 \
-            --input-dataset mod_chunks.npz 10_000_000 \
-            --output-dataset chunks.npz
-        
-        The resulting ``chunks.npz`` file can then be used to train a Remora model.
-        
-        Model Training
-        --------------
-        
-        Models are trained with the ``remora model train`` command.
-        For example a model can be trained with the following command.
-        
-        .. code-block:: bash
-        
-          remora \
-            model train \
-            chunks.npz \
-            --model remora/models/ConvLSTM_w_ref.py \
-            --device 0 \
-            --output-path train_results
-        
-        This command will produce a "best" model in torchscript format for use in Bonito, or ``remora infer`` commands.
-        
-        Model Inference
-        ---------------
-        
-        For testing purposes inference within Remora is provided.
-        
-        .. code-block:: bash
-        
-          remora \
-            infer from_pod5_and_bam \
-            can_signal.pod5 \
-            can_basecalls.bam \
-            --model train_results/model_best.pt \
-            --out-file can_infer.bam \
-            --device 0
-          remora \
-            infer from_pod5_and_bam \
-            mod_signal.pod5 \
-            mod_basecalls.bam \
-            --model train_results/model_best.pt \
-            --out-file mod_infer.bam \
-            --device 0
-        
-        Finally, ``Remora`` provides tools to validate these results.
-        Ground truth BED files references positions where each read should be called as the modified or canonical base listed in the BED name field.
-        
-        .. code-block:: bash
-        
-          remora \
-            validate from_modbams \
-            --bam-and-bed can_infer.bam can_ground_truth.bed \
-            --bam-and-bed mod_infer.bam mod_ground_truth.bed \
-            --full-output-filename validation_results.txt
-        
-        Raw Signal Analysis
-        -------------------
-        
-        As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
-        The ``remora analyze`` command group contains the ``plot ref_region`` command.
-        Additional commands will be added to this group to produce more useful raw signal analysis tasks.
-        
-        The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
-        
-        As an example using the test data, the following command produces the plot below.
-        
-        .. code-block:: bash
-        
-          remora \
-            analyze plot ref_region \
-            --pod5-and-bam can_reads.pod5 can_mappings.bam \
-            --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
-            --ref-regions ref_regions.bed \
-            --highlight-ranges mod_gt.bed \
-            --refine-kmer-level-table levels.txt \
-            --refine-rough-rescale \
-            --log-filename log.txt
-        
-        .. image:: images/plot_ref_region_fwd.png
-           :width: 600
-           :alt: Plot reference region image (forward strand)
-        
-        .. image:: images/plot_ref_region_rev.png
-           :width: 600
-           :alt: Plot reference region image (reverse strand)
-        
-        Raw Signal Analysis
-        -------------------
-        
-        The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
-        This is API is primarily accessed via the ``remora.io.Read`` object.
-        
-        The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
-        
-        Terms and Licence
-        -----------------
-        
-        This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
-        Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
-        Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
-        Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
-        Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
-        
-        © 2021 Oxford Nanopore Technologies Ltd.
-        Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
-        
-        Research Release
-        ----------------
-        
-        Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
 Provides-Extra: tests
+License-File: LICENSE.txt
+
+.. image:: /ONT_logo.png
+  :width: 800
+  :alt: [Oxford Nanopore Technologies]
+  :target: https://nanoporetech.com/
+
+Remora
+""""""
+
+Methylation/modified base calling separated from basecalling.
+Remora primarily provides an API to call modified bases for basecaller programs such as Bonito.
+Remora also provides the tools to prepare datasets, train modified base models and run simple inference.
+
+Installation
+------------
+
+Install from pypi:
+
+::
+
+   pip install ont-remora
+
+Install from github source for development:
+
+::
+
+   git clone git@github.com:nanoporetech/remora.git
+   pip install -e remora/[tests]
+
+It is recommended that Remora be installed in a virtual environment.
+For example ``python3.8 -m venv --prompt remora --copies venv; source venv/bin/activate``.
+
+See help for any Remora sub-command with the ``-h`` flag.
+
+Getting Started
+---------------
+
+Remora models are trained to perform binary or categorical prediction of modified base content of a nanopore read.
+Models may also be trained to perform canonical base prediction, but this feature may be removed at a later time.
+The rest of the documentation will focus on the modified base detection task.
+
+The Remora training/prediction input unit (referred to as a chunk) consists of:
+
+1. Section of normalized signal
+2. Canonical bases attributed to the section of signal
+3. Mapping between these two
+
+Chunks have a fixed signal length defined at data preparation time and saved as a model attribute.
+A fixed position within the chunk is defined as the "focus position".
+By default, this position is the center of the "focus base" being interrogated by the model.
+
+Pre-trained Models
+------------------
+
+See the selection of current released models with ``remora model list_pretrained``.
+Pre-trained models are stored remotely and can be downloaded using the ``remora model download`` command or will be downloaded on demand when needed.
+
+Models may be run from `Bonito <https://github.com/nanoporetech/bonito>`_.
+See Bonito documentation to apply Remora models.
+
+More advanced research models may be supplied via `Rerio <https://github.com/nanoporetech/rerio>`_.
+Note that older ONNX format models require Remora version < 2.0.
+
+Python API
+----------
+
+The Remora API can be applied to make modified base calls given a basecalled read via a ``RemoraRead`` object.
+
+* ``dacs`` (Data acquisition values) should be an int16 numpy array.
+* ``shift`` and ``scale`` are float values to convert dacs to mean=0 SD=1 scaling (or similar) for input to the Remora neural network.
+* ``str_seq`` is a string derived from ``sig`` (can be either basecalls or other downstream derived sequence; e.g. mapped reference positions).
+* ``seq_to_sig_map`` should be an int32 numpy array of length ``len(seq) + 1`` and elements should be indices within ``sig`` array assigned to each base in ``seq``.
+
+.. code-block:: python
+
+  from remora.model_util import load_model
+  from remora.data_chunks import RemoraRead
+  from remora.inference import call_read_mods
+
+  model, model_metadata = load_model("remora_train_results/model_best.pt")
+  read = RemoraRead(dacs, shift, scale, seq_to_sig_map, str_seq=seq)
+  mod_probs, _, pos = call_read_mods(
+    read,
+    model,
+    model_metadata,
+    return_mod_probs=True,
+  )
+
+``mod_probs`` will contain the probability of each modeled modified base as found in model_metadata["mod_long_names"].
+For example, run ``mod_probs.argmax(axis=1)`` to obtain the prediction for each input unit.
+``pos`` contains the position (index in input sequence) for each prediction within ``mod_probs``.
+
+Data Preparation
+----------------
+
+Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
+Note that the BAM file must contain the move table (default in Bonito and ``--emit-moves`` in Dorado) as well as the MD tag (default in Dorado with mapping and ``--MD`` argument for minimap2).
+
+The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
+Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
+
+K-mer tables for applicable conditions can be found in the `kmer_models repository <https://github.com/nanoporetech/kmer_models>`_.
+
+.. code-block:: bash
+
+  remora \
+    dataset prepare \
+    can_reads.pod5 \
+    can_mappings.bam \
+    --output-remora-training-file can_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --motif CG 0 \
+    --mod-base-control
+  remora \
+    dataset prepare \
+    mod_reads.pod5 \
+    mod_mappings.bam \
+    --output-remora-training-file mod_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --motif CG 0 \
+    --mod-base m 5mC
+  remora \
+    dataset merge \
+    --input-dataset can_chunks.npz 10_000_000 \
+    --input-dataset mod_chunks.npz 10_000_000 \
+    --output-dataset chunks.npz
+
+The resulting ``chunks.npz`` file can then be used to train a Remora model.
+
+Model Training
+--------------
+
+Models are trained with the ``remora model train`` command.
+For example a model can be trained with the following command.
+
+.. code-block:: bash
+
+  remora \
+    model train \
+    chunks.npz \
+    --model remora/models/ConvLSTM_w_ref.py \
+    --device 0 \
+    --output-path train_results
+
+This command will produce a "best" model in torchscript format for use in Bonito, or ``remora infer`` commands.
+
+Model Inference
+---------------
+
+For testing purposes inference within Remora is provided.
+
+.. code-block:: bash
+
+  remora \
+    infer from_pod5_and_bam \
+    can_signal.pod5 \
+    can_basecalls.bam \
+    --model train_results/model_best.pt \
+    --out-file can_infer.bam \
+    --device 0
+  remora \
+    infer from_pod5_and_bam \
+    mod_signal.pod5 \
+    mod_basecalls.bam \
+    --model train_results/model_best.pt \
+    --out-file mod_infer.bam \
+    --device 0
+
+Finally, ``Remora`` provides tools to validate these results.
+Ground truth BED files references positions where each read should be called as the modified or canonical base listed in the BED name field.
+
+.. code-block:: bash
+
+  remora \
+    validate from_modbams \
+    --bam-and-bed can_infer.bam can_ground_truth.bed \
+    --bam-and-bed mod_infer.bam mod_ground_truth.bed \
+    --full-output-filename validation_results.txt
+
+Raw Signal Analysis
+-------------------
+
+As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
+The ``remora analyze`` command group contains the ``plot ref_region`` command.
+Additional commands will be added to this group to produce more useful raw signal analysis tasks.
+
+The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
+
+As an example using the test data, the following command produces the plot below.
+
+.. code-block:: bash
+
+  remora \
+    analyze plot ref_region \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
+    --ref-regions ref_regions.bed \
+    --highlight-ranges mod_gt.bed \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --log-filename log.txt
+
+.. image:: images/plot_ref_region_fwd.png
+   :width: 600
+   :alt: Plot reference region image (forward strand)
+
+.. image:: images/plot_ref_region_rev.png
+   :width: 600
+   :alt: Plot reference region image (reverse strand)
+
+Raw Signal Analysis
+-------------------
+
+The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
+This is API is primarily accessed via the ``remora.io.Read`` object.
+
+The iPython notebooks (see ``notebooks`` directory) included in this repository exemplify some common analyses.
+
+Terms and Licence
+-----------------
+
+This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
+Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
+Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
+Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
+Research releases may be unstable and subject to rapid change by Oxford Nanopore Technologies.
+
+© 2021 Oxford Nanopore Technologies Ltd.
+Remora is distributed under the terms of the Oxford Nanopore Technologies' Public Licence.
+
+Research Release
+----------------
+
+Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools. Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests. However much as we would like to rectify every issue and piece of feedback users may have, the developers may have limited resource for support of this software. Research releases may be unstable and subject to rapid iteration by Oxford Nanopore Technologies.
```

### Comparing `ont-remora-2.1.2/src/ont_remora.egg-info/SOURCES.txt` & `ont-remora-2.1.3/src/ont_remora.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -27,8 +27,11 @@
 src/remora/parsers.py
 src/remora/prepare_train_data.py
 src/remora/refine_signal_map.py
 src/remora/refine_signal_map_core.pyx
 src/remora/train_model.py
 src/remora/util.py
 src/remora/validate.py
-src/remora/trained_models/readme.rst
+src/remora/trained_models/readme.rst
+tests/test_coding_standards.py
+tests/test_duplex.py
+tests/test_main.py
```

### Comparing `ont-remora-2.1.2/src/remora/constants.py` & `ont-remora-2.1.3/src/remora/constants.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/data_chunks.py` & `ont-remora-2.1.3/src/remora/data_chunks.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/download.py` & `ont-remora-2.1.3/src/remora/download.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/duplex_utils.py` & `ont-remora-2.1.3/src/remora/duplex_utils.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/encoded_kmers.pyx` & `ont-remora-2.1.3/src/remora/encoded_kmers.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/inference.py` & `ont-remora-2.1.3/src/remora/inference.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/io.py` & `ont-remora-2.1.3/src/remora/io.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/log.py` & `ont-remora-2.1.3/src/remora/log.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/main.py` & `ont-remora-2.1.3/src/remora/main.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/metrics.py` & `ont-remora-2.1.3/src/remora/metrics.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/model_util.py` & `ont-remora-2.1.3/src/remora/model_util.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/parsers.py` & `ont-remora-2.1.3/src/remora/parsers.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/prepare_train_data.py` & `ont-remora-2.1.3/src/remora/prepare_train_data.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/refine_signal_map.py` & `ont-remora-2.1.3/src/remora/refine_signal_map.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/refine_signal_map_core.pyx` & `ont-remora-2.1.3/src/remora/refine_signal_map_core.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 cdef inline int index_from_int_kmer(
     const int[::1] int_kmer,
     int kmer_len
 ):
     cdef int idx = 0
     cdef int kmer_pos
     for kmer_pos in range(kmer_len):
-        idx += int_kmer[kmer_len - kmer_pos - 1] * (4 ** kmer_pos)
+        idx += int_kmer[kmer_len - kmer_pos - 1] * <int>(4 ** kmer_pos)
     return idx
 
 
 def extract_levels(
     const int[::1] int_seq,
     const float[::1] int_kmer_levels,
     int kmer_len,
```

### Comparing `ont-remora-2.1.2/src/remora/train_model.py` & `ont-remora-2.1.3/src/remora/train_model.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/util.py` & `ont-remora-2.1.3/src/remora/util.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.1.2/src/remora/validate.py` & `ont-remora-2.1.3/src/remora/validate.py`

 * *Files identical despite different names*

