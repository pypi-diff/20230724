# Comparing `tmp/returnn-1.20230719.125702.tar.gz` & `tmp/returnn-1.20230724.124015.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230719.125702.tar", last modified: Wed Jul 19 11:10:25 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230724.124015.tar", last modified: Mon Jul 24 11:06:51 2023, max compression
```

## Comparing `returnn-1.20230719.125702.tar` & `returnn-1.20230724.124015.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 11:09:58.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-19 11:10:00.000000 returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   101797 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157965 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   545666 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73572 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:10:25.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-19 11:09:57.000000 returnn-1.20230719.125702/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-24 11:06:36.000000 returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101797 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157965 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   545666 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37521 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73572 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:06:51.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-24 11:06:33.000000 returnn-1.20230724.124015/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230719.125702/.gitignore` & `returnn-1.20230724.124015/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/.gitmodules` & `returnn-1.20230724.124015/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/CHANGELOG.md` & `returnn-1.20230724.124015/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/CODEOWNERS` & `returnn-1.20230724.124015/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/CONTRIBUTING.md` & `returnn-1.20230724.124015/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/LICENSE` & `returnn-1.20230724.124015/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/MANIFEST.in` & `returnn-1.20230724.124015/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/PKG-INFO` & `returnn-1.20230724.124015/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230719.125702
+Version: 1.20230724.124015
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230719.125702/README.rst` & `returnn-1.20230724.124015/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/__init__.py` & `returnn-1.20230724.124015/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/12AX.cluster_map` & `returnn-1.20230724.124015/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-fwd.config` & `returnn-1.20230724.124015/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-horovod-mpi.py` & `returnn-1.20230724.124015/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230724.124015/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-hyper-param-tuning.config` & `returnn-1.20230724.124015/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-iter-dataset.py` & `returnn-1.20230724.124015/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-list-devices.py` & `returnn-1.20230724.124015/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-lua-torch-layer.config` & `returnn-1.20230724.124015/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230724.124015/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-returnn-as-framework.py` & `returnn-1.20230724.124015/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-rf.config` & `returnn-1.20230724.124015/demos/demo-rf.config`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 dev = {"class": "Task12AXDataset", "num_seqs": 100, "fixed_random_seed": 1}
 
 time_dim = Dim(None, name="time")
 in_dim = Dim(9, name="in")
 out_dim = Dim(2, name="out")
 extern_data = {
     "data": {"dims": (batch_dim, time_dim, in_dim), "dtype": "float32"},
-    "classes": {"dims": (batch_dim, time_dim), "sparse_dim": out_dim, "dtype": "int32"},
+    "classes": {"dims": (batch_dim, time_dim), "sparse_dim": out_dim, "dtype": "int32", "available_for_inference": False},
 }
 model_outputs = {
     "output": {"dims": (batch_dim, time_dim, out_dim), "dtype": "float32"},
 }
 
 batching = "random"
 batch_size = 5000
```

### Comparing `returnn-1.20230719.125702/demos/demo-rhn-enwik8.config` & `returnn-1.20230724.124015/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-sprint-interface.py` & `returnn-1.20230724.124015/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-att-copy.config` & `returnn-1.20230724.124015/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-attention.config` & `returnn-1.20230724.124015/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-enc-dec.config` & `returnn-1.20230724.124015/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230724.124015/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230724.124015/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230724.124015/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230724.124015/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230724.124015/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-rec-self-att.config` & `returnn-1.20230724.124015/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230724.124015/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230724.124015/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo-torch.config` & `returnn-1.20230724.124015/demos/demo-torch.config`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 train = {"class": "Task12AXDataset", "num_seqs": 1000}
 dev = {"class": "Task12AXDataset", "num_seqs": 100, "fixed_random_seed": 1}
 
 num_inputs = 9
 num_outputs = 2
 extern_data = {
     "data": {"dim": num_inputs},
-    "classes": {"dim": num_outputs, "sparse": True},
+    "classes": {"dim": num_outputs, "sparse": True, "available_for_inference": False},
 }
 model_outputs = {
     "output": {"dim": num_outputs},
 }
 
 batching = "random"
 batch_size = 5000
@@ -60,14 +60,15 @@
 
 def forward_step(*, model: Model, extern_data: TensorDict):
     """
     Function used in inference.
     """
     data = extern_data["data"]
     out = model(data.raw_tensor)
