# Comparing `tmp/akida_models-1.1.9.tar.gz` & `tmp/akida_models-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/akida_models-1.1.9.tar", last modified: Wed Feb  8 10:09:57 2023, max compression
+gzip compressed data, was "dist/akida_models-1.2.0.tar", last modified: Mon Jul 24 07:44:08 2023, max compression
```

## Comparing `akida_models-1.1.9.tar` & `akida_models-1.2.0.tar`

### file list

```diff
@@ -1,103 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-02-08 10:09:51.000000 akida_models-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2635 2023-02-08 10:09:51.000000 akida_models-1.1.9/LICENSE.3rdparty
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-08 10:09:51.000000 akida_models-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      467 2023-02-08 10:09:57.000000 akida_models-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      147 2023-02-08 10:09:51.000000 akida_models-1.1.9/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/calibrable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/casia_webface/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/casia_webface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/casia_webface/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/centernet/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/centernet_batch_generator.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/centernet_loss.py
--rw-r--r--   0 root         (0) root         (0)     3839 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/centernet_processing.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/centernet_train.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/centernet/model_centernet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/cifar10/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cifar10/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cifar10/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)    16165 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/cwru/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cwru/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6457 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cwru/cwru_train.py
--rw-r--r--   0 root         (0) root         (0)     3525 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cwru/model_convtiny.py
--rw-r--r--   0 root         (0) root         (0)     6994 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/cyclic_lr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/detection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12510 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/batch_generator.py
--rw-r--r--   0 root         (0) root         (0)     5327 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/box_utils.py
--rw-r--r--   0 root         (0) root         (0)     4419 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/generate_anchors.py
--rw-r--r--   0 root         (0) root         (0)    11431 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/map_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/model_yolo.py
--rw-r--r--   0 root         (0) root         (0)    12177 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/processing.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/yolo_loss.py
--rw-r--r--   0 root         (0) root         (0)    10030 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/detection/yolo_train.py
--rw-r--r--   0 root         (0) root         (0)    11195 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/distiller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/dvs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18504 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/dvs_generator.py
--rw-r--r--   0 root         (0) root         (0)     6304 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/dvs_train.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/model_convtiny_gesture.py
--rw-r--r--   0 root         (0) root         (0)     6583 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/model_convtiny_handy.py
--rw-r--r--   0 root         (0) root         (0)    14435 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/dvs/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)    16608 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/filter_pruning.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/gamma_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/imagenet/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33671 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/imagenet_labels2names.py
--rw-r--r--   0 root         (0) root         (0)    25502 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/imagenet_train.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/imagenet_utils.py
--rw-r--r--   0 root         (0) root         (0)    22039 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_akidanet.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_akidanet18.py
--rw-r--r--   0 root         (0) root         (0)     4922 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_akidanet_edge.py
--rw-r--r--   0 root         (0) root         (0)    15427 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_mobilenet.py
--rw-r--r--   0 root         (0) root         (0)     4255 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_mobilenet_edge.py
--rw-r--r--   0 root         (0) root         (0)     8981 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/model_vgg.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/imagenet/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/kws/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/kws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5478 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/kws/kws_train.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/kws/model_ds_cnn.py
--rw-r--r--   0 root         (0) root         (0)    29214 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/kws/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)    21981 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/layer_blocks.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/macs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/mnist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/mnist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4867 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/mnist/mnist_train.py
--rw-r--r--   0 root         (0) root         (0)     5309 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/mnist/model_gxnor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/modelnet40/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/modelnet40/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8737 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/modelnet40/model_pointnet_plus.py
--rw-r--r--   0 root         (0) root         (0)     5771 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/modelnet40/modelnet40_train.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/modelnet40/pointnet_utils.py
--rw-r--r--   0 root         (0) root         (0)     8247 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/modelnet40/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     8177 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/param_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/portrait128/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/portrait128/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/portrait128/model_akida_unet.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/portrait128/portrait128_train.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/renaming.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/transformers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10952 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/transformers/model_deit.py
--rw-r--r--   0 root         (0) root         (0)    14435 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/transformers/model_vit.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models/utk_face/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/utk_face/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5927 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/utk_face/model_vgg.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/utk_face/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-02-08 10:09:51.000000 akida_models-1.1.9/akida_models/utk_face/utk_face_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)      467 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2955 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      605 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-08 10:09:57.000000 akida_models-1.1.9/akida_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 10:09:57.000000 akida_models-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-02-08 10:09:50.000000 akida_models-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-07-24 07:44:05.000000 akida_models-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-24 07:44:05.000000 akida_models-1.2.0/LICENSE.3rdparty
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-24 07:44:05.000000 akida_models-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      461 2023-07-24 07:44:08.000000 akida_models-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-24 07:44:05.000000 akida_models-1.2.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/casia_webface/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/casia_webface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/casia_webface/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/centernet/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/centernet_batch_generator.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/centernet_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/centernet_processing.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/centernet_train.py
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/centernet/model_centernet.py
+-rw-r--r--   0 root         (0) root         (0)    18344 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6994 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/cyclic_lr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/detection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12510 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/batch_generator.py
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/box_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/generate_anchors.py
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/map_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     6565 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/model_yolo.py
+-rw-r--r--   0 root         (0) root         (0)    12177 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/processing.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/yolo_loss.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/detection/yolo_train.py
+-rw-r--r--   0 root         (0) root         (0)    11195 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/distiller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/dvs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18504 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/dvs_generator.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/dvs_train.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/model_convtiny_gesture.py
+-rw-r--r--   0 root         (0) root         (0)     6256 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/model_convtiny_handy.py
+-rw-r--r--   0 root         (0) root         (0)    14435 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/dvs/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/extract.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/gamma_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/imagenet/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33671 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/imagenet_labels2names.py
+-rw-r--r--   0 root         (0) root         (0)    24273 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/imagenet_train.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/imagenet_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16245 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/model_akidanet.py
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/model_akidanet18.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/model_akidanet_edge.py
+-rw-r--r--   0 root         (0) root         (0)    14909 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/model_mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/imagenet/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/kws/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/kws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/kws/kws_train.py
+-rw-r--r--   0 root         (0) root         (0)     6230 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/kws/model_ds_cnn.py
+-rw-r--r--   0 root         (0) root         (0)    29692 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/kws/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    26466 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/layer_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/macs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/mnist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/mnist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/mnist/mnist_train.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/mnist/model_gxnor.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/model_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/modelnet40/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/modelnet40/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/modelnet40/model_pointnet_plus.py
+-rw-r--r--   0 root         (0) root         (0)     5227 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/modelnet40/modelnet40_train.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/modelnet40/pointnet_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8247 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/modelnet40/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     8177 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/param_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/portrait128/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/portrait128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6707 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/portrait128/model_akida_unet.py
+-rw-r--r--   0 root         (0) root         (0)     7613 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/portrait128/portrait128_train.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/transformers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11006 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/transformers/model_deit.py
+-rw-r--r--   0 root         (0) root         (0)    14489 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/transformers/model_vit.py
+-rw-r--r--   0 root         (0) root         (0)    12195 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/unfuse_sepconv_layers.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models/utk_face/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/utk_face/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4867 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/utk_face/model_vgg.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/utk_face/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-07-24 07:44:05.000000 akida_models-1.2.0/akida_models/utk_face/utk_face_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 07:44:08.000000 akida_models-1.2.0/akida_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 07:44:08.000000 akida_models-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-07-24 07:44:04.000000 akida_models-1.2.0/setup.py
```

### Comparing `akida_models-1.1.9/LICENSE` & `akida_models-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/LICENSE.3rdparty` & `akida_models-1.2.0/LICENSE.3rdparty`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/__init__.py` & `akida_models-1.2.0/akida_models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,45 +4,35 @@
 
 from .dvs.model_convtiny_gesture import (convtiny_dvs_gesture,
                                          convtiny_gesture_pretrained)
 from .dvs.model_convtiny_handy import (convtiny_dvs_handy,
                                        convtiny_handy_samsung_pretrained)
 from .imagenet.model_mobilenet import (mobilenet_imagenet,
                                        mobilenet_imagenet_pretrained)
-from .imagenet.model_vgg import (vgg_imagenet, vgg_imagenet_pretrained)
-from .imagenet.model_mobilenet_edge import (mobilenet_edge_imagenet,
-                                            mobilenet_edge_imagenet_pretrained)
 from .imagenet.model_akidanet import (
-    akidanet_imagenet, akidanet_imagenet_pretrained,
-    akidanet_cats_vs_dogs_pretrained, akidanet_imagenette_pretrained,
-    akidanet_faceidentification_pretrained,
-    akidanet_faceverification_pretrained, akidanet_melanoma_pretrained,
-    akidanet_odir5k_pretrained, akidanet_retinal_oct_pretrained,
-    akidanet_ecg_pretrained, akidanet_plantvillage_pretrained,
-    akidanet_cifar10_pretrained, akidanet_vww_pretrained)
+    akidanet_imagenet, akidanet_imagenet_pretrained, akidanet_faceidentification_pretrained,
+    akidanet_plantvillage_pretrained, akidanet_vww_pretrained)
 from .imagenet.model_akidanet_edge import (
     akidanet_edge_imagenet, akidanet_edge_imagenet_pretrained,
     akidanet_faceidentification_edge_pretrained)
 from .imagenet.model_akidanet18 import akidanet18_imagenet, akidanet18_imagenet_pretrained
 from .kws.model_ds_cnn import ds_cnn_kws, ds_cnn_kws_pretrained
 from .modelnet40.model_pointnet_plus import (pointnet_plus_modelnet40,
                                              pointnet_plus_modelnet40_pretrained
                                              )
 from .utk_face.model_vgg import vgg_utk_face, vgg_utk_face_pretrained
 from .detection.model_yolo import (yolo_base, yolo_widerface_pretrained,
                                    yolo_voc_pretrained)
-from .centernet.model_centernet import centernet_base
-from .cwru.model_convtiny import convtiny_cwru, convtiny_cwru_pretrained
+from .centernet.model_centernet import centernet_base, centernet_voc_pretrained
 from .mnist.model_gxnor import gxnor_mnist, gxnor_mnist_pretrained
 from .transformers.model_vit import (
     vit_imagenet, vit_ti16, bc_vit_ti16, bc_vit_ti16_imagenet_pretrained, vit_s16, vit_s32, vit_b16,
     vit_b32, vit_l16, vit_l32)
 from .transformers.model_deit import (
     deit_imagenet, deit_ti16, bc_deit_ti16, bc_deit_dist_ti16_imagenet_pretrained,
     deit_s16, deit_b16)
-from .portrait128.model_akida_unet import akida_unet_portrait128
+from .portrait128.model_akida_unet import akida_unet_portrait128, akida_unet_portrait128_pretrained
 
-from .calibrable import calibration_required
+from .extract import extract_samples
 from .gamma_constraint import add_gamma_constraint
-from .filter_pruning import delete_filters, prune_model
-from .renaming import rename_model_layers
-from .utils import fetch_file
+from .utils import fetch_file, get_params_by_version
+from .unfuse_sepconv_layers import unfuse_sepconv2d
```

### Comparing `akida_models-1.1.9/akida_models/casia_webface/preprocessing.py` & `akida_models-1.2.0/akida_models/casia_webface/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/centernet/centernet_batch_generator.py` & `akida_models-1.2.0/akida_models/centernet/centernet_batch_generator.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/centernet/centernet_loss.py` & `akida_models-1.2.0/akida_models/centernet/centernet_loss.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/centernet/centernet_processing.py` & `akida_models-1.2.0/akida_models/centernet/centernet_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     Args:
         output (tf.Tensor): model output to decode.
         nb_classes (int): number of classes.
         obj_threshold (float, optional): confidence threshold for a box. Defaults to 0.1.
         max_detection (int, optional): maximum number of boxes the model is allowed to produce.
             Defaults to 100.
-        kernel (int, optional) : max pool kernel size. Defaults to 5.
+        kernel (int, optional): max pool kernel size. Defaults to 5.
 
     Returns:
         List: `BoundingBox` objects
     """
 
     def _sigmoid(x):
         return 1. / (1. + np.exp(-x))
```

### Comparing `akida_models-1.1.9/akida_models/centernet/centernet_train.py` & `akida_models-1.2.0/akida_models/centernet/centernet_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
 Training script for CenterNet models
 """
+import os
 import pickle
 import argparse
 
 from keras import Model
+from cnn2snn import convert
 
-from ..training import get_training_parser, freeze_model_before, compile_model
+from ..training import get_training_parser, freeze_model_before, compile_model, save_model
 from ..detection.map_evaluation import MapEvaluation
 from ..param_scheduler import get_cosine_lr_scheduler
-from ..utils import get_tensorboard_callback, load_model
+from ..utils import get_tensorboard_callback
+from ..model_io import load_model
 
 from .centernet_batch_generator import BatchCenternetGenerator
 from .centernet_loss import CenternetLoss
 from .centernet_processing import decode_output
 
 
 def get_data(data_path):
@@ -142,15 +145,15 @@
 def main():
     """ Entry point for script and CLI usage. """
     global_parser = argparse.ArgumentParser(add_help=False)
     global_parser.add_argument("-d", "--data", default=None,
                                help="The pickle file generated by the preprocessing step")
     global_parser.add_argument("-obj", "--obj_thresh", type=float, default=0.1,
                                help="Confidence threshold for a box. Defaults to %(default)s")
-    global_parser.add_argument("-o", "--out_dir", type=str, default=None,
+    global_parser.add_argument("-o", "--out_dir", type=str, default='./logs',
                                help="The output directory (logs). Defaults to %(default)s")
     parsers = get_training_parser(batch_size=128, freeze_before=True, tune=True,
                                   global_parser=global_parser)
     args = parsers[0].parse_args()
 
     # Load data
     train_data, valid_data, labels = get_data(args.data)
@@ -169,28 +172,24 @@
     if "freeze_before" in args:
         freeze_model_before(model, args.freeze_before)
 
     # Compile model
     learning_rate = 1e-4 if args.action == "tune" else 1e-2
     compile_model(model, learning_rate=learning_rate, loss=CenternetLoss(), metrics=None)
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     if args.action in ["train", "tune"]:
         train(model, train_data, valid_data, labels, learning_rate, args.obj_thresh,
               args.epochs, args.batch_size, grid_size, out_dir=args.out_dir,
               tune=args.action == "tune")
-
-        if args.savemodel:
-            # Save the model
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
-        # TODO: enable this feature when cnn2snn support SeparableConv2DTranspose
-        # and full conversion into akida
         if args.akida:
-            raise NotImplementedError("Not implemented yet!")
+            model = convert(model)
         evaluate(model, valid_data, labels, args.obj_thresh)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/cli.py` & `akida_models-1.2.0/akida_models/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,34 +19,67 @@
 
 This package entry-point allows akida models to be instantiated and saved at a
 specified location.
 
 """
 
 import argparse
+import os
 
 from .utk_face.model_vgg import vgg_utk_face
 from .kws.model_ds_cnn import ds_cnn_kws
 from .modelnet40.model_pointnet_plus import pointnet_plus_modelnet40
 from .imagenet.model_mobilenet import mobilenet_imagenet
-from .imagenet.model_vgg import vgg_imagenet
 from .imagenet.model_akidanet import akidanet_imagenet
 from .imagenet.model_akidanet_edge import akidanet_edge_imagenet
 from .imagenet.model_akidanet18 import akidanet18_imagenet
-from .imagenet.model_mobilenet_edge import mobilenet_edge_imagenet
 from .detection.model_yolo import yolo_base
 from .dvs.model_convtiny_handy import convtiny_dvs_handy
 from .dvs.model_convtiny_gesture import convtiny_dvs_gesture
-from .cwru.model_convtiny import convtiny_cwru
 from .mnist.model_gxnor import gxnor_mnist
 from .transformers.model_vit import vit_ti16, bc_vit_ti16
 from .transformers.model_deit import deit_ti16, bc_deit_ti16
 from .portrait128.model_akida_unet import akida_unet_portrait128
 from .centernet.model_centernet import centernet_base
 from .macs import display_macs
+from .model_io import load_weights, save_weights, load_model
+from .unfuse_sepconv_layers import unfuse_sepconv2d
+
+
+def save_model_weights(model_path, weights_path):
+    """ CLI entry point to save the model weights in an npz file.
+
+    Args:
+        model_path (str): Path to the model to extract the weights from.
+        weights_path (str): Path to save the npz file.
+            Defaults to <model_path>.npz.
+    """
+    # Build name for weights file
+    if weights_path is None:
+        model_name = os.path.splitext(model_path)[0]
+        weights_path = f"{model_name}.npz"
+
+    # Load the model and save its weights
+    model = load_model(model_path)
+    save_weights(model, weights_path)
+    print(f"Saved model weights to {weights_path}.")
+
+
+def load_model_weights(model_path, weights_path):
+    """ CLI entry point to apply weights to a model from an npz file.
+
+    Args:
+        model_path (str): Path to the model on which apply the weights.
+        weights_path (str): Path to load the npz file.
+    """
+    # Update the model weights with the npz file
+    model = load_model(model_path)
+    load_weights(model, weights_path)
+    model.save(model_path, include_optimizer=False)
+    print(f"Saved model with new weights to {model_path}.")
 
 
 def add_transformers_args(parser, add_customs=False, default_norm='LN', default_act='GeLU'):
     """ Add transformers commons arguments to the given parser.
 
     Args:
         parser (argparse.ArgumentParser): parser to add args to
@@ -124,50 +157,44 @@
                           "--save_model",
                           type=str,
                           default=None,
                           help="The path/name to use to save the model")
     csp = c_parser.add_subparsers(dest="model",
                                   help="The type of model to be instantiated")
     csp.add_parser("vgg_utk_face", help="A VGG-like UTKFace model")
-    csp.add_parser("convtiny_dvs_handy", help="A Convtiny DVS handy model")
 
     dvsh_parser = csp.add_parser("convtiny_dvs_handy",
-                                 help="A Convtiny DVS model for akida")
+                                 help="A Convtiny DVS handy model")
     add_common_args(dvsh_parser, default_classes=9)
 
-    csp.add_parser("convtiny_dvs_gesture", help="A Convtiny DVS gesture model")
-
     dvsg_parser = csp.add_parser("convtiny_dvs_gesture",
-                                 help="A Convtiny DVS model for akida")
+                                 help="A Convtiny DVS gesture model")
     add_common_args(dvsg_parser, default_classes=10)
 
     csp.add_parser(
         "ds_cnn_kws",
         help="A Depthwise Separable MobileNet-like model for the Keyword"
         " Spotting example")
 
     mb_parser = csp.add_parser("mobilenet_imagenet",
                                help="A MobileNet V1 model for akida")
     add_common_args(mb_parser, default_classes=1000, default_alpha=1.0, default_img_size=224)
 
-    vgg_parser = csp.add_parser("vgg_imagenet", help="A VGG model for akida")
-    add_common_args(vgg_parser, default_classes=1000)
-
-    mbe_parser = csp.add_parser("mobilenet_imagenet_edge",
-                                help="A MobileNet V1 model modified for akida \
-                                edge learning")
-    add_common_args(mbe_parser, default_classes=1000, bw_required=True)
-
     an_parser = csp.add_parser("akidanet_imagenet", help="An AkidaNet model")
     add_common_args(an_parser, default_classes=1000, default_img_size=224, default_alpha=1.0)
 
     ane_parser = csp.add_parser("akidanet_edge_imagenet",
                                 help="An AkidaNet model modified for akida \
                                 edge learning")
     add_common_args(ane_parser, default_classes=1000, bw_required=True)
+    ane_parser.add_argument("-bl",
+                            "--base_layer",
+                            type=str,
+                            default="classifier",
+                            help="Last layer of the base model.")
 
     an18_parser = csp.add_parser("akidanet18_imagenet", help="An AkidaNet18 model")
     add_common_args(an18_parser, default_classes=1000, default_img_size=224)
 
     pnet_parser = csp.add_parser("pointnet_plus_modelnet40",
                                  help="A PointNet++ model for Akida")
     add_common_args(pnet_parser, default_classes=40)
@@ -182,15 +209,14 @@
     add_common_args(yl_parser, default_classes=1, default_alpha=0.5, bw_required=False)
     yl_parser.add_argument("-na",
                            "--number_anchors",
                            type=int,
                            default=5,
                            help="The number of anchor boxes")
 
-    csp.add_parser("convtiny_cwru", help="A Convtiny CWRU model for akida")
     csp.add_parser("gxnor_mnist", help="A GXNOR MNIST model for akida")
 
     akun_parser = csp.add_parser("akida_unet_portrait128",
                                  help="An Akida U-Net model for Portrait128 segmentation.")
     akun_parser.add_argument("-bw", "--base_weights", type=str, default=None,
                              help="The base AkidaNet weights to use for the encoder.")
 
@@ -220,14 +246,34 @@
     bc_deit_parser.add_argument("-b", "--blocks", type=int, default=12,
                                 help="Number of transformer blocks")
 
     macs_parser = sp.add_parser("macs", help="Get MACS for a Keras model")
     macs_parser.add_argument("-m", "--model", type=str)
     macs_parser.add_argument("-v", "--verbose", action="store_true")
 
+    unfuse_parser = sp.add_parser(
+        "unfuse", help="Unfuse SeparableConv2D layers of a Keras model")
+    unfuse_parser.add_argument("-m", "--model", type=str, required=True, help="Model to unfuse.")
+
+    # Save weights arguments
+    w_parser = sp.add_parser(
+        "save_weights", help="Store model's weights in an npz.")
+    w_parser.add_argument("-m", "--model", type=str, required=True,
+                          help="Model to extract weights from.")
+    w_parser.add_argument("-w", "--weights_path", type=str,
+                          help="Npz file that contains the saved weights.")
+
+    # Load weights arguments
+    w_parser = sp.add_parser(
+        "load_weights", help="Apply weights to a model from an npz file.")
+    w_parser.add_argument("-m", "--model", type=str, required=True,
+                          help="Model to apply the weights.")
+    w_parser.add_argument("-w", "--weights_path", type=str, required=True,
+                          help="Npz file that contains the weights to apply.")
+
     args = parser.parse_args()
     if args.action == "create":
         # Instantiate the wished model
         if args.model == "vgg_utk_face":
             model = vgg_utk_face()
         elif args.model == "convtiny_dvs_handy":
             model = convtiny_dvs_handy(classes=args.classes)
@@ -239,43 +285,37 @@
             model = pointnet_plus_modelnet40(alpha=args.alpha,
                                              classes=args.classes)
         elif args.model == "mobilenet_imagenet":
             input_shape = (args.image_size, args.image_size, 3)
             model = mobilenet_imagenet(input_shape,
                                        alpha=args.alpha,
                                        classes=args.classes)
-        elif args.model == "vgg_imagenet":
-            model = vgg_imagenet(classes=args.classes)
-        elif args.model == "mobilenet_imagenet_edge":
-            model = mobilenet_edge_imagenet(base_model=args.base_weights,
-                                            classes=args.classes)
         elif args.model == "akidanet_imagenet":
             input_shape = (args.image_size, args.image_size, 3)
             model = akidanet_imagenet(input_shape,
                                       alpha=args.alpha,
                                       classes=args.classes)
         elif args.model == "akidanet_edge_imagenet":
             model = akidanet_edge_imagenet(base_model=args.base_weights,
-                                           classes=args.classes)
+                                           classes=args.classes,
+                                           base_layer=args.base_layer)
         elif args.model == "akidanet18_imagenet":
             input_shape = (args.image_size, args.image_size, 3)
             model = akidanet18_imagenet(input_shape, classes=args.classes)
         elif args.model == "yolo_base":
             model = yolo_base(classes=args.classes,
                               nb_box=args.number_anchors,
                               alpha=args.alpha)
             if args.base_weights is not None:
                 model.load_weights(args.base_weights, by_name=True)
         elif args.model == "centernet":
             model = centernet_base(input_shape=(args.image_size, args.image_size, 3),
                                    classes=args.classes, alpha=args.alpha)
             if args.base_weights is not None:
                 model.load_weights(args.base_weights, by_name=True)
-        elif args.model == "convtiny_cwru":
-            model = convtiny_cwru()
         elif args.model == "gxnor_mnist":
             model = gxnor_mnist()
         elif args.model == "akida_unet_portrait128":
             model = akida_unet_portrait128()
             if args.base_weights is not None:
                 model.load_weights(args.base_weights, by_name=True)
         else:
@@ -305,18 +345,38 @@
             # Load provided weights
             if args.base_weights is not None:
                 model.load_weights(args.base_weights, by_name=True)
         # No need for default behaviour as the command-line parser only accepts
         # valid model types
         model_path = args.save_model
         if model_path is None:
-            models_by_name = ("mobilenet_imagenet", "mobilenet_imagenet_edge", "centernet")
+            models_by_name = ("mobilenet_imagenet", "centernet")
             model_path = f"{model.name}.h5" if args.model in models_by_name else f"{args.model}.h5"
 
         # If needed, add the extension
         if not model_path.endswith(".h5"):
             model_path = f"{model_path}.h5"
         model.save(model_path, include_optimizer=False)
         print(f"Model saved as {model_path}")
 
     elif args.action == "macs":
         display_macs(args.model, args.verbose)
+    elif args.action == "save_weights":
+        save_model_weights(
+            model_path=args.model,
+            weights_path=args.weights_path,
+        )
+    elif args.action == "load_weights":
+        load_model_weights(
+            model_path=args.model,
+            weights_path=args.weights_path,
+        )
+    elif args.action == "unfuse":
+        model = load_model(args.model)
+        unfused_model = unfuse_sepconv2d(model)
+        # strip file extension from model path
+        model_path = os.path.splitext(args.model)[0]
+        # Write new path for unfused model
+        model_path += "_unfused.h5"
+        # Save unfused model
+        unfused_model.save(model_path, include_optimizer=False)
+        print(f"{model.name} has been unfused and saved under {model_path}.")
```

### Comparing `akida_models-1.1.9/akida_models/cwru/model_convtiny.py` & `akida_models-1.2.0/akida_models/utk_face/model_vgg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,139 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2021 Brainchip Holdings Ltd.
+# Copyright 2020 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Convtiny model definition for CWRU classification.
+VGG model definition for UTKFace regression.
 """
 
 from keras import Model
-from keras.layers import Input, Softmax, Rescaling, Reshape
+from keras.layers import Dropout, Flatten, Input, Rescaling
 
-from cnn2snn import load_quantized_model
+from ..layer_blocks import conv_block, dense_block
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
+
+
+def vgg_utk_face(input_shape=(32, 32, 3), input_scaling=(127, -1)):
+    """Instantiates a VGG-like model for the regression example on age
+    estimation using UTKFace dataset.
+
+    Args:
+        input_shape (tuple, optional): input shape tuple of the model. Defaults to (32, 32, 3).
+        input_scaling (tuple, optional): scale factor and offset to apply to
+            inputs. Defaults to (127, -1). Note that following Akida convention,
+            the scale factor is an integer used as a divider.
 
-from ..layer_blocks import conv_block, separable_conv_block
-from ..utils import fetch_file
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/convtiny/'
+    Returns:
+        keras.Model: a Keras model for VGG/UTKFace
+    """
+    img_input = Input(shape=input_shape, name="input")
 
+    if input_scaling is None:
+        x = img_input
+    else:
+        scale, offset = input_scaling
+        x = Rescaling(1. / scale, offset, name="rescaling")(img_input)
 
-def convtiny_cwru():
-    """ Instantiates a CNN for CWRU classification with input shape (32, 32, 1)
-    and 10 classes.
+    # Model version management
+    _, _, relu_activation = get_params_by_version()
 
-    Returns:
-        keras.Model: a Keras model for Convtiny/CWRU
+    x = conv_block(x,
+                   filters=32,
+                   kernel_size=(3, 3),
+                   name='conv_0',
+                   use_bias=False,
+                   relu_activation=relu_activation,
+                   add_batchnorm=True)
 
-    """
-    img_input = Input(shape=(32, 32, 1), name="input")
-    x = Rescaling(1, -127, name="rescaling")(img_input)
     x = conv_block(x,
                    filters=32,
+                   kernel_size=(3, 3),
                    name='conv_1',
-                   kernel_size=(7, 7),
                    padding='same',
-                   add_activation=True,
                    pooling='max',
-                   pool_size=(2, 2))
+                   pool_size=2,
+                   use_bias=False,
+                   relu_activation=relu_activation,
+                   add_batchnorm=True)
+
+    x = Dropout(0.3, name="dropout_3")(x)
 
     x = conv_block(x,
-                   filters=32,
+                   filters=64,
+                   kernel_size=(3, 3),
+                   padding='same',
                    name='conv_2',
-                   kernel_size=(7, 7),
+                   use_bias=False,
+                   relu_activation=relu_activation,
+                   add_batchnorm=True)
+
+    x = conv_block(x,
+                   filters=64,
+                   kernel_size=(3, 3),
                    padding='same',
-                   add_activation=True,
+                   name='conv_3',
                    pooling='max',
-                   pool_size=(2, 2))
+                   pool_size=2,
+                   use_bias=False,
+                   relu_activation=relu_activation,
+                   add_batchnorm=True)
+
+    x = Dropout(0.3, name="dropout_4")(x)
+
+    x = conv_block(x,
+                   filters=84,
+                   kernel_size=(3, 3),
+                   padding='same',
+                   name='conv_4',
+                   use_bias=False,
+                   relu_activation=relu_activation,
+                   add_batchnorm=True)
+
+    x = Dropout(0.3, name="dropout_5")(x)
+    x = Flatten(name="flatten")(x)
+
+    x = dense_block(x,
+                    units=64,
+                    name='dense_1',
+                    use_bias=False,
+                    relu_activation=relu_activation,
+                    add_batchnorm=True)
 
-    x = separable_conv_block(x,
-                             filters=512,
-                             name='separable_1',
-                             kernel_size=(3, 3),
-                             padding='same',
-                             pooling='global_avg',
-                             use_bias=False,
-                             add_batchnorm=True,
-                             add_activation=True)
-
-    x = Reshape((1, 1, int(512)), name='reshape_1')(x)
-
-    x = separable_conv_block(x,
-                             filters=10,
-                             name='predictions',
-                             kernel_size=(3, 3),
-                             padding='same',
-                             use_bias=False,
-                             add_batchnorm=False,
-                             add_activation=False)
-    x = Reshape((10,), name='reshape_2')(x)
-    x = Softmax(name='act_softmax')(x)
+    x = dense_block(x, units=1, name='dense_2', relu_activation=False)
 
-    return Model(img_input, x, name='convtiny_cwru_32_10')
+    return Model(img_input, x, name='vgg_utk_face')
 
 
-def convtiny_cwru_pretrained():
+def vgg_utk_face_pretrained():
     """