+    rf.get_run_ctx().expected_outputs["output"].dims[1].dyn_size_ext.raw_tensor = data.dims[1].dyn_size_ext.raw_tensor
     rf.get_run_ctx().mark_as_default_output(tensor=out)
 
 
 def train_step(*, model: Model, extern_data: TensorDict, **_kwargs):
     """
     Function used in training/dev.
     """
```

### Comparing `returnn-1.20230719.125702/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230724.124015/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/demo.sh` & `returnn-1.20230724.124015/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230724.124015/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/README.txt` & `returnn-1.20230724.124015/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/config_demo` & `returnn-1.20230724.124015/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230724.124015/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/config_real` & `returnn-1.20230724.124015/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230724.124015/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/decode.py` & `returnn-1.20230724.124015/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230724.124015/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230724.124015/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230724.124015/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230724.124015/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230724.124015/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230724.124015/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230724.124015/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230724.124015/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/__init__.py` & `returnn-1.20230724.124015/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/__main__.py` & `returnn-1.20230724.124015/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/__old_mod_loader__.py` & `returnn-1.20230724.124015/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/__setup__.py` & `returnn-1.20230724.124015/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/config.py` & `returnn-1.20230724.124015/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/audio.py` & `returnn-1.20230724.124015/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/basic.py` & `returnn-1.20230724.124015/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/bundle_file.py` & `returnn-1.20230724.124015/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/cached.py` & `returnn-1.20230724.124015/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/cached2.py` & `returnn-1.20230724.124015/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/generating.py` & `returnn-1.20230724.124015/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/hdf.py` & `returnn-1.20230724.124015/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/lm.py` & `returnn-1.20230724.124015/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/map.py` & `returnn-1.20230724.124015/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/meta.py` & `returnn-1.20230724.124015/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/multi_proc.py` & `returnn-1.20230724.124015/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/normalization_data.py` & `returnn-1.20230724.124015/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/numpy_dump.py` & `returnn-1.20230724.124015/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/raw_wav.py` & `returnn-1.20230724.124015/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/sprint.py` & `returnn-1.20230724.124015/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/stereo.py` & `returnn-1.20230724.124015/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230724.124015/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/datasets/util/vocabulary.py` & `returnn-1.20230724.124015/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/engine/base.py` & `returnn-1.20230724.124015/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/engine/batch.py` & `returnn-1.20230724.124015/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230724.124015/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/edit.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/select.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/transform.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/extern/graph_editor/util.py` & `returnn-1.20230724.124015/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/forward_iface.py` & `returnn-1.20230724.124015/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/__init__.py` & `returnn-1.20230724.124015/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/_backend.py` & `returnn-1.20230724.124015/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/_numpy_backend.py` & `returnn-1.20230724.124015/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/_utils.py` & `returnn-1.20230724.124015/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/array_.py` & `returnn-1.20230724.124015/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/attention.py` & `returnn-1.20230724.124015/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/cond.py` & `returnn-1.20230724.124015/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/const.py` & `returnn-1.20230724.124015/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/container.py` & `returnn-1.20230724.124015/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/conv.py` & `returnn-1.20230724.124015/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/device.py` & `returnn-1.20230724.124015/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/dims.py` & `returnn-1.20230724.124015/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/dropout.py` & `returnn-1.20230724.124015/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/dtype.py` & `returnn-1.20230724.124015/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/encoder/base.py` & `returnn-1.20230724.124015/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/encoder/conformer.py` & `returnn-1.20230724.124015/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/init.py` & `returnn-1.20230724.124015/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/linear.py` & `returnn-1.20230724.124015/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/loop.py` & `returnn-1.20230724.124015/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/loss.py` & `returnn-1.20230724.124015/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/math_.py` & `returnn-1.20230724.124015/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/matmul.py` & `returnn-1.20230724.124015/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/module.py` & `returnn-1.20230724.124015/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/normalization.py` & `returnn-1.20230724.124015/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/parameter.py` & `returnn-1.20230724.124015/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/rand.py` & `returnn-1.20230724.124015/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/rec.py` & `returnn-1.20230724.124015/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/reduce.py` & `returnn-1.20230724.124015/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/run_ctx.py` & `returnn-1.20230724.124015/returnn/frontend/run_ctx.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 We can either be in param-init stage,
 or in the main training loop,
 or forwarding loop.
 """
 
 from __future__ import annotations
 from typing import Optional, Union, Any, Sequence, Dict
-import logging
 from dataclasses import dataclass
 from returnn.tensor import Tensor, Dim, TensorDict
 import returnn.frontend as rf
 from . import _backend
 
 
 __all__ = ["RunCtx", "Loss", "get_run_ctx", "init_train_step_run_ctx", "init_forward_step_run_ctx"]
@@ -396,20 +395,14 @@
     # In this case, it is common that the user does not explicitly specify the dyn sizes of the dim tags.
     # We accept this, but for ONNX export and maybe other cases,
     # we automatically fill in the dyn sizes from the raw tensor.
     # In case the dim tag has scalar size, this is non-ambiguous,
     # however, otherwise, it is ambiguous, so we print a warning that we always use the highest dim size.
     for axis, dim in enumerate(tensor.dims):
         if dim.dyn_size_ext and dim.dyn_size_ext.raw_tensor is None:
-            dim_value_raw = _backend.global_backend.get_shape_tuple_raw(raw_tensor)[axis]
-            dim_value = rf.convert_to_tensor(dim_value_raw, dims=())
-            dim_value = rf.cast(dim_value, dtype=dim.dyn_size_ext.dtype)
+            # Only non-scalar dyn sizes matter.
             if dim.dyn_size_ext.dims:
-                dyn_size = rf.full(dims=dim.dyn_size_ext.dims, fill_value=dim_value)
-                logging.warning(
+                raise Exception(
                     f"Output {name!r} {tensor}: Cannot infer dynamic size for dim {dim}. "
-                    f"Using {dyn_size} as fallback."
+                    f"You must explicitly specify the dyn size by assigning `{dim}.dyn_size_ext.raw_tensor = ...`."
                 )
-            else:
-                dyn_size = dim_value
-            dim.dyn_size_ext.raw_tensor = dyn_size.raw_tensor
     return tensor
```

### Comparing `returnn-1.20230719.125702/returnn/frontend/signal.py` & `returnn-1.20230724.124015/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/state.py` & `returnn-1.20230724.124015/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/tensor_array.py` & `returnn-1.20230724.124015/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/frontend/types.py` & `returnn-1.20230724.124015/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/import_/common.py` & `returnn-1.20230724.124015/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/import_/git.py` & `returnn-1.20230724.124015/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/import_/import_.py` & `returnn-1.20230724.124015/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/learning_rate_control.py` & `returnn-1.20230724.124015/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/log.py` & `returnn-1.20230724.124015/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/native_op.cpp` & `returnn-1.20230724.124015/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/native_op.py` & `returnn-1.20230724.124015/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/pretrain.py` & `returnn-1.20230724.124015/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/sprint/cache.py` & `returnn-1.20230724.124015/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/sprint/control.py` & `returnn-1.20230724.124015/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/sprint/error_signals.py` & `returnn-1.20230724.124015/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/sprint/extern_interface.py` & `returnn-1.20230724.124015/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/sprint/interface.py` & `returnn-1.20230724.124015/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/_dim_extra.py` & `returnn-1.20230724.124015/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/_tensor_extra.py` & `returnn-1.20230724.124015/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230724.124015/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230724.124015/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230724.124015/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/dim.py` & `returnn-1.20230724.124015/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/marked_dim.py` & `returnn-1.20230724.124015/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/tensor.py` & `returnn-1.20230724.124015/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tensor/tensor_dict.py` & `returnn-1.20230724.124015/returnn/tensor/tensor_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,68 +71,95 @@
             dim.reset_eager()
 
     def copy_template(self) -> TensorDict:
         """copy template"""
         return TensorDict({k: v.copy_template() for k, v in self.data.items()})
 
     def as_raw_tensor_dict(
-        self, *, include_const_sizes: bool = False, expected_type: Union[Type, Sequence[Type]] = object
+        self,
+        *,
+        include_const_sizes: bool = False,
+        include_scalar_dyn_sizes: bool = True,
+        exclude_duplicate_dims: bool = False,
+        expected_value_type: Union[Type, Sequence[Type]] = object,
     ) -> Dict[str, Any]:
         """
         :return: dict of raw tensors, including any sequence lengths / dynamic sizes
         """
+        assert not (include_const_sizes and not include_scalar_dyn_sizes)
+        visited_dims = set()
         out = {}
         for key, value in self.data.items():
             assert key not in out
             assert isinstance(
-                value.raw_tensor, expected_type
-            ), f"key {key} {value}: unexpected {type(value.raw_tensor)}, expected {expected_type}"
+                value.raw_tensor, expected_value_type
+            ), f"key {key} {value}: unexpected {type(value.raw_tensor)}, expected {expected_value_type}"
             out[key] = value.raw_tensor
             for i, dim in enumerate(value.dims):
+                if exclude_duplicate_dims and dim in visited_dims:
+                    continue
                 key_ = f"{key}:size{i}"
                 assert key_ not in out
                 if dim.is_batch_dim() and (not dim.dyn_size_ext or dim.dyn_size_ext.raw_tensor is None):
-                    dim_value = dim.get_dim_value()
-                    assert isinstance(
-                        dim_value, expected_type
-                    ), f"key {key_} {dim}: unexpected {type(dim_value)}, expected {expected_type}"
-                    out[key_] = dim_value
+                    if include_scalar_dyn_sizes:
+                        dim_value = dim.get_dim_value()
+                        assert isinstance(
+                            dim_value, expected_value_type
+                        ), f"key {key_} {dim}: unexpected {type(dim_value)}, expected {expected_value_type}"
+                        out[key_] = dim_value
                 elif dim.dyn_size_ext:
-                    assert isinstance(dim.dyn_size_ext.raw_tensor, expected_type), (
-                        f"key {key_} {dim} {dim.dyn_size_ext}:"
-                        f" unexpected {type(dim.dyn_size_ext.raw_tensor)}, expected {expected_type}"
-                    )
-                    out[key_] = dim.dyn_size_ext.raw_tensor
+                    if include_scalar_dyn_sizes or dim.dyn_size_ext.dims:
+                        assert isinstance(dim.dyn_size_ext.raw_tensor, expected_value_type), (
+                            f"key {key_} {dim} {dim.dyn_size_ext}:"
+                            f" unexpected {type(dim.dyn_size_ext.raw_tensor)}, expected {expected_value_type}"
+                        )
+                        out[key_] = dim.dyn_size_ext.raw_tensor
                 elif dim.size is not None:
-                    if include_const_sizes:
+                    if include_scalar_dyn_sizes and include_const_sizes:
                         assert isinstance(
-                            dim.size, expected_type
-                        ), f"key {key_} {dim}: unexpected {type(dim.size)}, expected {expected_type}"
+                            dim.size, expected_value_type
+                        ), f"key {key_} {dim}: unexpected {type(dim.size)}, expected {expected_value_type}"
                         out[key_] = dim.size
                 else:
                     raise Exception(f"cannot handle dim: {dim}")
+                visited_dims.add(dim)
         return out
 
-    def assign_from_raw_tensor_dict_(self, raw_tensor_dict: Dict[str, Any]):
+    def assign_from_raw_tensor_dict_(
+        self,
+        raw_tensor_dict: Dict[str, Any],
+        *,
+        with_scalar_dyn_sizes: bool = True,
+        duplicate_dims_are_excluded: bool = False,
+    ):
         """
         :param raw_tensor_dict: dict of raw tensors, including any sequence lengths / dynamic sizes