-    Helper method to retrieve a `convtiny_cwru` model that was trained on
-    CWRU dataset.
+    Helper method to retrieve a `vgg_utk_face` model that was trained on
+    UTK Face dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'convtiny_cwru_iq8_wq2_aq4.h5'
-    file_hash = '230b9e2e5901d5428fdba01f45f32ce261bcaabe4b5f861a58bed85e34f21f96'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v1 = 'vgg_utk_face_iq8_wq2_aq2.h5'
+    file_hash_v1 = 'e341d2d5e4655846ddc7aceff0d4e324cbfbcca16f3cfefc65e7b0863e4a23a3'
+    model_name_v2 = 'vgg_utk_face_i8_w4_a4.h5'
+    file_hash_v2 = '06a892b9e831767537b1da937bbacf05825c7493b7a5a9ba46bea4900de0563a'
+    model_path, model_name, file_hash = get_model_path("vgg", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/cyclic_lr.py` & `akida_models-1.2.0/akida_models/cyclic_lr.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/detection/batch_generator.py` & `akida_models-1.2.0/akida_models/detection/batch_generator.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/detection/box_utils.py` & `akida_models-1.2.0/akida_models/detection/box_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 def xywh_to_xyxy(boxes):
     """Convert a set of boxes from format xywh to xyxy, where each format represent:
 
         * 'xywh': format of ('cx', 'xy', 'w', 'h'), also called 'centroids' and
         * 'xyxy': format of ('x_min', 'y_min', 'x_max', 'y_max'), also called 'corners'.
 
     Args:
-        boxes (tf.tensor or np.ndarray): tensor with shape (N, 4)
+        boxes (tf.Tensor or np.ndarray): tensor with shape (N, 4)
 
     Returns:
-        tf.tensor or np.ndarray: tensor with new format
+        tf.Tensor or np.ndarray: tensor with new format
     """
     assert boxes.shape[-1] == 4, "Expected 4 as last dimension."
     x1y1 = boxes[..., :2] - 0.5 * boxes[..., -2:]
     x2y2 = boxes[..., :2] + 0.5 * boxes[..., -2:]
     if isinstance(boxes, tf.Tensor):
         return tf.concat([x1y1, x2y2], axis=-1)
     return np.concatenate([x1y1, x2y2], axis=-1)
@@ -44,18 +44,18 @@
 def xyxy_to_xywh(boxes):
     """Convert a set of boxes from format xyxy to xywh, where each format represent:
 
         * 'xyxy': format of ('x_min', 'y_min', 'x_max', 'y_max'), also called 'corners' and
         * 'xywh': format of ('cx', 'xy', 'w', 'h'), also called 'centroids'.
 
     Args:
-        boxes (tf.tensor): tensor with shape (N, 4)
+        boxes (tf.Tensor): tensor with shape (N, 4)
 
     Returns:
-        tf.tensor: tensor with new format
+        tf.Tensor: tensor with new format
     """
     assert boxes.shape[-1] == 4, "Expected 4 as last dimension."
     tf.debugging.assert_greater_equal(boxes[..., -2:], boxes[..., :2],
                                       "x2y2 must be greater than x1y1")
     wh = boxes[..., -2:] - boxes[..., :2]
     xy = boxes[..., :2] + 0.5 * wh
     if isinstance(boxes, tf.Tensor):
@@ -66,22 +66,24 @@
 def compute_overlap(a1, a2, mode="element_wise", box_format="xywh"):
     """Calculate ious between a1, a2 in two different modes:
 
         * element_wise: compute iou element-by-element, returning 1D array tensor,
         * outer_product: compute cross iou with all possible combination between inputs.
 
     Args:
-        a1 (tf.tensor or np.ndarray): set of boxes, with shape at least equal to (N, 4).
-        a2 (tf.tensor or np.ndarray): set of boxes, with compatible broadcast-shape
+        a1 (tf.Tensor or np.ndarray): set of boxes, with shape at least equal to (N, 4).
+        a2 (tf.Tensor or np.ndarray): set of boxes, with compatible broadcast-shape
             (in 'element_wise' mode) or shape at least equal to (N, 4) (in 'outer_product' mode).
+        mode (str, optional): the mode to use. 'element_wise' or 'outer_product'. Defaults to
+            "element_wise".
         box_format (str, optional): format of both inputs. Defaults to 'xywh'.
 
     Returns:
-        tf.tensor or np.ndarray: IoU between inputs with shape (N,) in 'element_wise',
-            otherwise (N, M).
+        tf.Tensor or np.ndarray: IoU between inputs with shape (N,) in 'element_wise',
+        otherwise (N, M).
     """
     format_choices = ["xywh", "xyxy"]
     mode_choises = ["element_wise", "outer_product"]
     assert box_format in format_choices, f"box format must be one of {format_choices}"
     assert mode in mode_choises, f"mode must be one of {mode_choises}"
 
     def process_boxes(a):
```

### Comparing `akida_models-1.1.9/akida_models/detection/generate_anchors.py` & `akida_models-1.2.0/akida_models/detection/generate_anchors.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         # assign samples to centroids
         assignments = np.argmin(distances, axis=1)
 
         if (assignments == prev_assignments).all():
             return centroids
 
         # calculate new centroids
-        centroid_sums = np.zeros((anchor_num, anchor_dim), np.float)
+        centroid_sums = np.zeros((anchor_num, anchor_dim), float)
         for i in range(ann_num):
             centroid_sums[assignments[i]] += ann_dims[i]
         for j in range(anchor_num):
             centroids[j] = centroid_sums[j] / (np.sum(assignments == j) + 1e-6)
 
         prev_assignments = assignments.copy()
```

### Comparing `akida_models-1.1.9/akida_models/detection/map_evaluation.py` & `akida_models-1.2.0/akida_models/detection/map_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,24 +135,27 @@
         for i in range(self._data_len):
             raw_image = load_image(self._data[i]['image_path'])
             raw_height, raw_width, _ = raw_image.shape
 
             if self._is_keras_model:
                 image = preprocess_image(raw_image, self._model.input_shape[1:])
                 input_image = image[np.newaxis, :]
-                output = self._model.predict(input_image)[0]
+                output = self._model.predict(input_image, verbose=0)[0]
             else:
                 image = preprocess_image(raw_image,
                                          self._model.layers[0].input_dims)
                 input_image = image[np.newaxis, :].astype(np.uint8)
                 potentials = self._model.predict(input_image)[0]
 
-                h, w, _ = potentials.shape
-                output = potentials.reshape(
-                    (h, w, len(self._anchors), 4 + 1 + self._num_classes))
+                if self._anchors:
+                    h, w, _ = potentials.shape
+                    output = potentials.reshape(
+                        (h, w, len(self._anchors), 4 + 1 + self._num_classes))
+                else:
+                    output = potentials
 
             pred_boxes = self._decode_output(output, self._anchors, self._num_classes,
                                              self._obj_threshold, self._nms_threshold)
 
             score = np.array([box.get_score() for box in pred_boxes])
             pred_labels = np.array([box.get_label() for box in pred_boxes])
```

### Comparing `akida_models-1.1.9/akida_models/detection/model_yolo.py` & `akida_models-1.2.0/akida_models/detection/model_yolo.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,152 +20,144 @@
 
 import pickle
 
 import numpy as np
 
 from keras import Model
 
-from cnn2snn import load_quantized_model, quantize
-
 from ..layer_blocks import yolo_head_block
 from ..imagenet.model_akidanet import akidanet_imagenet
 from ..utils import fetch_file
+from ..model_io import load_model, get_model_path
 
 
-def yolo_base(input_shape=(224, 224, 3),
-              classes=1,
-              nb_box=5,
-              alpha=1.0,
-              weight_quantization=0,
-              activ_quantization=0,
-              input_weight_quantization=None,
-              input_scaling=(127.5, -1)):
+def yolo_base(input_shape=(224, 224, 3), classes=1, nb_box=5, alpha=1.0, input_scaling=(127.5, -1)):
     """ Instantiates the YOLOv2 architecture.
 
     Args:
-        input_shape (tuple): input shape tuple
-        classes (int): number of classes to classify images into
-        nb_box (int): number of anchors boxes to use
-        alpha (float): controls the width of the model
-        weight_quantization (int): sets all weights in the model to have
-            a particular quantization bitwidth except for the weights in the
-            first layer.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization: sets all activations in the model to have a
-            particular activation quantization bitwidth.
-
-            * '0' implements floating point 32-bit activations.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        input_weight_quantization: sets weight quantization in the first layer.
-            Defaults to weight_quantization value.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
+        input_shape (tuple, optional): input shape tuple. Defaults to (224, 224, 3).
+        classes (int, optional): number of classes to classify images into. Defaults to 1.
+        nb_box (int, optional): number of anchors boxes to use. Defaults to 5.
+        alpha (float, optional): controls the width of the model. Defaults to 1.0.
         input_scaling (tuple, optional): scale factor and offset to apply to
             inputs. Defaults to (127.5, -1). Note that following Akida
             convention, the scale factor is a number used as a divider.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    # Overrides input weight quantization if None
-    if input_weight_quantization is None:
-        input_weight_quantization = weight_quantization
-
     # Create an AkidaNet network without top layers
-    base_model = akidanet_imagenet(
-        input_shape=input_shape,
-        alpha=alpha,
-        include_top=False,
-        weight_quantization=weight_quantization,
-        activ_quantization=activ_quantization,
-        input_weight_quantization=input_weight_quantization,
-        input_scaling=input_scaling)
+    base_model = akidanet_imagenet(input_shape=input_shape, alpha=alpha, include_top=False,
+                                   input_scaling=input_scaling)
 
     # Add YOLO top layers to the base model
     input_shape = base_model.input_shape
     x = yolo_head_block(base_model.layers[-1].output, num_boxes=nb_box, classes=classes)
     model = Model(inputs=base_model.input, outputs=x, name='yolo_base')
 
     # Initialize detection layer weights
-    layer = model.get_layer("detection_layer")
-    detection_weights = layer.get_weights()
+    layers = [layer for layer in model.layers if "detection_layer" in layer.name]
+    assert len(layers) in (1, 2), "No detection layer found."
+
+    if len(layers) == 1:
+        # sepconv is fused on Akida v1
+        layer = layers[0]
+        detection_weights = layer.get_weights()
+        dw_weights_shape = detection_weights[0].shape
+        pw_weights_shape = detection_weights[1].shape
+        bias_shape = detection_weights[2].shape
+    else:
+        # sepconv is unfused on Akida v2
+        dw_layer = layers[0]
+        pw_layer = layers[1]
+        dw_weights = dw_layer.get_weights()
+        assert len(dw_weights) == 1  # no bias
+        pw_weights = pw_layer.get_weights()
+        dw_weights_shape = dw_weights[0].shape
+        pw_weights_shape = pw_weights[0].shape
+        bias_shape = pw_weights[1].shape
 
     mu, sigma = 0, 0.1
 
     grid_size = model.output_shape[1:3]
     grid_area = grid_size[0] * grid_size[1]
 
     dw_kernel = np.random.normal(mu, sigma,
-                                 size=detection_weights[0].shape) / grid_area
+                                 size=dw_weights_shape) / grid_area
     pw_kernel = np.random.normal(mu, sigma,
-                                 size=detection_weights[1].shape) / grid_area
+                                 size=pw_weights_shape) / grid_area
     bias = np.random.normal(mu, sigma,
-                            size=detection_weights[2].shape) / grid_area
+                            size=bias_shape) / grid_area
 
-    layer.set_weights([dw_kernel, pw_kernel, bias])
+    if len(layers) == 1:
+        layer.set_weights([dw_kernel, pw_kernel, bias])
+    else:
+        dw_layer.set_weights([dw_kernel])
+        pw_layer.set_weights([pw_kernel, bias])
 
-    if ((weight_quantization != 0) or (activ_quantization != 0) or
-            (input_weight_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization,
-                        input_weight_quantization)
     return model
 
 
 def yolo_widerface_pretrained():
     """
     Helper method to retrieve a `yolo_base` model that was trained on WiderFace
     dataset and the anchors that are needed to interpet the model output.
 
     Returns:
         keras.Model, list: a Keras Model instance and a list of anchors.
 
     """
     anchors_name = 'widerface_anchors.pkl'
     anchors_path = fetch_file(
-        'http://data.brainchip.com/dataset-mirror/widerface/' + anchors_name,
+        'https://data.brainchip.com/dataset-mirror/widerface/' + anchors_name,
         fname=anchors_name,
         file_hash='325f92336a310d83fed71765436ee343bf3e39cbc12fd099d30677761aee9376',
         cache_subdir='datasets/widerface')
     with open(anchors_path, 'rb') as handle:
         anchors = pickle.load(handle)
 
-    model_name = 'yolo_akidanet_widerface_iq8_wq4_aq4.h5'
-    file_hash = 'd55744cbfbbe1131aa26015f38d99f1df7026347bae8f66683259e366e7b6e03'
-    model_path = fetch_file('http://data.brainchip.com/models/yolo/' + model_name,
+    model_name_v1 = 'yolo_akidanet_widerface_iq8_wq4_aq4.h5'
+    file_hash_v1 = 'd55744cbfbbe1131aa26015f38d99f1df7026347bae8f66683259e366e7b6e03'
+    model_name_v2 = 'yolo_akidanet_widerface_i8_w4_a4.h5'
+    file_hash_v2 = '13e4290c4f197c08ba93ded44a9f5a5ab07e793f1e216737134a700feeb74cf9'
+    model_path, model_name, file_hash = get_model_path("yolo", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
 
-    return load_quantized_model(model_path), anchors
+    return load_model(model_path), anchors
 
 
 def yolo_voc_pretrained():
     """
     Helper method to retrieve a `yolo_base` model that was trained on PASCAL
     VOC2012 dataset for 'person' and 'car' classes only, and the anchors that
     are needed to interpet the model output.
 
     Returns:
         keras.Model, list: a Keras Model instance and a list of anchors.
 
     """
     anchors_name = 'voc_anchors.pkl'
     anchors_path = fetch_file(
-        'http://data.brainchip.com/dataset-mirror/voc/' + anchors_name,
+        'https://data.brainchip.com/dataset-mirror/voc/' + anchors_name,
         fname=anchors_name,
         file_hash='b1fe1ed12691e100646cf52b1320f05abd17b2f546d3e12cdee87758cc9ed0ba',
         cache_subdir='datasets/voc')
     with open(anchors_path, 'rb') as handle:
         anchors = pickle.load(handle)
 
-    model_name = 'yolo_akidanet_voc_iq8_wq4_aq4.h5'
-    file_hash = 'e65b0b6bd4b08c2796c3bbea89343748195e29e240ce28e70489c53d06ca69d9'
-    model_path = fetch_file('http://data.brainchip.com/models/yolo/' + model_name,
+    model_name_v1 = 'yolo_akidanet_voc_iq8_wq4_aq4.h5'
+    file_hash_v1 = 'e65b0b6bd4b08c2796c3bbea89343748195e29e240ce28e70489c53d06ca69d9'
+    model_name_v2 = 'yolo_akidanet_voc_i8_w4_a4.h5'
+    file_hash_v2 = 'a66791f482e33f4a2bc05db652e604ce494a5e6a6253749429535c4007938174'
+    model_path, model_name, file_hash = get_model_path("yolo", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
 
-    return load_quantized_model(model_path), anchors
+    return load_model(model_path), anchors
```

### Comparing `akida_models-1.1.9/akida_models/detection/processing.py` & `akida_models-1.2.0/akida_models/detection/processing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/detection/yolo_loss.py` & `akida_models-1.2.0/akida_models/detection/yolo_loss.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/detection/yolo_train.py` & `akida_models-1.2.0/akida_models/detection/yolo_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
 Training script for YOLO models.
 """
 
+import os
 import pickle
 import argparse
 import numpy as np
 
 from keras import Model
 from keras.layers import Reshape
 from keras.callbacks import EarlyStopping
 
-from cnn2snn import load_quantized_model, convert
+from cnn2snn import convert
 
 from .yolo_loss import YoloLoss
 from .map_evaluation import MapEvaluation
 from .batch_generator import BatchYoloGenerator
-from ..training import get_training_parser, freeze_model_before, compile_model
+from ..training import get_training_parser, freeze_model_before, compile_model, save_model
+from ..model_io import load_model
 
 
 def get_data(data_path, anchors_path):
     """ Loads data.
 
     Args:
         data_path (str): path to data pickle file
@@ -140,15 +142,15 @@
     mAP, average_precisions = map_evaluator.evaluate_map()
     for label, average_precision in average_precisions.items():
         print(labels[label], '{:.4f}'.format(average_precision))
     print('mAP: {:.4f}'.format(mAP))
 
 
 def extract_samples(im_size, data, grid_size, anchors, labels, num_samples, out_file):
-    """ Extract samples from data and save them to a .npz file.
+    """ Extract samples from data and save them to a npz file.
 
     Args:
         im_size (int): image size
         data (dict): data container
         grid_size (tuple): the grid size
         anchors (list): list of anchors
         labels (list): list of labels
@@ -189,30 +191,25 @@
                                type=float,
                                default=0.5,
                                help="Non-Maximal Suppression threshold.")
 
     parsers = get_training_parser(batch_size=128,
                                   freeze_before=True,
                                   tune=True,
+                                  extract=True,
                                   global_parser=global_parser)
-    subparser = parsers[-1]
-    extract_parser = subparser.add_parser("extract",
-                                          help="Extract samples",
-                                          parents=[global_parser])
-    extract_parser.add_argument("-o", "--out_file", type=str,
-                                default='widerface_samples.npz', help="Name of the output file.")
 
     args = parsers[0].parse_args()
 
     # Load data
     train_data, valid_data, labels, anchors = get_data(args.data,
                                                        args.anchors_path)
 
     # Load the source model
-    base_model = load_quantized_model(args.model)
+    base_model = load_model(args.model)
 
     # Create a final reshape layer for loss computation
     grid_size = base_model.output_shape[1:3]
     output = Reshape(
         (grid_size[1], grid_size[0], len(anchors), 4 + 1 + len(labels)),
         name="YOLO_output")(base_model.output)
 
@@ -229,37 +226,36 @@
         learning_rate = 1e-5
 
     compile_model(model,
                   learning_rate=learning_rate,
                   loss=YoloLoss(anchors, grid_size, args.batch_size),
                   metrics=None)
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action in ["train", "tune"]:
         train(model, train_data, valid_data, anchors, labels, args.obj_thresh,
               args.nms_thresh, args.epochs, args.batch_size, grid_size)
-
-        if args.savemodel:
-            # Remove the last reshape layer introduced for training
-            model = Model(model.input, model.layers[-2].output)
-            # Save the model
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
+        # Remove the last reshape layer introduced for training
+        model = Model(model.input, model.layers[-2].output)
+        save_model(model, args.model, args.savemodel, args.action)
 
     elif args.action == 'eval':
         # Evaluate model accuracy
         if args.akida:
             # Drop the last reshape layer that is not Akida compatible
             if model.layers[-1].name == 'YOLO_output':
                 model = Model(model.input, model.layers[-2].output)
             model = convert(model)
         evaluate(model, valid_data, anchors, labels, args.obj_thresh,
                  args.nms_thresh)
 
     elif args.action == 'extract':
         input_shape = model.input.shape[1:]
         extract_samples(input_shape, train_data, grid_size, anchors,
-                        labels, args.batch_size, args.out_file)
+                        labels, args.batch_size, args.savefile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/distiller.py` & `akida_models-1.2.0/akida_models/distiller.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/dvs/dvs_generator.py` & `akida_models-1.2.0/akida_models/dvs/dvs_generator.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/dvs/dvs_train.py` & `akida_models-1.2.0/akida_models/dvs/dvs_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 import os
 import argparse
 import numpy as np
 import tensorflow as tf
 
 from keras.utils.np_utils import to_categorical
 
-from cnn2snn import load_quantized_model, convert
+from cnn2snn import convert
 
 from ..cyclic_lr import CyclicLR
 from ..training import (get_training_parser, compile_model, evaluate_model, evaluate_akida_model,
-                        print_history_stats, RestoreBest)
+                        print_history_stats, RestoreBest, save_model)
+from ..extract import extract_samples
 from ..utils import fetch_file
+from ..model_io import load_model
 
 
 def get_data(dataset, batch_size):
     """ Loads data.
 
     Dataset parameters for DVSDataGenerator are set from DVS pickles.
 
@@ -44,20 +46,20 @@
         batch_size (int): the batch size
 
     Returns:
         tf.dataset, tf.dataset, int: train dataset, test dataset and number of
         samples.
     """
     # Load pre-processed dataset
-    train_file = fetch_file(os.path.join('http://data.brainchip.com/dataset-mirror',
+    train_file = fetch_file(os.path.join('https://data.brainchip.com/dataset-mirror',
                                          dataset, dataset + '_preprocessed_train.npz'),
                             fname=dataset + '_preprocessed_train.npz',
                             cache_subdir=os.path.join('datasets', dataset))
 
-    test_file = fetch_file(os.path.join('http://data.brainchip.com/dataset-mirror',
+    test_file = fetch_file(os.path.join('https://data.brainchip.com/dataset-mirror',
                                         dataset, dataset + '_preprocessed_test.npz'),
                            fname=dataset + '_preprocessed_test.npz',
                            cache_subdir=os.path.join('datasets', dataset))
     train_data = np.load(train_file)
     x_train = train_data['x_train']
     y_train = to_categorical(train_data['y_train'])
 
@@ -127,47 +129,49 @@
                                type=str,
                                default='dvs_gesture',
                                choices=['dvs_gesture', 'samsung_handy'],
                                help="Dataset name (defaut=dvs_gesture)")
 
     parsers = get_training_parser(batch_size=32,
                                   tune=True,
+                                  extract=True,
                                   global_parser=global_parser)
     args = parsers[0].parse_args()
 
     # Load the source model
-    model = load_quantized_model(args.model)
+    model = load_model(args.model)
 
     # Compile model
     learning_rate = 0.001
     if args.action == 'tune':
         learning_rate = 0.0001
 
     compile_model(model, learning_rate=learning_rate)
 
     # Load data
     train_ds, test_ds, num_samples = get_data(args.dataset, args.batch_size)
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action in ["train", "tune"]:
         train_model(model, train_ds, test_ds, args.batch_size, learning_rate,
                     args.epochs, num_samples)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
         if args.akida:
-            model_ak = convert(model, input_is_image=False)
+            model_ak = convert(model)
             preds, labels = evaluate_akida_model(model_ak, test_ds, 'softmax')
             accuracy = (np.squeeze(np.argmax(preds, 1)) == np.argmax(labels,
                                                                      1)).mean()
             print(f"Akida accuracy: {accuracy}")
         else:
             evaluate_model(model, test_ds)
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, train_ds, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/dvs/model_convtiny_gesture.py` & `akida_models-1.2.0/akida_models/dvs/model_convtiny_handy.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,161 +11,161 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Convtiny model definition for DVS gesture classification.
+Convtiny model definition for DVS handy classification.
 """
 
 from keras import Model
 from keras.layers import Input, Reshape, Dropout, Activation
 
-from cnn2snn import load_quantized_model, quantize
-
 from ..layer_blocks import conv_block, separable_conv_block, dense_block
-from ..utils import fetch_file
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
 
 # Locally fixed config options
 # The number of neurons in the penultimate dense layer
 # This layer has binary output spikes, and could be a bottleneck
 # if care isn't taken to ensure enough info capacity
 NUM_SPIKING_NEURONS = 256
 
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/convtiny/'
-
 
-def convtiny_dvs_gesture(input_shape=(64, 64, 10),
-                         classes=10,
-                         weight_quantization=0,
-                         activ_quantization=0):
-    """Instantiates a CNN for the "IBM DVS Gesture" example.
+def convtiny_dvs_handy(input_shape=(120, 160, 2), classes=9):
+    """Instantiates a CNN for "Brainchip dvs_handy" example.
 
     Args:
-        input_shape (tuple): input shape tuple of the model
-        classes (int, optional): number of classes to classify images into. Defaults to 10.
-        weight_quantization (int): sets all weights in the model to have
-            a particular quantization bitwidth except for the weights in the
-            first layer.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization: sets all activations in the model to have a
-            particular activation quantization bitwidth.
-
-            * '0' implements floating point 32-bit activations.
-            * '1' through '8' implements n-bit weights where n is from 1-8 bits.
+        input_shape (tuple, optional): input shape tuple of the model. Defaults to (120, 160, 2).
+        classes (int, optional): number of classes to classify images into. Defaults to 9.
 
     Returns:
         keras.Model: a Keras convolutional model for DVS Gesture.
     """
 
     img_input = Input(input_shape, name="input")
 
+    # Model version management
+    fused, post_relu_gap, relu_activation = get_params_by_version()
+
     x = conv_block(img_input,
                    filters=16,
                    kernel_size=(3, 3),
-                   name='conv_01',
+                   name='conv_0',
                    use_bias=False,
                    add_batchnorm=True,
                    padding='same',
                    pooling='max',
                    pool_size=(2, 2),
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    strides=(1, 1))
 
     x = conv_block(x,
-                   filters=16,
+                   filters=32,
                    kernel_size=(3, 3),
-                   name='conv_02',
+                   name='conv_1',
                    use_bias=False,
                    add_batchnorm=True,
                    padding='same',
                    pooling='max',
                    pool_size=(2, 2),
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    strides=(1, 1))
 
     x = conv_block(x,
-                   filters=32,
+                   filters=64,
                    kernel_size=(3, 3),
-                   name='conv_03',
+                   name='conv_2',
                    use_bias=False,
                    add_batchnorm=True,
                    padding='same',
                    pooling='max',
                    pool_size=(2, 2),
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    strides=(1, 1))
 
     x = conv_block(x,
-                   filters=64,
+                   filters=128,
                    kernel_size=(3, 3),
-                   name='conv_04',
+                   name='conv_3',
                    use_bias=False,
                    add_batchnorm=True,
                    padding='same',
                    pooling='max',
                    pool_size=(2, 2),
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    strides=(1, 1))
 
     x = conv_block(x,
-                   filters=128,
+                   filters=256,
                    kernel_size=(3, 3),
-                   name='conv_05',
+                   name='conv_4',
                    use_bias=False,
                    add_batchnorm=True,
                    padding='same',
-                   pooling='global_avg',
+                   pooling='max',
                    pool_size=(2, 2),
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    strides=(1, 1))
 
-    bm_outshape = (1, 1, 128)
+    x = conv_block(x,
+                   filters=512,
+                   kernel_size=(3, 3),
+                   name='conv_5',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='global_avg',
+                   relu_activation=relu_activation,
+                   post_relu_gap=post_relu_gap,
+                   strides=(1, 1))
+
+    bm_outshape = (1, 1, 512)
 
     x = Reshape(bm_outshape, name='reshape_1')(x)
     x = Dropout(1e-3, name='dropout')(x)
 
     x = separable_conv_block(x,
                              filters=NUM_SPIKING_NEURONS,
                              kernel_size=(3, 3),
                              use_bias=False,
                              padding='same',
                              name='spiking_layer',
                              add_batchnorm=True,
-                             add_activation=True,
-                             pooling=None)
+                             pooling=None,
+                             relu_activation=relu_activation,
+                             fused=fused)
 
     x = dense_block(x,
                     units=classes,
                     name='dense',
                     add_batchnorm=False,
-                    add_activation=False,
+                    relu_activation=False,
                     use_bias=False)
+
     act_function = 'softmax' if classes > 1 else 'sigmoid'
     x = Activation(act_function, name=f'act_{act_function}')(x)
     x = Reshape((classes,), name='reshape_2')(x)
 
-    model = Model(inputs=img_input, outputs=x, name='dvs_network')
-
-    if ((weight_quantization != 0) or (activ_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization)
-    return model
+    return Model(inputs=img_input, outputs=x, name='dvs_network')
 
 
-def convtiny_gesture_pretrained():
-    """ Helper method to retrieve a `convtiny_dvs_gesture` model that was
-    trained on IBM DVS Gesture dataset.
+def convtiny_handy_samsung_pretrained():
+    """ Helper method to retrieve a `convtiny_dvs_handy` model that was trained
+    on samsung_handy dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'convtiny_dvs_gesture_iq4_wq4_aq4.h5'
-    file_hash = 'ad1a0a2ee13092921a914f25a6159dcb788540239d10ea96d3ff5fefec359281'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v1 = 'convtiny_dvs_handy_samsung_iq4_wq4_aq4.h5'
+    file_hash_v1 = 'ac5dbf1420fbedc402da4394bb22cf94ff5cff73adb428cca741d6550f663c71'
+    model_name_v2 = 'convtiny_dvs_handy_samsung_i4_w4_a4.h5'
+    file_hash_v2 = '29cd8beabcb0576312e8673e8bf7cc41b92f6be82685357f848dfae39a172076'
+    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/dvs/model_convtiny_handy.py` & `akida_models-1.2.0/akida_models/portrait128/model_akida_unet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,184 +1,142 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2020 Brainchip Holdings Ltd.
+# Copyright 2022 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Convtiny model definition for DVS handy classification.
+Akida U-Net model definition for semantic segmentation.
 """
 
-from keras import Model
-from keras.layers import Input, Reshape, Dropout, Activation
+from keras import Model, regularizers
+from keras.layers import Dropout, Activation
 
-from cnn2snn import load_quantized_model, quantize
+from cnn2snn import set_akida_version, AkidaVersion
 
-from ..layer_blocks import conv_block, separable_conv_block, dense_block
+from ..layer_blocks import sepconv_transpose_block, conv_block
+from ..imagenet.model_akidanet import akidanet_imagenet
 from ..utils import fetch_file
+from ..model_io import load_model, get_model_path
 
-# Locally fixed config options
-# The number of neurons in the penultimate dense layer
-# This layer has binary output spikes, and could be a bottleneck
-# if care isn't taken to ensure enough info capacity
-NUM_SPIKING_NEURONS = 256
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/convtiny/'
 
-
-def convtiny_dvs_handy(input_shape=(120, 160, 2),
-                       classes=9,
-                       weight_quantization=0,
-                       activ_quantization=0):
-    """Instantiates a CNN for "Brainchip dvs_handy" example.
+def akida_unet_portrait128(input_shape=(128, 128, 3),
+                           alpha=0.5,
+                           input_scaling=(128, -1)):
+    """Instantiates an Akida U-Net architecture.
+
+    It is composed of an AkidaNet-ImageNet encoder followed by a succession of Conv2DTranspose
+    layers for the decoder part.
+    It does not contain any skip connection (concatenation) between the encoder and the decoder
+    branches.
 
     Args:
-        input_shape (tuple): input shape tuple of the model
-        classes (int, optional): number of classes to classify images into. Defaults to 9.
-        weight_quantization (int): sets all weights in the model to have
-            a particular quantization bitwidth except for the weights in the
-            first layer.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization: sets all activations in the model to have a
-            particular activation quantization bitwidth.
-
-            * '0' implements floating point 32-bit activations.
-            * '1' through '8' implements n-bit weights where n is from 1-8 bits.
+        input_shape (tuple, optional): input shape tuple. Defaults to (128, 128, 3).
+        alpha (float, optional): controls the width (number of filters) of the model. Defaults to
+            0.5.
+        input_scaling (tuple, optional): scale factor and offset to apply to inputs. Defaults to
+            (128, -1). Note that following Akida convention, the scale factor is a number used as a
+            divider.
 
     Returns:
-        keras.Model: a Keras convolutional model for DVS Gesture.
+        keras.Model: a Keras Model instance.
     """
+    # This model is only available for akida 2.0
+    with set_akida_version(AkidaVersion.v2):
+        # Define weight regularization, will apply to pointwise weights of sepconv transposed layers
+        weight_regularizer = regularizers.l2(4e-5)
+
+        # Create an AkidaNet network without top layers
+        encoder = akidanet_imagenet(input_shape=input_shape,
+                                    alpha=alpha,
+                                    include_top=False,
+                                    input_scaling=input_scaling)
+
+        # Add the decoder layers
+        x = encoder.layers[-1].output
+        x = sepconv_transpose_block(x,
+                                    filters=int(512 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_0',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(256 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_1',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(128 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_2',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(64 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_3',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(32 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_4',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = conv_block(x, filters=1, kernel_size=(1, 1), relu_activation=False, name='head')
+        x = Activation('sigmoid', name="sigmoid_act")(x)
 
-    img_input = Input(input_shape, name="input")
+    # Build the whole model: encoder followed by decoder
+    return Model(inputs=encoder.input, outputs=x, name='akida_unet')
 
-    x = conv_block(img_input,
-                   filters=16,
-                   kernel_size=(3, 3),
-                   name='conv_0',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=32,
-                   kernel_size=(3, 3),
-                   name='conv_1',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=64,
-                   kernel_size=(3, 3),
-                   name='conv_2',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=128,
-                   kernel_size=(3, 3),
-                   name='conv_3',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=256,
-                   kernel_size=(3, 3),
-                   name='conv_4',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=512,
-                   kernel_size=(3, 3),
-                   name='conv_5',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='global_avg',
-                   pool_size=(2, 2),
-                   add_activation=True,
-                   strides=(1, 1))
-
-    bm_outshape = (1, 1, 512)
-
-    x = Reshape(bm_outshape, name='reshape_1')(x)
-    x = Dropout(1e-3, name='dropout')(x)
-
-    x = separable_conv_block(x,
-                             filters=NUM_SPIKING_NEURONS,
-                             kernel_size=(3, 3),
-                             use_bias=False,
-                             padding='same',
-                             name='spiking_layer',
-                             add_batchnorm=True,
-                             add_activation=True,
-                             pooling=None)
-
-    x = dense_block(x,
-                    units=classes,
-                    name='dense',
-                    add_batchnorm=False,
-                    add_activation=False,
-                    use_bias=False)
-
-    act_function = 'softmax' if classes > 1 else 'sigmoid'
-    x = Activation(act_function, name=f'act_{act_function}')(x)
-    x = Reshape((classes,), name='reshape_2')(x)
-
-    model = Model(inputs=img_input, outputs=x, name='dvs_network')
-
-    if ((weight_quantization != 0) or (activ_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization)
-    return model
-
-
-def convtiny_handy_samsung_pretrained():
-    """ Helper method to retrieve a `convtiny_dvs_handy` model that was trained
-    on samsung_handy dataset.
+
+def akida_unet_portrait128_pretrained():
+    """
+    Helper method to retrieve an `akida_unet` model that was trained on portrait128 dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'convtiny_dvs_handy_samsung_iq4_wq4_aq4.h5'
-    file_hash = 'ac5dbf1420fbedc402da4394bb22cf94ff5cff73adb428cca741d6550f663c71'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
-                            fname=model_name,
-                            file_hash=file_hash,
+    model_name_v2 = 'akida_unet_portrait128_i8_w8_a8.h5'
+    file_hash_v2 = 'cf5b2eff3b272e3bf3070b36f9e6ca903ac2694b976557053498a72643899a59'
+    model_path, model_name, file_hash = get_model_path("akida_unet", model_name_v2=model_name_v2,
+                                                       file_hash_v2=file_hash_v2)
+    model_path = fetch_file(model_path, fname=model_name, file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/dvs/preprocessing.py` & `akida_models-1.2.0/akida_models/dvs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/gamma_constraint.py` & `akida_models-1.2.0/akida_models/gamma_constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Custom constraint for BatchNormalization layers and a method helper to apply the
 constraint.
 """
 
 import warnings
 
 from keras.models import clone_model
-from keras.utils.generic_utils import custom_object_scope
+from keras.utils import custom_object_scope
 from keras.layers import BatchNormalization
 
 from cnn2snn.min_value_constraint import MinValueConstraint
 
 
 def add_gamma_constraint(model):
     """ Method helper to add a MinValueConstraint to an existing model so that
```

### Comparing `akida_models-1.1.9/akida_models/imagenet/imagenet_labels2names.py` & `akida_models-1.2.0/akida_models/imagenet/imagenet_labels2names.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/imagenet/imagenet_train.py` & `akida_models-1.2.0/akida_models/imagenet/imagenet_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,29 +30,30 @@
     tfds = None
 
 import keras
 from keras.callbacks import LearningRateScheduler
 from keras import Sequential
 from keras.optimizers import SGD, Adam
 from tensorflow_addons.optimizers import LAMB
-from keras.layers import Input, Activation
+from keras.layers import Input
 from keras.models import clone_model
 
 import akida
 from cnn2snn import convert
 from quantizeml.layers import AddPositionEmbs, ClassToken
 
 from .preprocessing import preprocess_image, DATA_AUGMENTATION
-from ..training import (get_training_parser, calibrate_model, freeze_model_before,
-                        print_history_stats, RestoreBest)
-from ..calibrable import calibration_required
+from ..training import (get_training_parser, freeze_model_before, print_history_stats, RestoreBest,
+                        save_model)
+from ..extract import extract_samples
 from ..transformers.model_vit import apply_embedding_weights
 from ..distiller import DeitDistiller
 from ..param_scheduler import get_cosine_lr_scheduler
-from ..utils import get_tensorboard_callback, load_model
+from ..utils import get_tensorboard_callback
+from ..model_io import load_model
 
 
 def get_imagenet_dataset(data_path, training, image_size, batch_size, data_aug=True, one_hot=False):
     """ Loads ImageNet 2012 dataset and builds a tf.dataset out of it.
 
     Args:
         data_path (str): path to the folder containing ImageNet tar files
@@ -139,21 +140,14 @@
     if isinstance(model, DeitDistiller):
         model.compile(optimizer=_get_optim(optimizer),
                       metrics=['accuracy', 'top_k_categorical_accuracy'],
                       student_loss_fn=keras.losses.CategoricalCrossentropy(from_logits=True),
                       distiller_type=distiller_type)
         return True
 
-    # Preserve legacy behavior where models have a softmax activation at the end
-    if isinstance(model.layers[-2], Activation):
-        model.compile(optimizer=_get_optim(optimizer),
-                      loss='sparse_categorical_crossentropy',
-                      metrics=['accuracy', 'sparse_top_k_categorical_accuracy'])
-        return False
-
     model.compile(optimizer=_get_optim(optimizer),
                   loss=keras.losses.CategoricalCrossentropy(from_logits=True),
                   metrics=['accuracy', 'top_k_categorical_accuracy'])
     return True
 
 
 def evaluate(model, val_dataset, batch_size, num_samples, val_steps):
@@ -185,15 +179,15 @@
                 log_samples = batch_size
             print(f"Logging every {log_samples} samples.")
         else:
             log_samples = num_samples
         while cur_samples < num_samples:
             x, y = next(it)
             y_ak = model.predict_classes(x.astype(np.uint8))
-            correct_preds += np.sum(y_ak == y.flatten())
+            correct_preds += np.sum(y_ak == np.argmax(y, -1))
             cur_samples += y_ak.shape[0]
             if cur_samples % log_samples == 0 and cur_samples < num_samples:
                 # Log current accuracy
                 accuracy = correct_preds / cur_samples
                 print(f"Accuracy after {cur_samples}: {accuracy}")
         accuracy = correct_preds / cur_samples
         print(f"Accuracy after {cur_samples}: {accuracy}")
@@ -322,23 +316,18 @@
         learning_rate (float, optional): the learning rate. Defaults to 1e-1.
         initial_epoch (int, optional): epoch at which to start training.
           Defaults to 0.
         lr_policy (str, optional): defines the learning rate policy to adopt. Values in
             ['exp_decay', 'cosine_decay', 'cosine_sched'] for exponential decay, cosine decay and
             cosine oscillation respectively. Defaults to 'exp_decay'.
     """
-    # 1. Check model validity
-    if calibration_required(model):
-        str_action = "tune" if tune else "train"
-        raise ValueError(f"{model.name} model must be calibrated before a {str_action}.")
-
-    # 2. Define training callbacks
+    # 1. Define training callbacks
     callbacks = []
 
-    # 2.1 Learning rate scheduler
+    # 1.1 Learning rate scheduler
     if lr_policy == 'exp_decay':
         LR_START = learning_rate
         LR_END = 1e-4
         # number of epochs you first keep the learning rate constant
         LR_EPOCH_CONSTANT = 10
         # Modify default values for fine-tuning
         if tune:
@@ -387,23 +376,23 @@
         lr_scheduler = LearningRateScheduler(cos_lr_scheduler)
     elif lr_policy == 'cosine_sched':
         lr_scheduler = get_cosine_lr_scheduler(learning_rate, num_epochs * train_steps)
     else:
         raise ValueError(f"Unsupported learning rate policy '{lr_policy}'.")
     callbacks.append(lr_scheduler)
 
-    # 2.2 Model checkpoints (save best model and retrieve it when training is complete)
+    # 1.2 Model checkpoints (save best model and retrieve it when training is complete)
     restore_model = RestoreBest(model)
     callbacks.append(restore_model)
 
-    # 2.3 Tensorboard logs
+    # 1.3 Tensorboard logs
     tensorboard = get_tensorboard_callback(out_dir, prefix='imagenet')
     callbacks.append(tensorboard)
 
-    # 3. Train
+    # 2. Train
     history = model.fit(train_dataset,
                         steps_per_epoch=train_steps,
                         epochs=num_epochs,
                         callbacks=callbacks,
                         validation_data=val_dataset,
                         validation_steps=val_steps,
                         initial_epoch=initial_epoch)
@@ -423,15 +412,15 @@
     global_parser.add_argument("-o",
                                "--out_dir",
                                type=str,
                                default='./logs',
                                help="The output directory (logs, checkpoints).")
 
     parsers = get_training_parser(batch_size=128,
-                                  calibrate=True,
+                                  extract=True,
                                   freeze_before=True,
                                   tune=True,
                                   global_parser=global_parser)
 
     train_parser = parsers[1]
     train_parser.add_argument("-lr",
                               "--learning_rate",
@@ -518,14 +507,15 @@
                                 default=None,
                                 help="Save model with the specified name")
 
     args = parsers[0].parse_args()
 
     # Load the source model
     model = load_model(args.model)
+    im_size = model.input_shape[1]
 
     # Try to load the teacher model, used after to train with Knowledge Distillation
     # Hyperparameters takes from https://arxiv.org/pdf/2012.12877.pdf
     if getattr(args, 'teacher', False):
         if args.distiller_type not in ['none', 'soft', 'hard']:
             raise ValueError("Distiller type must be one of ['none', 'soft', 'hard']")
         teacher = load_model(args.teacher)
@@ -538,28 +528,28 @@
         freeze_model_before(model, args.freeze_before)
 
     # Compile model
     one_hot = compile_model(train_model, optimizer=getattr(args, "optim", "SGD"),
                             distiller_type=getattr(args, "distiller_type", "none"))
 
     # Load validation data
-    if args.action != 'rescale':
-        im_size = model.input_shape[1]
+    if args.action in ['train', 'tune', 'eval']:
         val_ds, val_steps = get_imagenet_dataset(args.data_dir, False, im_size,
                                                  args.batch_size, data_aug=False, one_hot=one_hot)
+    # Load training data
+    if args.action in ['train', 'tune', 'extract']:
+        data_aug = args.data_aug if args.action in ['train', 'tune'] else False
+        train_ds, train_steps = get_imagenet_dataset(args.data_dir, True, im_size,
+                                                     args.batch_size, data_aug, one_hot=one_hot)
 
     # Disable QuantizeML assertions
     os.environ["ASSERT_ENABLED"] = "0"
 
     # Train model
     if args.action in ['train', 'tune']:
-        # Load training data
-        train_ds, train_steps = get_imagenet_dataset(args.data_dir, True,
-                                                     im_size, args.batch_size,
-                                                     args.data_aug, one_hot=one_hot)
         tune = args.action == 'tune'
 
         learning_rate = args.learning_rate
         if args.lr_policy == 'cosine_decay':
             # Tune learning rate following https://arxiv.org/pdf/2012.12877.pdf
             learning_rate *= args.batch_size / 512
 
@@ -570,44 +560,27 @@
               val_steps,
               args.out_dir,
               args.epochs,
               tune=tune,
               learning_rate=learning_rate,
               initial_epoch=args.initial_epoch,
               lr_policy=args.lr_policy)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
+        save_model(model, args.model, args.savemodel, args.action)
 
     elif args.action == 'eval':
         # Evaluate model accuracy
         if args.akida:
             model = convert(model)
         evaluate(model, val_ds, args.batch_size, args.num_samples, val_steps)
 
     elif args.action == 'rescale':
         # Rescale model
         m = rescale(model, args.input_size)
+        save_model(m, args.model, args.savemodel, args.action)
 
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            m.save(args.savemodel, include_optimizer=False)
-            print(f"Rescaled model saved as {args.savemodel}")
-
-    elif args.action == "calibrate":
-        # Calibrate model
-        # Load training data without data augmentation
-        train_ds, train_steps = get_imagenet_dataset(args.data_dir, True,
-                                                     im_size, args.batch_size,
-                                                     False, one_hot=one_hot)
-        calibrate_model(model, train_ds, args.num_samples, args.batch_size, args.epochs)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Calibrated model saved as {args.savemodel}")
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, train_ds, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/imagenet/imagenet_utils.py` & `akida_models-1.2.0/akida_models/imagenet/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/imagenet/model_akidanet_edge.py` & `akida_models-1.2.0/akida_models/imagenet/model_akidanet_edge.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,112 +17,125 @@
 """
 This model is an adaptation of the `akidanet_imagenet` model for edge
 applications. It is based on AkidaNet with top layers replaced by a quantized
 spike extractor and a classification layer.
 """
 
 from keras import Model
-from keras.layers import Reshape, Activation
+from keras.layers import Reshape
 
-from cnn2snn import load_quantized_model, quantize_layer
+from cnn2snn import quantize_layer, get_akida_version, AkidaVersion
 
 from ..layer_blocks import separable_conv_block, dense_block
-from ..utils import fetch_file
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
 
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/akidanet_edge/'
 
-
-def akidanet_edge_imagenet(base_model, classes):
+def akidanet_edge_imagenet(base_model, classes, base_layer="classifier"):
     """Instantiates an AkidaNet-edge architecture.
 
     Args:
-        base_model (str/keras.Model): an akidanet_imagenet quantized model.
+        base_model (str/keras.Model): an akidanet_imagenet base model.
         classes (int): the number of classes for the edge classifier.
+        base_layer (str, optional): the last base layer. Defaults to "classifier".
 
     Returns:
         keras.Model: a Keras Model instance.
     """
     if isinstance(base_model, str):
-        base_model = load_quantized_model(base_model)
+        base_model = load_model(base_model)
 
+    is_v1 = get_akida_version() == AkidaVersion.v1
     try:
-        # Identify the last separable, which is the base model classifier
-        base_classifier = base_model.get_layer("separable_14")
-        # remember the classifier weight bitwidth
-        wq = base_classifier.quantizer.bitwidth
+        # Identify the base model classifier
+        base_classifier = base_model.get_layer(base_layer)
+        if is_v1:
+            # remember the classifier weight bitwidth
+            wq = base_classifier.quantizer.bitwidth
     except Exception as e:
-        raise ValueError("The base model is not a quantized \
-                          AkidaNet/Imagenet model") from e
+        raise ValueError("The base model is not a quantized AkidaNet/Imagenet model") from e
+
+    # Model version management
+    fused, _, _ = get_params_by_version()
 
     # Recreate a model with all layers up to the classifier
     x = base_classifier.input
-    # Add the new end layer with kernel_size (3, 3) instead of (1,1) for
+    x = Reshape((1, 1, x.shape[-1]))(x)
+    # Add the new end layer with kernel_size (3, 3) instead of (1, 1) for
     # hardware compatibility reasons
+    # Because it will be quantized to 1 bit, the ReLU max_value should be set to 1
     x = separable_conv_block(x,
                              filters=2048,
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
                              name='spike_generator',
-                             add_activation=True)
+                             fused=fused,
+                             relu_activation='ReLU1')
 
     # Then add the Akida edge learning layer that will be dropped after
     x = dense_block(x,
                     classes,
                     name="classification_layer",
-                    add_activation=False,
+                    relu_activation=False,
                     add_batchnorm=False,
                     use_bias=False)
-    act_function = 'softmax' if classes > 1 else 'sigmoid'
-    x = Activation(act_function, name=f'act_{act_function}')(x)
-    x = Reshape((classes,), name='reshape_2')(x)
+    x = Reshape((classes,), name="reshape_3")(x)
 
     # Create model
     model = Model(inputs=base_model.input,
                   outputs=x,
                   name=f"{base_model.name}_edge")
 
-    # Quantize edge layers
-    model = quantize_layer(model, 'spike_generator', wq)
-    model = quantize_layer(model, 'spike_generator/relu', 1)
-    # NOTE: quantization set to 2 here, to be as close as
-    # possible to the Akida native layer that will replace this one,
-    # with binary weights.
-    model = quantize_layer(model, 'classification_layer', 2)
+    # When targeting Akida V1, edge layers can be quantized and tuned which is not the case for V2
+    # (float head training is required).
+    if is_v1:
+        # Quantize edge layers
+        model = quantize_layer(model, 'spike_generator', wq)
+        model = quantize_layer(model, 'spike_generator/relu', 1)
+        # NOTE: quantization set to 2 here, to be as close as
+        # possible to the Akida native layer that will replace this one,
+        # with binary weights.
+        model = quantize_layer(model, 'classification_layer', 2)
 
     return model
 
 
 def akidanet_edge_imagenet_pretrained():
     """ Helper method to retrieve a `akidanet_edge_imagenet` model that was
     trained on ImageNet dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'akidanet_imagenet_224_alpha_50_edge_iq8_wq4_aq4.h5'
-    file_hash = '6c5361533c7bc94133936d799eae36414d66ec40f5a13429dfc3de3734b97bd6'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v1 = 'akidanet_imagenet_224_alpha_50_edge_iq8_wq4_aq4.h5'
+    file_hash_v1 = '71ffc3acb09e5682e479505f6b288bd2736311ce46d3974bdf7b2c02916e52a8'
+    model_path, model_name, file_hash = get_model_path("akidanet_edge", model_name_v1, file_hash_v1)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
 
 
 def akidanet_faceidentification_edge_pretrained():
     """
     Helper method to retrieve an `akidanet_edge_imagenet` model that was trained
     on CASIA Webface dataset and that performs face identification.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'akidanet_faceidentification_edge_iq8_wq4_aq4.h5'
-    file_hash = '61838682cc88cec6dc9a347f1a301bfa9e94fbcbc7a52a273789259de07d3104'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v1 = 'akidanet_faceidentification_edge_iq8_wq4_aq4.h5'
+    file_hash_v1 = '61838682cc88cec6dc9a347f1a301bfa9e94fbcbc7a52a273789259de07d3104'
+    model_name_v2 = 'akidanet_faceidentification_edge_i8_w4_a4.h5'
+    file_hash_v2 = '2b0fed9bb88674ebba2925cdd76c26232c418d43b7e05b8ba8121861fcc49137'
+    model_path, model_name, file_hash = get_model_path("akidanet_edge", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/imagenet/model_mobilenet.py` & `akida_models-1.2.0/akida_models/imagenet/model_mobilenet.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,35 +24,29 @@
     - overall architecture compatible with Akida (conv stride 2 replaced with
      max pool),
     - options to quantize weights and activations,
     - different initialization options.
 """
 
 from keras import Model, regularizers
-from keras.layers import (Input, Reshape, Dropout, Activation, Rescaling)
-
-from cnn2snn import load_quantized_model, quantize
+from keras.layers import Input, Dropout, Rescaling
 
 from .imagenet_utils import obtain_input_shape
-from ..layer_blocks import conv_block, separable_conv_block
-from ..utils import fetch_file
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/mobilenet/'
+from ..layer_blocks import conv_block, separable_conv_block, dense_block
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
 
 
 def mobilenet_imagenet(input_shape=None,
                        alpha=1.0,
                        dropout=1e-3,
                        include_top=True,
                        pooling=None,
                        classes=1000,
-                       use_stride2=False,
-                       weight_quantization=0,
-                       activ_quantization=0,
-                       input_weight_quantization=None,
+                       use_stride2=True,
                        input_scaling=(128, -1)):
     """Instantiates the MobileNet architecture.
 
     Args:
         input_shape (tuple, optional): shape tuple. Defaults to None.
         alpha (float, optional): controls the width of the model.
             Defaults to 1.0.
@@ -74,46 +68,27 @@
               output of the last convolutional block.
             * `avg` means that global average pooling will be applied to the
               output of the last convolutional block, and thus the output of the
               model will be a 2D tensor.
         classes (int, optional): optional number of classes to classify images
             into, only to be specified if `include_top` is `True`. Defaults to 1000.
         use_stride2 (bool, optional): replace max pooling operations by stride 2
-            convolutions in layers separable 2, 4, 6 and 12. Defaults to False.
-        weight_quantization (int, optional): sets all weights in the model to have
-            a particular quantization bitwidth except for the weights in the
-            first layer.
-            Defaults to 0.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization (int, optional): sets all activations in the model to have a
-            particular activation quantization bitwidth.
-            Defaults to 0.
-
-            * '0' implements floating point 32-bit activations.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        input_weight_quantization (int, optional): sets weight quantization in the first layer.
-            Defaults to weight_quantization value.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
+            convolutions in layers separable 2, 4, 6 and 12. Defaults to True.
         input_scaling (tuple, optional): scale factor and offset to apply to
             inputs. Defaults to (128, -1). Note that following Akida convention,
             the scale factor is an integer used as a divider.
 
     Returns:
         keras.Model: a Keras model for MobileNet/ImageNet.
 
     Raises:
         ValueError: in case of invalid input shape.
     """
-    # check if overrides have been provided and override
-    if input_weight_quantization is None:
-        input_weight_quantization = weight_quantization
+    # Model version management
+    fused, post_relu_gap, relu_activation = get_params_by_version(relu_v2='ReLU7.5')
 
     # Define weight regularization, will apply to the first convolutional layer
     # and to all pointwise weights of separable convolutional layers.
     weight_regularizer = regularizers.l2(4e-5)
 
     # Define stride 2 or max pooling
     if use_stride2:
@@ -155,187 +130,184 @@
                    filters=int(32 * alpha),
                    name='conv_0',
                    kernel_size=(3, 3),
                    padding='same',
                    use_bias=False,
                    strides=2,
                    add_batchnorm=True,
-                   add_activation=True,
+                   relu_activation=relu_activation,
                    kernel_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(64 * alpha),
                              name='separable_1',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(128 * alpha),
                              name='separable_2',
                              kernel_size=(3, 3),
                              padding='same',
                              pooling=sep_conv_pooling,
                              strides=strides,
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(128 * alpha),
                              name='separable_3',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(256 * alpha),
                              name='separable_4',
                              kernel_size=(3, 3),
                              padding='same',
                              pooling=sep_conv_pooling,
                              strides=strides,
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(256 * alpha),
                              name='separable_5',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_6',
                              kernel_size=(3, 3),
                              padding='same',
                              pooling=sep_conv_pooling,
                              strides=strides,
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_7',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_8',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_9',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_10',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(512 * alpha),
                              name='separable_11',
                              kernel_size=(3, 3),
                              padding='same',
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     x = separable_conv_block(x,
                              filters=int(1024 * alpha),
                              name='separable_12',
                              kernel_size=(3, 3),
                              padding='same',
                              pooling=sep_conv_pooling,
                              strides=strides,
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
                              pointwise_regularizer=weight_regularizer)
 
     # Last separable layer with global pooling
     layer_pooling = 'global_avg' if include_top or pooling == 'avg' else None
     x = separable_conv_block(x,
                              filters=int(1024 * alpha),
                              name='separable_13',
                              kernel_size=(3, 3),
                              padding='same',
                              pooling=layer_pooling,
                              use_bias=False,
                              add_batchnorm=True,
-                             add_activation=True,
+                             relu_activation=relu_activation,
+                             fused=fused,
+                             post_relu_gap=post_relu_gap,
                              pointwise_regularizer=weight_regularizer)
 
     if include_top:
-        shape = (1, 1, int(1024 * alpha))
-
-        x = Reshape(shape, name='reshape_1')(x)
         x = Dropout(dropout, name='dropout')(x)
-
-        x = separable_conv_block(x,
-                                 filters=classes,
-                                 name='separable_14',
-                                 kernel_size=(3, 3),
-                                 padding='same',
-                                 use_bias=False,
-                                 add_batchnorm=False,
-                                 add_activation=False,
-                                 pointwise_regularizer=weight_regularizer)
-        act_function = 'softmax' if classes > 1 else 'sigmoid'
-        x = Activation(act_function, name=f'act_{act_function}')(x)
-        x = Reshape((classes,), name='reshape_2')(x)
+        x = dense_block(x,
+                        units=classes,
+                        name='classifier',
+                        use_bias=False,
+                        add_batchnorm=False,
+                        relu_activation=False,
+                        kernel_regularizer=weight_regularizer)
 
     # Create model.
-    model = Model(img_input,
-                  x,
-                  name='mobilenet_%0.2f_%s_%s' % (alpha, rows, classes))
-
-    if ((weight_quantization != 0) or (activ_quantization != 0) or
-            (input_weight_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization,
-                        input_weight_quantization)
-    return model
+    return Model(img_input, x, name='mobilenet_%0.2f_%s_%s' % (alpha, rows, classes))
 
 
 def mobilenet_imagenet_pretrained(alpha=1.0):
     """
     Helper method to retrieve a `mobilenet_imagenet` model that was trained on
     ImageNet dataset.
 
@@ -343,24 +315,32 @@
         alpha (float): width of the model.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
     if alpha == 1.0:
-        model_name = 'mobilenet_imagenet_224_iq8_wq4_aq4.h5'
-        file_hash = '242a5d6e155f9677e4a295d6c0b092061ab442bd2c51898663d818b706fc2c34'
+        model_name_v1 = 'mobilenet_imagenet_224_iq8_wq4_aq4.h5'
+        file_hash_v1 = '4e63ea329b3f2f773a0b9d6fef4e449639fda89d17e48bb7132b6ad86585c867'
+        model_name_v2 = 'mobilenet_imagenet_224_alpha_1_i8_w4_a4.h5'
+        file_hash_v2 = 'da329c8b6836c141a7b836875dbcabd36d8efd5b90d9719f50e2d4facea4868a'
     elif alpha == 0.5:
-        model_name = 'mobilenet_imagenet_224_alpha_50_iq8_wq4_aq4.h5'
-        file_hash = 'aa8fec3c21455dbb16dc86063ea07fcba792dcdaf8293c58db42dc379c78afc1'
+        model_name_v1 = 'mobilenet_imagenet_224_alpha_50_iq8_wq4_aq4.h5'
+        file_hash_v1 = '6a5c51cb1a5ae022f2c025affb4022842078dbbb970fb07fdc9fd9e0eb1acd2f'
+        model_name_v2 = 'mobilenet_imagenet_224_alpha_0.5_i8_w4_a4.h5'
+        file_hash_v2 = 'c7277a7850c777a39c90023a7c509696bc7a2cb61590d3c88841f1ee3bc14003'
     elif alpha == 0.25:
-        model_name = 'mobilenet_imagenet_224_alpha_25_iq8_wq4_aq4.h5'
-        file_hash = '2765b8b24e880f593dbb18d73e8750e51a3dfc8f38f2978d9d6679e3f970466a'
+        model_name_v1 = 'mobilenet_imagenet_224_alpha_25_iq8_wq4_aq4.h5'
+        file_hash_v1 = '35ad51e662ed04b68978865ccb1c16bf024fa013146488b2a9c18c80d1efab29'
+        model_name_v2 = 'mobilenet_imagenet_224_alpha_0.25_i8_w4_a4.h5'
+        file_hash_v2 = '29eb66a023fa808735e66f3716e3a8d6429a5d9621e6ed875de4fc8104682a14'
     else:
         raise ValueError(
             f"Requested model with alpha={alpha} is not available.")
 
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_path, model_name, file_hash = get_model_path("mobilenet", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/imagenet/model_vgg.py` & `akida_models-1.2.0/akida_models/modelnet40/model_pointnet_plus.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,225 +11,185 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-VGG model definition for ImageNet classification.
+PointNet++ model definition for ModelNet40 classification.
 """
 
-from keras import Model, regularizers
-from keras.layers import (Input, Activation, Dropout, Flatten, Rescaling)
+from keras import layers, Model, regularizers
 
-from cnn2snn import quantize, load_quantized_model
-
-from ..layer_blocks import conv_block, dense_block
-from ..utils import fetch_file
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/vgg/'
-
-
-def vgg_imagenet(input_shape=(224, 224, 3),
-                 classes=1000,
-                 include_top=True,
-                 pooling=None,
-                 weight_quantization=0,
-                 activ_quantization=0,
-                 input_weight_quantization=None,
-                 input_scaling=(128, -1)):
-    """Instantiates a VGG11 architecture with reduced number of filters in
-    convolutional layers (i.e. a quarter of the filters of the original
-    implementation of https://arxiv.org/pdf/1409.1556.pdf).
+from .pointnet_utils import get_reshape_factor
+from ..layer_blocks import conv_block, dense_block, act_to_layer
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
+
+
+def pointnet_plus_modelnet40(selected_points=128, features=3, knn_points=64, classes=40, alpha=1.0):
+    """ Instantiates a PointNet++ model for the ModelNet40 classification.
+
+    This example implements the point cloud deep learning paper
+    `PointNet (Qi et al., 2017) <https://arxiv.org/abs/1612.00593>`_. For a
+    detailed introduction on PointNet see `this blog post
+    <https://medium.com/@luis_gonzales/an-in-depth-look-at-pointnet-111d7efdaa1a>`_.
+
+    PointNet++ is conceived as a repeated series of operations: sampling and
+    grouping of points, followed by the trainable convnet itself. Those
+    operations are then repeated at increased scale.
+    Each of the selected points is taken as the centroid of the K-nearest
+    neighbours. This defines a localized group.
 
     Args:
-        input_shape (tuple, optional): input shape tuple. Defaults to (224, 224,
-            3).
-        classes (int, optional): optional number of classes to classify images
-            into. Defaults to 1000.
-        include_top (bool, optional): whether to include the classification
-            layers at the top of the model. Defaults to True.
-        pooling (str, optional): Optional pooling mode for feature extraction
-            when `include_top` is `False`. Defaults to None.
-
-            * `None` means that the output of the model will be the 4D tensor
-              output of the last convolutional block.
-            * `avg` means that global average pooling will be applied to the
-              output of the last convolutional block, and thus the output of the
-              model will be a 2D tensor.
-        weight_quantization (int, optional): sets all weights in the model to
-            have a particular quantization bitwidth except for the weights in
-            the first layer. Defaults to 0.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization (int, optional): sets all activations in the model to
-            have a particular activation quantization bitwidth. Defaults to 0.
-
-            * '0' implements floating point 32-bit activations.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        input_weight_quantization(int, optional): sets weight quantization in
-            the first layer. Defaults to weight_quantization value.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        input_scaling (tuple, optional): scale factor and offset to apply to
-            inputs. Defaults to (128, -1). Note that following Akida convention,
-            the scale factor is an integer used as a divider.
+        selected_points (int, optional): the number of points to process per
+            sample. Default is 128.
+        features (int, optional): the number of features. Expected values are
+            1 or 3. Default is 3.
+        knn_points (int, optional): the number of points to include in each
+            localised group. Must be a power of 2, and ideally an integer square
+            (so 64, or 16 for a deliberately small network, or 256 for large).
+            Default is 64.
+        classes (int, optional): the number of classes for the classifier.
+            Default is 40.
+        alpha (float, optional): network filters multiplier. Default is 1.0.
 
     Returns:
-        keras.Model: a Keras model for VGG/ImageNet
-
+        keras.Model: a quantized Keras model for PointNet++/ModelNet40.
     """
-    # check if overrides have been provided and override
-    if input_weight_quantization is None:
-        input_weight_quantization = weight_quantization
-
-    # Define weight regularization
-    weight_regularizer = regularizers.l2(4e-5)
-
-    img_input = Input(shape=input_shape, name="input")
-
-    if input_scaling is None:
-        x = img_input
-    else:
-        scale, offset = input_scaling
-        x = Rescaling(1. / scale, offset, name="rescaling")(img_input)
+    # Model version management
+    _, post_relu_gap, relu_activation = get_params_by_version()
+
+    # Adapt input shape with preprocessing
+    reshape_factor = get_reshape_factor(knn_points)
+    input_shape = (selected_points * reshape_factor,
+                   knn_points // reshape_factor, features)
+
+    inputs = layers.Input(shape=input_shape, name="input")
+    base_filter_num = round(32 * alpha)
+    reg = regularizers.l1_l2(1e-7, 1e-7)
+
+    # Rescale [0, 255] inputs to [-1, 1]
+    x = layers.Rescaling(1./127, -1, name="rescaling")(inputs)
 
     # Block 1
     x = conv_block(x,
-                   filters=16,
+                   filters=base_filter_num,
                    name='block_1/conv_1',
                    kernel_size=(3, 3),
                    padding='same',
-                   kernel_regularizer=weight_regularizer,
                    add_batchnorm=True,
-                   add_activation=True,
-                   pooling='max',
-                   pool_size=(2, 2))
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_1/conv_1/relu_1')(x)
+
+    x = conv_block(x,
+                   filters=base_filter_num,
+                   name='block_1/conv_2',
+                   kernel_size=(1, 1),
+                   padding='same',
+                   add_batchnorm=True,
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_1/conv_2/relu_1')(x)
+    x = layers.MaxPool2D(padding='same', name='max_pooling2d')(x)
 
     # Block 2
     x = conv_block(x,
-                   filters=32,
+                   filters=base_filter_num * 2,
                    name='block_2/conv_1',
-                   kernel_size=(3, 3),
+                   kernel_size=(1, 1),
+                   padding='same',
+                   add_batchnorm=True,
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_2/conv_1/relu_1')(x)
+    x = conv_block(x,
+                   filters=base_filter_num * 2,
+                   name='block_2/conv_2',
+                   kernel_size=(1, 1),
                    padding='same',
-                   kernel_regularizer=weight_regularizer,
                    add_batchnorm=True,
-                   add_activation=True,
-                   pooling='max',
-                   pool_size=(2, 2))
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_2/conv_2/relu_1')(x)
+    if knn_points >= 8:
+        x = layers.MaxPool2D(padding='same', name='max_pooling2d_1')(x)
 
     # Block 3
     x = conv_block(x,
-                   filters=64,
+                   filters=base_filter_num * 4,
                    name='block_3/conv_1',
-                   kernel_size=(3, 3),
+                   kernel_size=(1, 1),
                    padding='same',
-                   kernel_regularizer=weight_regularizer,
                    add_batchnorm=True,
-                   add_activation=True)
-
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_3/conv_1/relu_1')(x)
     x = conv_block(x,
-                   filters=64,
+                   filters=base_filter_num * 4,
                    name='block_3/conv_2',
-                   kernel_size=(3, 3),
+                   kernel_size=(1, 1),
                    padding='same',
-                   kernel_regularizer=weight_regularizer,
                    add_batchnorm=True,
-                   add_activation=True,
-                   pooling='max',
-                   pool_size=(2, 2))
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_3/conv_2/relu_1')(x)
+    if knn_points >= 32:
+        x = layers.MaxPool2D(padding='same', name='max_pooling2d_2')(x)
 
     # Block 4
     x = conv_block(x,
-                   filters=128,
+                   filters=base_filter_num * 8,
                    name='block_4/conv_1',
-                   kernel_size=(3, 3),
-                   padding='same',
-                   kernel_regularizer=weight_regularizer,
-                   add_batchnorm=True,
-                   add_activation=True)
-
-    x = conv_block(x,
-                   filters=128,
-                   name='block_4/conv_2',
-                   kernel_size=(3, 3),
+                   kernel_size=(1, 1),
                    padding='same',
-                   kernel_regularizer=weight_regularizer,
                    add_batchnorm=True,
-                   add_activation=True,
-                   pooling='max',
-                   pool_size=(2, 2))
+                   relu_activation=False)
+    x = act_to_layer(relu_activation, activity_regularizer=reg, name='block_4/conv_1/relu_1')(x)
+    if knn_points >= 128:
+        x = layers.MaxPool2D(padding='same', name='max_pooling2d_3')(x)
 
     # Block 5
     x = conv_block(x,
-                   filters=128,
+                   filters=base_filter_num * 16,
                    name='block_5/conv_1',
-                   kernel_size=(3, 3),
-                   padding='same',
-                   kernel_regularizer=weight_regularizer,
-                   add_batchnorm=True,
-                   add_activation=True)
+                   kernel_size=(1, 1),
+                   pooling='global_avg',
+                   post_relu_gap=post_relu_gap,
+                   padding='same',
+                   add_batchnorm=True)
+
+    # Block 6
+    x = layers.Reshape((1, 1, x.shape[-1]))(x)
+    x = dense_block(x,
+                    units=base_filter_num * 16,
+                    name='fc_1',
+                    relu_activation=relu_activation,
+                    add_batchnorm=True)
+    x = dense_block(x,
+                    units=base_filter_num * 8,
+                    name='fc_2',
+                    relu_activation=relu_activation,
+                    add_batchnorm=True)
+    x = layers.Dense(classes, activation=None, name="dense")(x)
+    act_function = 'softmax' if classes > 1 else 'sigmoid'
+    x = layers.Activation(act_function, name=f'act_{act_function}')(x)
+    outputs = layers.Reshape((classes,))(x)
 
-    layer_pooling = 'global_avg' if pooling == 'avg' else 'max'
-    x = conv_block(x,
-                   filters=128,
-                   name='block_5/conv_2',
-                   kernel_size=(3, 3),
-                   padding='same',
-                   kernel_regularizer=weight_regularizer,
-                   add_batchnorm=True,
-                   add_activation=True,
-                   pooling=layer_pooling,
-                   pool_size=(2, 2))
-
-    if include_top:
-        # Classification block
-        x = Flatten(name='flatten')(x)
-        x = dense_block(x,
-                        units=4096,
-                        name='fc_1',
-                        add_batchnorm=True,
-                        add_activation=True)
-        x = Dropout(0.5, name='dropout_1')(x)
-        x = dense_block(x,
-                        units=4096,
-                        name='fc_2',
-                        add_batchnorm=True,
-                        add_activation=True)
-        x = Dropout(0.5, name='dropout_2')(x)
-        x = dense_block(x,
-                        units=classes,
-                        name='predictions',
-                        add_batchnorm=False,
-                        add_activation=False)
-
-        act_function = 'softmax' if classes > 1 else 'sigmoid'
-        x = Activation(act_function, name=f'act_{act_function}')(x)
-
-    # Create model
-    model = Model(img_input, x, name='vgg11_%s_%s' % (input_shape[0], classes))
-
-    if ((weight_quantization != 0) or (activ_quantization != 0) or
-            (input_weight_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization,
-                        input_weight_quantization)
-    return model
+    return Model(inputs=inputs, outputs=outputs, name="pointnet_plus")
 
 
-def vgg_imagenet_pretrained():
+def pointnet_plus_modelnet40_pretrained():
     """
-    Helper method to retrieve a `vgg_imagenet` model that was trained on
-    ImageNet dataset.
+    Helper method to retrieve a `pointnet_plus` model that was trained on
+    ModelNet40 dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
-
     """
-    model_name = 'vgg11_imagenet_224_iq8_wq4_aq4.h5'
-    file_hash = '40fe5e7fdf083604d3bbe8eba314a832d1dc1f218a743bef244ff6ce2f3c9bfe'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v1 = 'pointnet_plus_modelnet40_iq8_wq4_aq4.h5'
+    file_hash_v1 = '9a49fcdf4742f0bfefb6e16c006d66d4064d9fc0ee30abc1bbd2341f5c5f8fec'
+    model_name_v2 = 'pointnet_plus_modelnet40_i8_w4_a4.h5'
+    file_hash_v2 = 'b4f0ae9a25e2f5ee6068ed5818ac839359dfb5e9e4af880479a70338dc08734b'
+    model_path, model_name, file_hash = get_model_path("pointnet_plus", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/imagenet/preprocessing.py` & `akida_models-1.2.0/akida_models/imagenet/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 
 import numpy as np
 import keras
 import tensorflow as tf
 import tensorflow_addons as tfa
 
-from akida_models.imagenet.imagenet_labels2names import imagenet_labels
+from .imagenet_labels2names import imagenet_labels
 
 
 class RandomColorJitter(keras.layers.Layer):
     """RandomColorJitter class.
 
     Randomly adds color jitter to an image. Color jitter means to add random brightness, contrast,
     saturation, and hue to an image. There is a 80% chance that an image will be randomly
```

### Comparing `akida_models-1.1.9/akida_models/kws/kws_train.py` & `akida_models-1.2.0/akida_models/kws/kws_train.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,31 +19,33 @@
 """
 
 import os
 import pickle
 
 from keras.utils.np_utils import to_categorical
 
-from cnn2snn import load_quantized_model, quantize_layer, convert
+from cnn2snn import quantize_layer, convert
 
 from ..cyclic_lr import CyclicLR
-from ..training import (get_training_parser, calibrate_model, compile_model, evaluate_model,
-                        print_history_stats, RestoreBest)
+from ..training import (get_training_parser, compile_model, evaluate_model, print_history_stats,
+                        RestoreBest, save_model)
+from ..extract import extract_samples
 from ..utils import fetch_file
+from ..model_io import load_model
 
 
 def get_data():
     """ Loads KWS data.
 
     Returns:
         tuple: train data, train labels, validation data and validation labels
     """
     # Load pre-processed dataset
     fname = fetch_file(
-        'http://data.brainchip.com/dataset-mirror/kws/kws_preprocessed_all_words_except_backward_follow_forward.pkl',
+        'https://data.brainchip.com/dataset-mirror/kws/kws_preprocessed_all_words_except_backward_follow_forward.pkl',
         fname='kws_preprocessed_all_words_except_backward_follow_forward.pkl',
         cache_subdir=os.path.join('datasets', 'kws'))
 
     print('Loading pre-processed dataset...')
     with open(fname, 'rb') as f:
         [x_train, y_train, x_val, y_val, _, _, _, _] = pickle.load(f)
 
@@ -93,65 +95,53 @@
                         callbacks=callbacks)
     print_history_stats(history)
 
 
 def main():
     """ Entry point for script and CLI usage.
     """
-    parsers = get_training_parser(calibrate=True, batch_size=100, global_batch_size=False)
+    parsers = get_training_parser(batch_size=100, global_batch_size=False, extract=True)
 
     train_parser = parsers[1]
     train_parser.add_argument("-laq",
                               "--last_activ_quantization",
                               type=int,
                               default=None,
                               help="The last layer activation quantization")
 
     args = parsers[0].parse_args()
 
     # Load the source model
-    model = load_quantized_model(args.model)
+    model = load_model(args.model)
 
     # If specified, change the last layer activation bitwidth
     if "last_activ_quantization" in args and args.last_activ_quantization:
         model = quantize_layer(model, 'separable_4/relu', args.last_activ_quantization)
 
     # Compile model
     compile_model(model, learning_rate=2e-3)
 
     # Load data
     x_train, y_train, x_val, y_val = get_data()
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action == "train":
-        train_model(model, x_train, y_train, x_val, y_val, args.batch_size,
-                    args.epochs)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        train_model(model, x_train, y_train, x_val, y_val, args.batch_size, args.epochs)
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
         if args.akida:
             model_ak = convert(model)
             accuracy = model_ak.evaluate(x_val.astype('uint8'), y_val)
             print(f"Accuracy: {accuracy}")
         else:
             evaluate_model(model, x_val, y=to_categorical(y_val))
-
-    elif args.action == "calibrate":
-        # Calibrate model
-        calibrate_model(model,
-                        x_train,
-                        num_samples=args.num_samples,
-                        batch_size=args.batch_size,
-                        epochs=args.epochs)
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Calibrated model saved as {args.savemodel}")
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, x_train, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/kws/preprocessing.py` & `akida_models-1.2.0/akida_models/kws/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 RANDOM_SEED = 59185
 
 
 def prepare_model_settings(sample_rate, clip_duration_ms, window_size_ms,
                            window_stride_ms, feature_bin_count):
     """Calculates common settings needed for all models.
 
-  Args:
-    sample_rate: Number of audio samples per second.
-    clip_duration_ms: Length of each audio clip to be analyzed.
-    window_size_ms: Duration of frequency analysis window.
-    window_stride_ms: How far to move in time between frequency windows.
-    feature_bin_count: Number of frequency bins to use for analysis.
-
-  Returns:
-    Dictionary containing common settings.
-
-  Raises:
-    ValueError: If the preprocessing mode isn't recognized.
-  """
+    Args:
+        sample_rate: Number of audio samples per second.
+        clip_duration_ms: Length of each audio clip to be analyzed.
+        window_size_ms: Duration of frequency analysis window.
+        window_stride_ms: How far to move in time between frequency windows.
+        feature_bin_count: Number of frequency bins to use for analysis.
+
+    Returns:
+        Dictionary containing common settings.
+
+    Raises:
+        ValueError: If the preprocessing mode isn't recognized.
+    """
     desired_samples = int(sample_rate * clip_duration_ms / 1000)
     window_size_samples = int(sample_rate * window_size_ms / 1000)
     window_stride_samples = int(sample_rate * window_stride_ms / 1000)
     length_minus_window = (desired_samples - window_size_samples)
     if length_minus_window < 0:
         spectrogram_length = 0
     else:
@@ -82,46 +82,46 @@
         'fingerprint_size': fingerprint_size,
     }
 
 
 def prepare_words_list(wanted_words):
     """Prepends common tokens to the custom word list.
 
-  Args:
-    wanted_words: List of strings containing the custom words.
+    Args:
+        wanted_words: List of strings containing the custom words.
 
-  Returns:
-    List with the standard silence and unknown tokens added.
-  """
+    Returns:
+        List with the standard silence and unknown tokens added.
+    """
     return [SILENCE_LABEL, UNKNOWN_WORD_LABEL] + wanted_words
 
 
 def which_set(filename, validation_percentage, testing_percentage):
     """Determines which data partition the file should belong to.
 
-  We want to keep files in the same training, validation, or testing sets even
-  if new ones are added over time. This makes it less likely that testing
-  samples will accidentally be reused in training when long runs are restarted
-  for example. To keep this stability, a hash of the filename is taken and used
-  to determine which set it should belong to. This determination only depends on
-  the name and the set proportions, so it won't change as other files are added.
-
-  It's also useful to associate particular files as related (for example words
-  spoken by the same person), so anything after '_nohash_' in a filename is
-  ignored for set determination. This ensures that 'bobby_nohash_0.wav' and
-  'bobby_nohash_1.wav' are always in the same set, for example.
-
-  Args:
-    filename: File path of the data sample.
-    validation_percentage: How much of the data set to use for validation.
-    testing_percentage: How much of the data set to use for testing.
-
-  Returns:
-    String, one of 'training', 'validation', or 'testing'.
-  """
+    We want to keep files in the same training, validation, or testing sets even
+    if new ones are added over time. This makes it less likely that testing
+    samples will accidentally be reused in training when long runs are restarted
+    for example. To keep this stability, a hash of the filename is taken and used
+    to determine which set it should belong to. This determination only depends on
+    the name and the set proportions, so it won't change as other files are added.
+
+    It's also useful to associate particular files as related (for example words
+    spoken by the same person), so anything after '_nohash_' in a filename is
+    ignored for set determination. This ensures that 'bobby_nohash_0.wav' and
+    'bobby_nohash_1.wav' are always in the same set, for example.
+
+    Args:
+        filename: File path of the data sample.
+        validation_percentage: How much of the data set to use for validation.
+        testing_percentage: How much of the data set to use for testing.
+
+    Returns:
+        String, one of 'training', 'validation', or 'testing'.
+    """
     base_name = os.path.basename(filename)
     # We want to ignore anything after '_nohash_' in the file name when
     # deciding which set to put a wav in, so the data set creator has a way of
     # grouping wavs that are close variations of each other.
     hash_name = re.sub(r'_nohash_.*$', '', base_name)
     # This looks a bit magical, but we need to decide whether this file should
     # go into the training, testing, or validation sets, and we want to keep
@@ -175,24 +175,24 @@
             self.prepare_background_data()
         self.prepare_processing_graph()
 
     @staticmethod
     def maybe_download_and_extract_dataset(data_url, dest_directory):
         """Download and extract data set tar file.
 
-    If the data set we're using doesn't already exist, this function
-    downloads it from the TensorFlow.org website and unpacks it into a
-    directory.
-    If the data_url is none, don't download anything and expect the data
-    directory to contain the correct files already.
-
-    Args:
-      data_url: Web location of the tar file containing the data set.
-      dest_directory: File path to extract data to.
-    """
+        If the data set we're using doesn't already exist, this function
+        downloads it from the TensorFlow.org website and unpacks it into a
+        directory.
+        If the data_url is none, don't download anything and expect the data
+        directory to contain the correct files already.
+
+        Args:
+            data_url: Web location of the tar file containing the data set.
+            dest_directory: File path to extract data to.
+        """
         if not data_url:
             return
         if not os.path.exists(dest_directory):
             os.makedirs(dest_directory)
         filename = data_url.split('/')[-1]
         filepath = os.path.join(dest_directory, filename)
         if not os.path.exists(filepath):
@@ -220,35 +220,35 @@
             tar.extractall(dest_directory)
 
     def prepare_data_index(self, silence_percentage, unknown_percentage,
                            wanted_words, validation_percentage,
                            testing_percentage):
         """Prepares a list of the samples organized by set and label.
 