+        :param with_scalar_dyn_sizes: `include_scalar_dyn_sizes` was used in :func:`as_raw_tensor_dict`
+        :param duplicate_dims_are_excluded: `exclude_duplicate_dims` was used in :func:`as_raw_tensor_dict`
         """
+        visited_dims = set()
         for key, value in self.data.items():
             assert key in raw_tensor_dict
             value.raw_tensor = raw_tensor_dict[key]
             for i, dim in enumerate(value.dims):
+                if duplicate_dims_are_excluded and dim in visited_dims:
+                    continue
                 key_ = f"{key}:size{i}"
                 if dim.is_batch_dim() and not dim.dyn_size_ext:
                     dim.dyn_size_ext = Tensor("batch", [], dtype="int32")
                 if dim.dyn_size_ext:
-                    assert key_ in raw_tensor_dict
-                    dim.dyn_size_ext.raw_tensor = raw_tensor_dict[key_]
+                    if not with_scalar_dyn_sizes and not dim.dyn_size_ext.dims:
+                        pass
+                    else:
+                        assert key_ in raw_tensor_dict, f"keys: f{raw_tensor_dict.keys()}"
+                        dim.dyn_size_ext.raw_tensor = raw_tensor_dict[key_]
                 else:
                     if key_ in raw_tensor_dict:
                         assert dim.size == raw_tensor_dict[key_]
+                visited_dims.add(dim)
 
 
 def _convert_to_tensor(opts: _TensorT, *, name: Optional[str] = None) -> Tensor:
     """
     :param opts:
     """
     if isinstance(opts, Tensor):
```

### Comparing `returnn-1.20230719.125702/returnn/tensor/utils.py` & `returnn-1.20230724.124015/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/compat.py` & `returnn-1.20230724.124015/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/data_pipeline.py` & `returnn-1.20230724.124015/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/distributed.py` & `returnn-1.20230724.124015/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/engine.py` & `returnn-1.20230724.124015/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230724.124015/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230724.124015/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/horovod.py` & `returnn-1.20230724.124015/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230724.124015/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/base.py` & `returnn-1.20230724.124015/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/basic.py` & `returnn-1.20230724.124015/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/rec.py` & `returnn-1.20230724.124015/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/segmental_model.py` & `returnn-1.20230724.124015/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/signal_processing.py` & `returnn-1.20230724.124015/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/layers/variable.py` & `returnn-1.20230724.124015/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/native_op.py` & `returnn-1.20230724.124015/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/network.py` & `returnn-1.20230724.124015/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/sprint.py` & `returnn-1.20230724.124015/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/updater.py` & `returnn-1.20230724.124015/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/util/basic.py` & `returnn-1.20230724.124015/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/util/data.py` & `returnn-1.20230724.124015/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230724.124015/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/util/ken_lm.py` & `returnn-1.20230724.124015/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/tf/util/open_fst.py` & `returnn-1.20230724.124015/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/data/pipeline.py` & `returnn-1.20230724.124015/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230724.124015/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/data/tensor_utils.py` & `returnn-1.20230724.124015/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/distributed.py` & `returnn-1.20230724.124015/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/engine.py` & `returnn-1.20230724.124015/returnn/torch/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,14 +529,16 @@
             self._pt_model = rf_module_to_pt_module(model)
         elif isinstance(model, torch.nn.Module):
             self._pt_model = model
         else:
             raise TypeError(f"get_model returned {model} of type {type(model)}, expected rf.Module or torch.nn.Module")
         assert isinstance(self._pt_model, torch.nn.Module)
         print("Model:", self._pt_model, file=log.v4)
+        num_params = sum([parameter.numel() for parameter in self._pt_model.parameters()])
+        print(f"net params #: {num_params}", file=log.v2)
 
         if checkpoint_state is not None:
             self._pt_model.load_state_dict(checkpoint_state["model"])
         preload_from_files = self.config.typed_value("preload_from_files", {})
         if preload_from_files:
             # see `preload_from_files` in tf engine and `returnn.tf.network.CustomCheckpointLoader`
             # We use the reversed sorted order here to achieve consistent behavior with the TF engine.
```

### Comparing `returnn-1.20230719.125702/returnn/torch/frontend/_backend.py` & `returnn-1.20230724.124015/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/frontend/_rand.py` & `returnn-1.20230724.124015/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/frontend/bridge.py` & `returnn-1.20230724.124015/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/torch/updater.py` & `returnn-1.20230724.124015/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/basic.py` & `returnn-1.20230724.124015/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/better_exchook.py` & `returnn-1.20230724.124015/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/bpe.py` & `returnn-1.20230724.124015/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/debug.py` & `returnn-1.20230724.124015/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/debug_helpers.py` & `returnn-1.20230724.124015/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/fsa.py` & `returnn-1.20230724.124015/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230724.124015/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/pprint.py` & `returnn-1.20230724.124015/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/py-to-pickle.cpp` & `returnn-1.20230724.124015/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/sig_proc.py` & `returnn-1.20230724.124015/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn/util/task_system.py` & `returnn-1.20230724.124015/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/returnn.egg-info/PKG-INFO` & `returnn-1.20230724.124015/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230719.125702
+Version: 1.20230724.124015
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230719.125702/returnn.egg-info/SOURCES.txt` & `returnn-1.20230724.124015/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/setup.py` & `returnn-1.20230724.124015/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/DummySprintExec.py` & `returnn-1.20230724.124015/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230724.124015/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230724.124015/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230724.124015/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/_set_num_threads1.py` & `returnn-1.20230724.124015/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/_setup_test_env.py` & `returnn-1.20230724.124015/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/bpe-unicode-demo.codes` & `returnn-1.20230724.124015/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/bpe-unicode-demo.vocab` & `returnn-1.20230724.124015/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/lexicon_opt.isyms` & `returnn-1.20230724.124015/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/lexicon_opt.jpg` & `returnn-1.20230724.124015/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/lint_common.py` & `returnn-1.20230724.124015/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/pycharm-inspect.py` & `returnn-1.20230724.124015/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/pylint.py` & `returnn-1.20230724.124015/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/returnn-as-framework.py` & `returnn-1.20230724.124015/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/rf_utils.py` & `returnn-1.20230724.124015/tests/rf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         v_tf = out_tf_raw[k]
         numpy.testing.assert_allclose(v_pt, v_tf, atol=1e-5, rtol=1e-5, err_msg=f"output {k!r} differs")
     return out_pt
 
 
 def run_model_torch(extern_data: TensorDict, get_model: rf.GetModelFunc, forward_step: rf.StepFunc) -> TensorDict:
     """run"""
-    extern_data_raw = extern_data.as_raw_tensor_dict(expected_type=numpy.ndarray)
+    extern_data_raw = extern_data.as_raw_tensor_dict(expected_value_type=numpy.ndarray)
     rf.select_backend_torch()
     rf.set_random_seed(42)
 
     # Inplace replace Numpy by Torch.
     # Inplace because dim tags cannot easily be copied (then they are not the same).
     # We recover extern_data in the end.
     tensor_dict_numpy_to_torch_(extern_data)
@@ -107,15 +107,15 @@
 
     extern_data.assign_from_raw_tensor_dict_(extern_data_raw)
     return outputs
 
 
 def run_model_net_dict_tf(extern_data: TensorDict, get_model: rf.GetModelFunc, forward_step: rf.StepFunc) -> TensorDict:
     """run"""
-    extern_data_raw = extern_data.as_raw_tensor_dict(expected_type=numpy.ndarray)
+    extern_data_raw = extern_data.as_raw_tensor_dict(expected_value_type=numpy.ndarray)
     extern_data.reset_content()
     rf.select_backend_returnn_layers_tf()
     rf.set_random_seed(42)
 
     from returnn.tf.frontend_layers.config_entry_points import get_net_dict
 
     config = Config(
@@ -155,17 +155,17 @@
         for k, v in outputs_layers.data.items():
             v: Tensor[rfl.Layer]
             assert isinstance(v.raw_tensor, rfl.Layer)
             layer_name = v.raw_tensor.get_abs_name()
             layer = net.get_layer(layer_name)
             outputs_tf.data[k] = layer.output.copy()
 
-        fetches = outputs_tf.as_raw_tensor_dict(expected_type=tf.Tensor)
+        fetches = outputs_tf.as_raw_tensor_dict(expected_value_type=tf.Tensor)
         assert set(extern_data.data.keys()) == set(net.extern_data.data.keys())
-        extern_data_tf_placeholders = net.extern_data.as_raw_tensor_dict(expected_type=tf.Tensor)
+        extern_data_tf_placeholders = net.extern_data.as_raw_tensor_dict(expected_value_type=tf.Tensor)
         assert set(extern_data_tf_placeholders.keys()) == set(extern_data_raw.keys())
         feed_dict = {extern_data_tf_placeholders[k]: v for k, v in extern_data_raw.items()}
 
         outputs_numpy_raw = session.run(fetches, feed_dict=feed_dict)
 
         # Scalars are not Numpy arrays, but our code below assumes that we only have Numpy arrays.
         # So we convert them here.
```

### Comparing `returnn-1.20230719.125702/tests/spelling.dic` & `returnn-1.20230724.124015/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Config.py` & `returnn-1.20230724.124015/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Dataset.py` & `returnn-1.20230724.124015/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Fsa.py` & `returnn-1.20230724.124015/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_GeneratingDataset.py` & `returnn-1.20230724.124015/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_HDFDataset.py` & `returnn-1.20230724.124015/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_LearningRateControl.py` & `returnn-1.20230724.124015/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Log.py` & `returnn-1.20230724.124015/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_MultiProcDataset.py` & `returnn-1.20230724.124015/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_PTDataset.py` & `returnn-1.20230724.124015/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Pretrain.py` & `returnn-1.20230724.124015/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_ResNet.py` & `returnn-1.20230724.124015/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_SprintDataset.py` & `returnn-1.20230724.124015/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_SprintInterface.py` & `returnn-1.20230724.124015/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFEngine.py` & `returnn-1.20230724.124015/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFNativeOp.py` & `returnn-1.20230724.124015/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFNetworkLayer.py` & `returnn-1.20230724.124015/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230724.124015/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230724.124015/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFUpdater.py` & `returnn-1.20230724.124015/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TFUtil.py` & `returnn-1.20230724.124015/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TF_determinism.py` & `returnn-1.20230724.124015/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TaskSystem.py` & `returnn-1.20230724.124015/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230724.124015/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_TranslationDataset.py` & `returnn-1.20230724.124015/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_Util.py` & `returnn-1.20230724.124015/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_demos.py` & `returnn-1.20230724.124015/tests/test_demos.py`

 * *Files 15% similar despite different names*

```diff
@@ -145,33 +145,93 @@
     cleanup_tmp_models("demos/demo-torch.config")
     out = run(py, "rnn.py", "demos/demo-torch.config", print_stdout=True)
     # Also see test_demo_tf_task12ax above.
     fer = parse_last_fer(out)
     assert_less(fer, 0.02)
 
 
-def _test_torch_export_to_onnx(cfg_filename: str):
+def _test_torch_export_to_onnx(cfg_filename: str) -> str:
+    """
+    Executes the demo passed as a parameter and returns the ONNX exported model as a filename.
+
+    :param cfg_filename: Demo filename, either "demos/demo-rf.config" or "demos/demo-torch.config".
+    :return: Filename representing the ONNX model location.
+    """
     cleanup_tmp_models(cfg_filename)
     out = run(py, "rnn.py", cfg_filename, "--num_epochs", "1", "--device", "cpu")
     out_pt_model = re.search(r"\nSave model under (.*)\n", out, re.MULTILINE)
     assert out_pt_model, "Could not find the model filename in the output:\n%s" % out
     out_pt_model = out_pt_model.group(1)
     print("*** PT model:", out_pt_model)
     out_onnx_model = out_pt_model.replace(".pt", ".onnx")
     run(py, "tools/torch_export_to_onnx.py", cfg_filename, out_pt_model, out_onnx_model, print_stdout=True)
 
+    return out_onnx_model
+
+
+def _test_torch_onnx_inference_no_seq_lens(out_onnx_model: str):
+    """
+    Tests the inference of the torch demo with an ONNX model passed as parameter.
+    """
+    import onnxruntime as ort
+
+    torch.manual_seed(42)
+    # Set arbitrary values to pass to the model, respecting the input size (9).
+    dummy_data = torch.randn([3, 50, 9])
+
+    session = ort.InferenceSession(out_onnx_model)
+    outputs_onnx = session.run(
+        None,
+        {
+            "data": dummy_data.numpy(),
+        },
+    )
+    print("*** Result:", torch.FloatTensor(outputs_onnx[0]))
+    print("*** Batch size:", torch.IntTensor(outputs_onnx[1]))
+    print("*** Sequence lengths:", torch.IntTensor(outputs_onnx[2]))
+
+
+def _test_torch_onnx_inference_seq_lens_in_out(out_onnx_model: str):
+    """
+    Tests the inference of the torch demo with an ONNX model passed as parameter.
+    """
+    print(out_onnx_model)
+    import onnxruntime as ort
+
+    torch.manual_seed(42)
+    # Set arbitrary values to pass to the model, respecting the input size (9).
+    dummy_data = torch.randn([3, 50, 9])
+    dummy_seq_lens = torch.tensor([27, 50, 43], dtype=torch.int32)
+
+    session = ort.InferenceSession(out_onnx_model)
+    outputs_onnx = session.run(
+        None,
+        {
+            "data": dummy_data.numpy(),
+            "data:size1": dummy_seq_lens.numpy(),
+        },
+    )
+    out_result = torch.FloatTensor(outputs_onnx[0])
+    out_seq_lens = torch.IntTensor(outputs_onnx[1])
+    print("*** Result:", out_result)
+    print("*** Sequence lengths:", out_seq_lens)
+
+    assert out_result.shape == torch.Size([3, 50, 2])
+
 
 @unittest.skipIf(not torch, "no PyTorch")
 def test_demo_torch_export_to_onnx():
-    _test_torch_export_to_onnx("demos/demo-torch.config")
+    out_onnx_model = _test_torch_export_to_onnx("demos/demo-torch.config")
+    _test_torch_onnx_inference_seq_lens_in_out(out_onnx_model)
 
 
 @unittest.skipIf(not torch, "no PyTorch")
-def test_demo_rf_torch_export_to_onnx():
-    _test_torch_export_to_onnx("demos/demo-rf.config")
+def test_demo_rf_export_to_onnx():
+    out_onnx_model = _test_torch_export_to_onnx("demos/demo-rf.config")
+    _test_torch_onnx_inference_seq_lens_in_out(out_onnx_model)
 
 
 @unittest.skipIf(not torch, "no PyTorch")
 def test_demo_rf_torch_task12ax():
     cleanup_tmp_models("demos/demo-rf.config")
     out = run(py, "rnn.py", "demos/demo-rf.config", print_stdout=True)
     # Also see test_demo_tf_task12ax above.
```

### Comparing `returnn-1.20230719.125702/tests/test_fork_exec.py` & `returnn-1.20230724.124015/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_hdf_dump.py` & `returnn-1.20230724.124015/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_array.py` & `returnn-1.20230724.124015/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_attention.py` & `returnn-1.20230724.124015/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_base.py` & `returnn-1.20230724.124015/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_cond.py` & `returnn-1.20230724.124015/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_const.py` & `returnn-1.20230724.124015/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_container.py` & `returnn-1.20230724.124015/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_conv.py` & `returnn-1.20230724.124015/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_encoder_conformer.py` & `returnn-1.20230724.124015/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_loop.py` & `returnn-1.20230724.124015/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_math.py` & `returnn-1.20230724.124015/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_normalization.py` & `returnn-1.20230724.124015/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_rec.py` & `returnn-1.20230724.124015/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_reduce.py` & `returnn-1.20230724.124015/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_rf_signal.py` & `returnn-1.20230724.124015/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_tensor.py` & `returnn-1.20230724.124015/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_tools.py` & `returnn-1.20230724.124015/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_torch_engine.py` & `returnn-1.20230724.124015/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_torch_frontend.py` & `returnn-1.20230724.124015/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tests/test_torch_internal_frontend.py` & `returnn-1.20230724.124015/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/analyze-dataset-batches.py` & `returnn-1.20230724.124015/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/bliss-collect-seq-lens.py` & `returnn-1.20230724.124015/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/bliss-dump-text.py` & `returnn-1.20230724.124015/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/bliss-get-segment-names.py` & `returnn-1.20230724.124015/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/bliss-to-ogg-zip.py` & `returnn-1.20230724.124015/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/bpe-create-lexicon.py` & `returnn-1.20230724.124015/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/calculate-word-error-rate.py` & `returnn-1.20230724.124015/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/cleanup-old-models.py` & `returnn-1.20230724.124015/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/collect-orth-symbols.py` & `returnn-1.20230724.124015/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/collect-words.py` & `returnn-1.20230724.124015/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/compile_native_op.py` & `returnn-1.20230724.124015/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/compile_tf_graph.py` & `returnn-1.20230724.124015/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/debug-dump-search-scores.py` & `returnn-1.20230724.124015/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/debug-plot-search-scores.py` & `returnn-1.20230724.124015/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-dataset-raw-strings.py` & `returnn-1.20230724.124015/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-dataset.py` & `returnn-1.20230724.124015/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-forward-stats.py` & `returnn-1.20230724.124015/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-forward.py` & `returnn-1.20230724.124015/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-network-json.py` & `returnn-1.20230724.124015/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/dump-pickle.py` & `returnn-1.20230724.124015/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230724.124015/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/get-attention-weights.py` & `returnn-1.20230724.124015/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/get-best-model-epoch.py` & `returnn-1.20230724.124015/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/hdf_dump.py` & `returnn-1.20230724.124015/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230724.124015/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/import-blocks-mt-model.py` & `returnn-1.20230724.124015/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/import-t2t-mt-model.py` & `returnn-1.20230724.124015/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/Makefile` & `returnn-1.20230724.124015/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/README.md` & `returnn-1.20230724.124015/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/example/README.md` & `returnn-1.20230724.124015/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230724.124015/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230724.124015/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230724.124015/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/file.h` & `returnn-1.20230724.124015/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230724.124015/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230724.124015/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/main.cc` & `returnn-1.20230724.124015/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230724.124015/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230724.124015/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230724.124015/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/tf_avg_checkpoints.py` & `returnn-1.20230724.124015/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/tf_inspect_checkpoint.py` & `returnn-1.20230724.124015/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.125702/tools/tf_inspect_summary_log.py` & `returnn-1.20230724.124015/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