-    The training loop needs a list of all the available data, organized by
-    which partition it should belong to, and with ground truth labels attached.
-    This function analyzes the folders below the `data_dir`, figures out the
-    right
-    labels for each file based on the name of the subdirectory it belongs to,
-    and uses a stable hash to assign it to a data set partition.
-
-    Args:
-      silence_percentage: How much of the resulting data should be background.
-      unknown_percentage: How much should be audio outside the wanted classes.
-      wanted_words: Labels of the classes we want to be able to recognize.
-      validation_percentage: How much of the data set to use for validation.
-      testing_percentage: How much of the data set to use for testing.
-
-    Returns:
-      Dictionary containing a list of file information for each set partition,
-      and a lookup map for each class to determine its numeric index.
-
-    Raises:
-      Exception: If expected files are not found.
-    """
+        The training loop needs a list of all the available data, organized by
+        which partition it should belong to, and with ground truth labels attached.
+        This function analyzes the folders below the `data_dir`, figures out the
+        right
+        labels for each file based on the name of the subdirectory it belongs to,
+        and uses a stable hash to assign it to a data set partition.
+
+        Args:
+            silence_percentage: How much of the resulting data should be background.
+            unknown_percentage: How much should be audio outside the wanted classes.
+            wanted_words: Labels of the classes we want to be able to recognize.
+            validation_percentage: How much of the data set to use for validation.
+            testing_percentage: How much of the data set to use for testing.
+
+        Returns:
+            Dictionary containing a list of file information for each set partition,
+            and a lookup map for each class to determine its numeric index.
+
+        Raises:
+            Exception: If expected files are not found.
+        """
         # Make sure the shuffling and picking of unknowns is deterministic.
         random.seed(RANDOM_SEED)
         wanted_words_index = {}
         for index, wanted_word in enumerate(wanted_words):
             wanted_words_index[wanted_word] = index + 2
         self.data_index = {'validation': [], 'testing': [], 'training': []}
         unknown_index = {'validation': [], 'testing': [], 'training': []}
@@ -312,31 +312,31 @@
                 self.word_to_index[word] = wanted_words_index[word]
             else:
                 self.word_to_index[word] = UNKNOWN_WORD_INDEX
         self.word_to_index[SILENCE_LABEL] = SILENCE_INDEX
 
     def prepare_background_data(self):
         """Searches a folder for background noise audio, and loads it into
-         memory.
-
-    It's expected that the background audio samples will be in a subdirectory
-    named '_background_noise_' inside the 'data_dir' folder, as .wavs that match
-    the sample rate of the training data, but can be much longer in duration.
-
-    If the '_background_noise_' folder doesn't exist at all, this isn't an
-    error, it's just taken to mean that no background noise augmentation should
-    be used. If the folder does exist, but it's empty, that's treated as an
-    error.
+        memory.
 
-    Returns:
-      List of raw PCM-encoded audio samples of background noise.
-
-    Raises:
-      Exception: If files aren't found in the folder.
-    """
+        It's expected that the background audio samples will be in a subdirectory
+        named '_background_noise_' inside the 'data_dir' folder, as .wavs that match
+        the sample rate of the training data, but can be much longer in duration.
+
+        If the '_background_noise_' folder doesn't exist at all, this isn't an
+        error, it's just taken to mean that no background noise augmentation should
+        be used. If the folder does exist, but it's empty, that's treated as an
+        error.
+
+        Returns:
+            List of raw PCM-encoded audio samples of background noise.
+
+        Raises:
+            Exception: If files aren't found in the folder.
+        """
         self.background_data = []
         background_dir = os.path.join(self.data_dir, BACKGROUND_NOISE_DIR_NAME)
         if not os.path.exists(background_dir):
             return self.background_data
 
         search_path = os.path.join(self.data_dir, BACKGROUND_NOISE_DIR_NAME,
                                    '*.wav')
@@ -349,18 +349,18 @@
             raise Exception('No background wav files were found in ' +
                             search_path)
         return []
 
     def prepare_processing_graph(self):
         """Builds a TensorFlow graph to apply the input distortions.
 
-    Creates a graph that loads a WAVE file, decodes it, scales the volume,
-    shifts it in time, adds in background noise, calculates a spectrogram, and
-    then builds an MFCC fingerprint from that.
-    """
+        Creates a graph that loads a WAVE file, decodes it, scales the volume,
+        shifts it in time, adds in background noise, calculates a spectrogram, and
+        then builds an MFCC fingerprint from that.
+        """
 
         @tf.function
         def processing_graph(wav_filename, foreground_volume,
                              time_shift_padding, time_shift_offset,
                              background_data, background_volume,
                              model_settings):
             desired_samples = model_settings['desired_samples']
@@ -403,34 +403,34 @@
 
         self.processing_graph = processing_graph
 
     def get_data(self, how_many, offset, background_frequency,
                  background_volume_range, time_shift, mode):
         """Gather samples from the data set, applying transformations as needed.
 
-    When the mode is 'training', a random selection of samples will be returned,
-    otherwise the first N clips in the partition will be used. This ensures that
-    validation always uses the same samples, reducing noise in the metrics.
+        When the mode is 'training', a random selection of samples will be returned,
+        otherwise the first N clips in the partition will be used. This ensures that
+        validation always uses the same samples, reducing noise in the metrics.
+
+        Args:
+            how_many: Desired number of samples to return. -1 means the entire
+                contents of this partition.
+            offset: Where to start when fetching deterministically.
+            background_frequency: How many clips will have background noise, 0.0 to
+                1.0.
+            background_volume_range: How loud the background noise will be.
+            time_shift: How much to randomly shift the clips by in time.
+            mode: Which partition to use, must be 'training', 'validation', or
+                'testing'.
 
-    Args:
-      how_many: Desired number of samples to return. -1 means the entire
-        contents of this partition.
-      offset: Where to start when fetching deterministically.
-      background_frequency: How many clips will have background noise, 0.0 to
-        1.0.
-      background_volume_range: How loud the background noise will be.
-      time_shift: How much to randomly shift the clips by in time.
-      mode: Which partition to use, must be 'training', 'validation', or
-        'testing'.
-
-    Returns:
-      List of sample data for the transformed samples, and list of label indexes
+        Returns:
+            List of sample data for the transformed samples, and list of label indexes
 
-    Raises:
-      ValueError: If background samples are too short.
+        Raises:
+            ValueError: If background samples are too short.
     """
         # Raise an error if data are not present, i.e. data directory is None
         if self.data_dir is None:
             raise RuntimeError(
                 "Calling 'get_data' method requires to have a valid "
                 "data directory. Here, data_dir=None")
 
@@ -517,23 +517,23 @@
             label_index = self.word_to_index[sample['label']]
             labels[i - offset] = label_index
         return data, labels
 
     def get_features_for_wav(self, wav_filename):
         """Applies the feature transformation process to the input_wav.
 
-    Runs the feature generation process (generally producing a spectrogram from
-    the input samples) on the WAV file. This can be useful for testing and
-    verifying implementations being run on other platforms.
+        Runs the feature generation process (generally producing a spectrogram from
+        the input samples) on the WAV file. This can be useful for testing and
+        verifying implementations being run on other platforms.
 
-    Args:
-      wav_filename: The path to the input audio file.
+        Args:
+            wav_filename: The path to the input audio file.
 
-    Returns:
-      Numpy data array containing the generated features.
+        Returns:
+            Numpy data array containing the generated features.
     """
         desired_samples = self.model_settings['desired_samples']
         background_data = tf.constant(np.zeros([desired_samples, 1]),
                                       tf.float32)
         input_dict = {
             'wav_filename': tf.constant(wav_filename),
             'time_shift_padding': tf.constant([[0, 0], [0, 0]]),
@@ -554,28 +554,28 @@
     def get_augmented_data_for_wav(self,
                                    wav_filename,
                                    background_frequency,
                                    background_volume_range,
                                    time_shift,
                                    num_augmented_samples=1):
         """Applies the feature transformation process to a wav audio file,
-         adding data augmentation (background noise and time shifting).
-
-    Args:
-      wav_filename (str): The path to the input audio file.
-      background_frequency: How many clips will have background noise, 0.0 to
-        1.0.
-      background_volume_range: How loud the background noise will be.
-      time_shift: How much to randomly shift the clips by in time.
-      num_augmented_samples: How many samples will be generated using data
-        augmentation.
+        adding data augmentation (background noise and time shifting).
 
-    Returns:
-      Numpy data array containing the generated features for every augmented
-        sample.
+        Args:
+            wav_filename (str): The path to the input audio file.
+            background_frequency: How many clips will have background noise, 0.0 to
+                1.0.
+            background_volume_range: How loud the background noise will be.
+            time_shift: How much to randomly shift the clips by in time.
+            num_augmented_samples: How many samples will be generated using data
+                augmentation.
+
+        Returns:
+            Numpy data array containing the generated features for every augmented
+            sample.
     """
         data = np.zeros(
             (num_augmented_samples, self.model_settings['fingerprint_size']))
         desired_samples = self.model_settings['desired_samples']
 
         for i in range(num_augmented_samples):
             # If we're time shifting, set up the offset for this sample.
```

### Comparing `akida_models-1.1.9/akida_models/layer_blocks.py` & `akida_models-1.2.0/akida_models/layer_blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,185 +15,226 @@
 # limitations under the License.
 # ******************************************************************************
 """
 Layers blocks definitions.
 """
 from functools import partial
 
-from keras.layers import (BatchNormalization, ReLU, Conv2D, SeparableConv2D, Dense, MaxPool2D,
-                          AvgPool2D, GlobalAvgPool2D, LayerNormalization, Dropout, Add,
+from keras.layers import (BatchNormalization, ReLU, Conv2D, DepthwiseConv2D, SeparableConv2D, Dense,
+                          MaxPool2D, GlobalAvgPool2D, LayerNormalization, Dropout, Add,
                           Conv2DTranspose, Reshape)
 from keras.activations import swish
 from keras.initializers import TruncatedNormal
 from tensorflow_addons.layers import GELU, GroupNormalization
 
-from quantizeml.layers import (Attention, LayerMadNormalization, SeparableConv2DTranspose,
+from quantizeml.layers import (Attention, LayerMadNormalization, DepthwiseConv2DTranspose,
                                ExtractToken)
+from .utils import get_params_by_version
 
 
 def _add_pooling_layer(x, pooling_type, pool_size, padding, layer_base_name):
     """Add a pooling layer in the graph.
 
     From an input tensor 'x', the function returns the output tensor after
     a pooling layer defined by 'pooling_type'.
 
     Args:
         x (tf.Tensor): the input tensor
-        pooling_type (str): type of pooling among the following: 'max',
-            'avg' or 'global_avg'.
+        pooling_type (str): type of pooling among the following: 'max' or 'global_avg'.
         pool_size (int or tuple of 2 integers): factors by which to
             downscale (vertical, horizontal). (2, 2) will halve the input in
             both spatial dimension. If only one integer is specified, the same
             window length will be used for both dimensions.
         padding (str): one of "valid" or "same" (case-insensitive).
         layer_base_name (str): base name for the pooling layer.
 
     Returns:
         tf.Tensor: an output tensor after pooling
     """
     if pooling_type == 'max':
         return MaxPool2D(pool_size=pool_size,
                          padding=padding,
                          name=layer_base_name + '/maxpool')(x)
-    if pooling_type == 'avg':
-        return AvgPool2D(pool_size=pool_size,
-                         padding=padding,
-                         name=layer_base_name + '/avgpool')(x)
     if pooling_type == 'global_avg':
         return GlobalAvgPool2D(name=layer_base_name + '/global_avg')(x)
-    raise ValueError("'pooling_type' argument must be 'max', 'avg' or 'global_avg'.")
+    raise ValueError("'pooling_type' argument must be 'max' or 'global_avg'.")
 
 
 def conv_block(inputs,
                filters,
                kernel_size,
                pooling=None,
+               post_relu_gap=False,
                pool_size=(2, 2),
                add_batchnorm=False,
-               add_activation=True,
+               relu_activation='ReLU3.75',
                **kwargs):
     """Adds a convolutional layer with optional layers in the following order:
     max pooling, batch normalization, activation.
 
     Args:
         inputs (tf.Tensor): input tensor of shape `(rows, cols, channels)`
         filters (int): the dimensionality of the output space
             (i.e. the number of output filters in the convolution).
         kernel_size (int or tuple of 2 integers): specifying the
             height and width of the 2D convolution kernel.
             Can be a single integer to specify the same value for
             all spatial dimensions.
-        pooling (str): add a pooling layer of type 'pooling' among the
-            values 'max', 'avg', 'global_max' or 'global_avg', with pooling
-            size set to pool_size. If 'None', no pooling will be added.
-        pool_size (int or tuple of 2 integers): factors by which to
-            downscale (vertical, horizontal). (2, 2) will halve the input in
-            both spatial dimension. If only one integer is specified, the same
-            window length will be used for both dimensions.
-        add_batchnorm (bool): add a BatchNormalization layer
-        add_activation (bool): add a ReLU layer
+        pooling (str, optional): add a pooling layer of type 'pooling' among the values 'max' or
+            'global_avg', with pooling size set to pool_size. If 'None', no pooling will be added.
+        post_relu_gap (bool, optional): when pooling is 'global_avg', indicates if the pooling comes
+            before or after ReLU activation. Defaults to False.
+        pool_size (int or tuple of 2 integers, optional): factors by which to downscale (vertical,
+            horizontal). (2, 2) will halve the input in both spatial dimension. If only one integer
+            is specified, the same window length will be used for both dimensions.
+        add_batchnorm (bool, optional): add a BatchNormalization layer
+        relu_activation (str, optional): the ReLU activation to add to the layer in the form 'ReLUx'
+            where 'x' is the max_value to use. Set to False to disable activation. Defaults to
+            'ReLU3.75'.
         **kwargs: arguments passed to the keras.Conv2D layer, such as
             strides, padding, use_bias, weight_regularizer, etc.
 
     Returns:
         tf.Tensor: output tensor of conv2D block.
     """
     if 'activation' in kwargs and kwargs['activation']:
         raise ValueError("Keyword argument 'activation' in conv_block must be None.")
     if 'dilation_rate' in kwargs and kwargs['dilation_rate'] not in [1, [1, 1], (1, 1)]:
         raise ValueError("Keyword argument 'dilation_rate' is not supported in conv_block.")
 
     conv_layer = Conv2D(filters, kernel_size, **kwargs)
     x = conv_layer(inputs)
 
-    if pooling:
-        x = _add_pooling_layer(x, pooling, pool_size, conv_layer.padding,
-                               conv_layer.name)
+    if pooling == 'max' or (pooling == 'global_avg' and not post_relu_gap):
+        x = _add_pooling_layer(x, pooling, pool_size, conv_layer.padding, conv_layer.name)
 
     if add_batchnorm:
         x = BatchNormalization(name=conv_layer.name + '/BN')(x)
 
-    if add_activation:
-        x = ReLU(6.0, name=conv_layer.name + '/relu')(x)
+    if relu_activation:
+        x = act_to_layer(relu_activation, name=conv_layer.name + '/relu')(x)
 
+    if post_relu_gap and pooling == 'global_avg':
+        x = _add_pooling_layer(x, pooling, pool_size, conv_layer.padding, conv_layer.name)
     return x
 
 
 def separable_conv_block(inputs,
                          filters,
                          kernel_size,
+                         strides=1,
+                         padding="same",
+                         use_bias=True,
                          pooling=None,
+                         post_relu_gap=False,
                          pool_size=(2, 2),
                          add_batchnorm=False,
-                         add_activation=True,
-                         **kwargs):
+                         relu_activation='ReLU3.75',
+                         fused=True,
+                         name=None,
+                         kernel_initializer='glorot_uniform',
+                         pointwise_regularizer=None):
     """Adds a separable convolutional layer with optional layers in the
     following order: global average pooling, max pooling, batch normalization,
     activation.
 
     Args:
         inputs (tf.Tensor): input tensor of shape `(height, width, channels)`
         filters (int): the dimensionality of the output space
             (i.e. the number of output filters in the pointwise convolution).
         kernel_size (int or tuple of 2 integers): specifying the
             height and width of the 2D convolution window. Can be a single
             integer to specify the same value for all spatial dimensions.
-        pooling (str): add a pooling layer of type 'pooling' among the
-            values 'max', 'avg', 'global_max' or 'global_avg', with pooling
-            size set to pool_size. If 'None', no pooling will be added.
-        pool_size (int or tuple of 2 integers): factors by which to
-            downscale (vertical, horizontal). (2, 2) will halve the input in
-            both spatial dimension. If only one integer is specified, the same
-            window length will be used for both dimensions.
-        add_batchnorm (bool): add a BatchNormalization layer
-        add_activation (bool): add a ReLU layer
-        **kwargs: arguments passed to the keras.SeparableConv2D layer,
-            such as strides, padding, use_bias, etc.
+        strides (int or tuple of 2 integers, optional): strides of the depthwise convolution.
+            Defaults to 1.
+        padding (str, optional): padding mode for the depthwise convolution. Defaults to 'same'.
+        use_bias (bool, optional): whether the layer uses a bias vector. Defaults to True.
+        pooling (str, optional): add a pooling layer of type 'pooling' among the values 'max', or
+            'global_avg', with pooling size set to pool_size. If 'None', no pooling will be added.
+        post_relu_gap (bool, optional): when pooling is 'global_avg', indicates if the pooling comes
+            before or after ReLU activation. Defaults to False.
+        pool_size (int or tuple of 2 integers, optional): factors by which to downscale (vertical,
+            horizontal). (2, 2) will halve the input in both spatial dimension. If only one integer
+            is specified, the same window length will be used for both dimensions.
+        add_batchnorm (bool, optional): add a BatchNormalization layer
+        relu_activation (str, optional): the ReLU activation to add to the layer in the form 'ReLUx'
+            where 'x' is the max_value to use. Set to False to disable activation. Defaults to
+            'ReLU3.75'.
+        fused (bool, optional): If True use a SeparableConv2D layer otherwise use a
+            DepthwiseConv2D + Conv2D layers. Defaults to True.
+        name (str, optional): name of the layer. Defaults to None.
+        kernel_initializer (keras.initializer, optional): initializer for both kernels. Defaults to
+            'glorot_uniform'.
+        pointwise_regularizer (keras.regularizers, optional): regularizer function applied to the
+            pointwise kernel matrix. Defaults to None.
 
     Returns:
         tf.Tensor: output tensor of separable conv block.
     """
-    if 'activation' in kwargs and kwargs['activation']:
-        raise ValueError("Keyword argument 'activation' in separable_conv_block must be None.")
-    if 'dilation_rate' in kwargs and kwargs['dilation_rate'] not in [1, [1, 1], (1, 1)]:
-        raise ValueError("Keyword argument 'dilation_rate' is not supported in "
-                         "separable_conv_block.")
-    if 'depth_multiplier' in kwargs and kwargs['depth_multiplier'] != 1:
-        raise ValueError("Keyword argument 'depth_multiplier' is not "
-                         "supported in separable_conv_block.")
-
-    sep_conv_layer = SeparableConv2D(filters, kernel_size, **kwargs)
-    x = sep_conv_layer(inputs)
-
-    if pooling:
-        x = _add_pooling_layer(x, pooling, pool_size, sep_conv_layer.padding,
-                               sep_conv_layer.name)
+    if name:
+        dw_name = "dw_" + name
+        pw_name = "pw_" + name
+
+    else:
+        dw_name = pw_name = None
+    # if fused set a SeparableConv2D layer
+    if fused:
+        sep_conv_layer = SeparableConv2D(filters, kernel_size, strides=strides, padding=padding,
+                                         use_bias=use_bias,
+                                         depthwise_initializer=kernel_initializer,
+                                         pointwise_initializer=kernel_initializer,
+                                         pointwise_regularizer=pointwise_regularizer,
+                                         name=name)
+        x = sep_conv_layer(inputs)
+        main_layer_name = sep_conv_layer.name
+    # if not fused set a DepthwiseConv2D + Conv2D layer (the Conv2D applies a Pointwise convolution)
+    else:
+        depth_conv_layer = DepthwiseConv2D(kernel_size, strides=strides, padding=padding,
+                                           use_bias=False,
+                                           depthwise_initializer=kernel_initializer,
+                                           name=dw_name)
+        point_conv_layer = Conv2D(filters, (1, 1), use_bias=use_bias, padding='same',
+                                  kernel_initializer=kernel_initializer,
+                                  kernel_regularizer=pointwise_regularizer,
+                                  name=pw_name)
+
+        x = depth_conv_layer(inputs)
+        x = point_conv_layer(x)
+
+        main_layer_name = point_conv_layer.name
+
+    if pooling == 'max' or (pooling == 'global_avg' and not post_relu_gap):
+        x = _add_pooling_layer(x, pooling, pool_size, padding, main_layer_name)
 
     if add_batchnorm:
-        x = BatchNormalization(name=sep_conv_layer.name + '/BN')(x)
+        x = BatchNormalization(name=main_layer_name + '/BN')(x)
 
-    if add_activation:
-        x = ReLU(6.0, name=sep_conv_layer.name + '/relu')(x)
+    if relu_activation:
+        x = act_to_layer(relu_activation, name=main_layer_name + '/relu')(x)
 
+    if post_relu_gap and pooling == 'global_avg':
+        x = _add_pooling_layer(x, pooling, pool_size, padding, main_layer_name)
     return x
 
 
 def dense_block(inputs,
                 units,
                 add_batchnorm=False,
-                add_activation=True,
+                relu_activation='ReLU3.75',
                 **kwargs):
     """Adds a dense layer with optional layers in the following order:
     batch normalization, activation.
 
     Args:
         inputs (tf.Tensor): Input tensor of shape `(rows, cols, channels)`
         units (int): dimensionality of the output space
-        add_batchnorm (bool): add a BatchNormalization layer
-        add_activation (bool): add a ReLU layer
+        add_batchnorm (bool, optional): add a BatchNormalization layer
+        relu_activation (str, optional): the ReLU activation to add to the layer in the form 'ReLUx'
+            where 'x' is the max_value to use. Set to False to disable activation. Defaults to
+            'ReLU3.75'.
         **kwargs: arguments passed to the Dense layer, such as
             use_bias, kernel_initializer, weight_regularizer, etc.
 
     Returns:
         tf.Tensor: output tensor of the dense block.
     """
     if 'activation' in kwargs and kwargs['activation']:
@@ -201,16 +242,16 @@
 
     dense_layer = Dense(units, **kwargs)
     x = dense_layer(inputs)
 
     if add_batchnorm:
         x = BatchNormalization(name=dense_layer.name + '/BN')(x)
 
-    if add_activation:
-        x = ReLU(6.0, name=dense_layer.name + '/relu')(x)
+    if relu_activation:
+        x = act_to_layer(relu_activation, name=dense_layer.name + '/relu')(x)
 
     return x
 
 
 def act_to_layer(act, **kwargs):
     """ Get activation layer from string.
 
@@ -380,28 +421,30 @@
     return outputs, (weights, x_norm2)
 
 
 def conv_transpose_block(inputs,
                          filters,
                          kernel_size,
                          add_batchnorm=False,
-                         add_activation=True,
+                         relu_activation='ReLU8',
                          **kwargs):
     """Adds a transposed convolutional layer with optional layers in the following order:
     batch normalization, activation.
 
     Args:
         inputs (tf.Tensor): input tensor of shape `(rows, cols, channels)`
         filters (int): the dimensionality of the output space (i.e. the number of output filters in
             the convolution).
         kernel_size (int or tuple of 2 integers): specifying the height and width of the 2D
             convolution kernel. Can be a single integer to specify the same value for all spatial
             dimensions.
         add_batchnorm (bool, optional): add a BatchNormalization layer. Defaults to False.
-        add_activation (bool, optional): add a ReLU8 layer. Defaults to True.
+        relu_activation (str, optional): the ReLU activation to add to the layer in the form 'ReLUx'
+            where 'x' is the max_value to use. Set to False to disable activation. Defaults to
+            'ReLU3.75'.
         **kwargs: arguments passed to the keras.Conv2DTranspose layer, such as strides, padding,
             use_bias, weight_regularizer, etc.
 
     Returns:
         tf.Tensor: output tensor of transposed convolution block.
     """
     if 'activation' in kwargs and kwargs['activation']:
@@ -412,61 +455,88 @@
 
     conv_trans_layer = Conv2DTranspose(filters, kernel_size, **kwargs)
     x = conv_trans_layer(inputs)
 
     if add_batchnorm:
         x = BatchNormalization(name=conv_trans_layer.name + '/BN')(x)
 
-    if add_activation:
-        x = ReLU(8.0, name=conv_trans_layer.name + '/relu')(x)
+    if relu_activation:
+        x = act_to_layer(relu_activation, name=conv_trans_layer.name + '/relu')(x)
 
     return x
 
 
 def sepconv_transpose_block(inputs,
                             filters,
                             kernel_size,
+                            strides=2,
+                            padding='same',
+                            use_bias=True,
                             add_batchnorm=False,
-                            add_activation=True,
-                            **kwargs):
+                            relu_activation='ReLU3.75',
+                            name=None,
+                            kernel_initializer='glorot_uniform',
+                            pointwise_regularizer=None):
     """Adds a transposed separable convolutional layer with optional layers in the following order:
     batch normalization, activation.
 
+    The separable operation is made of a DepthwiseConv2DTranspose followed by a pointwise Conv2D.
+
     Args:
         inputs (tf.Tensor): input tensor of shape `(rows, cols, channels)`
         filters (int): the dimensionality of the output space (i.e. the number of output filters in
             the pointwise convolution).
-        kernel_size (int or tuple of 2 integers): specifying the height and width of the 2D
-            convolution kernel. Can be a single integer to specify the same value for all spatial
+        kernel_size (int or tuple of 2 integers): specifying the height and width of the depthwise
+            transpose kernel. Can be a single integer to specify the same value for all spatial
             dimensions.
+        strides (int or tuple of 2 integers, optional): strides of the transposed depthwise.
+            Defaults to 2.
+        padding (str, optional): padding mode for the transposed depthwise. Defaults to 'same'.
+        use_bias (bool, optional): whether the layer uses a bias vectors. Defaults to True.
         add_batchnorm (bool, optional): add a BatchNormalization layer. Defaults to False.
-        add_activation (bool, optional): add a ReLU8 layer. Defaults to True.
-        **kwargs: arguments passed to the SeparableConv2DTranspose layer, such as strides, padding,
-            use_bias, weight_regularizer, etc.
+        relu_activation (str, optional): the ReLU activation to add to the layer in the form 'ReLUx'
+            where 'x' is the max_value to use. Set to False to disable activation. Defaults to
+            'ReLU3.75'.
+        name (str, optional): name of the layer. Defaults to None.
+        kernel_initializer (keras.initializer, optional): initializer for both kernels. Defaults to
+            'glorot_uniform'.
+        pointwise_regularizer (keras.regularizers, optional): regularizer function applied to the
+            pointwise kernel matrix. Defaults to None.
 
     Returns:
         tf.Tensor: output tensor of transposed separable convolution block.
     """
-    if 'activation' in kwargs and kwargs['activation']:
-        raise ValueError("Keyword argument 'activation' in separable_conv_block must be None.")
-    if 'dilation_rate' in kwargs and kwargs['dilation_rate'] not in [1, [1, 1], (1, 1)]:
-        raise ValueError("Keyword argument 'dilation_rate' is not supported in "
-                         "separable_conv_block.")
-    if 'depth_multiplier' in kwargs and kwargs['depth_multiplier'] != 1:
-        raise ValueError("Keyword argument 'depth_multiplier' is not "
-                         "supported in separable_conv_block.")
+    if name:
+        dw_name = "dw_" + name
+        pw_name = "pw_" + name
+    else:
+        dw_name, pw_name = None, None
+
+    dw_trans_layer = DepthwiseConv2DTranspose(kernel_size,
+                                              strides=strides,
+                                              padding=padding,
+                                              use_bias=use_bias,
+                                              depthwise_initializer=kernel_initializer,
+                                              name=dw_name)
+    pw_layer = Conv2D(filters,
+                      kernel_size=1,
+                      padding='valid',
+                      use_bias=use_bias,
+                      kernel_regularizer=pointwise_regularizer,
+                      kernel_initializer=kernel_initializer,
+                      name=pw_name)
 
-    sepconv_trans_layer = SeparableConv2DTranspose(filters, kernel_size, **kwargs)
-    x = sepconv_trans_layer(inputs)
+    x = dw_trans_layer(inputs)
+    x = pw_layer(x)
 
     if add_batchnorm:
-        x = BatchNormalization(name=sepconv_trans_layer.name + '/BN')(x)
+        x = BatchNormalization(name=pw_layer.name + '/BN')(x)
 
-    if add_activation:
-        x = ReLU(8.0, name=sepconv_trans_layer.name + '/relu')(x)
+    if relu_activation:
+        x = act_to_layer(relu_activation, name=pw_layer.name + '/relu')(x)
 
     return x
 
 
 def yolo_head_block(x, num_boxes, classes, filters=1024):
     """Adds the `YOLOv2 detection head <https://arxiv.org/pdf/1612.08242.pdf>`_, at the output
     of a model.
@@ -479,26 +549,29 @@
 
     Returns:
         :obj:`tf.Tensor`: output tensor of yolo detection head block.
 
     Notes:
         This block replaces conv layers by separable_conv, to decrease the amount of parameters.
     """
+    # Model version management
+    fused, _, relu_activation = get_params_by_version(relu_v2='ReLU7.5')
+
     x = separable_conv_block(x, filters=filters, name='1conv',
                              kernel_size=(3, 3), padding='same', use_bias=False,
-                             add_activation=True, add_batchnorm=True)
+                             relu_activation=relu_activation, add_batchnorm=True, fused=fused)
     x = separable_conv_block(x, filters=filters, name='2conv',
                              kernel_size=(3, 3), padding='same', use_bias=False,
-                             add_activation=True, add_batchnorm=True)
+                             relu_activation=relu_activation, add_batchnorm=True, fused=fused)
     x = separable_conv_block(x, filters=filters, name='3conv',
                              kernel_size=(3, 3), padding='same', use_bias=False,
-                             add_activation=True, add_batchnorm=True)
+                             relu_activation=relu_activation, add_batchnorm=True, fused=fused)
     x = separable_conv_block(x, filters=(num_boxes * (4 + 1 + classes)), name='detection_layer',
                              kernel_size=(3, 3), padding='same', use_bias=True,
-                             add_activation=False, add_batchnorm=False)
+                             relu_activation=False, add_batchnorm=False, fused=fused)
     return x
 
 
 def vit_extract_feature_map(y, feat_shape, num_non_patch=1):
     """Add a ExtractToken + Reshape layers to convert the plain ViT output into a feature map.
 
     All tokens will be extracted except those considered as class tokens (``num_non_patch``)
```

### Comparing `akida_models-1.1.9/akida_models/macs.py` & `akida_models-1.2.0/akida_models/macs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import tensorflow as tf
 from tensorflow.python.framework.convert_to_constants import (
         convert_variables_to_constants_v2_as_graph)
 
-from quantizeml.models import load_model
-from cnn2snn import load_quantized_model
+from .model_io import load_model
 
 
 def get_flops(model):
     """
     Calculate FLOPS for a tf.keras.Model or tf.keras.Sequential model in inference mode.
 
     It uses tf.compat.v1.profiler under the hood.
@@ -54,19 +53,15 @@
     By default it displays only the total MACS.
 
     Args:
         model (:obj:`keras.Model`): the model to evaluate
         verbose (bool): display MACS for each operation
 
     """
-    try:
-        model = load_model(model_path)
-    except ValueError:
-        model = load_quantized_model(model_path)
-
+    model = load_model(model_path)
     flops = get_flops(model)
 
     if verbose:
         def display_children_macs(nodes):
             for node in nodes:
                 print(f"{node.name}: {node.total_float_ops / 2:e} MACS")
                 display_children_macs(node.children)
```

### Comparing `akida_models-1.1.9/akida_models/mnist/model_gxnor.py` & `akida_models-1.2.0/akida_models/centernet/model_centernet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,133 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2021 Brainchip Holdings Ltd.
+# Copyright 2023 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-GXNOR model definition for MNIST classification.
+CenterNet model definition for detection
 """
+import numpy as np
 
-from keras import Model
-from keras.layers import Input, Flatten, Rescaling
+from keras import Model, initializers
+from keras.layers import Conv2D
 
-from cnn2snn import quantize, load_quantized_model
+from cnn2snn import set_akida_version, AkidaVersion
 
-from ..layer_blocks import conv_block, dense_block
+from .. import akidanet_imagenet
+from ..layer_blocks import (separable_conv_block, conv_block, conv_transpose_block,
+                            sepconv_transpose_block)
 from ..utils import fetch_file
+from ..model_io import load_model, get_model_path
 
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/gxnor/'
 
-
-def gxnor_mnist(weight_quantization=0,
-                activ_quantization=0,
-                input_weight_quantization=None):
-    """ Instantiates a Keras GXNOR model with an additional dense layer to make
-    better classification.
-
-    The paper describing the original model can be found `here
-    <https://www.sciencedirect.com/science/article/pii/S0893608018300108>`_.
+def centernet_base(input_shape=(224, 224, 3),
+                   classes=2,
+                   alpha=0.5,
+                   input_scaling=(127, -1)):
+    """ A Keras Model implementing the CenterNet architecture, on top of an AkidaNet backbone
 
     Args:
-        weight_quantization (int, optional): sets all weights in the model to
-            have a particular quantization bitwidth except for the weights in
-            the first layer. Defaults to 0.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        activ_quantization (int, optional): sets all activations in the model to
-            have a particular activation quantization bitwidth. Defaults to 0.
-
-            * '0' implements floating point 32-bit activations.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
-        input_weight_quantization(int, optional): sets weight quantization in
-            the first layer. Defaults to weight_quantization value.
-
-            * '0' implements floating point 32-bit weights.
-            * '2' through '8' implements n-bit weights where n is from 2-8 bits.
+        input_shape (tuple, optional): input shape. Defaults to (224, 224, 3).
+        classes (int, optional): number of output classes. Defaults to 2.
+        alpha (float, optional): controls the width of the model. Defaults to 0.5.
+        input_scaling (tuple, optional): input scaling. Defaults to (127, -1).
 
     Returns:
-        keras.Model: a Keras model for GXNOR/MNIST
+        keras.Model: a Keras Model instance.
     """
+    # This model is only available for akida 2.0
+    with set_akida_version(AkidaVersion.v2):
+        # Create an AkidaNet network without top layers
+        base_model = akidanet_imagenet(
+            input_shape=input_shape,
+            alpha=alpha,
+            include_top=False,
+            input_scaling=input_scaling)
+
+        x = base_model.layers[-1].output
+
+        # Build the neck with up convolutions
+        num_deconv_filters = [256, 128, 64]
+
+        for i, (n_filt) in enumerate(num_deconv_filters):
+            if n_filt <= 128:
+                curr_block = conv_block
+                block_type = "conv"
+                kwargs = {}
+                transpose_block = conv_transpose_block
+            else:
+                curr_block = separable_conv_block
+                block_type = "sepconv"
+                kwargs = {'fused': False}
+                transpose_block = sepconv_transpose_block
+
+            x = curr_block(x,
+                           filters=n_filt,
+                           name=f'neck_{block_type}_{i}',
+                           kernel_size=(3, 3),
+                           padding='same',
+                           use_bias=False,
+                           relu_activation='ReLU7.5',
+                           add_batchnorm=True,
+                           **kwargs)
+            x = transpose_block(x,
+                                filters=n_filt,
+                                name=f"neck_transpose_{block_type}_{i}",
+                                kernel_size=(4, 4),
+                                padding="same",
+                                strides=(2, 2),
+                                use_bias=False,
+                                relu_activation='ReLU7.5',
+                                add_batchnorm=True)
+
+        # Build the head which is composed of 2 consecutive convs
+        bias_initializer = initializers.Constant(float(-np.log((1 - 0.1) / 0.1)))
+        init_kernel = initializers.RandomNormal(stddev=0.001, seed=6)
+        # In the legacy model there is 3 branches of 64 filters each one.
+        # This could be merged in one branch
+        x = conv_block(x, 3 * 64, (3, 3),
+                       add_batchnorm=True,
+                       use_bias=False,
+                       relu_activation='ReLU7.5',
+                       padding="same",
+                       name="head_conv_1",
+                       kernel_initializer=init_kernel)
+        # The output is built by #classes and box coordinates in xywh
+        x = Conv2D(classes + 4,
+                   (1, 1),
+                   padding="same",
+                   use_bias=True,
+                   name="head_conv_2",
+                   bias_initializer=bias_initializer,
+                   kernel_initializer=init_kernel)(x)
 
-    # check if overrides have been provided and override
-    if input_weight_quantization is None:
-        input_weight_quantization = weight_quantization
-
-    img_input = Input(shape=(28, 28, 1), name="input")
-    x = Rescaling(1. / 255, name="rescaling")(img_input)
-
-    # Block 1
-    x = conv_block(x,
-                   filters=32,
-                   name='block_1/conv_1',
-                   kernel_size=(5, 5),
-                   padding='same',
-                   add_batchnorm=True,
-                   add_activation=True,
-                   pooling='max',
-                   pool_size=(2, 2))
-
-    # Block 2
-    x = conv_block(x,
-                   filters=64,
-                   name='block_2/conv_1',
-                   kernel_size=(3, 3),
-                   padding='same',
-                   add_batchnorm=True,
-                   add_activation=True,
-                   strides=2,
-                   pool_size=(2, 2))
-
-    # Classification block
-    x = Flatten(name='flatten')(x)
-    x = dense_block(x,
-                    units=512,
-                    name='fc_1',
-                    add_batchnorm=True,
-                    add_activation=True)
-    x = dense_block(x,
-                    units=10,
-                    name='predictions',
-                    add_batchnorm=True,
-                    add_activation=False)
-
-    # Create model
-    model = Model(img_input, x, name='gxnor_mnist')
-
-    if ((weight_quantization != 0) or (activ_quantization != 0) or
-            (input_weight_quantization != 0)):
-        return quantize(model, weight_quantization, activ_quantization,
-                        input_weight_quantization)
-    return model
-
-
-def gxnor_mnist_pretrained():
-    """ Helper method to retrieve a `gxnor_mnist` model that was trained on
-    MNIST dataset.
-
-    This model was trained with the distillation knowledge method, using
-    the EfficientNet model from `this repository
-    <https://github.com/EscVM/Efficient-CapsNet>`_ and the `Distiller` class from
-    the knowledge distillation toolkit (`akida_models.distiller`).
-
-    The float training was done for 30 epochs with a learning rate of 1e-4
-    After that we gradually quantize the model from:
-    8-4-4 --> 4-4-4 --> 4-4-2 --> 2-2-2 --> 2-2-1 tuning the model at each step
-    with the same distillation training method for 5 epochs and a learning rate
-    of 5e-5.
+    # Build the model
+    return Model(inputs=base_model.input, outputs=x, name='centernet_base')
+
+
+def centernet_voc_pretrained():
+    """
+    Helper method to retrieve an `centernet_base` model that was trained on VOC detection dataset.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
-    model_name = 'gxnor_mnist_iq2_wq2_aq1.h5'
-    file_hash = '836d4d32bf6a25620782f783419a1eae0c90460f3c291e2c5a8ed4a6cf36b035'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
-                            fname=model_name,
-                            file_hash=file_hash,
+    model_name_v2 = 'centernet_akidanet_voc_i8_w8_a8.h5'
+    file_hash_v2 = '5705206ecb5b006afd33838ada04d69d7dea0beda34727dee2a4bc0a80b9fd8b'
+    model_path, model_name, file_hash = get_model_path("centernet", model_name_v2=model_name_v2,
+                                                       file_hash_v2=file_hash_v2)
+    model_path = fetch_file(model_path, fname=model_name, file_hash=file_hash,
                             cache_subdir='models')
-    return load_quantized_model(model_path)
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/modelnet40/modelnet40_train.py` & `akida_models-1.2.0/akida_models/modelnet40/modelnet40_train.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
 ModelNet40 model training script.
 """
 
+import os
 import argparse
-import keras
 import numpy as np
 
 from keras.callbacks import LearningRateScheduler
 
-from cnn2snn import load_quantized_model, convert
+from cnn2snn import convert
 
 from .preprocessing import get_modelnet, get_modelnet_from_file
 
-from ..training import get_training_parser, compile_model, print_history_stats
+from ..training import (get_training_parser, compile_model, print_history_stats, evaluate_model,
+                        evaluate_akida_model, save_model)
+from ..extract import extract_samples
+from ..model_io import load_model
 
 
 def get_data(batch_size, selected_points, knn_points):
     """ Loads data.
 
     Args:
         batch_size (int): the batch size
@@ -81,41 +84,14 @@
     history = model.fit(train_dataset,
                         validation_data=test_dataset,
                         epochs=epochs,
                         callbacks=callbacks)
     print_history_stats(history)
 
 
-def evaluate_model(model, test_dataset):
-    """ Evaluates model performances.
-
-    Args:
-        model (keras.Model or akida.Model): the model to evaluate.
-        test_dataset (tf.dataset): evaluation dataset.
-    """
-    labels = np.concatenate([labels for x, labels in test_dataset], axis=0)
-
-    if isinstance(model, keras.Model):
-        preds = np.squeeze(np.argmax(model.predict(test_dataset), axis=1))
-    else:
-        pots_akida = np.empty(shape=[0, model.output_shape[-1]],
-                              dtype=np.float32)
-
-        for batch, _ in test_dataset:
-            # Rescale inputs to Akida
-            pots = (batch.numpy() * 127 + 127).astype('uint8')
-            pots_batch = model.predict(pots)
-            pots_akida = np.concatenate((pots_akida, pots_batch.squeeze()))
-
-        preds = np.squeeze(np.argmax(pots_akida, 1))
-
-    acc = np.sum(preds == labels) / labels.shape[0]
-    print(f"Accuracy: {acc}")
-
-
 def main():
     """ Entry point for script and CLI usage.
     """
     global_parser = argparse.ArgumentParser(add_help=False)
     global_parser.add_argument(
         "-p",
         "--selected_points",
@@ -126,39 +102,44 @@
     global_parser.add_argument("-n",
                                "--knn_points",
                                type=int,
                                default=64,
                                help="The number of points to include in each \
                         localised group. (default 64)")
 
-    parser = get_training_parser(batch_size=16, global_parser=global_parser)[0]
+    parser = get_training_parser(batch_size=16, global_parser=global_parser, extract=True)[0]
     args = parser.parse_args()
 
     # Load the source model
-    model = load_quantized_model(args.model)
+    model = load_model(args.model)
 
     # Compile model
     compile_model(model, loss="sparse_categorical_crossentropy")
 
     # Load data
     train_dataset, test_dataset = get_data(args.batch_size,
                                            args.selected_points,
                                            args.knn_points)
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action == "train":
         train_model(model, train_dataset, test_dataset, args.epochs)
-
-        # Save model in Keras format (h5)
-        if args.savemodel is not None:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
         if args.akida:
-            model = convert(model, input_scaling=(127, 127))
-        evaluate_model(model, test_dataset)
+            model = convert(model)
+            preds, labels = evaluate_akida_model(model, test_dataset, 'softmax')
+            accuracy = (np.argmax(preds, 1) == labels).mean()
+            print(f"Akida accuracy: {accuracy}")
+        else:
+            evaluate_model(model, test_dataset)
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, train_dataset, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/modelnet40/pointnet_utils.py` & `akida_models-1.2.0/akida_models/modelnet40/pointnet_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,21 +133,25 @@
 
     if num_features > 3:
         sh = tf.shape(outpoints)
         subtraction_padding = tf.zeros((sh[0], sh[1], 1, sh[3] - 3))
         subtraction_helper = tf.concat(
             [subtraction_helper, subtraction_padding], -1)
 
-    outpoints = (outpoints - subtraction_helper) / 127.0
+    outpoints = outpoints - subtraction_helper
 
     reshape_factor = get_reshape_factor(knn_points)
 
     # put the dimension to be folded last
     x = tf.transpose(outpoints, perm=[0, 3, 1, 2])
     # fold
     x = tf.reshape(x, [
         -1, num_features, selected_points * reshape_factor,
         int(knn_points / reshape_factor)
     ])
     # put dimensions back to original order
     points = tf.transpose(x, perm=[0, 2, 3, 1])
+
+    # Go back to [0, 255] uint8 range for homogeneity with Akida. The model will have a rescaling
+    # layer to get back to [-1, 1].
+    points = points + 127
     return points, label
```

### Comparing `akida_models-1.1.9/akida_models/modelnet40/preprocessing.py` & `akida_models-1.2.0/akida_models/modelnet40/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/param_scheduler.py` & `akida_models-1.2.0/akida_models/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.1.9/akida_models/portrait128/model_akida_unet.py` & `akida_models-1.2.0/akida_models/dvs/model_convtiny_gesture.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,157 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2022 Brainchip Holdings Ltd.
+# Copyright 2020 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Akida U-Net model definition for semantic segmentation.
+Convtiny model definition for DVS gesture classification.
 """
 
-from keras import Model, regularizers
-from keras.layers import Dropout, Activation
+from keras import Model
+from keras.layers import Input, Reshape, Dropout, Activation
 
-from ..layer_blocks import sepconv_transpose_block, dense_block
-from ..imagenet.model_akidanet import akidanet_imagenet
+from ..layer_blocks import conv_block, separable_conv_block, dense_block
+from ..utils import fetch_file, get_params_by_version
+from ..model_io import load_model, get_model_path
+
+# Locally fixed config options
+# The number of neurons in the penultimate dense layer
+# This layer has binary output spikes, and could be a bottleneck
+# if care isn't taken to ensure enough info capacity
+NUM_SPIKING_NEURONS = 256
 
 
-def akida_unet_portrait128(input_shape=(128, 128, 3),
-                           alpha=0.5,
-                           input_scaling=(128, -1)):
-    """Instantiates an Akida U-Net architecture.
-
-    It is composed of an AkidaNet-ImageNet encoder followed by a succession of Conv2DTranspose
-    layers for the decoder part.
-    It does not contain any skip connection (concatenation) between the encoder and the decoder
-    branches.
+def convtiny_dvs_gesture(input_shape=(64, 64, 10), classes=10):
+    """Instantiates a CNN for the "IBM DVS Gesture" example.
 
     Args:
-        input_shape (tuple, optional): input shape tuple. Defaults to (128, 128, 3).
-        alpha (float, optional): controls the width (number of filters) of the model. Defaults to
-            0.5.
-        input_scaling (tuple, optional): scale factor and offset to apply to inputs. Defaults to
-            (128, -1). Note that following Akida convention, the scale factor is a number used as a
-            divider.
+        input_shape (tuple, optional): input shape tuple of the model. Defaults to (64, 64, 10).
+        classes (int, optional): number of classes to classify images into. Defaults to 10.
 
     Returns:
-        keras.Model: a Keras Model instance.
+        keras.Model: a Keras convolutional model for DVS Gesture.
     """
-    # Define weight regularization, will apply to pointwise weights of sepconv transposed layers
-    weight_regularizer = regularizers.l2(4e-5)
+    # Model version management
+    fused, post_relu_gap, relu_activation = get_params_by_version()
+
+    img_input = Input(input_shape, name="input")
+
+    x = conv_block(img_input,
+                   filters=16,
+                   kernel_size=(3, 3),
+                   name='conv_01',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=16,
+                   kernel_size=(3, 3),
+                   name='conv_02',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=32,
+                   kernel_size=(3, 3),
+                   name='conv_03',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=64,
+                   kernel_size=(3, 3),
+                   name='conv_04',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=128,
+                   kernel_size=(3, 3),
+                   name='conv_05',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='global_avg',
+                   relu_activation=relu_activation,
+                   post_relu_gap=post_relu_gap,
+                   strides=(1, 1))
+
+    bm_outshape = (1, 1, 128)
+
+    x = Reshape(bm_outshape, name='reshape_1')(x)
+    x = Dropout(1e-3, name='dropout')(x)
+
+    x = separable_conv_block(x,
+                             filters=NUM_SPIKING_NEURONS,
+                             kernel_size=(3, 3),
+                             use_bias=False,
+                             padding='same',
+                             name='spiking_layer',
+                             add_batchnorm=True,
+                             pooling=None,
+                             relu_activation=relu_activation,
+                             fused=fused)
+
+    x = dense_block(x,
+                    units=classes,
+                    name='dense',
+                    add_batchnorm=False,
+                    relu_activation=False,
+                    use_bias=False)
+    act_function = 'softmax' if classes > 1 else 'sigmoid'
+    x = Activation(act_function, name=f'act_{act_function}')(x)
+    x = Reshape((classes,), name='reshape_2')(x)
+
+    return Model(inputs=img_input, outputs=x, name='dvs_network')
+
+
+def convtiny_gesture_pretrained():
+    """ Helper method to retrieve a `convtiny_dvs_gesture` model that was
+    trained on IBM DVS Gesture dataset.
 
-    # Create an AkidaNet network without top layers
-    encoder = akidanet_imagenet(input_shape=input_shape,
-                                alpha=alpha,
-                                include_top=False,
-                                input_scaling=input_scaling)
-
-    # Add the decoder layers
-    x = encoder.layers[-1].output
-    x = sepconv_transpose_block(x,
-                                filters=int(512 * alpha),
-                                kernel_size=(3, 3),
-                                strides=2,
-                                padding='same',
-                                kernel_initializer='he_normal',
-                                add_batchnorm=True,
-                                name='sepconv_t_0',
-                                pointwise_regularizer=weight_regularizer)
-    x = Dropout(0.5)(x)
-    x = sepconv_transpose_block(x,
-                                filters=int(256 * alpha),
-                                kernel_size=(3, 3),
-                                strides=2,
-                                padding='same',
-                                kernel_initializer='he_normal',
-                                add_batchnorm=True,
-                                name='sepconv_t_1',
-                                pointwise_regularizer=weight_regularizer)
-    x = Dropout(0.5)(x)
-    x = sepconv_transpose_block(x,
-                                filters=int(128 * alpha),
-                                kernel_size=(3, 3),
-                                strides=2,
-                                padding='same',
-                                kernel_initializer='he_normal',
-                                add_batchnorm=True,
-                                name='sepconv_t_2',
-                                pointwise_regularizer=weight_regularizer)
-    x = Dropout(0.5)(x)
-    x = sepconv_transpose_block(x,
-                                filters=int(64 * alpha),
-                                kernel_size=(3, 3),
-                                strides=2,
-                                padding='same',
-                                kernel_initializer='he_normal',
-                                add_batchnorm=True,
-                                name='sepconv_t_3',
-                                pointwise_regularizer=weight_regularizer)
-    x = Dropout(0.5)(x)
-    x = sepconv_transpose_block(x,
-                                filters=int(32 * alpha),
-                                kernel_size=(3, 3),
-                                strides=2,
-                                padding='same',
-                                kernel_initializer='he_normal',
-                                add_batchnorm=True,
-                                name='sepconv_t_4',
-                                pointwise_regularizer=weight_regularizer)
-    x = Dropout(0.5)(x)
-    x = dense_block(x, units=1, add_activation=False, name='head')
-    x = Activation('sigmoid', name="sigmoid_act")(x)
+    Returns:
+        keras.Model: a Keras Model instance.
 
-    # Build the whole model: encoder followed by decoder
-    return Model(inputs=encoder.input, outputs=x, name='akida_unet')
+    """
+    model_name_v1 = 'convtiny_dvs_gesture_iq4_wq4_aq4.h5'
+    file_hash_v1 = 'ad1a0a2ee13092921a914f25a6159dcb788540239d10ea96d3ff5fefec359281'
+    model_name_v2 = 'convtiny_dvs_gesture_i4_w4_a4.h5'
+    file_hash_v2 = '2921c29c04c0fda278000df18bb63d77c1e8a2d3bc23e32963f92072d26c2771'
+    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
+                            fname=model_name,
+                            file_hash=file_hash,
+                            cache_subdir='models')
+    return load_model(model_path)
```

### Comparing `akida_models-1.1.9/akida_models/portrait128/portrait128_train.py` & `akida_models-1.2.0/akida_models/portrait128/portrait128_train.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 """
 Portrait128 training script.
 """
 
 import os
 import argparse
 
+import tensorflow as tf
 import numpy as np
 from keras.preprocessing.image import ImageDataGenerator
 from keras.metrics import BinaryIoU
 
-from cnn2snn import load_quantized_model
-
-from akida_models.param_scheduler import get_cosine_lr_scheduler
+from cnn2snn import convert
 
+from ..param_scheduler import get_cosine_lr_scheduler
 from ..training import (get_training_parser, compile_model, evaluate_model, print_history_stats,
-                        RestoreBest)
+                        RestoreBest, save_model)
+from ..extract import extract_samples
+from ..model_io import load_model
 
 
 def get_data(path, batch_size):
     """ Loads Portrait128 data.
 
     Args:
         path (str): path to npy data
@@ -114,51 +116,89 @@
                         steps_per_epoch=steps_per_epoch,
                         validation_steps=val_steps,
                         validation_data=val_gen,
                         callbacks=callbacks)
     print_history_stats(history)
 
 
+def evaluate_akida_model(model, val_gen, val_steps):
+    """ Evaluates Akida model.
+
+    Args:
+        model (akida.Model): model to evaluate
+        val_gen (generator): validation data
+        val_steps (int): validation steps
+    """
+    # Initialize to None to allow different shapes depending on the caller
+    labels = None
+    pots = None
+
+    for _ in range(val_steps):
+        batch, label_batch = next(val_gen)
+        pots_batch = model.predict(batch.astype('uint8'))
+
+        if labels is None:
+            labels = label_batch
+            pots = pots_batch
+        else:
+            labels = np.concatenate((labels, label_batch))
+            pots = np.concatenate((pots, pots_batch))
+    preds = tf.keras.activations.sigmoid(pots)
+
+    m_binary_iou = tf.keras.metrics.BinaryIoU(target_class_ids=[0, 1], threshold=0.5)
+    m_binary_iou.update_state(labels, preds)
+    binary_iou = m_binary_iou.result().numpy()
+
+    m_accuracy = tf.keras.metrics.Accuracy()
+    m_accuracy.update_state(labels, preds > 0.5)
+    accuracy = m_accuracy.result().numpy()
+    print(f"Akida BinaryIoU/pixel accuracy: {binary_iou:.4f}/{100*accuracy:.2f}%")
+
+
 def main():
     """ Entry point for script and CLI usage.
     """
     global_parser = argparse.ArgumentParser(add_help=False)
     global_parser.add_argument("-d", "--data", type=str,
                                default="/hdd/datasets/Portrait128/data/",
                                help="Path to the Portrait128 data.")
 
-    parsers = get_training_parser(batch_size=32, tune=True, global_parser=global_parser)
+    parsers = get_training_parser(batch_size=32, tune=True, extract=True,
+                                  global_parser=global_parser)
     args = parsers[0].parse_args()
 
     # Load the source model
-    model = load_quantized_model(args.model)
+    model = load_model(args.model)
 
     # Compile model
     learning_rate = 3e-5
     if args.action == "tune":
         learning_rate /= 10
 
     compile_model(model, learning_rate=learning_rate, loss='binary_crossentropy',
                   metrics=[BinaryIoU(), 'accuracy'])
 
     # Load data
     train_gen, val_gen, steps_per_epoch, val_steps = get_data(args.data, args.batch_size)
 
+    # Disable QuantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action in ["train", "tune"]:
         train_model(model, train_gen, steps_per_epoch, val_gen,
                     val_steps, args.epochs, learning_rate)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
         if args.akida:
-            raise NotImplementedError('Converting segmentation models is not supported yet.')
-        evaluate_model(model, val_gen, steps=val_steps, print_history=True)
+            model = convert(model)
+            evaluate_akida_model(model, val_gen, val_steps)
+        else:
+            evaluate_model(model, val_gen, steps=val_steps, print_history=True)
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, train_gen, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models/training.py` & `akida_models-1.2.0/akida_models/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 import argparse
 import numpy as np
 
 from keras.preprocessing.image import DirectoryIterator
 from keras.optimizers import Adam
 from keras.layers import Activation
 from keras.callbacks import ModelCheckpoint
-from keras.utils.generic_utils import Progbar
-from quantizeml.layers import calibration
 
 
 def compile_model(model,
                   learning_rate=1e-3,
                   loss='categorical_crossentropy',
                   metrics=None):
     """ Compiles the model using Adam optimizer.
@@ -70,38 +68,14 @@
             if layer.name == freeze_before:
                 trainable = True
             layer.trainable = trainable
         if not trainable:
             raise ValueError(f"No such layer {freeze_before} in model.")
 
 
-def calibrate_model(model, x, num_samples, batch_size=None, epochs=1):
-    """Calibrates model
-
-    Args:
-        model (keras.Model): the model to calibrate
-        x (tf.Dataset, np.array or generator): train input data
-        num_samples (int): total number of samples before declaring the calibration round finished.
-        batch_size (int, optional): the batch size. Defaults to None.
-        epochs (int, optional): the number of epochs. Defaults to 1.
-    """
-    if batch_size is None:
-        steps = num_samples
-    else:
-        assert batch_size > 0, "The batch size should be strictly positive."
-        steps = np.ceil(num_samples / batch_size)
-
-    with calibration(True):
-        progbar = Progbar(epochs)
-        for epoch in range(epochs):
-            progbar.update(epoch)
-            model.predict(x=x, steps=steps, batch_size=batch_size, verbose=0)
-        progbar.update(epochs, finalize=epochs)
-
-
 def evaluate_model(model,
                    x,
                    y=None,
                    batch_size=None,
                    steps=None,
                    print_history=False):
     """ Evaluates model performances.
@@ -152,15 +126,21 @@
     if isinstance(x, DirectoryIterator):
         steps = np.math.ceil(x.samples / x.batch_size)
 
     for batch, label_batch in x:
         if not isinstance(batch, np.ndarray):
             batch = batch.numpy()
 
-        pots_batch = model.predict(batch.astype('uint8'))
+        # Retrieve input_signed value: cannot use getattr here because LayerParams does not
+        # implement a default value.
+        input_signed = 'input_signed' in dir(model.get_layer(0).parameters)
+        if input_signed:
+            input_signed = model.get_layer(0).parameters.input_signed
+        type = 'int8' if input_signed else 'uint8'
+        pots_batch = model.predict(batch.astype(type))
 
         if labels is None:
             labels = label_batch
             pots = pots_batch.squeeze(axis=(1, 2))
         else:
             labels = np.concatenate((labels, label_batch))
             pots = np.concatenate((pots, pots_batch.squeeze(axis=(1, 2))))
@@ -170,44 +150,42 @@
         if steps is not None and x.total_batches_seen == steps:
             break
 
     return Activation(activation)(pots), labels
 
 
 def get_training_parser(batch_size,
-                        calibrate=False,
+                        extract=False,
                         tune=False,
                         freeze_before=False,
                         global_batch_size=True,
                         global_parser=None):
     """ Instantiates a base arguments parser for training scripts.
 
     The returned parser comes with train, tune and eval actions as subparsers
     (with default parameters) for which one can add arguments if required.
 
     Args:
         batch_size (int): batch size default value
-        calibrate (bool, optional): either to add a calibrate action or not. Defaults to
+        extract (bool, optional): either to add an extract action or not. Defaults to
             False.
         tune (bool, optional): either to add a tune action or not. Defaults to
             False.
         freeze_before (bool, optional): either to add a "--freeze_before"
             parameter in train and tune actions or not. Defaults to False.
         global_batch_size (bool, optional): either to add batch size as a
             global parser parameter or for train/tune actions only. Defaults to
             True.
         global_parser (argparse.ArgumentParser, optional): global parser with
             custom parameters. Defaults to None.
 
     Returns:
-        argparse.ArgumentParser, argparse.ArgumentParser,
-        argparse.ArgumentParser, argparse.ArgumentParser,
-        argparse.ArgumentParser,
-        argparse._SubParsersAction: main parser and train, calibrate, tune and eval actions
-            subparsers and the subparser object.
+        argparse.ArgumentParser, argparse.ArgumentParser, argparse.ArgumentParser,
+        argparse.ArgumentParser, argparse.ArgumentParser, argparse._SubParsersAction: main parser
+        and train, tune, eval, and extract actions subparsers and the subparser object.
     """
 
     # Define a strictly positive int type for parameters
     def positive_int(value):
         ivalue = int(value)
         if ivalue <= 0:
             raise argparse.ArgumentTypeError(
@@ -272,35 +250,38 @@
     tune_parser = None
     if tune:
         tune_parser = subparsers.add_parser("tune",
                                             parents=[parent_parser],
                                             help="Tune a Keras model")
 
     # Other subparsers
-    calibrate_parser = None
-    if calibrate:
-        calibrate_parser = subparsers.add_parser("calibrate",
-                                                 parents=[parent_parser],
-                                                 help="Calibrate a Keras model")
-        calibrate_parser.add_argument("-ns",
-                                      "--num_samples",
-                                      type=positive_int,
-                                      default=1024,
-                                      help="Number of samples to use for calibration")
+    extract_parser = None
+    if extract:
+        extract_parser = subparsers.add_parser("extract",
+                                               parents=[global_parser],
+                                               help="Extract samples from the dataset")
+        if not global_batch_size:
+            extract_parser.add_argument("-b",
+                                        "--batch_size",
+                                        type=positive_int,
+                                        default=batch_size,
+                                        help="The batch size")
+        extract_parser.add_argument("-s", "--savefile", type=str,
+                                    default='samples.npz', help="Samples filename.")
 
     eval_parser = subparsers.add_parser("eval",
                                         help="Evaluate a model",
                                         parents=[global_parser])
 
     eval_parser.add_argument("-ak",
                              "--akida",
                              action='store_true',
                              help="Converts to an Akida model and evaluate")
 
-    return parser, train_parser, tune_parser, eval_parser, calibrate_parser, subparsers
+    return parser, train_parser, tune_parser, eval_parser, extract_parser, subparsers
 
 
 def print_history_stats(history):
     """Prints a basic statistics of the training/eval history.
 
     Args:
         history (keras.callbacks.History): history of the training/eval process
@@ -341,7 +322,25 @@
                          mode=mode)
 
     def on_train_end(self, logs=None):
         if os.path.exists(self.filepath):
             self.model.load_weights(self.filepath)
         # Clean temp directory
         self.temp_dir.cleanup()
+
+
+def save_model(model, model_path, save_path=None, action_str='saved'):
+    """ Saves the model with the given or a default name.
+
+    Args:
+        model (keras.Model): the model to save
+        model_path (str): the original model path
+        save_path (str): the path to save the model. Defaults to None.
+        action_str (str): the 'action' used in the training script, will be appended to the original
+            model path when save_path is None. Defaults to 'saved'.
+    """
+    if not save_path:
+        save_path = os.path.splitext(model_path)[0]
+        save_path += f"_{action_str}.h5"
+
+    model.save(save_path, include_optimizer=False)
+    print(f"Model saved as {save_path}.")
```

### Comparing `akida_models-1.1.9/akida_models/transformers/model_deit.py` & `akida_models-1.2.0/akida_models/transformers/model_deit.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 from quantizeml.layers import AddPositionEmbs, ClassToken, Add, ExtractToken
 from quantizeml.models import load_model
 
 from .model_vit import CONFIG_TI, CONFIG_S, CONFIG_B
 from ..imagenet.imagenet_utils import IMAGENET_MEAN, IMAGENET_STD
 from ..layer_blocks import norm_to_layer, transformer_block
 from ..utils import fetch_file
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/deit/'
+from ..model_io import get_model_path
 
 
 def deit_imagenet(input_shape,
                   num_blocks,
                   hidden_size,
                   num_heads,
                   name,
@@ -209,20 +208,21 @@
     )
 
 
 def bc_deit_dist_ti16_imagenet_pretrained():
     """ Helper method to retrieve a `bc_deit_dist_ti16` model that was trained on ImageNet dataset.
 
     Returns:
-        keras.Model, dict: a Keras Model instance and the quantization configuration as a JSON
-        formatted dict.
+        keras.Model: a Keras Model instance
     """
-    model_name = 'bc_deit_dist_ti16_224_quant_config_4bit.h5'
-    file_hash = '0d8b1c46e215be149974e6116e2e88a50a9c6d2186f7131f4fb0b3f23aaa2aac'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v2 = 'bc_deit_dist_ti16_224_i8_w8_a8.h5'
+    file_hash_v2 = '4e40e36beb56a926b18cab4c5880aa3cbe768e0e40c9c91abca6063a72763044'
+    model_path, model_name, file_hash = get_model_path("deit", model_name_v2=model_name_v2,
+                                                       file_hash_v2=file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
     return load_model(model_path)
 
 
 def deit_s16(input_shape=(224, 224, 3), classes=1000, distilled=False, include_top=True):
```

### Comparing `akida_models-1.1.9/akida_models/transformers/model_vit.py` & `akida_models-1.2.0/akida_models/transformers/model_vit.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 import typing_extensions as tx
 
 from quantizeml.layers import AddPositionEmbs, ClassToken, ExtractToken
 from quantizeml.models import load_model
 
 from ..layer_blocks import transformer_block, norm_to_layer
 from ..utils import fetch_file
-
-BASE_WEIGHT_PATH = 'http://data.brainchip.com/models/vit/'
+from ..model_io import get_model_path
 
 
 ConfigDict = tx.TypedDict(
     "ConfigDict",
     {
         "dropout": float,
         "mlp_dim": int,
@@ -270,20 +269,21 @@
     )
 
 
 def bc_vit_ti16_imagenet_pretrained():
     """ Helper method to retrieve a `bc_vit_ti16` model that was trained on ImageNet dataset.
 
     Returns:
-        keras.Model, dict: a Keras Model instance and the quantization configuration as a JSON
-        formatted dict.
+        keras.Model: a Keras Model instance
     """
-    model_name = 'bc_vit_ti16_224_quant_config_4bit.h5'
-    file_hash = '8c3623e293e91f19c332eefaa54fb77b88118a3868eeb50e870e51b89857ceb1'
-    model_path = fetch_file(BASE_WEIGHT_PATH + model_name,
+    model_name_v2 = 'bc_vit_ti16_224_i8_w8_a8.h5'
+    file_hash_v2 = '15ee27991b18f3cb7f38a1ea8e0ed10168b7ca7924baba4fe08593a8caf29a35'
+    model_path, model_name, file_hash = get_model_path("vit", model_name_v2=model_name_v2,
+                                                       file_hash_v2=file_hash_v2)
+    model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
     return load_model(model_path)
 
 
 def vit_s16(input_shape=(224, 224, 3), classes=1000, include_top=True):
```

### Comparing `akida_models-1.1.9/akida_models/utils.py` & `akida_models-1.2.0/akida_models/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 from six.moves.urllib.parse import urlsplit
 
 import tensorflow as tf
 from keras.utils import io_utils
 from keras.utils.data_utils import validate_file, _extract_archive
 from keras.utils.generic_utils import Progbar
 from keras.callbacks import TensorBoard
-
-from cnn2snn import load_quantized_model
-from quantizeml.models import load_model as qml_load_model
+from cnn2snn import get_akida_version, AkidaVersion
 
 
 def fetch_file(origin, fname=None, file_hash=None, cache_subdir="datasets", extract=False,
                cache_dir=None):
     """ Downloads a file from a URL if it is not already in the cache.
 
     Reimplements `keras.utils.get_file` without raising an error when detecting a file_hash
@@ -125,33 +123,14 @@
 
     if extract:
         _extract_archive(fpath, datadir)
 
     return fpath
 
 
-def load_model(model_path):
-    """Combine the cnn2snn.load_quantized_model and quantizeml.load_model
-
-    Args:
-        model_path (str): model path
-
-    Returns:
-        keras.Model: the load model
-    """
-    try:
-        model = load_quantized_model(model_path)
-    except Exception:
-        try:
-            model = qml_load_model(model_path)
-        except Exception as e:
-            raise e.__class__('Cannot load provided model.')
-    return model
-
-
 def get_tensorboard_callback(out_dir, histogram_freq=1, prefix=''):
     """Build a Tensorboard call, pointing to the output directory
 
     Args:
         out_dir (str): parent directory of the folder to create
         histogram_freq (int, optional): frequency to export logs. Defaults to 1.
         prefix (str, optional): prefix name. Defaults to ''.
@@ -174,7 +153,26 @@
     file_writer = tf.summary.create_file_writer(log_dir + "/metrics")
     file_writer.set_as_default()
     return TensorBoard(log_dir=log_dir,
                        histogram_freq=histogram_freq,
                        update_freq='epoch',
                        write_graph=False,
                        profile_batch=0)
+
+
+def get_params_by_version(relu_v2='ReLU3.75'):
+    """Provides the layer parameters depending on Akida version
+
+    With Akida v1, sepconv are fused, the ReLU max value is 6.
+    With Akida v2, sepconv are unfused, the ReLU max value is "relu_v2" and the ReLU is at the end
+    of the block with GAP.
+
+    Args:
+        relu_v2 (str, optional): ReLUx string when targetting V2. Defaults to ReLU3.75.
+    Returns:
+        bool, bool, str: fused, post_relu_gap, relu_activation
+    """
+    # Model version management
+    if get_akida_version() == AkidaVersion.v1:
+        return True, False, 'ReLU6'
+    # Akida v2
+    return False, True, relu_v2
```

### Comparing `akida_models-1.1.9/akida_models/utk_face/preprocessing.py` & `akida_models-1.2.0/akida_models/utk_face/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     Returns:
         np.array, np.array, np.array, np.array: train set, train labels, test
         set and test labels as numpy arrays
 
     """
     dataset = fetch_file(
-        "http://data.brainchip.com/dataset-mirror/utk_face/UTKFace_preprocessed.tar.gz",
+        "https://data.brainchip.com/dataset-mirror/utk_face/UTKFace_preprocessed.tar.gz",
         fname="UTKFace_preprocessed.tar.gz",
         cache_subdir='datasets/',
         extract=True)
     file_path = os.path.join(os.path.dirname(dataset), "UTKFace")
 
     train_path = os.path.join(file_path, "train")
     test_path = os.path.join(file_path, "test")
```

### Comparing `akida_models-1.1.9/akida_models/utk_face/utk_face_train.py` & `akida_models-1.2.0/akida_models/utk_face/utk_face_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
 Training script for UTKFace model.
 """
+import os
 import numpy as np
 
 from keras.callbacks import LearningRateScheduler
 
-from cnn2snn import load_quantized_model, convert
+from cnn2snn import convert
 
-from ..training import get_training_parser, compile_model, evaluate_model, print_history_stats
+from ..training import (get_training_parser, compile_model, evaluate_model, print_history_stats,
+                        save_model)
+from ..extract import extract_samples
+from ..model_io import load_model
 from .preprocessing import load_data
 
 
 def get_data():
     """ Loads UTKFace data.
 
     Returns:
-        np.array, np.array, np.array, np.array:  train set, train labels, test
+        np.array, np.array, np.array, np.array: train set, train labels, test
             set and test labels
     """
     # Load the dataset
     x_train, y_train, x_test, y_test = load_data()
 
     return x_train.astype('float32'), y_train, x_test.astype('float32'), y_test
 
@@ -45,15 +49,15 @@
 
     Args:
         model (keras.Model): the model to train
         x_train (numpy.ndarray): train data
         y_train (numpy.ndarray): train labels
         x_test (numpy.ndarray): test data
         y_test (numpy.ndarray): test labels
-        epochs (int):  the number of epochs
+        epochs (int): the number of epochs
         batch_size (int): the batch size
     """
     # Learning rate: be more aggressive at the beginning, and apply decay
     lr_start = 1e-3
     lr_end = 1e-4
     lr_decay = (lr_end / lr_start)**(1. / epochs)
 
@@ -69,42 +73,42 @@
                         callbacks=callbacks)
     print_history_stats(history)
 
 
 def main():
     """ Entry point for script and CLI usage.
     """
-    parser = get_training_parser(batch_size=128, global_batch_size=False)[0]
+    parser = get_training_parser(batch_size=128, global_batch_size=False, extract=True)[0]
     args = parser.parse_args()
 
     # Load the source model
-    model = load_quantized_model(args.model)
+    model = load_model(args.model)
 
     # Compile model
-    compile_model(model, loss='mae', metrics=None)
+    compile_model(model, loss='mae', metrics=['mae'])
 
     # Load data
     x_train, y_train, x_test, y_test = get_data()
 
+    # Disable quantizeML assertions
+    os.environ["ASSERT_ENABLED"] = "0"
+
     # Train model
     if args.action == "train":
-        train_model(model, x_train, y_train, x_test, y_test, args.epochs,
-                    args.batch_size)
-
-        # Save model in Keras format (h5)
-        if args.savemodel:
-            model.save(args.savemodel, include_optimizer=False)
-            print(f"Trained model saved as {args.savemodel}")
-
+        train_model(model, x_train, y_train, x_test, y_test, args.epochs, args.batch_size)
+        save_model(model, args.model, args.savemodel, args.action)
     elif args.action == "eval":
         # Evaluate model accuracy
         if args.akida:
             model_ak = convert(model)
             y = model_ak.predict(x_test.astype(np.uint8))
             mae = np.sum(np.abs(y_test.squeeze() - y.squeeze())) / len(y_test)
             print("Validation accuracy: {0:.4f}".format(mae))
         else:
             evaluate_model(model, x_test, y=y_test, print_history=True)
+    elif args.action == 'extract':
+        # Extract samples from dataset
+        extract_samples(args.savefile, x_train, args.batch_size)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akida_models-1.1.9/akida_models.egg-info/SOURCES.txt` & `akida_models-1.2.0/akida_models.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 LICENSE.3rdparty
 MANIFEST.in
 README
 setup.py
 akida_models/__init__.py
-akida_models/calibrable.py
 akida_models/cli.py
 akida_models/cyclic_lr.py
 akida_models/distiller.py
-akida_models/filter_pruning.py
+akida_models/extract.py
 akida_models/gamma_constraint.py
 akida_models/layer_blocks.py
 akida_models/macs.py
+akida_models/model_io.py
 akida_models/param_scheduler.py
-akida_models/renaming.py
 akida_models/training.py
+akida_models/unfuse_sepconv_layers.py
 akida_models/utils.py
 akida_models.egg-info/PKG-INFO
 akida_models.egg-info/SOURCES.txt
 akida_models.egg-info/dependency_links.txt
 akida_models.egg-info/entry_points.txt
 akida_models.egg-info/requires.txt
 akida_models.egg-info/top_level.txt
@@ -26,19 +26,14 @@
 akida_models/casia_webface/preprocessing.py
 akida_models/centernet/__init__.py
 akida_models/centernet/centernet_batch_generator.py
 akida_models/centernet/centernet_loss.py
 akida_models/centernet/centernet_processing.py
 akida_models/centernet/centernet_train.py
 akida_models/centernet/model_centernet.py
-akida_models/cifar10/__init__.py
-akida_models/cifar10/preprocessing.py
-akida_models/cwru/__init__.py
-akida_models/cwru/cwru_train.py
-akida_models/cwru/model_convtiny.py
 akida_models/detection/__init__.py
 akida_models/detection/batch_generator.py
 akida_models/detection/box_utils.py
 akida_models/detection/generate_anchors.py
 akida_models/detection/map_evaluation.py
 akida_models/detection/model_yolo.py
 akida_models/detection/processing.py
@@ -54,16 +49,14 @@
 akida_models/imagenet/imagenet_labels2names.py
 akida_models/imagenet/imagenet_train.py
 akida_models/imagenet/imagenet_utils.py
 akida_models/imagenet/model_akidanet.py
 akida_models/imagenet/model_akidanet18.py
 akida_models/imagenet/model_akidanet_edge.py
 akida_models/imagenet/model_mobilenet.py
-akida_models/imagenet/model_mobilenet_edge.py
-akida_models/imagenet/model_vgg.py
 akida_models/imagenet/preprocessing.py
 akida_models/kws/__init__.py
 akida_models/kws/kws_train.py
 akida_models/kws/model_ds_cnn.py
 akida_models/kws/preprocessing.py
 akida_models/mnist/__init__.py
 akida_models/mnist/mnist_train.py
```

### Comparing `akida_models-1.1.9/akida_models.egg-info/entry_points.txt` & `akida_models-1.2.0/akida_models.egg-info/entry_points.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [console_scripts]
 akida_models = akida_models.cli:main
 centernet_train = akida_models.centernet.centernet_train:main
-cwru_train = akida_models.cwru.cwru_train:main
 dvs_train = akida_models.dvs.dvs_train:main
 imagenet_train = akida_models.imagenet.imagenet_train:main
 kws_train = akida_models.kws.kws_train:main
 mnist_train = akida_models.mnist.mnist_train:main
 modelnet40_train = akida_models.modelnet40.modelnet40_train:main
 portrait128_train = akida_models.portrait128.portrait128_train:main
 utk_face_train = akida_models.utk_face.utk_face_train:main
```

### Comparing `akida_models-1.1.9/setup.py` & `akida_models-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='akida_models',
-      version='1.1.9',
+      version='1.2.0',
       description='Akida Models',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      author='David Corvoysier',
-      author_email='dcorvoysier@brainchip.com',
+      author='Kevin Tsiknos',
+      author_email='ktsiknos@brainchip.com',
       url='https://doc.brainchipinc.com',
       license='Apache 2.0',
       license_files=['LICENSE', 'LICENSE.3rdparty'],
       packages=find_packages(),
       entry_points={
         'console_scripts': [
             'akida_models = akida_models.cli:main',
             'utk_face_train = akida_models.utk_face.utk_face_train:main',
             'kws_train = akida_models.kws.kws_train:main',
             'modelnet40_train = akida_models.modelnet40.modelnet40_train:main',
             'yolo_train = akida_models.detection.yolo_train:main',
             'dvs_train = akida_models.dvs.dvs_train:main',
-            'cwru_train = akida_models.cwru.cwru_train:main',
             'mnist_train = akida_models.mnist.mnist_train:main',
             'imagenet_train = akida_models.imagenet.imagenet_train:main',
             'portrait128_train = akida_models.portrait128.portrait128_train:main',
             'centernet_train = akida_models.centernet.centernet_train:main'
         ]
       },
-      install_requires=['cnn2snn~=2.3.0', 'quantizeml~=0.3.1', 'scipy', 'opencv-python', 'mtcnn',
+      install_requires=['cnn2snn~=2.4.0', 'quantizeml~=0.5.2', 'scipy', 'opencv-python', 'mtcnn',
         'imgaug', 'trimesh', 'tensorflow-addons>=0.18.0'],
       python_requires='>=3.7')
```

